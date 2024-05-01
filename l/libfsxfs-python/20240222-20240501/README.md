# Comparing `tmp/libfsxfs-python-20240222.tar.gz` & `tmp/libfsxfs-python-20240501.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libfsxfs-python-20240222.tar", last modified: Thu Feb 22 19:02:30 2024, max compression
+gzip compressed data, was "libfsxfs-python-20240501.tar", last modified: Wed May  1 17:05:56 2024, max compression
```

## Comparing `libfsxfs-python-20240222.tar` & `libfsxfs-python-20240501.tar`

### file list

```diff
@@ -1,924 +1,924 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:28.000000 libfsxfs-20240222/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_area.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_mapped_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1291 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_area.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_mapped_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_segments_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_segments_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33624 2024-02-22 06:58:59.000000 libfsxfs-20240222/libfdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-02-22 06:58:40.000000 libfsxfs-20240222/libfdata/libfdata_vector.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/fsxfstools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1781 2024-02-22 06:45:17.000000 libfsxfs-20240222/fsxfstools/fsxfstools_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-02-22 06:45:17.000000 libfsxfs-20240222/fsxfstools/fsxfstools_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36321 2024-02-22 06:46:25.000000 libfsxfs-20240222/fsxfstools/mount_dokan.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3061 2024-02-22 06:46:25.000000 libfsxfs-20240222/fsxfstools/mount_file_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1486 2024-02-22 06:45:17.000000 libfsxfs-20240222/fsxfstools/fsxfstools_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4145 2024-02-22 06:45:17.000000 libfsxfs-20240222/fsxfstools/fsxfstools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37913 2024-02-22 06:46:25.000000 libfsxfs-20240222/fsxfstools/mount_fuse.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1472 2024-02-22 06:45:17.000000 libfsxfs-20240222/fsxfstools/fsxfstools_output.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4426 2024-02-22 06:46:25.000000 libfsxfs-20240222/fsxfstools/info_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5417 2024-02-22 06:45:17.000000 libfsxfs-20240222/fsxfstools/mount_dokan.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1771 2024-02-22 06:45:17.000000 libfsxfs-20240222/fsxfstools/fsxfstools_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3297 2024-02-22 06:45:17.000000 libfsxfs-20240222/fsxfstools/digest_hash.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30757 2024-02-22 06:46:25.000000 libfsxfs-20240222/fsxfstools/mount_file_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1409 2024-02-22 06:45:17.000000 libfsxfs-20240222/fsxfstools/fsxfstools_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-22 06:45:17.000000 libfsxfs-20240222/fsxfstools/fsxfstools_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2516 2023-12-03 09:07:58.000000 libfsxfs-20240222/fsxfstools/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-02-22 06:45:17.000000 libfsxfs-20240222/fsxfstools/fsxfstools_libfsxfs.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10866 2024-02-22 06:46:25.000000 libfsxfs-20240222/fsxfstools/fsxfsinfo.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22158 2024-02-22 06:46:25.000000 libfsxfs-20240222/fsxfstools/mount_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    63194 2024-02-22 06:46:25.000000 libfsxfs-20240222/fsxfstools/info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3661 2024-02-22 06:46:25.000000 libfsxfs-20240222/fsxfstools/mount_file_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1761 2024-02-22 06:45:17.000000 libfsxfs-20240222/fsxfstools/fsxfstools_signal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1474 2024-02-22 06:45:17.000000 libfsxfs-20240222/fsxfstools/fsxfstools_libhmac.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1213 2024-02-22 06:45:17.000000 libfsxfs-20240222/fsxfstools/fsxfstools_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-02-22 06:45:17.000000 libfsxfs-20240222/fsxfstools/fsxfstools_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-02-22 06:45:17.000000 libfsxfs-20240222/fsxfstools/fsxfstools_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3324 2024-02-22 06:46:25.000000 libfsxfs-20240222/fsxfstools/mount_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1483 2024-02-22 06:45:17.000000 libfsxfs-20240222/fsxfstools/fsxfstools_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-02-22 06:45:17.000000 libfsxfs-20240222/fsxfstools/fsxfstools_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5751 2024-02-22 06:45:17.000000 libfsxfs-20240222/fsxfstools/fsxfstools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19354 2024-02-22 06:46:25.000000 libfsxfs-20240222/fsxfstools/mount_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15469 2024-02-22 06:46:25.000000 libfsxfs-20240222/fsxfstools/fsxfsmount.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34940 2024-02-22 06:58:59.000000 libfsxfs-20240222/fsxfstools/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-02-22 06:45:17.000000 libfsxfs-20240222/fsxfstools/fsxfstools_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1244 2024-02-22 06:45:17.000000 libfsxfs-20240222/fsxfstools/digest_hash.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3050 2024-02-22 06:46:25.000000 libfsxfs-20240222/fsxfstools/mount_fuse.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1590 2024-02-22 06:45:17.000000 libfsxfs-20240222/fsxfstools/fsxfstools_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-02-22 06:45:15.000000 libfsxfs-20240222/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-02-22 06:58:59.000000 libfsxfs-20240222/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 06:45:15.000000 libfsxfs-20240222/NEWS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-02-22 06:58:59.000000 libfsxfs-20240222/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:28.000000 libfsxfs-20240222/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-22 06:58:42.000000 libfsxfs-20240222/libfguid/libfguid_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-02-22 06:58:42.000000 libfsxfs-20240222/libfguid/libfguid_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-02-22 06:58:42.000000 libfsxfs-20240222/libfguid/libfguid_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-22 06:58:42.000000 libfsxfs-20240222/libfguid/libfguid_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      681 2024-02-22 06:58:42.000000 libfsxfs-20240222/libfguid/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-22 06:58:42.000000 libfsxfs-20240222/libfguid/libfguid_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-22 06:58:42.000000 libfsxfs-20240222/libfguid/libfguid_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-02-22 06:58:42.000000 libfsxfs-20240222/libfguid/libfguid_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-02-22 06:58:42.000000 libfsxfs-20240222/libfguid/libfguid_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-02-22 06:58:42.000000 libfsxfs-20240222/libfguid/libfguid_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-02-22 06:58:42.000000 libfsxfs-20240222/libfguid/libfguid_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29839 2024-02-22 06:58:59.000000 libfsxfs-20240222/libfguid/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-22 06:58:42.000000 libfsxfs-20240222/libfguid/libfguid_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3453 2024-02-22 06:45:15.000000 libfsxfs-20240222/libfsxfs.spec.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:27.000000 libfsxfs-20240222/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2023-12-03 09:07:57.000000 libfsxfs-20240222/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18233 2023-12-03 09:07:58.000000 libfsxfs-20240222/m4/libfdatetime.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:07:57.000000 libfsxfs-20240222/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2023-12-03 09:07:57.000000 libfsxfs-20240222/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:07:58.000000 libfsxfs-20240222/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:07:57.000000 libfsxfs-20240222/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31269 2023-12-03 09:07:57.000000 libfsxfs-20240222/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:07:57.000000 libfsxfs-20240222/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:07:58.000000 libfsxfs-20240222/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2023-12-03 09:07:57.000000 libfsxfs-20240222/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-12-03 09:07:57.000000 libfsxfs-20240222/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2023-12-03 09:07:57.000000 libfsxfs-20240222/m4/libcsplit.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 09:07:57.000000 libfsxfs-20240222/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-12-03 09:07:57.000000 libfsxfs-20240222/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-02-22 06:58:52.000000 libfsxfs-20240222/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-02-22 06:58:52.000000 libfsxfs-20240222/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15545 2023-12-03 09:07:57.000000 libfsxfs-20240222/m4/libfdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:07:58.000000 libfsxfs-20240222/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5232 2023-12-03 09:07:58.000000 libfsxfs-20240222/m4/libfuse.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-02-22 06:58:52.000000 libfsxfs-20240222/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:07:57.000000 libfsxfs-20240222/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 09:07:57.000000 libfsxfs-20240222/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-12-03 09:07:57.000000 libfsxfs-20240222/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2023-12-03 09:07:58.000000 libfsxfs-20240222/m4/libfguid.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2023-12-03 09:07:57.000000 libfsxfs-20240222/m4/libbfio.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8319 2023-12-03 09:07:58.000000 libfsxfs-20240222/m4/libhmac.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:07:57.000000 libfsxfs-20240222/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-02-22 06:58:52.000000 libfsxfs-20240222/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:07:58.000000 libfsxfs-20240222/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:07:58.000000 libfsxfs-20240222/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-02-22 06:58:52.000000 libfsxfs-20240222/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:07:57.000000 libfsxfs-20240222/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:07:58.000000 libfsxfs-20240222/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27481 2023-12-03 09:07:57.000000 libfsxfs-20240222/m4/libcrypto.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:07:58.000000 libfsxfs-20240222/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7325 2023-12-03 09:07:57.000000 libfsxfs-20240222/m4/libfcache.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-12-03 09:07:57.000000 libfsxfs-20240222/m4/pthread.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:27.000000 libfsxfs-20240222/include/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      474 2024-02-22 06:45:15.000000 libfsxfs-20240222/include/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:27.000000 libfsxfs-20240222/include/libfsxfs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2221 2024-02-22 06:45:16.000000 libfsxfs-20240222/include/libfsxfs/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2219 2024-02-22 06:59:10.000000 libfsxfs-20240222/include/libfsxfs/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5032 2024-02-22 06:45:16.000000 libfsxfs-20240222/include/libfsxfs/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4901 2024-02-22 06:59:10.000000 libfsxfs-20240222/include/libfsxfs/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-02-22 06:45:16.000000 libfsxfs-20240222/include/libfsxfs/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2024-02-22 06:45:16.000000 libfsxfs-20240222/include/libfsxfs/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-22 06:45:16.000000 libfsxfs-20240222/include/libfsxfs/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1487 2024-02-22 06:59:10.000000 libfsxfs-20240222/include/libfsxfs/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5306 2024-02-22 06:45:16.000000 libfsxfs-20240222/include/libfsxfs/codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28385 2024-02-22 06:58:59.000000 libfsxfs-20240222/include/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26614 2024-02-22 06:45:16.000000 libfsxfs-20240222/include/libfsxfs.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26614 2024-02-22 06:59:10.000000 libfsxfs-20240222/include/libfsxfs.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:27.000000 libfsxfs-20240222/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-02-22 06:45:16.000000 libfsxfs-20240222/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-02-22 06:45:16.000000 libfsxfs-20240222/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-02-22 06:45:16.000000 libfsxfs-20240222/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-02-22 06:45:16.000000 libfsxfs-20240222/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-02-22 06:45:16.000000 libfsxfs-20240222/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-02-22 06:45:16.000000 libfsxfs-20240222/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-02-22 06:45:16.000000 libfsxfs-20240222/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-02-22 06:45:15.000000 libfsxfs-20240222/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-02-22 06:45:16.000000 libfsxfs-20240222/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7374 2024-02-22 06:59:11.000000 libfsxfs-20240222/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17849 2024-02-22 06:58:58.000000 libfsxfs-20240222/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18894 2024-02-22 06:59:11.000000 libfsxfs-20240222/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-02-22 06:45:16.000000 libfsxfs-20240222/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-02-22 06:45:16.000000 libfsxfs-20240222/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-02-22 06:45:16.000000 libfsxfs-20240222/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25392 2024-02-22 06:58:59.000000 libfsxfs-20240222/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:28.000000 libfsxfs-20240222/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-02-22 06:58:31.000000 libfsxfs-20240222/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-02-22 06:58:31.000000 libfsxfs-20240222/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2024-02-22 06:58:31.000000 libfsxfs-20240222/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-02-22 06:58:31.000000 libfsxfs-20240222/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-22 06:58:31.000000 libfsxfs-20240222/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-02-22 06:58:31.000000 libfsxfs-20240222/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-02-22 06:58:31.000000 libfsxfs-20240222/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-02-22 06:58:31.000000 libfsxfs-20240222/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-02-22 06:58:31.000000 libfsxfs-20240222/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-02-22 06:58:31.000000 libfsxfs-20240222/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30395 2024-02-22 06:58:59.000000 libfsxfs-20240222/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-22 06:58:31.000000 libfsxfs-20240222/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-02-22 06:58:31.000000 libfsxfs-20240222/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-02-22 06:58:31.000000 libfsxfs-20240222/libclocale/libclocale_codepage.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:28.000000 libfsxfs-20240222/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-02-22 06:58:38.000000 libfsxfs-20240222/libfcache/libfcache_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-02-22 06:58:38.000000 libfsxfs-20240222/libfcache/libfcache_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-02-22 06:58:38.000000 libfsxfs-20240222/libfcache/libfcache_cache_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-22 06:58:38.000000 libfsxfs-20240222/libfcache/libfcache_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-02-22 06:58:38.000000 libfsxfs-20240222/libfcache/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-22 06:58:38.000000 libfsxfs-20240222/libfcache/libfcache_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-22 06:58:38.000000 libfsxfs-20240222/libfcache/libfcache_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-02-22 06:58:38.000000 libfsxfs-20240222/libfcache/libfcache_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-02-22 06:58:38.000000 libfsxfs-20240222/libfcache/libfcache_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-22 06:58:38.000000 libfsxfs-20240222/libfcache/libfcache_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-22 06:58:38.000000 libfsxfs-20240222/libfcache/libfcache_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-02-22 06:58:38.000000 libfsxfs-20240222/libfcache/libfcache_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-22 06:58:38.000000 libfsxfs-20240222/libfcache/libfcache_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-02-22 06:58:38.000000 libfsxfs-20240222/libfcache/libfcache_cache_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30868 2024-02-22 06:58:59.000000 libfsxfs-20240222/libfcache/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-02-22 06:58:38.000000 libfsxfs-20240222/libfcache/libfcache_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-02-22 06:58:38.000000 libfsxfs-20240222/libfcache/libfcache_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-02-22 06:58:38.000000 libfsxfs-20240222/libfcache/libfcache_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2303 2023-12-03 09:07:43.000000 libfsxfs-20240222/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:28.000000 libfsxfs-20240222/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_file_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_file_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_file_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_file_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_file_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_file_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_memory_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_file_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_file_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_memory_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_memory_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33854 2024-02-22 06:58:59.000000 libfsxfs-20240222/libbfio/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_memory_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-02-22 06:58:25.000000 libfsxfs-20240222/libbfio/libbfio_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:07:42.000000 libfsxfs-20240222/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-02-22 06:58:59.000000 libfsxfs-20240222/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:27.000000 libfsxfs-20240222/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-02-22 06:45:15.000000 libfsxfs-20240222/dpkg/libfsxfs-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1026 2024-02-22 06:45:18.000000 libfsxfs-20240222/dpkg/copyright
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:27.000000 libfsxfs-20240222/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-02-22 06:45:15.000000 libfsxfs-20240222/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-02-22 06:45:15.000000 libfsxfs-20240222/dpkg/libfsxfs-tools.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2119 2024-02-22 06:45:15.000000 libfsxfs-20240222/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      769 2024-02-22 06:45:15.000000 libfsxfs-20240222/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-02-22 06:45:15.000000 libfsxfs-20240222/dpkg/libfsxfs-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      121 2024-02-22 06:45:15.000000 libfsxfs-20240222/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2024-02-22 06:59:11.000000 libfsxfs-20240222/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-02-22 06:45:15.000000 libfsxfs-20240222/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-02-22 06:45:15.000000 libfsxfs-20240222/dpkg/libfsxfs.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      486 2024-02-22 06:59:11.000000 libfsxfs-20240222/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-02-22 06:45:15.000000 libfsxfs-20240222/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1983258 2024-02-22 06:58:57.000000 libfsxfs-20240222/configure
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2408 2024-02-22 06:59:11.000000 libfsxfs-20240222/libfsxfs.spec
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-02-22 06:58:59.000000 libfsxfs-20240222/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-02-22 06:58:59.000000 libfsxfs-20240222/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-02-22 06:45:42.000000 libfsxfs-20240222/msvscpp/libfdata/libfdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/fsxfsinfo/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7194 2024-02-22 06:45:42.000000 libfsxfs-20240222/msvscpp/fsxfsinfo/fsxfsinfo.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/fsxfs_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5645 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/fsxfs_test_error/fsxfs_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/fsxfs_test_tools_info_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6164 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/fsxfs_test_tools_info_handle/fsxfs_test_tools_info_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/fsxfs_test_extent/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5894 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/fsxfs_test_extent/fsxfs_test_extent.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40758 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/libfsxfs.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/fsxfs_test_file_system_block_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5948 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/fsxfs_test_file_system_block_header/fsxfs_test_file_system_block_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/fsxfsmount/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7669 2024-02-22 06:45:42.000000 libfsxfs-20240222/msvscpp/fsxfsmount/fsxfsmount.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-02-22 06:45:42.000000 libfsxfs-20240222/msvscpp/libfguid/libfguid.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/fsxfs_test_inode_btree_record/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5930 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/fsxfs_test_inode_btree_record/fsxfs_test_inode_btree_record.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/fsxfs_test_directory_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5921 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/fsxfs_test_directory_entry/fsxfs_test_directory_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/fsxfs_test_directory_table_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5942 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/fsxfs_test_directory_table_header/fsxfs_test_directory_table_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-02-22 06:45:42.000000 libfsxfs-20240222/msvscpp/libclocale/libclocale.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/fsxfs_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6560 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/fsxfs_test_support/fsxfs_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-02-22 06:45:42.000000 libfsxfs-20240222/msvscpp/libfcache/libfcache.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2277 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-02-22 06:45:42.000000 libfsxfs-20240222/msvscpp/libbfio/libbfio.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/fsxfs_test_block_directory_footer/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5942 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/fsxfs_test_block_directory_footer/fsxfs_test_block_directory_footer.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/fsxfs_test_io_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5903 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/fsxfs_test_io_handle/fsxfs_test_io_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/pyfsxfs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6839 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/pyfsxfs/pyfsxfs.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-02-22 06:45:42.000000 libfsxfs-20240222/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/fsxfs_test_block_directory_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5942 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/fsxfs_test_block_directory_header/fsxfs_test_block_directory_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/fsxfs_test_attributes_table/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6007 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/fsxfs_test_attributes_table/fsxfs_test_attributes_table.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-02-22 06:45:42.000000 libfsxfs-20240222/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/fsxfs_test_inode_information/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/fsxfs_test_inode_information/fsxfs_test_inode_information.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/fsxfs_test_superblock/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6156 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/fsxfs_test_superblock/fsxfs_test_superblock.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/fsxfs_test_buffer_data_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5930 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/fsxfs_test_buffer_data_handle/fsxfs_test_buffer_data_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/fsxfs_test_btree_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5912 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/fsxfs_test_btree_header/fsxfs_test_btree_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/libfsxfs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13845 2024-02-22 06:45:42.000000 libfsxfs-20240222/msvscpp/libfsxfs/libfsxfs.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-02-22 06:45:42.000000 libfsxfs-20240222/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/fsxfs_test_volume/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6557 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/fsxfs_test_volume/fsxfs_test_volume.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-02-22 06:45:42.000000 libfsxfs-20240222/msvscpp/libcpath/libcpath.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/fsxfs_test_attribute_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5924 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/fsxfs_test_attribute_values/fsxfs_test_attribute_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/fsxfs_test_tools_signal/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5839 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/fsxfs_test_tools_signal/fsxfs_test_tools_signal.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/fsxfs_test_attributes_table_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5945 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/fsxfs_test_attributes_table_header/fsxfs_test_attributes_table_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/fsxfs_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5732 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/fsxfs_test_notify/fsxfs_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/fsxfs_test_inode_btree/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5909 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/fsxfs_test_inode_btree/fsxfs_test_inode_btree.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/libhmac/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5312 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/libhmac/libhmac.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-02-22 06:45:42.000000 libfsxfs-20240222/msvscpp/libcsplit/libcsplit.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/fsxfs_test_attributes_leaf_block_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5960 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/fsxfs_test_attributes_leaf_block_header/fsxfs_test_attributes_leaf_block_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-02-22 06:45:42.000000 libfsxfs-20240222/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24637 2024-02-22 06:58:59.000000 libfsxfs-20240222/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/fsxfs_test_tools_output/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5839 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/fsxfs_test_tools_output/fsxfs_test_tools_output.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-02-22 06:45:42.000000 libfsxfs-20240222/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-02-22 06:45:42.000000 libfsxfs-20240222/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/fsxfs_test_btree_block/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6159 2024-02-22 06:46:01.000000 libfsxfs-20240222/msvscpp/fsxfs_test_btree_block/fsxfs_test_btree_block.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/msvscpp/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-02-22 06:45:42.000000 libfsxfs-20240222/msvscpp/libfdatetime/libfdatetime.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/pyfsxfs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1826 2024-02-22 06:45:17.000000 libfsxfs-20240222/pyfsxfs/pyfsxfs_datetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15962 2024-02-22 06:45:17.000000 libfsxfs-20240222/pyfsxfs/pyfsxfs.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1525 2024-02-22 06:45:17.000000 libfsxfs-20240222/pyfsxfs/pyfsxfs_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6952 2024-02-22 06:46:25.000000 libfsxfs-20240222/pyfsxfs/pyfsxfs_file_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8876 2024-02-22 06:45:17.000000 libfsxfs-20240222/pyfsxfs/pyfsxfs_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9546 2024-02-22 06:45:17.000000 libfsxfs-20240222/pyfsxfs/pyfsxfs_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3486 2024-02-22 06:46:25.000000 libfsxfs-20240222/pyfsxfs/pyfsxfs_extended_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-22 06:45:17.000000 libfsxfs-20240222/pyfsxfs/pyfsxfs_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28440 2024-02-22 06:46:25.000000 libfsxfs-20240222/pyfsxfs/pyfsxfs_extended_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24416 2024-02-22 06:46:25.000000 libfsxfs-20240222/pyfsxfs/pyfsxfs_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    71800 2024-02-22 06:46:25.000000 libfsxfs-20240222/pyfsxfs/pyfsxfs_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2033 2024-02-22 06:45:17.000000 libfsxfs-20240222/pyfsxfs/pyfsxfs_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-02-22 06:45:17.000000 libfsxfs-20240222/pyfsxfs/pyfsxfs_libfsxfs.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1332 2023-12-03 09:07:58.000000 libfsxfs-20240222/pyfsxfs/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-22 06:45:17.000000 libfsxfs-20240222/pyfsxfs/pyfsxfs_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9439 2024-02-22 06:45:17.000000 libfsxfs-20240222/pyfsxfs/pyfsxfs_file_entries.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2634 2024-02-22 06:45:17.000000 libfsxfs-20240222/pyfsxfs/pyfsxfs_extended_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1868 2024-02-22 06:45:17.000000 libfsxfs-20240222/pyfsxfs/pyfsxfs.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1540 2024-02-22 06:45:17.000000 libfsxfs-20240222/pyfsxfs/pyfsxfs_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16609 2024-02-22 06:45:17.000000 libfsxfs-20240222/pyfsxfs/pyfsxfs_datetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4118 2024-02-22 06:45:17.000000 libfsxfs-20240222/pyfsxfs/pyfsxfs_file_object_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2736 2024-02-22 06:46:25.000000 libfsxfs-20240222/pyfsxfs/pyfsxfs_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33880 2024-02-22 06:45:17.000000 libfsxfs-20240222/pyfsxfs/pyfsxfs_file_object_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2487 2024-02-22 06:45:17.000000 libfsxfs-20240222/pyfsxfs/pyfsxfs_file_entries.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47874 2024-02-22 06:58:59.000000 libfsxfs-20240222/pyfsxfs/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2024-02-22 06:45:17.000000 libfsxfs-20240222/pyfsxfs/pyfsxfs_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9890 2024-02-22 06:46:25.000000 libfsxfs-20240222/pyfsxfs/pyfsxfs_extended_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       92 2024-02-22 06:45:16.000000 libfsxfs-20240222/AUTHORS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:28.000000 libfsxfs-20240222/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-22 06:58:30.000000 libfsxfs-20240222/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-02-22 06:58:30.000000 libfsxfs-20240222/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-22 06:58:30.000000 libfsxfs-20240222/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-02-22 06:58:30.000000 libfsxfs-20240222/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-02-22 06:58:30.000000 libfsxfs-20240222/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-02-22 06:58:30.000000 libfsxfs-20240222/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      942 2024-02-22 06:58:30.000000 libfsxfs-20240222/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-02-22 06:58:30.000000 libfsxfs-20240222/libcfile/libcfile_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-22 06:58:30.000000 libfsxfs-20240222/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-02-22 06:58:30.000000 libfsxfs-20240222/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-22 06:58:30.000000 libfsxfs-20240222/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-02-22 06:58:30.000000 libfsxfs-20240222/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-22 06:58:30.000000 libfsxfs-20240222/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-22 06:58:30.000000 libfsxfs-20240222/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-02-22 06:58:30.000000 libfsxfs-20240222/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-22 06:58:30.000000 libfsxfs-20240222/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-02-22 06:58:30.000000 libfsxfs-20240222/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31159 2024-02-22 06:58:59.000000 libfsxfs-20240222/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-22 06:58:30.000000 libfsxfs-20240222/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-22 06:58:30.000000 libfsxfs-20240222/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-02-22 06:58:30.000000 libfsxfs-20240222/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-02-22 06:58:30.000000 libfsxfs-20240222/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      435 2024-02-22 06:46:01.000000 libfsxfs-20240222/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-02-22 06:58:59.000000 libfsxfs-20240222/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:28.000000 libfsxfs-20240222/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1127 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32843 2024-02-22 06:58:59.000000 libfsxfs-20240222/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-22 06:58:26.000000 libfsxfs-20240222/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-02-22 06:45:15.000000 libfsxfs-20240222/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      487 2024-02-22 06:45:15.000000 libfsxfs-20240222/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-02-22 06:58:59.000000 libfsxfs-20240222/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-02-22 06:45:15.000000 libfsxfs-20240222/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1508 2024-02-22 06:45:15.000000 libfsxfs-20240222/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:07:43.000000 libfsxfs-20240222/config.rpath
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      705 2024-02-22 06:45:15.000000 libfsxfs-20240222/libfsxfs.pc.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:28.000000 libfsxfs-20240222/libfsxfs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2304 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_btree_block.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3804 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1505 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_extents.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_btree_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32101 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_extended_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11271 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_directory_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1825 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1082 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28204 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_superblock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3464 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_superblock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8038 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_file_system_block_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2036 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1871 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_inode_btree_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_block_directory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6640 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_directory_table_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3159 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34470 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2129 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/fsxfs_block_directory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    99176 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19006 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_block_directory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2146 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1080 2024-02-22 06:59:11.000000 libfsxfs-20240222/libfsxfs/libfsxfs.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2339 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1731 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18245 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_directory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3847 2023-12-03 09:08:01.000000 libfsxfs-20240222/libfsxfs/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3751 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/fsxfs_inode_information.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5405 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_inode.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1971 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_attributes_leaf_block_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7517 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_extents.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9801 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/fsxfs_superblock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18038 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_extent_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7821 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_buffer_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4499 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/fsxfs_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22490 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_inode_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2216 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_file_system_block.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7881 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_extent.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12172 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_inode_information.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12050 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_directory_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4327 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_extent_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15544 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_attribute_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5046 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_extended_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2328 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_buffer_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14356 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10961 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_file_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1805 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_block_directory_footer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7870 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_attributes_leaf_block_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1942 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_directory_table_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_attribute_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1880 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_block_directory_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1979 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_extent.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5811 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3178 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_inode_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_extent_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7475 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_block_directory_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4581 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_block_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44504 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_inode.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5330 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/fsxfs_attributes_block.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1398 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2674 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_extent_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9101 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/fsxfs_inode.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2638 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_directory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9380 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1726 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_block_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/fsxfs_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2013 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_file_system_block_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1889 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_attributes_table_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3157 2024-02-22 06:59:11.000000 libfsxfs-20240222/libfsxfs/libfsxfs_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5700 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_attributes_table_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3060 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_directory_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24809 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_file_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12058 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_attributes_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1867 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_attributes_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1896 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_directory_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2427 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/fsxfs_file_system_block.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5661 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_inode_btree_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55528 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3170 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_file_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43177 2024-02-22 06:58:59.000000 libfsxfs-20240222/libfsxfs/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9681 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_btree_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9365 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_file_system_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2217 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_inode_information.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10957 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_btree_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10984 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_data_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5454 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_block_directory_footer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_data_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2624 2024-02-22 06:45:17.000000 libfsxfs-20240222/libfsxfs/libfsxfs_attributes.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:27.000000 libfsxfs-20240222/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-02-22 06:58:37.000000 libfsxfs-20240222/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-02-22 06:58:37.000000 libfsxfs-20240222/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-02-22 06:58:37.000000 libfsxfs-20240222/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-02-22 06:58:37.000000 libfsxfs-20240222/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-02-22 06:58:37.000000 libfsxfs-20240222/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-02-22 06:58:37.000000 libfsxfs-20240222/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-22 06:58:37.000000 libfsxfs-20240222/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-02-22 06:58:37.000000 libfsxfs-20240222/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-02-22 06:58:37.000000 libfsxfs-20240222/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-02-22 06:58:37.000000 libfsxfs-20240222/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-02-22 06:58:37.000000 libfsxfs-20240222/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-02-22 06:58:37.000000 libfsxfs-20240222/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-02-22 06:58:37.000000 libfsxfs-20240222/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-02-22 06:58:37.000000 libfsxfs-20240222/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-02-22 06:58:37.000000 libfsxfs-20240222/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-02-22 06:58:37.000000 libfsxfs-20240222/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-02-22 06:58:37.000000 libfsxfs-20240222/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-02-22 06:58:37.000000 libfsxfs-20240222/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-02-22 06:58:37.000000 libfsxfs-20240222/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-02-22 06:58:37.000000 libfsxfs-20240222/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-22 06:58:37.000000 libfsxfs-20240222/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-02-22 06:58:37.000000 libfsxfs-20240222/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-02-22 06:58:37.000000 libfsxfs-20240222/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-02-22 06:58:37.000000 libfsxfs-20240222/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-02-22 06:58:37.000000 libfsxfs-20240222/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-02-22 06:58:37.000000 libfsxfs-20240222/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-02-22 06:58:37.000000 libfsxfs-20240222/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33249 2024-02-22 06:58:59.000000 libfsxfs-20240222/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-02-22 06:58:37.000000 libfsxfs-20240222/libcthreads/libcthreads_queue.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-02-22 06:58:59.000000 libfsxfs-20240222/test-driver
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:28.000000 libfsxfs-20240222/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-02-22 06:58:34.000000 libfsxfs-20240222/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-22 06:58:34.000000 libfsxfs-20240222/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-02-22 06:58:34.000000 libfsxfs-20240222/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      842 2024-02-22 06:58:34.000000 libfsxfs-20240222/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-22 06:58:34.000000 libfsxfs-20240222/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-22 06:58:34.000000 libfsxfs-20240222/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-22 06:58:34.000000 libfsxfs-20240222/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-02-22 06:58:34.000000 libfsxfs-20240222/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-02-22 06:58:34.000000 libfsxfs-20240222/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-02-22 06:58:34.000000 libfsxfs-20240222/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-22 06:58:34.000000 libfsxfs-20240222/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-22 06:58:34.000000 libfsxfs-20240222/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30437 2024-02-22 06:58:59.000000 libfsxfs-20240222/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-22 06:58:34.000000 libfsxfs-20240222/libcpath/libcpath_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-22 06:58:34.000000 libfsxfs-20240222/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-02-22 06:58:34.000000 libfsxfs-20240222/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-02-22 06:58:34.000000 libfsxfs-20240222/libcpath/libcpath_path.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1063 2023-12-03 09:07:43.000000 libfsxfs-20240222/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1888 2024-02-22 06:45:18.000000 libfsxfs-20240222/manuals/fsxfsinfo.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      190 2023-12-03 09:07:58.000000 libfsxfs-20240222/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13196 2024-02-22 06:45:18.000000 libfsxfs-20240222/manuals/libfsxfs.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1414 2024-02-22 06:45:18.000000 libfsxfs-20240222/manuals/fsxfsmount.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27394 2024-02-22 06:58:59.000000 libfsxfs-20240222/manuals/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1709 2024-02-22 06:45:18.000000 libfsxfs-20240222/tests/fsxfs_test_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5706 2024-02-22 06:45:18.000000 libfsxfs-20240222/tests/fsxfs_test_tools_info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11403 2024-02-22 06:46:01.000000 libfsxfs-20240222/tests/fsxfs_test_attributes_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4323 2024-02-22 06:45:18.000000 libfsxfs-20240222/tests/fsxfs_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26898 2024-02-22 06:46:01.000000 libfsxfs-20240222/tests/fsxfs_test_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4700 2024-02-22 06:45:18.000000 libfsxfs-20240222/tests/fsxfs_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-02-22 06:45:18.000000 libfsxfs-20240222/tests/fsxfs_test_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9963 2024-02-22 06:46:01.000000 libfsxfs-20240222/tests/fsxfs_test_block_directory_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-02-22 06:45:18.000000 libfsxfs-20240222/tests/fsxfs_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-02-22 06:45:18.000000 libfsxfs-20240222/tests/fsxfs_test_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11592 2024-02-22 06:46:01.000000 libfsxfs-20240222/tests/fsxfs_test_file_system_block_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6420 2024-02-22 06:46:01.000000 libfsxfs-20240222/tests/fsxfs_test_directory_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8672 2024-02-22 06:46:25.000000 libfsxfs-20240222/tests/pyfsxfs_test_volume.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4076 2024-02-22 06:46:25.000000 libfsxfs-20240222/tests/test_tools.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5952 2024-02-22 06:46:01.000000 libfsxfs-20240222/tests/fsxfs_test_extent.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6196 2024-02-22 06:46:01.000000 libfsxfs-20240222/tests/fsxfs_test_inode_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-02-22 06:45:18.000000 libfsxfs-20240222/tests/fsxfs_test_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15297 2024-02-22 06:46:01.000000 libfsxfs-20240222/tests/fsxfs_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10870 2024-02-22 06:46:01.000000 libfsxfs-20240222/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18310 2024-02-22 06:46:01.000000 libfsxfs-20240222/tests/fsxfs_test_attribute_values.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3348 2024-02-22 06:45:17.000000 libfsxfs-20240222/tests/test_fsxfsinfo.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4169 2024-02-22 06:45:18.000000 libfsxfs-20240222/tests/fsxfs_test_tools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15726 2024-02-22 06:46:01.000000 libfsxfs-20240222/tests/fsxfs_test_functions.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19056 2024-02-22 06:46:01.000000 libfsxfs-20240222/tests/fsxfs_test_inode_information.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11789 2024-02-22 06:46:01.000000 libfsxfs-20240222/tests/fsxfs_test_attributes_leaf_block_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8574 2024-02-22 06:45:18.000000 libfsxfs-20240222/tests/fsxfs_test_macros.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-02-22 06:45:17.000000 libfsxfs-20240222/tests/test_manpage.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4086 2024-02-22 06:45:18.000000 libfsxfs-20240222/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1997 2024-02-22 06:46:25.000000 libfsxfs-20240222/tests/fsxfs_test_functions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-02-22 06:45:18.000000 libfsxfs-20240222/tests/fsxfs_test_libfsxfs.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9899 2024-02-22 06:46:01.000000 libfsxfs-20240222/tests/fsxfs_test_directory_table_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9978 2024-02-22 06:46:01.000000 libfsxfs-20240222/tests/fsxfs_test_attributes_table_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9911 2024-02-22 06:46:01.000000 libfsxfs-20240222/tests/fsxfs_test_block_directory_footer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2447 2024-02-22 06:45:18.000000 libfsxfs-20240222/tests/fsxfs_test_tools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8185 2024-02-22 06:46:01.000000 libfsxfs-20240222/tests/fsxfs_test_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-02-22 06:45:18.000000 libfsxfs-20240222/tests/fsxfs_test_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-02-22 06:45:18.000000 libfsxfs-20240222/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3139 2024-02-22 06:45:18.000000 libfsxfs-20240222/tests/fsxfs_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-02-22 06:45:18.000000 libfsxfs-20240222/tests/fsxfs_test_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-02-22 06:45:18.000000 libfsxfs-20240222/tests/fsxfs_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3464 2024-02-22 06:46:25.000000 libfsxfs-20240222/tests/pyfsxfs_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2800 2024-02-22 06:45:18.000000 libfsxfs-20240222/tests/fsxfs_test_buffer_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15930 2024-02-22 06:46:01.000000 libfsxfs-20240222/tests/fsxfs_test_superblock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    77398 2024-02-22 06:58:59.000000 libfsxfs-20240222/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9515 2024-02-22 06:46:01.000000 libfsxfs-20240222/tests/fsxfs_test_inode_btree_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10685 2024-02-22 06:46:01.000000 libfsxfs-20240222/tests/fsxfs_test_btree_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18604 2024-02-22 06:46:01.000000 libfsxfs-20240222/tests/fsxfs_test_btree_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-02-22 06:45:18.000000 libfsxfs-20240222/tests/fsxfs_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-22 06:45:18.000000 libfsxfs-20240222/tests/fsxfs_test_unused.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4393 2024-02-22 06:46:25.000000 libfsxfs-20240222/tests/test_library.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2625 2024-02-22 06:45:17.000000 libfsxfs-20240222/ossfuzz/volume_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2024 2023-12-03 09:08:00.000000 libfsxfs-20240222/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-02-22 06:45:17.000000 libfsxfs-20240222/ossfuzz/ossfuzz_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5429 2024-02-22 06:45:17.000000 libfsxfs-20240222/ossfuzz/file_entry_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3320 2024-02-22 06:45:17.000000 libfsxfs-20240222/ossfuzz/extended_attribute_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      972 2024-02-22 06:45:17.000000 libfsxfs-20240222/ossfuzz/ossfuzz_libfsxfs.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36747 2024-02-22 06:58:59.000000 libfsxfs-20240222/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-02-22 06:58:52.000000 libfsxfs-20240222/ltmain.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/libhmac/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47989 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_sha1_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_sha224.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50026 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_sha512_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14448 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_md5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2079 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_md5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1942 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9362 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14650 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_sha512.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45648 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_sha256_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_sha224.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1623 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2060 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_sha1.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3443 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_sha256_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1121 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45605 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_sha224_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_md5_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_sha256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3368 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_sha1_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32969 2024-02-22 06:58:59.000000 libfsxfs-20240222/libhmac/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_sha256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3461 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_sha224_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3444 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_sha512_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_sha512.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14514 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_sha1.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40596 2024-02-22 06:58:44.000000 libfsxfs-20240222/libhmac/libhmac_md5_context.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:28.000000 libfsxfs-20240222/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-02-22 06:58:35.000000 libfsxfs-20240222/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-02-22 06:58:35.000000 libfsxfs-20240222/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-02-22 06:58:35.000000 libfsxfs-20240222/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-02-22 06:58:35.000000 libfsxfs-20240222/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-22 06:58:35.000000 libfsxfs-20240222/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      884 2024-02-22 06:58:35.000000 libfsxfs-20240222/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-22 06:58:35.000000 libfsxfs-20240222/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-02-22 06:58:35.000000 libfsxfs-20240222/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-22 06:58:35.000000 libfsxfs-20240222/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-02-22 06:58:35.000000 libfsxfs-20240222/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-22 06:58:35.000000 libfsxfs-20240222/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-02-22 06:58:35.000000 libfsxfs-20240222/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-22 06:58:35.000000 libfsxfs-20240222/libcsplit/libcsplit_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-22 06:58:35.000000 libfsxfs-20240222/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-22 06:58:35.000000 libfsxfs-20240222/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-02-22 06:58:35.000000 libfsxfs-20240222/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31217 2024-02-22 06:58:59.000000 libfsxfs-20240222/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-02-22 06:58:35.000000 libfsxfs-20240222/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-02-22 06:58:35.000000 libfsxfs-20240222/libcsplit/libcsplit_narrow_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:29.000000 libfsxfs-20240222/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:08:00.000000 libfsxfs-20240222/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:08:00.000000 libfsxfs-20240222/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:08:00.000000 libfsxfs-20240222/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:08:00.000000 libfsxfs-20240222/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:08:00.000000 libfsxfs-20240222/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:08:00.000000 libfsxfs-20240222/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:08:00.000000 libfsxfs-20240222/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:08:00.000000 libfsxfs-20240222/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:08:00.000000 libfsxfs-20240222/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1854 2024-02-22 06:59:10.000000 libfsxfs-20240222/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:08:00.000000 libfsxfs-20240222/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:08:00.000000 libfsxfs-20240222/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:28.000000 libfsxfs-20240222/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4197 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53961 2024-02-22 06:58:59.000000 libfsxfs-20240222/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-02-22 06:58:47.000000 libfsxfs-20240222/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41467 2024-02-22 06:58:59.000000 libfsxfs-20240222/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:28.000000 libfsxfs-20240222/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-22 06:58:32.000000 libfsxfs-20240222/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-22 06:58:32.000000 libfsxfs-20240222/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-02-22 06:58:32.000000 libfsxfs-20240222/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-02-22 06:58:32.000000 libfsxfs-20240222/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-02-22 06:58:32.000000 libfsxfs-20240222/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-22 06:58:32.000000 libfsxfs-20240222/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-02-22 06:58:32.000000 libfsxfs-20240222/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-02-22 06:58:32.000000 libfsxfs-20240222/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-02-22 06:58:32.000000 libfsxfs-20240222/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-02-22 06:58:32.000000 libfsxfs-20240222/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-02-22 06:58:32.000000 libfsxfs-20240222/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30271 2024-02-22 06:58:59.000000 libfsxfs-20240222/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-02-22 06:58:32.000000 libfsxfs-20240222/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-02-22 06:58:32.000000 libfsxfs-20240222/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:27.000000 libfsxfs-20240222/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-02-22 06:58:28.000000 libfsxfs-20240222/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-02-22 06:58:28.000000 libfsxfs-20240222/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-22 06:58:28.000000 libfsxfs-20240222/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-02-22 06:58:28.000000 libfsxfs-20240222/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-02-22 06:58:28.000000 libfsxfs-20240222/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-22 06:58:28.000000 libfsxfs-20240222/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-02-22 06:58:28.000000 libfsxfs-20240222/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-02-22 06:58:28.000000 libfsxfs-20240222/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-02-22 06:58:28.000000 libfsxfs-20240222/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-22 06:58:28.000000 libfsxfs-20240222/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-22 06:58:28.000000 libfsxfs-20240222/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29784 2024-02-22 06:58:59.000000 libfsxfs-20240222/libcerror/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-22 19:02:28.000000 libfsxfs-20240222/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-02-22 06:58:41.000000 libfsxfs-20240222/libfdatetime/libfdatetime_floatingtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-02-22 06:58:41.000000 libfsxfs-20240222/libfdatetime/libfdatetime_nsf_timedate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-02-22 06:58:41.000000 libfsxfs-20240222/libfdatetime/libfdatetime_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-02-22 06:58:41.000000 libfsxfs-20240222/libfdatetime/libfdatetime_floatingtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-02-22 06:58:41.000000 libfsxfs-20240222/libfdatetime/libfdatetime_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-02-22 06:58:41.000000 libfsxfs-20240222/libfdatetime/libfdatetime_hfs_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-02-22 06:58:41.000000 libfsxfs-20240222/libfdatetime/libfdatetime_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-02-22 06:58:41.000000 libfsxfs-20240222/libfdatetime/libfdatetime_hfs_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1148 2024-02-22 06:58:41.000000 libfsxfs-20240222/libfdatetime/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-02-22 06:58:41.000000 libfsxfs-20240222/libfdatetime/libfdatetime_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-02-22 06:58:41.000000 libfsxfs-20240222/libfdatetime/libfdatetime_systemtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-22 06:58:41.000000 libfsxfs-20240222/libfdatetime/libfdatetime_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-02-22 06:58:41.000000 libfsxfs-20240222/libfdatetime/libfdatetime_posix_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-02-22 06:58:41.000000 libfsxfs-20240222/libfdatetime/libfdatetime_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-02-22 06:58:41.000000 libfsxfs-20240222/libfdatetime/libfdatetime_fat_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-02-22 06:58:41.000000 libfsxfs-20240222/libfdatetime/libfdatetime_systemtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-02-22 06:58:41.000000 libfsxfs-20240222/libfdatetime/libfdatetime_nsf_timedate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-02-22 06:58:41.000000 libfsxfs-20240222/libfdatetime/libfdatetime_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-02-22 06:58:41.000000 libfsxfs-20240222/libfdatetime/libfdatetime_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-02-22 06:58:41.000000 libfsxfs-20240222/libfdatetime/libfdatetime_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-02-22 06:58:41.000000 libfsxfs-20240222/libfdatetime/libfdatetime_posix_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-02-22 06:58:41.000000 libfsxfs-20240222/libfdatetime/libfdatetime_date_time_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-02-22 06:58:41.000000 libfsxfs-20240222/libfdatetime/libfdatetime_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-02-22 06:58:41.000000 libfsxfs-20240222/libfdatetime/libfdatetime_date_time_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-02-22 06:58:41.000000 libfsxfs-20240222/libfdatetime/libfdatetime_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33010 2024-02-22 06:58:59.000000 libfsxfs-20240222/libfdatetime/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-02-22 06:58:41.000000 libfsxfs-20240222/libfdatetime/libfdatetime_fat_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56884 2024-02-22 06:58:55.000000 libfsxfs-20240222/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8065 2024-02-22 06:45:15.000000 libfsxfs-20240222/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      418 2024-02-22 19:02:30.228888 libfsxfs-20240222/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:54.000000 libfsxfs-20240501/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_area.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_mapped_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1287 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_area.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_mapped_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_segments_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_segments_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34244 2024-05-01 16:29:53.000000 libfsxfs-20240501/libfdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-05-01 16:29:32.000000 libfsxfs-20240501/libfdata/libfdata_vector.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:54.000000 libfsxfs-20240501/fsxfstools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1781 2024-05-01 16:06:34.000000 libfsxfs-20240501/fsxfstools/fsxfstools_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-05-01 16:06:34.000000 libfsxfs-20240501/fsxfstools/fsxfstools_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36321 2024-05-01 16:08:07.000000 libfsxfs-20240501/fsxfstools/mount_dokan.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3061 2024-05-01 16:08:07.000000 libfsxfs-20240501/fsxfstools/mount_file_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1486 2024-05-01 16:06:34.000000 libfsxfs-20240501/fsxfstools/fsxfstools_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4145 2024-05-01 16:06:34.000000 libfsxfs-20240501/fsxfstools/fsxfstools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37913 2024-05-01 16:08:07.000000 libfsxfs-20240501/fsxfstools/mount_fuse.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1472 2024-05-01 16:06:34.000000 libfsxfs-20240501/fsxfstools/fsxfstools_output.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4426 2024-05-01 16:08:07.000000 libfsxfs-20240501/fsxfstools/info_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5417 2024-05-01 16:06:34.000000 libfsxfs-20240501/fsxfstools/mount_dokan.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1771 2024-05-01 16:06:34.000000 libfsxfs-20240501/fsxfstools/fsxfstools_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3297 2024-05-01 16:06:34.000000 libfsxfs-20240501/fsxfstools/digest_hash.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30757 2024-05-01 16:08:07.000000 libfsxfs-20240501/fsxfstools/mount_file_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1409 2024-05-01 16:06:34.000000 libfsxfs-20240501/fsxfstools/fsxfstools_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-01 16:06:34.000000 libfsxfs-20240501/fsxfstools/fsxfstools_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2512 2024-05-01 16:09:40.000000 libfsxfs-20240501/fsxfstools/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-05-01 16:06:34.000000 libfsxfs-20240501/fsxfstools/fsxfstools_libfsxfs.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10866 2024-05-01 16:08:07.000000 libfsxfs-20240501/fsxfstools/fsxfsinfo.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22158 2024-05-01 16:08:07.000000 libfsxfs-20240501/fsxfstools/mount_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    63194 2024-05-01 16:08:07.000000 libfsxfs-20240501/fsxfstools/info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3661 2024-05-01 16:08:07.000000 libfsxfs-20240501/fsxfstools/mount_file_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1761 2024-05-01 16:06:34.000000 libfsxfs-20240501/fsxfstools/fsxfstools_signal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1474 2024-05-01 16:06:34.000000 libfsxfs-20240501/fsxfstools/fsxfstools_libhmac.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1213 2024-05-01 16:06:34.000000 libfsxfs-20240501/fsxfstools/fsxfstools_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-05-01 16:06:34.000000 libfsxfs-20240501/fsxfstools/fsxfstools_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-05-01 16:06:34.000000 libfsxfs-20240501/fsxfstools/fsxfstools_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3324 2024-05-01 16:08:07.000000 libfsxfs-20240501/fsxfstools/mount_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1483 2024-05-01 16:06:34.000000 libfsxfs-20240501/fsxfstools/fsxfstools_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-05-01 16:06:34.000000 libfsxfs-20240501/fsxfstools/fsxfstools_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5751 2024-05-01 16:06:34.000000 libfsxfs-20240501/fsxfstools/fsxfstools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19354 2024-05-01 16:08:07.000000 libfsxfs-20240501/fsxfstools/mount_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15469 2024-05-01 16:08:07.000000 libfsxfs-20240501/fsxfstools/fsxfsmount.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35468 2024-05-01 16:29:53.000000 libfsxfs-20240501/fsxfstools/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-05-01 16:06:34.000000 libfsxfs-20240501/fsxfstools/fsxfstools_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1244 2024-05-01 16:06:34.000000 libfsxfs-20240501/fsxfstools/digest_hash.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3050 2024-05-01 16:08:07.000000 libfsxfs-20240501/fsxfstools/mount_fuse.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1590 2024-05-01 16:06:34.000000 libfsxfs-20240501/fsxfstools/fsxfstools_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-05-01 16:06:31.000000 libfsxfs-20240501/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-05-01 16:29:53.000000 libfsxfs-20240501/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 16:06:31.000000 libfsxfs-20240501/NEWS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-05-01 16:29:54.000000 libfsxfs-20240501/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:54.000000 libfsxfs-20240501/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-01 16:29:35.000000 libfsxfs-20240501/libfguid/libfguid_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-05-01 16:29:35.000000 libfsxfs-20240501/libfguid/libfguid_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-05-01 16:29:35.000000 libfsxfs-20240501/libfguid/libfguid_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-01 16:29:35.000000 libfsxfs-20240501/libfguid/libfguid_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      677 2024-05-01 16:29:35.000000 libfsxfs-20240501/libfguid/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-01 16:29:35.000000 libfsxfs-20240501/libfguid/libfguid_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-01 16:29:35.000000 libfsxfs-20240501/libfguid/libfguid_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-05-01 16:29:35.000000 libfsxfs-20240501/libfguid/libfguid_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-05-01 16:29:35.000000 libfsxfs-20240501/libfguid/libfguid_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-05-01 16:29:35.000000 libfsxfs-20240501/libfguid/libfguid_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-05-01 16:29:35.000000 libfsxfs-20240501/libfguid/libfguid_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30045 2024-05-01 16:29:53.000000 libfsxfs-20240501/libfguid/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-01 16:29:35.000000 libfsxfs-20240501/libfguid/libfguid_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3453 2024-05-01 16:06:31.000000 libfsxfs-20240501/libfsxfs.spec.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:53.000000 libfsxfs-20240501/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11734 2024-05-01 16:06:35.000000 libfsxfs-20240501/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18489 2024-05-01 16:06:35.000000 libfsxfs-20240501/m4/libfdatetime.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:07:57.000000 libfsxfs-20240501/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9615 2024-05-01 16:06:35.000000 libfsxfs-20240501/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:07:58.000000 libfsxfs-20240501/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:07:57.000000 libfsxfs-20240501/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-05-01 16:06:35.000000 libfsxfs-20240501/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:07:57.000000 libfsxfs-20240501/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:07:58.000000 libfsxfs-20240501/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-05-01 16:06:35.000000 libfsxfs-20240501/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-05-01 16:06:35.000000 libfsxfs-20240501/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7625 2024-05-01 16:06:35.000000 libfsxfs-20240501/m4/libcsplit.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-05-01 16:06:35.000000 libfsxfs-20240501/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-05-01 16:06:35.000000 libfsxfs-20240501/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-05-01 16:29:46.000000 libfsxfs-20240501/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-05-01 16:29:46.000000 libfsxfs-20240501/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15781 2024-05-01 16:06:35.000000 libfsxfs-20240501/m4/libfdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:07:58.000000 libfsxfs-20240501/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7058 2024-05-01 16:06:35.000000 libfsxfs-20240501/m4/libfuse.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-05-01 16:29:45.000000 libfsxfs-20240501/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:07:57.000000 libfsxfs-20240501/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-05-01 16:06:35.000000 libfsxfs-20240501/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-05-01 16:06:35.000000 libfsxfs-20240501/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5876 2024-05-01 16:06:35.000000 libfsxfs-20240501/m4/libfguid.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11923 2024-05-01 16:06:35.000000 libfsxfs-20240501/m4/libbfio.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8550 2024-05-01 16:06:35.000000 libfsxfs-20240501/m4/libhmac.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:07:57.000000 libfsxfs-20240501/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-05-01 16:29:46.000000 libfsxfs-20240501/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:07:58.000000 libfsxfs-20240501/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:07:58.000000 libfsxfs-20240501/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-05-01 16:29:46.000000 libfsxfs-20240501/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:07:57.000000 libfsxfs-20240501/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-05-01 16:06:35.000000 libfsxfs-20240501/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27647 2024-05-01 16:06:35.000000 libfsxfs-20240501/m4/libcrypto.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:07:58.000000 libfsxfs-20240501/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7566 2024-05-01 16:06:35.000000 libfsxfs-20240501/m4/libfcache.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-05-01 16:06:35.000000 libfsxfs-20240501/m4/pthread.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:53.000000 libfsxfs-20240501/include/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      425 2024-05-01 16:09:27.000000 libfsxfs-20240501/include/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:53.000000 libfsxfs-20240501/include/libfsxfs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2221 2024-05-01 16:06:33.000000 libfsxfs-20240501/include/libfsxfs/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2219 2024-05-01 16:30:06.000000 libfsxfs-20240501/include/libfsxfs/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5032 2024-05-01 16:06:33.000000 libfsxfs-20240501/include/libfsxfs/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4901 2024-05-01 16:30:06.000000 libfsxfs-20240501/include/libfsxfs/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-01 16:06:33.000000 libfsxfs-20240501/include/libfsxfs/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2024-05-01 16:06:33.000000 libfsxfs-20240501/include/libfsxfs/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-01 16:06:33.000000 libfsxfs-20240501/include/libfsxfs/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1487 2024-05-01 16:30:06.000000 libfsxfs-20240501/include/libfsxfs/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5306 2024-05-01 16:06:33.000000 libfsxfs-20240501/include/libfsxfs/codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28421 2024-05-01 16:29:53.000000 libfsxfs-20240501/include/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26614 2024-05-01 16:06:33.000000 libfsxfs-20240501/include/libfsxfs.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26614 2024-05-01 16:30:06.000000 libfsxfs-20240501/include/libfsxfs.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:53.000000 libfsxfs-20240501/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-05-01 16:06:33.000000 libfsxfs-20240501/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-05-01 16:06:33.000000 libfsxfs-20240501/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-05-01 16:06:33.000000 libfsxfs-20240501/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-05-01 16:06:33.000000 libfsxfs-20240501/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-01 16:06:33.000000 libfsxfs-20240501/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-05-01 16:06:33.000000 libfsxfs-20240501/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-05-01 16:06:33.000000 libfsxfs-20240501/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-05-01 16:09:27.000000 libfsxfs-20240501/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-05-01 16:06:33.000000 libfsxfs-20240501/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7374 2024-05-01 16:30:06.000000 libfsxfs-20240501/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17932 2024-05-01 16:29:52.000000 libfsxfs-20240501/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18983 2024-05-01 16:30:06.000000 libfsxfs-20240501/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-05-01 16:06:33.000000 libfsxfs-20240501/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-05-01 16:06:33.000000 libfsxfs-20240501/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-05-01 16:06:33.000000 libfsxfs-20240501/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25455 2024-05-01 16:29:53.000000 libfsxfs-20240501/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:53.000000 libfsxfs-20240501/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-05-01 16:29:21.000000 libfsxfs-20240501/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-05-01 16:29:21.000000 libfsxfs-20240501/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-05-01 16:29:21.000000 libfsxfs-20240501/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-05-01 16:29:21.000000 libfsxfs-20240501/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-01 16:29:21.000000 libfsxfs-20240501/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-01 16:29:21.000000 libfsxfs-20240501/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-05-01 16:29:21.000000 libfsxfs-20240501/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-05-01 16:29:21.000000 libfsxfs-20240501/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-05-01 16:29:21.000000 libfsxfs-20240501/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-05-01 16:29:21.000000 libfsxfs-20240501/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30653 2024-05-01 16:29:53.000000 libfsxfs-20240501/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-01 16:29:21.000000 libfsxfs-20240501/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-05-01 16:29:21.000000 libfsxfs-20240501/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-05-01 16:29:21.000000 libfsxfs-20240501/libclocale/libclocale_codepage.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:54.000000 libfsxfs-20240501/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-01 16:29:30.000000 libfsxfs-20240501/libfcache/libfcache_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-05-01 16:29:30.000000 libfsxfs-20240501/libfcache/libfcache_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-05-01 16:29:30.000000 libfsxfs-20240501/libfcache/libfcache_cache_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-01 16:29:30.000000 libfsxfs-20240501/libfcache/libfcache_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      876 2024-05-01 16:29:31.000000 libfsxfs-20240501/libfcache/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-01 16:29:30.000000 libfsxfs-20240501/libfcache/libfcache_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-01 16:29:30.000000 libfsxfs-20240501/libfcache/libfcache_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-05-01 16:29:30.000000 libfsxfs-20240501/libfcache/libfcache_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-05-01 16:29:30.000000 libfsxfs-20240501/libfcache/libfcache_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-01 16:29:30.000000 libfsxfs-20240501/libfcache/libfcache_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-01 16:29:30.000000 libfsxfs-20240501/libfcache/libfcache_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-05-01 16:29:30.000000 libfsxfs-20240501/libfcache/libfcache_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-01 16:29:30.000000 libfsxfs-20240501/libfcache/libfcache_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-05-01 16:29:30.000000 libfsxfs-20240501/libfcache/libfcache_cache_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31162 2024-05-01 16:29:53.000000 libfsxfs-20240501/libfcache/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-01 16:29:30.000000 libfsxfs-20240501/libfcache/libfcache_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-05-01 16:29:31.000000 libfsxfs-20240501/libfcache/libfcache_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-05-01 16:29:30.000000 libfsxfs-20240501/libfcache/libfcache_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2111 2024-05-01 16:11:35.000000 libfsxfs-20240501/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:54.000000 libfsxfs-20240501/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_file_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_file_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_file_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_file_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_file_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_file_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_memory_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_file_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_file_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_memory_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_memory_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34505 2024-05-01 16:29:53.000000 libfsxfs-20240501/libbfio/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_memory_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-05-01 16:29:15.000000 libfsxfs-20240501/libbfio/libbfio_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:07:42.000000 libfsxfs-20240501/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-05-01 16:29:53.000000 libfsxfs-20240501/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:53.000000 libfsxfs-20240501/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-05-01 16:06:31.000000 libfsxfs-20240501/dpkg/libfsxfs-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1026 2024-05-01 16:06:35.000000 libfsxfs-20240501/dpkg/copyright
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:53.000000 libfsxfs-20240501/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-05-01 16:06:31.000000 libfsxfs-20240501/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-05-01 16:06:31.000000 libfsxfs-20240501/dpkg/libfsxfs-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2119 2024-05-01 16:06:31.000000 libfsxfs-20240501/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      769 2024-05-01 16:06:31.000000 libfsxfs-20240501/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-05-01 16:06:31.000000 libfsxfs-20240501/dpkg/libfsxfs-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      121 2024-05-01 16:06:31.000000 libfsxfs-20240501/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2024-05-01 16:30:06.000000 libfsxfs-20240501/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-05-01 16:06:31.000000 libfsxfs-20240501/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-05-01 16:06:31.000000 libfsxfs-20240501/dpkg/libfsxfs.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      486 2024-05-01 16:30:06.000000 libfsxfs-20240501/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-05-01 16:06:31.000000 libfsxfs-20240501/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1990719 2024-05-01 16:29:51.000000 libfsxfs-20240501/configure
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2410 2024-05-01 16:30:06.000000 libfsxfs-20240501/libfsxfs.spec
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-05-01 16:29:53.000000 libfsxfs-20240501/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-05-01 16:29:53.000000 libfsxfs-20240501/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-05-01 16:07:26.000000 libfsxfs-20240501/msvscpp/libfdata/libfdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/fsxfsinfo/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7194 2024-05-01 16:07:26.000000 libfsxfs-20240501/msvscpp/fsxfsinfo/fsxfsinfo.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/fsxfs_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5645 2024-05-01 16:07:46.000000 libfsxfs-20240501/msvscpp/fsxfs_test_error/fsxfs_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/fsxfs_test_tools_info_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6164 2024-05-01 16:07:46.000000 libfsxfs-20240501/msvscpp/fsxfs_test_tools_info_handle/fsxfs_test_tools_info_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/fsxfs_test_extent/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5894 2024-05-01 16:07:46.000000 libfsxfs-20240501/msvscpp/fsxfs_test_extent/fsxfs_test_extent.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40758 2024-05-01 16:07:46.000000 libfsxfs-20240501/msvscpp/libfsxfs.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/fsxfs_test_file_system_block_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5948 2024-05-01 16:07:46.000000 libfsxfs-20240501/msvscpp/fsxfs_test_file_system_block_header/fsxfs_test_file_system_block_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/fsxfsmount/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7669 2024-05-01 16:07:26.000000 libfsxfs-20240501/msvscpp/fsxfsmount/fsxfsmount.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-05-01 16:07:26.000000 libfsxfs-20240501/msvscpp/libfguid/libfguid.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/fsxfs_test_inode_btree_record/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5930 2024-05-01 16:07:46.000000 libfsxfs-20240501/msvscpp/fsxfs_test_inode_btree_record/fsxfs_test_inode_btree_record.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/fsxfs_test_directory_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5921 2024-05-01 16:07:46.000000 libfsxfs-20240501/msvscpp/fsxfs_test_directory_entry/fsxfs_test_directory_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/fsxfs_test_directory_table_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5942 2024-05-01 16:07:46.000000 libfsxfs-20240501/msvscpp/fsxfs_test_directory_table_header/fsxfs_test_directory_table_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-05-01 16:07:26.000000 libfsxfs-20240501/msvscpp/libclocale/libclocale.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/fsxfs_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6560 2024-05-01 16:07:46.000000 libfsxfs-20240501/msvscpp/fsxfs_test_support/fsxfs_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-05-01 16:07:26.000000 libfsxfs-20240501/msvscpp/libfcache/libfcache.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2248 2024-05-01 16:09:48.000000 libfsxfs-20240501/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-05-01 16:07:26.000000 libfsxfs-20240501/msvscpp/libbfio/libbfio.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/fsxfs_test_block_directory_footer/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5942 2024-05-01 16:07:46.000000 libfsxfs-20240501/msvscpp/fsxfs_test_block_directory_footer/fsxfs_test_block_directory_footer.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/fsxfs_test_io_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5903 2024-05-01 16:07:46.000000 libfsxfs-20240501/msvscpp/fsxfs_test_io_handle/fsxfs_test_io_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/pyfsxfs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6839 2024-05-01 16:07:46.000000 libfsxfs-20240501/msvscpp/pyfsxfs/pyfsxfs.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-05-01 16:07:26.000000 libfsxfs-20240501/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/fsxfs_test_block_directory_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5942 2024-05-01 16:07:46.000000 libfsxfs-20240501/msvscpp/fsxfs_test_block_directory_header/fsxfs_test_block_directory_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/fsxfs_test_attributes_table/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6007 2024-05-01 16:07:46.000000 libfsxfs-20240501/msvscpp/fsxfs_test_attributes_table/fsxfs_test_attributes_table.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-05-01 16:07:26.000000 libfsxfs-20240501/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/fsxfs_test_inode_information/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-05-01 16:07:46.000000 libfsxfs-20240501/msvscpp/fsxfs_test_inode_information/fsxfs_test_inode_information.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/fsxfs_test_superblock/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6156 2024-05-01 16:07:46.000000 libfsxfs-20240501/msvscpp/fsxfs_test_superblock/fsxfs_test_superblock.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/fsxfs_test_buffer_data_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5930 2024-05-01 16:07:46.000000 libfsxfs-20240501/msvscpp/fsxfs_test_buffer_data_handle/fsxfs_test_buffer_data_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/fsxfs_test_btree_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5912 2024-05-01 16:07:46.000000 libfsxfs-20240501/msvscpp/fsxfs_test_btree_header/fsxfs_test_btree_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/libfsxfs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13845 2024-05-01 16:07:26.000000 libfsxfs-20240501/msvscpp/libfsxfs/libfsxfs.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-05-01 16:07:26.000000 libfsxfs-20240501/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/fsxfs_test_volume/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6557 2024-05-01 16:07:46.000000 libfsxfs-20240501/msvscpp/fsxfs_test_volume/fsxfs_test_volume.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-05-01 16:07:26.000000 libfsxfs-20240501/msvscpp/libcpath/libcpath.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/fsxfs_test_attribute_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5924 2024-05-01 16:07:46.000000 libfsxfs-20240501/msvscpp/fsxfs_test_attribute_values/fsxfs_test_attribute_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/fsxfs_test_tools_signal/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5839 2024-05-01 16:07:46.000000 libfsxfs-20240501/msvscpp/fsxfs_test_tools_signal/fsxfs_test_tools_signal.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/fsxfs_test_attributes_table_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5945 2024-05-01 16:07:46.000000 libfsxfs-20240501/msvscpp/fsxfs_test_attributes_table_header/fsxfs_test_attributes_table_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/fsxfs_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5732 2024-05-01 16:07:46.000000 libfsxfs-20240501/msvscpp/fsxfs_test_notify/fsxfs_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/fsxfs_test_inode_btree/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5909 2024-05-01 16:07:46.000000 libfsxfs-20240501/msvscpp/fsxfs_test_inode_btree/fsxfs_test_inode_btree.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/libhmac/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5312 2024-05-01 16:07:46.000000 libfsxfs-20240501/msvscpp/libhmac/libhmac.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-05-01 16:07:26.000000 libfsxfs-20240501/msvscpp/libcsplit/libcsplit.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/fsxfs_test_attributes_leaf_block_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5960 2024-05-01 16:07:46.000000 libfsxfs-20240501/msvscpp/fsxfs_test_attributes_leaf_block_header/fsxfs_test_attributes_leaf_block_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-05-01 16:07:26.000000 libfsxfs-20240501/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24693 2024-05-01 16:29:54.000000 libfsxfs-20240501/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/fsxfs_test_tools_output/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5839 2024-05-01 16:07:46.000000 libfsxfs-20240501/msvscpp/fsxfs_test_tools_output/fsxfs_test_tools_output.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-05-01 16:07:26.000000 libfsxfs-20240501/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-05-01 16:07:26.000000 libfsxfs-20240501/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/fsxfs_test_btree_block/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6159 2024-05-01 16:07:46.000000 libfsxfs-20240501/msvscpp/fsxfs_test_btree_block/fsxfs_test_btree_block.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/msvscpp/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-05-01 16:07:26.000000 libfsxfs-20240501/msvscpp/libfdatetime/libfdatetime.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:54.000000 libfsxfs-20240501/pyfsxfs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1826 2024-05-01 16:06:34.000000 libfsxfs-20240501/pyfsxfs/pyfsxfs_datetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15962 2024-05-01 16:06:34.000000 libfsxfs-20240501/pyfsxfs/pyfsxfs.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1525 2024-05-01 16:06:34.000000 libfsxfs-20240501/pyfsxfs/pyfsxfs_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6952 2024-05-01 16:08:07.000000 libfsxfs-20240501/pyfsxfs/pyfsxfs_file_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8876 2024-05-01 16:06:34.000000 libfsxfs-20240501/pyfsxfs/pyfsxfs_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9546 2024-05-01 16:06:34.000000 libfsxfs-20240501/pyfsxfs/pyfsxfs_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3486 2024-05-01 16:08:07.000000 libfsxfs-20240501/pyfsxfs/pyfsxfs_extended_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-01 16:06:34.000000 libfsxfs-20240501/pyfsxfs/pyfsxfs_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28413 2024-05-01 16:08:07.000000 libfsxfs-20240501/pyfsxfs/pyfsxfs_extended_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24416 2024-05-01 16:08:07.000000 libfsxfs-20240501/pyfsxfs/pyfsxfs_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    71773 2024-05-01 16:08:07.000000 libfsxfs-20240501/pyfsxfs/pyfsxfs_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2033 2024-05-01 16:06:34.000000 libfsxfs-20240501/pyfsxfs/pyfsxfs_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-05-01 16:06:34.000000 libfsxfs-20240501/pyfsxfs/pyfsxfs_libfsxfs.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1311 2024-05-01 16:10:53.000000 libfsxfs-20240501/pyfsxfs/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-01 16:06:34.000000 libfsxfs-20240501/pyfsxfs/pyfsxfs_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9439 2024-05-01 16:06:34.000000 libfsxfs-20240501/pyfsxfs/pyfsxfs_file_entries.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2634 2024-05-01 16:06:34.000000 libfsxfs-20240501/pyfsxfs/pyfsxfs_extended_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1868 2024-05-01 16:06:34.000000 libfsxfs-20240501/pyfsxfs/pyfsxfs.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1540 2024-05-01 16:06:34.000000 libfsxfs-20240501/pyfsxfs/pyfsxfs_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16609 2024-05-01 16:06:34.000000 libfsxfs-20240501/pyfsxfs/pyfsxfs_datetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4118 2024-05-01 16:06:34.000000 libfsxfs-20240501/pyfsxfs/pyfsxfs_file_object_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2736 2024-05-01 16:08:07.000000 libfsxfs-20240501/pyfsxfs/pyfsxfs_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33880 2024-05-01 16:06:34.000000 libfsxfs-20240501/pyfsxfs/pyfsxfs_file_object_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2487 2024-05-01 16:06:34.000000 libfsxfs-20240501/pyfsxfs/pyfsxfs_file_entries.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48484 2024-05-01 16:29:54.000000 libfsxfs-20240501/pyfsxfs/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2024-05-01 16:06:34.000000 libfsxfs-20240501/pyfsxfs/pyfsxfs_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9890 2024-05-01 16:08:07.000000 libfsxfs-20240501/pyfsxfs/pyfsxfs_extended_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       92 2024-05-01 16:06:33.000000 libfsxfs-20240501/AUTHORS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:54.000000 libfsxfs-20240501/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-01 16:29:20.000000 libfsxfs-20240501/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-05-01 16:29:20.000000 libfsxfs-20240501/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-01 16:29:20.000000 libfsxfs-20240501/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-01 16:29:20.000000 libfsxfs-20240501/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-05-01 16:29:20.000000 libfsxfs-20240501/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-05-01 16:29:20.000000 libfsxfs-20240501/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      938 2024-05-01 16:29:20.000000 libfsxfs-20240501/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-01 16:29:20.000000 libfsxfs-20240501/libcfile/libcfile_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-01 16:29:20.000000 libfsxfs-20240501/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-05-01 16:29:20.000000 libfsxfs-20240501/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-01 16:29:20.000000 libfsxfs-20240501/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-01 16:29:20.000000 libfsxfs-20240501/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-01 16:29:20.000000 libfsxfs-20240501/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-01 16:29:20.000000 libfsxfs-20240501/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-05-01 16:29:20.000000 libfsxfs-20240501/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-01 16:29:20.000000 libfsxfs-20240501/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-05-01 16:29:20.000000 libfsxfs-20240501/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31486 2024-05-01 16:29:53.000000 libfsxfs-20240501/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-01 16:29:20.000000 libfsxfs-20240501/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-01 16:29:20.000000 libfsxfs-20240501/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-05-01 16:29:20.000000 libfsxfs-20240501/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-05-01 16:29:20.000000 libfsxfs-20240501/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      435 2024-05-01 16:08:30.000000 libfsxfs-20240501/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-05-01 16:29:53.000000 libfsxfs-20240501/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:53.000000 libfsxfs-20240501/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-05-01 16:29:53.000000 libfsxfs-20240501/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-01 16:29:16.000000 libfsxfs-20240501/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-05-01 16:06:31.000000 libfsxfs-20240501/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      487 2024-05-01 16:06:31.000000 libfsxfs-20240501/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-05-01 16:29:53.000000 libfsxfs-20240501/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-05-01 16:06:31.000000 libfsxfs-20240501/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1508 2024-05-01 16:06:31.000000 libfsxfs-20240501/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:07:43.000000 libfsxfs-20240501/config.rpath
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      705 2024-05-01 16:06:31.000000 libfsxfs-20240501/libfsxfs.pc.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:54.000000 libfsxfs-20240501/libfsxfs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2304 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_btree_block.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3804 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1505 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_extents.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_btree_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32101 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_extended_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11271 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_directory_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1825 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1082 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28204 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_superblock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3464 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_superblock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8038 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_file_system_block_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2036 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1871 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_inode_btree_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_block_directory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6640 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_directory_table_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3159 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34470 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2129 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/fsxfs_block_directory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    99176 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19006 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_block_directory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2146 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1080 2024-05-01 16:30:06.000000 libfsxfs-20240501/libfsxfs/libfsxfs.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2339 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1731 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18245 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_directory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3833 2024-05-01 16:11:09.000000 libfsxfs-20240501/libfsxfs/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3751 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/fsxfs_inode_information.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5405 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_inode.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1971 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_attributes_leaf_block_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7517 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_extents.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9801 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/fsxfs_superblock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18038 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_extent_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7821 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_buffer_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4499 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/fsxfs_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22490 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_inode_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2216 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_file_system_block.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7881 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_extent.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12172 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_inode_information.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12050 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_directory_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4327 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_extent_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15544 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_attribute_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5046 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_extended_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2328 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_buffer_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14356 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10961 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_file_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1805 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_block_directory_footer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7870 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_attributes_leaf_block_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1942 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_directory_table_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_attribute_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1880 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_block_directory_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1979 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_extent.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5811 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3178 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_inode_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_extent_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7475 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_block_directory_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4581 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_block_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44504 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_inode.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5330 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/fsxfs_attributes_block.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1398 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2674 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_extent_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9101 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/fsxfs_inode.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2638 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_directory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9380 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1726 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_block_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/fsxfs_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2013 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_file_system_block_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1889 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_attributes_table_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3157 2024-05-01 16:30:06.000000 libfsxfs-20240501/libfsxfs/libfsxfs_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5700 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_attributes_table_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3060 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_directory_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24809 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_file_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12058 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_attributes_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1867 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_attributes_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1896 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_directory_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2427 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/fsxfs_file_system_block.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5661 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_inode_btree_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55528 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3170 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_file_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45037 2024-05-01 16:29:53.000000 libfsxfs-20240501/libfsxfs/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9681 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_btree_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9365 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_file_system_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2217 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_inode_information.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10957 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_btree_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10984 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_data_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5454 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_block_directory_footer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_data_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2624 2024-05-01 16:06:34.000000 libfsxfs-20240501/libfsxfs/libfsxfs_attributes.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:53.000000 libfsxfs-20240501/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-05-01 16:29:29.000000 libfsxfs-20240501/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-05-01 16:29:29.000000 libfsxfs-20240501/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-05-01 16:29:29.000000 libfsxfs-20240501/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-05-01 16:29:29.000000 libfsxfs-20240501/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-05-01 16:29:29.000000 libfsxfs-20240501/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-05-01 16:29:29.000000 libfsxfs-20240501/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-01 16:29:29.000000 libfsxfs-20240501/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-05-01 16:29:29.000000 libfsxfs-20240501/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-05-01 16:29:29.000000 libfsxfs-20240501/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-05-01 16:29:29.000000 libfsxfs-20240501/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-05-01 16:29:29.000000 libfsxfs-20240501/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-05-01 16:29:29.000000 libfsxfs-20240501/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-05-01 16:29:29.000000 libfsxfs-20240501/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-05-01 16:29:29.000000 libfsxfs-20240501/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-05-01 16:29:29.000000 libfsxfs-20240501/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-05-01 16:29:29.000000 libfsxfs-20240501/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-05-01 16:29:29.000000 libfsxfs-20240501/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-05-01 16:29:29.000000 libfsxfs-20240501/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-05-01 16:29:29.000000 libfsxfs-20240501/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-05-01 16:29:29.000000 libfsxfs-20240501/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-01 16:29:29.000000 libfsxfs-20240501/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-05-01 16:29:29.000000 libfsxfs-20240501/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-05-01 16:29:29.000000 libfsxfs-20240501/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-05-01 16:29:29.000000 libfsxfs-20240501/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-05-01 16:29:29.000000 libfsxfs-20240501/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-05-01 16:29:29.000000 libfsxfs-20240501/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-05-01 16:29:29.000000 libfsxfs-20240501/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33838 2024-05-01 16:29:53.000000 libfsxfs-20240501/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-05-01 16:29:29.000000 libfsxfs-20240501/libcthreads/libcthreads_queue.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-05-01 16:29:54.000000 libfsxfs-20240501/test-driver
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:54.000000 libfsxfs-20240501/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-05-01 16:29:24.000000 libfsxfs-20240501/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-01 16:29:24.000000 libfsxfs-20240501/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-05-01 16:29:24.000000 libfsxfs-20240501/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2024-05-01 16:29:24.000000 libfsxfs-20240501/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-01 16:29:24.000000 libfsxfs-20240501/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-01 16:29:24.000000 libfsxfs-20240501/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-01 16:29:24.000000 libfsxfs-20240501/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-05-01 16:29:24.000000 libfsxfs-20240501/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-05-01 16:29:24.000000 libfsxfs-20240501/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-01 16:29:24.000000 libfsxfs-20240501/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-01 16:29:24.000000 libfsxfs-20240501/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-01 16:29:24.000000 libfsxfs-20240501/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30684 2024-05-01 16:29:53.000000 libfsxfs-20240501/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-01 16:29:24.000000 libfsxfs-20240501/libcpath/libcpath_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-01 16:29:24.000000 libfsxfs-20240501/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-05-01 16:29:24.000000 libfsxfs-20240501/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-05-01 16:29:24.000000 libfsxfs-20240501/libcpath/libcpath_path.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1063 2023-12-03 09:07:43.000000 libfsxfs-20240501/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1888 2024-05-01 16:06:35.000000 libfsxfs-20240501/manuals/fsxfsinfo.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      161 2024-05-01 16:10:37.000000 libfsxfs-20240501/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13196 2024-05-01 16:06:35.000000 libfsxfs-20240501/manuals/libfsxfs.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1414 2024-05-01 16:06:35.000000 libfsxfs-20240501/manuals/fsxfsmount.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27450 2024-05-01 16:29:54.000000 libfsxfs-20240501/manuals/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1709 2024-05-01 16:06:35.000000 libfsxfs-20240501/tests/fsxfs_test_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5706 2024-05-01 16:06:35.000000 libfsxfs-20240501/tests/fsxfs_test_tools_info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11403 2024-05-01 16:07:46.000000 libfsxfs-20240501/tests/fsxfs_test_attributes_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4323 2024-05-01 16:06:35.000000 libfsxfs-20240501/tests/fsxfs_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26898 2024-05-01 16:07:46.000000 libfsxfs-20240501/tests/fsxfs_test_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4700 2024-05-01 16:06:35.000000 libfsxfs-20240501/tests/fsxfs_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-05-01 16:06:35.000000 libfsxfs-20240501/tests/fsxfs_test_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9963 2024-05-01 16:07:46.000000 libfsxfs-20240501/tests/fsxfs_test_block_directory_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-05-01 16:06:35.000000 libfsxfs-20240501/tests/fsxfs_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-05-01 16:06:35.000000 libfsxfs-20240501/tests/fsxfs_test_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11592 2024-05-01 16:07:46.000000 libfsxfs-20240501/tests/fsxfs_test_file_system_block_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6420 2024-05-01 16:07:46.000000 libfsxfs-20240501/tests/fsxfs_test_directory_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8672 2024-05-01 16:08:18.000000 libfsxfs-20240501/tests/pyfsxfs_test_volume.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4045 2024-05-01 16:09:12.000000 libfsxfs-20240501/tests/test_tools.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5952 2024-05-01 16:07:46.000000 libfsxfs-20240501/tests/fsxfs_test_extent.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6196 2024-05-01 16:07:46.000000 libfsxfs-20240501/tests/fsxfs_test_inode_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-05-01 16:06:35.000000 libfsxfs-20240501/tests/fsxfs_test_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15297 2024-05-01 16:07:46.000000 libfsxfs-20240501/tests/fsxfs_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10887 2024-05-01 16:10:24.000000 libfsxfs-20240501/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18310 2024-05-01 16:07:46.000000 libfsxfs-20240501/tests/fsxfs_test_attribute_values.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3317 2024-05-01 16:06:34.000000 libfsxfs-20240501/tests/test_fsxfsinfo.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4169 2024-05-01 16:06:35.000000 libfsxfs-20240501/tests/fsxfs_test_tools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15726 2024-05-01 16:07:46.000000 libfsxfs-20240501/tests/fsxfs_test_functions.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19056 2024-05-01 16:07:46.000000 libfsxfs-20240501/tests/fsxfs_test_inode_information.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11789 2024-05-01 16:07:46.000000 libfsxfs-20240501/tests/fsxfs_test_attributes_leaf_block_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8574 2024-05-01 16:06:35.000000 libfsxfs-20240501/tests/fsxfs_test_macros.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-01 16:06:34.000000 libfsxfs-20240501/tests/test_manpage.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4415 2024-05-01 16:06:34.000000 libfsxfs-20240501/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1997 2024-05-01 16:08:40.000000 libfsxfs-20240501/tests/fsxfs_test_functions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-05-01 16:06:35.000000 libfsxfs-20240501/tests/fsxfs_test_libfsxfs.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9899 2024-05-01 16:07:46.000000 libfsxfs-20240501/tests/fsxfs_test_directory_table_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9978 2024-05-01 16:07:46.000000 libfsxfs-20240501/tests/fsxfs_test_attributes_table_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9911 2024-05-01 16:07:46.000000 libfsxfs-20240501/tests/fsxfs_test_block_directory_footer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2447 2024-05-01 16:06:35.000000 libfsxfs-20240501/tests/fsxfs_test_tools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8185 2024-05-01 16:07:46.000000 libfsxfs-20240501/tests/fsxfs_test_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-05-01 16:06:34.000000 libfsxfs-20240501/tests/fsxfs_test_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-05-01 16:06:34.000000 libfsxfs-20240501/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3139 2024-05-01 16:06:34.000000 libfsxfs-20240501/tests/fsxfs_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-05-01 16:06:34.000000 libfsxfs-20240501/tests/fsxfs_test_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-05-01 16:06:35.000000 libfsxfs-20240501/tests/fsxfs_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3464 2024-05-01 16:08:18.000000 libfsxfs-20240501/tests/pyfsxfs_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2800 2024-05-01 16:06:34.000000 libfsxfs-20240501/tests/fsxfs_test_buffer_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15930 2024-05-01 16:07:46.000000 libfsxfs-20240501/tests/fsxfs_test_superblock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    79067 2024-05-01 16:29:54.000000 libfsxfs-20240501/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9515 2024-05-01 16:07:46.000000 libfsxfs-20240501/tests/fsxfs_test_inode_btree_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10685 2024-05-01 16:07:46.000000 libfsxfs-20240501/tests/fsxfs_test_btree_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18604 2024-05-01 16:07:46.000000 libfsxfs-20240501/tests/fsxfs_test_btree_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-05-01 16:06:35.000000 libfsxfs-20240501/tests/fsxfs_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-01 16:06:35.000000 libfsxfs-20240501/tests/fsxfs_test_unused.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4362 2024-05-01 16:08:57.000000 libfsxfs-20240501/tests/test_library.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2625 2024-05-01 16:06:34.000000 libfsxfs-20240501/ossfuzz/volume_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2020 2024-05-01 16:09:58.000000 libfsxfs-20240501/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-05-01 16:06:34.000000 libfsxfs-20240501/ossfuzz/ossfuzz_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5429 2024-05-01 16:06:34.000000 libfsxfs-20240501/ossfuzz/file_entry_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3320 2024-05-01 16:06:34.000000 libfsxfs-20240501/ossfuzz/extended_attribute_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      972 2024-05-01 16:06:34.000000 libfsxfs-20240501/ossfuzz/ossfuzz_libfsxfs.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36956 2024-05-01 16:29:54.000000 libfsxfs-20240501/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-05-01 16:29:45.000000 libfsxfs-20240501/ltmain.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:54.000000 libfsxfs-20240501/libhmac/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47989 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_sha1_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_sha224.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50026 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_sha512_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14448 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_md5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2079 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_md5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1942 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9362 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14650 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_sha512.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45648 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_sha256_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_sha224.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1623 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2060 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_sha1.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3443 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_sha256_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1117 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45605 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_sha224_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_md5_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_sha256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3368 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_sha1_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33549 2024-05-01 16:29:54.000000 libfsxfs-20240501/libhmac/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_sha256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3461 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_sha224_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3444 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_sha512_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_sha512.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14514 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_sha1.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40596 2024-05-01 16:29:37.000000 libfsxfs-20240501/libhmac/libhmac_md5_context.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:53.000000 libfsxfs-20240501/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-05-01 16:29:28.000000 libfsxfs-20240501/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-05-01 16:29:28.000000 libfsxfs-20240501/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-05-01 16:29:28.000000 libfsxfs-20240501/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-05-01 16:29:28.000000 libfsxfs-20240501/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-01 16:29:28.000000 libfsxfs-20240501/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-05-01 16:29:28.000000 libfsxfs-20240501/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-01 16:29:28.000000 libfsxfs-20240501/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-05-01 16:29:28.000000 libfsxfs-20240501/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-01 16:29:28.000000 libfsxfs-20240501/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-05-01 16:29:28.000000 libfsxfs-20240501/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-01 16:29:28.000000 libfsxfs-20240501/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-05-01 16:29:28.000000 libfsxfs-20240501/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-01 16:29:28.000000 libfsxfs-20240501/libcsplit/libcsplit_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-01 16:29:28.000000 libfsxfs-20240501/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-01 16:29:28.000000 libfsxfs-20240501/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-05-01 16:29:28.000000 libfsxfs-20240501/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31581 2024-05-01 16:29:53.000000 libfsxfs-20240501/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-05-01 16:29:28.000000 libfsxfs-20240501/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-05-01 16:29:28.000000 libfsxfs-20240501/libcsplit/libcsplit_narrow_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:55.000000 libfsxfs-20240501/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:08:00.000000 libfsxfs-20240501/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:08:00.000000 libfsxfs-20240501/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:08:00.000000 libfsxfs-20240501/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:08:00.000000 libfsxfs-20240501/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:08:00.000000 libfsxfs-20240501/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:08:00.000000 libfsxfs-20240501/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:08:00.000000 libfsxfs-20240501/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:08:00.000000 libfsxfs-20240501/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:08:00.000000 libfsxfs-20240501/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1854 2024-05-01 16:30:06.000000 libfsxfs-20240501/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:08:00.000000 libfsxfs-20240501/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:08:00.000000 libfsxfs-20240501/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:53.000000 libfsxfs-20240501/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57165 2024-05-01 16:29:54.000000 libfsxfs-20240501/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-05-01 16:29:40.000000 libfsxfs-20240501/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41405 2024-05-01 16:29:53.000000 libfsxfs-20240501/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:53.000000 libfsxfs-20240501/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-01 16:29:23.000000 libfsxfs-20240501/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-01 16:29:23.000000 libfsxfs-20240501/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-05-01 16:29:23.000000 libfsxfs-20240501/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-05-01 16:29:23.000000 libfsxfs-20240501/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-05-01 16:29:23.000000 libfsxfs-20240501/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-01 16:29:23.000000 libfsxfs-20240501/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-05-01 16:29:23.000000 libfsxfs-20240501/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-05-01 16:29:23.000000 libfsxfs-20240501/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-05-01 16:29:23.000000 libfsxfs-20240501/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-05-01 16:29:23.000000 libfsxfs-20240501/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-05-01 16:29:23.000000 libfsxfs-20240501/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30522 2024-05-01 16:29:53.000000 libfsxfs-20240501/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-01 16:29:23.000000 libfsxfs-20240501/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-05-01 16:29:23.000000 libfsxfs-20240501/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:53.000000 libfsxfs-20240501/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-05-01 16:29:18.000000 libfsxfs-20240501/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-05-01 16:29:18.000000 libfsxfs-20240501/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-01 16:29:18.000000 libfsxfs-20240501/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-05-01 16:29:18.000000 libfsxfs-20240501/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-05-01 16:29:18.000000 libfsxfs-20240501/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-01 16:29:18.000000 libfsxfs-20240501/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-05-01 16:29:18.000000 libfsxfs-20240501/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-05-01 16:29:18.000000 libfsxfs-20240501/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-05-01 16:29:18.000000 libfsxfs-20240501/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-01 16:29:18.000000 libfsxfs-20240501/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-01 16:29:18.000000 libfsxfs-20240501/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29989 2024-05-01 16:29:53.000000 libfsxfs-20240501/libcerror/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 17:05:54.000000 libfsxfs-20240501/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-05-01 16:29:34.000000 libfsxfs-20240501/libfdatetime/libfdatetime_floatingtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-05-01 16:29:34.000000 libfsxfs-20240501/libfdatetime/libfdatetime_nsf_timedate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-05-01 16:29:34.000000 libfsxfs-20240501/libfdatetime/libfdatetime_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-05-01 16:29:34.000000 libfsxfs-20240501/libfdatetime/libfdatetime_floatingtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-05-01 16:29:34.000000 libfsxfs-20240501/libfdatetime/libfdatetime_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-05-01 16:29:34.000000 libfsxfs-20240501/libfdatetime/libfdatetime_hfs_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-05-01 16:29:34.000000 libfsxfs-20240501/libfdatetime/libfdatetime_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-05-01 16:29:34.000000 libfsxfs-20240501/libfdatetime/libfdatetime_hfs_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1144 2024-05-01 16:29:34.000000 libfsxfs-20240501/libfdatetime/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-05-01 16:29:34.000000 libfsxfs-20240501/libfdatetime/libfdatetime_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-05-01 16:29:34.000000 libfsxfs-20240501/libfdatetime/libfdatetime_systemtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-01 16:29:34.000000 libfsxfs-20240501/libfdatetime/libfdatetime_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-05-01 16:29:34.000000 libfsxfs-20240501/libfdatetime/libfdatetime_posix_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-05-01 16:29:34.000000 libfsxfs-20240501/libfdatetime/libfdatetime_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-05-01 16:29:34.000000 libfsxfs-20240501/libfdatetime/libfdatetime_fat_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-05-01 16:29:34.000000 libfsxfs-20240501/libfdatetime/libfdatetime_systemtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-05-01 16:29:34.000000 libfsxfs-20240501/libfdatetime/libfdatetime_nsf_timedate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-05-01 16:29:34.000000 libfsxfs-20240501/libfdatetime/libfdatetime_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-05-01 16:29:34.000000 libfsxfs-20240501/libfdatetime/libfdatetime_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-05-01 16:29:34.000000 libfsxfs-20240501/libfdatetime/libfdatetime_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-05-01 16:29:34.000000 libfsxfs-20240501/libfdatetime/libfdatetime_posix_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-05-01 16:29:34.000000 libfsxfs-20240501/libfdatetime/libfdatetime_date_time_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-05-01 16:29:34.000000 libfsxfs-20240501/libfdatetime/libfdatetime_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-05-01 16:29:34.000000 libfsxfs-20240501/libfdatetime/libfdatetime_date_time_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-05-01 16:29:34.000000 libfsxfs-20240501/libfdatetime/libfdatetime_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33573 2024-05-01 16:29:53.000000 libfsxfs-20240501/libfdatetime/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-05-01 16:29:34.000000 libfsxfs-20240501/libfdatetime/libfdatetime_fat_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56884 2024-05-01 16:29:49.000000 libfsxfs-20240501/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8065 2024-05-01 16:06:31.000000 libfsxfs-20240501/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      418 2024-05-01 17:05:56.064075 libfsxfs-20240501/PKG-INFO
```

### Comparing `libfsxfs-20240222/libfdata/libfdata_error.h` & `libfsxfs-20240501/libfdata/libfdata_error.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_area.c` & `libfsxfs-20240501/libfdata/libfdata_area.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_stream.h` & `libfsxfs-20240501/libfdata/libfdata_stream.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_cache.h` & `libfsxfs-20240501/libfdata/libfdata_cache.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_range_list.c` & `libfsxfs-20240501/libfdata/libfdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_mapped_range.c` & `libfsxfs-20240501/libfdata/libfdata_mapped_range.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_libcerror.h` & `libfsxfs-20240501/libfdata/libfdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_definitions.h` & `libfsxfs-20240501/libfdata/libfdata_definitions.h`

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

### Comparing `libfsxfs-20240222/libfdata/libfdata_list.c` & `libfsxfs-20240501/libfdata/libfdata_list.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_libcdata.h` & `libfsxfs-20240501/libfdata/libfdata_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_list.h` & `libfsxfs-20240501/libfdata/libfdata_list.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_list_element.h` & `libfsxfs-20240501/libfdata/libfdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/Makefile.am` & `libfsxfs-20240501/libfdata/Makefile.am`

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

### Comparing `libfsxfs-20240222/libfdata/libfdata_libcnotify.h` & `libfsxfs-20240501/libfdata/libfdata_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_extern.h` & `libfsxfs-20240501/libfdata/libfdata_extern.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_notify.c` & `libfsxfs-20240501/libfdata/libfdata_notify.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_cache.c` & `libfsxfs-20240501/libfdata/libfdata_cache.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_stream.c` & `libfsxfs-20240501/libfdata/libfdata_stream.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_unused.h` & `libfsxfs-20240501/libfdata/libfdata_unused.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_range.h` & `libfsxfs-20240501/libfdata/libfdata_range.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_area.h` & `libfsxfs-20240501/libfdata/libfdata_area.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_error.c` & `libfsxfs-20240501/libfdata/libfdata_error.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_support.h` & `libfsxfs-20240501/libfdata/libfdata_support.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_range.c` & `libfsxfs-20240501/libfdata/libfdata_range.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_mapped_range.h` & `libfsxfs-20240501/libfdata/libfdata_mapped_range.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_support.c` & `libfsxfs-20240501/libfdata/libfdata_support.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_list_element.c` & `libfsxfs-20240501/libfdata/libfdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_segments_array.c` & `libfsxfs-20240501/libfdata/libfdata_segments_array.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_types.h` & `libfsxfs-20240501/libfdata/libfdata_types.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_notify.h` & `libfsxfs-20240501/libfdata/libfdata_notify.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_range_list.h` & `libfsxfs-20240501/libfdata/libfdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_segments_array.h` & `libfsxfs-20240501/libfdata/libfdata_segments_array.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/Makefile.in` & `libfsxfs-20240501/libfdata/Makefile.in`

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

### Comparing `libfsxfs-20240222/libfdata/libfdata_vector.c` & `libfsxfs-20240501/libfdata/libfdata_vector.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_libfcache.h` & `libfsxfs-20240501/libfdata/libfdata_libfcache.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdata/libfdata_vector.h` & `libfsxfs-20240501/libfdata/libfdata_vector.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/fsxfstools_libuna.h` & `libfsxfs-20240501/fsxfstools/fsxfstools_libuna.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/fsxfstools_getopt.h` & `libfsxfs-20240501/fsxfstools/fsxfstools_getopt.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/mount_dokan.c` & `libfsxfs-20240501/fsxfstools/mount_dokan.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/mount_file_system.h` & `libfsxfs-20240501/fsxfstools/mount_file_system.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/fsxfstools_libfcache.h` & `libfsxfs-20240501/fsxfstools/fsxfstools_libfcache.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/fsxfstools_output.c` & `libfsxfs-20240501/fsxfstools/fsxfstools_output.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/mount_fuse.c` & `libfsxfs-20240501/fsxfstools/mount_fuse.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/fsxfstools_output.h` & `libfsxfs-20240501/fsxfstools/fsxfstools_output.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/info_handle.h` & `libfsxfs-20240501/fsxfstools/info_handle.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/mount_dokan.h` & `libfsxfs-20240501/fsxfstools/mount_dokan.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/fsxfstools_libfdatetime.h` & `libfsxfs-20240501/fsxfstools/fsxfstools_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/digest_hash.c` & `libfsxfs-20240501/fsxfstools/digest_hash.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/mount_file_system.c` & `libfsxfs-20240501/fsxfstools/mount_file_system.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/fsxfstools_libcpath.h` & `libfsxfs-20240501/fsxfstools/fsxfstools_libcpath.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/fsxfstools_unused.h` & `libfsxfs-20240501/fsxfstools/fsxfstools_unused.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/Makefile.am` & `libfsxfs-20240501/fsxfstools/Makefile.am`

 * *Files 1% similar despite different names*

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
@@ -94,17 +94,15 @@
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libfsxfs/libfsxfs.la \
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
 	@echo "Running splint on fsxfsinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(fsxfsinfo_SOURCES)
```

### Comparing `libfsxfs-20240222/fsxfstools/fsxfstools_libfsxfs.h` & `libfsxfs-20240501/fsxfstools/fsxfstools_libfsxfs.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/fsxfsinfo.c` & `libfsxfs-20240501/fsxfstools/fsxfsinfo.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/mount_file_entry.c` & `libfsxfs-20240501/fsxfstools/mount_file_entry.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/info_handle.c` & `libfsxfs-20240501/fsxfstools/info_handle.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/mount_file_entry.h` & `libfsxfs-20240501/fsxfstools/mount_file_entry.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/fsxfstools_signal.h` & `libfsxfs-20240501/fsxfstools/fsxfstools_signal.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/fsxfstools_libhmac.h` & `libfsxfs-20240501/fsxfstools/fsxfstools_libhmac.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/fsxfstools_i18n.h` & `libfsxfs-20240501/fsxfstools/fsxfstools_i18n.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/fsxfstools_libclocale.h` & `libfsxfs-20240501/fsxfstools/fsxfstools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/fsxfstools_libbfio.h` & `libfsxfs-20240501/fsxfstools/fsxfstools_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/mount_handle.h` & `libfsxfs-20240501/fsxfstools/mount_handle.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/fsxfstools_libcerror.h` & `libfsxfs-20240501/fsxfstools/fsxfstools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/fsxfstools_libcnotify.h` & `libfsxfs-20240501/fsxfstools/fsxfstools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/fsxfstools_signal.c` & `libfsxfs-20240501/fsxfstools/fsxfstools_signal.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/mount_handle.c` & `libfsxfs-20240501/fsxfstools/mount_handle.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/fsxfsmount.c` & `libfsxfs-20240501/fsxfstools/fsxfsmount.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/Makefile.in` & `libfsxfs-20240501/fsxfstools/Makefile.in`

 * *Files 1% similar despite different names*

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
@@ -631,15 +633,16 @@
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libfsxfs/libfsxfs.la \
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
@@ -896,23 +899,37 @@
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
+	-rm -f ./$(DEPDIR)/fsxfsinfo.Po
+	-rm -f ./$(DEPDIR)/fsxfsmount.Po
+	-rm -f ./$(DEPDIR)/fsxfstools_getopt.Po
+	-rm -f ./$(DEPDIR)/fsxfstools_output.Po
+	-rm -f ./$(DEPDIR)/fsxfstools_signal.Po
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
 
@@ -1007,17 +1024,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on fsxfsinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(fsxfsinfo_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfsxfs-20240222/fsxfstools/fsxfstools_getopt.c` & `libfsxfs-20240501/fsxfstools/fsxfstools_getopt.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/digest_hash.h` & `libfsxfs-20240501/fsxfstools/digest_hash.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/mount_fuse.h` & `libfsxfs-20240501/fsxfstools/mount_fuse.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/fsxfstools/fsxfstools_libfdata.h` & `libfsxfs-20240501/fsxfstools/fsxfstools_libfdata.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/COPYING` & `libfsxfs-20240501/COPYING`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/install-sh` & `libfsxfs-20240501/install-sh`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/depcomp` & `libfsxfs-20240501/depcomp`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfguid/libfguid_error.c` & `libfsxfs-20240501/libfguid/libfguid_error.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfguid/libfguid_support.h` & `libfsxfs-20240501/libfguid/libfguid_support.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfguid/libfguid_identifier.h` & `libfsxfs-20240501/libfguid/libfguid_identifier.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfguid/libfguid_libcerror.h` & `libfsxfs-20240501/libfguid/libfguid_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfguid/Makefile.am` & `libfsxfs-20240501/libfguid/Makefile.am`

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

### Comparing `libfsxfs-20240222/libfguid/libfguid_unused.h` & `libfsxfs-20240501/libfguid/libfguid_unused.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfguid/libfguid_extern.h` & `libfsxfs-20240501/libfguid/libfguid_extern.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfguid/libfguid_types.h` & `libfsxfs-20240501/libfguid/libfguid_types.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfguid/libfguid_identifier.c` & `libfsxfs-20240501/libfguid/libfguid_identifier.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfguid/libfguid_support.c` & `libfsxfs-20240501/libfguid/libfguid_support.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfguid/libfguid_definitions.h` & `libfsxfs-20240501/libfguid/libfguid_definitions.h`

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

### Comparing `libfsxfs-20240222/libfguid/Makefile.in` & `libfsxfs-20240501/libfguid/Makefile.in`

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

### Comparing `libfsxfs-20240222/libfguid/libfguid_error.h` & `libfsxfs-20240501/libfguid/libfguid_error.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs.spec.in` & `libfsxfs-20240501/libfsxfs.spec.in`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/m4/libcfile.m4` & `libfsxfs-20240501/m4/libcfile.m4`

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

### Comparing `libfsxfs-20240222/m4/libfdatetime.m4` & `libfsxfs-20240501/m4/libfdatetime.m4`

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

### Comparing `libfsxfs-20240222/m4/tests.m4` & `libfsxfs-20240501/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/m4/libcpath.m4` & `libfsxfs-20240501/m4/libcpath.m4`

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

### Comparing `libfsxfs-20240222/m4/lib-prefix.m4` & `libfsxfs-20240501/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/m4/progtest.m4` & `libfsxfs-20240501/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/m4/libuna.m4` & `libfsxfs-20240501/m4/libuna.m4`

 * *Files 2% similar despite different names*

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
@@ -938,16 +940,17 @@
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
@@ -969,15 +972,15 @@
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

### Comparing `libfsxfs-20240222/m4/gettext.m4` & `libfsxfs-20240501/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/m4/lib-ld.m4` & `libfsxfs-20240501/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/m4/libclocale.m4` & `libfsxfs-20240501/m4/libclocale.m4`

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

### Comparing `libfsxfs-20240222/m4/libcdata.m4` & `libfsxfs-20240501/m4/libcdata.m4`

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

### Comparing `libfsxfs-20240222/m4/libcsplit.m4` & `libfsxfs-20240501/m4/libcsplit.m4`

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

### Comparing `libfsxfs-20240222/m4/common.m4` & `libfsxfs-20240501/m4/common.m4`

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

### Comparing `libfsxfs-20240222/m4/libcthreads.m4` & `libfsxfs-20240501/m4/libcthreads.m4`

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

### Comparing `libfsxfs-20240222/m4/ltversion.m4` & `libfsxfs-20240501/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/m4/ltsugar.m4` & `libfsxfs-20240501/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/m4/libfdata.m4` & `libfsxfs-20240501/m4/libfdata.m4`

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

### Comparing `libfsxfs-20240222/m4/host-cpu-c-abi.m4` & `libfsxfs-20240501/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/m4/libfuse.m4` & `libfsxfs-20240501/m4/libfuse.m4`

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

### Comparing `libfsxfs-20240222/m4/libtool.m4` & `libfsxfs-20240501/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/m4/po.m4` & `libfsxfs-20240501/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/m4/libcerror.m4` & `libfsxfs-20240501/m4/libcerror.m4`

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

### Comparing `libfsxfs-20240222/m4/libcnotify.m4` & `libfsxfs-20240501/m4/libcnotify.m4`

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

### Comparing `libfsxfs-20240222/m4/libfguid.m4` & `libfsxfs-20240501/m4/libfguid.m4`

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

### Comparing `libfsxfs-20240222/m4/libbfio.m4` & `libfsxfs-20240501/m4/libbfio.m4`

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

### Comparing `libfsxfs-20240222/m4/libhmac.m4` & `libfsxfs-20240501/m4/libhmac.m4`

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

### Comparing `libfsxfs-20240222/m4/intlmacosx.m4` & `libfsxfs-20240501/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/m4/lt~obsolete.m4` & `libfsxfs-20240501/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/m4/lib-link.m4` & `libfsxfs-20240501/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/m4/iconv.m4` & `libfsxfs-20240501/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/m4/ltoptions.m4` & `libfsxfs-20240501/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/m4/nls.m4` & `libfsxfs-20240501/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/m4/python.m4` & `libfsxfs-20240501/m4/python.m4`

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

### Comparing `libfsxfs-20240222/m4/libcrypto.m4` & `libfsxfs-20240501/m4/libcrypto.m4`

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

### Comparing `libfsxfs-20240222/m4/types.m4` & `libfsxfs-20240501/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/m4/libfcache.m4` & `libfsxfs-20240501/m4/libfcache.m4`

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

### Comparing `libfsxfs-20240222/m4/pthread.m4` & `libfsxfs-20240501/m4/pthread.m4`

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

### Comparing `libfsxfs-20240222/include/libfsxfs/definitions.h.in` & `libfsxfs-20240501/include/libfsxfs/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/include/libfsxfs/definitions.h` & `libfsxfs-20240501/include/libfsxfs/definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBFSXFS_DEFINITIONS_H )
 #define _LIBFSXFS_DEFINITIONS_H
 
 #include <libfsxfs/types.h>
 
-#define LIBFSXFS_VERSION			20240222
+#define LIBFSXFS_VERSION			20240501
 
 /* The version string
  */
-#define LIBFSXFS_VERSION_STRING			"20240222"
+#define LIBFSXFS_VERSION_STRING			"20240501"
 
 /* The file access
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBFSXFS_ACCESS_FLAGS
```

### Comparing `libfsxfs-20240222/include/libfsxfs/types.h.in` & `libfsxfs-20240501/include/libfsxfs/types.h.in`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/include/libfsxfs/types.h` & `libfsxfs-20240501/include/libfsxfs/types.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/include/libfsxfs/features.h.in` & `libfsxfs-20240501/include/libfsxfs/features.h.in`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/include/libfsxfs/error.h` & `libfsxfs-20240501/include/libfsxfs/error.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/include/libfsxfs/extern.h` & `libfsxfs-20240501/include/libfsxfs/extern.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/include/libfsxfs/features.h` & `libfsxfs-20240501/include/libfsxfs/features.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/include/libfsxfs/codepage.h` & `libfsxfs-20240501/include/libfsxfs/codepage.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/include/Makefile.in` & `libfsxfs-20240501/include/Makefile.in`

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
 	libfsxfs.h.in \
 	libfsxfs/definitions.h.in \
 	libfsxfs/features.h.in \
 	libfsxfs/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfsxfs.h \
+	libfsxfs/definitions.h \
+	libfsxfs/features.h \
+	libfsxfs/types.h \
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
-	-rm -f libfsxfs.h
-	-rm -f libfsxfs/definitions.h
-	-rm -f libfsxfs/features.h
-	-rm -f libfsxfs/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfsxfs-20240222/include/libfsxfs.h.in` & `libfsxfs-20240501/include/libfsxfs.h.in`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/include/libfsxfs.h` & `libfsxfs-20240501/include/libfsxfs.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/common/config_borlandc.h` & `libfsxfs-20240501/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/common/file_stream.h` & `libfsxfs-20240501/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/common/memory.h` & `libfsxfs-20240501/common/memory.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/common/byte_stream.h` & `libfsxfs-20240501/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/common/common.h` & `libfsxfs-20240501/common/common.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/common/config_winapi.h` & `libfsxfs-20240501/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/common/system_string.h` & `libfsxfs-20240501/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/common/types.h.in` & `libfsxfs-20240501/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/common/types.h` & `libfsxfs-20240501/common/types.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/common/config.h.in` & `libfsxfs-20240501/common/config.h.in`

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

### Comparing `libfsxfs-20240222/common/config.h` & `libfsxfs-20240501/common/config.h`

 * *Files 1% similar despite different names*

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
 #define PACKAGE_NAME "libfsxfs"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libfsxfs 20240222"
+#define PACKAGE_STRING "libfsxfs 20240501"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libfsxfs"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240222"
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
-#define VERSION "20240222"
+#define VERSION "20240501"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libfsxfs-20240222/common/wide_string.h` & `libfsxfs-20240501/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/common/narrow_string.h` & `libfsxfs-20240501/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/common/config_msc.h` & `libfsxfs-20240501/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/common/Makefile.in` & `libfsxfs-20240501/common/Makefile.in`

 * *Files 1% similar despite different names*

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

### Comparing `libfsxfs-20240222/libclocale/libclocale_wide_string.c` & `libfsxfs-20240501/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libclocale/libclocale_support.h` & `libfsxfs-20240501/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libclocale/Makefile.am` & `libfsxfs-20240501/libclocale/Makefile.am`

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

### Comparing `libfsxfs-20240222/libclocale/libclocale_definitions.h` & `libfsxfs-20240501/libclocale/libclocale_definitions.h`

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

### Comparing `libfsxfs-20240222/libclocale/libclocale_unused.h` & `libfsxfs-20240501/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libclocale/libclocale_libcerror.h` & `libfsxfs-20240501/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libclocale/libclocale_locale.h` & `libfsxfs-20240501/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libclocale/libclocale_support.c` & `libfsxfs-20240501/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libclocale/libclocale_codepage.c` & `libfsxfs-20240501/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libclocale/libclocale_locale.c` & `libfsxfs-20240501/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libclocale/Makefile.in` & `libfsxfs-20240501/libclocale/Makefile.in`

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

### Comparing `libfsxfs-20240222/libclocale/libclocale_extern.h` & `libfsxfs-20240501/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libclocale/libclocale_wide_string.h` & `libfsxfs-20240501/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libclocale/libclocale_codepage.h` & `libfsxfs-20240501/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfcache/libfcache_libcdata.h` & `libfsxfs-20240501/libfcache/libfcache_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfcache/libfcache_types.h` & `libfsxfs-20240501/libfcache/libfcache_types.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfcache/libfcache_cache_value.c` & `libfsxfs-20240501/libfcache/libfcache_cache_value.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfcache/libfcache_unused.h` & `libfsxfs-20240501/libfcache/libfcache_unused.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfcache/Makefile.am` & `libfsxfs-20240501/libfcache/Makefile.am`

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

### Comparing `libfsxfs-20240222/libfcache/libfcache_support.h` & `libfsxfs-20240501/libfcache/libfcache_support.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfcache/libfcache_error.h` & `libfsxfs-20240501/libfcache/libfcache_error.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfcache/libfcache_support.c` & `libfsxfs-20240501/libfcache/libfcache_support.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfcache/libfcache_cache.h` & `libfsxfs-20240501/libfcache/libfcache_cache.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfcache/libfcache_error.c` & `libfsxfs-20240501/libfcache/libfcache_error.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfcache/libfcache_libcerror.h` & `libfsxfs-20240501/libfcache/libfcache_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfcache/libfcache_date_time.c` & `libfsxfs-20240501/libfcache/libfcache_date_time.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfcache/libfcache_extern.h` & `libfsxfs-20240501/libfcache/libfcache_extern.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfcache/libfcache_cache_value.h` & `libfsxfs-20240501/libfcache/libfcache_cache_value.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfcache/Makefile.in` & `libfsxfs-20240501/libfcache/Makefile.in`

 * *Files 1% similar despite different names*

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

### Comparing `libfsxfs-20240222/libfcache/libfcache_date_time.h` & `libfsxfs-20240501/libfcache/libfcache_date_time.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfcache/libfcache_definitions.h` & `libfsxfs-20240501/libfcache/libfcache_definitions.h`

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

### Comparing `libfsxfs-20240222/libfcache/libfcache_cache.c` & `libfsxfs-20240501/libfcache/libfcache_cache.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/Makefile.am` & `libfsxfs-20240501/Makefile.am`

 * *Files 18% similar despite different names*

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
+	libfsxfs.pc \
+	libfsxfs.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 
 pkgconfig_DATA = \
 	libfsxfs.pc
 
 libtool: @LIBTOOL_DEPS@
@@ -92,19 +99,7 @@
 	(cd $(srcdir)/libfcache && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdata && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdatetime && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfguid && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfsxfs && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libfsxfs.pc
-	-rm -f libfsxfs.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
```

### Comparing `libfsxfs-20240222/libbfio/libbfio_file_range.h` & `libfsxfs-20240501/libbfio/libbfio_file_range.h`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_file_range_io_handle.c` & `libfsxfs-20240501/libbfio/libbfio_file_range_io_handle.c`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_support.c` & `libfsxfs-20240501/libbfio/libbfio_support.c`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_libcpath.h` & `libfsxfs-20240501/libbfio/libbfio_libcpath.h`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_error.h` & `libfsxfs-20240501/libbfio/libbfio_error.h`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_libclocale.h` & `libfsxfs-20240501/libbfio/libbfio_libclocale.h`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_error.c` & `libfsxfs-20240501/libbfio/libbfio_error.c`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_libuna.h` & `libfsxfs-20240501/libbfio/libbfio_libuna.h`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_file_io_handle.h` & `libfsxfs-20240501/libbfio/libbfio_file_io_handle.h`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_file_pool.h` & `libfsxfs-20240501/libbfio/libbfio_file_pool.h`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_file_range.c` & `libfsxfs-20240501/libbfio/libbfio_file_range.c`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_types.h` & `libfsxfs-20240501/libbfio/libbfio_types.h`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_unused.h` & `libfsxfs-20240501/libbfio/libbfio_unused.h`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_libcdata.h` & `libfsxfs-20240501/libbfio/libbfio_libcdata.h`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_file.h` & `libfsxfs-20240501/libbfio/libbfio_file.h`

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

### Comparing `libfsxfs-20240222/libbfio/Makefile.am` & `libfsxfs-20240501/libbfio/Makefile.am`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_libcfile.h` & `libfsxfs-20240501/libbfio/libbfio_libcfile.h`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_definitions.h` & `libfsxfs-20240501/libbfio/libbfio_definitions.h`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_codepage.h` & `libfsxfs-20240501/libbfio/libbfio_codepage.h`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_file_io_handle.c` & `libfsxfs-20240501/libbfio/libbfio_file_io_handle.c`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_support.h` & `libfsxfs-20240501/libbfio/libbfio_support.h`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_memory_range.h` & `libfsxfs-20240501/libbfio/libbfio_memory_range.h`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_file_pool.c` & `libfsxfs-20240501/libbfio/libbfio_file_pool.c`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_file_range_io_handle.h` & `libfsxfs-20240501/libbfio/libbfio_file_range_io_handle.h`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_libcthreads.h` & `libfsxfs-20240501/libbfio/libbfio_libcthreads.h`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_system_string.h` & `libfsxfs-20240501/libbfio/libbfio_system_string.h`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_memory_range_io_handle.c` & `libfsxfs-20240501/libbfio/libbfio_memory_range_io_handle.c`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_handle.c` & `libfsxfs-20240501/libbfio/libbfio_handle.c`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_file.c` & `libfsxfs-20240501/libbfio/libbfio_file.c`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_handle.h` & `libfsxfs-20240501/libbfio/libbfio_handle.h`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_memory_range.c` & `libfsxfs-20240501/libbfio/libbfio_memory_range.c`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_pool.c` & `libfsxfs-20240501/libbfio/libbfio_pool.c`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_libcerror.h` & `libfsxfs-20240501/libbfio/libbfio_libcerror.h`

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

### Comparing `libfsxfs-20240222/libbfio/Makefile.in` & `libfsxfs-20240501/libbfio/Makefile.in`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_system_string.c` & `libfsxfs-20240501/libbfio/libbfio_system_string.c`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_memory_range_io_handle.h` & `libfsxfs-20240501/libbfio/libbfio_memory_range_io_handle.h`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_extern.h` & `libfsxfs-20240501/libbfio/libbfio_extern.h`

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

### Comparing `libfsxfs-20240222/libbfio/libbfio_pool.h` & `libfsxfs-20240501/libbfio/libbfio_pool.h`

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

### Comparing `libfsxfs-20240222/config.guess` & `libfsxfs-20240501/config.guess`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/dpkg/copyright` & `libfsxfs-20240501/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/dpkg/control` & `libfsxfs-20240501/dpkg/control`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/dpkg/rules` & `libfsxfs-20240501/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/COPYING.LESSER` & `libfsxfs-20240501/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/configure` & `libfsxfs-20240501/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libfsxfs 20240222.
+# Generated by GNU Autoconf 2.71 for libfsxfs 20240501.
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
 PACKAGE_NAME='libfsxfs'
 PACKAGE_TARNAME='libfsxfs'
-PACKAGE_VERSION='20240222'
-PACKAGE_STRING='libfsxfs 20240222'
+PACKAGE_VERSION='20240501'
+PACKAGE_STRING='libfsxfs 20240501'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libfsxfs.h.in"
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
-\`configure' configures libfsxfs 20240222 to adapt to many kinds of systems.
+\`configure' configures libfsxfs 20240501 to adapt to many kinds of systems.
 
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
-     short | recursive ) echo "Configuration of libfsxfs 20240222:";;
+     short | recursive ) echo "Configuration of libfsxfs 20240501:";;
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
-libfsxfs configure 20240222
+libfsxfs configure 20240501
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
 
-It was created by libfsxfs $as_me 20240222, which was
+It was created by libfsxfs $as_me 20240501, which was
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
  PACKAGE='libfsxfs'
- VERSION='20240222'
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
@@ -40547,15 +40573,16 @@
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
@@ -40580,15 +40607,15 @@
 
 fi
 
 
     if test "x$ac_cv_libuna" != xyes
 then :
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBUNA 1" >>confdefs.h
@@ -40658,15 +40685,15 @@
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
@@ -41847,15 +41874,16 @@
 
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
@@ -42169,15 +42197,15 @@
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
@@ -42247,15 +42275,15 @@
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
@@ -43052,15 +43080,16 @@
 
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
@@ -43250,15 +43279,15 @@
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: mkdir
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCPATH 1" >>confdefs.h
@@ -43328,15 +43357,15 @@
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
@@ -45446,15 +45475,16 @@
 
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
@@ -45479,15 +45509,15 @@
 
 fi
 
 
     if test "x$ac_cv_libbfio" != xyes
 then :
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBBFIO 1" >>confdefs.h
@@ -45557,15 +45587,15 @@
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
@@ -46477,15 +46507,16 @@
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
@@ -46578,15 +46609,15 @@
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
@@ -46656,15 +46687,15 @@
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
@@ -49944,15 +49975,16 @@
 
 
 
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
@@ -49977,15 +50009,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdata" != xyes
 then :
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATA 1" >>confdefs.h
@@ -50055,15 +50087,15 @@
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
@@ -53499,15 +53531,16 @@
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
@@ -53532,15 +53565,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdatetime" != xyes
 then :
 
-  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime";
+  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime -I\$(top_srcdir)/libfdatetime";
   ac_cv_libfdatetime_LIBADD="../libfdatetime/libfdatetime.la";
 
   ac_cv_libfdatetime=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATETIME 1" >>confdefs.h
@@ -53610,15 +53643,15 @@
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
@@ -54192,15 +54225,16 @@
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
@@ -54225,15 +54259,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfguid" != xyes
 then :
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFGUID 1" >>confdefs.h
@@ -54544,16 +54578,20 @@
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
 
@@ -54716,15 +54754,15 @@
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
@@ -55722,15 +55760,16 @@
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
@@ -55836,15 +55875,15 @@
 
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
@@ -60022,15 +60061,15 @@
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
@@ -60095,33 +60134,107 @@
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
+
+pkg_failed=no
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse3 >= 3.0" >&5
+printf %s "checking for fuse3 >= 3.0... " >&6; }
 
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
@@ -60189,51 +60302,110 @@
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
@@ -60396,45 +60568,38 @@
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
@@ -60602,29 +60767,49 @@
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
@@ -60655,14 +60840,20 @@
 
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
 
@@ -60670,14 +60861,22 @@
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
 
@@ -61603,15 +61802,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libfsxfs $as_me 20240222, which was
+This file was extended by libfsxfs $as_me 20240501, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -61671,15 +61870,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libfsxfs config.status 20240222
+libfsxfs config.status 20240501
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libfsxfs-20240222/libfsxfs.spec` & `libfsxfs-20240501/libfsxfs.spec`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libfsxfs
-Version: 20240222
+Version: 20240501
 Release: 1
 Summary: Library to support the X File System (XFS) format
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libfsxfs
               
@@ -36,16 +36,16 @@
 
 %description -n libfsxfs-python3
 Python 3 bindings for libfsxfs
 
 %package -n libfsxfs-tools
 Summary: Several tools for reading X File System (XFS) volumes
 Group: Applications/System
-Requires: libfsxfs = %{version}-%{release} openssl fuse-libs 
-BuildRequires: openssl-devel fuse-devel 
+Requires: libfsxfs = %{version}-%{release} openssl fuse3-libs 
+BuildRequires: openssl-devel fuse3-devel 
 
 %description -n libfsxfs-tools
 Several tools for reading X File System (XFS) volumes
 
 %prep
 %setup -q
 
@@ -91,10 +91,10 @@
 %files -n libfsxfs-tools
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Thu Feb 22 2024 Joachim Metz <joachim.metz@gmail.com> 20240222-1
+* Wed May  1 2024 Joachim Metz <joachim.metz@gmail.com> 20240501-1
 - Auto-generated
```

### Comparing `libfsxfs-20240222/compile` & `libfsxfs-20240501/compile`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/missing` & `libfsxfs-20240501/missing`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/libfdata/libfdata.vcproj` & `libfsxfs-20240501/msvscpp/libfdata/libfdata.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/fsxfsinfo/fsxfsinfo.vcproj` & `libfsxfs-20240501/msvscpp/fsxfsinfo/fsxfsinfo.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/fsxfs_test_error/fsxfs_test_error.vcproj` & `libfsxfs-20240501/msvscpp/fsxfs_test_error/fsxfs_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/fsxfs_test_tools_info_handle/fsxfs_test_tools_info_handle.vcproj` & `libfsxfs-20240501/msvscpp/fsxfs_test_tools_info_handle/fsxfs_test_tools_info_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/fsxfs_test_extent/fsxfs_test_extent.vcproj` & `libfsxfs-20240501/msvscpp/fsxfs_test_extent/fsxfs_test_extent.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/libfsxfs.sln` & `libfsxfs-20240501/msvscpp/libfsxfs.sln`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/fsxfs_test_file_system_block_header/fsxfs_test_file_system_block_header.vcproj` & `libfsxfs-20240501/msvscpp/fsxfs_test_file_system_block_header/fsxfs_test_file_system_block_header.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/fsxfsmount/fsxfsmount.vcproj` & `libfsxfs-20240501/msvscpp/fsxfsmount/fsxfsmount.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/libfguid/libfguid.vcproj` & `libfsxfs-20240501/msvscpp/libfguid/libfguid.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/fsxfs_test_inode_btree_record/fsxfs_test_inode_btree_record.vcproj` & `libfsxfs-20240501/msvscpp/fsxfs_test_inode_btree_record/fsxfs_test_inode_btree_record.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/fsxfs_test_directory_entry/fsxfs_test_directory_entry.vcproj` & `libfsxfs-20240501/msvscpp/fsxfs_test_directory_entry/fsxfs_test_directory_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/fsxfs_test_directory_table_header/fsxfs_test_directory_table_header.vcproj` & `libfsxfs-20240501/msvscpp/fsxfs_test_directory_table_header/fsxfs_test_directory_table_header.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/libclocale/libclocale.vcproj` & `libfsxfs-20240501/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/fsxfs_test_support/fsxfs_test_support.vcproj` & `libfsxfs-20240501/msvscpp/fsxfs_test_support/fsxfs_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/libfcache/libfcache.vcproj` & `libfsxfs-20240501/msvscpp/libfcache/libfcache.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/Makefile.am` & `libfsxfs-20240501/msvscpp/Makefile.am`

 * *Files 3% similar despite different names*

```diff
@@ -44,13 +44,11 @@
 	libuna/libuna.vcproj \
 	pyfsxfs/pyfsxfs.vcproj \
 	libfsxfs.sln
 
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

### Comparing `libfsxfs-20240222/msvscpp/libbfio/libbfio.vcproj` & `libfsxfs-20240501/msvscpp/libbfio/libbfio.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/fsxfs_test_block_directory_footer/fsxfs_test_block_directory_footer.vcproj` & `libfsxfs-20240501/msvscpp/fsxfs_test_block_directory_footer/fsxfs_test_block_directory_footer.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/fsxfs_test_io_handle/fsxfs_test_io_handle.vcproj` & `libfsxfs-20240501/msvscpp/fsxfs_test_io_handle/fsxfs_test_io_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/pyfsxfs/pyfsxfs.vcproj` & `libfsxfs-20240501/msvscpp/pyfsxfs/pyfsxfs.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/libcfile/libcfile.vcproj` & `libfsxfs-20240501/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/fsxfs_test_block_directory_header/fsxfs_test_block_directory_header.vcproj` & `libfsxfs-20240501/msvscpp/fsxfs_test_block_directory_header/fsxfs_test_block_directory_header.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/fsxfs_test_attributes_table/fsxfs_test_attributes_table.vcproj` & `libfsxfs-20240501/msvscpp/fsxfs_test_attributes_table/fsxfs_test_attributes_table.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/libcdata/libcdata.vcproj` & `libfsxfs-20240501/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/fsxfs_test_inode_information/fsxfs_test_inode_information.vcproj` & `libfsxfs-20240501/msvscpp/fsxfs_test_inode_information/fsxfs_test_inode_information.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/fsxfs_test_superblock/fsxfs_test_superblock.vcproj` & `libfsxfs-20240501/msvscpp/fsxfs_test_superblock/fsxfs_test_superblock.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/fsxfs_test_buffer_data_handle/fsxfs_test_buffer_data_handle.vcproj` & `libfsxfs-20240501/msvscpp/fsxfs_test_buffer_data_handle/fsxfs_test_buffer_data_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/fsxfs_test_btree_header/fsxfs_test_btree_header.vcproj` & `libfsxfs-20240501/msvscpp/fsxfs_test_btree_header/fsxfs_test_btree_header.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/libfsxfs/libfsxfs.vcproj` & `libfsxfs-20240501/msvscpp/libfsxfs/libfsxfs.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/libcthreads/libcthreads.vcproj` & `libfsxfs-20240501/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/fsxfs_test_volume/fsxfs_test_volume.vcproj` & `libfsxfs-20240501/msvscpp/fsxfs_test_volume/fsxfs_test_volume.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/libcpath/libcpath.vcproj` & `libfsxfs-20240501/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/fsxfs_test_attribute_values/fsxfs_test_attribute_values.vcproj` & `libfsxfs-20240501/msvscpp/fsxfs_test_attribute_values/fsxfs_test_attribute_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/fsxfs_test_tools_signal/fsxfs_test_tools_signal.vcproj` & `libfsxfs-20240501/msvscpp/fsxfs_test_tools_signal/fsxfs_test_tools_signal.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/fsxfs_test_attributes_table_header/fsxfs_test_attributes_table_header.vcproj` & `libfsxfs-20240501/msvscpp/fsxfs_test_attributes_table_header/fsxfs_test_attributes_table_header.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/fsxfs_test_notify/fsxfs_test_notify.vcproj` & `libfsxfs-20240501/msvscpp/fsxfs_test_notify/fsxfs_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/fsxfs_test_inode_btree/fsxfs_test_inode_btree.vcproj` & `libfsxfs-20240501/msvscpp/fsxfs_test_inode_btree/fsxfs_test_inode_btree.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/libhmac/libhmac.vcproj` & `libfsxfs-20240501/msvscpp/libhmac/libhmac.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/libcsplit/libcsplit.vcproj` & `libfsxfs-20240501/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/fsxfs_test_attributes_leaf_block_header/fsxfs_test_attributes_leaf_block_header.vcproj` & `libfsxfs-20240501/msvscpp/fsxfs_test_attributes_leaf_block_header/fsxfs_test_attributes_leaf_block_header.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/libuna/libuna.vcproj` & `libfsxfs-20240501/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/Makefile.in` & `libfsxfs-20240501/msvscpp/Makefile.in`

 * *Files 0% similar despite different names*

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
@@ -520,15 +522,16 @@
 	libuna/libuna.vcproj \
 	pyfsxfs/pyfsxfs.vcproj \
 	libfsxfs.sln
 
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
@@ -632,23 +635,25 @@
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
@@ -727,13 +732,10 @@
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

### Comparing `libfsxfs-20240222/msvscpp/fsxfs_test_tools_output/fsxfs_test_tools_output.vcproj` & `libfsxfs-20240501/msvscpp/fsxfs_test_tools_output/fsxfs_test_tools_output.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/libcnotify/libcnotify.vcproj` & `libfsxfs-20240501/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/libcerror/libcerror.vcproj` & `libfsxfs-20240501/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/fsxfs_test_btree_block/fsxfs_test_btree_block.vcproj` & `libfsxfs-20240501/msvscpp/fsxfs_test_btree_block/fsxfs_test_btree_block.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/msvscpp/libfdatetime/libfdatetime.vcproj` & `libfsxfs-20240501/msvscpp/libfdatetime/libfdatetime.vcproj`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/pyfsxfs/pyfsxfs_datetime.h` & `libfsxfs-20240501/pyfsxfs/pyfsxfs_datetime.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/pyfsxfs/pyfsxfs.c` & `libfsxfs-20240501/pyfsxfs/pyfsxfs.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/pyfsxfs/pyfsxfs_libbfio.h` & `libfsxfs-20240501/pyfsxfs/pyfsxfs_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/pyfsxfs/pyfsxfs_file_entry.h` & `libfsxfs-20240501/pyfsxfs/pyfsxfs_file_entry.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/pyfsxfs/pyfsxfs_integer.c` & `libfsxfs-20240501/pyfsxfs/pyfsxfs_integer.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/pyfsxfs/pyfsxfs_error.c` & `libfsxfs-20240501/pyfsxfs/pyfsxfs_error.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/pyfsxfs/pyfsxfs_extended_attribute.h` & `libfsxfs-20240501/pyfsxfs/pyfsxfs_extended_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/pyfsxfs/pyfsxfs_unused.h` & `libfsxfs-20240501/pyfsxfs/pyfsxfs_unused.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/pyfsxfs/pyfsxfs_extended_attribute.c` & `libfsxfs-20240501/pyfsxfs/pyfsxfs_extended_attribute.c`

 * *Files 2% similar despite different names*

```diff
@@ -42,22 +42,22 @@
 	  "get_name() -> Unicode string\n"
 	  "\n"
 	  "Retrieves the name." },
 
 	{ "read_buffer",
 	  (PyCFunction) pyfsxfs_extended_attribute_read_buffer,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read_buffer(size) -> Binary string\n"
+	  "read_buffer(size)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data." },
 
 	{ "read_buffer_at_offset",
 	  (PyCFunction) pyfsxfs_extended_attribute_read_buffer_at_offset,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read_buffer_at_offset(size, offset) -> Binary string\n"
+	  "read_buffer_at_offset(size, offset)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data at a specific offset." },
 
 	{ "seek_offset",
 	  (PyCFunction) pyfsxfs_extended_attribute_seek_offset,
 	  METH_VARARGS | METH_KEYWORDS,
 	  "seek_offset(offset, whence) -> None\n"
@@ -70,15 +70,15 @@
 	  "get_offset() -> Integer\n"
 	  "\n"
 	  "Retrieves the current offset within the data." },
 
 	{ "read",
 	  (PyCFunction) pyfsxfs_extended_attribute_read_buffer,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read(size) -> Binary string\n"
+	  "read(size)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data." },
 
 	{ "seek",
 	  (PyCFunction) pyfsxfs_extended_attribute_seek_offset,
 	  METH_VARARGS | METH_KEYWORDS,
 	  "seek(offset, whence) -> None\n"
```

### Comparing `libfsxfs-20240222/pyfsxfs/pyfsxfs_volume.c` & `libfsxfs-20240501/pyfsxfs/pyfsxfs_volume.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/pyfsxfs/pyfsxfs_file_entry.c` & `libfsxfs-20240501/pyfsxfs/pyfsxfs_file_entry.c`

 * *Files 0% similar despite different names*

```diff
@@ -201,22 +201,22 @@
 	  "get_sub_file_entry_by_name(name) -> Object or None\n"
 	  "\n"
 	  "Retrieves the sub file entry for an UTF-8 encoded name specified by the name." },
 
 	{ "read_buffer",
 	  (PyCFunction) pyfsxfs_file_entry_read_buffer,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read_buffer(size) -> Binary string\n"
+	  "read_buffer(size)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data at the current offset." },
 
 	{ "read_buffer_at_offset",
 	  (PyCFunction) pyfsxfs_file_entry_read_buffer_at_offset,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read_buffer_at_offset(size, offset) -> Binary string\n"
+	  "read_buffer_at_offset(size, offset)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data at a specific offset." },
 
 	{ "seek_offset",
 	  (PyCFunction) pyfsxfs_file_entry_seek_offset,
 	  METH_VARARGS | METH_KEYWORDS,
 	  "seek_offset(offset, whence) -> None\n"
@@ -229,15 +229,15 @@
 	  "get_offset() -> Integer\n"
 	  "\n"
 	  "Retrieves the current offset of the data." },
 
 	{ "read",
 	  (PyCFunction) pyfsxfs_file_entry_read_buffer,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read(size) -> Binary string\n"
+	  "read(size)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data at the current offset." },
 
 	{ "seek",
 	  (PyCFunction) pyfsxfs_file_entry_seek_offset,
 	  METH_VARARGS | METH_KEYWORDS,
 	  "seek(offset, whence) -> None\n"
```

### Comparing `libfsxfs-20240222/pyfsxfs/pyfsxfs_python.h` & `libfsxfs-20240501/pyfsxfs/pyfsxfs_python.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/pyfsxfs/pyfsxfs_libfsxfs.h` & `libfsxfs-20240501/pyfsxfs/pyfsxfs_libfsxfs.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/pyfsxfs/Makefile.am` & `libfsxfs-20240501/pyfsxfs/Makefile.am`

 * *Files 13% similar despite different names*

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
 
 pyfsxfs_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pyfsxfs_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
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

### Comparing `libfsxfs-20240222/pyfsxfs/pyfsxfs_libcerror.h` & `libfsxfs-20240501/pyfsxfs/pyfsxfs_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/pyfsxfs/pyfsxfs_file_entries.c` & `libfsxfs-20240501/pyfsxfs/pyfsxfs_file_entries.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/pyfsxfs/pyfsxfs_extended_attributes.h` & `libfsxfs-20240501/pyfsxfs/pyfsxfs_extended_attributes.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/pyfsxfs/pyfsxfs.h` & `libfsxfs-20240501/pyfsxfs/pyfsxfs.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/pyfsxfs/pyfsxfs_error.h` & `libfsxfs-20240501/pyfsxfs/pyfsxfs_error.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/pyfsxfs/pyfsxfs_datetime.c` & `libfsxfs-20240501/pyfsxfs/pyfsxfs_datetime.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/pyfsxfs/pyfsxfs_file_object_io_handle.h` & `libfsxfs-20240501/pyfsxfs/pyfsxfs_file_object_io_handle.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/pyfsxfs/pyfsxfs_volume.h` & `libfsxfs-20240501/pyfsxfs/pyfsxfs_volume.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/pyfsxfs/pyfsxfs_file_object_io_handle.c` & `libfsxfs-20240501/pyfsxfs/pyfsxfs_file_object_io_handle.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/pyfsxfs/pyfsxfs_file_entries.h` & `libfsxfs-20240501/pyfsxfs/pyfsxfs_file_entries.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/pyfsxfs/Makefile.in` & `libfsxfs-20240501/pyfsxfs/Makefile.in`

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
 
 @HAVE_PYTHON_TRUE@pyfsxfs_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pyfsxfs_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
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
+		-rm -f ./$(DEPDIR)/pyfsxfs_la-pyfsxfs.Plo
+	-rm -f ./$(DEPDIR)/pyfsxfs_la-pyfsxfs_datetime.Plo
+	-rm -f ./$(DEPDIR)/pyfsxfs_la-pyfsxfs_error.Plo
+	-rm -f ./$(DEPDIR)/pyfsxfs_la-pyfsxfs_extended_attribute.Plo
+	-rm -f ./$(DEPDIR)/pyfsxfs_la-pyfsxfs_extended_attributes.Plo
+	-rm -f ./$(DEPDIR)/pyfsxfs_la-pyfsxfs_file_entries.Plo
+	-rm -f ./$(DEPDIR)/pyfsxfs_la-pyfsxfs_file_entry.Plo
+	-rm -f ./$(DEPDIR)/pyfsxfs_la-pyfsxfs_file_object_io_handle.Plo
+	-rm -f ./$(DEPDIR)/pyfsxfs_la-pyfsxfs_integer.Plo
+	-rm -f ./$(DEPDIR)/pyfsxfs_la-pyfsxfs_volume.Plo
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

### Comparing `libfsxfs-20240222/pyfsxfs/pyfsxfs_integer.h` & `libfsxfs-20240501/pyfsxfs/pyfsxfs_integer.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/pyfsxfs/pyfsxfs_extended_attributes.c` & `libfsxfs-20240501/pyfsxfs/pyfsxfs_extended_attributes.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcfile/libcfile_extern.h` & `libfsxfs-20240501/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcfile/libcfile_support.h` & `libfsxfs-20240501/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcfile/libcfile_unused.h` & `libfsxfs-20240501/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcfile/libcfile_notify.h` & `libfsxfs-20240501/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcfile/libcfile_support.c` & `libfsxfs-20240501/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcfile/libcfile_types.h` & `libfsxfs-20240501/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcfile/Makefile.am` & `libfsxfs-20240501/libcfile/Makefile.am`

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

### Comparing `libfsxfs-20240222/libcfile/libcfile_notify.c` & `libfsxfs-20240501/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcfile/libcfile_system_string.h` & `libfsxfs-20240501/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcfile/libcfile_file.h` & `libfsxfs-20240501/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcfile/libcfile_libcnotify.h` & `libfsxfs-20240501/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcfile/libcfile_system_string.c` & `libfsxfs-20240501/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcfile/libcfile_error.h` & `libfsxfs-20240501/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcfile/libcfile_libcerror.h` & `libfsxfs-20240501/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcfile/libcfile_file.c` & `libfsxfs-20240501/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcfile/libcfile_libclocale.h` & `libfsxfs-20240501/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcfile/libcfile_winapi.h` & `libfsxfs-20240501/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcfile/Makefile.in` & `libfsxfs-20240501/libcfile/Makefile.in`

 * *Files 4% similar despite different names*

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

### Comparing `libfsxfs-20240222/libcfile/libcfile_error.c` & `libfsxfs-20240501/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcfile/libcfile_libuna.h` & `libfsxfs-20240501/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcfile/libcfile_winapi.c` & `libfsxfs-20240501/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcfile/libcfile_definitions.h` & `libfsxfs-20240501/libcfile/libcfile_definitions.h`

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

### Comparing `libfsxfs-20240222/INSTALL` & `libfsxfs-20240501/INSTALL`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcdata/libcdata_list_element.h` & `libfsxfs-20240501/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcdata/libcdata_array.h` & `libfsxfs-20240501/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcdata/libcdata_definitions.h` & `libfsxfs-20240501/libcdata/libcdata_definitions.h`

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

### Comparing `libfsxfs-20240222/libcdata/libcdata_libcerror.h` & `libfsxfs-20240501/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcdata/libcdata_unused.h` & `libfsxfs-20240501/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcdata/libcdata_btree.h` & `libfsxfs-20240501/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcdata/libcdata_btree.c` & `libfsxfs-20240501/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcdata/libcdata_support.c` & `libfsxfs-20240501/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcdata/libcdata_list.c` & `libfsxfs-20240501/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcdata/libcdata_extern.h` & `libfsxfs-20240501/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcdata/libcdata_list.h` & `libfsxfs-20240501/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcdata/libcdata_btree_values_list.h` & `libfsxfs-20240501/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcdata/Makefile.am` & `libfsxfs-20240501/libcdata/Makefile.am`

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

### Comparing `libfsxfs-20240222/libcdata/libcdata_btree_node.h` & `libfsxfs-20240501/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcdata/libcdata_range_list_value.h` & `libfsxfs-20240501/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcdata/libcdata_range_list.h` & `libfsxfs-20240501/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcdata/libcdata_range_list.c` & `libfsxfs-20240501/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcdata/libcdata_array.c` & `libfsxfs-20240501/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcdata/libcdata_list_element.c` & `libfsxfs-20240501/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcdata/libcdata_libcthreads.h` & `libfsxfs-20240501/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcdata/libcdata_tree_node.h` & `libfsxfs-20240501/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcdata/libcdata_error.h` & `libfsxfs-20240501/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcdata/libcdata_types.h` & `libfsxfs-20240501/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcdata/libcdata_btree_node.c` & `libfsxfs-20240501/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcdata/libcdata_tree_node.c` & `libfsxfs-20240501/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcdata/libcdata_support.h` & `libfsxfs-20240501/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcdata/Makefile.in` & `libfsxfs-20240501/libcdata/Makefile.in`

 * *Files 3% similar despite different names*

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

### Comparing `libfsxfs-20240222/libcdata/libcdata_range_list_value.c` & `libfsxfs-20240501/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcdata/libcdata_btree_values_list.c` & `libfsxfs-20240501/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcdata/libcdata_error.c` & `libfsxfs-20240501/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/config.sub` & `libfsxfs-20240501/config.sub`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/setup.py` & `libfsxfs-20240501/setup.py`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/acinclude.m4` & `libfsxfs-20240501/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/config.rpath` & `libfsxfs-20240501/config.rpath`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs.pc.in` & `libfsxfs-20240501/libfsxfs.pc.in`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_btree_block.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_btree_block.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_io_handle.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_io_handle.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_libfcache.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_libfcache.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_extents.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_extents.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_btree_header.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_btree_header.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_libcthreads.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_extended_attribute.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_extended_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_libcnotify.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_directory_table.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_directory_table.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs.c` & `libfsxfs-20240501/libfsxfs/libfsxfs.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs.rc.in` & `libfsxfs-20240501/libfsxfs/libfsxfs.rc.in`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_superblock.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_superblock.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_superblock.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_superblock.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_file_system_block_header.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_file_system_block_header.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_support.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_support.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_inode_btree_record.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_inode_btree_record.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_notify.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_notify.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_block_directory.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_block_directory.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_directory_table_header.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_directory_table_header.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_definitions.h.in` & `libfsxfs-20240501/libfsxfs/libfsxfs_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_attributes.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_attributes.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/fsxfs_block_directory.h` & `libfsxfs-20240501/libfsxfs/fsxfs_block_directory.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_file_entry.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_file_entry.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_block_directory.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_block_directory.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_io_handle.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_io_handle.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs.rc` & `libfsxfs-20240501/libfsxfs/libfsxfs.rc`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to support the X File System (XFS) format\0"
-      VALUE "FileVersion",		"20240222" "\0"
+      VALUE "FileVersion",		"20240501" "\0"
       VALUE "InternalName",		"libfsxfs.dll\0"
       VALUE "LegalCopyright",		"(C) 2020-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libfsxfs.dll\0"
       VALUE "ProductName",		"libfsxfs\0"
-      VALUE "ProductVersion",		"20240222" "\0"
+      VALUE "ProductVersion",		"20240501" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libfsxfs/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_libcdata.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_debug.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_debug.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_types.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_types.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_directory.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_directory.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_extern.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_extern.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/Makefile.am` & `libfsxfs-20240501/libfsxfs/Makefile.am`

 * *Files 14% similar despite different names*

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
@@ -103,21 +103,19 @@
 libfsxfs_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libfsxfs_definitions.h.in \
 	libfsxfs.rc \
 	libfsxfs.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfsxfs_definitions.h \
+	libfsxfs.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libfsxfs_definitions.h
-	-rm -f libfsxfs.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfsxfs ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfsxfs_la_SOURCES)
```

### Comparing `libfsxfs-20240222/libfsxfs/fsxfs_inode_information.h` & `libfsxfs-20240501/libfsxfs/fsxfs_inode_information.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_inode.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_inode.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_attributes_leaf_block_header.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_attributes_leaf_block_header.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_extents.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_extents.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/fsxfs_superblock.h` & `libfsxfs-20240501/libfsxfs/fsxfs_superblock.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_unused.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_unused.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_extent_btree.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_extent_btree.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_buffer_data_handle.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_buffer_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/fsxfs_btree.h` & `libfsxfs-20240501/libfsxfs/fsxfs_btree.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_inode_btree.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_inode_btree.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_libfdata.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_libfdata.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_libuna.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_libuna.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_file_system_block.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_file_system_block.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_extent.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_extent.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_inode_information.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_inode_information.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_directory_entry.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_directory_entry.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_extent_list.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_extent_list.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_attribute_values.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_attribute_values.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_extended_attribute.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_extended_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_buffer_data_handle.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_buffer_data_handle.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_debug.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_debug.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_file_entry.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_file_entry.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_block_directory_footer.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_block_directory_footer.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_attributes_leaf_block_header.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_attributes_leaf_block_header.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_directory_table_header.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_directory_table_header.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_attribute_values.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_attribute_values.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_error.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_error.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_block_directory_header.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_block_directory_header.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_error.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_error.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_extent.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_extent.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_volume.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_volume.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_inode_btree.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_inode_btree.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_notify.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_notify.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_extent_list.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_extent_list.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_block_directory_header.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_block_directory_header.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_block_data_handle.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_block_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_inode.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_inode.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/fsxfs_attributes_block.h` & `libfsxfs-20240501/libfsxfs/fsxfs_attributes_block.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_libfguid.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_libcerror.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_extent_btree.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_extent_btree.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/fsxfs_inode.h` & `libfsxfs-20240501/libfsxfs/fsxfs_inode.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_directory.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_directory.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_libclocale.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_support.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_support.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_libfdatetime.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_block_data_handle.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_block_data_handle.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/fsxfs_attributes.h` & `libfsxfs-20240501/libfsxfs/fsxfs_attributes.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_file_system_block_header.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_file_system_block_header.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_attributes_table_header.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_attributes_table_header.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_definitions.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_definitions.h`

 * *Files 3% similar despite different names*

```diff
@@ -33,19 +33,19 @@
 #if !defined( HAVE_LOCAL_LIBFSXFS )
 #include <libfsxfs/definitions.h>
 
 /* The definitions in <libfsxfs/definitions.h> are copied here
  * for local use of libfsxfs
  */
 #else
-#define LIBFSXFS_VERSION						20240222
+#define LIBFSXFS_VERSION						20240501
 
 /* The version string
  */
-#define LIBFSXFS_VERSION_STRING						"20240222"
+#define LIBFSXFS_VERSION_STRING						"20240501"
 
 /* The file access
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBFSXFS_ACCESS_FLAGS
```

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_attributes_table_header.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_attributes_table_header.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_directory_entry.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_directory_entry.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_file_system.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_file_system.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_attributes_table.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_attributes_table.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_attributes_table.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_attributes_table.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_directory_table.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_directory_table.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/fsxfs_file_system_block.h` & `libfsxfs-20240501/libfsxfs/fsxfs_file_system_block.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_inode_btree_record.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_inode_btree_record.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_volume.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_volume.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_file_system.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_file_system.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_libbfio.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/Makefile.in` & `libfsxfs-20240501/libfsxfs/Makefile.in`

 * *Files 6% similar despite different names*

```diff
@@ -540,14 +540,16 @@
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
@@ -608,16 +610,16 @@
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
@@ -714,15 +716,18 @@
 
 libfsxfs_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libfsxfs_definitions.h.in \
 	libfsxfs.rc \
 	libfsxfs.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfsxfs_definitions.h \
+	libfsxfs.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -990,24 +995,64 @@
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
+		-rm -f ./$(DEPDIR)/libfsxfs.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_attribute_values.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_attributes.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_attributes_leaf_block_header.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_attributes_table.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_attributes_table_header.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_block_data_handle.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_block_directory.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_block_directory_footer.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_block_directory_header.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_btree_block.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_btree_header.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_buffer_data_handle.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_data_stream.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_debug.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_directory.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_directory_entry.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_directory_table.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_directory_table_header.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_error.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_extended_attribute.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_extent.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_extent_btree.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_extent_list.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_extents.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_file_entry.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_file_system.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_file_system_block.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_file_system_block_header.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_inode.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_inode_btree.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_inode_btree_record.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_inode_information.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_notify.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_superblock.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_support.Plo
+	-rm -f ./$(DEPDIR)/libfsxfs_volume.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1128,19 +1173,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libfsxfs_definitions.h
-	-rm -f libfsxfs.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfsxfs ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfsxfs_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_btree_block.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_btree_block.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_file_system_block.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_file_system_block.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_inode_information.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_inode_information.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_btree_header.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_btree_header.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_data_stream.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_data_stream.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_block_directory_footer.c` & `libfsxfs-20240501/libfsxfs/libfsxfs_block_directory_footer.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_data_stream.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_data_stream.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfsxfs/libfsxfs_attributes.h` & `libfsxfs-20240501/libfsxfs/libfsxfs_attributes.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcthreads/libcthreads_thread.h` & `libfsxfs-20240501/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcthreads/libcthreads_read_write_lock.h` & `libfsxfs-20240501/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcthreads/libcthreads_thread.c` & `libfsxfs-20240501/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcthreads/libcthreads_thread_pool.h` & `libfsxfs-20240501/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcthreads/libcthreads_support.h` & `libfsxfs-20240501/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcthreads/libcthreads_lock.h` & `libfsxfs-20240501/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcthreads/libcthreads_unused.h` & `libfsxfs-20240501/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcthreads/libcthreads_lock.c` & `libfsxfs-20240501/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcthreads/libcthreads_condition.h` & `libfsxfs-20240501/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcthreads/libcthreads_repeating_thread.h` & `libfsxfs-20240501/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcthreads/Makefile.am` & `libfsxfs-20240501/libcthreads/Makefile.am`

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

### Comparing `libfsxfs-20240222/libcthreads/libcthreads_support.c` & `libfsxfs-20240501/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcthreads/libcthreads_mutex.c` & `libfsxfs-20240501/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcthreads/libcthreads_queue.c` & `libfsxfs-20240501/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcthreads/libcthreads_mutex.h` & `libfsxfs-20240501/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcthreads/libcthreads_types.h` & `libfsxfs-20240501/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcthreads/libcthreads_thread_attributes.h` & `libfsxfs-20240501/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcthreads/libcthreads_condition.c` & `libfsxfs-20240501/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcthreads/libcthreads_error.c` & `libfsxfs-20240501/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcthreads/libcthreads_read_write_lock.c` & `libfsxfs-20240501/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcthreads/libcthreads_libcerror.h` & `libfsxfs-20240501/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcthreads/libcthreads_definitions.h` & `libfsxfs-20240501/libcthreads/libcthreads_definitions.h`

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

### Comparing `libfsxfs-20240222/libcthreads/libcthreads_thread_pool.c` & `libfsxfs-20240501/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcthreads/libcthreads_error.h` & `libfsxfs-20240501/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcthreads/libcthreads_thread_attributes.c` & `libfsxfs-20240501/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcthreads/libcthreads_extern.h` & `libfsxfs-20240501/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcthreads/libcthreads_repeating_thread.c` & `libfsxfs-20240501/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcthreads/Makefile.in` & `libfsxfs-20240501/libcthreads/Makefile.in`

 * *Files 5% similar despite different names*

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

### Comparing `libfsxfs-20240222/libcthreads/libcthreads_queue.h` & `libfsxfs-20240501/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/test-driver` & `libfsxfs-20240501/test-driver`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcpath/libcpath_support.c` & `libfsxfs-20240501/libcpath/libcpath_support.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcpath/libcpath_libcerror.h` & `libfsxfs-20240501/libcpath/libcpath_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcpath/libcpath_definitions.h` & `libfsxfs-20240501/libcpath/libcpath_definitions.h`

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

### Comparing `libfsxfs-20240222/libcpath/Makefile.am` & `libfsxfs-20240501/libcpath/Makefile.am`

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

### Comparing `libfsxfs-20240222/libcpath/libcpath_error.c` & `libfsxfs-20240501/libcpath/libcpath_error.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcpath/libcpath_extern.h` & `libfsxfs-20240501/libcpath/libcpath_extern.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcpath/libcpath_system_string.h` & `libfsxfs-20240501/libcpath/libcpath_system_string.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcpath/libcpath_support.h` & `libfsxfs-20240501/libcpath/libcpath_support.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcpath/libcpath_libcsplit.h` & `libfsxfs-20240501/libcpath/libcpath_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcpath/libcpath_system_string.c` & `libfsxfs-20240501/libcpath/libcpath_system_string.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcpath/libcpath_libclocale.h` & `libfsxfs-20240501/libcpath/libcpath_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcpath/libcpath_error.h` & `libfsxfs-20240501/libcpath/libcpath_error.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcpath/Makefile.in` & `libfsxfs-20240501/libcpath/Makefile.in`

 * *Files 4% similar despite different names*

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

### Comparing `libfsxfs-20240222/libcpath/libcpath_libuna.h` & `libfsxfs-20240501/libcpath/libcpath_libuna.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcpath/libcpath_unused.h` & `libfsxfs-20240501/libcpath/libcpath_unused.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcpath/libcpath_path.c` & `libfsxfs-20240501/libcpath/libcpath_path.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcpath/libcpath_path.h` & `libfsxfs-20240501/libcpath/libcpath_path.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/ChangeLog` & `libfsxfs-20240501/ChangeLog`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/manuals/fsxfsinfo.1` & `libfsxfs-20240501/manuals/fsxfsinfo.1`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/manuals/libfsxfs.3` & `libfsxfs-20240501/manuals/libfsxfs.3`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/manuals/fsxfsmount.1` & `libfsxfs-20240501/manuals/fsxfsmount.1`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/manuals/Makefile.in` & `libfsxfs-20240501/manuals/Makefile.in`

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
 	libfsxfs.3
 
 EXTRA_DIST = \
 	fsxfsinfo.1 \
 	fsxfsmount.1 \
 	libfsxfs.3
 
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

### Comparing `libfsxfs-20240222/tests/fsxfs_test_libbfio.h` & `libfsxfs-20240501/tests/fsxfs_test_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_tools_info_handle.c` & `libfsxfs-20240501/tests/fsxfs_test_tools_info_handle.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_attributes_table.c` & `libfsxfs-20240501/tests/fsxfs_test_attributes_table.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_notify.c` & `libfsxfs-20240501/tests/fsxfs_test_notify.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_volume.c` & `libfsxfs-20240501/tests/fsxfs_test_volume.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_memory.c` & `libfsxfs-20240501/tests/fsxfs_test_memory.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_libclocale.h` & `libfsxfs-20240501/tests/fsxfs_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_block_directory_header.c` & `libfsxfs-20240501/tests/fsxfs_test_block_directory_header.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_libcnotify.h` & `libfsxfs-20240501/tests/fsxfs_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_libcdata.h` & `libfsxfs-20240501/tests/fsxfs_test_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_file_system_block_header.c` & `libfsxfs-20240501/tests/fsxfs_test_file_system_block_header.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_directory_entry.c` & `libfsxfs-20240501/tests/fsxfs_test_directory_entry.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/pyfsxfs_test_volume.py` & `libfsxfs-20240501/tests/pyfsxfs_test_volume.py`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/test_tools.sh` & `libfsxfs-20240501/tests/test_tools.sh`

 * *Files 2% similar despite different names*

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

### Comparing `libfsxfs-20240222/tests/fsxfs_test_extent.c` & `libfsxfs-20240501/tests/fsxfs_test_extent.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_inode_btree.c` & `libfsxfs-20240501/tests/fsxfs_test_inode_btree.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_libuna.h` & `libfsxfs-20240501/tests/fsxfs_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_support.c` & `libfsxfs-20240501/tests/fsxfs_test_support.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/Makefile.am` & `libfsxfs-20240501/tests/Makefile.am`

 * *Files 2% similar despite different names*

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
@@ -439,13 +439,12 @@
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libfsxfs/libfsxfs.la \
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

### Comparing `libfsxfs-20240222/tests/fsxfs_test_attribute_values.c` & `libfsxfs-20240501/tests/fsxfs_test_attribute_values.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/test_fsxfsinfo.sh` & `libfsxfs-20240501/tests/test_fsxfsinfo.sh`

 * *Files 8% similar despite different names*

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
 
 PROFILES=("fsxfsinfo" "fsxfsinfo_fs");
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

### Comparing `libfsxfs-20240222/tests/fsxfs_test_tools_signal.c` & `libfsxfs-20240501/tests/fsxfs_test_tools_signal.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_functions.c` & `libfsxfs-20240501/tests/fsxfs_test_functions.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_inode_information.c` & `libfsxfs-20240501/tests/fsxfs_test_inode_information.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_attributes_leaf_block_header.c` & `libfsxfs-20240501/tests/fsxfs_test_attributes_leaf_block_header.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_macros.h` & `libfsxfs-20240501/tests/fsxfs_test_macros.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/test_python_module.sh` & `libfsxfs-20240501/tests/test_python_module.sh`

 * *Files 8% similar despite different names*

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
 
+LIBRARY_NAME="libfsxfs";
+PYTHON_MODULE="pyfsxfs";
+
 test_python_function()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyfsxfs_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_SCRIPT}";
 	local RESULT=$?;
 
 	return ${RESULT};
 }
 
 test_python_function_with_input()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyfsxfs_test_${TEST_FUNCTION}.py";
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
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "pyfsxfs");
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

### Comparing `libfsxfs-20240222/tests/fsxfs_test_functions.h` & `libfsxfs-20240501/tests/fsxfs_test_functions.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_libfsxfs.h` & `libfsxfs-20240501/tests/fsxfs_test_libfsxfs.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_directory_table_header.c` & `libfsxfs-20240501/tests/fsxfs_test_directory_table_header.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_attributes_table_header.c` & `libfsxfs-20240501/tests/fsxfs_test_attributes_table_header.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_block_directory_footer.c` & `libfsxfs-20240501/tests/fsxfs_test_block_directory_footer.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_tools_output.c` & `libfsxfs-20240501/tests/fsxfs_test_tools_output.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_io_handle.c` & `libfsxfs-20240501/tests/fsxfs_test_io_handle.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_getopt.c` & `libfsxfs-20240501/tests/fsxfs_test_getopt.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/test_runner.sh` & `libfsxfs-20240501/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_error.c` & `libfsxfs-20240501/tests/fsxfs_test_error.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_getopt.h` & `libfsxfs-20240501/tests/fsxfs_test_getopt.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_libcerror.h` & `libfsxfs-20240501/tests/fsxfs_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/pyfsxfs_test_support.py` & `libfsxfs-20240501/tests/pyfsxfs_test_support.py`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_buffer_data_handle.c` & `libfsxfs-20240501/tests/fsxfs_test_buffer_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_superblock.c` & `libfsxfs-20240501/tests/fsxfs_test_superblock.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/Makefile.in` & `libfsxfs-20240501/tests/Makefile.in`

 * *Files 10% similar despite different names*

```diff
@@ -887,14 +887,16 @@
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
@@ -956,16 +958,16 @@
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
@@ -1369,16 +1371,18 @@
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libfsxfs/libfsxfs.la \
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
@@ -1914,24 +1918,58 @@
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
 	-rm -f ../fsxfstools/$(DEPDIR)/$(am__dirstamp)
 	-rm -f ../fsxfstools/$(am__dirstamp)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ../fsxfstools/$(DEPDIR)/digest_hash.Po
+	-rm -f ../fsxfstools/$(DEPDIR)/fsxfstools_output.Po
+	-rm -f ../fsxfstools/$(DEPDIR)/fsxfstools_signal.Po
+	-rm -f ../fsxfstools/$(DEPDIR)/info_handle.Po
+	-rm -f ./$(DEPDIR)/fsxfs_test_attribute_values.Po
+	-rm -f ./$(DEPDIR)/fsxfs_test_attributes_leaf_block_header.Po
+	-rm -f ./$(DEPDIR)/fsxfs_test_attributes_table.Po
+	-rm -f ./$(DEPDIR)/fsxfs_test_attributes_table_header.Po
+	-rm -f ./$(DEPDIR)/fsxfs_test_block_directory_footer.Po
+	-rm -f ./$(DEPDIR)/fsxfs_test_block_directory_header.Po
+	-rm -f ./$(DEPDIR)/fsxfs_test_btree_block.Po
+	-rm -f ./$(DEPDIR)/fsxfs_test_btree_header.Po
+	-rm -f ./$(DEPDIR)/fsxfs_test_buffer_data_handle.Po
+	-rm -f ./$(DEPDIR)/fsxfs_test_directory_entry.Po
+	-rm -f ./$(DEPDIR)/fsxfs_test_directory_table_header.Po
+	-rm -f ./$(DEPDIR)/fsxfs_test_error.Po
+	-rm -f ./$(DEPDIR)/fsxfs_test_extent.Po
+	-rm -f ./$(DEPDIR)/fsxfs_test_file_system_block_header.Po
+	-rm -f ./$(DEPDIR)/fsxfs_test_functions.Po
+	-rm -f ./$(DEPDIR)/fsxfs_test_getopt.Po
+	-rm -f ./$(DEPDIR)/fsxfs_test_inode_btree.Po
+	-rm -f ./$(DEPDIR)/fsxfs_test_inode_btree_record.Po
+	-rm -f ./$(DEPDIR)/fsxfs_test_inode_information.Po
+	-rm -f ./$(DEPDIR)/fsxfs_test_io_handle.Po
+	-rm -f ./$(DEPDIR)/fsxfs_test_memory.Po
+	-rm -f ./$(DEPDIR)/fsxfs_test_notify.Po
+	-rm -f ./$(DEPDIR)/fsxfs_test_superblock.Po
+	-rm -f ./$(DEPDIR)/fsxfs_test_support.Po
+	-rm -f ./$(DEPDIR)/fsxfs_test_tools_info_handle.Po
+	-rm -f ./$(DEPDIR)/fsxfs_test_tools_output.Po
+	-rm -f ./$(DEPDIR)/fsxfs_test_tools_signal.Po
+	-rm -f ./$(DEPDIR)/fsxfs_test_volume.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -2046,13 +2084,10 @@
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

### Comparing `libfsxfs-20240222/tests/fsxfs_test_inode_btree_record.c` & `libfsxfs-20240501/tests/fsxfs_test_inode_btree_record.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_btree_header.c` & `libfsxfs-20240501/tests/fsxfs_test_btree_header.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_btree_block.c` & `libfsxfs-20240501/tests/fsxfs_test_btree_block.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_memory.h` & `libfsxfs-20240501/tests/fsxfs_test_memory.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/fsxfs_test_unused.h` & `libfsxfs-20240501/tests/fsxfs_test_unused.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/tests/test_library.sh` & `libfsxfs-20240501/tests/test_library.sh`

 * *Files 3% similar despite different names*

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
 
 LIBRARY_TESTS="attribute_values attributes_leaf_block_header attributes_table attributes_table_header block_directory_footer block_directory_header btree_block btree_header buffer_data_handle directory_entry directory_table_header error extent file_system_block_header inode_btree inode_btree_record inode_information io_handle notify superblock";
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

### Comparing `libfsxfs-20240222/ossfuzz/volume_fuzzer.cc` & `libfsxfs-20240501/ossfuzz/volume_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/ossfuzz/Makefile.am` & `libfsxfs-20240501/ossfuzz/Makefile.am`

 * *Files 3% similar despite different names*

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
 	../libfsxfs/libfsxfs.la \
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

### Comparing `libfsxfs-20240222/ossfuzz/ossfuzz_libbfio.h` & `libfsxfs-20240501/ossfuzz/ossfuzz_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/ossfuzz/file_entry_fuzzer.cc` & `libfsxfs-20240501/ossfuzz/file_entry_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/ossfuzz/extended_attribute_fuzzer.cc` & `libfsxfs-20240501/ossfuzz/extended_attribute_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/ossfuzz/ossfuzz_libfsxfs.h` & `libfsxfs-20240501/ossfuzz/ossfuzz_libfsxfs.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/ossfuzz/Makefile.in` & `libfsxfs-20240501/ossfuzz/Makefile.in`

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
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libfsxfs/libfsxfs.la \
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

### Comparing `libfsxfs-20240222/ltmain.sh` & `libfsxfs-20240501/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/libhmac_sha1_context.c` & `libfsxfs-20240501/libhmac/libhmac_sha1_context.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/libhmac_sha224.h` & `libfsxfs-20240501/libhmac/libhmac_sha224.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/libhmac_sha512_context.c` & `libfsxfs-20240501/libhmac/libhmac_sha512_context.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/libhmac_extern.h` & `libfsxfs-20240501/libhmac/libhmac_extern.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/libhmac_md5.c` & `libfsxfs-20240501/libhmac/libhmac_md5.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/libhmac_md5.h` & `libfsxfs-20240501/libhmac/libhmac_md5.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/libhmac_error.h` & `libfsxfs-20240501/libhmac/libhmac_error.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/libhmac_types.h` & `libfsxfs-20240501/libhmac/libhmac_types.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/libhmac_byte_stream.h` & `libfsxfs-20240501/libhmac/libhmac_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/libhmac_sha512.c` & `libfsxfs-20240501/libhmac/libhmac_sha512.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/libhmac_sha256_context.c` & `libfsxfs-20240501/libhmac/libhmac_sha256_context.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/libhmac_sha224.c` & `libfsxfs-20240501/libhmac/libhmac_sha224.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/libhmac_definitions.h` & `libfsxfs-20240501/libhmac/libhmac_definitions.h`

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

### Comparing `libfsxfs-20240222/libhmac/libhmac_unused.h` & `libfsxfs-20240501/libhmac/libhmac_unused.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/libhmac_sha1.h` & `libfsxfs-20240501/libhmac/libhmac_sha1.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/libhmac_sha256_context.h` & `libfsxfs-20240501/libhmac/libhmac_sha256_context.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/Makefile.am` & `libfsxfs-20240501/libhmac/Makefile.am`

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

### Comparing `libfsxfs-20240222/libhmac/libhmac_sha224_context.c` & `libfsxfs-20240501/libhmac/libhmac_sha224_context.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/libhmac_md5_context.h` & `libfsxfs-20240501/libhmac/libhmac_md5_context.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/libhmac_sha256.c` & `libfsxfs-20240501/libhmac/libhmac_sha256.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/libhmac_sha1_context.h` & `libfsxfs-20240501/libhmac/libhmac_sha1_context.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/libhmac_libcerror.h` & `libfsxfs-20240501/libhmac/libhmac_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/libhmac_error.c` & `libfsxfs-20240501/libhmac/libhmac_error.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/libhmac_support.h` & `libfsxfs-20240501/libhmac/libhmac_support.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/Makefile.in` & `libfsxfs-20240501/libhmac/Makefile.in`

 * *Files 3% similar despite different names*

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

### Comparing `libfsxfs-20240222/libhmac/libhmac_sha256.h` & `libfsxfs-20240501/libhmac/libhmac_sha256.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/libhmac_sha224_context.h` & `libfsxfs-20240501/libhmac/libhmac_sha224_context.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/libhmac_sha512_context.h` & `libfsxfs-20240501/libhmac/libhmac_sha512_context.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/libhmac_sha512.h` & `libfsxfs-20240501/libhmac/libhmac_sha512.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/libhmac_support.c` & `libfsxfs-20240501/libhmac/libhmac_support.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/libhmac_sha1.c` & `libfsxfs-20240501/libhmac/libhmac_sha1.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libhmac/libhmac_md5_context.c` & `libfsxfs-20240501/libhmac/libhmac_md5_context.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcsplit/libcsplit_narrow_string.c` & `libfsxfs-20240501/libcsplit/libcsplit_narrow_string.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcsplit/libcsplit_definitions.h` & `libfsxfs-20240501/libcsplit/libcsplit_definitions.h`

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

### Comparing `libfsxfs-20240222/libcsplit/libcsplit_types.h` & `libfsxfs-20240501/libcsplit/libcsplit_types.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcsplit/libcsplit_wide_split_string.c` & `libfsxfs-20240501/libcsplit/libcsplit_wide_split_string.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcsplit/libcsplit_support.h` & `libfsxfs-20240501/libcsplit/libcsplit_support.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcsplit/Makefile.am` & `libfsxfs-20240501/libcsplit/Makefile.am`

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

### Comparing `libfsxfs-20240222/libcsplit/libcsplit_libcerror.h` & `libfsxfs-20240501/libcsplit/libcsplit_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcsplit/libcsplit_wide_string.c` & `libfsxfs-20240501/libcsplit/libcsplit_wide_string.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcsplit/libcsplit_unused.h` & `libfsxfs-20240501/libcsplit/libcsplit_unused.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcsplit/libcsplit_wide_split_string.h` & `libfsxfs-20240501/libcsplit/libcsplit_wide_split_string.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcsplit/libcsplit_error.c` & `libfsxfs-20240501/libcsplit/libcsplit_error.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcsplit/libcsplit_narrow_split_string.c` & `libfsxfs-20240501/libcsplit/libcsplit_narrow_split_string.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcsplit/libcsplit_extern.h` & `libfsxfs-20240501/libcsplit/libcsplit_extern.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcsplit/libcsplit_error.h` & `libfsxfs-20240501/libcsplit/libcsplit_error.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcsplit/libcsplit_support.c` & `libfsxfs-20240501/libcsplit/libcsplit_support.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcsplit/libcsplit_wide_string.h` & `libfsxfs-20240501/libcsplit/libcsplit_wide_string.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcsplit/Makefile.in` & `libfsxfs-20240501/libcsplit/Makefile.in`

 * *Files 1% similar despite different names*

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

### Comparing `libfsxfs-20240222/libcsplit/libcsplit_narrow_split_string.h` & `libfsxfs-20240501/libcsplit/libcsplit_narrow_split_string.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcsplit/libcsplit_narrow_string.h` & `libfsxfs-20240501/libcsplit/libcsplit_narrow_string.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/po/remove-potcdate.sin` & `libfsxfs-20240501/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/po/Makefile.in.in` & `libfsxfs-20240501/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/po/en@quot.header` & `libfsxfs-20240501/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/po/en@boldquot.header` & `libfsxfs-20240501/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/po/insert-header.sin` & `libfsxfs-20240501/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/po/Makevars` & `libfsxfs-20240501/po/Makevars`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/po/Makevars.in` & `libfsxfs-20240501/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/po/Rules-quot` & `libfsxfs-20240501/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_windows_1251.c` & `libfsxfs-20240501/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_utf16_string.c` & `libfsxfs-20240501/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_base16_stream.c` & `libfsxfs-20240501/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_utf8_stream.h` & `libfsxfs-20240501/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_iso_8859_2.h` & `libfsxfs-20240501/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_windows_932.c` & `libfsxfs-20240501/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_dingbats.h` & `libfsxfs-20240501/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_utf8_string.c` & `libfsxfs-20240501/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_base64_stream.c` & `libfsxfs-20240501/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_error.h` & `libfsxfs-20240501/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_turkish.h` & `libfsxfs-20240501/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_unicode_character.c` & `libfsxfs-20240501/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_gaelic.c` & `libfsxfs-20240501/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_arabic.h` & `libfsxfs-20240501/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_thai.c` & `libfsxfs-20240501/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_windows_874.h` & `libfsxfs-20240501/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_iso_8859_15.h` & `libfsxfs-20240501/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_utf8_string.h` & `libfsxfs-20240501/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_iso_8859_16.c` & `libfsxfs-20240501/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_windows_1255.c` & `libfsxfs-20240501/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_utf7_stream.c` & `libfsxfs-20240501/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_byte_stream.h` & `libfsxfs-20240501/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_koi8_u.c` & `libfsxfs-20240501/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_unused.h` & `libfsxfs-20240501/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_iso_8859_6.c` & `libfsxfs-20240501/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_iso_8859_14.c` & `libfsxfs-20240501/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_base64_stream.h` & `libfsxfs-20240501/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_error.c` & `libfsxfs-20240501/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_centraleurroman.h` & `libfsxfs-20240501/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_romanian.c` & `libfsxfs-20240501/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_iso_8859_6.h` & `libfsxfs-20240501/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_iso_8859_9.c` & `libfsxfs-20240501/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_russian.h` & `libfsxfs-20240501/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_dingbats.c` & `libfsxfs-20240501/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_iso_8859_15.c` & `libfsxfs-20240501/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_windows_936.c` & `libfsxfs-20240501/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_croatian.h` & `libfsxfs-20240501/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_scsu.h` & `libfsxfs-20240501/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/Makefile.am` & `libfsxfs-20240501/libuna/Makefile.am`

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

### Comparing `libfsxfs-20240222/libuna/libuna_utf32_stream.c` & `libfsxfs-20240501/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_windows_936.h` & `libfsxfs-20240501/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_iso_8859_10.c` & `libfsxfs-20240501/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_roman.c` & `libfsxfs-20240501/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_utf7_stream.h` & `libfsxfs-20240501/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_iso_8859_3.h` & `libfsxfs-20240501/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_thai.h` & `libfsxfs-20240501/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_farsi.h` & `libfsxfs-20240501/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_ukrainian.c` & `libfsxfs-20240501/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_inuit.c` & `libfsxfs-20240501/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_windows_932.h` & `libfsxfs-20240501/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_windows_874.c` & `libfsxfs-20240501/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_iso_8859_5.c` & `libfsxfs-20240501/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_iso_8859_10.h` & `libfsxfs-20240501/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_definitions.h` & `libfsxfs-20240501/libuna/libuna_definitions.h`

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

### Comparing `libfsxfs-20240222/libuna/libuna_url_stream.h` & `libfsxfs-20240501/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_icelandic.h` & `libfsxfs-20240501/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_koi8_u.h` & `libfsxfs-20240501/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_utf16_stream.c` & `libfsxfs-20240501/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_windows_1253.c` & `libfsxfs-20240501/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_iso_8859_4.h` & `libfsxfs-20240501/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_greek.c` & `libfsxfs-20240501/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_libcerror.h` & `libfsxfs-20240501/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_centraleurroman.c` & `libfsxfs-20240501/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_windows_1254.c` & `libfsxfs-20240501/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_iso_8859_13.h` & `libfsxfs-20240501/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_iso_8859_7.h` & `libfsxfs-20240501/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_windows_1255.h` & `libfsxfs-20240501/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_unicode_character.h` & `libfsxfs-20240501/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_iso_8859_8.h` & `libfsxfs-20240501/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_iso_8859_13.c` & `libfsxfs-20240501/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_windows_949.h` & `libfsxfs-20240501/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_cyrillic.c` & `libfsxfs-20240501/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_celtic.c` & `libfsxfs-20240501/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_support.h` & `libfsxfs-20240501/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_iso_8859_4.c` & `libfsxfs-20240501/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_windows_949.c` & `libfsxfs-20240501/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_utf16_stream.h` & `libfsxfs-20240501/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_symbol.c` & `libfsxfs-20240501/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_roman.h` & `libfsxfs-20240501/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_windows_1257.c` & `libfsxfs-20240501/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_windows_1254.h` & `libfsxfs-20240501/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_windows_950.c` & `libfsxfs-20240501/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_extern.h` & `libfsxfs-20240501/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_windows_1256.c` & `libfsxfs-20240501/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_types.h` & `libfsxfs-20240501/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_base32_stream.h` & `libfsxfs-20240501/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_windows_1253.h` & `libfsxfs-20240501/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_iso_8859_16.h` & `libfsxfs-20240501/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_utf8_stream.c` & `libfsxfs-20240501/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_windows_1250.h` & `libfsxfs-20240501/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_iso_8859_2.c` & `libfsxfs-20240501/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_support.c` & `libfsxfs-20240501/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_koi8_r.c` & `libfsxfs-20240501/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_iso_8859_5.h` & `libfsxfs-20240501/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_utf16_string.h` & `libfsxfs-20240501/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_utf32_string.c` & `libfsxfs-20240501/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_icelandic.c` & `libfsxfs-20240501/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_windows_1256.h` & `libfsxfs-20240501/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_utf32_string.h` & `libfsxfs-20240501/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_romanian.h` & `libfsxfs-20240501/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_iso_8859_8.c` & `libfsxfs-20240501/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_koi8_r.h` & `libfsxfs-20240501/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_cyrillic.h` & `libfsxfs-20240501/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_arabic.c` & `libfsxfs-20240501/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_croatian.c` & `libfsxfs-20240501/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_iso_8859_9.h` & `libfsxfs-20240501/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_greek.h` & `libfsxfs-20240501/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_windows_1258.h` & `libfsxfs-20240501/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_iso_8859_7.c` & `libfsxfs-20240501/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/Makefile.in` & `libfsxfs-20240501/libuna/Makefile.in`

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

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_iso_8859_3.c` & `libfsxfs-20240501/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_windows_1250.c` & `libfsxfs-20240501/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_scsu.c` & `libfsxfs-20240501/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_windows_1252.c` & `libfsxfs-20240501/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_turkish.c` & `libfsxfs-20240501/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_ukrainian.h` & `libfsxfs-20240501/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_russian.c` & `libfsxfs-20240501/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_windows_1258.c` & `libfsxfs-20240501/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_celtic.h` & `libfsxfs-20240501/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_byte_stream.c` & `libfsxfs-20240501/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_gaelic.h` & `libfsxfs-20240501/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_utf32_stream.h` & `libfsxfs-20240501/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_symbol.h` & `libfsxfs-20240501/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_windows_1257.h` & `libfsxfs-20240501/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_inuit.h` & `libfsxfs-20240501/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_mac_farsi.c` & `libfsxfs-20240501/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_windows_950.h` & `libfsxfs-20240501/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_url_stream.c` & `libfsxfs-20240501/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_windows_1251.h` & `libfsxfs-20240501/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_windows_1252.h` & `libfsxfs-20240501/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_codepage_iso_8859_14.h` & `libfsxfs-20240501/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_base16_stream.h` & `libfsxfs-20240501/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libuna/libuna_base32_stream.c` & `libfsxfs-20240501/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/Makefile.in` & `libfsxfs-20240501/Makefile.in`

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
+	libfsxfs.pc \
+	libfsxfs.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libfsxfs.pc
 
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
 	(cd $(srcdir)/libfsxfs && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libfsxfs.pc
-	-rm -f libfsxfs.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfsxfs-20240222/libcnotify/libcnotify_definitions.h` & `libfsxfs-20240501/libcnotify/libcnotify_definitions.h`

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

### Comparing `libfsxfs-20240222/libcnotify/libcnotify_extern.h` & `libfsxfs-20240501/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcnotify/libcnotify_support.c` & `libfsxfs-20240501/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcnotify/libcnotify_stream.h` & `libfsxfs-20240501/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcnotify/Makefile.am` & `libfsxfs-20240501/libcnotify/Makefile.am`

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

### Comparing `libfsxfs-20240222/libcnotify/libcnotify_unused.h` & `libfsxfs-20240501/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcnotify/libcnotify_verbose.h` & `libfsxfs-20240501/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcnotify/libcnotify_print.h` & `libfsxfs-20240501/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcnotify/libcnotify_stream.c` & `libfsxfs-20240501/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcnotify/libcnotify_support.h` & `libfsxfs-20240501/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcnotify/libcnotify_verbose.c` & `libfsxfs-20240501/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcnotify/Makefile.in` & `libfsxfs-20240501/libcnotify/Makefile.in`

 * *Files 2% similar despite different names*

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

### Comparing `libfsxfs-20240222/libcnotify/libcnotify_libcerror.h` & `libfsxfs-20240501/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcnotify/libcnotify_print.c` & `libfsxfs-20240501/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcerror/libcerror_system.c` & `libfsxfs-20240501/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcerror/libcerror_error.c` & `libfsxfs-20240501/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcerror/libcerror_extern.h` & `libfsxfs-20240501/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcerror/Makefile.am` & `libfsxfs-20240501/libcerror/Makefile.am`

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

### Comparing `libfsxfs-20240222/libcerror/libcerror_types.h` & `libfsxfs-20240501/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcerror/libcerror_support.h` & `libfsxfs-20240501/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcerror/libcerror_error.h` & `libfsxfs-20240501/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcerror/libcerror_system.h` & `libfsxfs-20240501/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcerror/libcerror_definitions.h` & `libfsxfs-20240501/libcerror/libcerror_definitions.h`

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

### Comparing `libfsxfs-20240222/libcerror/libcerror_support.c` & `libfsxfs-20240501/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcerror/libcerror_unused.h` & `libfsxfs-20240501/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libcerror/Makefile.in` & `libfsxfs-20240501/libcerror/Makefile.in`

 * *Files 1% similar despite different names*

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

### Comparing `libfsxfs-20240222/libfdatetime/libfdatetime_floatingtime.h` & `libfsxfs-20240501/libfdatetime/libfdatetime_floatingtime.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdatetime/libfdatetime_nsf_timedate.c` & `libfsxfs-20240501/libfdatetime/libfdatetime_nsf_timedate.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdatetime/libfdatetime_error.h` & `libfsxfs-20240501/libfdatetime/libfdatetime_error.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdatetime/libfdatetime_floatingtime.c` & `libfsxfs-20240501/libfdatetime/libfdatetime_floatingtime.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdatetime/libfdatetime_support.h` & `libfsxfs-20240501/libfdatetime/libfdatetime_support.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdatetime/libfdatetime_hfs_time.h` & `libfsxfs-20240501/libfdatetime/libfdatetime_hfs_time.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdatetime/libfdatetime_definitions.h` & `libfsxfs-20240501/libfdatetime/libfdatetime_definitions.h`

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

### Comparing `libfsxfs-20240222/libfdatetime/libfdatetime_hfs_time.c` & `libfsxfs-20240501/libfdatetime/libfdatetime_hfs_time.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdatetime/Makefile.am` & `libfsxfs-20240501/libfdatetime/Makefile.am`

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

### Comparing `libfsxfs-20240222/libfdatetime/libfdatetime_filetime.c` & `libfsxfs-20240501/libfdatetime/libfdatetime_filetime.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdatetime/libfdatetime_systemtime.h` & `libfsxfs-20240501/libfdatetime/libfdatetime_systemtime.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdatetime/libfdatetime_extern.h` & `libfsxfs-20240501/libfdatetime/libfdatetime_extern.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdatetime/libfdatetime_posix_time.c` & `libfsxfs-20240501/libfdatetime/libfdatetime_posix_time.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdatetime/libfdatetime_unused.h` & `libfsxfs-20240501/libfdatetime/libfdatetime_unused.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdatetime/libfdatetime_fat_date_time.h` & `libfsxfs-20240501/libfdatetime/libfdatetime_fat_date_time.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdatetime/libfdatetime_systemtime.c` & `libfsxfs-20240501/libfdatetime/libfdatetime_systemtime.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdatetime/libfdatetime_nsf_timedate.h` & `libfsxfs-20240501/libfdatetime/libfdatetime_nsf_timedate.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdatetime/libfdatetime_libcerror.h` & `libfsxfs-20240501/libfdatetime/libfdatetime_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdatetime/libfdatetime_support.c` & `libfsxfs-20240501/libfdatetime/libfdatetime_support.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdatetime/libfdatetime_error.c` & `libfsxfs-20240501/libfdatetime/libfdatetime_error.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdatetime/libfdatetime_posix_time.h` & `libfsxfs-20240501/libfdatetime/libfdatetime_posix_time.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdatetime/libfdatetime_date_time_values.h` & `libfsxfs-20240501/libfdatetime/libfdatetime_date_time_values.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdatetime/libfdatetime_filetime.h` & `libfsxfs-20240501/libfdatetime/libfdatetime_filetime.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdatetime/libfdatetime_date_time_values.c` & `libfsxfs-20240501/libfdatetime/libfdatetime_date_time_values.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdatetime/libfdatetime_types.h` & `libfsxfs-20240501/libfdatetime/libfdatetime_types.h`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/libfdatetime/Makefile.in` & `libfsxfs-20240501/libfdatetime/Makefile.in`

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

### Comparing `libfsxfs-20240222/libfdatetime/libfdatetime_fat_date_time.c` & `libfsxfs-20240501/libfdatetime/libfdatetime_fat_date_time.c`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/aclocal.m4` & `libfsxfs-20240501/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libfsxfs-20240222/configure.ac` & `libfsxfs-20240501/configure.ac`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libfsxfs],
- [20240222],
+ [20240501],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libfsxfs.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

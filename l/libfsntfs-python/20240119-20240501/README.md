# Comparing `tmp/libfsntfs-python-20240119.tar.gz` & `tmp/libfsntfs-python-20240501.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libfsntfs-python-20240119.tar", last modified: Fri Jan 19 20:20:10 2024, max compression
+gzip compressed data, was "libfsntfs-python-20240501.tar", last modified: Wed May  1 09:45:01 2024, max compression
```

## Comparing `libfsntfs-python-20240119.tar` & `libfsntfs-python-20240501.tar`

### file list

```diff
@@ -1,1249 +1,1249 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:08.000000 libfsntfs-20240119/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_area.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_mapped_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1291 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_area.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_mapped_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_segments_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_segments_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34463 2024-01-19 18:57:45.000000 libfsntfs-20240119/libfdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-01-19 18:57:25.000000 libfsntfs-20240119/libfdata/libfdata_vector.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-01-19 04:04:50.000000 libfsntfs-20240119/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-01-19 18:57:44.000000 libfsntfs-20240119/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 04:04:50.000000 libfsntfs-20240119/NEWS
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2545 2024-01-19 18:57:55.000000 libfsntfs-20240119/libfsntfs.spec
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/pyfsntfs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1881 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8886 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2872 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_guid.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5521 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_security_descriptor_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8894 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3190 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_mft_metadata_file_entries.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1549 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1777 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_file_attribute_flags.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10060 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_object_identifier_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23169 2024-01-19 04:07:50.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_volume_information_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1361 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23602 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_standard_information_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1507 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2918 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_volume_file_entries.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9460 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_reparse_point_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1553 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_security_descriptor_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2533 2023-12-03 09:07:00.000000 libfsntfs-20240119/pyfsntfs/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40011 2024-01-19 04:07:50.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6734 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_volume_information_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    96932 2024-01-19 04:07:50.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2064 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_object_identifier_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8966 2024-01-19 04:07:50.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_file_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2036 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10741 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_volume_file_entries.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2297 2024-01-19 04:07:50.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_usn_change_journal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9495 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_data_streams.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33969 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_file_object_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1837 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_datetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12627 2024-01-19 04:07:50.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4156 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_file_object_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1553 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16625 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_datetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1809 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_reparse_point_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3400 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_standard_information_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23738 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_file_name_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3228 2024-01-19 04:07:50.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_mft_metadata_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3956 2024-01-19 04:07:50.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1180 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_guid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_data_streams.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1528 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9341 2024-01-19 04:07:50.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3169 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_file_name_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_file_entries.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_attribute_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_volume_name_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9566 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27880 2024-01-19 04:07:50.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_data_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9481 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_file_entries.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1701 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23657 2024-01-19 04:07:50.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_mft_metadata_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10659 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_attribute_types.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11552 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_mft_metadata_file_entries.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_libfsntfs.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2386 2024-01-19 04:07:50.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    79617 2024-01-19 18:57:45.000000 libfsntfs-20240119/pyfsntfs/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3199 2024-01-19 04:07:50.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_data_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10577 2024-01-19 04:07:50.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_usn_change_journal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10377 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_file_attribute_flags.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5315 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_volume_name_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-01-19 04:04:53.000000 libfsntfs-20240119/pyfsntfs/pyfsntfs_unused.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-01-19 18:57:45.000000 libfsntfs-20240119/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:08.000000 libfsntfs-20240119/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-01-19 18:57:27.000000 libfsntfs-20240119/libfguid/libfguid_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-01-19 18:57:27.000000 libfsntfs-20240119/libfguid/libfguid_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-01-19 18:57:27.000000 libfsntfs-20240119/libfguid/libfguid_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-01-19 18:57:27.000000 libfsntfs-20240119/libfguid/libfguid_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      681 2024-01-19 18:57:27.000000 libfsntfs-20240119/libfguid/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-01-19 18:57:27.000000 libfsntfs-20240119/libfguid/libfguid_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-01-19 18:57:27.000000 libfsntfs-20240119/libfguid/libfguid_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-01-19 18:57:27.000000 libfsntfs-20240119/libfguid/libfguid_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-01-19 18:57:27.000000 libfsntfs-20240119/libfguid/libfguid_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-01-19 18:57:27.000000 libfsntfs-20240119/libfguid/libfguid_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-01-19 18:57:27.000000 libfsntfs-20240119/libfguid/libfguid_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30678 2024-01-19 18:57:45.000000 libfsntfs-20240119/libfguid/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-01-19 18:57:27.000000 libfsntfs-20240119/libfguid/libfguid_error.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:07.000000 libfsntfs-20240119/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8809 2023-12-03 09:06:58.000000 libfsntfs-20240119/m4/libfwnt.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2023-12-03 09:06:57.000000 libfsntfs-20240119/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18233 2023-12-03 09:06:58.000000 libfsntfs-20240119/m4/libfdatetime.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:06:58.000000 libfsntfs-20240119/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2023-12-03 09:06:58.000000 libfsntfs-20240119/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:06:57.000000 libfsntfs-20240119/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:06:57.000000 libfsntfs-20240119/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31269 2023-12-03 09:06:57.000000 libfsntfs-20240119/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:06:57.000000 libfsntfs-20240119/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:06:58.000000 libfsntfs-20240119/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2023-12-03 09:06:58.000000 libfsntfs-20240119/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-12-03 09:06:57.000000 libfsntfs-20240119/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2023-12-03 09:06:57.000000 libfsntfs-20240119/m4/libcsplit.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 09:06:57.000000 libfsntfs-20240119/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-12-03 09:06:58.000000 libfsntfs-20240119/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-01-19 18:57:40.000000 libfsntfs-20240119/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-01-19 18:57:40.000000 libfsntfs-20240119/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15545 2023-12-03 09:06:57.000000 libfsntfs-20240119/m4/libfdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:06:57.000000 libfsntfs-20240119/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4527 2023-12-03 09:06:57.000000 libfsntfs-20240119/m4/libfusn.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5232 2023-12-03 09:06:58.000000 libfsntfs-20240119/m4/libfuse.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-01-19 18:57:39.000000 libfsntfs-20240119/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:06:57.000000 libfsntfs-20240119/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 09:06:58.000000 libfsntfs-20240119/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-12-03 09:06:58.000000 libfsntfs-20240119/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2023-12-03 09:06:58.000000 libfsntfs-20240119/m4/libfguid.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2023-12-03 09:06:58.000000 libfsntfs-20240119/m4/libbfio.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8319 2023-12-03 09:06:57.000000 libfsntfs-20240119/m4/libhmac.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:06:57.000000 libfsntfs-20240119/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-01-19 18:57:40.000000 libfsntfs-20240119/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:06:57.000000 libfsntfs-20240119/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:06:58.000000 libfsntfs-20240119/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-01-19 18:57:39.000000 libfsntfs-20240119/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:06:58.000000 libfsntfs-20240119/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:06:58.000000 libfsntfs-20240119/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27481 2023-12-03 09:06:58.000000 libfsntfs-20240119/m4/libcrypto.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:06:57.000000 libfsntfs-20240119/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7325 2023-12-03 09:06:58.000000 libfsntfs-20240119/m4/libfcache.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-12-03 09:06:58.000000 libfsntfs-20240119/m4/pthread.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:07.000000 libfsntfs-20240119/include/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    65343 2024-01-19 18:57:55.000000 libfsntfs-20240119/include/libfsntfs.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    65343 2024-01-19 04:04:52.000000 libfsntfs-20240119/include/libfsntfs.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      489 2024-01-19 04:04:50.000000 libfsntfs-20240119/include/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:07.000000 libfsntfs-20240119/include/libfsntfs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4079 2024-01-19 04:04:52.000000 libfsntfs-20240119/include/libfsntfs/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4077 2024-01-19 18:57:55.000000 libfsntfs-20240119/include/libfsntfs/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5224 2024-01-19 04:04:52.000000 libfsntfs-20240119/include/libfsntfs/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-01-19 18:57:55.000000 libfsntfs-20240119/include/libfsntfs/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-01-19 04:04:52.000000 libfsntfs-20240119/include/libfsntfs/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-01-19 04:04:52.000000 libfsntfs-20240119/include/libfsntfs/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1436 2024-01-19 04:04:52.000000 libfsntfs-20240119/include/libfsntfs/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1499 2024-01-19 18:57:55.000000 libfsntfs-20240119/include/libfsntfs/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5422 2024-01-19 04:04:52.000000 libfsntfs-20240119/include/libfsntfs/codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29243 2024-01-19 18:57:44.000000 libfsntfs-20240119/include/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:07.000000 libfsntfs-20240119/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-01-19 04:04:52.000000 libfsntfs-20240119/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-01-19 04:04:52.000000 libfsntfs-20240119/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-01-19 04:04:52.000000 libfsntfs-20240119/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-01-19 04:04:52.000000 libfsntfs-20240119/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-01-19 04:04:52.000000 libfsntfs-20240119/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-01-19 04:04:52.000000 libfsntfs-20240119/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-01-19 04:04:52.000000 libfsntfs-20240119/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-01-19 04:04:50.000000 libfsntfs-20240119/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-01-19 04:04:52.000000 libfsntfs-20240119/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-01-19 18:57:55.000000 libfsntfs-20240119/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18422 2024-01-19 18:57:44.000000 libfsntfs-20240119/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19504 2024-01-19 04:23:24.000000 libfsntfs-20240119/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-01-19 04:04:52.000000 libfsntfs-20240119/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-01-19 04:04:52.000000 libfsntfs-20240119/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-01-19 04:04:52.000000 libfsntfs-20240119/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26231 2024-01-19 18:57:44.000000 libfsntfs-20240119/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:08.000000 libfsntfs-20240119/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-01-19 18:57:17.000000 libfsntfs-20240119/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-01-19 18:57:17.000000 libfsntfs-20240119/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2024-01-19 18:57:17.000000 libfsntfs-20240119/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-01-19 18:57:17.000000 libfsntfs-20240119/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-01-19 18:57:17.000000 libfsntfs-20240119/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-01-19 18:57:17.000000 libfsntfs-20240119/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-01-19 18:57:17.000000 libfsntfs-20240119/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-01-19 18:57:17.000000 libfsntfs-20240119/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-01-19 18:57:17.000000 libfsntfs-20240119/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-01-19 18:57:17.000000 libfsntfs-20240119/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31234 2024-01-19 18:57:45.000000 libfsntfs-20240119/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-01-19 18:57:17.000000 libfsntfs-20240119/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-01-19 18:57:17.000000 libfsntfs-20240119/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-01-19 18:57:17.000000 libfsntfs-20240119/libclocale/libclocale_codepage.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:08.000000 libfsntfs-20240119/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-01-19 18:57:23.000000 libfsntfs-20240119/libfcache/libfcache_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-01-19 18:57:23.000000 libfsntfs-20240119/libfcache/libfcache_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-01-19 18:57:23.000000 libfsntfs-20240119/libfcache/libfcache_cache_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-01-19 18:57:23.000000 libfsntfs-20240119/libfcache/libfcache_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-01-19 18:57:23.000000 libfsntfs-20240119/libfcache/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-01-19 18:57:23.000000 libfsntfs-20240119/libfcache/libfcache_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-01-19 18:57:23.000000 libfsntfs-20240119/libfcache/libfcache_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-01-19 18:57:23.000000 libfsntfs-20240119/libfcache/libfcache_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-01-19 18:57:23.000000 libfsntfs-20240119/libfcache/libfcache_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-01-19 18:57:23.000000 libfsntfs-20240119/libfcache/libfcache_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-01-19 18:57:23.000000 libfsntfs-20240119/libfcache/libfcache_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-01-19 18:57:23.000000 libfsntfs-20240119/libfcache/libfcache_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-01-19 18:57:23.000000 libfsntfs-20240119/libfcache/libfcache_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-01-19 18:57:23.000000 libfsntfs-20240119/libfcache/libfcache_cache_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31707 2024-01-19 18:57:45.000000 libfsntfs-20240119/libfcache/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-01-19 18:57:23.000000 libfsntfs-20240119/libfcache/libfcache_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-01-19 18:57:23.000000 libfsntfs-20240119/libfcache/libfcache_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-01-19 18:57:23.000000 libfsntfs-20240119/libfcache/libfcache_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2390 2023-12-03 09:06:56.000000 libfsntfs-20240119/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:08.000000 libfsntfs-20240119/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_file_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_file_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_file_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_file_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_file_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_file_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_memory_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_file_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_file_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_memory_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_memory_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34693 2024-01-19 18:57:44.000000 libfsntfs-20240119/libbfio/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_memory_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-01-19 18:57:11.000000 libfsntfs-20240119/libbfio/libbfio_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:06:56.000000 libfsntfs-20240119/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-01-19 18:57:44.000000 libfsntfs-20240119/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:07.000000 libfsntfs-20240119/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-01-19 04:04:50.000000 libfsntfs-20240119/dpkg/libfsntfs-tools.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1028 2024-01-19 04:04:54.000000 libfsntfs-20240119/dpkg/copyright
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:07.000000 libfsntfs-20240119/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-01-19 04:04:50.000000 libfsntfs-20240119/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2240 2024-01-19 04:04:50.000000 libfsntfs-20240119/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      777 2024-01-19 04:04:50.000000 libfsntfs-20240119/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-01-19 04:04:50.000000 libfsntfs-20240119/dpkg/libfsntfs-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      122 2024-01-19 04:04:50.000000 libfsntfs-20240119/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      141 2024-01-19 18:57:55.000000 libfsntfs-20240119/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-01-19 04:04:50.000000 libfsntfs-20240119/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-01-19 04:04:50.000000 libfsntfs-20240119/dpkg/libfsntfs.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-01-19 04:04:50.000000 libfsntfs-20240119/dpkg/libfsntfs-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      489 2024-01-19 18:57:55.000000 libfsntfs-20240119/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-01-19 04:04:50.000000 libfsntfs-20240119/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  2047730 2024-01-19 18:57:43.000000 libfsntfs-20240119/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-01-19 18:57:44.000000 libfsntfs-20240119/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-01-19 18:57:44.000000 libfsntfs-20240119/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-01-19 04:05:18.000000 libfsntfs-20240119/msvscpp/libfdata/libfdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_directory_entries_tree/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6169 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_directory_entries_tree/fsntfs_test_directory_entries_tree.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_file_name_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6068 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_file_name_values/fsntfs_test_file_name_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_index_node/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6050 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_index_node/fsntfs_test_index_node.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_volume_information_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6095 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_volume_information_values/fsntfs_test_volume_information_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_io_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6047 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_io_handle/fsntfs_test_io_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_compressed_block_data_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6357 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_compressed_block_data_handle/fsntfs_test_compressed_block_data_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_object_identifier_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6092 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_object_identifier_values/fsntfs_test_object_identifier_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_profiler/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6044 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_profiler/fsntfs_test_profiler.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_data_stream/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6470 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_data_stream/fsntfs_test_data_stream.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/pyfsntfs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10444 2024-01-19 04:05:18.000000 libfsntfs-20240119/msvscpp/pyfsntfs/pyfsntfs.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_security_descriptor_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6352 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_security_descriptor_values/fsntfs_test_security_descriptor_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_file_system/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6470 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_file_system/fsntfs_test_file_system.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_tools_info_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6628 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_tools_info_handle/fsntfs_test_tools_info_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-01-19 04:05:18.000000 libfsntfs-20240119/msvscpp/libfguid/libfguid.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5786 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_error/fsntfs_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_mft_attribute_list_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6176 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_mft_attribute_list_entry/fsntfs_test_mft_attribute_list_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_mft_entry_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6068 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_mft_entry_header/fsntfs_test_mft_entry_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_buffer_data_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6074 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_buffer_data_handle/fsntfs_test_buffer_data_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_file_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6467 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_file_entry/fsntfs_test_file_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_reparse_point_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6080 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_reparse_point_values/fsntfs_test_reparse_point_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_security_descriptor_index/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6178 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_security_descriptor_index/fsntfs_test_security_descriptor_index.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-01-19 04:05:18.000000 libfsntfs-20240119/msvscpp/libclocale/libclocale.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_index/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6035 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_index/fsntfs_test_index.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfsinfo/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7959 2024-01-19 04:05:18.000000 libfsntfs-20240119/msvscpp/fsntfsinfo/fsntfsinfo.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_index_entry_vector/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6496 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_index_entry_vector/fsntfs_test_index_entry_vector.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-01-19 04:05:18.000000 libfsntfs-20240119/msvscpp/libfcache/libfcache.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5606 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-01-19 04:05:18.000000 libfsntfs-20240119/msvscpp/libbfio/libbfio.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_fixup_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5892 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_fixup_values/fsntfs_test_fixup_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_index_root_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6071 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_index_root_header/fsntfs_test_index_root_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_index_value/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6053 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_index_value/fsntfs_test_index_value.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_compression/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5889 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_compression/fsntfs_test_compression.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_attribute/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6211 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_attribute/fsntfs_test_attribute.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_index_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6306 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_index_entry/fsntfs_test_index_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_mft_metadata_file/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6824 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_mft_metadata_file/fsntfs_test_mft_metadata_file.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_sds_index_value/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6065 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_sds_index_value/fsntfs_test_sds_index_value.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_security_descriptor_index_value/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6113 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_security_descriptor_index_value/fsntfs_test_security_descriptor_index_value.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_mft_attribute_list/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6158 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_mft_attribute_list/fsntfs_test_mft_attribute_list.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_standard_information_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6101 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_standard_information_values/fsntfs_test_standard_information_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_mft_attribute/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6143 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_mft_attribute/fsntfs_test_mft_attribute.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-01-19 04:05:18.000000 libfsntfs-20240119/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_usn_change_journal/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6238 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_usn_change_journal/fsntfs_test_usn_change_journal.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_compressed_block_vector/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6511 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_compressed_block_vector/fsntfs_test_compressed_block_vector.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_volume_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6312 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_volume_header/fsntfs_test_volume_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_tools_mount_path_string/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6014 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_tools_mount_path_string/fsntfs_test_tools_mount_path_string.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-01-19 04:05:18.000000 libfsntfs-20240119/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_volume_name_attribute/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6083 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_volume_name_attribute/fsntfs_test_volume_name_attribute.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_txf_data_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6065 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_txf_data_values/fsntfs_test_txf_data_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_compression_unit_descriptor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6101 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_compression_unit_descriptor/fsntfs_test_compression_unit_descriptor.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_directory_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6149 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_directory_entry/fsntfs_test_directory_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_tools_digest_hash/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5984 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_tools_digest_hash/fsntfs_test_tools_digest_hash.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_data_run/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6128 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_data_run/fsntfs_test_data_run.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_compressed_block/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6068 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_compressed_block/fsntfs_test_compressed_block.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_volume_information_attribute/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6104 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_volume_information_attribute/fsntfs_test_volume_information_attribute.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_mft/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6029 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_mft/fsntfs_test_mft.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_reparse_point_attribute/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6089 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_reparse_point_attribute/fsntfs_test_reparse_point_attribute.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-01-19 04:05:18.000000 libfsntfs-20240119/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_file_name_attribute/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6077 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_file_name_attribute/fsntfs_test_file_name_attribute.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_index_entry_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6074 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_index_entry_header/fsntfs_test_index_entry_header.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    87512 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/libfsntfs.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-01-19 04:05:18.000000 libfsntfs-20240119/msvscpp/libcpath/libcpath.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5874 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_notify/fsntfs_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfsmount/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8022 2024-01-19 04:05:18.000000 libfsntfs-20240119/msvscpp/fsntfsmount/fsntfsmount.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_cluster_block/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6312 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_cluster_block/fsntfs_test_cluster_block.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_tools_path_string/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6068 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_tools_path_string/fsntfs_test_tools_path_string.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_cluster_block_stream/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6164 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_cluster_block_stream/fsntfs_test_cluster_block_stream.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/libfusn/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5308 2024-01-19 04:05:18.000000 libfsntfs-20240119/msvscpp/libfusn/libfusn.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_cluster_block_vector/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6502 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_cluster_block_vector/fsntfs_test_cluster_block_vector.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_tools_output/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5983 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_tools_output/fsntfs_test_tools_output.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_volume/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6873 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_volume/fsntfs_test_volume.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/libfwnt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6895 2024-01-19 04:05:18.000000 libfsntfs-20240119/msvscpp/libfwnt/libfwnt.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_tools_bodyfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6053 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_tools_bodyfile/fsntfs_test_tools_bodyfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/libfsntfs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20944 2024-01-19 04:05:18.000000 libfsntfs-20240119/msvscpp/libfsntfs/libfsntfs.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_name/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6032 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_name/fsntfs_test_name.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_extent/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6038 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_extent/fsntfs_test_extent.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_index_node_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6071 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_index_node_header/fsntfs_test_index_node_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/libhmac/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6182 2024-01-19 04:05:18.000000 libfsntfs-20240119/msvscpp/libhmac/libhmac.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_attribute_list_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6080 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_attribute_list_entry/fsntfs_test_attribute_list_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-01-19 04:05:18.000000 libfsntfs-20240119/msvscpp/libcsplit/libcsplit.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_bitmap_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6059 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_bitmap_values/fsntfs_test_bitmap_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_logged_utility_stream_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6104 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_logged_utility_stream_values/fsntfs_test_logged_utility_stream_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-01-19 04:05:18.000000 libfsntfs-20240119/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28805 2024-01-19 18:57:45.000000 libfsntfs-20240119/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_cluster_block_data/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6411 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_cluster_block_data/fsntfs_test_cluster_block_data.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_tools_signal/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5983 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_tools_signal/fsntfs_test_tools_signal.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_volume_name_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6074 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_volume_name_values/fsntfs_test_volume_name_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6712 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_support/fsntfs_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-01-19 04:05:18.000000 libfsntfs-20240119/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_path_hint/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6047 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_path_hint/fsntfs_test_path_hint.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_compressed_data_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6170 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_compressed_data_handle/fsntfs_test_compressed_data_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_mft_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6300 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_mft_entry/fsntfs_test_mft_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-01-19 04:05:18.000000 libfsntfs-20240119/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-01-19 04:05:18.000000 libfsntfs-20240119/msvscpp/libfdatetime/libfdatetime.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/msvscpp/fsntfs_test_compression_unit_data_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6104 2024-01-19 04:07:27.000000 libfsntfs-20240119/msvscpp/fsntfs_test_compression_unit_data_handle/fsntfs_test_compression_unit_data_handle.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       93 2024-01-19 04:04:52.000000 libfsntfs-20240119/AUTHORS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:08.000000 libfsntfs-20240119/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-01-19 18:57:15.000000 libfsntfs-20240119/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-01-19 18:57:15.000000 libfsntfs-20240119/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-01-19 18:57:15.000000 libfsntfs-20240119/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-01-19 18:57:15.000000 libfsntfs-20240119/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-01-19 18:57:15.000000 libfsntfs-20240119/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-01-19 18:57:15.000000 libfsntfs-20240119/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      942 2024-01-19 18:57:15.000000 libfsntfs-20240119/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-01-19 18:57:15.000000 libfsntfs-20240119/libcfile/libcfile_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-01-19 18:57:15.000000 libfsntfs-20240119/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-01-19 18:57:15.000000 libfsntfs-20240119/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-01-19 18:57:15.000000 libfsntfs-20240119/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-01-19 18:57:15.000000 libfsntfs-20240119/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-01-19 18:57:15.000000 libfsntfs-20240119/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-01-19 18:57:15.000000 libfsntfs-20240119/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-01-19 18:57:15.000000 libfsntfs-20240119/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-01-19 18:57:15.000000 libfsntfs-20240119/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-01-19 18:57:15.000000 libfsntfs-20240119/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31998 2024-01-19 18:57:45.000000 libfsntfs-20240119/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-01-19 18:57:15.000000 libfsntfs-20240119/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-01-19 18:57:15.000000 libfsntfs-20240119/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-01-19 18:57:15.000000 libfsntfs-20240119/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-01-19 18:57:15.000000 libfsntfs-20240119/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      684 2024-01-19 04:04:50.000000 libfsntfs-20240119/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-01-19 18:57:44.000000 libfsntfs-20240119/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:08.000000 libfsntfs-20240119/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1127 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33682 2024-01-19 18:57:44.000000 libfsntfs-20240119/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-01-19 18:57:13.000000 libfsntfs-20240119/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-01-19 04:04:50.000000 libfsntfs-20240119/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      490 2024-01-19 04:04:50.000000 libfsntfs-20240119/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-01-19 18:57:44.000000 libfsntfs-20240119/config.sub
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      757 2024-01-19 04:04:50.000000 libfsntfs-20240119/libfsntfs.pc.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-01-19 04:04:50.000000 libfsntfs-20240119/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1816 2024-01-19 04:07:50.000000 libfsntfs-20240119/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:06:56.000000 libfsntfs-20240119/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:07.000000 libfsntfs-20240119/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-01-19 18:57:22.000000 libfsntfs-20240119/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-01-19 18:57:22.000000 libfsntfs-20240119/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-01-19 18:57:22.000000 libfsntfs-20240119/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-01-19 18:57:22.000000 libfsntfs-20240119/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-01-19 18:57:22.000000 libfsntfs-20240119/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-01-19 18:57:22.000000 libfsntfs-20240119/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-01-19 18:57:22.000000 libfsntfs-20240119/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-01-19 18:57:22.000000 libfsntfs-20240119/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-01-19 18:57:22.000000 libfsntfs-20240119/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-01-19 18:57:22.000000 libfsntfs-20240119/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-01-19 18:57:22.000000 libfsntfs-20240119/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-01-19 18:57:22.000000 libfsntfs-20240119/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-01-19 18:57:22.000000 libfsntfs-20240119/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-01-19 18:57:22.000000 libfsntfs-20240119/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-01-19 18:57:22.000000 libfsntfs-20240119/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-01-19 18:57:22.000000 libfsntfs-20240119/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-01-19 18:57:22.000000 libfsntfs-20240119/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-01-19 18:57:22.000000 libfsntfs-20240119/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-01-19 18:57:22.000000 libfsntfs-20240119/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-01-19 18:57:22.000000 libfsntfs-20240119/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-01-19 18:57:22.000000 libfsntfs-20240119/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-01-19 18:57:22.000000 libfsntfs-20240119/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-01-19 18:57:22.000000 libfsntfs-20240119/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-01-19 18:57:22.000000 libfsntfs-20240119/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-01-19 18:57:22.000000 libfsntfs-20240119/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-01-19 18:57:22.000000 libfsntfs-20240119/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-01-19 18:57:22.000000 libfsntfs-20240119/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34088 2024-01-19 18:57:45.000000 libfsntfs-20240119/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-01-19 18:57:22.000000 libfsntfs-20240119/libcthreads/libcthreads_queue.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/fsntfstools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/fsntfstools_signal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1723 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/mount_path_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37237 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/mount_dokan.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2561 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/mount_file_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5776 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/fsntfstools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28494 2024-01-19 04:07:50.000000 libfsntfs-20240119/fsntfstools/mount_fuse.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9036 2024-01-19 04:07:50.000000 libfsntfs-20240119/fsntfstools/info_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5420 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/mount_dokan.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15540 2024-01-19 04:07:50.000000 libfsntfs-20240119/fsntfstools/fsntfsmount.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4539 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/fsntfstools_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1729 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/path_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3298 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/digest_hash.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13694 2024-01-19 04:07:50.000000 libfsntfs-20240119/fsntfstools/mount_file_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1446 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/fsntfstools_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1489 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/fsntfstools_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1481 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/fsntfstools_output.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1751 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/fsntfstools_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/fsntfstools_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1507 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/fsntfstools_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2825 2023-12-03 09:06:56.000000 libfsntfs-20240119/fsntfstools/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      989 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/fsntfstools_libfsntfs.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1216 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/fsntfstools_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1283 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/bodyfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24694 2024-01-19 04:07:50.000000 libfsntfs-20240119/fsntfstools/mount_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   214387 2024-01-19 04:07:50.000000 libfsntfs-20240119/fsntfstools/info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3829 2024-01-19 04:07:50.000000 libfsntfs-20240119/fsntfstools/mount_file_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1486 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/fsntfstools_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11773 2024-01-19 04:07:50.000000 libfsntfs-20240119/fsntfstools/fsntfsinfo.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/fsntfstools_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/fsntfstools_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/fsntfstools_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1751 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/fsntfstools_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/fsntfstools_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2568 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/mount_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21648 2024-01-19 04:07:50.000000 libfsntfs-20240119/fsntfstools/mount_path_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1774 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/fsntfstools_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1784 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/fsntfstools_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/fsntfstools_libfusn.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16556 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/mount_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1477 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/fsntfstools_libhmac.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36705 2024-01-19 18:57:44.000000 libfsntfs-20240119/fsntfstools/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8836 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/bodyfile.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1245 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/digest_hash.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4584 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/fsntfstools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2856 2024-01-19 04:07:50.000000 libfsntfs-20240119/fsntfstools/mount_fuse.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20256 2024-01-19 04:04:54.000000 libfsntfs-20240119/fsntfstools/path_string.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-01-19 18:57:45.000000 libfsntfs-20240119/test-driver
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:08.000000 libfsntfs-20240119/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-01-19 18:57:19.000000 libfsntfs-20240119/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-01-19 18:57:19.000000 libfsntfs-20240119/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-01-19 18:57:19.000000 libfsntfs-20240119/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      842 2024-01-19 18:57:19.000000 libfsntfs-20240119/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-01-19 18:57:19.000000 libfsntfs-20240119/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-01-19 18:57:19.000000 libfsntfs-20240119/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-01-19 18:57:19.000000 libfsntfs-20240119/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-01-19 18:57:19.000000 libfsntfs-20240119/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-01-19 18:57:19.000000 libfsntfs-20240119/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-01-19 18:57:19.000000 libfsntfs-20240119/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-01-19 18:57:19.000000 libfsntfs-20240119/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-01-19 18:57:19.000000 libfsntfs-20240119/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31276 2024-01-19 18:57:45.000000 libfsntfs-20240119/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-01-19 18:57:19.000000 libfsntfs-20240119/libcpath/libcpath_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-01-19 18:57:19.000000 libfsntfs-20240119/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-01-19 18:57:19.000000 libfsntfs-20240119/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-01-19 18:57:19.000000 libfsntfs-20240119/libcpath/libcpath_path.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12127 2023-12-03 09:06:56.000000 libfsntfs-20240119/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30945 2024-01-19 04:04:54.000000 libfsntfs-20240119/manuals/libfsntfs.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      162 2023-12-03 09:06:57.000000 libfsntfs-20240119/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2097 2024-01-19 04:04:54.000000 libfsntfs-20240119/manuals/fsntfsinfo.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28205 2024-01-19 18:57:45.000000 libfsntfs-20240119/manuals/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42075 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_compressed_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35027 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_volume_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4215 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_tools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35342 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_security_descriptor_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1373 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3179 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26242 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_directory_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27562 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_file_name_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30750 2024-01-19 04:07:50.000000 libfsntfs-20240119/tests/pyfsntfs_test_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19485 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_cluster_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8293 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2469 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_tools_output.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4130 2024-01-19 04:07:50.000000 libfsntfs-20240119/tests/test_tools.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23213 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_attribute_list_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21070 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_mft_entry_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    61128 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_cluster_block_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15073 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_volume_name_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36448 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_index_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8609 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10754 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_compression_unit_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    92407 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_compressed_block_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6929 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_compressed_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11627 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_fixup_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35794 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_mft_attribute_list_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10504 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_security_descriptor_index.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31426 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15448 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15608 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_logged_utility_stream_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1714 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_rwlock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28529 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_standard_information_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4171 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_tools_digest_hash.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1713 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14811 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_volume_information_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9464 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_sds_index_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67794 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_index_entry_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   110662 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_file_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2007 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_functions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    46804 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9711 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_index.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15740 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_functions.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8643 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_extent.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39562 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_reparse_point_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19673 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_tools_mount_path_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6160 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_path_hint.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    51596 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_mft_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_rwlock.c
--rwxr--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/test_manpage.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10607 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_mft.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9304 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_index_node_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4539 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_getopt.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3856 2024-01-19 04:07:50.000000 libfsntfs-20240119/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15536 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_index_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7485 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_tools_bodyfile.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9322 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_index_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17926 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_buffer_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      989 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_libfsntfs.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1712 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4747 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35037 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_directory_entries_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9719 2024-01-19 04:07:50.000000 libfsntfs-20240119/tests/pyfsntfs_test_attribute.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15806 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_index_root_header.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4333 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/test_fsntfsinfo_bodyfile.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11117 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_volume_information_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30542 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_cluster_block_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7132 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_profiler.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    92860 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_cluster_block_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   127913 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_compression.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    59087 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_mft_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8845 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_usn_change_journal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7326 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_compression_unit_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4370 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43184 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_file_name_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13439 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_tools_path_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13963 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_txf_data_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16019 2024-01-19 04:07:50.000000 libfsntfs-20240119/tests/pyfsntfs_test_volume.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100559 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_compressed_block_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1745 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    63509 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15523 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_security_descriptor_index_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31345 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_volume_name_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   259855 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_file_entry.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3403 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/test_fsntfsinfo.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   144131 2024-01-19 18:57:45.000000 libfsntfs-20240119/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1557 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   132840 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_data_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/pyfsntfs_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33492 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_mft_metadata_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12477 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_mft_attribute_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24256 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_name.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23688 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_reparse_point_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14322 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_object_identifier_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5750 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_tools_info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12691 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_data_run.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14470 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_bitmap_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14589 2024-01-19 04:07:27.000000 libfsntfs-20240119/tests/fsntfs_test_index_entry_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1468 2024-01-19 04:04:54.000000 libfsntfs-20240119/tests/fsntfs_test_libclocale.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     5148 2024-01-19 04:07:50.000000 libfsntfs-20240119/tests/test_library.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2255 2024-01-19 04:04:53.000000 libfsntfs-20240119/ossfuzz/volume_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2027 2023-12-03 09:07:03.000000 libfsntfs-20240119/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2430 2024-01-19 04:04:53.000000 libfsntfs-20240119/ossfuzz/mft_metadata_file_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      977 2024-01-19 04:04:53.000000 libfsntfs-20240119/ossfuzz/ossfuzz_libfsntfs.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-01-19 04:04:53.000000 libfsntfs-20240119/ossfuzz/ossfuzz_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3119 2024-01-19 04:04:53.000000 libfsntfs-20240119/ossfuzz/file_entry_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37616 2024-01-19 18:57:45.000000 libfsntfs-20240119/ossfuzz/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/libfusn/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-01-19 18:57:28.000000 libfsntfs-20240119/libfusn/libfusn_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1877 2024-01-19 18:57:28.000000 libfsntfs-20240119/libfusn/libfusn_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26484 2024-01-19 18:57:28.000000 libfsntfs-20240119/libfusn/libfusn_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-01-19 18:57:28.000000 libfsntfs-20240119/libfusn/libfusn_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1375 2024-01-19 18:57:28.000000 libfsntfs-20240119/libfusn/libfusn_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-01-19 18:57:28.000000 libfsntfs-20240119/libfusn/libfusn_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      817 2024-01-19 18:57:28.000000 libfsntfs-20240119/libfusn/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-01-19 18:57:28.000000 libfsntfs-20240119/libfusn/libfusn_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-01-19 18:57:28.000000 libfsntfs-20240119/libfusn/libfusn_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-01-19 18:57:28.000000 libfsntfs-20240119/libfusn/libfusn_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2327 2024-01-19 18:57:28.000000 libfsntfs-20240119/libfusn/fusn_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-01-19 18:57:28.000000 libfsntfs-20240119/libfusn/libfusn_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12280 2024-01-19 18:57:28.000000 libfsntfs-20240119/libfusn/libfusn_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31214 2024-01-19 18:57:45.000000 libfsntfs-20240119/libfusn/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-01-19 18:57:28.000000 libfsntfs-20240119/libfusn/libfusn_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-01-19 18:57:28.000000 libfsntfs-20240119/libfusn/libfusn_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4234 2024-01-19 18:57:28.000000 libfsntfs-20240119/libfusn/libfusn_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1723 2024-01-19 18:57:28.000000 libfsntfs-20240119/libfusn/libfusn_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-01-19 18:57:28.000000 libfsntfs-20240119/libfusn/libfusn_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-01-19 18:57:39.000000 libfsntfs-20240119/ltmain.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:08.000000 libfsntfs-20240119/libfwnt/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_locale_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26551 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_lzxpress.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30230 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_security_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7049 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_bit_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_lznt1.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1348 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5264 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_security_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2072 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_huffman_tree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2795 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_access_control_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27064 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_security_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13639 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_access_control_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3470 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13113 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_huffman_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8377 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15166 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_lznt1.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18859 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_locale_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1464 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2797 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_lzx.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19962 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_access_control_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2326 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_lzxpress.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3336 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_security_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36036 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_lzx.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34903 2024-01-19 18:57:45.000000 libfsntfs-20240119/libfwnt/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2039 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_bit_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1908 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3209 2024-01-19 18:57:30.000000 libfsntfs-20240119/libfwnt/libfwnt_access_control_entry.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/libfsntfs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8711 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_index_entry_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1401 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2807 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_mft.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2829 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_compressed_block_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5756 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_sds_index_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5329 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_directory_entries_tree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23422 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_security_descriptor_index.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9488 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_txf_data_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19693 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_security_descriptor_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32475 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_reparse_point_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1587 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_compressed_block.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4026 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_compressed_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1797 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_index_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1332 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_compression.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8183 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_profiler.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19566 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_standard_information_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2427 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/fsntfs_mft_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12901 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_index_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5499 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_volume_information_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25555 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_cluster_block_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/fsntfs_volume_information.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11491 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_object_identifier_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5429 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9737 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_data_run.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3290 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_attribute_list_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3833 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_index.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2815 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_standard_information_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1706 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2414 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_security_descriptor_index_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20087 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_reparse_point_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    54272 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_mft_metadata_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17017 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_mft_entry_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1880 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/fsntfs_txf_data.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20304 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_standard_information_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12727 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_cluster_block_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7382 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_attribute_list_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1978 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_volume_name_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_cluster_block_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25012 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_volume_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1645 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_attribute_list_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23871 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_compressed_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_index_node_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1469 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/fsntfs_logged_utility_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21101 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_mft_attribute_list_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13566 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_object_identifier_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7849 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_logged_utility_stream_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17579 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_bitmap_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2766 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94395 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16323 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1892 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_cluster_block.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2062 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_object_identifier_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8562 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_index_root_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2373 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6767 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_index_node_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3924 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/fsntfs_mft_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2448 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_index_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6394 2023-12-03 09:06:58.000000 libfsntfs-20240119/libfsntfs/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7028 2024-01-19 18:57:55.000000 libfsntfs-20240119/libfsntfs/libfsntfs_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4755 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_file_name_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/fsntfs_object_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2289 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_txf_data_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19319 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1932 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6301 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_cluster_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1793 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/fsntfs_mft_attribute_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2255 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_volume_information_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39152 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48386 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_file_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9103 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_compression_unit_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4582 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_usn_change_journal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16683 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_mft.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3227 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_security_descriptor_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8168 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_volume_name_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2503 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/fsntfs_standard_information.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3756 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_mft_attribute_list_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29763 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_file_name_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2413 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_index_root_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2574 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6361 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_mft_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4131 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_extent.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    60465 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_mft_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1621 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_volume_information_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18720 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_usn_change_journal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12076 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_compressed_block_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3360 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_directory_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2639 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_compression_unit_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3248 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/fsntfs_volume_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3159 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_security_descriptor_index.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4217 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_standard_information_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15319 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_file_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4008 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_file_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1967 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_name.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1678 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_sds_index_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5165 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_fixup_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1105 2024-01-19 18:57:55.000000 libfsntfs-20240119/libfsntfs/libfsntfs.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13362 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_index_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1286 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_fixup_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1107 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4610 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_cluster_block_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    77724 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_mft_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1909 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/fsntfs_secure.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13040 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_index_entry_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1877 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_cluster_block_vector.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1608 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7978 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_security_descriptor_index_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2343 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_buffer_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2786 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_volume_name_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1677 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_extent.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3950 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_mft_attribute_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12385 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_compressed_block_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29282 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_index.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7850 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_buffer_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1706 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3190 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_reparse_point_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2349 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_path_hint.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2486 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/fsntfs_reparse_point.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2184 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_logged_utility_stream_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4404 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_data_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8832 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_volume_information_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20199 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_file_name_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3149 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/fsntfs_index.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12001 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_index_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2144 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_index_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2005 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2392 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_object_identifier_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3381 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_compressed_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5970 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_mft_metadata_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1729 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2228 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_bitmap_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   171864 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15524 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_directory_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1846 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_cluster_block_data.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2420 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_compression_unit_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22736 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_mft_attribute_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5402 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_security_descriptor_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7030 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1984 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_compressed_block_vector.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23692 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_name.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3207 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_file_name_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55021 2024-01-19 18:57:45.000000 libfsntfs-20240119/libfsntfs/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8311 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28629 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_data_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3874 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_mft_entry_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15709 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_volume_name_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4428 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_reparse_point_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    63741 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_directory_entries_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4088 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_compression.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9290 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_mft_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2038 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_data_run.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8597 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_path_hint.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2253 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_index_entry_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1892 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_index_entry_vector.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1646 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_security_descriptor_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2102 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_profiler.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17815 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_attribute_list_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2318 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/fsntfs_file_name.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20903 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_compression_unit_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3475 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_volume_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-01-19 04:04:53.000000 libfsntfs-20240119/libfsntfs/libfsntfs_unused.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/libhmac/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47989 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_sha1_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_sha224.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50026 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_sha512_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14448 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_md5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2079 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_md5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1942 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9362 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14650 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_sha512.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45648 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_sha256_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_sha224.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1623 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2060 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_sha1.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3443 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_sha256_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1121 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45605 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_sha224_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_md5_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_sha256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3368 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_sha1_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33808 2024-01-19 18:57:45.000000 libfsntfs-20240119/libhmac/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_sha256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3461 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_sha224_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3444 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_sha512_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_sha512.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14514 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_sha1.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40596 2024-01-19 18:57:32.000000 libfsntfs-20240119/libhmac/libhmac_md5_context.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:08.000000 libfsntfs-20240119/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-01-19 18:57:20.000000 libfsntfs-20240119/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-01-19 18:57:20.000000 libfsntfs-20240119/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-01-19 18:57:20.000000 libfsntfs-20240119/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-01-19 18:57:20.000000 libfsntfs-20240119/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-01-19 18:57:20.000000 libfsntfs-20240119/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      884 2024-01-19 18:57:20.000000 libfsntfs-20240119/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-01-19 18:57:20.000000 libfsntfs-20240119/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-01-19 18:57:20.000000 libfsntfs-20240119/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-01-19 18:57:20.000000 libfsntfs-20240119/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-01-19 18:57:20.000000 libfsntfs-20240119/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-01-19 18:57:20.000000 libfsntfs-20240119/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-01-19 18:57:20.000000 libfsntfs-20240119/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-01-19 18:57:20.000000 libfsntfs-20240119/libcsplit/libcsplit_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-01-19 18:57:20.000000 libfsntfs-20240119/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-01-19 18:57:20.000000 libfsntfs-20240119/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-01-19 18:57:20.000000 libfsntfs-20240119/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32056 2024-01-19 18:57:45.000000 libfsntfs-20240119/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-01-19 18:57:20.000000 libfsntfs-20240119/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-01-19 18:57:20.000000 libfsntfs-20240119/libcsplit/libcsplit_narrow_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:09.000000 libfsntfs-20240119/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:07:03.000000 libfsntfs-20240119/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:07:03.000000 libfsntfs-20240119/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:07:03.000000 libfsntfs-20240119/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:07:03.000000 libfsntfs-20240119/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:07:03.000000 libfsntfs-20240119/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:07:03.000000 libfsntfs-20240119/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:07:03.000000 libfsntfs-20240119/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:07:03.000000 libfsntfs-20240119/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:07:03.000000 libfsntfs-20240119/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1855 2024-01-19 18:57:55.000000 libfsntfs-20240119/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:07:03.000000 libfsntfs-20240119/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:07:03.000000 libfsntfs-20240119/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:08.000000 libfsntfs-20240119/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4162 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    54753 2024-01-19 18:57:45.000000 libfsntfs-20240119/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-01-19 18:57:35.000000 libfsntfs-20240119/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42413 2024-01-19 18:57:44.000000 libfsntfs-20240119/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:08.000000 libfsntfs-20240119/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-01-19 18:57:18.000000 libfsntfs-20240119/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-01-19 18:57:18.000000 libfsntfs-20240119/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-01-19 18:57:18.000000 libfsntfs-20240119/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-01-19 18:57:18.000000 libfsntfs-20240119/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-01-19 18:57:18.000000 libfsntfs-20240119/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-01-19 18:57:18.000000 libfsntfs-20240119/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-01-19 18:57:18.000000 libfsntfs-20240119/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-01-19 18:57:18.000000 libfsntfs-20240119/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-01-19 18:57:18.000000 libfsntfs-20240119/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-01-19 18:57:18.000000 libfsntfs-20240119/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-01-19 18:57:18.000000 libfsntfs-20240119/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31110 2024-01-19 18:57:45.000000 libfsntfs-20240119/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-01-19 18:57:18.000000 libfsntfs-20240119/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-01-19 18:57:18.000000 libfsntfs-20240119/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:07.000000 libfsntfs-20240119/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-01-19 18:57:14.000000 libfsntfs-20240119/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-01-19 18:57:14.000000 libfsntfs-20240119/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-01-19 18:57:14.000000 libfsntfs-20240119/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-01-19 18:57:14.000000 libfsntfs-20240119/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-01-19 18:57:14.000000 libfsntfs-20240119/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-01-19 18:57:14.000000 libfsntfs-20240119/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-01-19 18:57:14.000000 libfsntfs-20240119/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-01-19 18:57:14.000000 libfsntfs-20240119/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-01-19 18:57:14.000000 libfsntfs-20240119/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-01-19 18:57:14.000000 libfsntfs-20240119/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-01-19 18:57:14.000000 libfsntfs-20240119/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30623 2024-01-19 18:57:44.000000 libfsntfs-20240119/libcerror/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-19 20:20:08.000000 libfsntfs-20240119/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-01-19 18:57:26.000000 libfsntfs-20240119/libfdatetime/libfdatetime_floatingtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-01-19 18:57:26.000000 libfsntfs-20240119/libfdatetime/libfdatetime_nsf_timedate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-01-19 18:57:26.000000 libfsntfs-20240119/libfdatetime/libfdatetime_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-01-19 18:57:26.000000 libfsntfs-20240119/libfdatetime/libfdatetime_floatingtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-01-19 18:57:26.000000 libfsntfs-20240119/libfdatetime/libfdatetime_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-01-19 18:57:26.000000 libfsntfs-20240119/libfdatetime/libfdatetime_hfs_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-01-19 18:57:26.000000 libfsntfs-20240119/libfdatetime/libfdatetime_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-01-19 18:57:26.000000 libfsntfs-20240119/libfdatetime/libfdatetime_hfs_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1148 2024-01-19 18:57:26.000000 libfsntfs-20240119/libfdatetime/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-01-19 18:57:26.000000 libfsntfs-20240119/libfdatetime/libfdatetime_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-01-19 18:57:26.000000 libfsntfs-20240119/libfdatetime/libfdatetime_systemtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-01-19 18:57:26.000000 libfsntfs-20240119/libfdatetime/libfdatetime_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-01-19 18:57:26.000000 libfsntfs-20240119/libfdatetime/libfdatetime_posix_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-01-19 18:57:26.000000 libfsntfs-20240119/libfdatetime/libfdatetime_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-01-19 18:57:26.000000 libfsntfs-20240119/libfdatetime/libfdatetime_fat_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-01-19 18:57:26.000000 libfsntfs-20240119/libfdatetime/libfdatetime_systemtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-01-19 18:57:26.000000 libfsntfs-20240119/libfdatetime/libfdatetime_nsf_timedate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-01-19 18:57:26.000000 libfsntfs-20240119/libfdatetime/libfdatetime_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-01-19 18:57:26.000000 libfsntfs-20240119/libfdatetime/libfdatetime_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-01-19 18:57:26.000000 libfsntfs-20240119/libfdatetime/libfdatetime_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-01-19 18:57:26.000000 libfsntfs-20240119/libfdatetime/libfdatetime_posix_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-01-19 18:57:26.000000 libfsntfs-20240119/libfdatetime/libfdatetime_date_time_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-01-19 18:57:26.000000 libfsntfs-20240119/libfdatetime/libfdatetime_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-01-19 18:57:26.000000 libfsntfs-20240119/libfdatetime/libfdatetime_date_time_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-01-19 18:57:26.000000 libfsntfs-20240119/libfdatetime/libfdatetime_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33849 2024-01-19 18:57:45.000000 libfsntfs-20240119/libfdatetime/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-01-19 18:57:26.000000 libfsntfs-20240119/libfdatetime/libfdatetime_fat_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56940 2024-01-19 18:57:42.000000 libfsntfs-20240119/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3708 2024-01-19 04:04:50.000000 libfsntfs-20240119/libfsntfs.spec.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8566 2024-01-19 04:04:50.000000 libfsntfs-20240119/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      421 2024-01-19 20:20:10.822888 libfsntfs-20240119/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:59.000000 libfsntfs-20240501/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:58.000000 libfsntfs-20240501/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_area.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_mapped_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1287 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_area.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_mapped_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_segments_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_segments_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35083 2024-05-01 08:33:49.000000 libfsntfs-20240501/libfdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-05-01 08:33:07.000000 libfsntfs-20240501/libfdata/libfdata_vector.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-05-01 07:57:38.000000 libfsntfs-20240501/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-05-01 08:33:48.000000 libfsntfs-20240501/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:38.000000 libfsntfs-20240501/NEWS
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2547 2024-05-01 08:34:02.000000 libfsntfs-20240501/libfsntfs.spec
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:59.000000 libfsntfs-20240501/pyfsntfs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1881 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8886 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2872 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_guid.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5521 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_security_descriptor_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8894 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3190 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_mft_metadata_file_entries.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1549 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1777 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_file_attribute_flags.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10060 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_object_identifier_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23169 2024-05-01 07:59:38.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_volume_information_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1361 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23602 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_standard_information_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1507 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2918 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_volume_file_entries.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9460 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_reparse_point_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1553 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_security_descriptor_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2529 2024-05-01 08:04:13.000000 libfsntfs-20240501/pyfsntfs/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40011 2024-05-01 07:59:38.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6734 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_volume_information_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    96932 2024-05-01 07:59:38.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2064 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_object_identifier_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8966 2024-05-01 07:59:38.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_file_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2036 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10741 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_volume_file_entries.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2297 2024-05-01 07:59:38.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_usn_change_journal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9495 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_data_streams.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33969 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_file_object_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1837 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_datetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12627 2024-05-01 07:59:38.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4156 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_file_object_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1553 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16625 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_datetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1809 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_reparse_point_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3400 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_standard_information_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23738 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_file_name_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3228 2024-05-01 07:59:38.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_mft_metadata_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3956 2024-05-01 07:59:38.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1180 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_guid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_data_streams.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1528 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9341 2024-05-01 07:59:38.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3169 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_file_name_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_file_entries.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_attribute_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_volume_name_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9566 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27880 2024-05-01 07:59:38.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_data_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9481 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_file_entries.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1701 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23657 2024-05-01 07:59:38.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_mft_metadata_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10659 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_attribute_types.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11552 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_mft_metadata_file_entries.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_libfsntfs.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2386 2024-05-01 07:59:38.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81352 2024-05-01 08:33:49.000000 libfsntfs-20240501/pyfsntfs/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3199 2024-05-01 07:59:38.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_data_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10577 2024-05-01 07:59:38.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_usn_change_journal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10377 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_file_attribute_flags.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5315 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_volume_name_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-01 07:57:44.000000 libfsntfs-20240501/pyfsntfs/pyfsntfs_unused.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-05-01 08:33:49.000000 libfsntfs-20240501/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:58.000000 libfsntfs-20240501/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-01 08:33:24.000000 libfsntfs-20240501/libfguid/libfguid_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-05-01 08:33:24.000000 libfsntfs-20240501/libfguid/libfguid_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-05-01 08:33:24.000000 libfsntfs-20240501/libfguid/libfguid_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-01 08:33:24.000000 libfsntfs-20240501/libfguid/libfguid_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      677 2024-05-01 08:33:24.000000 libfsntfs-20240501/libfguid/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-01 08:33:24.000000 libfsntfs-20240501/libfguid/libfguid_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-01 08:33:24.000000 libfsntfs-20240501/libfguid/libfguid_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-05-01 08:33:24.000000 libfsntfs-20240501/libfguid/libfguid_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-05-01 08:33:24.000000 libfsntfs-20240501/libfguid/libfguid_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-05-01 08:33:24.000000 libfsntfs-20240501/libfguid/libfguid_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-05-01 08:33:24.000000 libfsntfs-20240501/libfguid/libfguid_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30884 2024-05-01 08:33:49.000000 libfsntfs-20240501/libfguid/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-01 08:33:24.000000 libfsntfs-20240501/libfguid/libfguid_error.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:57.000000 libfsntfs-20240501/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9040 2024-05-01 07:57:46.000000 libfsntfs-20240501/m4/libfwnt.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11734 2024-05-01 07:57:46.000000 libfsntfs-20240501/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18489 2024-05-01 07:57:46.000000 libfsntfs-20240501/m4/libfdatetime.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:06:58.000000 libfsntfs-20240501/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9615 2024-05-01 07:57:46.000000 libfsntfs-20240501/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:06:57.000000 libfsntfs-20240501/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:06:57.000000 libfsntfs-20240501/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-05-01 07:57:46.000000 libfsntfs-20240501/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:06:57.000000 libfsntfs-20240501/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:06:58.000000 libfsntfs-20240501/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-05-01 07:57:46.000000 libfsntfs-20240501/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-05-01 07:57:46.000000 libfsntfs-20240501/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7625 2024-05-01 07:57:46.000000 libfsntfs-20240501/m4/libcsplit.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-05-01 07:57:46.000000 libfsntfs-20240501/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-05-01 07:57:46.000000 libfsntfs-20240501/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-05-01 08:33:42.000000 libfsntfs-20240501/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-05-01 08:33:42.000000 libfsntfs-20240501/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15781 2024-05-01 07:57:46.000000 libfsntfs-20240501/m4/libfdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:06:57.000000 libfsntfs-20240501/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4758 2024-05-01 07:57:46.000000 libfsntfs-20240501/m4/libfusn.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7058 2024-05-01 07:57:46.000000 libfsntfs-20240501/m4/libfuse.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-05-01 08:33:42.000000 libfsntfs-20240501/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:06:57.000000 libfsntfs-20240501/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-05-01 07:57:46.000000 libfsntfs-20240501/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-05-01 07:57:46.000000 libfsntfs-20240501/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5876 2024-05-01 07:57:46.000000 libfsntfs-20240501/m4/libfguid.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11923 2024-05-01 07:57:46.000000 libfsntfs-20240501/m4/libbfio.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8550 2024-05-01 07:57:46.000000 libfsntfs-20240501/m4/libhmac.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:06:57.000000 libfsntfs-20240501/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-05-01 08:33:42.000000 libfsntfs-20240501/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:06:57.000000 libfsntfs-20240501/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:06:58.000000 libfsntfs-20240501/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-05-01 08:33:42.000000 libfsntfs-20240501/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:06:58.000000 libfsntfs-20240501/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-05-01 07:57:46.000000 libfsntfs-20240501/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27647 2024-05-01 07:57:46.000000 libfsntfs-20240501/m4/libcrypto.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:06:57.000000 libfsntfs-20240501/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7566 2024-05-01 07:57:46.000000 libfsntfs-20240501/m4/libfcache.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-05-01 07:57:46.000000 libfsntfs-20240501/m4/pthread.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:57.000000 libfsntfs-20240501/include/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    65343 2024-05-01 08:34:02.000000 libfsntfs-20240501/include/libfsntfs.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    65343 2024-05-01 07:57:42.000000 libfsntfs-20240501/include/libfsntfs.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      440 2024-05-01 08:02:44.000000 libfsntfs-20240501/include/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:57.000000 libfsntfs-20240501/include/libfsntfs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4079 2024-05-01 07:57:42.000000 libfsntfs-20240501/include/libfsntfs/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4077 2024-05-01 08:34:02.000000 libfsntfs-20240501/include/libfsntfs/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5224 2024-05-01 07:57:42.000000 libfsntfs-20240501/include/libfsntfs/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-05-01 08:34:02.000000 libfsntfs-20240501/include/libfsntfs/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-05-01 07:57:42.000000 libfsntfs-20240501/include/libfsntfs/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-05-01 07:57:42.000000 libfsntfs-20240501/include/libfsntfs/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1436 2024-05-01 07:57:42.000000 libfsntfs-20240501/include/libfsntfs/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1499 2024-05-01 08:34:02.000000 libfsntfs-20240501/include/libfsntfs/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5422 2024-05-01 07:57:42.000000 libfsntfs-20240501/include/libfsntfs/codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29279 2024-05-01 08:33:48.000000 libfsntfs-20240501/include/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:57.000000 libfsntfs-20240501/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-05-01 07:57:42.000000 libfsntfs-20240501/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-05-01 07:57:42.000000 libfsntfs-20240501/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-05-01 07:57:42.000000 libfsntfs-20240501/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-05-01 07:57:42.000000 libfsntfs-20240501/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-01 07:57:42.000000 libfsntfs-20240501/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-05-01 07:57:42.000000 libfsntfs-20240501/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-05-01 07:57:42.000000 libfsntfs-20240501/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-05-01 08:02:44.000000 libfsntfs-20240501/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-05-01 07:57:42.000000 libfsntfs-20240501/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-05-01 08:34:02.000000 libfsntfs-20240501/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18505 2024-05-01 08:33:48.000000 libfsntfs-20240501/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19593 2024-05-01 08:34:02.000000 libfsntfs-20240501/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-05-01 07:57:42.000000 libfsntfs-20240501/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-05-01 07:57:42.000000 libfsntfs-20240501/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-05-01 07:57:42.000000 libfsntfs-20240501/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26294 2024-05-01 08:33:48.000000 libfsntfs-20240501/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:57.000000 libfsntfs-20240501/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-05-01 08:32:44.000000 libfsntfs-20240501/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-05-01 08:32:44.000000 libfsntfs-20240501/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-05-01 08:32:44.000000 libfsntfs-20240501/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-05-01 08:32:44.000000 libfsntfs-20240501/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-01 08:32:44.000000 libfsntfs-20240501/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-01 08:32:44.000000 libfsntfs-20240501/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-05-01 08:32:44.000000 libfsntfs-20240501/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-05-01 08:32:44.000000 libfsntfs-20240501/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-05-01 08:32:44.000000 libfsntfs-20240501/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-05-01 08:32:44.000000 libfsntfs-20240501/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31492 2024-05-01 08:33:48.000000 libfsntfs-20240501/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-01 08:32:44.000000 libfsntfs-20240501/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-05-01 08:32:44.000000 libfsntfs-20240501/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-05-01 08:32:44.000000 libfsntfs-20240501/libclocale/libclocale_codepage.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:58.000000 libfsntfs-20240501/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-01 08:33:03.000000 libfsntfs-20240501/libfcache/libfcache_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-05-01 08:33:03.000000 libfsntfs-20240501/libfcache/libfcache_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-05-01 08:33:03.000000 libfsntfs-20240501/libfcache/libfcache_cache_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-01 08:33:03.000000 libfsntfs-20240501/libfcache/libfcache_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      876 2024-05-01 08:33:03.000000 libfsntfs-20240501/libfcache/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-01 08:33:03.000000 libfsntfs-20240501/libfcache/libfcache_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-01 08:33:03.000000 libfsntfs-20240501/libfcache/libfcache_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-05-01 08:33:03.000000 libfsntfs-20240501/libfcache/libfcache_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-05-01 08:33:03.000000 libfsntfs-20240501/libfcache/libfcache_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-01 08:33:03.000000 libfsntfs-20240501/libfcache/libfcache_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-01 08:33:03.000000 libfsntfs-20240501/libfcache/libfcache_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-05-01 08:33:03.000000 libfsntfs-20240501/libfcache/libfcache_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-01 08:33:03.000000 libfsntfs-20240501/libfcache/libfcache_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-05-01 08:33:03.000000 libfsntfs-20240501/libfcache/libfcache_cache_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32001 2024-05-01 08:33:49.000000 libfsntfs-20240501/libfcache/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-01 08:33:03.000000 libfsntfs-20240501/libfcache/libfcache_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-05-01 08:33:03.000000 libfsntfs-20240501/libfcache/libfcache_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-05-01 08:33:03.000000 libfsntfs-20240501/libfcache/libfcache_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2198 2024-05-01 08:04:51.000000 libfsntfs-20240501/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:58.000000 libfsntfs-20240501/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_file_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_file_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_file_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_file_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_file_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_file_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_memory_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_file_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_file_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_memory_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_memory_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35344 2024-05-01 08:33:48.000000 libfsntfs-20240501/libbfio/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_memory_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-05-01 08:32:29.000000 libfsntfs-20240501/libbfio/libbfio_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:06:56.000000 libfsntfs-20240501/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-05-01 08:33:48.000000 libfsntfs-20240501/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:57.000000 libfsntfs-20240501/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-05-01 07:57:38.000000 libfsntfs-20240501/dpkg/libfsntfs-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1028 2024-05-01 07:57:46.000000 libfsntfs-20240501/dpkg/copyright
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:57.000000 libfsntfs-20240501/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-05-01 07:57:38.000000 libfsntfs-20240501/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2240 2024-05-01 07:57:38.000000 libfsntfs-20240501/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      777 2024-05-01 07:57:38.000000 libfsntfs-20240501/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-05-01 07:57:38.000000 libfsntfs-20240501/dpkg/libfsntfs-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      122 2024-05-01 07:57:38.000000 libfsntfs-20240501/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      141 2024-05-01 08:34:02.000000 libfsntfs-20240501/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-05-01 07:57:38.000000 libfsntfs-20240501/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-05-01 07:57:38.000000 libfsntfs-20240501/dpkg/libfsntfs.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-05-01 07:57:38.000000 libfsntfs-20240501/dpkg/libfsntfs-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      489 2024-05-01 08:34:02.000000 libfsntfs-20240501/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-05-01 07:57:38.000000 libfsntfs-20240501/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  2055415 2024-05-01 08:33:46.000000 libfsntfs-20240501/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-05-01 08:33:48.000000 libfsntfs-20240501/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-05-01 08:33:48.000000 libfsntfs-20240501/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-05-01 07:58:20.000000 libfsntfs-20240501/msvscpp/libfdata/libfdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_directory_entries_tree/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6169 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_directory_entries_tree/fsntfs_test_directory_entries_tree.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_file_name_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6068 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_file_name_values/fsntfs_test_file_name_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_index_node/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6050 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_index_node/fsntfs_test_index_node.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_volume_information_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6095 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_volume_information_values/fsntfs_test_volume_information_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_io_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6047 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_io_handle/fsntfs_test_io_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_compressed_block_data_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6357 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_compressed_block_data_handle/fsntfs_test_compressed_block_data_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_object_identifier_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6092 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_object_identifier_values/fsntfs_test_object_identifier_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_profiler/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6044 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_profiler/fsntfs_test_profiler.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_data_stream/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6470 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_data_stream/fsntfs_test_data_stream.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/pyfsntfs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10444 2024-05-01 07:58:20.000000 libfsntfs-20240501/msvscpp/pyfsntfs/pyfsntfs.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_security_descriptor_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6352 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_security_descriptor_values/fsntfs_test_security_descriptor_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_file_system/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6470 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_file_system/fsntfs_test_file_system.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_tools_info_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6628 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_tools_info_handle/fsntfs_test_tools_info_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-05-01 07:58:20.000000 libfsntfs-20240501/msvscpp/libfguid/libfguid.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5786 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_error/fsntfs_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_mft_attribute_list_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6176 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_mft_attribute_list_entry/fsntfs_test_mft_attribute_list_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_mft_entry_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6068 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_mft_entry_header/fsntfs_test_mft_entry_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_buffer_data_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6074 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_buffer_data_handle/fsntfs_test_buffer_data_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_file_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6467 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_file_entry/fsntfs_test_file_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_reparse_point_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6080 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_reparse_point_values/fsntfs_test_reparse_point_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_security_descriptor_index/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6178 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_security_descriptor_index/fsntfs_test_security_descriptor_index.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-05-01 07:58:20.000000 libfsntfs-20240501/msvscpp/libclocale/libclocale.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_index/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6035 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_index/fsntfs_test_index.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfsinfo/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7959 2024-05-01 07:58:20.000000 libfsntfs-20240501/msvscpp/fsntfsinfo/fsntfsinfo.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_index_entry_vector/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6496 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_index_entry_vector/fsntfs_test_index_entry_vector.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-05-01 07:58:20.000000 libfsntfs-20240501/msvscpp/libfcache/libfcache.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5577 2024-05-01 08:04:02.000000 libfsntfs-20240501/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-05-01 07:58:20.000000 libfsntfs-20240501/msvscpp/libbfio/libbfio.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_fixup_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5892 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_fixup_values/fsntfs_test_fixup_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_index_root_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6071 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_index_root_header/fsntfs_test_index_root_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_index_value/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6053 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_index_value/fsntfs_test_index_value.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_compression/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5889 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_compression/fsntfs_test_compression.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_attribute/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6211 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_attribute/fsntfs_test_attribute.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_index_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6306 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_index_entry/fsntfs_test_index_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_mft_metadata_file/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6824 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_mft_metadata_file/fsntfs_test_mft_metadata_file.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_sds_index_value/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6065 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_sds_index_value/fsntfs_test_sds_index_value.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_security_descriptor_index_value/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6113 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_security_descriptor_index_value/fsntfs_test_security_descriptor_index_value.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_mft_attribute_list/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6158 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_mft_attribute_list/fsntfs_test_mft_attribute_list.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_standard_information_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6101 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_standard_information_values/fsntfs_test_standard_information_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_mft_attribute/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6143 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_mft_attribute/fsntfs_test_mft_attribute.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-05-01 07:58:20.000000 libfsntfs-20240501/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_usn_change_journal/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6238 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_usn_change_journal/fsntfs_test_usn_change_journal.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_compressed_block_vector/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6511 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_compressed_block_vector/fsntfs_test_compressed_block_vector.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_volume_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6312 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_volume_header/fsntfs_test_volume_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_tools_mount_path_string/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6014 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_tools_mount_path_string/fsntfs_test_tools_mount_path_string.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-05-01 07:58:20.000000 libfsntfs-20240501/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_volume_name_attribute/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6083 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_volume_name_attribute/fsntfs_test_volume_name_attribute.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_txf_data_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6065 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_txf_data_values/fsntfs_test_txf_data_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_compression_unit_descriptor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6101 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_compression_unit_descriptor/fsntfs_test_compression_unit_descriptor.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_directory_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6149 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_directory_entry/fsntfs_test_directory_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_tools_digest_hash/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5984 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_tools_digest_hash/fsntfs_test_tools_digest_hash.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_data_run/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6128 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_data_run/fsntfs_test_data_run.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_compressed_block/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6068 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_compressed_block/fsntfs_test_compressed_block.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_volume_information_attribute/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6104 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_volume_information_attribute/fsntfs_test_volume_information_attribute.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_mft/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6029 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_mft/fsntfs_test_mft.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_reparse_point_attribute/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6089 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_reparse_point_attribute/fsntfs_test_reparse_point_attribute.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-05-01 07:58:20.000000 libfsntfs-20240501/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_file_name_attribute/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6077 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_file_name_attribute/fsntfs_test_file_name_attribute.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_index_entry_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6074 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_index_entry_header/fsntfs_test_index_entry_header.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    87512 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/libfsntfs.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-05-01 07:58:20.000000 libfsntfs-20240501/msvscpp/libcpath/libcpath.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5874 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_notify/fsntfs_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfsmount/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8022 2024-05-01 07:58:20.000000 libfsntfs-20240501/msvscpp/fsntfsmount/fsntfsmount.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_cluster_block/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6312 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_cluster_block/fsntfs_test_cluster_block.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_tools_path_string/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6068 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_tools_path_string/fsntfs_test_tools_path_string.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_cluster_block_stream/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6164 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_cluster_block_stream/fsntfs_test_cluster_block_stream.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/libfusn/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5308 2024-05-01 07:58:20.000000 libfsntfs-20240501/msvscpp/libfusn/libfusn.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_cluster_block_vector/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6502 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_cluster_block_vector/fsntfs_test_cluster_block_vector.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_tools_output/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5983 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_tools_output/fsntfs_test_tools_output.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_volume/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6873 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_volume/fsntfs_test_volume.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/libfwnt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6895 2024-05-01 07:58:20.000000 libfsntfs-20240501/msvscpp/libfwnt/libfwnt.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_tools_bodyfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6053 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_tools_bodyfile/fsntfs_test_tools_bodyfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/libfsntfs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20944 2024-05-01 07:58:20.000000 libfsntfs-20240501/msvscpp/libfsntfs/libfsntfs.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_name/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6032 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_name/fsntfs_test_name.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_extent/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6038 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_extent/fsntfs_test_extent.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_index_node_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6071 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_index_node_header/fsntfs_test_index_node_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/libhmac/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6182 2024-05-01 07:58:20.000000 libfsntfs-20240501/msvscpp/libhmac/libhmac.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_attribute_list_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6080 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_attribute_list_entry/fsntfs_test_attribute_list_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-05-01 07:58:20.000000 libfsntfs-20240501/msvscpp/libcsplit/libcsplit.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_bitmap_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6059 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_bitmap_values/fsntfs_test_bitmap_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_logged_utility_stream_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6104 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_logged_utility_stream_values/fsntfs_test_logged_utility_stream_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-05-01 07:58:20.000000 libfsntfs-20240501/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28861 2024-05-01 08:33:49.000000 libfsntfs-20240501/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_cluster_block_data/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6411 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_cluster_block_data/fsntfs_test_cluster_block_data.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_tools_signal/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5983 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_tools_signal/fsntfs_test_tools_signal.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_volume_name_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6074 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_volume_name_values/fsntfs_test_volume_name_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6712 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_support/fsntfs_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-05-01 07:58:20.000000 libfsntfs-20240501/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_path_hint/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6047 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_path_hint/fsntfs_test_path_hint.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_compressed_data_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6170 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_compressed_data_handle/fsntfs_test_compressed_data_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_mft_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6300 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_mft_entry/fsntfs_test_mft_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-05-01 07:58:20.000000 libfsntfs-20240501/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-05-01 07:58:20.000000 libfsntfs-20240501/msvscpp/libfdatetime/libfdatetime.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:45:00.000000 libfsntfs-20240501/msvscpp/fsntfs_test_compression_unit_data_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6104 2024-05-01 07:58:54.000000 libfsntfs-20240501/msvscpp/fsntfs_test_compression_unit_data_handle/fsntfs_test_compression_unit_data_handle.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       93 2024-05-01 07:57:41.000000 libfsntfs-20240501/AUTHORS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:58.000000 libfsntfs-20240501/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-01 08:32:41.000000 libfsntfs-20240501/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-05-01 08:32:41.000000 libfsntfs-20240501/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-01 08:32:41.000000 libfsntfs-20240501/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-01 08:32:41.000000 libfsntfs-20240501/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-05-01 08:32:41.000000 libfsntfs-20240501/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-05-01 08:32:41.000000 libfsntfs-20240501/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      938 2024-05-01 08:32:41.000000 libfsntfs-20240501/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-01 08:32:41.000000 libfsntfs-20240501/libcfile/libcfile_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-01 08:32:41.000000 libfsntfs-20240501/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-05-01 08:32:41.000000 libfsntfs-20240501/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-01 08:32:41.000000 libfsntfs-20240501/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-01 08:32:41.000000 libfsntfs-20240501/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-01 08:32:41.000000 libfsntfs-20240501/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-01 08:32:41.000000 libfsntfs-20240501/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-05-01 08:32:41.000000 libfsntfs-20240501/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-01 08:32:41.000000 libfsntfs-20240501/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-05-01 08:32:41.000000 libfsntfs-20240501/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32325 2024-05-01 08:33:48.000000 libfsntfs-20240501/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-01 08:32:41.000000 libfsntfs-20240501/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-01 08:32:41.000000 libfsntfs-20240501/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-05-01 08:32:41.000000 libfsntfs-20240501/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-05-01 08:32:41.000000 libfsntfs-20240501/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      684 2024-05-01 07:57:38.000000 libfsntfs-20240501/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-05-01 08:33:48.000000 libfsntfs-20240501/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:57.000000 libfsntfs-20240501/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34238 2024-05-01 08:33:48.000000 libfsntfs-20240501/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-01 08:32:34.000000 libfsntfs-20240501/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-05-01 07:57:38.000000 libfsntfs-20240501/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      490 2024-05-01 07:57:38.000000 libfsntfs-20240501/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-05-01 08:33:48.000000 libfsntfs-20240501/config.sub
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      757 2024-05-01 07:57:38.000000 libfsntfs-20240501/libfsntfs.pc.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-05-01 07:57:38.000000 libfsntfs-20240501/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1816 2024-05-01 07:59:38.000000 libfsntfs-20240501/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:06:56.000000 libfsntfs-20240501/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:57.000000 libfsntfs-20240501/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-05-01 08:32:59.000000 libfsntfs-20240501/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-05-01 08:32:59.000000 libfsntfs-20240501/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-05-01 08:32:59.000000 libfsntfs-20240501/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-05-01 08:32:59.000000 libfsntfs-20240501/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-05-01 08:32:59.000000 libfsntfs-20240501/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-05-01 08:32:59.000000 libfsntfs-20240501/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-01 08:32:59.000000 libfsntfs-20240501/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-05-01 08:32:59.000000 libfsntfs-20240501/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-05-01 08:32:59.000000 libfsntfs-20240501/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-05-01 08:32:59.000000 libfsntfs-20240501/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-05-01 08:32:59.000000 libfsntfs-20240501/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-05-01 08:32:59.000000 libfsntfs-20240501/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-05-01 08:32:59.000000 libfsntfs-20240501/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-05-01 08:32:59.000000 libfsntfs-20240501/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-05-01 08:32:59.000000 libfsntfs-20240501/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-05-01 08:32:59.000000 libfsntfs-20240501/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-05-01 08:32:59.000000 libfsntfs-20240501/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-05-01 08:32:59.000000 libfsntfs-20240501/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-05-01 08:32:59.000000 libfsntfs-20240501/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-05-01 08:32:59.000000 libfsntfs-20240501/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-01 08:32:59.000000 libfsntfs-20240501/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-05-01 08:32:59.000000 libfsntfs-20240501/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-05-01 08:32:59.000000 libfsntfs-20240501/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-05-01 08:32:59.000000 libfsntfs-20240501/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-05-01 08:32:59.000000 libfsntfs-20240501/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-05-01 08:32:59.000000 libfsntfs-20240501/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-05-01 08:32:59.000000 libfsntfs-20240501/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34677 2024-05-01 08:33:49.000000 libfsntfs-20240501/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-05-01 08:32:59.000000 libfsntfs-20240501/libcthreads/libcthreads_queue.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:59.000000 libfsntfs-20240501/fsntfstools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/fsntfstools_signal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1723 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/mount_path_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37237 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/mount_dokan.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2561 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/mount_file_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5776 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/fsntfstools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28494 2024-05-01 07:59:38.000000 libfsntfs-20240501/fsntfstools/mount_fuse.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9036 2024-05-01 07:59:38.000000 libfsntfs-20240501/fsntfstools/info_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5420 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/mount_dokan.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15540 2024-05-01 07:59:38.000000 libfsntfs-20240501/fsntfstools/fsntfsmount.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4539 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/fsntfstools_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1729 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/path_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3298 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/digest_hash.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13694 2024-05-01 07:59:38.000000 libfsntfs-20240501/fsntfstools/mount_file_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1446 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/fsntfstools_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1489 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/fsntfstools_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1481 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/fsntfstools_output.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1751 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/fsntfstools_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/fsntfstools_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1507 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/fsntfstools_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2821 2024-05-01 08:03:55.000000 libfsntfs-20240501/fsntfstools/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      989 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/fsntfstools_libfsntfs.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1216 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/fsntfstools_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1283 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/bodyfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24694 2024-05-01 07:59:38.000000 libfsntfs-20240501/fsntfstools/mount_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   214389 2024-05-01 07:59:38.000000 libfsntfs-20240501/fsntfstools/info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3829 2024-05-01 07:59:38.000000 libfsntfs-20240501/fsntfstools/mount_file_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1486 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/fsntfstools_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11773 2024-05-01 07:59:38.000000 libfsntfs-20240501/fsntfstools/fsntfsinfo.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/fsntfstools_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/fsntfstools_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/fsntfstools_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1751 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/fsntfstools_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/fsntfstools_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2568 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/mount_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21648 2024-05-01 07:59:38.000000 libfsntfs-20240501/fsntfstools/mount_path_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1774 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/fsntfstools_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1784 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/fsntfstools_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/fsntfstools_libfusn.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16556 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/mount_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1477 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/fsntfstools_libhmac.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37346 2024-05-01 08:33:48.000000 libfsntfs-20240501/fsntfstools/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8836 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/bodyfile.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1245 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/digest_hash.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4584 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/fsntfstools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2856 2024-05-01 07:59:38.000000 libfsntfs-20240501/fsntfstools/mount_fuse.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20256 2024-05-01 07:57:44.000000 libfsntfs-20240501/fsntfstools/path_string.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-05-01 08:33:49.000000 libfsntfs-20240501/test-driver
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:58.000000 libfsntfs-20240501/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-05-01 08:32:51.000000 libfsntfs-20240501/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-01 08:32:51.000000 libfsntfs-20240501/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-05-01 08:32:51.000000 libfsntfs-20240501/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2024-05-01 08:32:51.000000 libfsntfs-20240501/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-01 08:32:51.000000 libfsntfs-20240501/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-01 08:32:51.000000 libfsntfs-20240501/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-01 08:32:51.000000 libfsntfs-20240501/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-05-01 08:32:51.000000 libfsntfs-20240501/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-05-01 08:32:51.000000 libfsntfs-20240501/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-01 08:32:51.000000 libfsntfs-20240501/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-01 08:32:51.000000 libfsntfs-20240501/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-01 08:32:51.000000 libfsntfs-20240501/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31523 2024-05-01 08:33:49.000000 libfsntfs-20240501/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-01 08:32:51.000000 libfsntfs-20240501/libcpath/libcpath_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-01 08:32:51.000000 libfsntfs-20240501/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-05-01 08:32:51.000000 libfsntfs-20240501/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-05-01 08:32:51.000000 libfsntfs-20240501/libcpath/libcpath_path.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12127 2023-12-03 09:06:56.000000 libfsntfs-20240501/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:59.000000 libfsntfs-20240501/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30945 2024-05-01 07:57:46.000000 libfsntfs-20240501/manuals/libfsntfs.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      133 2024-05-01 08:03:45.000000 libfsntfs-20240501/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2097 2024-05-01 07:57:46.000000 libfsntfs-20240501/manuals/fsntfsinfo.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28261 2024-05-01 08:33:49.000000 libfsntfs-20240501/manuals/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:59.000000 libfsntfs-20240501/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42075 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_compressed_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35027 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_volume_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4215 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_tools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35342 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_security_descriptor_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1373 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3179 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26242 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_directory_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27562 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_file_name_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30750 2024-05-01 07:59:38.000000 libfsntfs-20240501/tests/pyfsntfs_test_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19485 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_cluster_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8293 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2469 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_tools_output.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4099 2024-05-01 08:00:53.000000 libfsntfs-20240501/tests/test_tools.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23213 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_attribute_list_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21070 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_mft_entry_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    61128 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_cluster_block_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15073 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_volume_name_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36448 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_index_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8609 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10754 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_compression_unit_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    92407 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_compressed_block_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6929 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_compressed_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11627 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_fixup_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35794 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_mft_attribute_list_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10504 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_security_descriptor_index.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31443 2024-05-01 08:03:36.000000 libfsntfs-20240501/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15448 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15608 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_logged_utility_stream_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1714 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_rwlock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28529 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_standard_information_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4171 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_tools_digest_hash.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1713 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14811 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_volume_information_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9464 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_sds_index_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67794 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_index_entry_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   110662 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_file_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2007 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_functions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    46804 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9711 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_index.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15740 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_functions.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8643 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_extent.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39562 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_reparse_point_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19673 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_tools_mount_path_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6160 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_path_hint.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    51596 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_mft_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_rwlock.c
+-rwxr--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-01 07:57:45.000000 libfsntfs-20240501/tests/test_manpage.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10607 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_mft.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9304 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_index_node_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4539 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_getopt.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4438 2024-05-01 08:00:39.000000 libfsntfs-20240501/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15536 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_index_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7485 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_tools_bodyfile.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9322 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_index_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17926 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_buffer_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      989 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_libfsntfs.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1712 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4747 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35037 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_directory_entries_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9719 2024-05-01 07:59:38.000000 libfsntfs-20240501/tests/pyfsntfs_test_attribute.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-05-01 07:57:45.000000 libfsntfs-20240501/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15806 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_index_root_header.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4302 2024-05-01 08:01:31.000000 libfsntfs-20240501/tests/test_fsntfsinfo_bodyfile.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11117 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_volume_information_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30542 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_cluster_block_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7132 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_profiler.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    92860 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_cluster_block_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   127913 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_compression.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    59087 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_mft_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8845 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_usn_change_journal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7326 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_compression_unit_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4370 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43184 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_file_name_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13439 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_tools_path_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13963 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_txf_data_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16019 2024-05-01 07:59:38.000000 libfsntfs-20240501/tests/pyfsntfs_test_volume.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100559 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_compressed_block_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1745 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    63509 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15523 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_security_descriptor_index_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31345 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_volume_name_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   259855 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_file_entry.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3372 2024-05-01 07:57:45.000000 libfsntfs-20240501/tests/test_fsntfsinfo.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   148460 2024-05-01 08:33:49.000000 libfsntfs-20240501/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1557 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   132840 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_data_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1560 2024-05-01 07:57:45.000000 libfsntfs-20240501/tests/pyfsntfs_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33492 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_mft_metadata_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12477 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_mft_attribute_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24256 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_name.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23688 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_reparse_point_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14322 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_object_identifier_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5750 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_tools_info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12691 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_data_run.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14470 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_bitmap_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14589 2024-05-01 07:58:54.000000 libfsntfs-20240501/tests/fsntfs_test_index_entry_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1468 2024-05-01 07:57:46.000000 libfsntfs-20240501/tests/fsntfs_test_libclocale.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     5117 2024-05-01 08:00:24.000000 libfsntfs-20240501/tests/test_library.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:59.000000 libfsntfs-20240501/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2255 2024-05-01 07:57:43.000000 libfsntfs-20240501/ossfuzz/volume_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2023 2024-05-01 08:03:12.000000 libfsntfs-20240501/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2430 2024-05-01 07:57:43.000000 libfsntfs-20240501/ossfuzz/mft_metadata_file_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      977 2024-05-01 07:57:43.000000 libfsntfs-20240501/ossfuzz/ossfuzz_libfsntfs.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-05-01 07:57:43.000000 libfsntfs-20240501/ossfuzz/ossfuzz_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3119 2024-05-01 07:57:43.000000 libfsntfs-20240501/ossfuzz/file_entry_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37824 2024-05-01 08:33:49.000000 libfsntfs-20240501/ossfuzz/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:59.000000 libfsntfs-20240501/libfusn/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-05-01 08:33:27.000000 libfsntfs-20240501/libfusn/libfusn_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1877 2024-05-01 08:33:27.000000 libfsntfs-20240501/libfusn/libfusn_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26484 2024-05-01 08:33:27.000000 libfsntfs-20240501/libfusn/libfusn_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-05-01 08:33:27.000000 libfsntfs-20240501/libfusn/libfusn_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1375 2024-05-01 08:33:27.000000 libfsntfs-20240501/libfusn/libfusn_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-01 08:33:27.000000 libfsntfs-20240501/libfusn/libfusn_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      848 2024-05-01 08:33:27.000000 libfsntfs-20240501/libfusn/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-01 08:33:27.000000 libfsntfs-20240501/libfusn/libfusn_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-01 08:33:27.000000 libfsntfs-20240501/libfusn/libfusn_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-05-01 08:33:27.000000 libfsntfs-20240501/libfusn/libfusn_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2327 2024-05-01 08:33:27.000000 libfsntfs-20240501/libfusn/fusn_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-05-01 08:33:27.000000 libfsntfs-20240501/libfusn/libfusn_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12280 2024-05-01 08:33:27.000000 libfsntfs-20240501/libfusn/libfusn_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31498 2024-05-01 08:33:49.000000 libfsntfs-20240501/libfusn/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-01 08:33:27.000000 libfsntfs-20240501/libfusn/libfusn_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-05-01 08:33:27.000000 libfsntfs-20240501/libfusn/libfusn_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4234 2024-05-01 08:33:27.000000 libfsntfs-20240501/libfusn/libfusn_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1723 2024-05-01 08:33:27.000000 libfsntfs-20240501/libfusn/libfusn_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-01 08:33:27.000000 libfsntfs-20240501/libfusn/libfusn_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-05-01 08:33:41.000000 libfsntfs-20240501/ltmain.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:58.000000 libfsntfs-20240501/libfwnt/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_locale_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26551 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_lzxpress.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30230 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_security_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7049 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_bit_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_lznt1.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1344 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5264 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_security_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2072 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_huffman_tree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2795 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_access_control_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27064 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_security_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13639 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_access_control_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3470 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13113 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_huffman_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8377 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15166 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_lznt1.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18859 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_locale_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1464 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2797 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_lzx.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19962 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_access_control_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2326 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_lzxpress.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3336 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_security_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36036 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_lzx.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35602 2024-05-01 08:33:49.000000 libfsntfs-20240501/libfwnt/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2039 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_bit_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1908 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3209 2024-05-01 08:33:30.000000 libfsntfs-20240501/libfwnt/libfwnt_access_control_entry.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:59.000000 libfsntfs-20240501/libfsntfs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8711 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_index_entry_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1401 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2807 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_mft.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2829 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_compressed_block_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5756 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_sds_index_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5329 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_directory_entries_tree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23422 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_security_descriptor_index.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9488 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_txf_data_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19693 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_security_descriptor_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32475 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_reparse_point_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1587 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_compressed_block.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4026 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_compressed_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1797 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_index_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1332 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_compression.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8183 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_profiler.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19566 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_standard_information_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2427 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/fsntfs_mft_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12901 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_index_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5499 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_volume_information_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25555 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_cluster_block_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/fsntfs_volume_information.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11491 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_object_identifier_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5429 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9737 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_data_run.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3290 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_attribute_list_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3833 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_index.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2815 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_standard_information_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1706 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2414 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_security_descriptor_index_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20087 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_reparse_point_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    54272 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_mft_metadata_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17017 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_mft_entry_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1880 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/fsntfs_txf_data.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20304 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_standard_information_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12727 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_cluster_block_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7382 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_attribute_list_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1978 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_volume_name_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_cluster_block_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25012 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_volume_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1645 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_attribute_list_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23871 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_compressed_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_index_node_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1469 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/fsntfs_logged_utility_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21101 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_mft_attribute_list_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13566 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_object_identifier_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7849 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_logged_utility_stream_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17579 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_bitmap_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2766 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94395 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16323 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1892 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_cluster_block.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2062 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_object_identifier_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8562 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_index_root_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2373 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6767 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_index_node_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3924 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/fsntfs_mft_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2448 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_index_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6380 2024-05-01 08:03:02.000000 libfsntfs-20240501/libfsntfs/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7028 2024-05-01 08:34:02.000000 libfsntfs-20240501/libfsntfs/libfsntfs_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4755 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_file_name_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/fsntfs_object_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2289 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_txf_data_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19319 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1932 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6301 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_cluster_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1793 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/fsntfs_mft_attribute_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2255 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_volume_information_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39152 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48386 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_file_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9103 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_compression_unit_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4582 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_usn_change_journal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16683 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_mft.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3227 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_security_descriptor_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8168 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_volume_name_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2503 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/fsntfs_standard_information.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3756 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_mft_attribute_list_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29763 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_file_name_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2413 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_index_root_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2574 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6361 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_mft_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4131 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_extent.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    60465 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_mft_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1621 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_volume_information_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18720 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_usn_change_journal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12076 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_compressed_block_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3360 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_directory_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2639 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_compression_unit_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3248 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/fsntfs_volume_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3159 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_security_descriptor_index.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4217 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_standard_information_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15319 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_file_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4008 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_file_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1967 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_name.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1678 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_sds_index_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5165 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_fixup_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1105 2024-05-01 08:34:02.000000 libfsntfs-20240501/libfsntfs/libfsntfs.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13362 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_index_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1286 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_fixup_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1107 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4610 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_cluster_block_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    77724 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_mft_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1909 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/fsntfs_secure.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13040 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_index_entry_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1877 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_cluster_block_vector.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1608 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7978 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_security_descriptor_index_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2343 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_buffer_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2786 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_volume_name_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1677 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_extent.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3950 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_mft_attribute_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12385 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_compressed_block_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29282 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_index.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7850 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_buffer_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1706 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3190 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_reparse_point_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2349 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_path_hint.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2486 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/fsntfs_reparse_point.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2184 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_logged_utility_stream_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4404 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_data_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8832 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_volume_information_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20199 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_file_name_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3149 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/fsntfs_index.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12001 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_index_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2144 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_index_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2005 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2392 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_object_identifier_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3381 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_compressed_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5970 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_mft_metadata_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1729 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2228 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_bitmap_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   171864 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15524 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_directory_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1846 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_cluster_block_data.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2420 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_compression_unit_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22736 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_mft_attribute_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5402 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_security_descriptor_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7030 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1984 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_compressed_block_vector.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23692 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_name.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3207 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_file_name_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    58691 2024-05-01 08:33:49.000000 libfsntfs-20240501/libfsntfs/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8311 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28629 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_data_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3874 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_mft_entry_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15709 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_volume_name_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4428 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_reparse_point_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    63741 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_directory_entries_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4088 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_compression.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9290 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_mft_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2038 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_data_run.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8597 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_path_hint.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2253 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_index_entry_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1892 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_index_entry_vector.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1646 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_security_descriptor_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2102 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_profiler.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17815 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_attribute_list_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2318 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/fsntfs_file_name.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20903 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_compression_unit_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3475 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_volume_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-01 07:57:43.000000 libfsntfs-20240501/libfsntfs/libfsntfs_unused.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:59.000000 libfsntfs-20240501/libhmac/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47989 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_sha1_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_sha224.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50026 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_sha512_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14448 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_md5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2079 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_md5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1942 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9362 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14650 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_sha512.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45648 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_sha256_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_sha224.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1623 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2060 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_sha1.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3443 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_sha256_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1117 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45605 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_sha224_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_md5_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_sha256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3368 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_sha1_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34388 2024-05-01 08:33:49.000000 libfsntfs-20240501/libhmac/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_sha256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3461 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_sha224_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3444 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_sha512_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_sha512.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14514 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_sha1.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40596 2024-05-01 08:33:32.000000 libfsntfs-20240501/libhmac/libhmac_md5_context.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:58.000000 libfsntfs-20240501/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-05-01 08:32:54.000000 libfsntfs-20240501/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-05-01 08:32:54.000000 libfsntfs-20240501/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-05-01 08:32:54.000000 libfsntfs-20240501/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-05-01 08:32:54.000000 libfsntfs-20240501/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-01 08:32:54.000000 libfsntfs-20240501/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-05-01 08:32:54.000000 libfsntfs-20240501/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-01 08:32:54.000000 libfsntfs-20240501/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-05-01 08:32:54.000000 libfsntfs-20240501/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-01 08:32:54.000000 libfsntfs-20240501/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-05-01 08:32:54.000000 libfsntfs-20240501/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-01 08:32:54.000000 libfsntfs-20240501/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-05-01 08:32:54.000000 libfsntfs-20240501/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-01 08:32:54.000000 libfsntfs-20240501/libcsplit/libcsplit_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-01 08:32:54.000000 libfsntfs-20240501/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-01 08:32:54.000000 libfsntfs-20240501/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-05-01 08:32:54.000000 libfsntfs-20240501/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32420 2024-05-01 08:33:49.000000 libfsntfs-20240501/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-05-01 08:32:54.000000 libfsntfs-20240501/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-05-01 08:32:54.000000 libfsntfs-20240501/libcsplit/libcsplit_narrow_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:59.000000 libfsntfs-20240501/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:07:03.000000 libfsntfs-20240501/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:07:03.000000 libfsntfs-20240501/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:07:03.000000 libfsntfs-20240501/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:07:03.000000 libfsntfs-20240501/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:07:03.000000 libfsntfs-20240501/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:07:03.000000 libfsntfs-20240501/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:07:03.000000 libfsntfs-20240501/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:07:03.000000 libfsntfs-20240501/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:07:03.000000 libfsntfs-20240501/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1855 2024-05-01 08:34:02.000000 libfsntfs-20240501/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:07:03.000000 libfsntfs-20240501/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:07:03.000000 libfsntfs-20240501/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:58.000000 libfsntfs-20240501/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    58004 2024-05-01 08:33:49.000000 libfsntfs-20240501/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-05-01 08:33:36.000000 libfsntfs-20240501/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42351 2024-05-01 08:33:48.000000 libfsntfs-20240501/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:58.000000 libfsntfs-20240501/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-01 08:32:48.000000 libfsntfs-20240501/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-01 08:32:48.000000 libfsntfs-20240501/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-05-01 08:32:48.000000 libfsntfs-20240501/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-05-01 08:32:48.000000 libfsntfs-20240501/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-05-01 08:32:48.000000 libfsntfs-20240501/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-01 08:32:48.000000 libfsntfs-20240501/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-05-01 08:32:48.000000 libfsntfs-20240501/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-05-01 08:32:48.000000 libfsntfs-20240501/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-05-01 08:32:48.000000 libfsntfs-20240501/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-05-01 08:32:48.000000 libfsntfs-20240501/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-05-01 08:32:48.000000 libfsntfs-20240501/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31361 2024-05-01 08:33:48.000000 libfsntfs-20240501/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-01 08:32:48.000000 libfsntfs-20240501/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-05-01 08:32:48.000000 libfsntfs-20240501/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:57.000000 libfsntfs-20240501/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-05-01 08:32:39.000000 libfsntfs-20240501/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-05-01 08:32:39.000000 libfsntfs-20240501/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-01 08:32:39.000000 libfsntfs-20240501/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-05-01 08:32:39.000000 libfsntfs-20240501/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-05-01 08:32:39.000000 libfsntfs-20240501/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-01 08:32:39.000000 libfsntfs-20240501/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-05-01 08:32:39.000000 libfsntfs-20240501/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-05-01 08:32:39.000000 libfsntfs-20240501/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-05-01 08:32:39.000000 libfsntfs-20240501/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-01 08:32:39.000000 libfsntfs-20240501/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-01 08:32:39.000000 libfsntfs-20240501/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30828 2024-05-01 08:33:48.000000 libfsntfs-20240501/libcerror/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 09:44:58.000000 libfsntfs-20240501/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-05-01 08:33:15.000000 libfsntfs-20240501/libfdatetime/libfdatetime_floatingtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-05-01 08:33:15.000000 libfsntfs-20240501/libfdatetime/libfdatetime_nsf_timedate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-05-01 08:33:15.000000 libfsntfs-20240501/libfdatetime/libfdatetime_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-05-01 08:33:15.000000 libfsntfs-20240501/libfdatetime/libfdatetime_floatingtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-05-01 08:33:15.000000 libfsntfs-20240501/libfdatetime/libfdatetime_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-05-01 08:33:15.000000 libfsntfs-20240501/libfdatetime/libfdatetime_hfs_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-05-01 08:33:15.000000 libfsntfs-20240501/libfdatetime/libfdatetime_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-05-01 08:33:15.000000 libfsntfs-20240501/libfdatetime/libfdatetime_hfs_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1144 2024-05-01 08:33:15.000000 libfsntfs-20240501/libfdatetime/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-05-01 08:33:15.000000 libfsntfs-20240501/libfdatetime/libfdatetime_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-05-01 08:33:15.000000 libfsntfs-20240501/libfdatetime/libfdatetime_systemtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-01 08:33:15.000000 libfsntfs-20240501/libfdatetime/libfdatetime_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-05-01 08:33:15.000000 libfsntfs-20240501/libfdatetime/libfdatetime_posix_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-05-01 08:33:15.000000 libfsntfs-20240501/libfdatetime/libfdatetime_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-05-01 08:33:15.000000 libfsntfs-20240501/libfdatetime/libfdatetime_fat_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-05-01 08:33:15.000000 libfsntfs-20240501/libfdatetime/libfdatetime_systemtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-05-01 08:33:15.000000 libfsntfs-20240501/libfdatetime/libfdatetime_nsf_timedate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-05-01 08:33:15.000000 libfsntfs-20240501/libfdatetime/libfdatetime_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-05-01 08:33:15.000000 libfsntfs-20240501/libfdatetime/libfdatetime_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-05-01 08:33:15.000000 libfsntfs-20240501/libfdatetime/libfdatetime_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-05-01 08:33:15.000000 libfsntfs-20240501/libfdatetime/libfdatetime_posix_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-05-01 08:33:15.000000 libfsntfs-20240501/libfdatetime/libfdatetime_date_time_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-05-01 08:33:15.000000 libfsntfs-20240501/libfdatetime/libfdatetime_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-05-01 08:33:15.000000 libfsntfs-20240501/libfdatetime/libfdatetime_date_time_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-05-01 08:33:15.000000 libfsntfs-20240501/libfdatetime/libfdatetime_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34412 2024-05-01 08:33:49.000000 libfsntfs-20240501/libfdatetime/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-05-01 08:33:15.000000 libfsntfs-20240501/libfdatetime/libfdatetime_fat_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56940 2024-05-01 08:33:45.000000 libfsntfs-20240501/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3708 2024-05-01 07:57:38.000000 libfsntfs-20240501/libfsntfs.spec.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8566 2024-05-01 07:57:38.000000 libfsntfs-20240501/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      421 2024-05-01 09:45:01.109341 libfsntfs-20240501/PKG-INFO
```

### Comparing `libfsntfs-20240119/libfdata/libfdata_error.h` & `libfsntfs-20240501/libfdata/libfdata_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_area.c` & `libfsntfs-20240501/libfdata/libfdata_area.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_stream.h` & `libfsntfs-20240501/libfdata/libfdata_stream.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_cache.h` & `libfsntfs-20240501/libfdata/libfdata_cache.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_range_list.c` & `libfsntfs-20240501/libfdata/libfdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_mapped_range.c` & `libfsntfs-20240501/libfdata/libfdata_mapped_range.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_libcerror.h` & `libfsntfs-20240501/libfdata/libfdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_definitions.h` & `libfsntfs-20240501/libfdata/libfdata_definitions.h`

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

### Comparing `libfsntfs-20240119/libfdata/libfdata_list.c` & `libfsntfs-20240501/libfdata/libfdata_list.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_libcdata.h` & `libfsntfs-20240501/libfdata/libfdata_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_list.h` & `libfsntfs-20240501/libfdata/libfdata_list.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_list_element.h` & `libfsntfs-20240501/libfdata/libfdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/Makefile.am` & `libfsntfs-20240501/libfdata/Makefile.am`

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

### Comparing `libfsntfs-20240119/libfdata/libfdata_libcnotify.h` & `libfsntfs-20240501/libfdata/libfdata_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_extern.h` & `libfsntfs-20240501/libfdata/libfdata_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_notify.c` & `libfsntfs-20240501/libfdata/libfdata_notify.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_cache.c` & `libfsntfs-20240501/libfdata/libfdata_cache.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_stream.c` & `libfsntfs-20240501/libfdata/libfdata_stream.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_unused.h` & `libfsntfs-20240501/libfdata/libfdata_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_range.h` & `libfsntfs-20240501/libfdata/libfdata_range.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_area.h` & `libfsntfs-20240501/libfdata/libfdata_area.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_error.c` & `libfsntfs-20240501/libfdata/libfdata_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_support.h` & `libfsntfs-20240501/libfdata/libfdata_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_range.c` & `libfsntfs-20240501/libfdata/libfdata_range.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_mapped_range.h` & `libfsntfs-20240501/libfdata/libfdata_mapped_range.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_support.c` & `libfsntfs-20240501/libfdata/libfdata_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_list_element.c` & `libfsntfs-20240501/libfdata/libfdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_segments_array.c` & `libfsntfs-20240501/libfdata/libfdata_segments_array.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_types.h` & `libfsntfs-20240501/libfdata/libfdata_types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_notify.h` & `libfsntfs-20240501/libfdata/libfdata_notify.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_range_list.h` & `libfsntfs-20240501/libfdata/libfdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_segments_array.h` & `libfsntfs-20240501/libfdata/libfdata_segments_array.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/Makefile.in` & `libfsntfs-20240501/libfdata/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -500,14 +500,16 @@
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
@@ -572,16 +574,16 @@
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
 
@@ -605,15 +607,16 @@
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
@@ -825,24 +828,39 @@
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
 
@@ -938,17 +956,14 @@
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

### Comparing `libfsntfs-20240119/libfdata/libfdata_vector.c` & `libfsntfs-20240501/libfdata/libfdata_vector.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_libfcache.h` & `libfsntfs-20240501/libfdata/libfdata_libfcache.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdata/libfdata_vector.h` & `libfsntfs-20240501/libfdata/libfdata_vector.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/COPYING` & `libfsntfs-20240501/COPYING`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/install-sh` & `libfsntfs-20240501/install-sh`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs.spec` & `libfsntfs-20240501/libfsntfs.spec`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libfsntfs
-Version: 20240119
+Version: 20240501
 Release: 1
 Summary: Library to access the Windows New Technology File System (NTFS) format
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libfsntfs
                
@@ -36,16 +36,16 @@
 
 %description -n libfsntfs-python3
 Python 3 bindings for libfsntfs
 
 %package -n libfsntfs-tools
 Summary: Several tools for reading Windows New Technology File System (NTFS) volumes
 Group: Applications/System
-Requires: libfsntfs = %{version}-%{release} openssl fuse-libs  
-BuildRequires: openssl-devel fuse-devel  
+Requires: libfsntfs = %{version}-%{release} openssl fuse3-libs  
+BuildRequires: openssl-devel fuse3-devel  
 
 %description -n libfsntfs-tools
 Several tools for reading Windows New Technology File System (NTFS) volumes
 
 %prep
 %setup -q
 
@@ -91,10 +91,10 @@
 %files -n libfsntfs-tools
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Fri Jan 19 2024 Joachim Metz <joachim.metz@gmail.com> 20240119-1
+* Wed May  1 2024 Joachim Metz <joachim.metz@gmail.com> 20240501-1
 - Auto-generated
```

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_string.c` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_string.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_guid.c` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_guid.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_security_descriptor_attribute.c` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_security_descriptor_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_integer.c` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_integer.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_mft_metadata_file_entries.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_mft_metadata_file_entries.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_error.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_file_attribute_flags.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_file_attribute_flags.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_object_identifier_attribute.c` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_object_identifier_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs.c` & `libfsntfs-20240501/pyfsntfs/pyfsntfs.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_libclocale.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_volume_information_attribute.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_volume_information_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_libfguid.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_standard_information_attribute.c` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_standard_information_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_string.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_string.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_libcerror.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_volume_file_entries.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_volume_file_entries.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_reparse_point_attribute.c` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_reparse_point_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_security_descriptor_attribute.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_security_descriptor_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/Makefile.am` & `libfsntfs-20240501/pyfsntfs/Makefile.am`

 * *Files 6% similar despite different names*

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
@@ -65,13 +65,11 @@
 	@LIBFGUID_LIBADD@
 
 pyfsntfs_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pyfsntfs_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_volume.c` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_volume.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_volume_information_attribute.c` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_volume_information_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_file_entry.c` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_file_entry.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_object_identifier_attribute.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_object_identifier_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_file_entry.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_file_entry.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_python.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_python.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_volume_file_entries.c` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_volume_file_entries.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_usn_change_journal.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_usn_change_journal.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_data_streams.c` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_data_streams.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_file_object_io_handle.c` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_file_object_io_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_datetime.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_datetime.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_attribute.c` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_file_object_io_handle.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_file_object_io_handle.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_integer.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_integer.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_datetime.c` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_datetime.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_reparse_point_attribute.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_reparse_point_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_standard_information_attribute.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_standard_information_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_file_name_attribute.c` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_file_name_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_mft_metadata_file.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_mft_metadata_file.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_volume.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_volume.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_guid.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_guid.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_data_streams.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_data_streams.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_libbfio.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_attributes.c` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_attributes.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_attributes.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_attributes.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_file_name_attribute.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_file_name_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_file_entries.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_file_entries.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_attribute_types.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_attribute_types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_volume_name_attribute.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_volume_name_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_error.c` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_data_stream.c` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_data_stream.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_file_entries.c` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_file_entries.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_libuna.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_libuna.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_mft_metadata_file.c` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_mft_metadata_file.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_attribute_types.c` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_attribute_types.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_mft_metadata_file_entries.c` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_mft_metadata_file_entries.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_libfsntfs.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_libfsntfs.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_attribute.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/Makefile.in` & `libfsntfs-20240501/pyfsntfs/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -587,14 +587,16 @@
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
@@ -659,16 +661,16 @@
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
@@ -724,15 +726,16 @@
 @HAVE_PYTHON_TRUE@	@LIBCFILE_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBBFIO_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBFGUID_LIBADD@
 
 @HAVE_PYTHON_TRUE@pyfsntfs_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pyfsntfs_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -1174,24 +1177,53 @@
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
+		-rm -f ./$(DEPDIR)/pyfsntfs_la-pyfsntfs.Plo
+	-rm -f ./$(DEPDIR)/pyfsntfs_la-pyfsntfs_attribute.Plo
+	-rm -f ./$(DEPDIR)/pyfsntfs_la-pyfsntfs_attribute_types.Plo
+	-rm -f ./$(DEPDIR)/pyfsntfs_la-pyfsntfs_attributes.Plo
+	-rm -f ./$(DEPDIR)/pyfsntfs_la-pyfsntfs_data_stream.Plo
+	-rm -f ./$(DEPDIR)/pyfsntfs_la-pyfsntfs_data_streams.Plo
+	-rm -f ./$(DEPDIR)/pyfsntfs_la-pyfsntfs_datetime.Plo
+	-rm -f ./$(DEPDIR)/pyfsntfs_la-pyfsntfs_error.Plo
+	-rm -f ./$(DEPDIR)/pyfsntfs_la-pyfsntfs_file_attribute_flags.Plo
+	-rm -f ./$(DEPDIR)/pyfsntfs_la-pyfsntfs_file_entries.Plo
+	-rm -f ./$(DEPDIR)/pyfsntfs_la-pyfsntfs_file_entry.Plo
+	-rm -f ./$(DEPDIR)/pyfsntfs_la-pyfsntfs_file_name_attribute.Plo
+	-rm -f ./$(DEPDIR)/pyfsntfs_la-pyfsntfs_file_object_io_handle.Plo
+	-rm -f ./$(DEPDIR)/pyfsntfs_la-pyfsntfs_guid.Plo
+	-rm -f ./$(DEPDIR)/pyfsntfs_la-pyfsntfs_integer.Plo
+	-rm -f ./$(DEPDIR)/pyfsntfs_la-pyfsntfs_mft_metadata_file.Plo
+	-rm -f ./$(DEPDIR)/pyfsntfs_la-pyfsntfs_mft_metadata_file_entries.Plo
+	-rm -f ./$(DEPDIR)/pyfsntfs_la-pyfsntfs_object_identifier_attribute.Plo
+	-rm -f ./$(DEPDIR)/pyfsntfs_la-pyfsntfs_reparse_point_attribute.Plo
+	-rm -f ./$(DEPDIR)/pyfsntfs_la-pyfsntfs_security_descriptor_attribute.Plo
+	-rm -f ./$(DEPDIR)/pyfsntfs_la-pyfsntfs_standard_information_attribute.Plo
+	-rm -f ./$(DEPDIR)/pyfsntfs_la-pyfsntfs_string.Plo
+	-rm -f ./$(DEPDIR)/pyfsntfs_la-pyfsntfs_usn_change_journal.Plo
+	-rm -f ./$(DEPDIR)/pyfsntfs_la-pyfsntfs_volume.Plo
+	-rm -f ./$(DEPDIR)/pyfsntfs_la-pyfsntfs_volume_file_entries.Plo
+	-rm -f ./$(DEPDIR)/pyfsntfs_la-pyfsntfs_volume_information_attribute.Plo
+	-rm -f ./$(DEPDIR)/pyfsntfs_la-pyfsntfs_volume_name_attribute.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1302,13 +1334,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-pyexecLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_data_stream.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_data_stream.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_usn_change_journal.c` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_usn_change_journal.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_file_attribute_flags.c` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_file_attribute_flags.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_volume_name_attribute.c` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_volume_name_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/pyfsntfs/pyfsntfs_unused.h` & `libfsntfs-20240501/pyfsntfs/pyfsntfs_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/depcomp` & `libfsntfs-20240501/depcomp`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfguid/libfguid_error.c` & `libfsntfs-20240501/libfguid/libfguid_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfguid/libfguid_support.h` & `libfsntfs-20240501/libfguid/libfguid_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfguid/libfguid_identifier.h` & `libfsntfs-20240501/libfguid/libfguid_identifier.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfguid/libfguid_libcerror.h` & `libfsntfs-20240501/libfguid/libfguid_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfguid/Makefile.am` & `libfsntfs-20240501/libfguid/Makefile.am`

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

### Comparing `libfsntfs-20240119/libfguid/libfguid_unused.h` & `libfsntfs-20240501/libfguid/libfguid_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfguid/libfguid_extern.h` & `libfsntfs-20240501/libfguid/libfguid_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfguid/libfguid_types.h` & `libfsntfs-20240501/libfguid/libfguid_types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfguid/libfguid_identifier.c` & `libfsntfs-20240501/libfguid/libfguid_identifier.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfguid/libfguid_support.c` & `libfsntfs-20240501/libfguid/libfguid_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfguid/libfguid_definitions.h` & `libfsntfs-20240501/libfguid/libfguid_definitions.h`

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

### Comparing `libfsntfs-20240119/libfguid/Makefile.in` & `libfsntfs-20240501/libfguid/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -476,14 +476,16 @@
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
@@ -548,30 +550,31 @@
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
@@ -773,24 +776,29 @@
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
 
@@ -876,17 +884,14 @@
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

### Comparing `libfsntfs-20240119/libfguid/libfguid_error.h` & `libfsntfs-20240501/libfguid/libfguid_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/m4/libfwnt.m4` & `libfsntfs-20240501/m4/libfwnt.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfwnt required headers and functions
 dnl
-dnl Version: 20191217
+dnl Version: 20240413
 
 dnl Function to detect if libfwnt is available
 dnl ac_libfwnt_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFWNT_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfwnt" = xno],
     [ac_cv_libfwnt=no],
     [ac_cv_libfwnt=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfwnt which returns "yes" and --with-libfwnt= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect],
+      [test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_with_libfwnt" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfwnt"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfwnt}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfwnt}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfwnt],
           [1])
@@ -214,16 +216,17 @@
           fwnt,
           libfwnt_lzxpress_huffman_decompress,
           [ac_cv_libfwnt_dummy=yes],
           [ac_cv_libfwnt=no])
 
         ac_cv_libfwnt_LIBADD="-lfwnt"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_libfwnt" != xyes],
+      [test "x$ac_cv_libfwnt" != xyes && test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_with_libfwnt" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfwnt in directory: $ac_cv_with_libfwnt],
         [1])
       ])
     ])
 
   AS_IF(
@@ -245,15 +248,15 @@
     ])
   ])
 
 dnl Function to detect if libfwnt dependencies are available
 AC_DEFUN([AX_LIBFWNT_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfwnt_CPPFLAGS="-I../libfwnt";
+  ac_cv_libfwnt_CPPFLAGS="-I../libfwnt -I\$(top_srcdir)/libfwnt";
   ac_cv_libfwnt_LIBADD="../libfwnt/libfwnt.la";
 
   ac_cv_libfwnt=local
   ])
 
 dnl Function to detect how to enable libfwnt
 AC_DEFUN([AX_LIBFWNT_CHECK_ENABLE],
```

### Comparing `libfsntfs-20240119/m4/libcfile.m4` & `libfsntfs-20240501/m4/libcfile.m4`

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

### Comparing `libfsntfs-20240119/m4/libfdatetime.m4` & `libfsntfs-20240501/m4/libfdatetime.m4`

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

### Comparing `libfsntfs-20240119/m4/tests.m4` & `libfsntfs-20240501/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/m4/libcpath.m4` & `libfsntfs-20240501/m4/libcpath.m4`

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

### Comparing `libfsntfs-20240119/m4/lib-prefix.m4` & `libfsntfs-20240501/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/m4/progtest.m4` & `libfsntfs-20240501/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/m4/libuna.m4` & `libfsntfs-20240501/m4/libuna.m4`

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

### Comparing `libfsntfs-20240119/m4/gettext.m4` & `libfsntfs-20240501/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/m4/lib-ld.m4` & `libfsntfs-20240501/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/m4/libclocale.m4` & `libfsntfs-20240501/m4/libclocale.m4`

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

### Comparing `libfsntfs-20240119/m4/libcdata.m4` & `libfsntfs-20240501/m4/libcdata.m4`

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

### Comparing `libfsntfs-20240119/m4/libcsplit.m4` & `libfsntfs-20240501/m4/libcsplit.m4`

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

### Comparing `libfsntfs-20240119/m4/common.m4` & `libfsntfs-20240501/m4/common.m4`

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

### Comparing `libfsntfs-20240119/m4/libcthreads.m4` & `libfsntfs-20240501/m4/libcthreads.m4`

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

### Comparing `libfsntfs-20240119/m4/ltversion.m4` & `libfsntfs-20240501/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/m4/ltsugar.m4` & `libfsntfs-20240501/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/m4/libfdata.m4` & `libfsntfs-20240501/m4/libfdata.m4`

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

### Comparing `libfsntfs-20240119/m4/host-cpu-c-abi.m4` & `libfsntfs-20240501/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/m4/libfusn.m4` & `libfsntfs-20240501/m4/libfusn.m4`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfusn required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libfusn is available
 dnl ac_libfusn_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFUSN_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfusn" = xno],
     [ac_cv_libfusn=no],
     [ac_cv_libfusn=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfusn which returns "yes" and --with-libfusn= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfusn" != x && test "x$ac_cv_with_libfusn" != xauto-detect],
+      [test "x$ac_cv_with_libfusn" != x && test "x$ac_cv_with_libfusn" != xauto-detect && test "x$ac_cv_with_libfusn" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfusn"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfusn}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfusn}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfusn],
           [1])
@@ -75,16 +77,17 @@
           fusn,
           libfusn_record_get_size,
           [ac_cv_libfusn_dummy=yes],
           [ac_cv_libfusn=no])
 
         ac_cv_libfusn_LIBADD="-lfusn"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfusn" != x && test "x$ac_cv_with_libfusn" != xauto-detect && test "x$ac_cv_libfusn" != xyes],
+      [test "x$ac_cv_libfusn" != xyes && test "x$ac_cv_with_libfusn" != x && test "x$ac_cv_with_libfusn" != xauto-detect && test "x$ac_cv_with_libfusn" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfusn in directory: $ac_cv_with_libfusn],
         [1])
       ])
     ])
 
   AS_IF(
@@ -106,15 +109,15 @@
     ])
   ])
 
 dnl Function to detect if libfusn dependencies are available
 AC_DEFUN([AX_LIBFUSN_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfusn_CPPFLAGS="-I../libfusn";
+  ac_cv_libfusn_CPPFLAGS="-I../libfusn -I\$(top_srcdir)/libfusn";
   ac_cv_libfusn_LIBADD="../libfusn/libfusn.la";
 
   ac_cv_libfusn=local
   ])
 
 dnl Function to detect how to enable libfusn
 AC_DEFUN([AX_LIBFUSN_CHECK_ENABLE],
```

### Comparing `libfsntfs-20240119/m4/libfuse.m4` & `libfsntfs-20240501/m4/libfuse.m4`

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

### Comparing `libfsntfs-20240119/m4/libtool.m4` & `libfsntfs-20240501/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/m4/po.m4` & `libfsntfs-20240501/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/m4/libcerror.m4` & `libfsntfs-20240501/m4/libcerror.m4`

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

### Comparing `libfsntfs-20240119/m4/libcnotify.m4` & `libfsntfs-20240501/m4/libcnotify.m4`

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

### Comparing `libfsntfs-20240119/m4/libfguid.m4` & `libfsntfs-20240501/m4/libfguid.m4`

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

### Comparing `libfsntfs-20240119/m4/libbfio.m4` & `libfsntfs-20240501/m4/libbfio.m4`

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

### Comparing `libfsntfs-20240119/m4/libhmac.m4` & `libfsntfs-20240501/m4/libhmac.m4`

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

### Comparing `libfsntfs-20240119/m4/intlmacosx.m4` & `libfsntfs-20240501/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/m4/lt~obsolete.m4` & `libfsntfs-20240501/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/m4/lib-link.m4` & `libfsntfs-20240501/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/m4/iconv.m4` & `libfsntfs-20240501/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/m4/ltoptions.m4` & `libfsntfs-20240501/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/m4/nls.m4` & `libfsntfs-20240501/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/m4/python.m4` & `libfsntfs-20240501/m4/python.m4`

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

### Comparing `libfsntfs-20240119/m4/libcrypto.m4` & `libfsntfs-20240501/m4/libcrypto.m4`

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

### Comparing `libfsntfs-20240119/m4/types.m4` & `libfsntfs-20240501/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/m4/libfcache.m4` & `libfsntfs-20240501/m4/libfcache.m4`

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

### Comparing `libfsntfs-20240119/m4/pthread.m4` & `libfsntfs-20240501/m4/pthread.m4`

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

### Comparing `libfsntfs-20240119/include/libfsntfs.h` & `libfsntfs-20240501/include/libfsntfs.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/include/libfsntfs.h.in` & `libfsntfs-20240501/include/libfsntfs.h.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/include/libfsntfs/definitions.h.in` & `libfsntfs-20240501/include/libfsntfs/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/include/libfsntfs/definitions.h` & `libfsntfs-20240501/include/libfsntfs/definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBFSNTFS_DEFINITIONS_H )
 #define _LIBFSNTFS_DEFINITIONS_H
 
 #include <libfsntfs/types.h>
 
-#define LIBFSNTFS_VERSION					20240119
+#define LIBFSNTFS_VERSION					20240501
 
 /* The version string
  */
-#define LIBFSNTFS_VERSION_STRING				"20240119"
+#define LIBFSNTFS_VERSION_STRING				"20240501"
 
 /* The file access
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBFSNTFS_ACCESS_FLAGS
```

### Comparing `libfsntfs-20240119/include/libfsntfs/types.h.in` & `libfsntfs-20240501/include/libfsntfs/types.h.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/include/libfsntfs/types.h` & `libfsntfs-20240501/include/libfsntfs/types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/include/libfsntfs/features.h.in` & `libfsntfs-20240501/include/libfsntfs/features.h.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/include/libfsntfs/error.h` & `libfsntfs-20240501/include/libfsntfs/error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/include/libfsntfs/extern.h` & `libfsntfs-20240501/include/libfsntfs/extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/include/libfsntfs/features.h` & `libfsntfs-20240501/include/libfsntfs/features.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/include/libfsntfs/codepage.h` & `libfsntfs-20240501/include/libfsntfs/codepage.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/include/Makefile.in` & `libfsntfs-20240501/include/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -466,14 +466,16 @@
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
@@ -554,15 +556,20 @@
 
 EXTRA_DIST = \
 	libfsntfs.h.in \
 	libfsntfs/definitions.h.in \
 	libfsntfs/features.h.in \
 	libfsntfs/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfsntfs.h \
+	libfsntfs/definitions.h \
+	libfsntfs/features.h \
+	libfsntfs/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -759,23 +766,25 @@
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
@@ -857,17 +866,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libfsntfs.h
-	-rm -f libfsntfs/definitions.h
-	-rm -f libfsntfs/features.h
-	-rm -f libfsntfs/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfsntfs-20240119/common/config_borlandc.h` & `libfsntfs-20240501/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/common/file_stream.h` & `libfsntfs-20240501/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/common/memory.h` & `libfsntfs-20240501/common/memory.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/common/byte_stream.h` & `libfsntfs-20240501/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/common/common.h` & `libfsntfs-20240501/common/common.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/common/config_winapi.h` & `libfsntfs-20240501/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/common/system_string.h` & `libfsntfs-20240501/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/common/types.h.in` & `libfsntfs-20240501/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/common/types.h` & `libfsntfs-20240501/common/types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/common/config.h.in` & `libfsntfs-20240501/common/config.h.in`

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
 /* Define to 1 if you have the `fusn' library (-lfusn). */
 #undef HAVE_LIBFUSN
 
 /* Define to 1 if you have the <libfusn.h> header file. */
 #undef HAVE_LIBFUSN_H
 
 /* Define to 1 if you have the `fwnt' library (-lfwnt). */
```

### Comparing `libfsntfs-20240119/common/config.h` & `libfsntfs-20240501/common/config.h`

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
 
 /* Define to 1 if you have the `fusn' library (-lfusn). */
 /* #undef HAVE_LIBFUSN */
 
 /* Define to 1 if you have the <libfusn.h> header file. */
 /* #undef HAVE_LIBFUSN_H */
 
@@ -610,24 +613,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libfsntfs"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libfsntfs 20240119"
+#define PACKAGE_STRING "libfsntfs 20240501"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libfsntfs"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240119"
+#define PACKAGE_VERSION "20240501"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -648,15 +651,15 @@
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Define to 1 if your <sys/time.h> declares `struct tm'. */
 /* #undef TM_IN_SYS_TIME */
 
 /* Version number of package */
-#define VERSION "20240119"
+#define VERSION "20240501"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libfsntfs-20240119/common/wide_string.h` & `libfsntfs-20240501/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/common/narrow_string.h` & `libfsntfs-20240501/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/common/config_msc.h` & `libfsntfs-20240501/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/common/Makefile.in` & `libfsntfs-20240501/common/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -436,14 +436,16 @@
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
@@ -507,15 +509,17 @@
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
@@ -523,15 +527,18 @@
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
@@ -699,23 +706,25 @@
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
@@ -795,15 +804,10 @@
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

### Comparing `libfsntfs-20240119/libclocale/libclocale_wide_string.c` & `libfsntfs-20240501/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libclocale/libclocale_support.h` & `libfsntfs-20240501/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libclocale/Makefile.am` & `libfsntfs-20240501/libclocale/Makefile.am`

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

### Comparing `libfsntfs-20240119/libclocale/libclocale_definitions.h` & `libfsntfs-20240501/libclocale/libclocale_definitions.h`

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

### Comparing `libfsntfs-20240119/libclocale/libclocale_unused.h` & `libfsntfs-20240501/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libclocale/libclocale_libcerror.h` & `libfsntfs-20240501/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libclocale/libclocale_locale.h` & `libfsntfs-20240501/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libclocale/libclocale_support.c` & `libfsntfs-20240501/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libclocale/libclocale_codepage.c` & `libfsntfs-20240501/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libclocale/libclocale_locale.c` & `libfsntfs-20240501/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libclocale/Makefile.in` & `libfsntfs-20240501/libclocale/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -480,14 +480,16 @@
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
@@ -553,30 +555,31 @@
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
@@ -779,24 +782,30 @@
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
 
@@ -883,17 +892,14 @@
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

### Comparing `libfsntfs-20240119/libclocale/libclocale_extern.h` & `libfsntfs-20240501/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libclocale/libclocale_wide_string.h` & `libfsntfs-20240501/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libclocale/libclocale_codepage.h` & `libfsntfs-20240501/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfcache/libfcache_libcdata.h` & `libfsntfs-20240501/libfcache/libfcache_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfcache/libfcache_types.h` & `libfsntfs-20240501/libfcache/libfcache_types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfcache/libfcache_cache_value.c` & `libfsntfs-20240501/libfcache/libfcache_cache_value.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfcache/libfcache_unused.h` & `libfsntfs-20240501/libfcache/libfcache_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfcache/Makefile.am` & `libfsntfs-20240501/libfcache/Makefile.am`

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

### Comparing `libfsntfs-20240119/libfcache/libfcache_support.h` & `libfsntfs-20240501/libfcache/libfcache_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfcache/libfcache_error.h` & `libfsntfs-20240501/libfcache/libfcache_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfcache/libfcache_support.c` & `libfsntfs-20240501/libfcache/libfcache_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfcache/libfcache_cache.h` & `libfsntfs-20240501/libfcache/libfcache_cache.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfcache/libfcache_error.c` & `libfsntfs-20240501/libfcache/libfcache_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfcache/libfcache_libcerror.h` & `libfsntfs-20240501/libfcache/libfcache_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfcache/libfcache_date_time.c` & `libfsntfs-20240501/libfcache/libfcache_date_time.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfcache/libfcache_extern.h` & `libfsntfs-20240501/libfcache/libfcache_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfcache/libfcache_cache_value.h` & `libfsntfs-20240501/libfcache/libfcache_cache_value.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfcache/Makefile.in` & `libfsntfs-20240501/libfcache/Makefile.in`

 * *Files 2% similar despite different names*

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
@@ -555,16 +557,16 @@
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
@@ -576,15 +578,16 @@
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
@@ -788,24 +791,31 @@
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
 
@@ -893,17 +903,14 @@
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

### Comparing `libfsntfs-20240119/libfcache/libfcache_date_time.h` & `libfsntfs-20240501/libfcache/libfcache_date_time.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfcache/libfcache_definitions.h` & `libfsntfs-20240501/libfcache/libfcache_definitions.h`

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

### Comparing `libfsntfs-20240119/libfcache/libfcache_cache.c` & `libfsntfs-20240501/libfcache/libfcache_cache.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/Makefile.am` & `libfsntfs-20240501/Makefile.am`

 * *Files 6% similar despite different names*

```diff
@@ -62,16 +62,23 @@
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
+	libfsntfs.pc \
+	libfsntfs.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 
 pkgconfig_DATA = \
 	libfsntfs.pc
 
 libtool: @LIBTOOL_DEPS@
@@ -95,19 +102,7 @@
 	(cd $(srcdir)/libfdata && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdatetime && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfguid && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfwnt && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfsntfs && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libfsntfs.pc
-	-rm -f libfsntfs.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
```

### Comparing `libfsntfs-20240119/libbfio/libbfio_file_range.h` & `libfsntfs-20240501/libbfio/libbfio_file_range.h`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_file_range_io_handle.c` & `libfsntfs-20240501/libbfio/libbfio_file_range_io_handle.c`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_support.c` & `libfsntfs-20240501/libbfio/libbfio_support.c`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_libcpath.h` & `libfsntfs-20240501/libbfio/libbfio_libcpath.h`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_error.h` & `libfsntfs-20240501/libbfio/libbfio_error.h`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_libclocale.h` & `libfsntfs-20240501/libbfio/libbfio_libclocale.h`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_error.c` & `libfsntfs-20240501/libbfio/libbfio_error.c`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_libuna.h` & `libfsntfs-20240501/libbfio/libbfio_libuna.h`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_file_io_handle.h` & `libfsntfs-20240501/libbfio/libbfio_file_io_handle.h`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_file_pool.h` & `libfsntfs-20240501/libbfio/libbfio_file_pool.h`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_file_range.c` & `libfsntfs-20240501/libbfio/libbfio_file_range.c`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_types.h` & `libfsntfs-20240501/libbfio/libbfio_types.h`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_unused.h` & `libfsntfs-20240501/libbfio/libbfio_unused.h`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_libcdata.h` & `libfsntfs-20240501/libbfio/libbfio_libcdata.h`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_file.h` & `libfsntfs-20240501/libbfio/libbfio_file.h`

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

### Comparing `libfsntfs-20240119/libbfio/Makefile.am` & `libfsntfs-20240501/libbfio/Makefile.am`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_libcfile.h` & `libfsntfs-20240501/libbfio/libbfio_libcfile.h`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_definitions.h` & `libfsntfs-20240501/libbfio/libbfio_definitions.h`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_codepage.h` & `libfsntfs-20240501/libbfio/libbfio_codepage.h`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_file_io_handle.c` & `libfsntfs-20240501/libbfio/libbfio_file_io_handle.c`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_support.h` & `libfsntfs-20240501/libbfio/libbfio_support.h`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_memory_range.h` & `libfsntfs-20240501/libbfio/libbfio_memory_range.h`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_file_pool.c` & `libfsntfs-20240501/libbfio/libbfio_file_pool.c`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_file_range_io_handle.h` & `libfsntfs-20240501/libbfio/libbfio_file_range_io_handle.h`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_libcthreads.h` & `libfsntfs-20240501/libbfio/libbfio_libcthreads.h`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_system_string.h` & `libfsntfs-20240501/libbfio/libbfio_system_string.h`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_memory_range_io_handle.c` & `libfsntfs-20240501/libbfio/libbfio_memory_range_io_handle.c`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_handle.c` & `libfsntfs-20240501/libbfio/libbfio_handle.c`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_file.c` & `libfsntfs-20240501/libbfio/libbfio_file.c`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_handle.h` & `libfsntfs-20240501/libbfio/libbfio_handle.h`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_memory_range.c` & `libfsntfs-20240501/libbfio/libbfio_memory_range.c`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_pool.c` & `libfsntfs-20240501/libbfio/libbfio_pool.c`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_libcerror.h` & `libfsntfs-20240501/libbfio/libbfio_libcerror.h`

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

### Comparing `libfsntfs-20240119/libbfio/Makefile.in` & `libfsntfs-20240501/libbfio/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -501,14 +501,16 @@
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
@@ -573,16 +575,16 @@
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
@@ -613,15 +615,16 @@
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
@@ -832,24 +835,38 @@
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
 
@@ -918,14 +935,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -936,23 +955,22 @@
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

### Comparing `libfsntfs-20240119/libbfio/libbfio_system_string.c` & `libfsntfs-20240501/libbfio/libbfio_system_string.c`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_memory_range_io_handle.h` & `libfsntfs-20240501/libbfio/libbfio_memory_range_io_handle.h`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_extern.h` & `libfsntfs-20240501/libbfio/libbfio_extern.h`

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

### Comparing `libfsntfs-20240119/libbfio/libbfio_pool.h` & `libfsntfs-20240501/libbfio/libbfio_pool.h`

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

### Comparing `libfsntfs-20240119/config.guess` & `libfsntfs-20240501/config.guess`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/dpkg/copyright` & `libfsntfs-20240501/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/dpkg/control` & `libfsntfs-20240501/dpkg/control`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/dpkg/rules` & `libfsntfs-20240501/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/COPYING.LESSER` & `libfsntfs-20240501/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/configure` & `libfsntfs-20240501/configure`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libfsntfs 20240119.
+# Generated by GNU Autoconf 2.71 for libfsntfs 20240501.
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
 PACKAGE_NAME='libfsntfs'
 PACKAGE_TARNAME='libfsntfs'
-PACKAGE_VERSION='20240119'
-PACKAGE_STRING='libfsntfs 20240119'
+PACKAGE_VERSION='20240501'
+PACKAGE_STRING='libfsntfs 20240501'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libfsntfs.h.in"
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
@@ -1157,14 +1159,16 @@
 libfwnt_LIBS
 libfusn_CFLAGS
 libfusn_LIBS
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
@@ -1707,15 +1711,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libfsntfs 20240119 to adapt to many kinds of systems.
+\`configure' configures libfsntfs 20240501 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1778,15 +1782,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libfsntfs 20240119:";;
+     short | recursive ) echo "Configuration of libfsntfs 20240501:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1991,14 +1995,17 @@
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
@@ -2061,15 +2068,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libfsntfs configure 20240119
+libfsntfs configure 20240501
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2782,15 +2789,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libfsntfs $as_me 20240119, which was
+It was created by libfsntfs $as_me 20240501, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4271,15 +4278,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libfsntfs'
- VERSION='20240119'
+ VERSION='20240501'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -23866,15 +23873,15 @@
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
@@ -24365,15 +24372,16 @@
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
@@ -24515,15 +24523,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -24617,15 +24625,15 @@
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
@@ -26257,15 +26265,15 @@
 
 
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
@@ -26319,47 +26327,52 @@
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
@@ -26393,15 +26406,15 @@
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
@@ -26435,15 +26448,15 @@
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
@@ -26478,15 +26491,15 @@
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
@@ -26520,15 +26533,15 @@
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
@@ -26562,15 +26575,15 @@
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
@@ -26604,15 +26617,15 @@
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
@@ -26646,15 +26659,15 @@
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
@@ -26689,15 +26702,15 @@
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
@@ -26731,15 +26744,15 @@
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
@@ -26773,15 +26786,15 @@
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
@@ -26815,15 +26828,15 @@
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
@@ -26857,15 +26870,15 @@
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
@@ -26900,15 +26913,15 @@
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
@@ -26942,15 +26955,15 @@
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
@@ -26984,15 +26997,15 @@
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
@@ -27026,15 +27039,15 @@
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
@@ -27068,15 +27081,15 @@
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
@@ -27111,67 +27124,76 @@
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
 
@@ -27259,15 +27281,15 @@
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
@@ -31038,15 +31060,16 @@
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
@@ -31071,15 +31094,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcdata" != xyes
 then :
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDATA 1" >>confdefs.h
@@ -31149,15 +31172,15 @@
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
@@ -31704,15 +31727,16 @@
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
@@ -31868,15 +31892,15 @@
 
 printf "%s\n" "#define HAVE_LANGINFO_CODESET 1" >>confdefs.h
 
 
 fi
 
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCLOCALE 1" >>confdefs.h
@@ -31946,15 +31970,15 @@
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
@@ -32404,15 +32428,16 @@
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
@@ -32467,15 +32492,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -32545,15 +32570,15 @@
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
@@ -33268,15 +33293,16 @@
 
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
@@ -33301,15 +33327,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcsplit" != xyes
 then :
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCSPLIT 1" >>confdefs.h
@@ -33379,15 +33405,15 @@
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
@@ -40589,15 +40615,16 @@
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
@@ -40622,15 +40649,15 @@
 
 fi
 
 
     if test "x$ac_cv_libuna" != xyes
 then :
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBUNA 1" >>confdefs.h
@@ -40700,15 +40727,15 @@
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
@@ -41889,15 +41916,16 @@
 
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
@@ -42211,15 +42239,15 @@
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
@@ -42289,15 +42317,15 @@
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
@@ -43094,15 +43122,16 @@
 
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
@@ -43292,15 +43321,15 @@
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: mkdir
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCPATH 1" >>confdefs.h
@@ -43370,15 +43399,15 @@
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
@@ -45488,15 +45517,16 @@
 
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
@@ -45521,15 +45551,15 @@
 
 fi
 
 
     if test "x$ac_cv_libbfio" != xyes
 then :
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBBFIO 1" >>confdefs.h
@@ -45599,15 +45629,15 @@
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
@@ -46519,15 +46549,16 @@
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
@@ -46620,15 +46651,15 @@
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
@@ -46698,15 +46729,15 @@
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
@@ -49986,15 +50017,16 @@
 
 
 
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
@@ -50019,15 +50051,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdata" != xyes
 then :
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATA 1" >>confdefs.h
@@ -50097,15 +50129,15 @@
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
@@ -53541,15 +53573,16 @@
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
@@ -53574,15 +53607,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdatetime" != xyes
 then :
 
-  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime";
+  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime -I\$(top_srcdir)/libfdatetime";
   ac_cv_libfdatetime_LIBADD="../libfdatetime/libfdatetime.la";
 
   ac_cv_libfdatetime=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATETIME 1" >>confdefs.h
@@ -53652,15 +53685,15 @@
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
@@ -54234,15 +54267,16 @@
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
@@ -54267,15 +54301,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfguid" != xyes
 then :
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFGUID 1" >>confdefs.h
@@ -54345,15 +54379,15 @@
 printf "%s\n" "$ac_cv_with_libfwnt" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfwnt" = xno
 then :
   ac_cv_libfwnt=no
 else $as_nop
   ac_cv_libfwnt=check
-        if test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect
+                if test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_with_libfwnt" != xyes
 then :
   if test -d "$ac_cv_with_libfwnt"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfwnt}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfwnt}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -55735,15 +55769,16 @@
 fi
 
 
         ac_cv_libfwnt_LIBADD="-lfwnt"
 fi
 
 fi
-    if test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_libfwnt" != xyes
+
+    if test "x$ac_cv_libfwnt" != xyes && test "x$ac_cv_with_libfwnt" != x && test "x$ac_cv_with_libfwnt" != xauto-detect && test "x$ac_cv_with_libfwnt" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfwnt in directory: $ac_cv_with_libfwnt
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -55768,15 +55803,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfwnt" != xyes
 then :
 
-  ac_cv_libfwnt_CPPFLAGS="-I../libfwnt";
+  ac_cv_libfwnt_CPPFLAGS="-I../libfwnt -I\$(top_srcdir)/libfwnt";
   ac_cv_libfwnt_LIBADD="../libfwnt/libfwnt.la";
 
   ac_cv_libfwnt=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFWNT 1" >>confdefs.h
@@ -56112,16 +56147,20 @@
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
 
@@ -56284,15 +56323,15 @@
 printf "%s\n" "$ac_cv_with_libfusn" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfusn" = xno
 then :
   ac_cv_libfusn=no
 else $as_nop
   ac_cv_libfusn=check
-        if test "x$ac_cv_with_libfusn" != x && test "x$ac_cv_with_libfusn" != xauto-detect
+                if test "x$ac_cv_with_libfusn" != x && test "x$ac_cv_with_libfusn" != xauto-detect && test "x$ac_cv_with_libfusn" != xyes
 then :
   if test -d "$ac_cv_with_libfusn"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfusn}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfusn}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -56616,15 +56655,16 @@
 fi
 
 
         ac_cv_libfusn_LIBADD="-lfusn"
 fi
 
 fi
-    if test "x$ac_cv_with_libfusn" != x && test "x$ac_cv_with_libfusn" != xauto-detect && test "x$ac_cv_libfusn" != xyes
+
+    if test "x$ac_cv_libfusn" != xyes && test "x$ac_cv_with_libfusn" != x && test "x$ac_cv_with_libfusn" != xauto-detect && test "x$ac_cv_with_libfusn" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfusn in directory: $ac_cv_with_libfusn
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -56649,15 +56689,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfusn" != xyes
 then :
 
-  ac_cv_libfusn_CPPFLAGS="-I../libfusn";
+  ac_cv_libfusn_CPPFLAGS="-I../libfusn -I\$(top_srcdir)/libfusn";
   ac_cv_libfusn_LIBADD="../libfusn/libfusn.la";
 
   ac_cv_libfusn=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFUSN 1" >>confdefs.h
@@ -56727,15 +56767,15 @@
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
@@ -57733,15 +57773,16 @@
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
@@ -57847,15 +57888,15 @@
 
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
@@ -62033,15 +62074,15 @@
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
@@ -62106,33 +62147,107 @@
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
+fi
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
 fi
+        if test $_pkg_short_errors_supported = yes; then
+                fuse3_PKG_ERRORS=`$PKG_CONFIG --short-errors --print-errors --cflags --libs "fuse3 >= 3.0" 2>&1`
+        else
+                fuse3_PKG_ERRORS=`$PKG_CONFIG --print-errors --cflags --libs "fuse3 >= 3.0" 2>&1`
+        fi
+        # Put the nasty error message in config.log where it belongs
+        echo "$fuse3_PKG_ERRORS" >&5
 
-  if test "x$ac_cv_with_libfuse" = xno
-then :
-  ac_cv_libfuse=no
-else $as_nop
-      if test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"
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
@@ -62200,51 +62315,110 @@
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
@@ -62407,45 +62581,38 @@
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
@@ -62613,29 +62780,49 @@
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
@@ -62666,14 +62853,20 @@
 
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
 
@@ -62681,14 +62874,22 @@
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
 
@@ -63626,15 +63827,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libfsntfs $as_me 20240119, which was
+This file was extended by libfsntfs $as_me 20240501, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -63694,15 +63895,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libfsntfs config.status 20240119
+libfsntfs config.status 20240501
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libfsntfs-20240119/compile` & `libfsntfs-20240501/compile`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/missing` & `libfsntfs-20240501/missing`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/libfdata/libfdata.vcproj` & `libfsntfs-20240501/msvscpp/libfdata/libfdata.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_directory_entries_tree/fsntfs_test_directory_entries_tree.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_directory_entries_tree/fsntfs_test_directory_entries_tree.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_file_name_values/fsntfs_test_file_name_values.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_file_name_values/fsntfs_test_file_name_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_index_node/fsntfs_test_index_node.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_index_node/fsntfs_test_index_node.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_volume_information_values/fsntfs_test_volume_information_values.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_volume_information_values/fsntfs_test_volume_information_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_io_handle/fsntfs_test_io_handle.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_io_handle/fsntfs_test_io_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_compressed_block_data_handle/fsntfs_test_compressed_block_data_handle.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_compressed_block_data_handle/fsntfs_test_compressed_block_data_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_object_identifier_values/fsntfs_test_object_identifier_values.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_object_identifier_values/fsntfs_test_object_identifier_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_profiler/fsntfs_test_profiler.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_profiler/fsntfs_test_profiler.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_data_stream/fsntfs_test_data_stream.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_data_stream/fsntfs_test_data_stream.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/pyfsntfs/pyfsntfs.vcproj` & `libfsntfs-20240501/msvscpp/pyfsntfs/pyfsntfs.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_security_descriptor_values/fsntfs_test_security_descriptor_values.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_security_descriptor_values/fsntfs_test_security_descriptor_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_file_system/fsntfs_test_file_system.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_file_system/fsntfs_test_file_system.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_tools_info_handle/fsntfs_test_tools_info_handle.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_tools_info_handle/fsntfs_test_tools_info_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/libfguid/libfguid.vcproj` & `libfsntfs-20240501/msvscpp/libfguid/libfguid.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_error/fsntfs_test_error.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_error/fsntfs_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_mft_attribute_list_entry/fsntfs_test_mft_attribute_list_entry.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_mft_attribute_list_entry/fsntfs_test_mft_attribute_list_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_mft_entry_header/fsntfs_test_mft_entry_header.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_mft_entry_header/fsntfs_test_mft_entry_header.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_buffer_data_handle/fsntfs_test_buffer_data_handle.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_buffer_data_handle/fsntfs_test_buffer_data_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_file_entry/fsntfs_test_file_entry.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_file_entry/fsntfs_test_file_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_reparse_point_values/fsntfs_test_reparse_point_values.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_reparse_point_values/fsntfs_test_reparse_point_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_security_descriptor_index/fsntfs_test_security_descriptor_index.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_security_descriptor_index/fsntfs_test_security_descriptor_index.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/libclocale/libclocale.vcproj` & `libfsntfs-20240501/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_index/fsntfs_test_index.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_index/fsntfs_test_index.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfsinfo/fsntfsinfo.vcproj` & `libfsntfs-20240501/msvscpp/fsntfsinfo/fsntfsinfo.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_index_entry_vector/fsntfs_test_index_entry_vector.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_index_entry_vector/fsntfs_test_index_entry_vector.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/libfcache/libfcache.vcproj` & `libfsntfs-20240501/msvscpp/libfcache/libfcache.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/Makefile.am` & `libfsntfs-20240501/msvscpp/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -92,13 +92,11 @@
 	libuna/libuna.vcproj \
 	pyfsntfs/pyfsntfs.vcproj \
 	libfsntfs.sln
 
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

### Comparing `libfsntfs-20240119/msvscpp/libbfio/libbfio.vcproj` & `libfsntfs-20240501/msvscpp/libbfio/libbfio.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_fixup_values/fsntfs_test_fixup_values.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_fixup_values/fsntfs_test_fixup_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_index_root_header/fsntfs_test_index_root_header.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_index_root_header/fsntfs_test_index_root_header.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_index_value/fsntfs_test_index_value.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_index_value/fsntfs_test_index_value.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_compression/fsntfs_test_compression.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_compression/fsntfs_test_compression.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_attribute/fsntfs_test_attribute.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_attribute/fsntfs_test_attribute.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_index_entry/fsntfs_test_index_entry.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_index_entry/fsntfs_test_index_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_mft_metadata_file/fsntfs_test_mft_metadata_file.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_mft_metadata_file/fsntfs_test_mft_metadata_file.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_sds_index_value/fsntfs_test_sds_index_value.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_sds_index_value/fsntfs_test_sds_index_value.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_security_descriptor_index_value/fsntfs_test_security_descriptor_index_value.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_security_descriptor_index_value/fsntfs_test_security_descriptor_index_value.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_mft_attribute_list/fsntfs_test_mft_attribute_list.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_mft_attribute_list/fsntfs_test_mft_attribute_list.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_standard_information_values/fsntfs_test_standard_information_values.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_standard_information_values/fsntfs_test_standard_information_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_mft_attribute/fsntfs_test_mft_attribute.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_mft_attribute/fsntfs_test_mft_attribute.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/libcfile/libcfile.vcproj` & `libfsntfs-20240501/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_usn_change_journal/fsntfs_test_usn_change_journal.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_usn_change_journal/fsntfs_test_usn_change_journal.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_compressed_block_vector/fsntfs_test_compressed_block_vector.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_compressed_block_vector/fsntfs_test_compressed_block_vector.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_volume_header/fsntfs_test_volume_header.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_volume_header/fsntfs_test_volume_header.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_tools_mount_path_string/fsntfs_test_tools_mount_path_string.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_tools_mount_path_string/fsntfs_test_tools_mount_path_string.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/libcdata/libcdata.vcproj` & `libfsntfs-20240501/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_volume_name_attribute/fsntfs_test_volume_name_attribute.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_volume_name_attribute/fsntfs_test_volume_name_attribute.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_txf_data_values/fsntfs_test_txf_data_values.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_txf_data_values/fsntfs_test_txf_data_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_compression_unit_descriptor/fsntfs_test_compression_unit_descriptor.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_compression_unit_descriptor/fsntfs_test_compression_unit_descriptor.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_directory_entry/fsntfs_test_directory_entry.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_directory_entry/fsntfs_test_directory_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_tools_digest_hash/fsntfs_test_tools_digest_hash.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_tools_digest_hash/fsntfs_test_tools_digest_hash.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_data_run/fsntfs_test_data_run.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_data_run/fsntfs_test_data_run.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_compressed_block/fsntfs_test_compressed_block.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_compressed_block/fsntfs_test_compressed_block.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_volume_information_attribute/fsntfs_test_volume_information_attribute.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_volume_information_attribute/fsntfs_test_volume_information_attribute.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_mft/fsntfs_test_mft.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_mft/fsntfs_test_mft.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_reparse_point_attribute/fsntfs_test_reparse_point_attribute.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_reparse_point_attribute/fsntfs_test_reparse_point_attribute.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/libcthreads/libcthreads.vcproj` & `libfsntfs-20240501/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_file_name_attribute/fsntfs_test_file_name_attribute.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_file_name_attribute/fsntfs_test_file_name_attribute.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_index_entry_header/fsntfs_test_index_entry_header.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_index_entry_header/fsntfs_test_index_entry_header.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/libfsntfs.sln` & `libfsntfs-20240501/msvscpp/libfsntfs.sln`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/libcpath/libcpath.vcproj` & `libfsntfs-20240501/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_notify/fsntfs_test_notify.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_notify/fsntfs_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfsmount/fsntfsmount.vcproj` & `libfsntfs-20240501/msvscpp/fsntfsmount/fsntfsmount.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_cluster_block/fsntfs_test_cluster_block.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_cluster_block/fsntfs_test_cluster_block.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_tools_path_string/fsntfs_test_tools_path_string.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_tools_path_string/fsntfs_test_tools_path_string.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_cluster_block_stream/fsntfs_test_cluster_block_stream.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_cluster_block_stream/fsntfs_test_cluster_block_stream.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/libfusn/libfusn.vcproj` & `libfsntfs-20240501/msvscpp/libfusn/libfusn.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_cluster_block_vector/fsntfs_test_cluster_block_vector.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_cluster_block_vector/fsntfs_test_cluster_block_vector.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_tools_output/fsntfs_test_tools_output.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_tools_output/fsntfs_test_tools_output.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_volume/fsntfs_test_volume.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_volume/fsntfs_test_volume.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/libfwnt/libfwnt.vcproj` & `libfsntfs-20240501/msvscpp/libfwnt/libfwnt.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_tools_bodyfile/fsntfs_test_tools_bodyfile.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_tools_bodyfile/fsntfs_test_tools_bodyfile.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/libfsntfs/libfsntfs.vcproj` & `libfsntfs-20240501/msvscpp/libfsntfs/libfsntfs.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_name/fsntfs_test_name.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_name/fsntfs_test_name.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_extent/fsntfs_test_extent.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_extent/fsntfs_test_extent.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_index_node_header/fsntfs_test_index_node_header.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_index_node_header/fsntfs_test_index_node_header.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/libhmac/libhmac.vcproj` & `libfsntfs-20240501/msvscpp/libhmac/libhmac.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_attribute_list_entry/fsntfs_test_attribute_list_entry.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_attribute_list_entry/fsntfs_test_attribute_list_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/libcsplit/libcsplit.vcproj` & `libfsntfs-20240501/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_bitmap_values/fsntfs_test_bitmap_values.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_bitmap_values/fsntfs_test_bitmap_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_logged_utility_stream_values/fsntfs_test_logged_utility_stream_values.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_logged_utility_stream_values/fsntfs_test_logged_utility_stream_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/libuna/libuna.vcproj` & `libfsntfs-20240501/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/Makefile.in` & `libfsntfs-20240501/msvscpp/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -418,14 +418,16 @@
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
@@ -587,15 +589,16 @@
 	libuna/libuna.vcproj \
 	pyfsntfs/pyfsntfs.vcproj \
 	libfsntfs.sln
 
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
@@ -699,23 +702,25 @@
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
@@ -794,13 +799,10 @@
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

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_cluster_block_data/fsntfs_test_cluster_block_data.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_cluster_block_data/fsntfs_test_cluster_block_data.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_tools_signal/fsntfs_test_tools_signal.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_tools_signal/fsntfs_test_tools_signal.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_volume_name_values/fsntfs_test_volume_name_values.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_volume_name_values/fsntfs_test_volume_name_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_support/fsntfs_test_support.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_support/fsntfs_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/libcnotify/libcnotify.vcproj` & `libfsntfs-20240501/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_path_hint/fsntfs_test_path_hint.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_path_hint/fsntfs_test_path_hint.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_compressed_data_handle/fsntfs_test_compressed_data_handle.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_compressed_data_handle/fsntfs_test_compressed_data_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_mft_entry/fsntfs_test_mft_entry.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_mft_entry/fsntfs_test_mft_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/libcerror/libcerror.vcproj` & `libfsntfs-20240501/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/libfdatetime/libfdatetime.vcproj` & `libfsntfs-20240501/msvscpp/libfdatetime/libfdatetime.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/msvscpp/fsntfs_test_compression_unit_data_handle/fsntfs_test_compression_unit_data_handle.vcproj` & `libfsntfs-20240501/msvscpp/fsntfs_test_compression_unit_data_handle/fsntfs_test_compression_unit_data_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcfile/libcfile_extern.h` & `libfsntfs-20240501/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcfile/libcfile_support.h` & `libfsntfs-20240501/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcfile/libcfile_unused.h` & `libfsntfs-20240501/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcfile/libcfile_notify.h` & `libfsntfs-20240501/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcfile/libcfile_support.c` & `libfsntfs-20240501/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcfile/libcfile_types.h` & `libfsntfs-20240501/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcfile/Makefile.am` & `libfsntfs-20240501/libcfile/Makefile.am`

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

### Comparing `libfsntfs-20240119/libcfile/libcfile_notify.c` & `libfsntfs-20240501/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcfile/libcfile_system_string.h` & `libfsntfs-20240501/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcfile/libcfile_file.h` & `libfsntfs-20240501/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcfile/libcfile_libcnotify.h` & `libfsntfs-20240501/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcfile/libcfile_system_string.c` & `libfsntfs-20240501/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcfile/libcfile_error.h` & `libfsntfs-20240501/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcfile/libcfile_libcerror.h` & `libfsntfs-20240501/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcfile/libcfile_file.c` & `libfsntfs-20240501/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcfile/libcfile_libclocale.h` & `libfsntfs-20240501/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcfile/libcfile_winapi.h` & `libfsntfs-20240501/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcfile/Makefile.in` & `libfsntfs-20240501/libcfile/Makefile.in`

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
@@ -555,16 +557,16 @@
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
@@ -579,15 +581,16 @@
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
@@ -792,24 +795,32 @@
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
 
@@ -898,17 +909,14 @@
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

### Comparing `libfsntfs-20240119/libcfile/libcfile_error.c` & `libfsntfs-20240501/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcfile/libcfile_libuna.h` & `libfsntfs-20240501/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcfile/libcfile_winapi.c` & `libfsntfs-20240501/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcfile/libcfile_definitions.h` & `libfsntfs-20240501/libcfile/libcfile_definitions.h`

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

### Comparing `libfsntfs-20240119/README` & `libfsntfs-20240501/README`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/INSTALL` & `libfsntfs-20240501/INSTALL`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcdata/libcdata_list_element.h` & `libfsntfs-20240501/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcdata/libcdata_array.h` & `libfsntfs-20240501/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcdata/libcdata_definitions.h` & `libfsntfs-20240501/libcdata/libcdata_definitions.h`

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

### Comparing `libfsntfs-20240119/libcdata/libcdata_libcerror.h` & `libfsntfs-20240501/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcdata/libcdata_unused.h` & `libfsntfs-20240501/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcdata/libcdata_btree.h` & `libfsntfs-20240501/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcdata/libcdata_btree.c` & `libfsntfs-20240501/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcdata/libcdata_support.c` & `libfsntfs-20240501/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcdata/libcdata_list.c` & `libfsntfs-20240501/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcdata/libcdata_extern.h` & `libfsntfs-20240501/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcdata/libcdata_list.h` & `libfsntfs-20240501/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcdata/libcdata_btree_values_list.h` & `libfsntfs-20240501/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcdata/Makefile.am` & `libfsntfs-20240501/libcdata/Makefile.am`

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

### Comparing `libfsntfs-20240119/libcdata/libcdata_btree_node.h` & `libfsntfs-20240501/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcdata/libcdata_range_list_value.h` & `libfsntfs-20240501/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcdata/libcdata_range_list.h` & `libfsntfs-20240501/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcdata/libcdata_range_list.c` & `libfsntfs-20240501/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcdata/libcdata_array.c` & `libfsntfs-20240501/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcdata/libcdata_list_element.c` & `libfsntfs-20240501/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcdata/libcdata_libcthreads.h` & `libfsntfs-20240501/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcdata/libcdata_tree_node.h` & `libfsntfs-20240501/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcdata/libcdata_error.h` & `libfsntfs-20240501/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcdata/libcdata_types.h` & `libfsntfs-20240501/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcdata/libcdata_btree_node.c` & `libfsntfs-20240501/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcdata/libcdata_tree_node.c` & `libfsntfs-20240501/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcdata/libcdata_support.h` & `libfsntfs-20240501/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcdata/Makefile.in` & `libfsntfs-20240501/libcdata/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -497,14 +497,16 @@
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
@@ -569,16 +571,16 @@
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
@@ -595,15 +597,16 @@
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
@@ -813,24 +816,37 @@
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
 
@@ -924,17 +940,14 @@
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

### Comparing `libfsntfs-20240119/libcdata/libcdata_range_list_value.c` & `libfsntfs-20240501/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcdata/libcdata_btree_values_list.c` & `libfsntfs-20240501/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcdata/libcdata_error.c` & `libfsntfs-20240501/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/config.sub` & `libfsntfs-20240501/config.sub`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs.pc.in` & `libfsntfs-20240501/libfsntfs.pc.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/setup.py` & `libfsntfs-20240501/setup.py`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/acinclude.m4` & `libfsntfs-20240501/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/config.rpath` & `libfsntfs-20240501/config.rpath`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcthreads/libcthreads_thread.h` & `libfsntfs-20240501/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcthreads/libcthreads_read_write_lock.h` & `libfsntfs-20240501/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcthreads/libcthreads_thread.c` & `libfsntfs-20240501/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcthreads/libcthreads_thread_pool.h` & `libfsntfs-20240501/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcthreads/libcthreads_support.h` & `libfsntfs-20240501/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcthreads/libcthreads_lock.h` & `libfsntfs-20240501/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcthreads/libcthreads_unused.h` & `libfsntfs-20240501/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcthreads/libcthreads_lock.c` & `libfsntfs-20240501/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcthreads/libcthreads_condition.h` & `libfsntfs-20240501/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcthreads/libcthreads_repeating_thread.h` & `libfsntfs-20240501/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcthreads/Makefile.am` & `libfsntfs-20240501/libcthreads/Makefile.am`

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

### Comparing `libfsntfs-20240119/libcthreads/libcthreads_support.c` & `libfsntfs-20240501/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcthreads/libcthreads_mutex.c` & `libfsntfs-20240501/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcthreads/libcthreads_queue.c` & `libfsntfs-20240501/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcthreads/libcthreads_mutex.h` & `libfsntfs-20240501/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcthreads/libcthreads_types.h` & `libfsntfs-20240501/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcthreads/libcthreads_thread_attributes.h` & `libfsntfs-20240501/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcthreads/libcthreads_condition.c` & `libfsntfs-20240501/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcthreads/libcthreads_error.c` & `libfsntfs-20240501/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcthreads/libcthreads_read_write_lock.c` & `libfsntfs-20240501/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcthreads/libcthreads_libcerror.h` & `libfsntfs-20240501/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcthreads/libcthreads_definitions.h` & `libfsntfs-20240501/libcthreads/libcthreads_definitions.h`

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

### Comparing `libfsntfs-20240119/libcthreads/libcthreads_thread_pool.c` & `libfsntfs-20240501/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcthreads/libcthreads_error.h` & `libfsntfs-20240501/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcthreads/libcthreads_thread_attributes.c` & `libfsntfs-20240501/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcthreads/libcthreads_extern.h` & `libfsntfs-20240501/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcthreads/libcthreads_repeating_thread.c` & `libfsntfs-20240501/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcthreads/Makefile.in` & `libfsntfs-20240501/libcthreads/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -501,14 +501,16 @@
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
@@ -573,16 +575,16 @@
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
@@ -597,15 +599,16 @@
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
@@ -815,24 +818,37 @@
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
 
@@ -926,17 +942,14 @@
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

### Comparing `libfsntfs-20240119/libcthreads/libcthreads_queue.h` & `libfsntfs-20240501/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/fsntfstools_signal.h` & `libfsntfs-20240501/fsntfstools/fsntfstools_signal.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/mount_path_string.h` & `libfsntfs-20240501/fsntfstools/mount_path_string.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/mount_dokan.c` & `libfsntfs-20240501/fsntfstools/mount_dokan.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/mount_file_system.h` & `libfsntfs-20240501/fsntfstools/mount_file_system.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/fsntfstools_signal.c` & `libfsntfs-20240501/fsntfstools/fsntfstools_signal.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/mount_fuse.c` & `libfsntfs-20240501/fsntfstools/mount_fuse.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/info_handle.h` & `libfsntfs-20240501/fsntfstools/info_handle.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/mount_dokan.h` & `libfsntfs-20240501/fsntfstools/mount_dokan.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/fsntfsmount.c` & `libfsntfs-20240501/fsntfstools/fsntfsmount.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/fsntfstools_getopt.c` & `libfsntfs-20240501/fsntfstools/fsntfstools_getopt.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/path_string.h` & `libfsntfs-20240501/fsntfstools/path_string.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/digest_hash.c` & `libfsntfs-20240501/fsntfstools/digest_hash.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/mount_file_system.c` & `libfsntfs-20240501/fsntfstools/mount_file_system.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/fsntfstools_libfguid.h` & `libfsntfs-20240501/fsntfstools/fsntfstools_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/fsntfstools_libfcache.h` & `libfsntfs-20240501/fsntfstools/fsntfstools_libfcache.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/fsntfstools_output.h` & `libfsntfs-20240501/fsntfstools/fsntfstools_output.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/fsntfstools_libbfio.h` & `libfsntfs-20240501/fsntfstools/fsntfstools_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/fsntfstools_libfdata.h` & `libfsntfs-20240501/fsntfstools/fsntfstools_libfdata.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/fsntfstools_libclocale.h` & `libfsntfs-20240501/fsntfstools/fsntfstools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/Makefile.am` & `libfsntfs-20240501/fsntfstools/Makefile.am`

 * *Files 5% similar despite different names*

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
@@ -104,17 +104,15 @@
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libfsntfs/libfsntfs.la \
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
 	@echo "Running splint on fsntfsinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(fsntfsinfo_SOURCES)
```

### Comparing `libfsntfs-20240119/fsntfstools/fsntfstools_libfsntfs.h` & `libfsntfs-20240501/fsntfstools/fsntfstools_libfsntfs.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/fsntfstools_i18n.h` & `libfsntfs-20240501/fsntfstools/fsntfstools_i18n.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/bodyfile.h` & `libfsntfs-20240501/fsntfstools/bodyfile.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/mount_file_entry.c` & `libfsntfs-20240501/fsntfstools/mount_file_entry.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/info_handle.c` & `libfsntfs-20240501/fsntfstools/info_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -2156,15 +2156,15 @@
 				 "%s: unable to retrieve name string.",
 				 function );
 
 				goto on_error;
 			}
 			fprintf(
 			 info_handle->notify_stream,
-			 "\tAttribute name\t\t: " );
+			 "\tAttribute name\t\t\t: " );
 
 			if( info_handle_name_value_fprint(
 			     info_handle,
 			     value_string,
 			     value_string_size - 1,
 			     error ) != 1 )
 			{
```

### Comparing `libfsntfs-20240119/fsntfstools/mount_file_entry.h` & `libfsntfs-20240501/fsntfstools/mount_file_entry.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/fsntfstools_libcerror.h` & `libfsntfs-20240501/fsntfstools/fsntfstools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/fsntfsinfo.c` & `libfsntfs-20240501/fsntfstools/fsntfsinfo.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/fsntfstools_getopt.h` & `libfsntfs-20240501/fsntfstools/fsntfstools_getopt.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/fsntfstools_libcnotify.h` & `libfsntfs-20240501/fsntfstools/fsntfstools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/fsntfstools_libcpath.h` & `libfsntfs-20240501/fsntfstools/fsntfstools_libcpath.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/fsntfstools_libfwnt.h` & `libfsntfs-20240501/fsntfstools/fsntfstools_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/fsntfstools_unused.h` & `libfsntfs-20240501/fsntfstools/fsntfstools_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/mount_handle.h` & `libfsntfs-20240501/fsntfstools/mount_handle.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/mount_path_string.c` & `libfsntfs-20240501/fsntfstools/mount_path_string.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/fsntfstools_libfdatetime.h` & `libfsntfs-20240501/fsntfstools/fsntfstools_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/fsntfstools_libuna.h` & `libfsntfs-20240501/fsntfstools/fsntfstools_libuna.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/fsntfstools_libfusn.h` & `libfsntfs-20240501/fsntfstools/fsntfstools_libfusn.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/mount_handle.c` & `libfsntfs-20240501/fsntfstools/mount_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/fsntfstools_libhmac.h` & `libfsntfs-20240501/fsntfstools/fsntfstools_libhmac.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/Makefile.in` & `libfsntfs-20240501/fsntfstools/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -487,14 +487,16 @@
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
@@ -559,16 +561,16 @@
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
@@ -663,15 +665,16 @@
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libfsntfs/libfsntfs.la \
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
@@ -931,23 +934,40 @@
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
+		-rm -f ./$(DEPDIR)/bodyfile.Po
+	-rm -f ./$(DEPDIR)/digest_hash.Po
+	-rm -f ./$(DEPDIR)/fsntfsinfo.Po
+	-rm -f ./$(DEPDIR)/fsntfsmount.Po
+	-rm -f ./$(DEPDIR)/fsntfstools_getopt.Po
+	-rm -f ./$(DEPDIR)/fsntfstools_output.Po
+	-rm -f ./$(DEPDIR)/fsntfstools_signal.Po
+	-rm -f ./$(DEPDIR)/info_handle.Po
+	-rm -f ./$(DEPDIR)/mount_dokan.Po
+	-rm -f ./$(DEPDIR)/mount_file_entry.Po
+	-rm -f ./$(DEPDIR)/mount_file_system.Po
+	-rm -f ./$(DEPDIR)/mount_fuse.Po
+	-rm -f ./$(DEPDIR)/mount_handle.Po
+	-rm -f ./$(DEPDIR)/mount_path_string.Po
+	-rm -f ./$(DEPDIR)/path_string.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1045,17 +1065,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on fsntfsinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(fsntfsinfo_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfsntfs-20240119/fsntfstools/bodyfile.c` & `libfsntfs-20240501/fsntfstools/bodyfile.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/digest_hash.h` & `libfsntfs-20240501/fsntfstools/digest_hash.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/fsntfstools_output.c` & `libfsntfs-20240501/fsntfstools/fsntfstools_output.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/mount_fuse.h` & `libfsntfs-20240501/fsntfstools/mount_fuse.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/fsntfstools/path_string.c` & `libfsntfs-20240501/fsntfstools/path_string.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/test-driver` & `libfsntfs-20240501/test-driver`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcpath/libcpath_support.c` & `libfsntfs-20240501/libcpath/libcpath_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcpath/libcpath_libcerror.h` & `libfsntfs-20240501/libcpath/libcpath_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcpath/libcpath_definitions.h` & `libfsntfs-20240501/libcpath/libcpath_definitions.h`

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

### Comparing `libfsntfs-20240119/libcpath/Makefile.am` & `libfsntfs-20240501/libcpath/Makefile.am`

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

### Comparing `libfsntfs-20240119/libcpath/libcpath_error.c` & `libfsntfs-20240501/libcpath/libcpath_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcpath/libcpath_extern.h` & `libfsntfs-20240501/libcpath/libcpath_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcpath/libcpath_system_string.h` & `libfsntfs-20240501/libcpath/libcpath_system_string.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcpath/libcpath_support.h` & `libfsntfs-20240501/libcpath/libcpath_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcpath/libcpath_libcsplit.h` & `libfsntfs-20240501/libcpath/libcpath_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcpath/libcpath_system_string.c` & `libfsntfs-20240501/libcpath/libcpath_system_string.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcpath/libcpath_libclocale.h` & `libfsntfs-20240501/libcpath/libcpath_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcpath/libcpath_error.h` & `libfsntfs-20240501/libcpath/libcpath_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcpath/Makefile.in` & `libfsntfs-20240501/libcpath/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -477,14 +477,16 @@
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
@@ -549,16 +551,16 @@
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
@@ -570,15 +572,16 @@
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
@@ -781,24 +784,30 @@
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
 
@@ -885,17 +894,14 @@
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

### Comparing `libfsntfs-20240119/libcpath/libcpath_libuna.h` & `libfsntfs-20240501/libcpath/libcpath_libuna.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcpath/libcpath_unused.h` & `libfsntfs-20240501/libcpath/libcpath_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcpath/libcpath_path.c` & `libfsntfs-20240501/libcpath/libcpath_path.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcpath/libcpath_path.h` & `libfsntfs-20240501/libcpath/libcpath_path.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/ChangeLog` & `libfsntfs-20240501/ChangeLog`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/manuals/libfsntfs.3` & `libfsntfs-20240501/manuals/libfsntfs.3`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/manuals/fsntfsinfo.1` & `libfsntfs-20240501/manuals/fsntfsinfo.1`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/manuals/Makefile.in` & `libfsntfs-20240501/manuals/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -450,14 +450,16 @@
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
@@ -529,15 +531,16 @@
 	fsntfsinfo.1 \
 	libfsntfs.3
 
 EXTRA_DIST = \
 	fsntfsinfo.1 \
 	libfsntfs.3
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -730,23 +733,25 @@
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
@@ -828,13 +833,10 @@
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

### Comparing `libfsntfs-20240119/tests/fsntfs_test_compressed_data_handle.c` & `libfsntfs-20240501/tests/fsntfs_test_compressed_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_volume_header.c` & `libfsntfs-20240501/tests/fsntfs_test_volume_header.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_tools_signal.c` & `libfsntfs-20240501/tests/fsntfs_test_tools_signal.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_security_descriptor_values.c` & `libfsntfs-20240501/tests/fsntfs_test_security_descriptor_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_libcpath.h` & `libfsntfs-20240501/tests/fsntfs_test_libcpath.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_error.c` & `libfsntfs-20240501/tests/fsntfs_test_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_getopt.h` & `libfsntfs-20240501/tests/fsntfs_test_getopt.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_directory_entry.c` & `libfsntfs-20240501/tests/fsntfs_test_directory_entry.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_file_name_attribute.c` & `libfsntfs-20240501/tests/fsntfs_test_file_name_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/pyfsntfs_test_file_entry.py` & `libfsntfs-20240501/tests/pyfsntfs_test_file_entry.py`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_libfdata.h` & `libfsntfs-20240501/tests/fsntfs_test_libfdata.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_libcerror.h` & `libfsntfs-20240501/tests/fsntfs_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_cluster_block.c` & `libfsntfs-20240501/tests/fsntfs_test_cluster_block.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_io_handle.c` & `libfsntfs-20240501/tests/fsntfs_test_io_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_tools_output.c` & `libfsntfs-20240501/tests/fsntfs_test_tools_output.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/test_tools.sh` & `libfsntfs-20240501/tests/test_tools.sh`

 * *Files 10% similar despite different names*

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
 
 TOOLS_TESTS="bodyfile digest_hash info_handle mount_path_string output path_string signal";
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

### Comparing `libfsntfs-20240119/tests/fsntfs_test_attribute_list_entry.c` & `libfsntfs-20240501/tests/fsntfs_test_attribute_list_entry.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_mft_entry_header.c` & `libfsntfs-20240501/tests/fsntfs_test_mft_entry_header.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_cluster_block_data.c` & `libfsntfs-20240501/tests/fsntfs_test_cluster_block_data.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_volume_name_attribute.c` & `libfsntfs-20240501/tests/fsntfs_test_volume_name_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_index_entry.c` & `libfsntfs-20240501/tests/fsntfs_test_index_entry.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_macros.h` & `libfsntfs-20240501/tests/fsntfs_test_macros.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_compression_unit_data_handle.c` & `libfsntfs-20240501/tests/fsntfs_test_compression_unit_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_compressed_block_vector.c` & `libfsntfs-20240501/tests/fsntfs_test_compressed_block_vector.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_compressed_block.c` & `libfsntfs-20240501/tests/fsntfs_test_compressed_block.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_fixup_values.c` & `libfsntfs-20240501/tests/fsntfs_test_fixup_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_mft_attribute_list_entry.c` & `libfsntfs-20240501/tests/fsntfs_test_mft_attribute_list_entry.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_security_descriptor_index.c` & `libfsntfs-20240501/tests/fsntfs_test_security_descriptor_index.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/Makefile.am` & `libfsntfs-20240501/tests/Makefile.am`

 * *Files 0% similar despite different names*

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
@@ -1204,13 +1204,12 @@
 	fsntfs_test_unused.h \
 	fsntfs_test_volume_name_values.c
 
 fsntfs_test_volume_name_values_LDADD = \
 	../libfsntfs/libfsntfs.la \
 	@LIBCERROR_LIBADD@
 
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

### Comparing `libfsntfs-20240119/tests/fsntfs_test_support.c` & `libfsntfs-20240501/tests/fsntfs_test_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_logged_utility_stream_values.c` & `libfsntfs-20240501/tests/fsntfs_test_logged_utility_stream_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_rwlock.h` & `libfsntfs-20240501/tests/fsntfs_test_rwlock.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_standard_information_values.c` & `libfsntfs-20240501/tests/fsntfs_test_standard_information_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_tools_digest_hash.c` & `libfsntfs-20240501/tests/fsntfs_test_tools_digest_hash.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_memory.h` & `libfsntfs-20240501/tests/fsntfs_test_memory.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_volume_information_values.c` & `libfsntfs-20240501/tests/fsntfs_test_volume_information_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_sds_index_value.c` & `libfsntfs-20240501/tests/fsntfs_test_sds_index_value.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_index_entry_vector.c` & `libfsntfs-20240501/tests/fsntfs_test_index_entry_vector.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_file_system.c` & `libfsntfs-20240501/tests/fsntfs_test_file_system.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_functions.h` & `libfsntfs-20240501/tests/fsntfs_test_functions.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_attribute.c` & `libfsntfs-20240501/tests/fsntfs_test_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_index.c` & `libfsntfs-20240501/tests/fsntfs_test_index.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_functions.c` & `libfsntfs-20240501/tests/fsntfs_test_functions.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_extent.c` & `libfsntfs-20240501/tests/fsntfs_test_extent.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_reparse_point_values.c` & `libfsntfs-20240501/tests/fsntfs_test_reparse_point_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_tools_mount_path_string.c` & `libfsntfs-20240501/tests/fsntfs_test_tools_mount_path_string.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_path_hint.c` & `libfsntfs-20240501/tests/fsntfs_test_path_hint.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_mft_attribute.c` & `libfsntfs-20240501/tests/fsntfs_test_mft_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_rwlock.c` & `libfsntfs-20240501/tests/fsntfs_test_rwlock.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_mft.c` & `libfsntfs-20240501/tests/fsntfs_test_mft.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_index_node_header.c` & `libfsntfs-20240501/tests/fsntfs_test_index_node_header.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_getopt.c` & `libfsntfs-20240501/tests/fsntfs_test_getopt.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/test_python_module.sh` & `libfsntfs-20240501/tests/test_python_module.sh`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 #!/usr/bin/env bash
 # Tests Python module functions and types.
 #
-# Version: 20231005
+# Version: 20240417
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
+EXIT_NO_TESTS_RAN=5;
 EXIT_IGNORE=77;
 
 TEST_FUNCTIONS="support";
 TEST_FUNCTIONS_WITH_INPUT="attribute file_entry volume";
 OPTION_SETS=("offset");
 
 TEST_TOOL_DIRECTORY=".";
 INPUT_GLOB="*";
 
+LIBRARY_NAME="libfsntfs";
+PYTHON_MODULE="pyfsntfs";
+
 test_python_function()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyfsntfs_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_SCRIPT}";
 	local RESULT=$?;
 
 	return ${RESULT};
 }
 
 test_python_function_with_input()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyfsntfs_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	if ! test -d "input";
 	then
 		echo "Test input directory not found.";
 
 		return ${EXIT_IGNORE};
 	fi
@@ -45,15 +49,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "pyfsntfs");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "${PYTHON_MODULE}");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -120,38 +124,47 @@
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
 
-	if test ${RESULT} -ne ${EXIT_SUCCESS};
+	if test ${RESULT} -eq ${EXIT_NO_TESTS_RAN};
+	then
+		RESULT=${EXIT_IGNORE};
+	fi
+	if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
 	then
 		break;
 	fi
 done
 
 if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
 then
@@ -164,16 +177,19 @@
 	then
 		test_python_function_with_input "${TEST_FUNCTION}";
 		RESULT=$?;
 	else
 		test_python_function "${TEST_FUNCTION}";
 		RESULT=$?;
 	fi
-
-	if test ${RESULT} -ne ${EXIT_SUCCESS};
+	if test ${RESULT} -eq ${EXIT_NO_TESTS_RAN};
+	then
+		RESULT=${EXIT_IGNORE};
+	fi
+	if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
 	then
 		break;
 	fi
 done
 
 exit ${RESULT};
```

### Comparing `libfsntfs-20240119/tests/fsntfs_test_index_node.c` & `libfsntfs-20240501/tests/fsntfs_test_index_node.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_libcnotify.h` & `libfsntfs-20240501/tests/fsntfs_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_tools_bodyfile.c` & `libfsntfs-20240501/tests/fsntfs_test_tools_bodyfile.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_index_value.c` & `libfsntfs-20240501/tests/fsntfs_test_index_value.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_buffer_data_handle.c` & `libfsntfs-20240501/tests/fsntfs_test_buffer_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_libfsntfs.h` & `libfsntfs-20240501/tests/fsntfs_test_libfsntfs.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_libbfio.h` & `libfsntfs-20240501/tests/fsntfs_test_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_memory.c` & `libfsntfs-20240501/tests/fsntfs_test_memory.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_directory_entries_tree.c` & `libfsntfs-20240501/tests/fsntfs_test_directory_entries_tree.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/pyfsntfs_test_attribute.py` & `libfsntfs-20240501/tests/pyfsntfs_test_attribute.py`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/test_runner.sh` & `libfsntfs-20240501/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_index_root_header.c` & `libfsntfs-20240501/tests/fsntfs_test_index_root_header.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/test_fsntfsinfo_bodyfile.sh` & `libfsntfs-20240501/tests/test_fsntfsinfo_bodyfile.sh`

 * *Files 2% similar despite different names*

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
 
 PROFILES=("fsntfsinfo_bodyfile_fs" "fsntfsinfo_bodyfile_mft");
 OPTIONS_PER_PROFILE=("-Bbodyfile -H" "-Bbodyfile -Eall");
@@ -64,20 +64,17 @@
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

### Comparing `libfsntfs-20240119/tests/fsntfs_test_volume_information_attribute.c` & `libfsntfs-20240501/tests/fsntfs_test_volume_information_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_libfcache.h` & `libfsntfs-20240501/tests/fsntfs_test_libfcache.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_cluster_block_stream.c` & `libfsntfs-20240501/tests/fsntfs_test_cluster_block_stream.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_profiler.c` & `libfsntfs-20240501/tests/fsntfs_test_profiler.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_cluster_block_vector.c` & `libfsntfs-20240501/tests/fsntfs_test_cluster_block_vector.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_compression.c` & `libfsntfs-20240501/tests/fsntfs_test_compression.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_mft_entry.c` & `libfsntfs-20240501/tests/fsntfs_test_mft_entry.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_usn_change_journal.c` & `libfsntfs-20240501/tests/fsntfs_test_usn_change_journal.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_compression_unit_descriptor.c` & `libfsntfs-20240501/tests/fsntfs_test_compression_unit_descriptor.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_notify.c` & `libfsntfs-20240501/tests/fsntfs_test_notify.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_file_name_values.c` & `libfsntfs-20240501/tests/fsntfs_test_file_name_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_tools_path_string.c` & `libfsntfs-20240501/tests/fsntfs_test_tools_path_string.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_txf_data_values.c` & `libfsntfs-20240501/tests/fsntfs_test_txf_data_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/pyfsntfs_test_volume.py` & `libfsntfs-20240501/tests/pyfsntfs_test_volume.py`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_compressed_block_data_handle.c` & `libfsntfs-20240501/tests/fsntfs_test_compressed_block_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_libuna.h` & `libfsntfs-20240501/tests/fsntfs_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_volume.c` & `libfsntfs-20240501/tests/fsntfs_test_volume.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_security_descriptor_index_value.c` & `libfsntfs-20240501/tests/fsntfs_test_security_descriptor_index_value.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_volume_name_values.c` & `libfsntfs-20240501/tests/fsntfs_test_volume_name_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_file_entry.c` & `libfsntfs-20240501/tests/fsntfs_test_file_entry.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/test_fsntfsinfo.sh` & `libfsntfs-20240501/tests/test_fsntfsinfo.sh`

 * *Files 6% similar despite different names*

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
 
 PROFILES=("fsntfsinfo" "fsntfsinfo_fs" "fsntfsinfo_mft" "fsntfsinfo_usn");
 OPTIONS_PER_PROFILE=("" "-H" "-Eall" "-U");
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

### Comparing `libfsntfs-20240119/tests/Makefile.in` & `libfsntfs-20240501/tests/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -1381,14 +1381,16 @@
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
@@ -1454,16 +1456,16 @@
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
@@ -2586,16 +2588,18 @@
 	fsntfs_test_unused.h \
 	fsntfs_test_volume_name_values.c
 
 fsntfs_test_volume_name_values_LDADD = \
 	../libfsntfs/libfsntfs.la \
 	@LIBCERROR_LIBADD@
 
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
@@ -3379,24 +3383,108 @@
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
 	-rm -f ../fsntfstools/$(DEPDIR)/$(am__dirstamp)
 	-rm -f ../fsntfstools/$(am__dirstamp)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ../fsntfstools/$(DEPDIR)/bodyfile.Po
+	-rm -f ../fsntfstools/$(DEPDIR)/digest_hash.Po
+	-rm -f ../fsntfstools/$(DEPDIR)/fsntfstools_output.Po
+	-rm -f ../fsntfstools/$(DEPDIR)/fsntfstools_signal.Po
+	-rm -f ../fsntfstools/$(DEPDIR)/info_handle.Po
+	-rm -f ../fsntfstools/$(DEPDIR)/mount_path_string.Po
+	-rm -f ../fsntfstools/$(DEPDIR)/path_string.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_attribute.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_attribute_list_entry.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_bitmap_values.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_buffer_data_handle.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_cluster_block.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_cluster_block_data.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_cluster_block_stream.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_cluster_block_vector.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_compressed_block.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_compressed_block_data_handle.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_compressed_block_vector.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_compressed_data_handle.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_compression.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_compression_unit_data_handle.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_compression_unit_descriptor.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_data_run.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_data_stream.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_directory_entries_tree.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_directory_entry.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_error.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_extent.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_file_entry.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_file_name_attribute.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_file_name_values.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_file_system.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_fixup_values.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_functions.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_getopt.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_index.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_index_entry.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_index_entry_header.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_index_entry_vector.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_index_node.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_index_node_header.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_index_root_header.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_index_value.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_io_handle.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_logged_utility_stream_values.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_memory.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_mft.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_mft_attribute.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_mft_attribute_list.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_mft_attribute_list_entry.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_mft_entry.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_mft_entry_header.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_mft_metadata_file.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_name.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_notify.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_object_identifier_values.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_path_hint.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_profiler.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_reparse_point_attribute.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_reparse_point_values.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_rwlock.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_sds_index_value.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_security_descriptor_index.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_security_descriptor_index_value.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_security_descriptor_values.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_standard_information_values.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_support.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_tools_bodyfile.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_tools_digest_hash.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_tools_info_handle.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_tools_mount_path_string.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_tools_output.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_tools_path_string.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_tools_signal.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_txf_data_values.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_usn_change_journal.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_volume.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_volume_header.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_volume_information_attribute.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_volume_information_values.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_volume_name_attribute.Po
+	-rm -f ./$(DEPDIR)/fsntfs_test_volume_name_values.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -3561,13 +3649,10 @@
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

### Comparing `libfsntfs-20240119/tests/fsntfs_test_libcdata.h` & `libfsntfs-20240501/tests/fsntfs_test_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_data_stream.c` & `libfsntfs-20240501/tests/fsntfs_test_data_stream.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/pyfsntfs_test_support.py` & `libfsntfs-20240501/tests/pyfsntfs_test_support.py`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_mft_metadata_file.c` & `libfsntfs-20240501/tests/fsntfs_test_mft_metadata_file.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_mft_attribute_list.c` & `libfsntfs-20240501/tests/fsntfs_test_mft_attribute_list.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_name.c` & `libfsntfs-20240501/tests/fsntfs_test_name.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_reparse_point_attribute.c` & `libfsntfs-20240501/tests/fsntfs_test_reparse_point_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_object_identifier_values.c` & `libfsntfs-20240501/tests/fsntfs_test_object_identifier_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_tools_info_handle.c` & `libfsntfs-20240501/tests/fsntfs_test_tools_info_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_data_run.c` & `libfsntfs-20240501/tests/fsntfs_test_data_run.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_bitmap_values.c` & `libfsntfs-20240501/tests/fsntfs_test_bitmap_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_index_entry_header.c` & `libfsntfs-20240501/tests/fsntfs_test_index_entry_header.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_unused.h` & `libfsntfs-20240501/tests/fsntfs_test_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/fsntfs_test_libclocale.h` & `libfsntfs-20240501/tests/fsntfs_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/tests/test_library.sh` & `libfsntfs-20240501/tests/test_library.sh`

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
 
 LIBRARY_TESTS="attribute attribute_list_entry bitmap_values buffer_data_handle cluster_block cluster_block_data cluster_block_stream cluster_block_vector compressed_block compressed_block_data_handle compressed_block_vector compressed_data_handle compression compression_unit_data_handle compression_unit_descriptor data_run data_stream directory_entries_tree directory_entry error extent file_entry file_name_attribute file_name_values file_system fixup_values index index_entry index_entry_header index_entry_vector index_node index_node_header index_root_header index_value io_handle logged_utility_stream_values mft mft_attribute mft_attribute_list mft_attribute_list_entry mft_entry mft_entry_header name notify object_identifier_values path_hint profiler reparse_point_attribute reparse_point_values sds_index_value security_descriptor_index security_descriptor_index_value security_descriptor_values standard_information_values txf_data_values usn_change_journal volume_header volume_information_attribute volume_information_values volume_name_attribute volume_name_values";
 LIBRARY_TESTS_WITH_INPUT="mft_metadata_file support volume";
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

### Comparing `libfsntfs-20240119/ossfuzz/volume_fuzzer.cc` & `libfsntfs-20240501/ossfuzz/volume_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/ossfuzz/Makefile.am` & `libfsntfs-20240501/ossfuzz/Makefile.am`

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
 	../libfsntfs/libfsntfs.la \
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
 	@echo "Running splint on file_entry_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(file_entry_fuzzer_SOURCES)
 	@echo "Running splint on mft_metadata_file_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(mft_metadata_file_fuzzer_SOURCES)
 	@echo "Running splint on volume_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(volume_fuzzer_SOURCES)
```

### Comparing `libfsntfs-20240119/ossfuzz/mft_metadata_file_fuzzer.cc` & `libfsntfs-20240501/ossfuzz/mft_metadata_file_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/ossfuzz/ossfuzz_libfsntfs.h` & `libfsntfs-20240501/ossfuzz/ossfuzz_libfsntfs.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/ossfuzz/ossfuzz_libbfio.h` & `libfsntfs-20240501/ossfuzz/ossfuzz_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/ossfuzz/file_entry_fuzzer.cc` & `libfsntfs-20240501/ossfuzz/file_entry_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/ossfuzz/Makefile.in` & `libfsntfs-20240501/ossfuzz/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -513,14 +513,16 @@
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
@@ -585,16 +587,16 @@
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
@@ -650,15 +652,16 @@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libfsntfs/libfsntfs.la \
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
@@ -910,23 +913,28 @@
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
+		-rm -f ./$(DEPDIR)/file_entry_fuzzer.Po
+	-rm -f ./$(DEPDIR)/mft_metadata_file_fuzzer.Po
+	-rm -f ./$(DEPDIR)/volume_fuzzer.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1012,17 +1020,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on file_entry_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(file_entry_fuzzer_SOURCES)
 	@echo "Running splint on mft_metadata_file_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(mft_metadata_file_fuzzer_SOURCES)
 	@echo "Running splint on volume_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(volume_fuzzer_SOURCES)
```

### Comparing `libfsntfs-20240119/libfusn/libfusn_support.c` & `libfsntfs-20240501/libfusn/libfusn_support.c`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfusn/libfusn_debug.h` & `libfsntfs-20240501/libfusn/libfusn_debug.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Debug functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfusn/libfusn_record.c` & `libfsntfs-20240501/libfusn/libfusn_record.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Record functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfusn/libfusn_types.h` & `libfsntfs-20240501/libfusn/libfusn_types.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfusn/libfusn_libcnotify.h` & `libfsntfs-20240501/libfusn/libfusn_libcnotify.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcnotify header
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfusn/libfusn_unused.h` & `libfsntfs-20240501/libfusn/libfusn_unused.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfusn/Makefile.am` & `libfsntfs-20240501/libfusn/Makefile.am`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFUSN
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBFDATETIME_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfusn.la
 
@@ -21,17 +21,17 @@
 	libfusn_libuna.h \
 	libfusn_record.c libfusn_record.h \
 	libfusn_support.c libfusn_support.h \
 	libfusn_types.h \
 	libfusn_unused.h
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
 	@echo "Running splint on libfusn ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfusn_la_SOURCES)
```

### Comparing `libfsntfs-20240119/libfusn/libfusn_libcerror.h` & `libfsntfs-20240501/libfusn/libfusn_libcerror.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfusn/libfusn_error.c` & `libfsntfs-20240501/libfusn/libfusn_error.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfusn/libfusn_libuna.h` & `libfsntfs-20240501/libfusn/libfusn_libuna.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libuna header wrapper
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfusn/fusn_record.h` & `libfsntfs-20240501/libfusn/fusn_record.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The Update Sequence Number (USN) Journal record definition
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfusn/libfusn_support.h` & `libfsntfs-20240501/libfusn/libfusn_support.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfusn/libfusn_debug.c` & `libfsntfs-20240501/libfusn/libfusn_debug.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Debug functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfusn/Makefile.in` & `libfsntfs-20240501/libfusn/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -477,14 +477,16 @@
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
@@ -549,16 +551,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFUSN_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFUSN_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFUSN_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFUSN_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFUSN_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFUSN_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFUSN_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFUSN_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFUSN_TRUE@	@LIBFDATETIME_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFUSN_TRUE@noinst_LTLIBRARIES = libfusn.la
 @HAVE_LOCAL_LIBFUSN_TRUE@libfusn_la_SOURCES = \
@@ -572,15 +574,16 @@
 @HAVE_LOCAL_LIBFUSN_TRUE@	libfusn_libfdatetime.h \
 @HAVE_LOCAL_LIBFUSN_TRUE@	libfusn_libuna.h \
 @HAVE_LOCAL_LIBFUSN_TRUE@	libfusn_record.c libfusn_record.h \
 @HAVE_LOCAL_LIBFUSN_TRUE@	libfusn_support.c libfusn_support.h \
 @HAVE_LOCAL_LIBFUSN_TRUE@	libfusn_types.h \
 @HAVE_LOCAL_LIBFUSN_TRUE@	libfusn_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -783,24 +786,30 @@
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
+		-rm -f ./$(DEPDIR)/libfusn_debug.Plo
+	-rm -f ./$(DEPDIR)/libfusn_error.Plo
+	-rm -f ./$(DEPDIR)/libfusn_record.Plo
+	-rm -f ./$(DEPDIR)/libfusn_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -861,14 +870,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -879,23 +890,22 @@
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
 	@echo "Running splint on libfusn ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfusn_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfsntfs-20240119/libfusn/libfusn_extern.h` & `libfsntfs-20240501/libfusn/libfusn_extern.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfusn/libfusn_definitions.h` & `libfsntfs-20240501/libfusn/libfusn_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfusn/definitions.h> are copied here
  * for local use of libfusn
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFUSN_VERSION						20220119
+#define LIBFUSN_VERSION						20240416
 
 /* The version string
  */
-#define LIBFUSN_VERSION_STRING					"20220119"
+#define LIBFUSN_VERSION_STRING					"20240416"
 
 /* The byte order definitions
  */
 #define LIBFUSN_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define LIBFUSN_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The update reason flags
```

### Comparing `libfsntfs-20240119/libfusn/libfusn_record.h` & `libfsntfs-20240501/libfusn/libfusn_record.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Record functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfusn/libfusn_libfdatetime.h` & `libfsntfs-20240501/libfusn/libfusn_libfdatetime.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libfdatetime header wrapper
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfusn/libfusn_error.h` & `libfsntfs-20240501/libfusn/libfusn_error.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2011-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/ltmain.sh` & `libfsntfs-20240501/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_locale_identifier.h` & `libfsntfs-20240501/libfwnt/libfwnt_locale_identifier.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Locale identifier (LCID) functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_lzxpress.c` & `libfsntfs-20240501/libfwnt/libfwnt_lzxpress.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * LZXPRESS (de)compression functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_extern.h` & `libfsntfs-20240501/libfwnt/libfwnt_extern.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_security_identifier.c` & `libfsntfs-20240501/libfwnt/libfwnt_security_identifier.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows NT Security Identifier (SID) functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_libcerror.h` & `libfsntfs-20240501/libfwnt/libfwnt_libcerror.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_bit_stream.c` & `libfsntfs-20240501/libfwnt/libfwnt_bit_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Bit-stream functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_error.h` & `libfsntfs-20240501/libfwnt/libfwnt_error.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_lznt1.h` & `libfsntfs-20240501/libfwnt/libfwnt_lznt1.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * LZNT1 (de)compression functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_notify.c` & `libfsntfs-20240501/libfwnt/libfwnt_notify.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Notification functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/Makefile.am` & `libfsntfs-20240501/libfwnt/Makefile.am`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFWNT
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfwnt.la
@@ -30,19 +30,17 @@
 	libfwnt_security_descriptor.c libfwnt_security_descriptor.h \
 	libfwnt_security_identifier.c libfwnt_security_identifier.h \
 	libfwnt_support.c libfwnt_support.h \
 	libfwnt_types.h \
 	libfwnt_unused.h
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
 	@echo "Running splint on libfwnt ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfwnt_la_SOURCES)
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_security_identifier.h` & `libfsntfs-20240501/libfwnt/libfwnt_security_identifier.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows NT Security Identifier (SID) functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_support.h` & `libfsntfs-20240501/libfwnt/libfwnt_support.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_huffman_tree.h` & `libfsntfs-20240501/libfwnt/libfwnt_huffman_tree.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Huffman tree functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_error.c` & `libfsntfs-20240501/libfwnt/libfwnt_error.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_access_control_list.h` & `libfsntfs-20240501/libfwnt/libfwnt_access_control_list.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows NT Access Contol List (ACL) functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_security_descriptor.c` & `libfsntfs-20240501/libfwnt/libfwnt_security_descriptor.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows NT Security Descriptor functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_access_control_list.c` & `libfsntfs-20240501/libfwnt/libfwnt_access_control_list.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows NT Access Control List (ACL) functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_definitions.h` & `libfsntfs-20240501/libfwnt/libfwnt_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfwnt/definitions.h> are copied here
  * for local use of libfwnt
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFWNT_VERSION					20231124
+#define LIBFWNT_VERSION					20240415
 
 /* The version string
  */
-#define LIBFWNT_VERSION_STRING				"20231124"
+#define LIBFWNT_VERSION_STRING				"20240415"
 
 
 /* The endian definitions
  */
 #define LIBFWNT_ENDIAN_BIG				_BYTE_STREAM_ENDIAN_BIG
 #define LIBFWNT_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_huffman_tree.c` & `libfsntfs-20240501/libfwnt/libfwnt_huffman_tree.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Huffman tree functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_debug.c` & `libfsntfs-20240501/libfwnt/libfwnt_debug.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Debug functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_lznt1.c` & `libfsntfs-20240501/libfwnt/libfwnt_lznt1.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * LZNT1 (de)compression functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_notify.h` & `libfsntfs-20240501/libfwnt/libfwnt_notify.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Notification functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_locale_identifier.c` & `libfsntfs-20240501/libfwnt/libfwnt_locale_identifier.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Locale identifier (LCID) functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_debug.h` & `libfsntfs-20240501/libfwnt/libfwnt_debug.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Debug functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_libcdata.h` & `libfsntfs-20240501/libfwnt/libfwnt_libcdata.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcdata header wrapper
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_lzx.h` & `libfsntfs-20240501/libfwnt/libfwnt_lzx.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * LZX (un)compression functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_unused.h` & `libfsntfs-20240501/libfwnt/libfwnt_unused.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_libcnotify.h` & `libfsntfs-20240501/libfwnt/libfwnt_libcnotify.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcnotify header wrapper
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_access_control_entry.c` & `libfsntfs-20240501/libfwnt/libfwnt_access_control_entry.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows NT Access Control Entry (ACE) functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_lzxpress.h` & `libfsntfs-20240501/libfwnt/libfwnt_lzxpress.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * LZXPRESS (de)compression functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_security_descriptor.h` & `libfsntfs-20240501/libfwnt/libfwnt_security_descriptor.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows NT Security Descriptor functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_lzx.c` & `libfsntfs-20240501/libfwnt/libfwnt_lzx.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * LZX (un)compression functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/Makefile.in` & `libfsntfs-20240501/libfwnt/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -503,14 +503,16 @@
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
@@ -575,16 +577,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFWNT_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFWNT_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFWNT_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFWNT_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFWNT_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFWNT_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWNT_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWNT_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWNT_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFWNT_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFWNT_TRUE@noinst_LTLIBRARIES = libfwnt.la
@@ -607,15 +609,16 @@
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_notify.c libfwnt_notify.h \
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_security_descriptor.c libfwnt_security_descriptor.h \
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_security_identifier.c libfwnt_security_identifier.h \
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_support.c libfwnt_support.h \
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_types.h \
 @HAVE_LOCAL_LIBFWNT_TRUE@	libfwnt_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -828,24 +831,40 @@
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
+		-rm -f ./$(DEPDIR)/libfwnt_access_control_entry.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_access_control_list.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_bit_stream.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_debug.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_error.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_huffman_tree.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_locale_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_lznt1.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_lzx.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_lzxpress.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_notify.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_security_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_security_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfwnt_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -942,17 +961,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfwnt ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfwnt_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_bit_stream.h` & `libfsntfs-20240501/libfwnt/libfwnt_bit_stream.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Bit-stream functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_types.h` & `libfsntfs-20240501/libfwnt/libfwnt_types.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_support.c` & `libfsntfs-20240501/libfwnt/libfwnt_support.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfwnt/libfwnt_access_control_entry.h` & `libfsntfs-20240501/libfwnt/libfwnt_access_control_entry.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows NT Access Contol Entry (ACE) functions
  *
- * Copyright (C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_index_entry_header.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_index_entry_header.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_libfguid.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_mft.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_mft.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_compressed_block_data_handle.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_compressed_block_data_handle.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_sds_index_value.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_sds_index_value.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_directory_entries_tree.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_directory_entries_tree.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_security_descriptor_index.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_security_descriptor_index.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_txf_data_values.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_txf_data_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_security_descriptor_values.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_security_descriptor_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_reparse_point_values.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_reparse_point_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_compressed_block.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_compressed_block.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_compressed_block.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_compressed_block.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_index_entry.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_index_entry.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_compression.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_compression.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_profiler.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_profiler.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_standard_information_attribute.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_standard_information_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_libfcache.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_libfcache.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/fsntfs_mft_entry.h` & `libfsntfs-20240501/libfsntfs/fsntfs_mft_entry.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_index_value.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_index_value.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_volume_information_attribute.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_volume_information_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_cluster_block_stream.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_cluster_block_stream.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/fsntfs_volume_information.h` & `libfsntfs-20240501/libfsntfs/fsntfs_volume_information.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_object_identifier_values.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_object_identifier_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_io_handle.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_io_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_data_run.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_data_run.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_attribute_list_entry.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_attribute_list_entry.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_libcnotify.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_index.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_index.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_standard_information_attribute.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_standard_information_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_libbfio.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_security_descriptor_index_value.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_security_descriptor_index_value.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_reparse_point_attribute.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_reparse_point_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_mft_metadata_file.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_mft_metadata_file.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_mft_entry_header.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_mft_entry_header.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/fsntfs_txf_data.h` & `libfsntfs-20240501/libfsntfs/fsntfs_txf_data.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_standard_information_values.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_standard_information_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_cluster_block_vector.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_cluster_block_vector.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_attribute_list_attribute.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_attribute_list_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_volume_name_attribute.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_volume_name_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_cluster_block_stream.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_cluster_block_stream.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_volume_header.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_volume_header.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_attribute_list_attribute.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_attribute_list_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_compressed_data_handle.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_compressed_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_index_node_header.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_index_node_header.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/fsntfs_logged_utility_stream.h` & `libfsntfs-20240501/libfsntfs/fsntfs_logged_utility_stream.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_mft_attribute_list_entry.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_mft_attribute_list_entry.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_object_identifier_attribute.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_object_identifier_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_logged_utility_stream_values.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_logged_utility_stream_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_bitmap_values.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_bitmap_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_notify.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_notify.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_volume.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_volume.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_support.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_cluster_block.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_cluster_block.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_object_identifier_attribute.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_object_identifier_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_index_root_header.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_index_root_header.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_types.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_index_node_header.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_index_node_header.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_libclocale.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/fsntfs_mft_attribute.h` & `libfsntfs-20240501/libfsntfs/fsntfs_mft_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_index_node.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_index_node.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/Makefile.am` & `libfsntfs-20240501/libfsntfs/Makefile.am`

 * *Files 2% similar despite different names*

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
@@ -143,21 +143,19 @@
 libfsntfs_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libfsntfs_definitions.h.in \
 	libfsntfs.rc \
 	libfsntfs.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfsntfs_definitions.h \
+	libfsntfs.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libfsntfs_definitions.h
-	-rm -f libfsntfs.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfsntfs ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfsntfs_la_SOURCES)
```

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_definitions.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -35,19 +35,19 @@
 #if !defined( HAVE_LOCAL_LIBFSNTFS )
 #include <libfsntfs/definitions.h>
 
 /* The definitions in <libfsntfs/definitions.h> are copied here
  * for local use of libfsntfs
  */
 #else
-#define LIBFSNTFS_VERSION						20240119
+#define LIBFSNTFS_VERSION						20240501
 
 /* The version string
  */
-#define LIBFSNTFS_VERSION_STRING					"20240119"
+#define LIBFSNTFS_VERSION_STRING					"20240501"
 
 /* The file access
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBFSNTFS_ACCESS_FLAGS
```

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_file_name_values.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_file_name_values.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/fsntfs_object_identifier.h` & `libfsntfs-20240501/libfsntfs/fsntfs_object_identifier.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_txf_data_values.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_txf_data_values.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_debug.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_debug.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_libcthreads.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_cluster_block.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_cluster_block.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/fsntfs_mft_attribute_list.h` & `libfsntfs-20240501/libfsntfs/fsntfs_mft_attribute_list.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_volume_information_values.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_volume_information_values.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_attribute.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_file_system.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_file_system.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_compression_unit_descriptor.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_compression_unit_descriptor.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_attribute.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_usn_change_journal.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_usn_change_journal.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_mft.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_mft.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_debug.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_debug.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_security_descriptor_values.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_security_descriptor_values.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_volume_name_attribute.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_volume_name_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/fsntfs_standard_information.h` & `libfsntfs-20240501/libfsntfs/fsntfs_standard_information.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_mft_attribute_list_entry.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_mft_attribute_list_entry.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_file_name_values.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_file_name_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_index_root_header.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_index_root_header.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_libcerror.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_support.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_mft_attribute.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_mft_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_extent.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_extent.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_mft_attribute.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_mft_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_volume_information_attribute.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_volume_information_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_usn_change_journal.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_usn_change_journal.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_compressed_block_data_handle.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_compressed_block_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_libcdata.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_directory_entry.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_directory_entry.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_compression_unit_descriptor.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_compression_unit_descriptor.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/fsntfs_volume_header.h` & `libfsntfs-20240501/libfsntfs/fsntfs_volume_header.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_security_descriptor_index.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_security_descriptor_index.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_standard_information_values.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_standard_information_values.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_file_entry.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_file_entry.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_file_system.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_file_system.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_name.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_name.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_sds_index_value.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_sds_index_value.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_fixup_values.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_fixup_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs.rc` & `libfsntfs-20240501/libfsntfs/libfsntfs.rc`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the Windows New Technology File System (NTFS) format\0"
-      VALUE "FileVersion",		"20240119" "\0"
+      VALUE "FileVersion",		"20240501" "\0"
       VALUE "InternalName",		"libfsntfs.dll\0"
       VALUE "LegalCopyright",		"(C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libfsntfs.dll\0"
       VALUE "ProductName",		"libfsntfs\0"
-      VALUE "ProductVersion",		"20240119" "\0"
+      VALUE "ProductVersion",		"20240501" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libfsntfs/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_index_node.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_index_node.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_fixup_values.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_fixup_values.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs.rc.in` & `libfsntfs-20240501/libfsntfs/libfsntfs.rc.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_libuna.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_libuna.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs.c` & `libfsntfs-20240501/libfsntfs/libfsntfs.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_cluster_block_data.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_cluster_block_data.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_mft_entry.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_mft_entry.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/fsntfs_secure.h` & `libfsntfs-20240501/libfsntfs/fsntfs_secure.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_index_entry_vector.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_index_entry_vector.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_cluster_block_vector.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_cluster_block_vector.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_notify.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_notify.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_security_descriptor_index_value.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_security_descriptor_index_value.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_buffer_data_handle.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_buffer_data_handle.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_volume_name_values.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_volume_name_values.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_extent.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_extent.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_extern.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_mft_attribute_list.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_mft_attribute_list.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_compressed_block_vector.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_compressed_block_vector.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_index.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_index.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_buffer_data_handle.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_buffer_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_libfwnt.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_reparse_point_attribute.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_reparse_point_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_path_hint.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_path_hint.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/fsntfs_reparse_point.h` & `libfsntfs-20240501/libfsntfs/fsntfs_reparse_point.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_logged_utility_stream_values.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_logged_utility_stream_values.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_data_stream.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_data_stream.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_volume_information_values.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_volume_information_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_error.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_file_name_attribute.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_file_name_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/fsntfs_index.h` & `libfsntfs-20240501/libfsntfs/fsntfs_index.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_index_entry.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_index_entry.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_libfdata.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_libfdata.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_index_value.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_index_value.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_error.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_io_handle.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_io_handle.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_object_identifier_values.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_object_identifier_values.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_compressed_data_handle.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_compressed_data_handle.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_mft_metadata_file.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_mft_metadata_file.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_libfdatetime.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_bitmap_values.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_bitmap_values.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_file_entry.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_file_entry.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_directory_entry.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_directory_entry.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_cluster_block_data.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_cluster_block_data.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_compression_unit_data_handle.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_compression_unit_data_handle.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_mft_attribute_list.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_mft_attribute_list.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_security_descriptor_attribute.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_security_descriptor_attribute.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_definitions.h.in` & `libfsntfs-20240501/libfsntfs/libfsntfs_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_compressed_block_vector.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_compressed_block_vector.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_name.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_name.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_file_name_attribute.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_file_name_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/Makefile.in` & `libfsntfs-20240501/libfsntfs/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -611,14 +611,16 @@
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
@@ -683,16 +685,16 @@
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
@@ -829,15 +831,18 @@
 
 libfsntfs_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libfsntfs_definitions.h.in \
 	libfsntfs.rc \
 	libfsntfs.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfsntfs_definitions.h \
+	libfsntfs.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -1137,24 +1142,96 @@
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
+		-rm -f ./$(DEPDIR)/libfsntfs.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_attribute.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_attribute_list_attribute.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_attribute_list_entry.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_bitmap_values.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_buffer_data_handle.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_cluster_block.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_cluster_block_data.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_cluster_block_stream.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_cluster_block_vector.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_compressed_block.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_compressed_block_data_handle.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_compressed_block_vector.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_compressed_data_handle.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_compression.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_compression_unit_data_handle.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_compression_unit_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_data_run.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_data_stream.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_debug.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_directory_entries_tree.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_directory_entry.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_error.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_extent.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_file_entry.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_file_name_attribute.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_file_name_values.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_file_system.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_fixup_values.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_index.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_index_entry.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_index_entry_header.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_index_entry_vector.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_index_node.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_index_node_header.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_index_root_header.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_index_value.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_logged_utility_stream_values.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_mft.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_mft_attribute.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_mft_attribute_list.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_mft_attribute_list_entry.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_mft_entry.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_mft_entry_header.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_mft_metadata_file.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_name.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_notify.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_object_identifier_attribute.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_object_identifier_values.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_path_hint.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_profiler.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_reparse_point_attribute.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_reparse_point_values.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_sds_index_value.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_security_descriptor_attribute.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_security_descriptor_index.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_security_descriptor_index_value.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_security_descriptor_values.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_standard_information_attribute.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_standard_information_values.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_support.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_txf_data_values.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_usn_change_journal.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_volume.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_volume_header.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_volume_information_attribute.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_volume_information_values.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_volume_name_attribute.Plo
+	-rm -f ./$(DEPDIR)/libfsntfs_volume_name_values.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1307,19 +1384,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libfsntfs_definitions.h
-	-rm -f libfsntfs.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfsntfs ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfsntfs_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_volume.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_volume.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_data_stream.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_data_stream.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_mft_entry_header.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_mft_entry_header.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_volume_name_values.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_volume_name_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_reparse_point_values.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_reparse_point_values.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_directory_entries_tree.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_directory_entries_tree.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_compression.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_compression.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_mft_entry.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_mft_entry.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_data_run.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_data_run.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_path_hint.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_path_hint.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_index_entry_header.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_index_entry_header.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_index_entry_vector.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_index_entry_vector.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_security_descriptor_attribute.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_security_descriptor_attribute.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_profiler.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_profiler.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_attribute_list_entry.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_attribute_list_entry.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/fsntfs_file_name.h` & `libfsntfs-20240501/libfsntfs/fsntfs_file_name.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_compression_unit_data_handle.c` & `libfsntfs-20240501/libfsntfs/libfsntfs_compression_unit_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_volume_header.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_volume_header.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs/libfsntfs_unused.h` & `libfsntfs-20240501/libfsntfs/libfsntfs_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libhmac/libhmac_sha1_context.c` & `libfsntfs-20240501/libhmac/libhmac_sha1_context.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA1 context functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libhmac/libhmac_sha224.h` & `libfsntfs-20240501/libhmac/libhmac_sha224.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-224 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libhmac/libhmac_sha512_context.c` & `libfsntfs-20240501/libhmac/libhmac_sha512_context.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-512 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libhmac/libhmac_extern.h` & `libfsntfs-20240501/libhmac/libhmac_extern.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libhmac/libhmac_md5.c` & `libfsntfs-20240501/libhmac/libhmac_md5.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MD5 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libhmac/libhmac_md5.h` & `libfsntfs-20240501/libhmac/libhmac_md5.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MD5 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libhmac/libhmac_error.h` & `libfsntfs-20240501/libhmac/libhmac_error.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libhmac/libhmac_types.h` & `libfsntfs-20240501/libhmac/libhmac_types.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libhmac/libhmac_byte_stream.h` & `libfsntfs-20240501/libhmac/libhmac_byte_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Byte stream functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libhmac/libhmac_sha512.c` & `libfsntfs-20240501/libhmac/libhmac_sha512.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-512 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libhmac/libhmac_sha256_context.c` & `libfsntfs-20240501/libhmac/libhmac_sha256_context.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-256 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libhmac/libhmac_sha224.c` & `libfsntfs-20240501/libhmac/libhmac_sha224.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-224 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libhmac/libhmac_definitions.h` & `libfsntfs-20240501/libhmac/libhmac_definitions.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -30,19 +30,19 @@
 #if !defined( HAVE_LOCAL_LIBHMAC )
 #include <libhmac/definitions.h>
 
 /* The definitions in <libhmac/definitions.h> are copied here
  * for local use of libhmac
  */
 #else
-#define LIBHMAC_VERSION			20231127
+#define LIBHMAC_VERSION			20240417
 
 /* The libhmac version string
  */
-#define LIBHMAC_VERSION_STRING		"20231127"
+#define LIBHMAC_VERSION_STRING		"20240417"
 
 /* The digest hash sizes
  */
 #define LIBHMAC_MD5_HASH_SIZE		16
 #define LIBHMAC_SHA1_HASH_SIZE		20
 #define LIBHMAC_SHA224_HASH_SIZE	28
 #define LIBHMAC_SHA256_HASH_SIZE	32
```

### Comparing `libfsntfs-20240119/libhmac/libhmac_unused.h` & `libfsntfs-20240501/libhmac/libhmac_unused.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libhmac/libhmac_sha1.h` & `libfsntfs-20240501/libhmac/libhmac_sha1.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA1 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libhmac/libhmac_sha256_context.h` & `libfsntfs-20240501/libhmac/libhmac_sha256_context.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-256 context functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libhmac/Makefile.am` & `libfsntfs-20240501/libhmac/Makefile.am`

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

### Comparing `libfsntfs-20240119/libhmac/libhmac_sha224_context.c` & `libfsntfs-20240501/libhmac/libhmac_sha224_context.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-224 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libhmac/libhmac_md5_context.h` & `libfsntfs-20240501/libhmac/libhmac_md5_context.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MD5 context functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libhmac/libhmac_sha256.c` & `libfsntfs-20240501/libhmac/libhmac_sha256.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-256 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libhmac/libhmac_sha1_context.h` & `libfsntfs-20240501/libhmac/libhmac_sha1_context.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA1 context functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libhmac/libhmac_libcerror.h` & `libfsntfs-20240501/libcsplit/libcsplit_libcerror.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBHMAC_LIBCERROR_H )
-#define _LIBHMAC_LIBCERROR_H
+#if !defined( _LIBCSPLIT_LIBCERROR_H )
+#define _LIBCSPLIT_LIBCERROR_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCERROR for local use of libcerror
  */
 #if defined( HAVE_LOCAL_LIBCERROR )
 
@@ -42,9 +42,9 @@
 #define LIBCERROR_DLL_IMPORT
 #endif
 
 #include <libcerror.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCERROR ) */
 
-#endif /* !defined( _LIBHMAC_LIBCERROR_H ) */
+#endif /* !defined( _LIBCSPLIT_LIBCERROR_H ) */
```

### Comparing `libfsntfs-20240119/libhmac/libhmac_error.c` & `libfsntfs-20240501/libhmac/libhmac_error.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libhmac/libhmac_support.h` & `libfsntfs-20240501/libhmac/libhmac_support.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libhmac/Makefile.in` & `libfsntfs-20240501/libhmac/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -500,14 +500,16 @@
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
@@ -572,16 +574,16 @@
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
@@ -599,15 +601,16 @@
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
@@ -818,24 +821,38 @@
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
 
@@ -930,17 +947,14 @@
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

### Comparing `libfsntfs-20240119/libhmac/libhmac_sha256.h` & `libfsntfs-20240501/libhmac/libhmac_sha256.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-256 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libhmac/libhmac_sha224_context.h` & `libfsntfs-20240501/libhmac/libhmac_sha224_context.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-224 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libhmac/libhmac_sha512_context.h` & `libfsntfs-20240501/libhmac/libhmac_sha512_context.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-512 context functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libhmac/libhmac_sha512.h` & `libfsntfs-20240501/libhmac/libhmac_sha512.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-512 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libhmac/libhmac_support.c` & `libfsntfs-20240501/libuna/libuna_support.c`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -18,22 +18,22 @@
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include <common.h>
 #include <types.h>
 
-#include "libhmac_definitions.h"
-#include "libhmac_support.h"
+#include "libuna_definitions.h"
+#include "libuna_support.h"
 
-#if !defined( HAVE_LOCAL_LIBHMAC )
+#if !defined( HAVE_LOCAL_LIBUNA )
 
 /* Returns the library version as a string
  */
-const char *libhmac_get_version(
+const char *libuna_get_version(
              void )
 {
-	return( (const char *) LIBHMAC_VERSION_STRING );
+	return( (const char *) LIBUNA_VERSION_STRING );
 }
 
-#endif
+#endif /* !defined( HAVE_LOCAL_LIBUNA ) */
```

### Comparing `libfsntfs-20240119/libhmac/libhmac_sha1.c` & `libfsntfs-20240501/libhmac/libhmac_sha1.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA1 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libhmac/libhmac_md5_context.c` & `libfsntfs-20240501/libhmac/libhmac_md5_context.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MD5 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libcsplit/libcsplit_narrow_string.c` & `libfsntfs-20240501/libcsplit/libcsplit_narrow_string.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcsplit/libcsplit_definitions.h` & `libfsntfs-20240501/libcsplit/libcsplit_definitions.h`

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

### Comparing `libfsntfs-20240119/libcsplit/libcsplit_types.h` & `libfsntfs-20240501/libcsplit/libcsplit_types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcsplit/libcsplit_wide_split_string.c` & `libfsntfs-20240501/libcsplit/libcsplit_wide_split_string.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcsplit/libcsplit_support.h` & `libfsntfs-20240501/libcsplit/libcsplit_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcsplit/Makefile.am` & `libfsntfs-20240501/libcsplit/Makefile.am`

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

### Comparing `libfsntfs-20240119/libcsplit/libcsplit_libcerror.h` & `libfsntfs-20240501/libuna/libuna_libcerror.h`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBCSPLIT_LIBCERROR_H )
-#define _LIBCSPLIT_LIBCERROR_H
+#if !defined( _LIBUNA_LIBCERROR_H )
+#define _LIBUNA_LIBCERROR_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCERROR for local use of libcerror
  */
 #if defined( HAVE_LOCAL_LIBCERROR )
 
@@ -42,9 +42,9 @@
 #define LIBCERROR_DLL_IMPORT
 #endif
 
 #include <libcerror.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCERROR ) */
 
-#endif /* !defined( _LIBCSPLIT_LIBCERROR_H ) */
+#endif /* !defined( _LIBUNA_LIBCERROR_H ) */
```

### Comparing `libfsntfs-20240119/libcsplit/libcsplit_wide_string.c` & `libfsntfs-20240501/libcsplit/libcsplit_wide_string.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcsplit/libcsplit_unused.h` & `libfsntfs-20240501/libcsplit/libcsplit_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcsplit/libcsplit_wide_split_string.h` & `libfsntfs-20240501/libcsplit/libcsplit_wide_split_string.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcsplit/libcsplit_error.c` & `libfsntfs-20240501/libcsplit/libcsplit_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcsplit/libcsplit_narrow_split_string.c` & `libfsntfs-20240501/libcsplit/libcsplit_narrow_split_string.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcsplit/libcsplit_extern.h` & `libfsntfs-20240501/libcsplit/libcsplit_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcsplit/libcsplit_error.h` & `libfsntfs-20240501/libcsplit/libcsplit_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcsplit/libcsplit_support.c` & `libfsntfs-20240501/libcsplit/libcsplit_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcsplit/libcsplit_wide_string.h` & `libfsntfs-20240501/libcsplit/libcsplit_wide_string.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcsplit/Makefile.in` & `libfsntfs-20240501/libcsplit/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -487,14 +487,16 @@
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
@@ -559,16 +561,16 @@
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
@@ -577,15 +579,16 @@
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
@@ -790,24 +793,32 @@
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
 
@@ -896,17 +907,14 @@
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

### Comparing `libfsntfs-20240119/libcsplit/libcsplit_narrow_split_string.h` & `libfsntfs-20240501/libcsplit/libcsplit_narrow_split_string.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcsplit/libcsplit_narrow_string.h` & `libfsntfs-20240501/libcsplit/libcsplit_narrow_string.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/po/remove-potcdate.sin` & `libfsntfs-20240501/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/po/Makefile.in.in` & `libfsntfs-20240501/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/po/en@quot.header` & `libfsntfs-20240501/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/po/en@boldquot.header` & `libfsntfs-20240501/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/po/insert-header.sin` & `libfsntfs-20240501/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/po/Makevars` & `libfsntfs-20240501/po/Makevars`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/po/Makevars.in` & `libfsntfs-20240501/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/po/Rules-quot` & `libfsntfs-20240501/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_windows_1251.c` & `libfsntfs-20240501/libuna/libuna_codepage_windows_1251.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1251 codepage (Cyrillic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_utf16_string.c` & `libfsntfs-20240501/libuna/libuna_utf16_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_base16_stream.c` & `libfsntfs-20240501/libuna/libuna_base16_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base16 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_utf8_stream.h` & `libfsntfs-20240501/libuna/libuna_utf8_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_iso_8859_2.h` & `libfsntfs-20240501/libuna/libuna_codepage_iso_8859_2.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-2 codepage (Central European) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_windows_932.c` & `libfsntfs-20240501/libuna/libuna_codepage_windows_932.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 932 codepage (Japanese Shift-JIS) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_dingbats.h` & `libfsntfs-20240501/libuna/libuna_codepage_mac_dingbats.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacDingbats codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_utf8_string.c` & `libfsntfs-20240501/libuna/libuna_utf8_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_base64_stream.c` & `libfsntfs-20240501/libuna/libuna_base64_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base64 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_error.h` & `libfsntfs-20240501/libuna/libuna_error.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_turkish.h` & `libfsntfs-20240501/libuna/libuna_codepage_mac_turkish.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacTurkish codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_unicode_character.c` & `libfsntfs-20240501/libuna/libuna_unicode_character.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Unicode character functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_gaelic.c` & `libfsntfs-20240501/libuna/libuna_codepage_mac_gaelic.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacGaelic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_arabic.h` & `libfsntfs-20240501/libuna/libuna_codepage_mac_arabic.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacArabic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_thai.c` & `libfsntfs-20240501/libuna/libuna_codepage_mac_thai.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacThai codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_windows_874.h` & `libfsntfs-20240501/libuna/libuna_codepage_windows_874.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 874 codepage (Thai) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_iso_8859_15.h` & `libfsntfs-20240501/libuna/libuna_codepage_iso_8859_9.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-15 codepage (Latin 9) functions
+ * ISO 8859-9 codepage (Turkish) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,31 +15,31 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_15_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_15_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_9_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_9_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_15_byte_stream_to_unicode_base_0xa0[ 32 ];
+const uint16_t libuna_codepage_iso_8859_9_byte_stream_to_unicode_base_0xd0[ 48 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_15_unicode_to_byte_stream_base_0x00a0[ 32 ];
+const uint8_t libuna_codepage_iso_8859_9_unicode_to_byte_stream_base_0x00d0[ 48 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_15_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_9_H ) */
```

### Comparing `libfsntfs-20240119/libuna/libuna_utf8_string.h` & `libfsntfs-20240501/libuna/libuna_utf8_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_iso_8859_16.c` & `libfsntfs-20240501/libuna/libuna_codepage_iso_8859_16.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-16 codepage (Latin 10) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_windows_1255.c` & `libfsntfs-20240501/libuna/libuna_codepage_windows_1255.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1255 codepage (Hebrew) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_utf7_stream.c` & `libfsntfs-20240501/libuna/libuna_utf7_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-7 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_byte_stream.h` & `libfsntfs-20240501/libuna/libuna_byte_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Byte stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_koi8_u.c` & `libfsntfs-20240501/libuna/libuna_codepage_koi8_u.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * KOI8-U codepage (Ukrainian Cyrillic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_unused.h` & `libfsntfs-20240501/libuna/libuna_unused.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_iso_8859_6.c` & `libfsntfs-20240501/libuna/libuna_codepage_iso_8859_6.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-6 codepage (Arabic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_iso_8859_14.c` & `libfsntfs-20240501/libuna/libuna_codepage_iso_8859_14.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-14 codepage (Celtic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_base64_stream.h` & `libfsntfs-20240501/libuna/libuna_base64_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base64 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_error.c` & `libfsntfs-20240501/libuna/libuna_error.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_centraleurroman.h` & `libfsntfs-20240501/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCentralEurRoman codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_romanian.c` & `libfsntfs-20240501/libuna/libuna_codepage_mac_romanian.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRomanian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_iso_8859_6.h` & `libfsntfs-20240501/libuna/libuna_codepage_iso_8859_6.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-6 codepage (Arabic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_iso_8859_9.c` & `libfsntfs-20240501/libuna/libuna_codepage_iso_8859_9.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-9 codepage (Turkish) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_russian.h` & `libfsntfs-20240501/libuna/libuna_codepage_mac_russian.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRussian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_dingbats.c` & `libfsntfs-20240501/libuna/libuna_codepage_mac_dingbats.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacDingbats codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_iso_8859_15.c` & `libfsntfs-20240501/libuna/libuna_codepage_iso_8859_15.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-15 codepage (Latin 9) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_windows_936.c` & `libfsntfs-20240501/libuna/libuna_codepage_windows_936.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 936 codepage (Chinese Simplified) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_croatian.h` & `libfsntfs-20240501/libuna/libuna_codepage_mac_croatian.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCroatian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_scsu.h` & `libfsntfs-20240501/libuna/libuna_scsu.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Standard Compression Scheme for Unicode (SCSU) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/Makefile.am` & `libfsntfs-20240501/libuna/Makefile.am`

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
@@ -73,17 +73,17 @@
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
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
```

### Comparing `libfsntfs-20240119/libuna/libuna_utf32_stream.c` & `libfsntfs-20240501/libuna/libuna_utf32_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-32 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_windows_936.h` & `libfsntfs-20240501/libuna/libuna_codepage_windows_936.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 936 codepage (Chinese Simplified) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_iso_8859_10.c` & `libfsntfs-20240501/libuna/libuna_codepage_iso_8859_10.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-10 codepage (Nordic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_roman.c` & `libfsntfs-20240501/libuna/libuna_codepage_mac_roman.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRoman codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_utf7_stream.h` & `libfsntfs-20240501/libuna/libuna_utf7_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-7 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_iso_8859_3.h` & `libfsntfs-20240501/libuna/libuna_codepage_iso_8859_3.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-3 codepage (Latin 3) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_thai.h` & `libfsntfs-20240501/libuna/libuna_codepage_mac_thai.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacThai codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_farsi.h` & `libfsntfs-20240501/libuna/libuna_codepage_mac_farsi.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacFarsi codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_ukrainian.c` & `libfsntfs-20240501/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacUkrainian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_inuit.c` & `libfsntfs-20240501/libuna/libuna_codepage_mac_inuit.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacInuit codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_windows_932.h` & `libfsntfs-20240501/libuna/libuna_codepage_windows_932.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 932 codepage (Japanese Shift-JIS) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_windows_874.c` & `libfsntfs-20240501/libuna/libuna_codepage_windows_874.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 874 codepage (Thai) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_iso_8859_5.c` & `libfsntfs-20240501/libuna/libuna_codepage_iso_8859_5.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-5 codepage (Cyrillic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_iso_8859_10.h` & `libfsntfs-20240501/libuna/libuna_codepage_iso_8859_10.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-10 codepage (Nordic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_definitions.h` & `libfsntfs-20240501/libuna/libuna_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -31,19 +31,19 @@
 
 /* The definitions in <libuna/definitions.h> are copied here
  * for local use of libuna
  */
 #else
 #include <byte_stream.h>
 
-#define LIBUNA_VERSION						20230710
+#define LIBUNA_VERSION						20240414
 
 /* The libuna version string
  */
-#define LIBUNA_VERSION_STRING					"20230710"
+#define LIBUNA_VERSION_STRING					"20240414"
 
 /* The endian definitions
  */
 #define	LIBUNA_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define	LIBUNA_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The codepage definitions
```

### Comparing `libfsntfs-20240119/libuna/libuna_url_stream.h` & `libfsntfs-20240501/libuna/libuna_url_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Percent or URL encoded stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_icelandic.h` & `libfsntfs-20240501/libuna/libuna_codepage_mac_icelandic.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacIcelandic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_koi8_u.h` & `libfsntfs-20240501/libuna/libuna_codepage_koi8_u.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * KOI8-U codepage (Ukrainian Cyrillic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_utf16_stream.c` & `libfsntfs-20240501/libuna/libuna_utf16_stream.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_windows_1253.c` & `libfsntfs-20240501/libuna/libuna_codepage_windows_1253.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1253 codepage (Greek) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_iso_8859_4.h` & `libfsntfs-20240501/libuna/libuna_codepage_iso_8859_4.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-4 codepage (Baltic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_greek.c` & `libfsntfs-20240501/libuna/libuna_codepage_mac_greek.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacGreek codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_libcerror.h` & `libfsntfs-20240501/libfdatetime/libfdatetime_libcerror.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_LIBCERROR_H )
-#define _LIBUNA_LIBCERROR_H
+#if !defined( _LIBFDATETIME_LIBCERROR_H )
+#define _LIBFDATETIME_LIBCERROR_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCERROR for local use of libcerror
  */
 #if defined( HAVE_LOCAL_LIBCERROR )
 
@@ -42,9 +42,9 @@
 #define LIBCERROR_DLL_IMPORT
 #endif
 
 #include <libcerror.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCERROR ) */
 
-#endif /* !defined( _LIBUNA_LIBCERROR_H ) */
+#endif /* !defined( _LIBFDATETIME_LIBCERROR_H ) */
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_centraleurroman.c` & `libfsntfs-20240501/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCentralEurRoman codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_windows_1254.c` & `libfsntfs-20240501/libuna/libuna_codepage_windows_1254.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1254 codepage (Turkish) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_iso_8859_13.h` & `libfsntfs-20240501/libuna/libuna_codepage_iso_8859_13.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-13 codepage (Baltic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_iso_8859_7.h` & `libfsntfs-20240501/libuna/libuna_codepage_iso_8859_7.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-7 codepage (Greek) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_windows_1255.h` & `libfsntfs-20240501/libuna/libuna_codepage_windows_1251.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Windows 1255 codepage (Hebrew) functions
+ * Windows 1251 codepage (Cyrillic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1255_H )
-#define _LIBUNA_CODEPAGE_WINDOWS_1255_H
+#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1251_H )
+#define _LIBUNA_CODEPAGE_WINDOWS_1251_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_windows_1255_copy_from_byte_stream(
+int libuna_codepage_windows_1251_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_windows_1255_copy_to_byte_stream(
+int libuna_codepage_windows_1251_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1255_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1251_H ) */
```

### Comparing `libfsntfs-20240119/libuna/libuna_unicode_character.h` & `libfsntfs-20240501/libuna/libuna_unicode_character.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Unicode character functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_iso_8859_8.h` & `libfsntfs-20240501/libuna/libuna_codepage_iso_8859_8.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-8 codepage (Hebrew) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_iso_8859_13.c` & `libfsntfs-20240501/libuna/libuna_codepage_iso_8859_13.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-13 codepage (Baltic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_windows_949.h` & `libfsntfs-20240501/libuna/libuna_codepage_windows_949.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 949 codepage (Korean) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_cyrillic.c` & `libfsntfs-20240501/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCyrillic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_celtic.c` & `libfsntfs-20240501/libuna/libuna_codepage_mac_celtic.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCeltic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_support.h` & `libfsntfs-20240501/libuna/libuna_support.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_iso_8859_4.c` & `libfsntfs-20240501/libuna/libuna_codepage_iso_8859_4.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-4 codepage (Baltic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_windows_949.c` & `libfsntfs-20240501/libuna/libuna_codepage_windows_949.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 949 codepage (Korean) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_utf16_stream.h` & `libfsntfs-20240501/libuna/libuna_utf16_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_symbol.c` & `libfsntfs-20240501/libuna/libuna_codepage_mac_symbol.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacSymbol codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_roman.h` & `libfsntfs-20240501/libuna/libuna_codepage_mac_roman.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRoman codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_windows_1257.c` & `libfsntfs-20240501/libuna/libuna_codepage_windows_1257.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1257 codepage (Baltic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_windows_1254.h` & `libfsntfs-20240501/libuna/libuna_codepage_windows_1254.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1254 codepage (Turkish) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_windows_950.c` & `libfsntfs-20240501/libuna/libuna_codepage_windows_950.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 950 codepage (Traditional Chinese) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_extern.h` & `libfsntfs-20240501/libuna/libuna_extern.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_windows_1256.c` & `libfsntfs-20240501/libuna/libuna_codepage_windows_1256.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1256 codepage (Arabic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_types.h` & `libfsntfs-20240501/libuna/libuna_types.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_base32_stream.h` & `libfsntfs-20240501/libuna/libuna_base32_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base32 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_windows_1253.h` & `libfsntfs-20240501/libuna/libuna_codepage_windows_1253.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1253 codepage (Greek) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_iso_8859_16.h` & `libfsntfs-20240501/libuna/libuna_codepage_iso_8859_16.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-16 codepage (Latin 10) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_utf8_stream.c` & `libfsntfs-20240501/libuna/libuna_utf8_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_windows_1250.h` & `libfsntfs-20240501/libuna/libuna_codepage_windows_1250.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1250 codepage (Central European) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_iso_8859_2.c` & `libfsntfs-20240501/libuna/libuna_codepage_iso_8859_2.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-2 codepage (Central European) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_support.c` & `libfsntfs-20240501/libcerror/libcerror_support.c`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -18,22 +18,22 @@
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include <common.h>
 #include <types.h>
 
-#include "libuna_definitions.h"
-#include "libuna_support.h"
+#include "libcerror_definitions.h"
+#include "libcerror_support.h"
 
-#if !defined( HAVE_LOCAL_LIBUNA )
+#if !defined( HAVE_LOCAL_LIBCERROR )
 
 /* Returns the library version as a string
  */
-const char *libuna_get_version(
+const char *libcerror_get_version(
              void )
 {
-	return( (const char *) LIBUNA_VERSION_STRING );
+	return( (const char *) LIBCERROR_VERSION_STRING );
 }
 
-#endif /* !defined( HAVE_LOCAL_LIBUNA ) */
+#endif /* !defined( HAVE_LOCAL_LIBCERROR ) */
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_koi8_r.c` & `libfsntfs-20240501/libuna/libuna_codepage_koi8_r.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * KOI8-R codepage (Russian Cyrillic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_iso_8859_5.h` & `libfsntfs-20240501/libuna/libuna_codepage_iso_8859_15.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-5 codepage (Cyrillic) functions
+ * ISO 8859-15 codepage (Latin 9) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,31 +15,31 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_5_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_5_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_15_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_15_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_5_byte_stream_to_unicode_base_0xa0[ 96 ];
+const uint16_t libuna_codepage_iso_8859_15_byte_stream_to_unicode_base_0xa0[ 32 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_5_unicode_to_byte_stream_base_0x0400[ 96 ];
+const uint8_t libuna_codepage_iso_8859_15_unicode_to_byte_stream_base_0x00a0[ 32 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_5_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_15_H ) */
```

### Comparing `libfsntfs-20240119/libuna/libuna_utf16_string.h` & `libfsntfs-20240501/libuna/libuna_utf16_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_utf32_string.c` & `libfsntfs-20240501/libuna/libuna_utf32_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-32 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_icelandic.c` & `libfsntfs-20240501/libuna/libuna_codepage_mac_icelandic.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacIcelandic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_windows_1256.h` & `libfsntfs-20240501/libuna/libuna_codepage_windows_1256.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1256 codepage (Arabic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_utf32_string.h` & `libfsntfs-20240501/libuna/libuna_utf32_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-32 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_romanian.h` & `libfsntfs-20240501/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * MacRomanian codepage functions
+ * MacCyrillic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_MAC_ROMANIAN_H )
-#define _LIBUNA_CODEPAGE_MAC_ROMANIAN_H
+#if !defined( _LIBUNA_CODEPAGE_MAC_CYRILLIC_H )
+#define _LIBUNA_CODEPAGE_MAC_CYRILLIC_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_mac_romanian_copy_from_byte_stream(
+int libuna_codepage_mac_cyrillic_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_mac_romanian_copy_to_byte_stream(
+int libuna_codepage_mac_cyrillic_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_MAC_ROMANIAN_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_MAC_CYRILLIC_H ) */
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_iso_8859_8.c` & `libfsntfs-20240501/libuna/libuna_codepage_iso_8859_8.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-8 codepage (Hebrew) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_koi8_r.h` & `libfsntfs-20240501/libuna/libuna_codepage_koi8_r.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * KOI8-R codepage (Russian Cyrillic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_cyrillic.h` & `libfsntfs-20240501/libuna/libuna_codepage_mac_gaelic.h`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * MacCyrillic codepage functions
+ * MacGaelic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_MAC_CYRILLIC_H )
-#define _LIBUNA_CODEPAGE_MAC_CYRILLIC_H
+#if !defined( _LIBUNA_CODEPAGE_MAC_GAELIC_H )
+#define _LIBUNA_CODEPAGE_MAC_GAELIC_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_mac_cyrillic_copy_from_byte_stream(
+int libuna_codepage_mac_gaelic_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_mac_cyrillic_copy_to_byte_stream(
+int libuna_codepage_mac_gaelic_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_MAC_CYRILLIC_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_MAC_GAELIC_H ) */
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_arabic.c` & `libfsntfs-20240501/libuna/libuna_codepage_mac_arabic.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacArabic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_croatian.c` & `libfsntfs-20240501/libuna/libuna_codepage_mac_croatian.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCroatian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_iso_8859_9.h` & `libfsntfs-20240501/libuna/libuna_codepage_iso_8859_5.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-9 codepage (Turkish) functions
+ * ISO 8859-5 codepage (Cyrillic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,31 +15,31 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_9_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_9_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_5_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_5_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_9_byte_stream_to_unicode_base_0xd0[ 48 ];
+const uint16_t libuna_codepage_iso_8859_5_byte_stream_to_unicode_base_0xa0[ 96 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_9_unicode_to_byte_stream_base_0x00d0[ 48 ];
+const uint8_t libuna_codepage_iso_8859_5_unicode_to_byte_stream_base_0x0400[ 96 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_9_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_5_H ) */
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_greek.h` & `libfsntfs-20240501/libuna/libuna_codepage_mac_greek.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacGreek codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_windows_1258.h` & `libfsntfs-20240501/libuna/libuna_codepage_windows_1258.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1258 codepage (Vietnamese) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_iso_8859_7.c` & `libfsntfs-20240501/libuna/libuna_codepage_iso_8859_7.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-7 codepage (Greek) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/Makefile.in` & `libfsntfs-20240501/libuna/Makefile.in`

 * *Files 10% similar despite different names*

```diff
@@ -655,14 +655,16 @@
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
@@ -727,16 +729,16 @@
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
@@ -802,15 +804,16 @@
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
@@ -1072,24 +1075,89 @@
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
 
@@ -1209,14 +1277,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -1227,23 +1297,22 @@
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
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_iso_8859_3.c` & `libfsntfs-20240501/libuna/libuna_codepage_iso_8859_3.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-3 codepage (Latin 3) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_windows_1250.c` & `libfsntfs-20240501/libuna/libuna_codepage_windows_1250.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1250 codepage (Central European) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_scsu.c` & `libfsntfs-20240501/libuna/libuna_scsu.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Standard Compression Scheme for Unicode (SCSU) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_windows_1252.c` & `libfsntfs-20240501/libuna/libuna_codepage_windows_1252.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1252 codepage (Western European/Latin 1) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_turkish.c` & `libfsntfs-20240501/libuna/libuna_codepage_mac_turkish.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacTurkish codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_ukrainian.h` & `libfsntfs-20240501/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacUkrainian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_russian.c` & `libfsntfs-20240501/libuna/libuna_codepage_mac_russian.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRussian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_windows_1258.c` & `libfsntfs-20240501/libuna/libuna_codepage_windows_1258.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1258 codepage (Vietnamese) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_celtic.h` & `libfsntfs-20240501/libuna/libuna_codepage_mac_celtic.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCeltic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_byte_stream.c` & `libfsntfs-20240501/libuna/libuna_byte_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Byte stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_gaelic.h` & `libfsntfs-20240501/libuna/libuna_codepage_windows_1257.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * MacGaelic codepage functions
+ * Windows 1257 codepage (Baltic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_MAC_GAELIC_H )
-#define _LIBUNA_CODEPAGE_MAC_GAELIC_H
+#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1257_H )
+#define _LIBUNA_CODEPAGE_WINDOWS_1257_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_mac_gaelic_copy_from_byte_stream(
+int libuna_codepage_windows_1257_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_mac_gaelic_copy_to_byte_stream(
+int libuna_codepage_windows_1257_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_MAC_GAELIC_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1257_H ) */
```

### Comparing `libfsntfs-20240119/libuna/libuna_utf32_stream.h` & `libfsntfs-20240501/libuna/libuna_utf32_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-32 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_symbol.h` & `libfsntfs-20240501/libuna/libuna_codepage_mac_symbol.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacSymbol codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_windows_1257.h` & `libfsntfs-20240501/libuna/libuna_codepage_mac_inuit.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Windows 1257 codepage (Baltic) functions
+ * MacInuit codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1257_H )
-#define _LIBUNA_CODEPAGE_WINDOWS_1257_H
+#if !defined( _LIBUNA_CODEPAGE_MAC_INUIT_H )
+#define _LIBUNA_CODEPAGE_MAC_INUIT_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_windows_1257_copy_from_byte_stream(
+int libuna_codepage_mac_inuit_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_windows_1257_copy_to_byte_stream(
+int libuna_codepage_mac_inuit_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1257_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_MAC_INUIT_H ) */
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_inuit.h` & `libfsntfs-20240501/libuna/libuna_codepage_mac_romanian.h`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * MacInuit codepage functions
+ * MacRomanian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_MAC_INUIT_H )
-#define _LIBUNA_CODEPAGE_MAC_INUIT_H
+#if !defined( _LIBUNA_CODEPAGE_MAC_ROMANIAN_H )
+#define _LIBUNA_CODEPAGE_MAC_ROMANIAN_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_mac_inuit_copy_from_byte_stream(
+int libuna_codepage_mac_romanian_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_mac_inuit_copy_to_byte_stream(
+int libuna_codepage_mac_romanian_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_MAC_INUIT_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_MAC_ROMANIAN_H ) */
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_mac_farsi.c` & `libfsntfs-20240501/libuna/libuna_codepage_mac_farsi.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacFarsi codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_windows_950.h` & `libfsntfs-20240501/libuna/libuna_codepage_windows_950.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 950 codepage (Traditional Chinese) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_url_stream.c` & `libfsntfs-20240501/libuna/libuna_url_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Percent or URL encoded stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_windows_1251.h` & `libfsntfs-20240501/libuna/libuna_codepage_windows_1255.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Windows 1251 codepage (Cyrillic) functions
+ * Windows 1255 codepage (Hebrew) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1251_H )
-#define _LIBUNA_CODEPAGE_WINDOWS_1251_H
+#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1255_H )
+#define _LIBUNA_CODEPAGE_WINDOWS_1255_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_windows_1251_copy_from_byte_stream(
+int libuna_codepage_windows_1255_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_windows_1251_copy_to_byte_stream(
+int libuna_codepage_windows_1255_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1251_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1255_H ) */
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_windows_1252.h` & `libfsntfs-20240501/libuna/libuna_codepage_windows_1252.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1252 codepage (Western European/Latin 1) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_codepage_iso_8859_14.h` & `libfsntfs-20240501/libuna/libuna_codepage_iso_8859_14.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-14 codepage (Celtic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_base16_stream.h` & `libfsntfs-20240501/libuna/libuna_base16_stream.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base16 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/libuna/libuna_base32_stream.c` & `libfsntfs-20240501/libuna/libuna_base32_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base32 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfsntfs-20240119/Makefile.in` & `libfsntfs-20240501/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -537,14 +537,16 @@
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
@@ -675,16 +677,23 @@
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
+	libfsntfs.pc \
+	libfsntfs.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libfsntfs.pc
 
 all: all-recursive
 
@@ -1101,23 +1110,26 @@
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
 
@@ -1229,22 +1241,10 @@
 	(cd $(srcdir)/libfdata && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdatetime && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfguid && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfwnt && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfsntfs && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libfsntfs.pc
-	-rm -f libfsntfs.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfsntfs-20240119/libcnotify/libcnotify_definitions.h` & `libfsntfs-20240501/libcnotify/libcnotify_definitions.h`

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

### Comparing `libfsntfs-20240119/libcnotify/libcnotify_extern.h` & `libfsntfs-20240501/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcnotify/libcnotify_support.c` & `libfsntfs-20240501/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcnotify/libcnotify_stream.h` & `libfsntfs-20240501/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcnotify/Makefile.am` & `libfsntfs-20240501/libcnotify/Makefile.am`

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

### Comparing `libfsntfs-20240119/libcnotify/libcnotify_unused.h` & `libfsntfs-20240501/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcnotify/libcnotify_verbose.h` & `libfsntfs-20240501/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcnotify/libcnotify_print.h` & `libfsntfs-20240501/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcnotify/libcnotify_stream.c` & `libfsntfs-20240501/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcnotify/libcnotify_support.h` & `libfsntfs-20240501/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcnotify/libcnotify_verbose.c` & `libfsntfs-20240501/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcnotify/Makefile.in` & `libfsntfs-20240501/libcnotify/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -479,14 +479,16 @@
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
@@ -551,30 +553,31 @@
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
@@ -777,24 +780,30 @@
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
 
@@ -881,17 +890,14 @@
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

### Comparing `libfsntfs-20240119/libcnotify/libcnotify_libcerror.h` & `libfsntfs-20240501/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcnotify/libcnotify_print.c` & `libfsntfs-20240501/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcerror/libcerror_system.c` & `libfsntfs-20240501/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcerror/libcerror_error.c` & `libfsntfs-20240501/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcerror/libcerror_extern.h` & `libfsntfs-20240501/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcerror/Makefile.am` & `libfsntfs-20240501/libcerror/Makefile.am`

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

### Comparing `libfsntfs-20240119/libcerror/libcerror_types.h` & `libfsntfs-20240501/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcerror/libcerror_support.h` & `libfsntfs-20240501/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcerror/libcerror_error.h` & `libfsntfs-20240501/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcerror/libcerror_system.h` & `libfsntfs-20240501/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcerror/libcerror_definitions.h` & `libfsntfs-20240501/libcerror/libcerror_definitions.h`

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

### Comparing `libfsntfs-20240119/libcerror/libcerror_support.c` & `libfsntfs-20240501/libfdatetime/libfdatetime_support.c`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -18,22 +18,24 @@
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include <common.h>
 #include <types.h>
 
-#include "libcerror_definitions.h"
-#include "libcerror_support.h"
+#include <stdio.h>
 
-#if !defined( HAVE_LOCAL_LIBCERROR )
+#include "libfdatetime_definitions.h"
+#include "libfdatetime_support.h"
+
+#if !defined( HAVE_LOCAL_LIBFDATETIME )
 
 /* Returns the library version as a string
  */
-const char *libcerror_get_version(
+const char *libfdatetime_get_version(
              void )
 {
-	return( (const char *) LIBCERROR_VERSION_STRING );
+	return( (const char *) LIBFDATETIME_VERSION_STRING );
 }
 
-#endif /* !defined( HAVE_LOCAL_LIBCERROR ) */
+#endif
```

### Comparing `libfsntfs-20240119/libcerror/libcerror_unused.h` & `libfsntfs-20240501/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libcerror/Makefile.in` & `libfsntfs-20240501/libcerror/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -476,14 +476,16 @@
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
@@ -548,28 +550,29 @@
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
@@ -771,24 +774,29 @@
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
 
@@ -874,17 +882,14 @@
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

### Comparing `libfsntfs-20240119/libfdatetime/libfdatetime_floatingtime.h` & `libfsntfs-20240501/libfdatetime/libfdatetime_floatingtime.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdatetime/libfdatetime_nsf_timedate.c` & `libfsntfs-20240501/libfdatetime/libfdatetime_nsf_timedate.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdatetime/libfdatetime_error.h` & `libfsntfs-20240501/libfdatetime/libfdatetime_error.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdatetime/libfdatetime_floatingtime.c` & `libfsntfs-20240501/libfdatetime/libfdatetime_floatingtime.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdatetime/libfdatetime_support.h` & `libfsntfs-20240501/libfdatetime/libfdatetime_support.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdatetime/libfdatetime_hfs_time.h` & `libfsntfs-20240501/libfdatetime/libfdatetime_hfs_time.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdatetime/libfdatetime_definitions.h` & `libfsntfs-20240501/libfdatetime/libfdatetime_definitions.h`

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

### Comparing `libfsntfs-20240119/libfdatetime/libfdatetime_hfs_time.c` & `libfsntfs-20240501/libfdatetime/libfdatetime_hfs_time.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdatetime/Makefile.am` & `libfsntfs-20240501/libfdatetime/Makefile.am`

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

### Comparing `libfsntfs-20240119/libfdatetime/libfdatetime_filetime.c` & `libfsntfs-20240501/libfdatetime/libfdatetime_filetime.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdatetime/libfdatetime_systemtime.h` & `libfsntfs-20240501/libfdatetime/libfdatetime_systemtime.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdatetime/libfdatetime_extern.h` & `libfsntfs-20240501/libfdatetime/libfdatetime_extern.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdatetime/libfdatetime_posix_time.c` & `libfsntfs-20240501/libfdatetime/libfdatetime_posix_time.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdatetime/libfdatetime_unused.h` & `libfsntfs-20240501/libfdatetime/libfdatetime_unused.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdatetime/libfdatetime_fat_date_time.h` & `libfsntfs-20240501/libfdatetime/libfdatetime_fat_date_time.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdatetime/libfdatetime_systemtime.c` & `libfsntfs-20240501/libfdatetime/libfdatetime_systemtime.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdatetime/libfdatetime_nsf_timedate.h` & `libfsntfs-20240501/libfdatetime/libfdatetime_nsf_timedate.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdatetime/libfdatetime_libcerror.h` & `libfsntfs-20240501/libhmac/libhmac_libcerror.h`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBFDATETIME_LIBCERROR_H )
-#define _LIBFDATETIME_LIBCERROR_H
+#if !defined( _LIBHMAC_LIBCERROR_H )
+#define _LIBHMAC_LIBCERROR_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCERROR for local use of libcerror
  */
 #if defined( HAVE_LOCAL_LIBCERROR )
 
@@ -42,9 +42,9 @@
 #define LIBCERROR_DLL_IMPORT
 #endif
 
 #include <libcerror.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCERROR ) */
 
-#endif /* !defined( _LIBFDATETIME_LIBCERROR_H ) */
+#endif /* !defined( _LIBHMAC_LIBCERROR_H ) */
```

### Comparing `libfsntfs-20240119/libfdatetime/libfdatetime_error.c` & `libfsntfs-20240501/libfdatetime/libfdatetime_error.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdatetime/libfdatetime_posix_time.h` & `libfsntfs-20240501/libfdatetime/libfdatetime_posix_time.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdatetime/libfdatetime_date_time_values.h` & `libfsntfs-20240501/libfdatetime/libfdatetime_date_time_values.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdatetime/libfdatetime_filetime.h` & `libfsntfs-20240501/libfdatetime/libfdatetime_filetime.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdatetime/libfdatetime_date_time_values.c` & `libfsntfs-20240501/libfdatetime/libfdatetime_date_time_values.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdatetime/libfdatetime_types.h` & `libfsntfs-20240501/libfdatetime/libfdatetime_types.h`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfdatetime/Makefile.in` & `libfsntfs-20240501/libfdatetime/Makefile.in`

 * *Files 8% similar despite different names*

```diff
@@ -498,14 +498,16 @@
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
@@ -570,16 +572,16 @@
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
@@ -592,15 +594,16 @@
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
@@ -809,24 +812,36 @@
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
 
@@ -919,17 +934,14 @@
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

### Comparing `libfsntfs-20240119/libfdatetime/libfdatetime_fat_date_time.c` & `libfsntfs-20240501/libfdatetime/libfdatetime_fat_date_time.c`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/aclocal.m4` & `libfsntfs-20240501/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/libfsntfs.spec.in` & `libfsntfs-20240501/libfsntfs.spec.in`

 * *Files identical despite different names*

### Comparing `libfsntfs-20240119/configure.ac` & `libfsntfs-20240501/configure.ac`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libfsntfs],
- [20240119],
+ [20240501],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libfsntfs.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```


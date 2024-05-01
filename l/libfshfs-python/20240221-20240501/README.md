# Comparing `tmp/libfshfs-python-20240221.tar.gz` & `tmp/libfshfs-python-20240501.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libfshfs-python-20240221.tar", last modified: Wed Feb 21 06:20:12 2024, max compression
+gzip compressed data, was "libfshfs-python-20240501.tar", last modified: Wed May  1 07:57:13 2024, max compression
```

## Comparing `libfshfs-python-20240221.tar` & `libfshfs-python-20240501.tar`

### file list

```diff
@@ -1,1005 +1,1005 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:10.000000 libfshfs-20240221/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_area.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_mapped_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1291 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_area.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_mapped_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_segments_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_segments_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34498 2024-02-21 06:04:26.000000 libfshfs-20240221/libfdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-02-21 06:04:08.000000 libfshfs-20240221/libfdata/libfdata_vector.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/libfmos/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2023 2024-02-21 06:04:11.000000 libfshfs-20240221/libfmos/libfmos_lzfse_bit_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2269 2024-02-21 06:04:11.000000 libfshfs-20240221/libfmos/libfmos_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2964 2024-02-21 06:04:11.000000 libfshfs-20240221/libfmos/libfmos_lzfse_decoder.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2024-02-21 06:04:11.000000 libfshfs-20240221/libfmos/libfmos_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7799 2024-02-21 06:04:11.000000 libfshfs-20240221/libfmos/libfmos_adc.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3441 2024-02-21 06:04:11.000000 libfshfs-20240221/libfmos/libfmos_lzfse.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-02-21 06:04:11.000000 libfshfs-20240221/libfmos/libfmos_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1321 2024-02-21 06:04:11.000000 libfshfs-20240221/libfmos/libfmos_adc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-02-21 06:04:11.000000 libfshfs-20240221/libfmos/libfmos_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-21 06:04:11.000000 libfshfs-20240221/libfmos/libfmos_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      961 2024-02-21 06:04:11.000000 libfshfs-20240221/libfmos/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-21 06:04:11.000000 libfshfs-20240221/libfmos/libfmos_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25840 2024-02-21 06:04:11.000000 libfshfs-20240221/libfmos/libfmos_lzvn.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-02-21 06:04:11.000000 libfshfs-20240221/libfmos/libfmos_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6380 2024-02-21 06:04:11.000000 libfshfs-20240221/libfmos/libfmos_lzfse_bit_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3271 2024-02-21 06:04:11.000000 libfshfs-20240221/libfmos/libfmos_lzfse_decoder.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-21 06:04:11.000000 libfshfs-20240221/libfmos/libfmos_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    60280 2024-02-21 06:04:11.000000 libfshfs-20240221/libfmos/libfmos_lzfse.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-02-21 06:04:11.000000 libfshfs-20240221/libfmos/libfmos_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-21 06:04:11.000000 libfshfs-20240221/libfmos/libfmos_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-02-21 06:04:11.000000 libfshfs-20240221/libfmos/libfmos_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1326 2024-02-21 06:04:11.000000 libfshfs-20240221/libfmos/libfmos_lzvn.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-21 06:04:11.000000 libfshfs-20240221/libfmos/libfmos_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32435 2024-02-21 06:04:26.000000 libfshfs-20240221/libfmos/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-02-21 05:48:48.000000 libfshfs-20240221/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-02-21 06:04:25.000000 libfshfs-20240221/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 05:48:48.000000 libfshfs-20240221/NEWS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/libfshfs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13516 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_btree_node_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2004 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_btree_node_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21335 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_extents_btree_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40326 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_file_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4581 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_block_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3591 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_attribute_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1090 2024-02-21 06:04:37.000000 libfshfs-20240221/libfshfs/libfshfs.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31797 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_compressed_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2393 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_fork_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2857 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13183 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_file_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2094 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_huffman_tree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5206 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1398 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48205 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_directory_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21037 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_data_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28435 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_directory_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4979 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_file_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12883 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_btree_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6027 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_compressed_data_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3817 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_btree_node_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12308 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_thread_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22767 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1357 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_extents_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2280 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_bit_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9194 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_catalog_btree_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9595 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24114 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_master_directory_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1833 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_btree_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11422 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_fork_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48738 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_deflate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2321 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_btree_node_vector.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7276 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_extents_btree_key.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3002 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/fshfs_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19641 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_volume_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1836 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_btree_node_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4350 2023-12-03 09:06:53.000000 libfshfs-20240221/libfshfs/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3306 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_compressed_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4235 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_btree_node_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2830 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_catalog_btree_key.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5401 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4233 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_directory_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5723 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_directory_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2119 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_profiler.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1478 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/fshfs_compressed_data.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6809 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_btree_node_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5295 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_extent.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10716 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/fshfs_catalog_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14066 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_catalog_btree_key.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   147422 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4690 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35932 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_extended_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1792 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1726 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2841 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_attributes_btree_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2495 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_volume_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1868 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_thread_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15010 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_name.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2802 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_extents_btree_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_block_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2449 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_attributes_btree_key.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   240954 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_name.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_extent.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   106513 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_catalog_btree_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3488 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_deflate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4078 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_extents_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1594 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_btree_node_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1924 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/fshfs_attributes_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1987 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/fshfs_extents_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2036 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52766 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3699 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/fshfs_volume_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1327 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_compression.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8113 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_btree_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3304 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_master_directory_block.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36176 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_file_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16909 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_allocation_block_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4169 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/fshfs_master_directory_block.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9705 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_compression.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5073 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_extended_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4688 2024-02-21 06:04:37.000000 libfshfs-20240221/libfshfs/libfshfs_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_allocation_block_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20986 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_attribute_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1092 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7930 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_bit_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2593 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_btree_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10859 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_attributes_btree_key.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6090 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_file_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2328 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_buffer_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    46157 2024-02-21 06:04:26.000000 libfshfs-20240221/libfshfs/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3716 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_data_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20152 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20259 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_attributes_btree_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1886 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_compressed_data_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_libfmos.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1955 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_extents_btree_key.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12520 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_huffman_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7821 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs_buffer_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8243 2024-02-21 05:48:50.000000 libfshfs-20240221/libfshfs/libfshfs_profiler.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1835 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/libfshfs.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1514 2024-02-21 05:48:49.000000 libfshfs-20240221/libfshfs/fshfs_fork_descriptor.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-02-21 06:04:26.000000 libfshfs-20240221/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-21 06:04:10.000000 libfshfs-20240221/libfguid/libfguid_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-02-21 06:04:10.000000 libfshfs-20240221/libfguid/libfguid_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-02-21 06:04:10.000000 libfshfs-20240221/libfguid/libfguid_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-21 06:04:10.000000 libfshfs-20240221/libfguid/libfguid_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      681 2024-02-21 06:04:10.000000 libfshfs-20240221/libfguid/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-21 06:04:10.000000 libfshfs-20240221/libfguid/libfguid_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-21 06:04:10.000000 libfshfs-20240221/libfguid/libfguid_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-02-21 06:04:10.000000 libfshfs-20240221/libfguid/libfguid_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-02-21 06:04:10.000000 libfshfs-20240221/libfguid/libfguid_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-02-21 06:04:10.000000 libfshfs-20240221/libfguid/libfguid_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-02-21 06:04:10.000000 libfshfs-20240221/libfguid/libfguid_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30713 2024-02-21 06:04:26.000000 libfshfs-20240221/libfguid/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-21 06:04:10.000000 libfshfs-20240221/libfguid/libfguid_error.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:10.000000 libfshfs-20240221/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4428 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/libfmos.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18233 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/libfdatetime.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31269 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/libcsplit.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-02-21 06:04:20.000000 libfshfs-20240221/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-02-21 06:04:20.000000 libfshfs-20240221/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15545 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/libfdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5232 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/libfuse.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-02-21 06:04:20.000000 libfshfs-20240221/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/libfguid.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/libbfio.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8319 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/libhmac.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-02-21 06:04:20.000000 libfshfs-20240221/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-02-21 06:04:20.000000 libfshfs-20240221/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27481 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/libcrypto.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7325 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/libfcache.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/pthread.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7383 2023-12-03 09:06:54.000000 libfshfs-20240221/m4/zlib.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:10.000000 libfshfs-20240221/include/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:10.000000 libfshfs-20240221/include/libfshfs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2308 2024-02-21 05:48:49.000000 libfshfs-20240221/include/libfshfs/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2306 2024-02-21 06:04:37.000000 libfshfs-20240221/include/libfshfs/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5073 2024-02-21 05:48:49.000000 libfshfs-20240221/include/libfshfs/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4942 2024-02-21 06:04:37.000000 libfshfs-20240221/include/libfshfs/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-02-21 05:48:49.000000 libfshfs-20240221/include/libfshfs/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2024-02-21 05:48:49.000000 libfshfs-20240221/include/libfshfs/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-21 05:48:49.000000 libfshfs-20240221/include/libfshfs/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1487 2024-02-21 06:04:37.000000 libfshfs-20240221/include/libfshfs/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5306 2024-02-21 05:48:49.000000 libfshfs-20240221/include/libfshfs/codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      474 2024-02-21 05:48:48.000000 libfshfs-20240221/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31635 2024-02-21 06:04:37.000000 libfshfs-20240221/include/libfshfs.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31635 2024-02-21 05:48:49.000000 libfshfs-20240221/include/libfshfs.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29259 2024-02-21 06:04:25.000000 libfshfs-20240221/include/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:10.000000 libfshfs-20240221/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-02-21 05:48:49.000000 libfshfs-20240221/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-02-21 05:48:49.000000 libfshfs-20240221/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-02-21 05:48:49.000000 libfshfs-20240221/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-02-21 05:48:49.000000 libfshfs-20240221/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-02-21 05:48:49.000000 libfshfs-20240221/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-02-21 05:48:49.000000 libfshfs-20240221/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-02-21 05:48:49.000000 libfshfs-20240221/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-02-21 05:48:48.000000 libfshfs-20240221/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-02-21 05:48:49.000000 libfshfs-20240221/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7374 2024-02-21 06:04:37.000000 libfshfs-20240221/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18404 2024-02-21 06:04:25.000000 libfshfs-20240221/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19482 2024-02-21 06:04:37.000000 libfshfs-20240221/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-02-21 05:48:49.000000 libfshfs-20240221/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-02-21 05:48:49.000000 libfshfs-20240221/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-02-21 05:48:49.000000 libfshfs-20240221/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26266 2024-02-21 06:04:25.000000 libfshfs-20240221/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:10.000000 libfshfs-20240221/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-02-21 06:04:01.000000 libfshfs-20240221/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-02-21 06:04:01.000000 libfshfs-20240221/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2024-02-21 06:04:01.000000 libfshfs-20240221/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-02-21 06:04:01.000000 libfshfs-20240221/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-21 06:04:01.000000 libfshfs-20240221/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-02-21 06:04:01.000000 libfshfs-20240221/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-02-21 06:04:01.000000 libfshfs-20240221/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-02-21 06:04:01.000000 libfshfs-20240221/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-02-21 06:04:01.000000 libfshfs-20240221/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-02-21 06:04:01.000000 libfshfs-20240221/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31269 2024-02-21 06:04:25.000000 libfshfs-20240221/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-21 06:04:01.000000 libfshfs-20240221/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-02-21 06:04:01.000000 libfshfs-20240221/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-02-21 06:04:01.000000 libfshfs-20240221/libclocale/libclocale_codepage.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:10.000000 libfshfs-20240221/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-02-21 06:04:06.000000 libfshfs-20240221/libfcache/libfcache_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-02-21 06:04:06.000000 libfshfs-20240221/libfcache/libfcache_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-02-21 06:04:06.000000 libfshfs-20240221/libfcache/libfcache_cache_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-21 06:04:06.000000 libfshfs-20240221/libfcache/libfcache_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-02-21 06:04:06.000000 libfshfs-20240221/libfcache/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-21 06:04:06.000000 libfshfs-20240221/libfcache/libfcache_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-21 06:04:06.000000 libfshfs-20240221/libfcache/libfcache_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-02-21 06:04:06.000000 libfshfs-20240221/libfcache/libfcache_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-02-21 06:04:06.000000 libfshfs-20240221/libfcache/libfcache_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-21 06:04:06.000000 libfshfs-20240221/libfcache/libfcache_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-21 06:04:06.000000 libfshfs-20240221/libfcache/libfcache_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-02-21 06:04:06.000000 libfshfs-20240221/libfcache/libfcache_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-21 06:04:06.000000 libfshfs-20240221/libfcache/libfcache_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-02-21 06:04:06.000000 libfshfs-20240221/libfcache/libfcache_cache_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31742 2024-02-21 06:04:26.000000 libfshfs-20240221/libfcache/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-02-21 06:04:06.000000 libfshfs-20240221/libfcache/libfcache_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-02-21 06:04:06.000000 libfshfs-20240221/libfcache/libfcache_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-02-21 06:04:06.000000 libfshfs-20240221/libfcache/libfcache_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2365 2023-12-03 09:06:45.000000 libfshfs-20240221/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:10.000000 libfshfs-20240221/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_file_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_file_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_file_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_file_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_file_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_file_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_memory_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_file_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_file_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_memory_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_memory_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34728 2024-02-21 06:04:25.000000 libfshfs-20240221/libbfio/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_memory_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-02-21 06:03:55.000000 libfshfs-20240221/libbfio/libbfio_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:06:45.000000 libfshfs-20240221/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-02-21 06:04:25.000000 libfshfs-20240221/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:10.000000 libfshfs-20240221/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1026 2024-02-21 05:48:50.000000 libfshfs-20240221/dpkg/copyright
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:10.000000 libfshfs-20240221/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-02-21 05:48:48.000000 libfshfs-20240221/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2173 2024-02-21 05:48:48.000000 libfshfs-20240221/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      769 2024-02-21 05:48:48.000000 libfshfs-20240221/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      121 2024-02-21 05:48:48.000000 libfshfs-20240221/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2024-02-21 06:04:37.000000 libfshfs-20240221/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-02-21 05:48:48.000000 libfshfs-20240221/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-02-21 05:48:48.000000 libfshfs-20240221/dpkg/libfshfs-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-02-21 05:48:48.000000 libfshfs-20240221/dpkg/libfshfs-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-02-21 05:48:48.000000 libfshfs-20240221/dpkg/libfshfs.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-02-21 05:48:48.000000 libfshfs-20240221/dpkg/libfshfs-tools.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      486 2024-02-21 06:04:37.000000 libfshfs-20240221/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-02-21 05:48:48.000000 libfshfs-20240221/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  2003870 2024-02-21 06:04:24.000000 libfshfs-20240221/configure
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/pyfshfs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16609 2024-02-21 05:48:50.000000 libfshfs-20240221/pyfshfs/pyfshfs_datetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2740 2024-02-21 05:50:44.000000 libfshfs-20240221/pyfshfs/pyfshfs_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2634 2024-02-21 05:48:50.000000 libfshfs-20240221/pyfshfs/pyfshfs_extended_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3486 2024-02-21 05:50:44.000000 libfshfs-20240221/pyfshfs/pyfshfs_extended_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8876 2024-02-21 05:48:50.000000 libfshfs-20240221/pyfshfs/pyfshfs_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9439 2024-02-21 05:48:50.000000 libfshfs-20240221/pyfshfs/pyfshfs_file_entries.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3020 2024-02-21 05:50:44.000000 libfshfs-20240221/pyfshfs/pyfshfs_data_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4118 2024-02-21 05:48:50.000000 libfshfs-20240221/pyfshfs/pyfshfs_file_object_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1525 2024-02-21 05:48:50.000000 libfshfs-20240221/pyfshfs/pyfshfs_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2023-12-03 09:06:54.000000 libfshfs-20240221/pyfshfs/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9546 2024-02-21 05:48:50.000000 libfshfs-20240221/pyfshfs/pyfshfs_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28438 2024-02-21 05:50:44.000000 libfshfs-20240221/pyfshfs/pyfshfs_extended_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-21 05:48:50.000000 libfshfs-20240221/pyfshfs/pyfshfs_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33880 2024-02-21 05:48:50.000000 libfshfs-20240221/pyfshfs/pyfshfs_file_object_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1868 2024-02-21 05:48:50.000000 libfshfs-20240221/pyfshfs/pyfshfs.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84670 2024-02-21 05:50:44.000000 libfshfs-20240221/pyfshfs/pyfshfs_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2024-02-21 05:48:50.000000 libfshfs-20240221/pyfshfs/pyfshfs_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8068 2024-02-21 05:50:44.000000 libfshfs-20240221/pyfshfs/pyfshfs_file_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1540 2024-02-21 05:48:50.000000 libfshfs-20240221/pyfshfs/pyfshfs_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9890 2024-02-21 05:50:44.000000 libfshfs-20240221/pyfshfs/pyfshfs_extended_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25360 2024-02-21 05:50:44.000000 libfshfs-20240221/pyfshfs/pyfshfs_data_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2033 2024-02-21 05:48:50.000000 libfshfs-20240221/pyfshfs/pyfshfs_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50335 2024-02-21 06:04:26.000000 libfshfs-20240221/pyfshfs/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-21 05:48:50.000000 libfshfs-20240221/pyfshfs/pyfshfs_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1826 2024-02-21 05:48:50.000000 libfshfs-20240221/pyfshfs/pyfshfs_datetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16397 2024-02-21 05:48:50.000000 libfshfs-20240221/pyfshfs/pyfshfs.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-02-21 05:48:50.000000 libfshfs-20240221/pyfshfs/pyfshfs_libfshfs.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2487 2024-02-21 05:48:50.000000 libfshfs-20240221/pyfshfs/pyfshfs_file_entries.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24510 2024-02-21 05:50:44.000000 libfshfs-20240221/pyfshfs/pyfshfs_volume.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-02-21 06:04:25.000000 libfshfs-20240221/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-02-21 06:04:25.000000 libfshfs-20240221/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-02-21 05:49:12.000000 libfshfs-20240221/msvscpp/libfdata/libfdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_tools_signal/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5951 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_tools_signal/fshfs_test_tools_signal.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_btree_node_descriptor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6051 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_btree_node_descriptor/fshfs_test_btree_node_descriptor.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/libfmos/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5663 2024-02-21 05:49:12.000000 libfshfs-20240221/msvscpp/libfmos/libfmos.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_tools_output/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5951 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_tools_output/fshfs_test_tools_output.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_file_record/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6021 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_file_record/fshfs_test_file_record.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/libfshfs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15318 2024-02-21 05:49:12.000000 libfshfs-20240221/msvscpp/libfshfs/libfshfs.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/zlib/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6068 2024-02-21 05:49:12.000000 libfshfs-20240221/msvscpp/zlib/zlib.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_thread_record/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6027 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_thread_record/fshfs_test_thread_record.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-02-21 05:49:12.000000 libfshfs-20240221/msvscpp/libfguid/libfguid.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-02-21 05:49:12.000000 libfshfs-20240221/msvscpp/libclocale/libclocale.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_file_system/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6021 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_file_system/fshfs_test_file_system.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_name/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6289 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_name/fshfs_test_name.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_io_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6015 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_io_handle/fshfs_test_io_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_directory_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6033 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_directory_entry/fshfs_test_directory_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-02-21 05:49:12.000000 libfshfs-20240221/msvscpp/libfcache/libfcache.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2809 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-02-21 05:49:12.000000 libfshfs-20240221/msvscpp/libbfio/libbfio.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/pyfshfs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7009 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/pyfshfs/pyfshfs.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfsmount/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7735 2024-02-21 05:49:12.000000 libfshfs-20240221/msvscpp/fshfsmount/fshfsmount.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_deflate/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5932 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_deflate/fshfs_test_deflate.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5844 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_notify/fshfs_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_compression/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6021 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_compression/fshfs_test_compression.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-02-21 05:49:12.000000 libfshfs-20240221/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5757 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_error/fshfs_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_fork_descriptor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6033 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_fork_descriptor/fshfs_test_fork_descriptor.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-02-21 05:49:12.000000 libfshfs-20240221/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_btree_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6024 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_btree_header/fshfs_test_btree_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfsinfo/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7348 2024-02-21 05:49:12.000000 libfshfs-20240221/msvscpp/fshfsinfo/fshfsinfo.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_master_directory_block/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6304 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_master_directory_block/fshfs_test_master_directory_block.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49808 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/libfshfs.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_btree_file/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6268 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_btree_file/fshfs_test_btree_file.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_huffman_tree/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6024 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_huffman_tree/fshfs_test_huffman_tree.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-02-21 05:49:12.000000 libfshfs-20240221/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_btree_node_record/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6039 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_btree_node_record/fshfs_test_btree_node_record.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_attributes_btree_key/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6048 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_attributes_btree_key/fshfs_test_attributes_btree_key.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_bit_stream/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6018 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_bit_stream/fshfs_test_bit_stream.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-02-21 05:49:12.000000 libfshfs-20240221/msvscpp/libcpath/libcpath.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_catalog_btree_key/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6039 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_catalog_btree_key/fshfs_test_catalog_btree_key.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_extents_btree_key/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6039 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_extents_btree_key/fshfs_test_extents_btree_key.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_compressed_data_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6137 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_compressed_data_handle/fshfs_test_compressed_data_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_extent/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6006 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_extent/fshfs_test_extent.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_directory_record/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6036 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_directory_record/fshfs_test_directory_record.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/libhmac/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5312 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/libhmac/libhmac.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-02-21 05:49:12.000000 libfshfs-20240221/msvscpp/libcsplit/libcsplit.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-02-21 05:49:12.000000 libfshfs-20240221/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26043 2024-02-21 06:04:26.000000 libfshfs-20240221/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_profiler/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6012 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_profiler/fshfs_test_profiler.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6672 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_support/fshfs_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_attribute_record/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6036 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_attribute_record/fshfs_test_attribute_record.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_btree_node/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6018 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_btree_node/fshfs_test_btree_node.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_volume/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6669 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_volume/fshfs_test_volume.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-02-21 05:49:12.000000 libfshfs-20240221/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_file_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6018 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_file_entry/fshfs_test_file_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_tools_info_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6276 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_tools_info_handle/fshfs_test_tools_info_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-02-21 05:49:12.000000 libfshfs-20240221/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-02-21 05:49:12.000000 libfshfs-20240221/msvscpp/libfdatetime/libfdatetime.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_volume_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6277 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_volume_header/fshfs_test_volume_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/msvscpp/fshfs_test_buffer_data_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6042 2024-02-21 05:50:08.000000 libfshfs-20240221/msvscpp/fshfs_test_buffer_data_handle/fshfs_test_buffer_data_handle.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       92 2024-02-21 05:48:49.000000 libfshfs-20240221/AUTHORS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:10.000000 libfshfs-20240221/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-21 06:03:59.000000 libfshfs-20240221/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-02-21 06:03:59.000000 libfshfs-20240221/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-21 06:03:59.000000 libfshfs-20240221/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-02-21 06:03:59.000000 libfshfs-20240221/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-02-21 06:03:59.000000 libfshfs-20240221/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-02-21 06:03:59.000000 libfshfs-20240221/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      942 2024-02-21 06:03:59.000000 libfshfs-20240221/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-02-21 06:03:59.000000 libfshfs-20240221/libcfile/libcfile_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-21 06:03:59.000000 libfshfs-20240221/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-02-21 06:03:59.000000 libfshfs-20240221/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-21 06:03:59.000000 libfshfs-20240221/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-02-21 06:03:59.000000 libfshfs-20240221/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-21 06:03:59.000000 libfshfs-20240221/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-21 06:03:59.000000 libfshfs-20240221/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-02-21 06:03:59.000000 libfshfs-20240221/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-21 06:03:59.000000 libfshfs-20240221/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-02-21 06:03:59.000000 libfshfs-20240221/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32033 2024-02-21 06:04:25.000000 libfshfs-20240221/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-21 06:03:59.000000 libfshfs-20240221/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-21 06:03:59.000000 libfshfs-20240221/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-02-21 06:03:59.000000 libfshfs-20240221/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-02-21 06:03:59.000000 libfshfs-20240221/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      971 2024-02-21 05:50:08.000000 libfshfs-20240221/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-02-21 06:04:25.000000 libfshfs-20240221/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:10.000000 libfshfs-20240221/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1127 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33717 2024-02-21 06:04:25.000000 libfshfs-20240221/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-21 06:03:57.000000 libfshfs-20240221/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-02-21 05:48:48.000000 libfshfs-20240221/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      487 2024-02-21 05:48:48.000000 libfshfs-20240221/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-02-21 06:04:25.000000 libfshfs-20240221/config.sub
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      770 2024-02-21 05:48:48.000000 libfshfs-20240221/libfshfs.pc.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-02-21 05:48:48.000000 libfshfs-20240221/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1508 2024-02-21 05:48:48.000000 libfshfs-20240221/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:06:45.000000 libfshfs-20240221/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:10.000000 libfshfs-20240221/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-02-21 06:04:05.000000 libfshfs-20240221/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-02-21 06:04:05.000000 libfshfs-20240221/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-02-21 06:04:05.000000 libfshfs-20240221/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-02-21 06:04:05.000000 libfshfs-20240221/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-02-21 06:04:05.000000 libfshfs-20240221/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-02-21 06:04:05.000000 libfshfs-20240221/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-21 06:04:05.000000 libfshfs-20240221/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-02-21 06:04:05.000000 libfshfs-20240221/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-02-21 06:04:05.000000 libfshfs-20240221/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-02-21 06:04:05.000000 libfshfs-20240221/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-02-21 06:04:05.000000 libfshfs-20240221/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-02-21 06:04:05.000000 libfshfs-20240221/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-02-21 06:04:05.000000 libfshfs-20240221/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-02-21 06:04:05.000000 libfshfs-20240221/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-02-21 06:04:05.000000 libfshfs-20240221/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-02-21 06:04:05.000000 libfshfs-20240221/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-02-21 06:04:05.000000 libfshfs-20240221/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-02-21 06:04:05.000000 libfshfs-20240221/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-02-21 06:04:05.000000 libfshfs-20240221/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-02-21 06:04:05.000000 libfshfs-20240221/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-21 06:04:05.000000 libfshfs-20240221/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-02-21 06:04:05.000000 libfshfs-20240221/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-02-21 06:04:05.000000 libfshfs-20240221/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-02-21 06:04:05.000000 libfshfs-20240221/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-02-21 06:04:05.000000 libfshfs-20240221/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-02-21 06:04:05.000000 libfshfs-20240221/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-02-21 06:04:05.000000 libfshfs-20240221/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34123 2024-02-21 06:04:26.000000 libfshfs-20240221/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-02-21 06:04:05.000000 libfshfs-20240221/libcthreads/libcthreads_queue.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-02-21 06:04:26.000000 libfshfs-20240221/test-driver
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:10.000000 libfshfs-20240221/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-02-21 06:04:03.000000 libfshfs-20240221/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-21 06:04:03.000000 libfshfs-20240221/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-02-21 06:04:03.000000 libfshfs-20240221/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      842 2024-02-21 06:04:03.000000 libfshfs-20240221/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-21 06:04:03.000000 libfshfs-20240221/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-21 06:04:03.000000 libfshfs-20240221/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-21 06:04:03.000000 libfshfs-20240221/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-02-21 06:04:03.000000 libfshfs-20240221/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-02-21 06:04:03.000000 libfshfs-20240221/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-02-21 06:04:03.000000 libfshfs-20240221/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-21 06:04:03.000000 libfshfs-20240221/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-21 06:04:03.000000 libfshfs-20240221/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31311 2024-02-21 06:04:25.000000 libfshfs-20240221/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-21 06:04:03.000000 libfshfs-20240221/libcpath/libcpath_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-21 06:04:03.000000 libfshfs-20240221/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-02-21 06:04:03.000000 libfshfs-20240221/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-02-21 06:04:03.000000 libfshfs-20240221/libcpath/libcpath_path.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1912 2023-12-03 09:06:45.000000 libfshfs-20240221/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1989 2024-02-21 05:48:50.000000 libfshfs-20240221/manuals/fshfsinfo.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      190 2023-12-03 09:06:54.000000 libfshfs-20240221/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15268 2024-02-21 05:48:50.000000 libfshfs-20240221/manuals/libfshfs.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-21 05:48:50.000000 libfshfs-20240221/manuals/fshfsmount.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28268 2024-02-21 06:04:26.000000 libfshfs-20240221/manuals/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/tests/
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3348 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/test_fshfsinfo.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29883 2024-02-21 05:50:08.000000 libfshfs-20240221/tests/fshfs_test_directory_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1704 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15297 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_btree_node_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4323 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12439 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_compression.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39762 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_unicode_case_folding_mappings.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6139 2024-02-21 05:50:08.000000 libfshfs-20240221/tests/fshfs_test_file_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8954 2024-02-21 05:50:08.000000 libfshfs-20240221/tests/fshfs_test_btree_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5877 2024-02-21 05:50:08.000000 libfshfs-20240221/tests/fshfs_test_extent.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32976 2024-02-21 05:50:08.000000 libfshfs-20240221/tests/fshfs_test_file_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4700 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1709 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_libbfio.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4076 2024-02-21 05:50:44.000000 libfshfs-20240221/tests/test_tools.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15726 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_functions.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)  1117748 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_unicode_decomposition_mappings.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9757 2024-02-21 05:50:08.000000 libfshfs-20240221/tests/fshfs_test_attributes_btree_key.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8574 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17397 2024-02-21 05:50:08.000000 libfshfs-20240221/tests/fshfs_test_master_directory_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3464 2024-02-21 05:50:44.000000 libfshfs-20240221/tests/pyfshfs_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14000 2024-02-21 05:50:08.000000 libfshfs-20240221/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6750 2024-02-21 05:50:08.000000 libfshfs-20240221/tests/fshfs_test_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9259 2024-02-21 05:50:08.000000 libfshfs-20240221/tests/fshfs_test_thread_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11979 2024-02-21 05:50:08.000000 libfshfs-20240221/tests/fshfs_test_fork_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9484 2024-02-21 05:50:08.000000 libfshfs-20240221/tests/fshfs_test_extents_btree_key.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4086 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13779 2024-02-21 05:50:08.000000 libfshfs-20240221/tests/fshfs_test_bit_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18385 2024-02-21 05:50:08.000000 libfshfs-20240221/tests/fshfs_test_attribute_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17738 2024-02-21 05:50:08.000000 libfshfs-20240221/tests/fshfs_test_buffer_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1997 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_functions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4169 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_tools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10871 2024-02-21 05:50:08.000000 libfshfs-20240221/tests/fshfs_test_catalog_btree_key.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100638 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_deflate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30822 2024-02-21 05:50:08.000000 libfshfs-20240221/tests/fshfs_test_huffman_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9202 2024-02-21 05:50:44.000000 libfshfs-20240221/tests/pyfshfs_test_volume.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5706 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_tools_info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2447 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_tools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35448 2024-02-21 05:50:08.000000 libfshfs-20240221/tests/fshfs_test_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9474 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_btree_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_libfshfs.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4740 2024-02-21 05:50:08.000000 libfshfs-20240221/tests/fshfs_test_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3139 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19381 2024-02-21 05:50:08.000000 libfshfs-20240221/tests/fshfs_test_volume_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7050 2024-02-21 05:50:08.000000 libfshfs-20240221/tests/fshfs_test_profiler.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    88705 2024-02-21 06:04:26.000000 libfshfs-20240221/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6532 2024-02-21 05:50:08.000000 libfshfs-20240221/tests/fshfs_test_btree_node_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21042 2024-02-21 05:50:08.000000 libfshfs-20240221/tests/fshfs_test_compressed_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8056 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_io_handle.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4476 2024-02-21 05:50:44.000000 libfshfs-20240221/tests/test_library.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40566 2024-02-21 05:50:08.000000 libfshfs-20240221/tests/fshfs_test_directory_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32805 2024-02-21 05:48:50.000000 libfshfs-20240221/tests/fshfs_test_name.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2503 2024-02-21 05:48:50.000000 libfshfs-20240221/ossfuzz/volume_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2024 2023-12-03 09:06:47.000000 libfshfs-20240221/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-02-21 05:48:50.000000 libfshfs-20240221/ossfuzz/ossfuzz_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5686 2024-02-21 05:48:50.000000 libfshfs-20240221/ossfuzz/file_entry_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3320 2024-02-21 05:48:50.000000 libfshfs-20240221/ossfuzz/extended_attribute_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      972 2024-02-21 05:48:50.000000 libfshfs-20240221/ossfuzz/ossfuzz_libfshfs.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37621 2024-02-21 06:04:26.000000 libfshfs-20240221/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-02-21 06:04:20.000000 libfshfs-20240221/ltmain.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2487 2024-02-21 06:04:37.000000 libfshfs-20240221/libfshfs.spec
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/libhmac/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47989 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_sha1_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_sha224.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50026 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_sha512_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14448 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_md5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2079 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_md5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1942 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9362 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14650 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_sha512.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45648 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_sha256_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_sha224.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1623 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2060 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_sha1.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3443 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_sha256_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1121 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45605 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_sha224_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_md5_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_sha256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3368 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_sha1_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33843 2024-02-21 06:04:26.000000 libfshfs-20240221/libhmac/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_sha256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3461 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_sha224_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3444 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_sha512_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_sha512.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14514 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_sha1.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40596 2024-02-21 06:04:12.000000 libfshfs-20240221/libhmac/libhmac_md5_context.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:10.000000 libfshfs-20240221/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-02-21 06:04:04.000000 libfshfs-20240221/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-02-21 06:04:04.000000 libfshfs-20240221/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-02-21 06:04:04.000000 libfshfs-20240221/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-02-21 06:04:04.000000 libfshfs-20240221/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-21 06:04:04.000000 libfshfs-20240221/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      884 2024-02-21 06:04:04.000000 libfshfs-20240221/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-21 06:04:04.000000 libfshfs-20240221/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-02-21 06:04:04.000000 libfshfs-20240221/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-21 06:04:04.000000 libfshfs-20240221/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-02-21 06:04:04.000000 libfshfs-20240221/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-21 06:04:04.000000 libfshfs-20240221/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-02-21 06:04:04.000000 libfshfs-20240221/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-21 06:04:04.000000 libfshfs-20240221/libcsplit/libcsplit_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-21 06:04:04.000000 libfshfs-20240221/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-21 06:04:04.000000 libfshfs-20240221/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-02-21 06:04:04.000000 libfshfs-20240221/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32091 2024-02-21 06:04:25.000000 libfshfs-20240221/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-02-21 06:04:04.000000 libfshfs-20240221/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-02-21 06:04:04.000000 libfshfs-20240221/libcsplit/libcsplit_narrow_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:06:54.000000 libfshfs-20240221/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:06:54.000000 libfshfs-20240221/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:06:54.000000 libfshfs-20240221/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:06:54.000000 libfshfs-20240221/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:06:54.000000 libfshfs-20240221/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:06:54.000000 libfshfs-20240221/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:06:54.000000 libfshfs-20240221/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:06:54.000000 libfshfs-20240221/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:06:54.000000 libfshfs-20240221/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1854 2024-02-21 06:04:37.000000 libfshfs-20240221/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:06:54.000000 libfshfs-20240221/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:06:54.000000 libfshfs-20240221/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:10.000000 libfshfs-20240221/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4197 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    54835 2024-02-21 06:04:26.000000 libfshfs-20240221/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-02-21 06:04:15.000000 libfshfs-20240221/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42403 2024-02-21 06:04:25.000000 libfshfs-20240221/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:10.000000 libfshfs-20240221/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-21 06:04:02.000000 libfshfs-20240221/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-21 06:04:02.000000 libfshfs-20240221/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-02-21 06:04:02.000000 libfshfs-20240221/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-02-21 06:04:02.000000 libfshfs-20240221/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-02-21 06:04:02.000000 libfshfs-20240221/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-21 06:04:02.000000 libfshfs-20240221/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-02-21 06:04:02.000000 libfshfs-20240221/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-02-21 06:04:02.000000 libfshfs-20240221/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-02-21 06:04:02.000000 libfshfs-20240221/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-02-21 06:04:02.000000 libfshfs-20240221/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-02-21 06:04:02.000000 libfshfs-20240221/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31145 2024-02-21 06:04:25.000000 libfshfs-20240221/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-02-21 06:04:02.000000 libfshfs-20240221/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-02-21 06:04:02.000000 libfshfs-20240221/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:10.000000 libfshfs-20240221/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-02-21 06:03:58.000000 libfshfs-20240221/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-02-21 06:03:58.000000 libfshfs-20240221/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-21 06:03:58.000000 libfshfs-20240221/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-02-21 06:03:58.000000 libfshfs-20240221/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-02-21 06:03:58.000000 libfshfs-20240221/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-21 06:03:58.000000 libfshfs-20240221/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-02-21 06:03:58.000000 libfshfs-20240221/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-02-21 06:03:58.000000 libfshfs-20240221/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-02-21 06:03:58.000000 libfshfs-20240221/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-21 06:03:58.000000 libfshfs-20240221/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-21 06:03:58.000000 libfshfs-20240221/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30658 2024-02-21 06:04:25.000000 libfshfs-20240221/libcerror/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3619 2024-02-21 05:48:48.000000 libfshfs-20240221/libfshfs.spec.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:11.000000 libfshfs-20240221/fshfstools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1443 2024-02-21 05:48:50.000000 libfshfs-20240221/fshfstools/fshfstools_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1483 2024-02-21 05:48:50.000000 libfshfs-20240221/fshfstools/fshfstools_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4361 2024-02-21 05:48:50.000000 libfshfs-20240221/fshfstools/fshfstools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37213 2024-02-21 05:50:44.000000 libfshfs-20240221/fshfstools/mount_dokan.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3061 2024-02-21 05:50:44.000000 libfshfs-20240221/fshfstools/mount_file_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1213 2024-02-21 05:48:50.000000 libfshfs-20240221/fshfstools/fshfstools_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38773 2024-02-21 05:50:44.000000 libfshfs-20240221/fshfstools/mount_fuse.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4584 2024-02-21 05:50:44.000000 libfshfs-20240221/fshfstools/info_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5417 2024-02-21 05:48:50.000000 libfshfs-20240221/fshfstools/mount_dokan.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1474 2024-02-21 05:48:50.000000 libfshfs-20240221/fshfstools/fshfstools_libhmac.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3297 2024-02-21 05:48:50.000000 libfshfs-20240221/fshfstools/digest_hash.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30757 2024-02-21 05:50:44.000000 libfshfs-20240221/fshfstools/mount_file_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-02-21 05:48:50.000000 libfshfs-20240221/fshfstools/fshfstools_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2583 2023-12-03 09:06:51.000000 libfshfs-20240221/fshfstools/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1781 2024-02-21 05:48:50.000000 libfshfs-20240221/fshfstools/fshfstools_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1409 2024-02-21 05:48:50.000000 libfshfs-20240221/fshfstools/fshfstools_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25597 2024-02-21 05:50:44.000000 libfshfs-20240221/fshfstools/mount_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-02-21 05:48:50.000000 libfshfs-20240221/fshfstools/fshfstools_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70646 2024-02-21 05:50:44.000000 libfshfs-20240221/fshfstools/info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3822 2024-02-21 05:50:44.000000 libfshfs-20240221/fshfstools/mount_file_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1590 2024-02-21 05:48:50.000000 libfshfs-20240221/fshfstools/fshfstools_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3324 2024-02-21 05:50:44.000000 libfshfs-20240221/fshfstools/mount_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-02-21 05:48:50.000000 libfshfs-20240221/fshfstools/fshfstools_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-02-21 05:48:50.000000 libfshfs-20240221/fshfstools/fshfstools_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10890 2024-02-21 05:50:44.000000 libfshfs-20240221/fshfstools/fshfsinfo.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5751 2024-02-21 05:48:50.000000 libfshfs-20240221/fshfstools/fshfstools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-02-21 05:48:50.000000 libfshfs-20240221/fshfstools/fshfstools_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19354 2024-02-21 05:50:44.000000 libfshfs-20240221/fshfstools/mount_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-02-21 05:48:50.000000 libfshfs-20240221/fshfstools/fshfstools_libfshfs.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1771 2024-02-21 05:48:50.000000 libfshfs-20240221/fshfstools/fshfstools_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15501 2024-02-21 05:50:44.000000 libfshfs-20240221/fshfstools/fshfsmount.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1486 2024-02-21 05:48:50.000000 libfshfs-20240221/fshfstools/fshfstools_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35881 2024-02-21 06:04:25.000000 libfshfs-20240221/fshfstools/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1761 2024-02-21 05:48:50.000000 libfshfs-20240221/fshfstools/fshfstools_signal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1244 2024-02-21 05:48:50.000000 libfshfs-20240221/fshfstools/digest_hash.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-21 05:48:50.000000 libfshfs-20240221/fshfstools/fshfstools_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1472 2024-02-21 05:48:50.000000 libfshfs-20240221/fshfstools/fshfstools_output.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3050 2024-02-21 05:50:44.000000 libfshfs-20240221/fshfstools/mount_fuse.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-21 06:20:10.000000 libfshfs-20240221/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-02-21 06:04:09.000000 libfshfs-20240221/libfdatetime/libfdatetime_floatingtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-02-21 06:04:09.000000 libfshfs-20240221/libfdatetime/libfdatetime_nsf_timedate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-02-21 06:04:09.000000 libfshfs-20240221/libfdatetime/libfdatetime_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-02-21 06:04:09.000000 libfshfs-20240221/libfdatetime/libfdatetime_floatingtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-02-21 06:04:09.000000 libfshfs-20240221/libfdatetime/libfdatetime_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-02-21 06:04:09.000000 libfshfs-20240221/libfdatetime/libfdatetime_hfs_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-02-21 06:04:09.000000 libfshfs-20240221/libfdatetime/libfdatetime_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-02-21 06:04:09.000000 libfshfs-20240221/libfdatetime/libfdatetime_hfs_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1148 2024-02-21 06:04:09.000000 libfshfs-20240221/libfdatetime/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-02-21 06:04:09.000000 libfshfs-20240221/libfdatetime/libfdatetime_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-02-21 06:04:09.000000 libfshfs-20240221/libfdatetime/libfdatetime_systemtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-21 06:04:09.000000 libfshfs-20240221/libfdatetime/libfdatetime_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-02-21 06:04:09.000000 libfshfs-20240221/libfdatetime/libfdatetime_posix_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-02-21 06:04:09.000000 libfshfs-20240221/libfdatetime/libfdatetime_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-02-21 06:04:09.000000 libfshfs-20240221/libfdatetime/libfdatetime_fat_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-02-21 06:04:09.000000 libfshfs-20240221/libfdatetime/libfdatetime_systemtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-02-21 06:04:09.000000 libfshfs-20240221/libfdatetime/libfdatetime_nsf_timedate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-02-21 06:04:09.000000 libfshfs-20240221/libfdatetime/libfdatetime_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-02-21 06:04:09.000000 libfshfs-20240221/libfdatetime/libfdatetime_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-02-21 06:04:09.000000 libfshfs-20240221/libfdatetime/libfdatetime_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-02-21 06:04:09.000000 libfshfs-20240221/libfdatetime/libfdatetime_posix_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-02-21 06:04:09.000000 libfshfs-20240221/libfdatetime/libfdatetime_date_time_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-02-21 06:04:09.000000 libfshfs-20240221/libfdatetime/libfdatetime_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-02-21 06:04:09.000000 libfshfs-20240221/libfdatetime/libfdatetime_date_time_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-02-21 06:04:09.000000 libfshfs-20240221/libfdatetime/libfdatetime_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33884 2024-02-21 06:04:26.000000 libfshfs-20240221/libfdatetime/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-02-21 06:04:09.000000 libfshfs-20240221/libfdatetime/libfdatetime_fat_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56937 2024-02-21 06:04:22.000000 libfshfs-20240221/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8495 2024-02-21 05:48:48.000000 libfshfs-20240221/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      418 2024-02-21 06:20:12.603716 libfshfs-20240221/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:10.000000 libfshfs-20240501/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_area.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_mapped_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1287 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_area.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_mapped_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_segments_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_segments_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35118 2024-05-01 07:34:35.000000 libfshfs-20240501/libfdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-05-01 07:34:12.000000 libfshfs-20240501/libfdata/libfdata_vector.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:11.000000 libfshfs-20240501/libfmos/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2023 2024-05-01 07:34:18.000000 libfshfs-20240501/libfmos/libfmos_lzfse_bit_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2269 2024-05-01 07:34:18.000000 libfshfs-20240501/libfmos/libfmos_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2964 2024-05-01 07:34:18.000000 libfshfs-20240501/libfmos/libfmos_lzfse_decoder.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2024-05-01 07:34:18.000000 libfshfs-20240501/libfmos/libfmos_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7799 2024-05-01 07:34:18.000000 libfshfs-20240501/libfmos/libfmos_adc.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3441 2024-05-01 07:34:18.000000 libfshfs-20240501/libfmos/libfmos_lzfse.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-05-01 07:34:18.000000 libfshfs-20240501/libfmos/libfmos_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1321 2024-05-01 07:34:18.000000 libfshfs-20240501/libfmos/libfmos_adc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-05-01 07:34:18.000000 libfshfs-20240501/libfmos/libfmos_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-01 07:34:18.000000 libfshfs-20240501/libfmos/libfmos_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-05-01 07:34:18.000000 libfshfs-20240501/libfmos/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-01 07:34:18.000000 libfshfs-20240501/libfmos/libfmos_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25840 2024-05-01 07:34:18.000000 libfshfs-20240501/libfmos/libfmos_lzvn.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-05-01 07:34:18.000000 libfshfs-20240501/libfmos/libfmos_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6380 2024-05-01 07:34:18.000000 libfshfs-20240501/libfmos/libfmos_lzfse_bit_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3271 2024-05-01 07:34:18.000000 libfshfs-20240501/libfmos/libfmos_lzfse_decoder.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-01 07:34:18.000000 libfshfs-20240501/libfmos/libfmos_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    60280 2024-05-01 07:34:18.000000 libfshfs-20240501/libfmos/libfmos_lzfse.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-05-01 07:34:18.000000 libfshfs-20240501/libfmos/libfmos_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-01 07:34:18.000000 libfshfs-20240501/libfmos/libfmos_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-05-01 07:34:18.000000 libfshfs-20240501/libfmos/libfmos_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1326 2024-05-01 07:34:18.000000 libfshfs-20240501/libfmos/libfmos_lzvn.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-01 07:34:18.000000 libfshfs-20240501/libfmos/libfmos_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32840 2024-05-01 07:34:35.000000 libfshfs-20240501/libfmos/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-05-01 06:57:17.000000 libfshfs-20240501/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-05-01 07:34:34.000000 libfshfs-20240501/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 06:57:17.000000 libfshfs-20240501/NEWS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:11.000000 libfshfs-20240501/libfshfs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13516 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_btree_node_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2004 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_btree_node_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21335 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_extents_btree_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40326 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_file_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4581 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_block_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3591 2024-05-01 06:57:21.000000 libfshfs-20240501/libfshfs/libfshfs_attribute_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1090 2024-05-01 07:34:50.000000 libfshfs-20240501/libfshfs/libfshfs.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31797 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_compressed_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2393 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_fork_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2857 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13183 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_file_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2094 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_huffman_tree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5206 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1398 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48205 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_directory_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21037 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_data_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28435 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_directory_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4979 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_file_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12883 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_btree_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6027 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_compressed_data_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3817 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_btree_node_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12308 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_thread_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22767 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1357 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_extents_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2280 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_bit_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9194 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_catalog_btree_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9595 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24114 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_master_directory_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1833 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_btree_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11422 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_fork_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48738 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_deflate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2321 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_btree_node_vector.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7276 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_extents_btree_key.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3002 2024-05-01 06:57:21.000000 libfshfs-20240501/libfshfs/fshfs_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19641 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_volume_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1836 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_btree_node_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4336 2024-05-01 07:11:14.000000 libfshfs-20240501/libfshfs/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3306 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_compressed_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4235 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_btree_node_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2830 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_catalog_btree_key.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5401 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4233 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_directory_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5723 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_directory_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2119 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_profiler.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1478 2024-05-01 06:57:21.000000 libfshfs-20240501/libfshfs/fshfs_compressed_data.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6809 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_btree_node_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5295 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_extent.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10716 2024-05-01 06:57:21.000000 libfshfs-20240501/libfshfs/fshfs_catalog_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14066 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_catalog_btree_key.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   147422 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4690 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35932 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_extended_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1792 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1726 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2841 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_attributes_btree_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2495 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_volume_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1868 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_thread_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15010 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_name.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2802 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_extents_btree_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_block_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2449 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_attributes_btree_key.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   240954 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_name.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_extent.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   106513 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_catalog_btree_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3488 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_deflate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4078 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_extents_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1594 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_btree_node_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1924 2024-05-01 06:57:21.000000 libfshfs-20240501/libfshfs/fshfs_attributes_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1987 2024-05-01 06:57:21.000000 libfshfs-20240501/libfshfs/fshfs_extents_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2036 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52766 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3699 2024-05-01 06:57:21.000000 libfshfs-20240501/libfshfs/fshfs_volume_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1327 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_compression.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8113 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_btree_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3304 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_master_directory_block.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36176 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_file_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16909 2024-05-01 06:57:21.000000 libfshfs-20240501/libfshfs/libfshfs_allocation_block_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4169 2024-05-01 06:57:21.000000 libfshfs-20240501/libfshfs/fshfs_master_directory_block.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9705 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_compression.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5073 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_extended_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4688 2024-05-01 07:34:50.000000 libfshfs-20240501/libfshfs/libfshfs_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-05-01 06:57:21.000000 libfshfs-20240501/libfshfs/libfshfs_allocation_block_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20986 2024-05-01 06:57:21.000000 libfshfs-20240501/libfshfs/libfshfs_attribute_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1092 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7930 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_bit_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2593 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_btree_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10859 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_attributes_btree_key.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6090 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_file_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2328 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_buffer_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48355 2024-05-01 07:34:35.000000 libfshfs-20240501/libfshfs/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3716 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_data_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20152 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20259 2024-05-01 06:57:21.000000 libfshfs-20240501/libfshfs/libfshfs_attributes_btree_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1886 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_compressed_data_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_libfmos.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1955 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_extents_btree_key.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12520 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_huffman_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7821 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_buffer_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8243 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs_profiler.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1835 2024-05-01 06:57:22.000000 libfshfs-20240501/libfshfs/libfshfs.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1514 2024-05-01 06:57:21.000000 libfshfs-20240501/libfshfs/fshfs_fork_descriptor.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-05-01 07:34:35.000000 libfshfs-20240501/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:11.000000 libfshfs-20240501/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-01 07:34:16.000000 libfshfs-20240501/libfguid/libfguid_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-05-01 07:34:16.000000 libfshfs-20240501/libfguid/libfguid_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-05-01 07:34:16.000000 libfshfs-20240501/libfguid/libfguid_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-01 07:34:16.000000 libfshfs-20240501/libfguid/libfguid_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      677 2024-05-01 07:34:16.000000 libfshfs-20240501/libfguid/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-01 07:34:16.000000 libfshfs-20240501/libfguid/libfguid_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-01 07:34:16.000000 libfshfs-20240501/libfguid/libfguid_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-05-01 07:34:16.000000 libfshfs-20240501/libfguid/libfguid_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-05-01 07:34:16.000000 libfshfs-20240501/libfguid/libfguid_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-05-01 07:34:16.000000 libfshfs-20240501/libfguid/libfguid_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-05-01 07:34:16.000000 libfshfs-20240501/libfguid/libfguid_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30919 2024-05-01 07:34:35.000000 libfshfs-20240501/libfguid/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-01 07:34:16.000000 libfshfs-20240501/libfguid/libfguid_error.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:09.000000 libfshfs-20240501/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11734 2024-05-01 06:57:25.000000 libfshfs-20240501/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4659 2024-05-01 06:57:25.000000 libfshfs-20240501/m4/libfmos.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18489 2024-05-01 06:57:25.000000 libfshfs-20240501/m4/libfdatetime.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:06:54.000000 libfshfs-20240501/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9615 2024-05-01 06:57:25.000000 libfshfs-20240501/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:06:54.000000 libfshfs-20240501/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:06:54.000000 libfshfs-20240501/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-05-01 06:57:25.000000 libfshfs-20240501/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:06:54.000000 libfshfs-20240501/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:06:54.000000 libfshfs-20240501/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-05-01 06:57:24.000000 libfshfs-20240501/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-05-01 06:57:24.000000 libfshfs-20240501/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7625 2024-05-01 06:57:24.000000 libfshfs-20240501/m4/libcsplit.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-05-01 06:57:24.000000 libfshfs-20240501/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-05-01 06:57:24.000000 libfshfs-20240501/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-05-01 07:34:29.000000 libfshfs-20240501/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-05-01 07:34:29.000000 libfshfs-20240501/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15781 2024-05-01 06:57:25.000000 libfshfs-20240501/m4/libfdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:06:54.000000 libfshfs-20240501/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7058 2024-05-01 06:57:25.000000 libfshfs-20240501/m4/libfuse.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-05-01 07:34:28.000000 libfshfs-20240501/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:06:54.000000 libfshfs-20240501/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-05-01 06:57:24.000000 libfshfs-20240501/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-05-01 06:57:24.000000 libfshfs-20240501/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5876 2024-05-01 06:57:25.000000 libfshfs-20240501/m4/libfguid.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11923 2024-05-01 06:57:25.000000 libfshfs-20240501/m4/libbfio.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8550 2024-05-01 06:57:25.000000 libfshfs-20240501/m4/libhmac.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:06:54.000000 libfshfs-20240501/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-05-01 07:34:29.000000 libfshfs-20240501/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:06:54.000000 libfshfs-20240501/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:06:54.000000 libfshfs-20240501/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-05-01 07:34:29.000000 libfshfs-20240501/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:06:54.000000 libfshfs-20240501/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-05-01 06:57:24.000000 libfshfs-20240501/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27647 2024-05-01 06:57:24.000000 libfshfs-20240501/m4/libcrypto.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:06:54.000000 libfshfs-20240501/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7566 2024-05-01 06:57:25.000000 libfshfs-20240501/m4/libfcache.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-05-01 06:57:24.000000 libfshfs-20240501/m4/pthread.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7819 2024-05-01 06:57:24.000000 libfshfs-20240501/m4/zlib.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:09.000000 libfshfs-20240501/include/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:09.000000 libfshfs-20240501/include/libfshfs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2308 2024-05-01 06:57:20.000000 libfshfs-20240501/include/libfshfs/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2306 2024-05-01 07:34:50.000000 libfshfs-20240501/include/libfshfs/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5073 2024-05-01 06:57:20.000000 libfshfs-20240501/include/libfshfs/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4942 2024-05-01 07:34:50.000000 libfshfs-20240501/include/libfshfs/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-01 06:57:20.000000 libfshfs-20240501/include/libfshfs/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2024-05-01 06:57:20.000000 libfshfs-20240501/include/libfshfs/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-01 06:57:20.000000 libfshfs-20240501/include/libfshfs/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1487 2024-05-01 07:34:50.000000 libfshfs-20240501/include/libfshfs/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5306 2024-05-01 06:57:20.000000 libfshfs-20240501/include/libfshfs/codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      425 2024-05-01 07:10:07.000000 libfshfs-20240501/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31635 2024-05-01 07:34:50.000000 libfshfs-20240501/include/libfshfs.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31635 2024-05-01 06:57:20.000000 libfshfs-20240501/include/libfshfs.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29295 2024-05-01 07:34:34.000000 libfshfs-20240501/include/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:09.000000 libfshfs-20240501/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-05-01 06:57:20.000000 libfshfs-20240501/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-05-01 06:57:20.000000 libfshfs-20240501/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-05-01 06:57:20.000000 libfshfs-20240501/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-05-01 06:57:20.000000 libfshfs-20240501/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-01 06:57:20.000000 libfshfs-20240501/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-05-01 06:57:20.000000 libfshfs-20240501/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-05-01 06:57:20.000000 libfshfs-20240501/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-05-01 07:10:07.000000 libfshfs-20240501/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-05-01 06:57:20.000000 libfshfs-20240501/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7374 2024-05-01 07:34:50.000000 libfshfs-20240501/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18487 2024-05-01 07:34:34.000000 libfshfs-20240501/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2024-05-01 07:34:50.000000 libfshfs-20240501/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-05-01 06:57:20.000000 libfshfs-20240501/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-05-01 06:57:20.000000 libfshfs-20240501/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-05-01 06:57:20.000000 libfshfs-20240501/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26329 2024-05-01 07:34:34.000000 libfshfs-20240501/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:10.000000 libfshfs-20240501/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-05-01 07:33:59.000000 libfshfs-20240501/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-05-01 07:33:59.000000 libfshfs-20240501/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-05-01 07:33:59.000000 libfshfs-20240501/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-05-01 07:33:59.000000 libfshfs-20240501/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-01 07:33:59.000000 libfshfs-20240501/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-01 07:33:59.000000 libfshfs-20240501/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-05-01 07:33:59.000000 libfshfs-20240501/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-05-01 07:33:59.000000 libfshfs-20240501/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-05-01 07:33:59.000000 libfshfs-20240501/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-05-01 07:33:59.000000 libfshfs-20240501/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31527 2024-05-01 07:34:35.000000 libfshfs-20240501/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-01 07:33:59.000000 libfshfs-20240501/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-05-01 07:33:59.000000 libfshfs-20240501/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-05-01 07:33:59.000000 libfshfs-20240501/libclocale/libclocale_codepage.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:10.000000 libfshfs-20240501/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-01 07:34:10.000000 libfshfs-20240501/libfcache/libfcache_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-05-01 07:34:10.000000 libfshfs-20240501/libfcache/libfcache_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-05-01 07:34:10.000000 libfshfs-20240501/libfcache/libfcache_cache_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-01 07:34:10.000000 libfshfs-20240501/libfcache/libfcache_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      876 2024-05-01 07:34:10.000000 libfshfs-20240501/libfcache/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-01 07:34:10.000000 libfshfs-20240501/libfcache/libfcache_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-01 07:34:10.000000 libfshfs-20240501/libfcache/libfcache_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-05-01 07:34:10.000000 libfshfs-20240501/libfcache/libfcache_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-05-01 07:34:10.000000 libfshfs-20240501/libfcache/libfcache_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-01 07:34:10.000000 libfshfs-20240501/libfcache/libfcache_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-01 07:34:10.000000 libfshfs-20240501/libfcache/libfcache_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-05-01 07:34:10.000000 libfshfs-20240501/libfcache/libfcache_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-01 07:34:10.000000 libfshfs-20240501/libfcache/libfcache_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-05-01 07:34:10.000000 libfshfs-20240501/libfcache/libfcache_cache_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32036 2024-05-01 07:34:35.000000 libfshfs-20240501/libfcache/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-01 07:34:10.000000 libfshfs-20240501/libfcache/libfcache_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-05-01 07:34:10.000000 libfshfs-20240501/libfcache/libfcache_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-05-01 07:34:10.000000 libfshfs-20240501/libfcache/libfcache_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2173 2024-05-01 07:11:48.000000 libfshfs-20240501/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:10.000000 libfshfs-20240501/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_file_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_file_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_file_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_file_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_file_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_file_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_memory_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_file_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_file_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_memory_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_memory_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35379 2024-05-01 07:34:34.000000 libfshfs-20240501/libbfio/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_memory_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-05-01 07:33:52.000000 libfshfs-20240501/libbfio/libbfio_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:06:45.000000 libfshfs-20240501/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-05-01 07:34:34.000000 libfshfs-20240501/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:09.000000 libfshfs-20240501/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1026 2024-05-01 06:57:24.000000 libfshfs-20240501/dpkg/copyright
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:09.000000 libfshfs-20240501/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-05-01 06:57:17.000000 libfshfs-20240501/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2173 2024-05-01 06:57:17.000000 libfshfs-20240501/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      769 2024-05-01 06:57:17.000000 libfshfs-20240501/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      121 2024-05-01 06:57:17.000000 libfshfs-20240501/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2024-05-01 07:34:50.000000 libfshfs-20240501/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-05-01 06:57:17.000000 libfshfs-20240501/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-05-01 06:57:17.000000 libfshfs-20240501/dpkg/libfshfs-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-05-01 06:57:17.000000 libfshfs-20240501/dpkg/libfshfs-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-05-01 06:57:17.000000 libfshfs-20240501/dpkg/libfshfs.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-05-01 06:57:17.000000 libfshfs-20240501/dpkg/libfshfs-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      486 2024-05-01 07:34:50.000000 libfshfs-20240501/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-05-01 06:57:17.000000 libfshfs-20240501/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  2011903 2024-05-01 07:34:33.000000 libfshfs-20240501/configure
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:11.000000 libfshfs-20240501/pyfshfs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16609 2024-05-01 06:57:22.000000 libfshfs-20240501/pyfshfs/pyfshfs_datetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2740 2024-05-01 06:58:50.000000 libfshfs-20240501/pyfshfs/pyfshfs_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2634 2024-05-01 06:57:22.000000 libfshfs-20240501/pyfshfs/pyfshfs_extended_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3486 2024-05-01 06:58:50.000000 libfshfs-20240501/pyfshfs/pyfshfs_extended_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8876 2024-05-01 06:57:22.000000 libfshfs-20240501/pyfshfs/pyfshfs_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9439 2024-05-01 06:57:22.000000 libfshfs-20240501/pyfshfs/pyfshfs_file_entries.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3020 2024-05-01 06:58:50.000000 libfshfs-20240501/pyfshfs/pyfshfs_data_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4118 2024-05-01 06:57:22.000000 libfshfs-20240501/pyfshfs/pyfshfs_file_object_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1525 2024-05-01 06:57:22.000000 libfshfs-20240501/pyfshfs/pyfshfs_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1358 2024-05-01 07:11:00.000000 libfshfs-20240501/pyfshfs/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9546 2024-05-01 06:57:22.000000 libfshfs-20240501/pyfshfs/pyfshfs_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28411 2024-05-01 06:58:50.000000 libfshfs-20240501/pyfshfs/pyfshfs_extended_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-01 06:57:22.000000 libfshfs-20240501/pyfshfs/pyfshfs_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33880 2024-05-01 06:57:22.000000 libfshfs-20240501/pyfshfs/pyfshfs_file_object_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1868 2024-05-01 06:57:22.000000 libfshfs-20240501/pyfshfs/pyfshfs.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84643 2024-05-01 06:58:50.000000 libfshfs-20240501/pyfshfs/pyfshfs_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2024-05-01 06:57:22.000000 libfshfs-20240501/pyfshfs/pyfshfs_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8068 2024-05-01 06:58:50.000000 libfshfs-20240501/pyfshfs/pyfshfs_file_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1540 2024-05-01 06:57:22.000000 libfshfs-20240501/pyfshfs/pyfshfs_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9890 2024-05-01 06:58:50.000000 libfshfs-20240501/pyfshfs/pyfshfs_extended_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25360 2024-05-01 06:58:50.000000 libfshfs-20240501/pyfshfs/pyfshfs_data_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2033 2024-05-01 06:57:22.000000 libfshfs-20240501/pyfshfs/pyfshfs_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    51000 2024-05-01 07:34:35.000000 libfshfs-20240501/pyfshfs/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-01 06:57:22.000000 libfshfs-20240501/pyfshfs/pyfshfs_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1826 2024-05-01 06:57:22.000000 libfshfs-20240501/pyfshfs/pyfshfs_datetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16397 2024-05-01 06:57:22.000000 libfshfs-20240501/pyfshfs/pyfshfs.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-05-01 06:57:22.000000 libfshfs-20240501/pyfshfs/pyfshfs_libfshfs.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2487 2024-05-01 06:57:22.000000 libfshfs-20240501/pyfshfs/pyfshfs_file_entries.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24510 2024-05-01 06:58:50.000000 libfshfs-20240501/pyfshfs/pyfshfs_volume.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-05-01 07:34:34.000000 libfshfs-20240501/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-05-01 07:34:34.000000 libfshfs-20240501/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-05-01 06:57:52.000000 libfshfs-20240501/msvscpp/libfdata/libfdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_tools_signal/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5951 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_tools_signal/fshfs_test_tools_signal.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_btree_node_descriptor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6051 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_btree_node_descriptor/fshfs_test_btree_node_descriptor.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/libfmos/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5663 2024-05-01 06:57:52.000000 libfshfs-20240501/msvscpp/libfmos/libfmos.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_tools_output/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5951 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_tools_output/fshfs_test_tools_output.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_file_record/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6021 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_file_record/fshfs_test_file_record.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/libfshfs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15318 2024-05-01 06:57:52.000000 libfshfs-20240501/msvscpp/libfshfs/libfshfs.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/zlib/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6068 2024-05-01 06:57:52.000000 libfshfs-20240501/msvscpp/zlib/zlib.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_thread_record/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6027 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_thread_record/fshfs_test_thread_record.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-05-01 06:57:52.000000 libfshfs-20240501/msvscpp/libfguid/libfguid.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-05-01 06:57:52.000000 libfshfs-20240501/msvscpp/libclocale/libclocale.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_file_system/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6021 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_file_system/fshfs_test_file_system.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_name/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6289 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_name/fshfs_test_name.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_io_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6015 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_io_handle/fshfs_test_io_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_directory_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6033 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_directory_entry/fshfs_test_directory_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-05-01 06:57:52.000000 libfshfs-20240501/msvscpp/libfcache/libfcache.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2780 2024-05-01 07:10:50.000000 libfshfs-20240501/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-05-01 06:57:52.000000 libfshfs-20240501/msvscpp/libbfio/libbfio.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/pyfshfs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7009 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/pyfshfs/pyfshfs.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfsmount/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7735 2024-05-01 06:57:52.000000 libfshfs-20240501/msvscpp/fshfsmount/fshfsmount.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_deflate/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5932 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_deflate/fshfs_test_deflate.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5844 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_notify/fshfs_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_compression/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6021 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_compression/fshfs_test_compression.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-05-01 06:57:52.000000 libfshfs-20240501/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5757 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_error/fshfs_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_fork_descriptor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6033 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_fork_descriptor/fshfs_test_fork_descriptor.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-05-01 06:57:52.000000 libfshfs-20240501/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_btree_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6024 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_btree_header/fshfs_test_btree_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfsinfo/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7348 2024-05-01 06:57:52.000000 libfshfs-20240501/msvscpp/fshfsinfo/fshfsinfo.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_master_directory_block/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6304 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_master_directory_block/fshfs_test_master_directory_block.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49808 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/libfshfs.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_btree_file/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6268 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_btree_file/fshfs_test_btree_file.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_huffman_tree/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6024 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_huffman_tree/fshfs_test_huffman_tree.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-05-01 06:57:52.000000 libfshfs-20240501/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_btree_node_record/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6039 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_btree_node_record/fshfs_test_btree_node_record.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_attributes_btree_key/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6048 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_attributes_btree_key/fshfs_test_attributes_btree_key.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_bit_stream/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6018 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_bit_stream/fshfs_test_bit_stream.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-05-01 06:57:52.000000 libfshfs-20240501/msvscpp/libcpath/libcpath.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_catalog_btree_key/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6039 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_catalog_btree_key/fshfs_test_catalog_btree_key.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_extents_btree_key/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6039 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_extents_btree_key/fshfs_test_extents_btree_key.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_compressed_data_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6137 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_compressed_data_handle/fshfs_test_compressed_data_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_extent/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6006 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_extent/fshfs_test_extent.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_directory_record/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6036 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_directory_record/fshfs_test_directory_record.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/libhmac/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5312 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/libhmac/libhmac.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-05-01 06:57:52.000000 libfshfs-20240501/msvscpp/libcsplit/libcsplit.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-05-01 06:57:52.000000 libfshfs-20240501/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26099 2024-05-01 07:34:35.000000 libfshfs-20240501/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_profiler/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6012 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_profiler/fshfs_test_profiler.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6672 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_support/fshfs_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_attribute_record/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6036 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_attribute_record/fshfs_test_attribute_record.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_btree_node/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6018 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_btree_node/fshfs_test_btree_node.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_volume/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6669 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_volume/fshfs_test_volume.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-05-01 06:57:52.000000 libfshfs-20240501/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_file_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6018 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_file_entry/fshfs_test_file_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_tools_info_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6276 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_tools_info_handle/fshfs_test_tools_info_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-05-01 06:57:52.000000 libfshfs-20240501/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-05-01 06:57:52.000000 libfshfs-20240501/msvscpp/libfdatetime/libfdatetime.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_volume_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6277 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_volume_header/fshfs_test_volume_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/msvscpp/fshfs_test_buffer_data_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6042 2024-05-01 06:58:26.000000 libfshfs-20240501/msvscpp/fshfs_test_buffer_data_handle/fshfs_test_buffer_data_handle.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       92 2024-05-01 06:57:20.000000 libfshfs-20240501/AUTHORS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:10.000000 libfshfs-20240501/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-01 07:33:57.000000 libfshfs-20240501/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-05-01 07:33:57.000000 libfshfs-20240501/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-01 07:33:57.000000 libfshfs-20240501/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-01 07:33:57.000000 libfshfs-20240501/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-05-01 07:33:57.000000 libfshfs-20240501/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-05-01 07:33:57.000000 libfshfs-20240501/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      938 2024-05-01 07:33:57.000000 libfshfs-20240501/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-01 07:33:57.000000 libfshfs-20240501/libcfile/libcfile_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-01 07:33:57.000000 libfshfs-20240501/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-05-01 07:33:57.000000 libfshfs-20240501/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-01 07:33:57.000000 libfshfs-20240501/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-01 07:33:57.000000 libfshfs-20240501/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-01 07:33:57.000000 libfshfs-20240501/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-01 07:33:57.000000 libfshfs-20240501/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-05-01 07:33:57.000000 libfshfs-20240501/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-01 07:33:57.000000 libfshfs-20240501/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-05-01 07:33:57.000000 libfshfs-20240501/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32360 2024-05-01 07:34:35.000000 libfshfs-20240501/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-01 07:33:57.000000 libfshfs-20240501/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-01 07:33:57.000000 libfshfs-20240501/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-05-01 07:33:57.000000 libfshfs-20240501/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-05-01 07:33:57.000000 libfshfs-20240501/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      971 2024-05-01 06:58:50.000000 libfshfs-20240501/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-05-01 07:34:34.000000 libfshfs-20240501/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:10.000000 libfshfs-20240501/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34273 2024-05-01 07:34:35.000000 libfshfs-20240501/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-01 07:33:54.000000 libfshfs-20240501/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-05-01 06:57:17.000000 libfshfs-20240501/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      487 2024-05-01 06:57:17.000000 libfshfs-20240501/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-05-01 07:34:34.000000 libfshfs-20240501/config.sub
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      770 2024-05-01 06:57:17.000000 libfshfs-20240501/libfshfs.pc.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-05-01 06:57:17.000000 libfshfs-20240501/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1508 2024-05-01 06:57:17.000000 libfshfs-20240501/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:06:45.000000 libfshfs-20240501/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:10.000000 libfshfs-20240501/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-05-01 07:34:08.000000 libfshfs-20240501/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-05-01 07:34:08.000000 libfshfs-20240501/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-05-01 07:34:08.000000 libfshfs-20240501/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-05-01 07:34:08.000000 libfshfs-20240501/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-05-01 07:34:08.000000 libfshfs-20240501/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-05-01 07:34:08.000000 libfshfs-20240501/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-01 07:34:08.000000 libfshfs-20240501/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-05-01 07:34:08.000000 libfshfs-20240501/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-05-01 07:34:08.000000 libfshfs-20240501/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-05-01 07:34:08.000000 libfshfs-20240501/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-05-01 07:34:08.000000 libfshfs-20240501/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-05-01 07:34:08.000000 libfshfs-20240501/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-05-01 07:34:08.000000 libfshfs-20240501/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-05-01 07:34:08.000000 libfshfs-20240501/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-05-01 07:34:08.000000 libfshfs-20240501/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-05-01 07:34:08.000000 libfshfs-20240501/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-05-01 07:34:08.000000 libfshfs-20240501/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-05-01 07:34:08.000000 libfshfs-20240501/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-05-01 07:34:08.000000 libfshfs-20240501/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-05-01 07:34:08.000000 libfshfs-20240501/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-01 07:34:08.000000 libfshfs-20240501/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-05-01 07:34:08.000000 libfshfs-20240501/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-05-01 07:34:08.000000 libfshfs-20240501/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-05-01 07:34:08.000000 libfshfs-20240501/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-05-01 07:34:08.000000 libfshfs-20240501/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-05-01 07:34:08.000000 libfshfs-20240501/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-05-01 07:34:08.000000 libfshfs-20240501/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34712 2024-05-01 07:34:35.000000 libfshfs-20240501/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-05-01 07:34:08.000000 libfshfs-20240501/libcthreads/libcthreads_queue.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-05-01 07:34:35.000000 libfshfs-20240501/test-driver
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:10.000000 libfshfs-20240501/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-05-01 07:34:03.000000 libfshfs-20240501/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-01 07:34:03.000000 libfshfs-20240501/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-05-01 07:34:03.000000 libfshfs-20240501/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2024-05-01 07:34:03.000000 libfshfs-20240501/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-01 07:34:03.000000 libfshfs-20240501/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-01 07:34:03.000000 libfshfs-20240501/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-01 07:34:03.000000 libfshfs-20240501/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-05-01 07:34:03.000000 libfshfs-20240501/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-05-01 07:34:03.000000 libfshfs-20240501/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-01 07:34:03.000000 libfshfs-20240501/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-01 07:34:03.000000 libfshfs-20240501/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-01 07:34:03.000000 libfshfs-20240501/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31558 2024-05-01 07:34:35.000000 libfshfs-20240501/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-01 07:34:03.000000 libfshfs-20240501/libcpath/libcpath_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-01 07:34:03.000000 libfshfs-20240501/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-05-01 07:34:03.000000 libfshfs-20240501/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-05-01 07:34:03.000000 libfshfs-20240501/libcpath/libcpath_path.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1912 2023-12-03 09:06:45.000000 libfshfs-20240501/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:11.000000 libfshfs-20240501/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1989 2024-05-01 06:57:24.000000 libfshfs-20240501/manuals/fshfsinfo.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      161 2024-05-01 07:10:42.000000 libfshfs-20240501/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15268 2024-05-01 06:57:24.000000 libfshfs-20240501/manuals/libfshfs.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-01 06:57:24.000000 libfshfs-20240501/manuals/fshfsmount.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28324 2024-05-01 07:34:35.000000 libfshfs-20240501/manuals/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/tests/
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3317 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/test_fshfsinfo.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29883 2024-05-01 06:58:26.000000 libfshfs-20240501/tests/fshfs_test_directory_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1704 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15297 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_btree_node_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4323 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12439 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_compression.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39762 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_unicode_case_folding_mappings.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6139 2024-05-01 06:58:26.000000 libfshfs-20240501/tests/fshfs_test_file_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8954 2024-05-01 06:58:26.000000 libfshfs-20240501/tests/fshfs_test_btree_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5877 2024-05-01 06:58:26.000000 libfshfs-20240501/tests/fshfs_test_extent.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32976 2024-05-01 06:58:26.000000 libfshfs-20240501/tests/fshfs_test_file_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4700 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1709 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_libbfio.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4045 2024-05-01 07:08:34.000000 libfshfs-20240501/tests/test_tools.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15726 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_functions.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)  1117748 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_unicode_decomposition_mappings.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9757 2024-05-01 06:58:26.000000 libfshfs-20240501/tests/fshfs_test_attributes_btree_key.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8574 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17397 2024-05-01 06:58:26.000000 libfshfs-20240501/tests/fshfs_test_master_directory_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3464 2024-05-01 06:59:00.000000 libfshfs-20240501/tests/pyfshfs_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14017 2024-05-01 07:17:01.000000 libfshfs-20240501/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6750 2024-05-01 06:58:26.000000 libfshfs-20240501/tests/fshfs_test_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9259 2024-05-01 06:58:26.000000 libfshfs-20240501/tests/fshfs_test_thread_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11979 2024-05-01 06:58:26.000000 libfshfs-20240501/tests/fshfs_test_fork_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9484 2024-05-01 06:58:26.000000 libfshfs-20240501/tests/fshfs_test_extents_btree_key.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4415 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13779 2024-05-01 06:58:26.000000 libfshfs-20240501/tests/fshfs_test_bit_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18385 2024-05-01 06:58:26.000000 libfshfs-20240501/tests/fshfs_test_attribute_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17738 2024-05-01 06:58:26.000000 libfshfs-20240501/tests/fshfs_test_buffer_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1997 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_functions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4169 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_tools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10871 2024-05-01 06:58:26.000000 libfshfs-20240501/tests/fshfs_test_catalog_btree_key.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100638 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_deflate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30822 2024-05-01 06:58:26.000000 libfshfs-20240501/tests/fshfs_test_huffman_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9202 2024-05-01 06:59:00.000000 libfshfs-20240501/tests/pyfshfs_test_volume.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5706 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_tools_info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2447 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_tools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35448 2024-05-01 06:58:26.000000 libfshfs-20240501/tests/fshfs_test_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9474 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_btree_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_libfshfs.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4740 2024-05-01 06:58:26.000000 libfshfs-20240501/tests/fshfs_test_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3139 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19381 2024-05-01 06:58:26.000000 libfshfs-20240501/tests/fshfs_test_volume_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7050 2024-05-01 06:58:26.000000 libfshfs-20240501/tests/fshfs_test_profiler.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    90797 2024-05-01 07:34:35.000000 libfshfs-20240501/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6532 2024-05-01 06:58:26.000000 libfshfs-20240501/tests/fshfs_test_btree_node_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21042 2024-05-01 06:58:26.000000 libfshfs-20240501/tests/fshfs_test_compressed_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8056 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_io_handle.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4445 2024-05-01 07:08:19.000000 libfshfs-20240501/tests/test_library.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40566 2024-05-01 06:58:26.000000 libfshfs-20240501/tests/fshfs_test_directory_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32805 2024-05-01 06:57:24.000000 libfshfs-20240501/tests/fshfs_test_name.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:12.000000 libfshfs-20240501/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2503 2024-05-01 06:57:22.000000 libfshfs-20240501/ossfuzz/volume_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2020 2024-05-01 07:10:27.000000 libfshfs-20240501/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-05-01 06:57:22.000000 libfshfs-20240501/ossfuzz/ossfuzz_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5686 2024-05-01 06:57:22.000000 libfshfs-20240501/ossfuzz/file_entry_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3320 2024-05-01 06:57:22.000000 libfshfs-20240501/ossfuzz/extended_attribute_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      972 2024-05-01 06:57:22.000000 libfshfs-20240501/ossfuzz/ossfuzz_libfshfs.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37830 2024-05-01 07:34:35.000000 libfshfs-20240501/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-05-01 07:34:28.000000 libfshfs-20240501/ltmain.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2489 2024-05-01 07:34:50.000000 libfshfs-20240501/libfshfs.spec
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:11.000000 libfshfs-20240501/libhmac/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47989 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_sha1_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_sha224.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50026 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_sha512_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14448 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_md5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2079 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_md5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1942 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9362 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14650 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_sha512.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45648 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_sha256_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_sha224.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1623 2024-05-01 07:34:21.000000 libfshfs-20240501/libhmac/libhmac_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2060 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_sha1.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3443 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_sha256_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1117 2024-05-01 07:34:21.000000 libfshfs-20240501/libhmac/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45605 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_sha224_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_md5_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_sha256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3368 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_sha1_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34423 2024-05-01 07:34:35.000000 libfshfs-20240501/libhmac/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_sha256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3461 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_sha224_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3444 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_sha512_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_sha512.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14514 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_sha1.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40596 2024-05-01 07:34:20.000000 libfshfs-20240501/libhmac/libhmac_md5_context.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:10.000000 libfshfs-20240501/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-05-01 07:34:05.000000 libfshfs-20240501/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-05-01 07:34:05.000000 libfshfs-20240501/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-05-01 07:34:05.000000 libfshfs-20240501/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-05-01 07:34:05.000000 libfshfs-20240501/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-01 07:34:05.000000 libfshfs-20240501/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-05-01 07:34:05.000000 libfshfs-20240501/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-01 07:34:05.000000 libfshfs-20240501/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-05-01 07:34:05.000000 libfshfs-20240501/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-01 07:34:05.000000 libfshfs-20240501/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-05-01 07:34:05.000000 libfshfs-20240501/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-01 07:34:05.000000 libfshfs-20240501/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-05-01 07:34:05.000000 libfshfs-20240501/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-01 07:34:05.000000 libfshfs-20240501/libcsplit/libcsplit_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-01 07:34:05.000000 libfshfs-20240501/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-01 07:34:05.000000 libfshfs-20240501/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-05-01 07:34:05.000000 libfshfs-20240501/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32455 2024-05-01 07:34:35.000000 libfshfs-20240501/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-05-01 07:34:05.000000 libfshfs-20240501/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-05-01 07:34:05.000000 libfshfs-20240501/libcsplit/libcsplit_narrow_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:11.000000 libfshfs-20240501/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:06:54.000000 libfshfs-20240501/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:06:54.000000 libfshfs-20240501/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:06:54.000000 libfshfs-20240501/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:06:54.000000 libfshfs-20240501/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:06:54.000000 libfshfs-20240501/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:06:54.000000 libfshfs-20240501/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:06:54.000000 libfshfs-20240501/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:06:54.000000 libfshfs-20240501/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:06:54.000000 libfshfs-20240501/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1854 2024-05-01 07:34:49.000000 libfshfs-20240501/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:06:54.000000 libfshfs-20240501/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:06:54.000000 libfshfs-20240501/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:10.000000 libfshfs-20240501/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    58039 2024-05-01 07:34:35.000000 libfshfs-20240501/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-05-01 07:34:24.000000 libfshfs-20240501/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42341 2024-05-01 07:34:34.000000 libfshfs-20240501/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:10.000000 libfshfs-20240501/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-01 07:34:01.000000 libfshfs-20240501/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-01 07:34:01.000000 libfshfs-20240501/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-05-01 07:34:01.000000 libfshfs-20240501/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-05-01 07:34:01.000000 libfshfs-20240501/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-05-01 07:34:01.000000 libfshfs-20240501/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-01 07:34:01.000000 libfshfs-20240501/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-05-01 07:34:01.000000 libfshfs-20240501/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-05-01 07:34:01.000000 libfshfs-20240501/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-05-01 07:34:01.000000 libfshfs-20240501/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-05-01 07:34:01.000000 libfshfs-20240501/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-05-01 07:34:01.000000 libfshfs-20240501/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31396 2024-05-01 07:34:35.000000 libfshfs-20240501/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-01 07:34:01.000000 libfshfs-20240501/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-05-01 07:34:01.000000 libfshfs-20240501/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:09.000000 libfshfs-20240501/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-05-01 07:33:55.000000 libfshfs-20240501/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-05-01 07:33:55.000000 libfshfs-20240501/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-01 07:33:55.000000 libfshfs-20240501/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-05-01 07:33:55.000000 libfshfs-20240501/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-05-01 07:33:55.000000 libfshfs-20240501/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-01 07:33:55.000000 libfshfs-20240501/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-05-01 07:33:55.000000 libfshfs-20240501/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-05-01 07:33:55.000000 libfshfs-20240501/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-05-01 07:33:55.000000 libfshfs-20240501/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-01 07:33:55.000000 libfshfs-20240501/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-01 07:33:55.000000 libfshfs-20240501/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30863 2024-05-01 07:34:35.000000 libfshfs-20240501/libcerror/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3619 2024-05-01 06:57:17.000000 libfshfs-20240501/libfshfs.spec.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:11.000000 libfshfs-20240501/fshfstools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1443 2024-05-01 06:57:23.000000 libfshfs-20240501/fshfstools/fshfstools_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1483 2024-05-01 06:57:23.000000 libfshfs-20240501/fshfstools/fshfstools_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4361 2024-05-01 06:57:23.000000 libfshfs-20240501/fshfstools/fshfstools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37213 2024-05-01 06:58:50.000000 libfshfs-20240501/fshfstools/mount_dokan.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3061 2024-05-01 06:58:50.000000 libfshfs-20240501/fshfstools/mount_file_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1213 2024-05-01 06:57:23.000000 libfshfs-20240501/fshfstools/fshfstools_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38773 2024-05-01 06:58:50.000000 libfshfs-20240501/fshfstools/mount_fuse.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4584 2024-05-01 06:58:50.000000 libfshfs-20240501/fshfstools/info_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5417 2024-05-01 06:57:23.000000 libfshfs-20240501/fshfstools/mount_dokan.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1474 2024-05-01 06:57:23.000000 libfshfs-20240501/fshfstools/fshfstools_libhmac.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3297 2024-05-01 06:57:23.000000 libfshfs-20240501/fshfstools/digest_hash.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30757 2024-05-01 06:58:50.000000 libfshfs-20240501/fshfstools/mount_file_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-05-01 06:57:23.000000 libfshfs-20240501/fshfstools/fshfstools_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2579 2024-05-01 07:10:19.000000 libfshfs-20240501/fshfstools/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1781 2024-05-01 06:57:23.000000 libfshfs-20240501/fshfstools/fshfstools_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1409 2024-05-01 06:57:23.000000 libfshfs-20240501/fshfstools/fshfstools_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25597 2024-05-01 06:58:50.000000 libfshfs-20240501/fshfstools/mount_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-05-01 06:57:23.000000 libfshfs-20240501/fshfstools/fshfstools_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70646 2024-05-01 06:58:50.000000 libfshfs-20240501/fshfstools/info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3822 2024-05-01 06:58:50.000000 libfshfs-20240501/fshfstools/mount_file_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1590 2024-05-01 06:57:23.000000 libfshfs-20240501/fshfstools/fshfstools_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3324 2024-05-01 06:58:50.000000 libfshfs-20240501/fshfstools/mount_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-05-01 06:57:23.000000 libfshfs-20240501/fshfstools/fshfstools_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-05-01 06:57:23.000000 libfshfs-20240501/fshfstools/fshfstools_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10890 2024-05-01 06:58:50.000000 libfshfs-20240501/fshfstools/fshfsinfo.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5751 2024-05-01 06:57:23.000000 libfshfs-20240501/fshfstools/fshfstools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-05-01 06:57:23.000000 libfshfs-20240501/fshfstools/fshfstools_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19354 2024-05-01 06:58:50.000000 libfshfs-20240501/fshfstools/mount_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-05-01 06:57:23.000000 libfshfs-20240501/fshfstools/fshfstools_libfshfs.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1771 2024-05-01 06:57:23.000000 libfshfs-20240501/fshfstools/fshfstools_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15501 2024-05-01 06:58:50.000000 libfshfs-20240501/fshfstools/fshfsmount.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1486 2024-05-01 06:57:23.000000 libfshfs-20240501/fshfstools/fshfstools_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36409 2024-05-01 07:34:34.000000 libfshfs-20240501/fshfstools/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1761 2024-05-01 06:57:23.000000 libfshfs-20240501/fshfstools/fshfstools_signal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1244 2024-05-01 06:57:23.000000 libfshfs-20240501/fshfstools/digest_hash.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-01 06:57:23.000000 libfshfs-20240501/fshfstools/fshfstools_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1472 2024-05-01 06:57:23.000000 libfshfs-20240501/fshfstools/fshfstools_output.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3050 2024-05-01 06:58:50.000000 libfshfs-20240501/fshfstools/mount_fuse.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-01 07:57:10.000000 libfshfs-20240501/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-05-01 07:34:14.000000 libfshfs-20240501/libfdatetime/libfdatetime_floatingtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-05-01 07:34:14.000000 libfshfs-20240501/libfdatetime/libfdatetime_nsf_timedate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-05-01 07:34:14.000000 libfshfs-20240501/libfdatetime/libfdatetime_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-05-01 07:34:14.000000 libfshfs-20240501/libfdatetime/libfdatetime_floatingtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-05-01 07:34:14.000000 libfshfs-20240501/libfdatetime/libfdatetime_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-05-01 07:34:14.000000 libfshfs-20240501/libfdatetime/libfdatetime_hfs_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-05-01 07:34:14.000000 libfshfs-20240501/libfdatetime/libfdatetime_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-05-01 07:34:14.000000 libfshfs-20240501/libfdatetime/libfdatetime_hfs_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1144 2024-05-01 07:34:14.000000 libfshfs-20240501/libfdatetime/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-05-01 07:34:14.000000 libfshfs-20240501/libfdatetime/libfdatetime_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-05-01 07:34:14.000000 libfshfs-20240501/libfdatetime/libfdatetime_systemtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-01 07:34:14.000000 libfshfs-20240501/libfdatetime/libfdatetime_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-05-01 07:34:14.000000 libfshfs-20240501/libfdatetime/libfdatetime_posix_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-05-01 07:34:14.000000 libfshfs-20240501/libfdatetime/libfdatetime_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-05-01 07:34:14.000000 libfshfs-20240501/libfdatetime/libfdatetime_fat_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-05-01 07:34:14.000000 libfshfs-20240501/libfdatetime/libfdatetime_systemtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-05-01 07:34:14.000000 libfshfs-20240501/libfdatetime/libfdatetime_nsf_timedate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-05-01 07:34:14.000000 libfshfs-20240501/libfdatetime/libfdatetime_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-05-01 07:34:14.000000 libfshfs-20240501/libfdatetime/libfdatetime_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-05-01 07:34:14.000000 libfshfs-20240501/libfdatetime/libfdatetime_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-05-01 07:34:14.000000 libfshfs-20240501/libfdatetime/libfdatetime_posix_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-05-01 07:34:14.000000 libfshfs-20240501/libfdatetime/libfdatetime_date_time_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-05-01 07:34:14.000000 libfshfs-20240501/libfdatetime/libfdatetime_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-05-01 07:34:14.000000 libfshfs-20240501/libfdatetime/libfdatetime_date_time_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-05-01 07:34:14.000000 libfshfs-20240501/libfdatetime/libfdatetime_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34447 2024-05-01 07:34:35.000000 libfshfs-20240501/libfdatetime/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-05-01 07:34:14.000000 libfshfs-20240501/libfdatetime/libfdatetime_fat_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56937 2024-05-01 07:34:31.000000 libfshfs-20240501/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8495 2024-05-01 06:57:17.000000 libfshfs-20240501/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      418 2024-05-01 07:57:13.084123 libfshfs-20240501/PKG-INFO
```

### Comparing `libfshfs-20240221/libfdata/libfdata_error.h` & `libfshfs-20240501/libfdata/libfdata_error.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_area.c` & `libfshfs-20240501/libfdata/libfdata_area.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_stream.h` & `libfshfs-20240501/libfdata/libfdata_stream.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_cache.h` & `libfshfs-20240501/libfdata/libfdata_cache.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_range_list.c` & `libfshfs-20240501/libfdata/libfdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_mapped_range.c` & `libfshfs-20240501/libfdata/libfdata_mapped_range.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_libcerror.h` & `libfshfs-20240501/libfdata/libfdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_definitions.h` & `libfshfs-20240501/libfdata/libfdata_definitions.h`

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

### Comparing `libfshfs-20240221/libfdata/libfdata_list.c` & `libfshfs-20240501/libfdata/libfdata_list.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_libcdata.h` & `libfshfs-20240501/libfdata/libfdata_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_list.h` & `libfshfs-20240501/libfdata/libfdata_list.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_list_element.h` & `libfshfs-20240501/libfdata/libfdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/Makefile.am` & `libfshfs-20240501/libfdata/Makefile.am`

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

### Comparing `libfshfs-20240221/libfdata/libfdata_libcnotify.h` & `libfshfs-20240501/libfdata/libfdata_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_extern.h` & `libfshfs-20240501/libfdata/libfdata_extern.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_notify.c` & `libfshfs-20240501/libfdata/libfdata_notify.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_cache.c` & `libfshfs-20240501/libfdata/libfdata_cache.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_stream.c` & `libfshfs-20240501/libfdata/libfdata_stream.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_unused.h` & `libfshfs-20240501/libfdata/libfdata_unused.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_range.h` & `libfshfs-20240501/libfdata/libfdata_range.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_area.h` & `libfshfs-20240501/libfdata/libfdata_area.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_error.c` & `libfshfs-20240501/libfdata/libfdata_error.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_support.h` & `libfshfs-20240501/libfdata/libfdata_support.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_range.c` & `libfshfs-20240501/libfdata/libfdata_range.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_mapped_range.h` & `libfshfs-20240501/libfdata/libfdata_mapped_range.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_support.c` & `libfshfs-20240501/libfdata/libfdata_support.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_list_element.c` & `libfshfs-20240501/libfdata/libfdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_segments_array.c` & `libfshfs-20240501/libfdata/libfdata_segments_array.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_types.h` & `libfshfs-20240501/libfdata/libfdata_types.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_notify.h` & `libfshfs-20240501/libfdata/libfdata_notify.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_range_list.h` & `libfshfs-20240501/libfdata/libfdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_segments_array.h` & `libfshfs-20240501/libfdata/libfdata_segments_array.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/Makefile.in` & `libfshfs-20240501/libfdata/Makefile.in`

 * *Files 6% similar despite different names*

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
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
 
@@ -606,15 +608,16 @@
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
@@ -826,24 +829,39 @@
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
 
@@ -939,17 +957,14 @@
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

### Comparing `libfshfs-20240221/libfdata/libfdata_vector.c` & `libfshfs-20240501/libfdata/libfdata_vector.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_libfcache.h` & `libfshfs-20240501/libfdata/libfdata_libfcache.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdata/libfdata_vector.h` & `libfshfs-20240501/libfdata/libfdata_vector.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfmos/libfmos_lzfse_bit_stream.h` & `libfshfs-20240501/libfmos/libfmos_lzfse_bit_stream.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfmos/libfmos_definitions.h` & `libfshfs-20240501/libfmos/libfmos_definitions.h`

 * *Files 4% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfmos/definitions.h> are copied here
  * for local use of libfmos
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFMOS_VERSION					20240118
+#define LIBFMOS_VERSION					20240415
 
 /* The version string
  */
-#define LIBFMOS_VERSION_STRING				"20240118"
+#define LIBFMOS_VERSION_STRING				"20240415"
 
 #endif /* !defined( HAVE_LOCAL_LIBFMOS ) */
 
 #define LIBFMOS_LZFSE_NUMBER_OF_LITERAL_STATES		1024
 #define LIBFMOS_LZFSE_NUMBER_OF_LITERAL_SYMBOLS		256
 
 #define LIBFMOS_LZFSE_NUMBER_OF_L_VALUE_STATES		64
```

### Comparing `libfshfs-20240221/libfmos/libfmos_lzfse_decoder.c` & `libfshfs-20240501/libfmos/libfmos_lzfse_decoder.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfmos/libfmos_types.h` & `libfshfs-20240501/libfmos/libfmos_types.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfmos/libfmos_adc.c` & `libfshfs-20240501/libfmos/libfmos_adc.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfmos/libfmos_lzfse.h` & `libfshfs-20240501/libfmos/libfmos_lzfse.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfmos/libfmos_notify.h` & `libfshfs-20240501/libfmos/libfmos_notify.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfmos/libfmos_adc.h` & `libfshfs-20240501/libfmos/libfmos_adc.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfmos/libfmos_support.c` & `libfshfs-20240501/libfmos/libfmos_support.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfmos/libfmos_error.c` & `libfshfs-20240501/libfmos/libfmos_error.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfmos/Makefile.am` & `libfshfs-20240501/libfmos/Makefile.am`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFMOS
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfmos.la
 
@@ -22,19 +22,17 @@
 	libfmos_lzvn.c libfmos_lzvn.h \
 	libfmos_notify.c libfmos_notify.h \
 	libfmos_support.c libfmos_support.h \
 	libfmos_types.h \
 	libfmos_unused.h
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
 	@echo "Running splint on libfmos ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfmos_la_SOURCES)
```

### Comparing `libfshfs-20240221/libfmos/libfmos_unused.h` & `libfshfs-20240501/libfmos/libfmos_unused.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfmos/libfmos_lzvn.c` & `libfshfs-20240501/libfmos/libfmos_lzvn.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfmos/libfmos_libcnotify.h` & `libfshfs-20240501/libfmos/libfmos_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfmos/libfmos_lzfse_bit_stream.c` & `libfshfs-20240501/libfmos/libfmos_lzfse_bit_stream.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfmos/libfmos_lzfse_decoder.h` & `libfshfs-20240501/libfmos/libfmos_lzfse_decoder.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfmos/libfmos_libcerror.h` & `libfshfs-20240501/libfmos/libfmos_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfmos/libfmos_lzfse.c` & `libfshfs-20240501/libfmos/libfmos_lzfse.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfmos/libfmos_notify.c` & `libfshfs-20240501/libfmos/libfmos_notify.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfmos/libfmos_error.h` & `libfshfs-20240501/libfmos/libfmos_error.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfmos/libfmos_support.h` & `libfshfs-20240501/libfmos/libfmos_support.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfmos/libfmos_lzvn.h` & `libfshfs-20240501/libfmos/libfmos_lzvn.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfmos/libfmos_extern.h` & `libfshfs-20240501/libfmos/libfmos_extern.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfmos/Makefile.in` & `libfshfs-20240501/libfmos/Makefile.in`

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
@@ -558,16 +560,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBFMOS_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFMOS_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFMOS_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFMOS_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFMOS_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFMOS_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFMOS_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFMOS_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFMOS_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFMOS_TRUE@noinst_LTLIBRARIES = libfmos.la
 @HAVE_LOCAL_LIBFMOS_TRUE@libfmos_la_SOURCES = \
@@ -582,15 +584,16 @@
 @HAVE_LOCAL_LIBFMOS_TRUE@	libfmos_lzfse_decoder.c libfmos_lzfse_decoder.h \
 @HAVE_LOCAL_LIBFMOS_TRUE@	libfmos_lzvn.c libfmos_lzvn.h \
 @HAVE_LOCAL_LIBFMOS_TRUE@	libfmos_notify.c libfmos_notify.h \
 @HAVE_LOCAL_LIBFMOS_TRUE@	libfmos_support.c libfmos_support.h \
 @HAVE_LOCAL_LIBFMOS_TRUE@	libfmos_types.h \
 @HAVE_LOCAL_LIBFMOS_TRUE@	libfmos_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -797,24 +800,34 @@
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
+		-rm -f ./$(DEPDIR)/libfmos_adc.Plo
+	-rm -f ./$(DEPDIR)/libfmos_error.Plo
+	-rm -f ./$(DEPDIR)/libfmos_lzfse.Plo
+	-rm -f ./$(DEPDIR)/libfmos_lzfse_bit_stream.Plo
+	-rm -f ./$(DEPDIR)/libfmos_lzfse_decoder.Plo
+	-rm -f ./$(DEPDIR)/libfmos_lzvn.Plo
+	-rm -f ./$(DEPDIR)/libfmos_notify.Plo
+	-rm -f ./$(DEPDIR)/libfmos_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -905,17 +918,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfmos ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfmos_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfshfs-20240221/COPYING` & `libfshfs-20240501/COPYING`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/install-sh` & `libfshfs-20240501/install-sh`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_btree_node_vector.c` & `libfshfs-20240501/libfshfs/libfshfs_btree_node_vector.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_btree_node_descriptor.h` & `libfshfs-20240501/libfshfs/libfshfs_btree_node_descriptor.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_notify.h` & `libfshfs-20240501/libfshfs/libfshfs_notify.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_extents_btree_file.c` & `libfshfs-20240501/libfshfs/libfshfs_extents_btree_file.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_file_record.c` & `libfshfs-20240501/libfshfs/libfshfs_file_record.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_block_data_handle.c` & `libfshfs-20240501/libfshfs/libfshfs_block_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_attribute_record.h` & `libfshfs-20240501/libfshfs/libfshfs_attribute_record.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs.rc` & `libfshfs-20240501/libfshfs/libfshfs.rc`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the Hierarchical File System (HFS) format\0"
-      VALUE "FileVersion",		"20240221" "\0"
+      VALUE "FileVersion",		"20240501" "\0"
       VALUE "InternalName",		"libfshfs.dll\0"
       VALUE "LegalCopyright",		"(C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libfshfs.dll\0"
       VALUE "ProductName",		"libfshfs\0"
-      VALUE "ProductVersion",		"20240221" "\0"
+      VALUE "ProductVersion",		"20240501" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libfshfs/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libfshfs-20240221/libfshfs/libfshfs_compressed_data_handle.c` & `libfshfs-20240501/libfshfs/libfshfs_compressed_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_libuna.h` & `libfshfs-20240501/libfshfs/libfshfs_libuna.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_fork_descriptor.h` & `libfshfs-20240501/libfshfs/libfshfs_fork_descriptor.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_btree_node.h` & `libfshfs-20240501/libfshfs/libfshfs_btree_node.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_file_entry.h` & `libfshfs-20240501/libfshfs/libfshfs_file_entry.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_huffman_tree.h` & `libfshfs-20240501/libfshfs/libfshfs_huffman_tree.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_volume.h` & `libfshfs-20240501/libfshfs/libfshfs_volume.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_libfguid.h` & `libfshfs-20240501/libfshfs/libfshfs_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_libfcache.h` & `libfshfs-20240501/libfshfs/libfshfs_libfcache.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_directory_entry.c` & `libfshfs-20240501/libfshfs/libfshfs_directory_entry.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_data_stream.c` & `libfshfs-20240501/libfshfs/libfshfs_data_stream.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_directory_record.c` & `libfshfs-20240501/libfshfs/libfshfs_directory_record.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_file_record.h` & `libfshfs-20240501/libfshfs/libfshfs_file_record.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_btree_file.c` & `libfshfs-20240501/libfshfs/libfshfs_btree_file.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_libclocale.h` & `libfshfs-20240501/libfshfs/libfshfs_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_compressed_data_header.c` & `libfshfs-20240501/libfshfs/libfshfs_compressed_data_header.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_btree_node_record.c` & `libfshfs-20240501/libfshfs/libfshfs_btree_node_record.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_thread_record.c` & `libfshfs-20240501/libfshfs/libfshfs_thread_record.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_debug.c` & `libfshfs-20240501/libfshfs/libfshfs_debug.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_extents_record.h` & `libfshfs-20240501/libfshfs/libfshfs_extents_record.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_bit_stream.h` & `libfshfs-20240501/libfshfs/libfshfs_bit_stream.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_catalog_btree_file.h` & `libfshfs-20240501/libfshfs/libfshfs_catalog_btree_file.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_support.c` & `libfshfs-20240501/libfshfs/libfshfs_support.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_master_directory_block.c` & `libfshfs-20240501/libfshfs/libfshfs_master_directory_block.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_btree_header.h` & `libfshfs-20240501/libfshfs/libfshfs_btree_header.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_fork_descriptor.c` & `libfshfs-20240501/libfshfs/libfshfs_fork_descriptor.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_deflate.c` & `libfshfs-20240501/libfshfs/libfshfs_deflate.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_btree_node_vector.h` & `libfshfs-20240501/libfshfs/libfshfs_btree_node_vector.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_extents_btree_key.c` & `libfshfs-20240501/libfshfs/libfshfs_extents_btree_key.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_error.h` & `libfshfs-20240501/libfshfs/libfshfs_error.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_error.c` & `libfshfs-20240501/libfshfs/libfshfs_error.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/fshfs_btree.h` & `libfshfs-20240501/libfshfs/fshfs_btree.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_volume_header.c` & `libfshfs-20240501/libfshfs/libfshfs_volume_header.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_types.h` & `libfshfs-20240501/libfshfs/libfshfs_types.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_btree_node_record.h` & `libfshfs-20240501/libfshfs/libfshfs_btree_node_record.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/Makefile.am` & `libfshfs-20240501/libfshfs/Makefile.am`

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
@@ -115,21 +115,19 @@
 libfshfs_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libfshfs_definitions.h.in \
 	libfshfs.rc \
 	libfshfs.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfshfs_definitions.h \
+	libfshfs.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libfshfs_definitions.h
-	-rm -f libfshfs.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfshfs ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfshfs_la_SOURCES)
```

### Comparing `libfshfs-20240221/libfshfs/libfshfs_libcdata.h` & `libfshfs-20240501/libfshfs/libfshfs_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_compressed_data_handle.h` & `libfshfs-20240501/libfshfs/libfshfs_compressed_data_handle.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_btree_node_cache.c` & `libfshfs-20240501/libfshfs/libfshfs_btree_node_cache.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_catalog_btree_key.h` & `libfshfs-20240501/libfshfs/libfshfs_catalog_btree_key.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_io_handle.c` & `libfshfs-20240501/libfshfs/libfshfs_io_handle.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_unused.h` & `libfshfs-20240501/libfshfs/libfshfs_unused.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_directory_record.h` & `libfshfs-20240501/libfshfs/libfshfs_directory_record.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_directory_entry.h` & `libfshfs-20240501/libfshfs/libfshfs_directory_entry.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_profiler.h` & `libfshfs-20240501/libfshfs/libfshfs_profiler.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_libcnotify.h` & `libfshfs-20240501/libfshfs/libfshfs_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_extern.h` & `libfshfs-20240501/libfshfs/libfshfs_extern.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/fshfs_compressed_data.h` & `libfshfs-20240501/libfshfs/fshfs_compressed_data.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_btree_node_descriptor.c` & `libfshfs-20240501/libfshfs/libfshfs_btree_node_descriptor.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_extent.c` & `libfshfs-20240501/libfshfs/libfshfs_extent.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/fshfs_catalog_file.h` & `libfshfs-20240501/libfshfs/fshfs_catalog_file.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_catalog_btree_key.c` & `libfshfs-20240501/libfshfs/libfshfs_catalog_btree_key.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_file_entry.c` & `libfshfs-20240501/libfshfs/libfshfs_file_entry.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_definitions.h.in` & `libfshfs-20240501/libfshfs/libfshfs_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_extended_attribute.c` & `libfshfs-20240501/libfshfs/libfshfs_extended_attribute.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_io_handle.h` & `libfshfs-20240501/libfshfs/libfshfs_io_handle.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_libfdatetime.h` & `libfshfs-20240501/libfshfs/libfshfs_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_attributes_btree_file.h` & `libfshfs-20240501/libfshfs/libfshfs_attributes_btree_file.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_volume_header.h` & `libfshfs-20240501/libfshfs/libfshfs_volume_header.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_thread_record.h` & `libfshfs-20240501/libfshfs/libfshfs_thread_record.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_name.h` & `libfshfs-20240501/libfshfs/libfshfs_name.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_libbfio.h` & `libfshfs-20240501/libfshfs/libfshfs_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_extents_btree_file.h` & `libfshfs-20240501/libfshfs/libfshfs_extents_btree_file.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_block_data_handle.h` & `libfshfs-20240501/libfshfs/libfshfs_block_data_handle.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_attributes_btree_key.h` & `libfshfs-20240501/libfshfs/libfshfs_attributes_btree_key.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_name.c` & `libfshfs-20240501/libfshfs/libfshfs_name.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_extent.h` & `libfshfs-20240501/libfshfs/libfshfs_extent.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_catalog_btree_file.c` & `libfshfs-20240501/libfshfs/libfshfs_catalog_btree_file.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_deflate.h` & `libfshfs-20240501/libfshfs/libfshfs_deflate.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_extents_record.c` & `libfshfs-20240501/libfshfs/libfshfs_extents_record.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_btree_node_cache.h` & `libfshfs-20240501/libfshfs/libfshfs_btree_node_cache.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_libfdata.h` & `libfshfs-20240501/libfshfs/libfshfs_libfdata.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/fshfs_attributes_file.h` & `libfshfs-20240501/libfshfs/fshfs_attributes_file.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/fshfs_extents_file.h` & `libfshfs-20240501/libfshfs/fshfs_extents_file.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_support.h` & `libfshfs-20240501/libfshfs/libfshfs_support.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_libcthreads.h` & `libfshfs-20240501/libfshfs/libfshfs_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_volume.c` & `libfshfs-20240501/libfshfs/libfshfs_volume.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/fshfs_volume_header.h` & `libfshfs-20240501/libfshfs/fshfs_volume_header.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_compression.h` & `libfshfs-20240501/libfshfs/libfshfs_compression.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_btree_header.c` & `libfshfs-20240501/libfshfs/libfshfs_btree_header.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_master_directory_block.h` & `libfshfs-20240501/libfshfs/libfshfs_master_directory_block.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_file_system.c` & `libfshfs-20240501/libfshfs/libfshfs_file_system.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_allocation_block_stream.c` & `libfshfs-20240501/libfshfs/libfshfs_allocation_block_stream.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/fshfs_master_directory_block.h` & `libfshfs-20240501/libfshfs/fshfs_master_directory_block.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_libcerror.h` & `libfshfs-20240501/libfshfs/libfshfs_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_compression.c` & `libfshfs-20240501/libfshfs/libfshfs_compression.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_extended_attribute.h` & `libfshfs-20240501/libfshfs/libfshfs_extended_attribute.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_definitions.h` & `libfshfs-20240501/libfshfs/libfshfs_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -33,19 +33,19 @@
 #if !defined( HAVE_LOCAL_LIBFSHFS )
 #include <libfshfs/definitions.h>
 
 /* The definitions in <libfshfs/definitions.h> are copied here
  * for local use of libfshfs
  */
 #else
-#define LIBFSHFS_VERSION					20240221
+#define LIBFSHFS_VERSION					20240501
 
 /* The version string
  */
-#define LIBFSHFS_VERSION_STRING					"20240221"
+#define LIBFSHFS_VERSION_STRING					"20240501"
 
 /* The file access
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBFSHFS_ACCESS_FLAGS
```

### Comparing `libfshfs-20240221/libfshfs/libfshfs_allocation_block_stream.h` & `libfshfs-20240501/libfshfs/libfshfs_allocation_block_stream.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_attribute_record.c` & `libfshfs-20240501/libfshfs/libfshfs_attribute_record.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs.rc.in` & `libfshfs-20240501/libfshfs/libfshfs.rc.in`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_notify.c` & `libfshfs-20240501/libfshfs/libfshfs_notify.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_bit_stream.c` & `libfshfs-20240501/libfshfs/libfshfs_bit_stream.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_btree_file.h` & `libfshfs-20240501/libfshfs/libfshfs_btree_file.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_attributes_btree_key.c` & `libfshfs-20240501/libfshfs/libfshfs_attributes_btree_key.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_file_system.h` & `libfshfs-20240501/libfshfs/libfshfs_file_system.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_buffer_data_handle.h` & `libfshfs-20240501/libfshfs/libfshfs_buffer_data_handle.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/Makefile.in` & `libfshfs-20240501/libfshfs/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -565,14 +565,16 @@
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
@@ -637,16 +639,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -755,15 +757,18 @@
 
 libfshfs_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libfshfs_definitions.h.in \
 	libfshfs.rc \
 	libfshfs.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfshfs_definitions.h \
+	libfshfs.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -1038,24 +1043,71 @@
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
+		-rm -f ./$(DEPDIR)/libfshfs.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_allocation_block_stream.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_attribute_record.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_attributes_btree_file.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_attributes_btree_key.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_bit_stream.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_block_data_handle.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_btree_file.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_btree_header.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_btree_node.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_btree_node_cache.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_btree_node_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_btree_node_record.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_btree_node_vector.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_buffer_data_handle.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_catalog_btree_file.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_catalog_btree_key.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_compressed_data_handle.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_compressed_data_header.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_compression.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_data_stream.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_debug.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_deflate.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_directory_entry.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_directory_record.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_error.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_extended_attribute.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_extent.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_extents_btree_file.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_extents_btree_key.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_extents_record.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_file_entry.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_file_record.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_file_system.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_fork_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_huffman_tree.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_master_directory_block.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_name.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_notify.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_profiler.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_support.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_thread_record.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_volume.Plo
+	-rm -f ./$(DEPDIR)/libfshfs_volume_header.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1183,19 +1235,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libfshfs_definitions.h
-	-rm -f libfshfs.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfshfs ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfshfs_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfshfs-20240221/libfshfs/libfshfs_data_stream.h` & `libfshfs-20240501/libfshfs/libfshfs_data_stream.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_btree_node.c` & `libfshfs-20240501/libfshfs/libfshfs_btree_node.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_attributes_btree_file.c` & `libfshfs-20240501/libfshfs/libfshfs_attributes_btree_file.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_debug.h` & `libfshfs-20240501/libfshfs/libfshfs_debug.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_compressed_data_header.h` & `libfshfs-20240501/libfshfs/libfshfs_compressed_data_header.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_libfmos.h` & `libfshfs-20240501/libfshfs/libfshfs_libfmos.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_extents_btree_key.h` & `libfshfs-20240501/libfshfs/libfshfs_extents_btree_key.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_huffman_tree.c` & `libfshfs-20240501/libfshfs/libfshfs_huffman_tree.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_buffer_data_handle.c` & `libfshfs-20240501/libfshfs/libfshfs_buffer_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs_profiler.c` & `libfshfs-20240501/libfshfs/libfshfs_profiler.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/libfshfs.c` & `libfshfs-20240501/libfshfs/libfshfs.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs/fshfs_fork_descriptor.h` & `libfshfs-20240501/libfshfs/fshfs_fork_descriptor.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/depcomp` & `libfshfs-20240501/depcomp`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfguid/libfguid_error.c` & `libfshfs-20240501/libfguid/libfguid_error.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfguid/libfguid_support.h` & `libfshfs-20240501/libfguid/libfguid_support.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfguid/libfguid_identifier.h` & `libfshfs-20240501/libfguid/libfguid_identifier.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfguid/libfguid_libcerror.h` & `libfshfs-20240501/libfguid/libfguid_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfguid/Makefile.am` & `libfshfs-20240501/libfguid/Makefile.am`

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

### Comparing `libfshfs-20240221/libfguid/libfguid_unused.h` & `libfshfs-20240501/libfguid/libfguid_unused.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfguid/libfguid_extern.h` & `libfshfs-20240501/libfguid/libfguid_extern.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfguid/libfguid_types.h` & `libfshfs-20240501/libfguid/libfguid_types.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfguid/libfguid_identifier.c` & `libfshfs-20240501/libfguid/libfguid_identifier.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfguid/libfguid_support.c` & `libfshfs-20240501/libfguid/libfguid_support.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfguid/libfguid_definitions.h` & `libfshfs-20240501/libfguid/libfguid_definitions.h`

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

### Comparing `libfshfs-20240221/libfguid/Makefile.in` & `libfshfs-20240501/libfguid/Makefile.in`

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
@@ -549,30 +551,31 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -774,24 +777,29 @@
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
 
@@ -877,17 +885,14 @@
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

### Comparing `libfshfs-20240221/libfguid/libfguid_error.h` & `libfshfs-20240501/libfguid/libfguid_error.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/m4/libcfile.m4` & `libfshfs-20240501/m4/libcfile.m4`

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

### Comparing `libfshfs-20240221/m4/libfmos.m4` & `libfshfs-20240501/m4/libfmos.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfmos required headers and functions
 dnl
-dnl Version: 20220804
+dnl Version: 20240413
 
 dnl Function to detect if libfmos is available
 dnl ac_libfmos_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFMOS_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfmos" = xno],
     [ac_cv_libfmos=no],
     [ac_cv_libfmos=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfmos which returns "yes" and --with-libfmos= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfmos" != x && test "x$ac_cv_with_libfmos" != xauto-detect],
+      [test "x$ac_cv_with_libfmos" != x && test "x$ac_cv_with_libfmos" != xauto-detect && test "x$ac_cv_with_libfmos" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfmos"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfmos}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfmos}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfmos],
           [1])
@@ -72,16 +74,17 @@
           fmos,
           libfmos_lzvn_decompress,
           [ac_cv_libfmos_dummy=yes],
           [ac_cv_libfmos=no])
 
         ac_cv_libfmos_LIBADD="-lfmos"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfmos" != x && test "x$ac_cv_with_libfmos" != xauto-detect && test "x$ac_cv_libfmos" != xyes],
+      [test "x$ac_cv_libfmos" != xyes && test "x$ac_cv_with_libfmos" != x && test "x$ac_cv_with_libfmos" != xauto-detect && test "x$ac_cv_with_libfmos" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfmos in directory: $ac_cv_with_libfmos],
         [1])
       ])
     ])
 
   AS_IF(
@@ -103,15 +106,15 @@
     ])
   ])
 
 dnl Function to detect if libfmos dependencies are available
 AC_DEFUN([AX_LIBFMOS_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfmos_CPPFLAGS="-I../libfmos";
+  ac_cv_libfmos_CPPFLAGS="-I../libfmos -I\$(top_srcdir)/libfmos";
   ac_cv_libfmos_LIBADD="../libfmos/libfmos.la";
 
   ac_cv_libfmos=local
   ])
 
 dnl Function to detect how to enable libfmos
 AC_DEFUN([AX_LIBFMOS_CHECK_ENABLE],
```

### Comparing `libfshfs-20240221/m4/libfdatetime.m4` & `libfshfs-20240501/m4/libfdatetime.m4`

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

### Comparing `libfshfs-20240221/m4/tests.m4` & `libfshfs-20240501/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/m4/libcpath.m4` & `libfshfs-20240501/m4/libcpath.m4`

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

### Comparing `libfshfs-20240221/m4/lib-prefix.m4` & `libfshfs-20240501/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/m4/progtest.m4` & `libfshfs-20240501/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/m4/libuna.m4` & `libfshfs-20240501/m4/libuna.m4`

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

### Comparing `libfshfs-20240221/m4/gettext.m4` & `libfshfs-20240501/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/m4/lib-ld.m4` & `libfshfs-20240501/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/m4/libclocale.m4` & `libfshfs-20240501/m4/libclocale.m4`

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

### Comparing `libfshfs-20240221/m4/libcdata.m4` & `libfshfs-20240501/m4/libcdata.m4`

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

### Comparing `libfshfs-20240221/m4/libcsplit.m4` & `libfshfs-20240501/m4/libcsplit.m4`

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

### Comparing `libfshfs-20240221/m4/common.m4` & `libfshfs-20240501/m4/common.m4`

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

### Comparing `libfshfs-20240221/m4/libcthreads.m4` & `libfshfs-20240501/m4/libcthreads.m4`

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

### Comparing `libfshfs-20240221/m4/ltversion.m4` & `libfshfs-20240501/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/m4/ltsugar.m4` & `libfshfs-20240501/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/m4/libfdata.m4` & `libfshfs-20240501/m4/libfdata.m4`

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

### Comparing `libfshfs-20240221/m4/host-cpu-c-abi.m4` & `libfshfs-20240501/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/m4/libfuse.m4` & `libfshfs-20240501/m4/libfuse.m4`

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

### Comparing `libfshfs-20240221/m4/libtool.m4` & `libfshfs-20240501/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/m4/po.m4` & `libfshfs-20240501/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/m4/libcerror.m4` & `libfshfs-20240501/m4/libcerror.m4`

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

### Comparing `libfshfs-20240221/m4/libcnotify.m4` & `libfshfs-20240501/m4/libcnotify.m4`

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

### Comparing `libfshfs-20240221/m4/libfguid.m4` & `libfshfs-20240501/m4/libfguid.m4`

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

### Comparing `libfshfs-20240221/m4/libbfio.m4` & `libfshfs-20240501/m4/libbfio.m4`

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

### Comparing `libfshfs-20240221/m4/libhmac.m4` & `libfshfs-20240501/m4/libhmac.m4`

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

### Comparing `libfshfs-20240221/m4/intlmacosx.m4` & `libfshfs-20240501/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/m4/lt~obsolete.m4` & `libfshfs-20240501/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/m4/lib-link.m4` & `libfshfs-20240501/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/m4/iconv.m4` & `libfshfs-20240501/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/m4/ltoptions.m4` & `libfshfs-20240501/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/m4/nls.m4` & `libfshfs-20240501/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/m4/python.m4` & `libfshfs-20240501/m4/python.m4`

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

### Comparing `libfshfs-20240221/m4/libcrypto.m4` & `libfshfs-20240501/m4/libcrypto.m4`

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

### Comparing `libfshfs-20240221/m4/types.m4` & `libfshfs-20240501/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/m4/libfcache.m4` & `libfshfs-20240501/m4/libfcache.m4`

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

### Comparing `libfshfs-20240221/m4/pthread.m4` & `libfshfs-20240501/m4/pthread.m4`

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

### Comparing `libfshfs-20240221/m4/zlib.m4` & `libfshfs-20240501/m4/zlib.m4`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 dnl Checks for zlib required headers and functions
 dnl
-dnl Version: 20201230
+dnl Version: 20240314
 
 dnl Function to detect if zlib is available
 AC_DEFUN([AX_ZLIB_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_zlib" = xno],
     [ac_cv_zlib=no],
     [ac_cv_zlib=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-zlib which returns "yes" and --with-zlib= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect],
+      [test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect && test "x$ac_cv_with_zlib" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_zlib"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_zlib}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_zlib}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_zlib],
           [1])
@@ -58,14 +60,21 @@
             [Missing function: zlibVersion in library: zlib.],
             [1])
           ])
 
         ac_cv_zlib_LIBADD="-lz";
         ])
       ])
+
+    AS_IF(
+      [test "x$ac_cv_zlib" != xyes && test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect && test "x$ac_cv_with_zlib" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported zlib in directory: $ac_cv_with_zlib],
+        [1])
+      ])
     ])
 
   AS_IF(
     [test "x$ac_cv_zlib" = xzlib],
     [AC_DEFINE(
       [HAVE_ZLIB],
       [1],
```

### Comparing `libfshfs-20240221/include/libfshfs/definitions.h.in` & `libfshfs-20240501/include/libfshfs/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/include/libfshfs/definitions.h` & `libfshfs-20240501/include/libfshfs/definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBFSHFS_DEFINITIONS_H )
 #define _LIBFSHFS_DEFINITIONS_H
 
 #include <libfshfs/types.h>
 
-#define LIBFSHFS_VERSION			20240221
+#define LIBFSHFS_VERSION			20240501
 
 /* The version string
  */
-#define LIBFSHFS_VERSION_STRING			"20240221"
+#define LIBFSHFS_VERSION_STRING			"20240501"
 
 /* The file access
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBFSHFS_ACCESS_FLAGS
```

### Comparing `libfshfs-20240221/include/libfshfs/types.h.in` & `libfshfs-20240501/include/libfshfs/types.h.in`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/include/libfshfs/types.h` & `libfshfs-20240501/include/libfshfs/types.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/include/libfshfs/features.h.in` & `libfshfs-20240501/include/libfshfs/features.h.in`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/include/libfshfs/error.h` & `libfshfs-20240501/include/libfshfs/error.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/include/libfshfs/extern.h` & `libfshfs-20240501/include/libfshfs/extern.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/include/libfshfs/features.h` & `libfshfs-20240501/include/libfshfs/features.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/include/libfshfs/codepage.h` & `libfshfs-20240501/include/libfshfs/codepage.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/include/libfshfs.h` & `libfshfs-20240501/include/libfshfs.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/include/libfshfs.h.in` & `libfshfs-20240501/include/libfshfs.h.in`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/include/Makefile.in` & `libfshfs-20240501/include/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -467,14 +467,16 @@
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
@@ -555,15 +557,20 @@
 
 EXTRA_DIST = \
 	libfshfs.h.in \
 	libfshfs/definitions.h.in \
 	libfshfs/features.h.in \
 	libfshfs/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfshfs.h \
+	libfshfs/definitions.h \
+	libfshfs/features.h \
+	libfshfs/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -760,23 +767,25 @@
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
@@ -858,17 +867,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libfshfs.h
-	-rm -f libfshfs/definitions.h
-	-rm -f libfshfs/features.h
-	-rm -f libfshfs/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfshfs-20240221/common/config_borlandc.h` & `libfshfs-20240501/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/common/file_stream.h` & `libfshfs-20240501/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/common/memory.h` & `libfshfs-20240501/common/memory.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/common/byte_stream.h` & `libfshfs-20240501/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/common/common.h` & `libfshfs-20240501/common/common.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/common/config_winapi.h` & `libfshfs-20240501/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/common/system_string.h` & `libfshfs-20240501/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/common/types.h.in` & `libfshfs-20240501/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/common/types.h` & `libfshfs-20240501/common/types.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/common/config.h.in` & `libfshfs-20240501/common/config.h.in`

 * *Files 0% similar despite different names*

```diff
@@ -245,14 +245,17 @@
 
 /* Define to 1 if you have the <libfmos.h> header file. */
 #undef HAVE_LIBFMOS_H
 
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

### Comparing `libfshfs-20240221/common/config.h` & `libfshfs-20240501/common/config.h`

 * *Files 1% similar despite different names*

```diff
@@ -244,15 +244,18 @@
 /* Define to 1 if you have the `fmos' library (-lfmos). */
 /* #undef HAVE_LIBFMOS */
 
 /* Define to 1 if you have the <libfmos.h> header file. */
 /* #undef HAVE_LIBFMOS_H */
 
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
 
@@ -610,24 +613,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libfshfs"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libfshfs 20240221"
+#define PACKAGE_STRING "libfshfs 20240501"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libfshfs"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240221"
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
-#define VERSION "20240221"
+#define VERSION "20240501"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libfshfs-20240221/common/wide_string.h` & `libfshfs-20240501/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/common/narrow_string.h` & `libfshfs-20240501/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/common/config_msc.h` & `libfshfs-20240501/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/common/Makefile.in` & `libfshfs-20240501/common/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -437,14 +437,16 @@
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
@@ -508,15 +510,17 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -524,15 +528,18 @@
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
@@ -700,23 +707,25 @@
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
@@ -796,15 +805,10 @@
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

### Comparing `libfshfs-20240221/libclocale/libclocale_wide_string.c` & `libfshfs-20240501/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libclocale/libclocale_support.h` & `libfshfs-20240501/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libclocale/Makefile.am` & `libfshfs-20240501/libclocale/Makefile.am`

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

### Comparing `libfshfs-20240221/libclocale/libclocale_definitions.h` & `libfshfs-20240501/libclocale/libclocale_definitions.h`

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

### Comparing `libfshfs-20240221/libclocale/libclocale_unused.h` & `libfshfs-20240501/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libclocale/libclocale_libcerror.h` & `libfshfs-20240501/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libclocale/libclocale_locale.h` & `libfshfs-20240501/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libclocale/libclocale_support.c` & `libfshfs-20240501/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libclocale/libclocale_codepage.c` & `libfshfs-20240501/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libclocale/libclocale_locale.c` & `libfshfs-20240501/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libclocale/Makefile.in` & `libfshfs-20240501/libclocale/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -481,14 +481,16 @@
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
@@ -554,30 +556,31 @@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -780,24 +783,30 @@
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
 
@@ -884,17 +893,14 @@
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

### Comparing `libfshfs-20240221/libclocale/libclocale_extern.h` & `libfshfs-20240501/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libclocale/libclocale_wide_string.h` & `libfshfs-20240501/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libclocale/libclocale_codepage.h` & `libfshfs-20240501/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfcache/libfcache_libcdata.h` & `libfshfs-20240501/libfcache/libfcache_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfcache/libfcache_types.h` & `libfshfs-20240501/libfcache/libfcache_types.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfcache/libfcache_cache_value.c` & `libfshfs-20240501/libfcache/libfcache_cache_value.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfcache/libfcache_unused.h` & `libfshfs-20240501/libfcache/libfcache_unused.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfcache/Makefile.am` & `libfshfs-20240501/libfcache/Makefile.am`

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

### Comparing `libfshfs-20240221/libfcache/libfcache_support.h` & `libfshfs-20240501/libfcache/libfcache_support.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfcache/libfcache_error.h` & `libfshfs-20240501/libfcache/libfcache_error.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfcache/libfcache_support.c` & `libfshfs-20240501/libfcache/libfcache_support.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfcache/libfcache_cache.h` & `libfshfs-20240501/libfcache/libfcache_cache.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfcache/libfcache_error.c` & `libfshfs-20240501/libfcache/libfcache_error.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfcache/libfcache_libcerror.h` & `libfshfs-20240501/libfcache/libfcache_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfcache/libfcache_date_time.c` & `libfshfs-20240501/libfcache/libfcache_date_time.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfcache/libfcache_extern.h` & `libfshfs-20240501/libfcache/libfcache_extern.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfcache/libfcache_cache_value.h` & `libfshfs-20240501/libfcache/libfcache_cache_value.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfcache/Makefile.in` & `libfshfs-20240501/libfcache/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -484,14 +484,16 @@
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
@@ -556,16 +558,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -577,15 +579,16 @@
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
@@ -789,24 +792,31 @@
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
 
@@ -894,17 +904,14 @@
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

### Comparing `libfshfs-20240221/libfcache/libfcache_date_time.h` & `libfshfs-20240501/libfcache/libfcache_date_time.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfcache/libfcache_definitions.h` & `libfshfs-20240501/libfcache/libfcache_definitions.h`

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

### Comparing `libfshfs-20240221/libfcache/libfcache_cache.c` & `libfshfs-20240501/libfcache/libfcache_cache.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/Makefile.am` & `libfshfs-20240501/Makefile.am`

 * *Files 3% similar despite different names*

```diff
@@ -61,16 +61,23 @@
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
+	libfshfs.pc \
+	libfshfs.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 
 pkgconfig_DATA = \
 	libfshfs.pc
 
 libtool: @LIBTOOL_DEPS@
@@ -94,19 +101,7 @@
 	(cd $(srcdir)/libfdata && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdatetime && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfguid && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfmos && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfshfs && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libfshfs.pc
-	-rm -f libfshfs.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
```

### Comparing `libfshfs-20240221/libbfio/libbfio_file_range.h` & `libfshfs-20240501/libbfio/libbfio_file_range.h`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_file_range_io_handle.c` & `libfshfs-20240501/libbfio/libbfio_file_range_io_handle.c`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_support.c` & `libfshfs-20240501/libbfio/libbfio_support.c`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_libcpath.h` & `libfshfs-20240501/libbfio/libbfio_libcpath.h`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_error.h` & `libfshfs-20240501/libbfio/libbfio_error.h`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_libclocale.h` & `libfshfs-20240501/libbfio/libbfio_libclocale.h`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_error.c` & `libfshfs-20240501/libbfio/libbfio_error.c`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_libuna.h` & `libfshfs-20240501/libbfio/libbfio_libuna.h`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_file_io_handle.h` & `libfshfs-20240501/libbfio/libbfio_file_io_handle.h`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_file_pool.h` & `libfshfs-20240501/libbfio/libbfio_file_pool.h`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_file_range.c` & `libfshfs-20240501/libbfio/libbfio_file_range.c`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_types.h` & `libfshfs-20240501/libbfio/libbfio_types.h`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_unused.h` & `libfshfs-20240501/libbfio/libbfio_unused.h`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_libcdata.h` & `libfshfs-20240501/libbfio/libbfio_libcdata.h`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_file.h` & `libfshfs-20240501/libbfio/libbfio_file.h`

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

### Comparing `libfshfs-20240221/libbfio/Makefile.am` & `libfshfs-20240501/libbfio/Makefile.am`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_libcfile.h` & `libfshfs-20240501/libbfio/libbfio_libcfile.h`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_definitions.h` & `libfshfs-20240501/libbfio/libbfio_definitions.h`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_codepage.h` & `libfshfs-20240501/libbfio/libbfio_codepage.h`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_file_io_handle.c` & `libfshfs-20240501/libbfio/libbfio_file_io_handle.c`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_support.h` & `libfshfs-20240501/libbfio/libbfio_support.h`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_memory_range.h` & `libfshfs-20240501/libbfio/libbfio_memory_range.h`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_file_pool.c` & `libfshfs-20240501/libbfio/libbfio_file_pool.c`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_file_range_io_handle.h` & `libfshfs-20240501/libbfio/libbfio_file_range_io_handle.h`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_libcthreads.h` & `libfshfs-20240501/libbfio/libbfio_libcthreads.h`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_system_string.h` & `libfshfs-20240501/libbfio/libbfio_system_string.h`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_memory_range_io_handle.c` & `libfshfs-20240501/libbfio/libbfio_memory_range_io_handle.c`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_handle.c` & `libfshfs-20240501/libbfio/libbfio_handle.c`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_file.c` & `libfshfs-20240501/libbfio/libbfio_file.c`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_handle.h` & `libfshfs-20240501/libbfio/libbfio_handle.h`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_memory_range.c` & `libfshfs-20240501/libbfio/libbfio_memory_range.c`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_pool.c` & `libfshfs-20240501/libbfio/libbfio_pool.c`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_libcerror.h` & `libfshfs-20240501/libbfio/libbfio_libcerror.h`

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

### Comparing `libfshfs-20240221/libbfio/Makefile.in` & `libfshfs-20240501/libbfio/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -502,14 +502,16 @@
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
@@ -574,16 +576,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -614,15 +616,16 @@
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
@@ -833,24 +836,38 @@
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
 
@@ -919,14 +936,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -937,23 +956,22 @@
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

### Comparing `libfshfs-20240221/libbfio/libbfio_system_string.c` & `libfshfs-20240501/libbfio/libbfio_system_string.c`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_memory_range_io_handle.h` & `libfshfs-20240501/libbfio/libbfio_memory_range_io_handle.h`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_extern.h` & `libfshfs-20240501/libbfio/libbfio_extern.h`

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

### Comparing `libfshfs-20240221/libbfio/libbfio_pool.h` & `libfshfs-20240501/libbfio/libbfio_pool.h`

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

### Comparing `libfshfs-20240221/config.guess` & `libfshfs-20240501/config.guess`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/dpkg/copyright` & `libfshfs-20240501/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/dpkg/control` & `libfshfs-20240501/dpkg/control`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/dpkg/rules` & `libfshfs-20240501/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/COPYING.LESSER` & `libfshfs-20240501/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/configure` & `libfshfs-20240501/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libfshfs 20240221.
+# Generated by GNU Autoconf 2.71 for libfshfs 20240501.
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
 PACKAGE_NAME='libfshfs'
 PACKAGE_TARNAME='libfshfs'
-PACKAGE_VERSION='20240221'
-PACKAGE_STRING='libfshfs 20240221'
+PACKAGE_VERSION='20240501'
+PACKAGE_STRING='libfshfs 20240501'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libfshfs.h.in"
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
@@ -1156,14 +1158,16 @@
 libfmos_LIBS
 zlib_CFLAGS
 zlib_LIBS
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
@@ -1706,15 +1710,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libfshfs 20240221 to adapt to many kinds of systems.
+\`configure' configures libfshfs 20240501 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1777,15 +1781,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libfshfs 20240221:";;
+     short | recursive ) echo "Configuration of libfshfs 20240501:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1988,14 +1992,17 @@
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
@@ -2058,15 +2065,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libfshfs configure 20240221
+libfshfs configure 20240501
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2779,15 +2786,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libfshfs $as_me 20240221, which was
+It was created by libfshfs $as_me 20240501, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4268,15 +4275,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libfshfs'
- VERSION='20240221'
+ VERSION='20240501'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -23863,15 +23870,15 @@
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
@@ -24362,15 +24369,16 @@
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
@@ -24512,15 +24520,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -24614,15 +24622,15 @@
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
@@ -26254,15 +26262,15 @@
 
 
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
@@ -26316,47 +26324,52 @@
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
@@ -26390,15 +26403,15 @@
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
@@ -26432,15 +26445,15 @@
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
@@ -26475,15 +26488,15 @@
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
@@ -26517,15 +26530,15 @@
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
@@ -26559,15 +26572,15 @@
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
@@ -26601,15 +26614,15 @@
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
@@ -26643,15 +26656,15 @@
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
@@ -26686,15 +26699,15 @@
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
@@ -26728,15 +26741,15 @@
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
@@ -26770,15 +26783,15 @@
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
@@ -26812,15 +26825,15 @@
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
@@ -26854,15 +26867,15 @@
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
@@ -26897,15 +26910,15 @@
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
@@ -26939,15 +26952,15 @@
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
@@ -26981,15 +26994,15 @@
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
@@ -27023,15 +27036,15 @@
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
@@ -27065,15 +27078,15 @@
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
@@ -27108,67 +27121,76 @@
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
 
@@ -27256,15 +27278,15 @@
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
@@ -31035,15 +31057,16 @@
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
@@ -31068,15 +31091,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcdata" != xyes
 then :
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDATA 1" >>confdefs.h
@@ -31146,15 +31169,15 @@
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
@@ -31701,15 +31724,16 @@
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
@@ -31865,15 +31889,15 @@
 
 printf "%s\n" "#define HAVE_LANGINFO_CODESET 1" >>confdefs.h
 
 
 fi
 
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCLOCALE 1" >>confdefs.h
@@ -31943,15 +31967,15 @@
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
@@ -32401,15 +32425,16 @@
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
@@ -32464,15 +32489,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -32542,15 +32567,15 @@
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
@@ -33265,15 +33290,16 @@
 
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
@@ -33298,15 +33324,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcsplit" != xyes
 then :
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCSPLIT 1" >>confdefs.h
@@ -33376,15 +33402,15 @@
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
@@ -40586,15 +40612,16 @@
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
@@ -40619,15 +40646,15 @@
 
 fi
 
 
     if test "x$ac_cv_libuna" != xyes
 then :
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBUNA 1" >>confdefs.h
@@ -40697,15 +40724,15 @@
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
@@ -41886,15 +41913,16 @@
 
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
@@ -42208,15 +42236,15 @@
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
@@ -42286,15 +42314,15 @@
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
@@ -43091,15 +43119,16 @@
 
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
@@ -43289,15 +43318,15 @@
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: mkdir
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCPATH 1" >>confdefs.h
@@ -43367,15 +43396,15 @@
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
@@ -45485,15 +45514,16 @@
 
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
@@ -45518,15 +45548,15 @@
 
 fi
 
 
     if test "x$ac_cv_libbfio" != xyes
 then :
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBBFIO 1" >>confdefs.h
@@ -45596,15 +45626,15 @@
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
@@ -46516,15 +46546,16 @@
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
@@ -46617,15 +46648,15 @@
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
@@ -46695,15 +46726,15 @@
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
@@ -49983,15 +50014,16 @@
 
 
 
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
@@ -50016,15 +50048,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdata" != xyes
 then :
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATA 1" >>confdefs.h
@@ -50094,15 +50126,15 @@
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
@@ -53538,15 +53570,16 @@
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
@@ -53571,15 +53604,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdatetime" != xyes
 then :
 
-  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime";
+  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime -I\$(top_srcdir)/libfdatetime";
   ac_cv_libfdatetime_LIBADD="../libfdatetime/libfdatetime.la";
 
   ac_cv_libfdatetime=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATETIME 1" >>confdefs.h
@@ -53649,15 +53682,15 @@
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
@@ -54231,15 +54264,16 @@
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
@@ -54264,15 +54298,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfguid" != xyes
 then :
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFGUID 1" >>confdefs.h
@@ -54342,15 +54376,15 @@
 printf "%s\n" "$ac_cv_with_libfmos" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfmos" = xno
 then :
   ac_cv_libfmos=no
 else $as_nop
   ac_cv_libfmos=check
-        if test "x$ac_cv_with_libfmos" != x && test "x$ac_cv_with_libfmos" != xauto-detect
+                if test "x$ac_cv_with_libfmos" != x && test "x$ac_cv_with_libfmos" != xauto-detect && test "x$ac_cv_with_libfmos" != xyes
 then :
   if test -d "$ac_cv_with_libfmos"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfmos}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfmos}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -54632,15 +54666,16 @@
 fi
 
 
         ac_cv_libfmos_LIBADD="-lfmos"
 fi
 
 fi
-    if test "x$ac_cv_with_libfmos" != x && test "x$ac_cv_with_libfmos" != xauto-detect && test "x$ac_cv_libfmos" != xyes
+
+    if test "x$ac_cv_libfmos" != xyes && test "x$ac_cv_with_libfmos" != x && test "x$ac_cv_with_libfmos" != xauto-detect && test "x$ac_cv_with_libfmos" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfmos in directory: $ac_cv_with_libfmos
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -54665,15 +54700,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfmos" != xyes
 then :
 
-  ac_cv_libfmos_CPPFLAGS="-I../libfmos";
+  ac_cv_libfmos_CPPFLAGS="-I../libfmos -I\$(top_srcdir)/libfmos";
   ac_cv_libfmos_LIBADD="../libfmos/libfmos.la";
 
   ac_cv_libfmos=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFMOS 1" >>confdefs.h
@@ -54743,15 +54778,15 @@
 printf "%s\n" "$ac_cv_with_zlib" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_zlib" = xno
 then :
   ac_cv_zlib=no
 else $as_nop
   ac_cv_zlib=check
-        if test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect
+                if test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect && test "x$ac_cv_with_zlib" != xyes
 then :
   if test -d "$ac_cv_with_zlib"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_zlib}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_zlib}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -54918,14 +54953,23 @@
 
         ac_cv_zlib_LIBADD="-lz";
 
 fi
 
 fi
 
+    if test "x$ac_cv_zlib" != xyes && test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect && test "x$ac_cv_with_zlib" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported zlib in directory: $ac_cv_with_zlib
+See \`config.log' for more details" "$LINENO" 5; }
+
+fi
+
 fi
 
   if test "x$ac_cv_zlib" = xzlib
 then :
 
 printf "%s\n" "#define HAVE_ZLIB 1" >>confdefs.h
 
@@ -55297,16 +55341,20 @@
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
 
@@ -55469,15 +55517,15 @@
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
@@ -56475,15 +56523,16 @@
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
@@ -56589,15 +56638,15 @@
 
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
@@ -60775,15 +60824,15 @@
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
@@ -60848,33 +60897,107 @@
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
@@ -60942,51 +61065,110 @@
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
@@ -61149,45 +61331,38 @@
 then :
   ac_cv_libfuse_dummy=yes
 else $as_nop
   ac_cv_libfuse=no
 fi
 
 
-        ac_cv_libfuse_LIBADD="-lfuse";
+                ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
+        if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ac_cv_libfuse_LIBADD="-lfuse3"
+else $as_nop
+  ac_cv_libfuse_LIBADD="-lfuse"
+fi
 
 fi
 
 fi
 
         if test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno
 then :
-  CPPFLAGS="$CPPFLAGS -DFUSE_USE_VERSION=26"
+  CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
       ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_osxfuse_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_OSXFUSE_FUSE_H 1" >>confdefs.h
 
 fi
 
 
-            if test "x$ac_cv_header_osxfuse_fuse_h" = xno
-then :
-  { ac_cv_header_osxfuse_fuse_h=; unset ac_cv_header_osxfuse_fuse_h;}
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64"
-        ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
-if test "x$ac_cv_header_osxfuse_fuse_h" = xyes
-then :
-  printf "%s\n" "#define HAVE_OSXFUSE_FUSE_H 1" >>confdefs.h
-
-fi
-
-
-fi
-
       if test "x$ac_cv_header_osxfuse_fuse_h" = xno
 then :
   ac_cv_libfuse=no
 else $as_nop
           ac_cv_libfuse=libosxfuse
 
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_daemonize in -losxfuse" >&5
@@ -61355,29 +61530,49 @@
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
@@ -61408,14 +61603,20 @@
 
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
 
@@ -61423,14 +61624,22 @@
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
 
@@ -62362,15 +62571,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libfshfs $as_me 20240221, which was
+This file was extended by libfshfs $as_me 20240501, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -62430,15 +62639,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libfshfs config.status 20240221
+libfshfs config.status 20240501
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libfshfs-20240221/pyfshfs/pyfshfs_datetime.c` & `libfshfs-20240501/pyfshfs/pyfshfs_datetime.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/pyfshfs/pyfshfs_volume.h` & `libfshfs-20240501/pyfshfs/pyfshfs_volume.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/pyfshfs/pyfshfs_extended_attributes.h` & `libfshfs-20240501/pyfshfs/pyfshfs_extended_attributes.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/pyfshfs/pyfshfs_extended_attribute.h` & `libfshfs-20240501/pyfshfs/pyfshfs_extended_attribute.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/pyfshfs/pyfshfs_integer.c` & `libfshfs-20240501/pyfshfs/pyfshfs_integer.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/pyfshfs/pyfshfs_file_entries.c` & `libfshfs-20240501/pyfshfs/pyfshfs_file_entries.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/pyfshfs/pyfshfs_data_stream.h` & `libfshfs-20240501/pyfshfs/pyfshfs_data_stream.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/pyfshfs/pyfshfs_file_object_io_handle.h` & `libfshfs-20240501/pyfshfs/pyfshfs_file_object_io_handle.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/pyfshfs/pyfshfs_libbfio.h` & `libfshfs-20240501/pyfshfs/pyfshfs_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/pyfshfs/Makefile.am` & `libfshfs-20240501/pyfshfs/Makefile.am`

 * *Files 15% similar despite different names*

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
@@ -44,14 +44,11 @@
 	@LIBBFIO_LIBADD@
 
 pyfshfs_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pyfshfs_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
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

### Comparing `libfshfs-20240221/pyfshfs/pyfshfs_error.c` & `libfshfs-20240501/pyfshfs/pyfshfs_error.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/pyfshfs/pyfshfs_extended_attribute.c` & `libfshfs-20240501/pyfshfs/pyfshfs_extended_attribute.c`

 * *Files 0% similar despite different names*

```diff
@@ -42,22 +42,22 @@
 	  "get_name() -> Unicode string\n"
 	  "\n"
 	  "Retrieves the name." },
 
 	{ "read_buffer",
 	  (PyCFunction) pyfshfs_extended_attribute_read_buffer,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read_buffer(size) -> Binary string\n"
+	  "read_buffer(size)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data." },
 
 	{ "read_buffer_at_offset",
 	  (PyCFunction) pyfshfs_extended_attribute_read_buffer_at_offset,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read_buffer_at_offset(size, offset) -> Binary string\n"
+	  "read_buffer_at_offset(size, offset)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data at a specific offset." },
 
 	{ "seek_offset",
 	  (PyCFunction) pyfshfs_extended_attribute_seek_offset,
 	  METH_VARARGS | METH_KEYWORDS,
 	  "seek_offset(offset, whence) -> None\n"
@@ -70,15 +70,15 @@
 	  "get_offset() -> Integer\n"
 	  "\n"
 	  "Retrieves the current offset within the data." },
 
 	{ "read",
 	  (PyCFunction) pyfshfs_extended_attribute_read_buffer,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read(size) -> Binary string\n"
+	  "read(size)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data." },
 
 	{ "seek",
 	  (PyCFunction) pyfshfs_extended_attribute_seek_offset,
 	  METH_VARARGS | METH_KEYWORDS,
 	  "seek(offset, whence) -> None\n"
```

### Comparing `libfshfs-20240221/pyfshfs/pyfshfs_unused.h` & `libfshfs-20240501/pyfshfs/pyfshfs_unused.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/pyfshfs/pyfshfs_file_object_io_handle.c` & `libfshfs-20240501/pyfshfs/pyfshfs_file_object_io_handle.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/pyfshfs/pyfshfs.h` & `libfshfs-20240501/pyfshfs/pyfshfs.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/pyfshfs/pyfshfs_file_entry.c` & `libfshfs-20240501/pyfshfs/pyfshfs_file_entry.c`

 * *Files 0% similar despite different names*

```diff
@@ -258,22 +258,22 @@
 	  "get_sub_file_entry_by_name(name) -> Object or None\n"
 	  "\n"
 	  "Retrieves the sub file entry for an UTF-8 encoded name specified by the name." },
 
 	{ "read_buffer",
 	  (PyCFunction) pyfshfs_file_entry_read_buffer,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read_buffer(size) -> Binary string\n"
+	  "read_buffer(size)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data at the current offset." },
 
 	{ "read_buffer_at_offset",
 	  (PyCFunction) pyfshfs_file_entry_read_buffer_at_offset,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read_buffer_at_offset(size, offset) -> Binary string\n"
+	  "read_buffer_at_offset(size, offset)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data at a specific offset." },
 
 	{ "seek_offset",
 	  (PyCFunction) pyfshfs_file_entry_seek_offset,
 	  METH_VARARGS | METH_KEYWORDS,
 	  "seek_offset(offset, whence) -> None\n"
@@ -286,15 +286,15 @@
 	  "get_offset() -> Integer\n"
 	  "\n"
 	  "Retrieves the current offset of the data." },
 
 	{ "read",
 	  (PyCFunction) pyfshfs_file_entry_read_buffer,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read(size) -> Binary string\n"
+	  "read(size)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data at the current offset." },
 
 	{ "seek",
 	  (PyCFunction) pyfshfs_file_entry_seek_offset,
 	  METH_VARARGS | METH_KEYWORDS,
 	  "seek(offset, whence) -> None\n"
```

### Comparing `libfshfs-20240221/pyfshfs/pyfshfs_integer.h` & `libfshfs-20240501/pyfshfs/pyfshfs_integer.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/pyfshfs/pyfshfs_file_entry.h` & `libfshfs-20240501/pyfshfs/pyfshfs_file_entry.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/pyfshfs/pyfshfs_error.h` & `libfshfs-20240501/pyfshfs/pyfshfs_error.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/pyfshfs/pyfshfs_extended_attributes.c` & `libfshfs-20240501/pyfshfs/pyfshfs_extended_attributes.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/pyfshfs/pyfshfs_data_stream.c` & `libfshfs-20240501/pyfshfs/pyfshfs_data_stream.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/pyfshfs/pyfshfs_python.h` & `libfshfs-20240501/pyfshfs/pyfshfs_python.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/pyfshfs/Makefile.in` & `libfshfs-20240501/pyfshfs/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -531,14 +531,16 @@
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
@@ -603,16 +605,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -647,15 +649,16 @@
 @HAVE_PYTHON_TRUE@	@LIBUNA_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBBFIO_LIBADD@
 
 @HAVE_PYTHON_TRUE@pyfshfs_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pyfshfs_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -969,24 +972,37 @@
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
+		-rm -f ./$(DEPDIR)/pyfshfs_la-pyfshfs.Plo
+	-rm -f ./$(DEPDIR)/pyfshfs_la-pyfshfs_data_stream.Plo
+	-rm -f ./$(DEPDIR)/pyfshfs_la-pyfshfs_datetime.Plo
+	-rm -f ./$(DEPDIR)/pyfshfs_la-pyfshfs_error.Plo
+	-rm -f ./$(DEPDIR)/pyfshfs_la-pyfshfs_extended_attribute.Plo
+	-rm -f ./$(DEPDIR)/pyfshfs_la-pyfshfs_extended_attributes.Plo
+	-rm -f ./$(DEPDIR)/pyfshfs_la-pyfshfs_file_entries.Plo
+	-rm -f ./$(DEPDIR)/pyfshfs_la-pyfshfs_file_entry.Plo
+	-rm -f ./$(DEPDIR)/pyfshfs_la-pyfshfs_file_object_io_handle.Plo
+	-rm -f ./$(DEPDIR)/pyfshfs_la-pyfshfs_integer.Plo
+	-rm -f ./$(DEPDIR)/pyfshfs_la-pyfshfs_volume.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1081,14 +1097,10 @@
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

### Comparing `libfshfs-20240221/pyfshfs/pyfshfs_libcerror.h` & `libfshfs-20240501/pyfshfs/pyfshfs_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/pyfshfs/pyfshfs_datetime.h` & `libfshfs-20240501/pyfshfs/pyfshfs_datetime.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/pyfshfs/pyfshfs.c` & `libfshfs-20240501/pyfshfs/pyfshfs.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/pyfshfs/pyfshfs_libfshfs.h` & `libfshfs-20240501/pyfshfs/pyfshfs_libfshfs.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/pyfshfs/pyfshfs_file_entries.h` & `libfshfs-20240501/pyfshfs/pyfshfs_file_entries.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/pyfshfs/pyfshfs_volume.c` & `libfshfs-20240501/pyfshfs/pyfshfs_volume.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/compile` & `libfshfs-20240501/compile`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/missing` & `libfshfs-20240501/missing`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/libfdata/libfdata.vcproj` & `libfshfs-20240501/msvscpp/libfdata/libfdata.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_tools_signal/fshfs_test_tools_signal.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_tools_signal/fshfs_test_tools_signal.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_btree_node_descriptor/fshfs_test_btree_node_descriptor.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_btree_node_descriptor/fshfs_test_btree_node_descriptor.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/libfmos/libfmos.vcproj` & `libfshfs-20240501/msvscpp/libfmos/libfmos.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_tools_output/fshfs_test_tools_output.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_tools_output/fshfs_test_tools_output.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_file_record/fshfs_test_file_record.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_file_record/fshfs_test_file_record.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/libfshfs/libfshfs.vcproj` & `libfshfs-20240501/msvscpp/libfshfs/libfshfs.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/zlib/zlib.vcproj` & `libfshfs-20240501/msvscpp/zlib/zlib.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_thread_record/fshfs_test_thread_record.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_thread_record/fshfs_test_thread_record.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/libfguid/libfguid.vcproj` & `libfshfs-20240501/msvscpp/libfguid/libfguid.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/libclocale/libclocale.vcproj` & `libfshfs-20240501/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_file_system/fshfs_test_file_system.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_file_system/fshfs_test_file_system.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_name/fshfs_test_name.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_name/fshfs_test_name.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_io_handle/fshfs_test_io_handle.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_io_handle/fshfs_test_io_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_directory_entry/fshfs_test_directory_entry.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_directory_entry/fshfs_test_directory_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/libfcache/libfcache.vcproj` & `libfshfs-20240501/msvscpp/libfcache/libfcache.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/Makefile.am` & `libfshfs-20240501/msvscpp/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -56,13 +56,11 @@
 	pyfshfs/pyfshfs.vcproj \
 	zlib/zlib.vcproj \
 	libfshfs.sln
 
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

### Comparing `libfshfs-20240221/msvscpp/libbfio/libbfio.vcproj` & `libfshfs-20240501/msvscpp/libbfio/libbfio.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/pyfshfs/pyfshfs.vcproj` & `libfshfs-20240501/msvscpp/pyfshfs/pyfshfs.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfsmount/fshfsmount.vcproj` & `libfshfs-20240501/msvscpp/fshfsmount/fshfsmount.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_deflate/fshfs_test_deflate.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_deflate/fshfs_test_deflate.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_notify/fshfs_test_notify.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_notify/fshfs_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_compression/fshfs_test_compression.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_compression/fshfs_test_compression.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/libcfile/libcfile.vcproj` & `libfshfs-20240501/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_error/fshfs_test_error.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_error/fshfs_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_fork_descriptor/fshfs_test_fork_descriptor.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_fork_descriptor/fshfs_test_fork_descriptor.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/libcdata/libcdata.vcproj` & `libfshfs-20240501/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_btree_header/fshfs_test_btree_header.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_btree_header/fshfs_test_btree_header.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfsinfo/fshfsinfo.vcproj` & `libfshfs-20240501/msvscpp/fshfsinfo/fshfsinfo.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_master_directory_block/fshfs_test_master_directory_block.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_master_directory_block/fshfs_test_master_directory_block.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/libfshfs.sln` & `libfshfs-20240501/msvscpp/libfshfs.sln`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_btree_file/fshfs_test_btree_file.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_btree_file/fshfs_test_btree_file.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_huffman_tree/fshfs_test_huffman_tree.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_huffman_tree/fshfs_test_huffman_tree.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/libcthreads/libcthreads.vcproj` & `libfshfs-20240501/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_btree_node_record/fshfs_test_btree_node_record.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_btree_node_record/fshfs_test_btree_node_record.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_attributes_btree_key/fshfs_test_attributes_btree_key.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_attributes_btree_key/fshfs_test_attributes_btree_key.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_bit_stream/fshfs_test_bit_stream.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_bit_stream/fshfs_test_bit_stream.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/libcpath/libcpath.vcproj` & `libfshfs-20240501/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_catalog_btree_key/fshfs_test_catalog_btree_key.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_catalog_btree_key/fshfs_test_catalog_btree_key.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_extents_btree_key/fshfs_test_extents_btree_key.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_extents_btree_key/fshfs_test_extents_btree_key.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_compressed_data_handle/fshfs_test_compressed_data_handle.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_compressed_data_handle/fshfs_test_compressed_data_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_extent/fshfs_test_extent.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_extent/fshfs_test_extent.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_directory_record/fshfs_test_directory_record.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_directory_record/fshfs_test_directory_record.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/libhmac/libhmac.vcproj` & `libfshfs-20240501/msvscpp/libhmac/libhmac.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/libcsplit/libcsplit.vcproj` & `libfshfs-20240501/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/libuna/libuna.vcproj` & `libfshfs-20240501/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/Makefile.in` & `libfshfs-20240501/msvscpp/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -419,14 +419,16 @@
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
@@ -552,15 +554,16 @@
 	pyfshfs/pyfshfs.vcproj \
 	zlib/zlib.vcproj \
 	libfshfs.sln
 
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
@@ -664,23 +667,25 @@
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
@@ -759,13 +764,10 @@
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

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_profiler/fshfs_test_profiler.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_profiler/fshfs_test_profiler.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_support/fshfs_test_support.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_support/fshfs_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_attribute_record/fshfs_test_attribute_record.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_attribute_record/fshfs_test_attribute_record.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_btree_node/fshfs_test_btree_node.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_btree_node/fshfs_test_btree_node.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_volume/fshfs_test_volume.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_volume/fshfs_test_volume.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/libcnotify/libcnotify.vcproj` & `libfshfs-20240501/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_file_entry/fshfs_test_file_entry.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_file_entry/fshfs_test_file_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_tools_info_handle/fshfs_test_tools_info_handle.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_tools_info_handle/fshfs_test_tools_info_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/libcerror/libcerror.vcproj` & `libfshfs-20240501/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/libfdatetime/libfdatetime.vcproj` & `libfshfs-20240501/msvscpp/libfdatetime/libfdatetime.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_volume_header/fshfs_test_volume_header.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_volume_header/fshfs_test_volume_header.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/msvscpp/fshfs_test_buffer_data_handle/fshfs_test_buffer_data_handle.vcproj` & `libfshfs-20240501/msvscpp/fshfs_test_buffer_data_handle/fshfs_test_buffer_data_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcfile/libcfile_extern.h` & `libfshfs-20240501/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcfile/libcfile_support.h` & `libfshfs-20240501/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcfile/libcfile_unused.h` & `libfshfs-20240501/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcfile/libcfile_notify.h` & `libfshfs-20240501/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcfile/libcfile_support.c` & `libfshfs-20240501/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcfile/libcfile_types.h` & `libfshfs-20240501/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcfile/Makefile.am` & `libfshfs-20240501/libcfile/Makefile.am`

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

### Comparing `libfshfs-20240221/libcfile/libcfile_notify.c` & `libfshfs-20240501/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcfile/libcfile_system_string.h` & `libfshfs-20240501/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcfile/libcfile_file.h` & `libfshfs-20240501/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcfile/libcfile_libcnotify.h` & `libfshfs-20240501/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcfile/libcfile_system_string.c` & `libfshfs-20240501/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcfile/libcfile_error.h` & `libfshfs-20240501/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcfile/libcfile_libcerror.h` & `libfshfs-20240501/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcfile/libcfile_file.c` & `libfshfs-20240501/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcfile/libcfile_libclocale.h` & `libfshfs-20240501/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcfile/libcfile_winapi.h` & `libfshfs-20240501/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcfile/Makefile.in` & `libfshfs-20240501/libcfile/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -484,14 +484,16 @@
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
@@ -556,16 +558,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -580,15 +582,16 @@
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
@@ -793,24 +796,32 @@
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
 
@@ -899,17 +910,14 @@
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

### Comparing `libfshfs-20240221/libcfile/libcfile_error.c` & `libfshfs-20240501/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcfile/libcfile_libuna.h` & `libfshfs-20240501/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcfile/libcfile_winapi.c` & `libfshfs-20240501/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcfile/libcfile_definitions.h` & `libfshfs-20240501/libcfile/libcfile_definitions.h`

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

### Comparing `libfshfs-20240221/README` & `libfshfs-20240501/README`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/INSTALL` & `libfshfs-20240501/INSTALL`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcdata/libcdata_list_element.h` & `libfshfs-20240501/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcdata/libcdata_array.h` & `libfshfs-20240501/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcdata/libcdata_definitions.h` & `libfshfs-20240501/libcdata/libcdata_definitions.h`

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

### Comparing `libfshfs-20240221/libcdata/libcdata_libcerror.h` & `libfshfs-20240501/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcdata/libcdata_unused.h` & `libfshfs-20240501/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcdata/libcdata_btree.h` & `libfshfs-20240501/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcdata/libcdata_btree.c` & `libfshfs-20240501/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcdata/libcdata_support.c` & `libfshfs-20240501/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcdata/libcdata_list.c` & `libfshfs-20240501/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcdata/libcdata_extern.h` & `libfshfs-20240501/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcdata/libcdata_list.h` & `libfshfs-20240501/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcdata/libcdata_btree_values_list.h` & `libfshfs-20240501/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcdata/Makefile.am` & `libfshfs-20240501/libcdata/Makefile.am`

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

### Comparing `libfshfs-20240221/libcdata/libcdata_btree_node.h` & `libfshfs-20240501/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcdata/libcdata_range_list_value.h` & `libfshfs-20240501/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcdata/libcdata_range_list.h` & `libfshfs-20240501/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcdata/libcdata_range_list.c` & `libfshfs-20240501/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcdata/libcdata_array.c` & `libfshfs-20240501/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcdata/libcdata_list_element.c` & `libfshfs-20240501/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcdata/libcdata_libcthreads.h` & `libfshfs-20240501/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcdata/libcdata_tree_node.h` & `libfshfs-20240501/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcdata/libcdata_error.h` & `libfshfs-20240501/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcdata/libcdata_types.h` & `libfshfs-20240501/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcdata/libcdata_btree_node.c` & `libfshfs-20240501/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcdata/libcdata_tree_node.c` & `libfshfs-20240501/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcdata/libcdata_support.h` & `libfshfs-20240501/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcdata/Makefile.in` & `libfshfs-20240501/libcdata/Makefile.in`

 * *Files 2% similar despite different names*

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
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -596,15 +598,16 @@
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
@@ -814,24 +817,37 @@
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
 
@@ -925,17 +941,14 @@
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

### Comparing `libfshfs-20240221/libcdata/libcdata_range_list_value.c` & `libfshfs-20240501/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcdata/libcdata_btree_values_list.c` & `libfshfs-20240501/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcdata/libcdata_error.c` & `libfshfs-20240501/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/config.sub` & `libfshfs-20240501/config.sub`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs.pc.in` & `libfshfs-20240501/libfshfs.pc.in`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/setup.py` & `libfshfs-20240501/setup.py`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/acinclude.m4` & `libfshfs-20240501/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/config.rpath` & `libfshfs-20240501/config.rpath`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcthreads/libcthreads_thread.h` & `libfshfs-20240501/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcthreads/libcthreads_read_write_lock.h` & `libfshfs-20240501/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcthreads/libcthreads_thread.c` & `libfshfs-20240501/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcthreads/libcthreads_thread_pool.h` & `libfshfs-20240501/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcthreads/libcthreads_support.h` & `libfshfs-20240501/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcthreads/libcthreads_lock.h` & `libfshfs-20240501/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcthreads/libcthreads_unused.h` & `libfshfs-20240501/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcthreads/libcthreads_lock.c` & `libfshfs-20240501/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcthreads/libcthreads_condition.h` & `libfshfs-20240501/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcthreads/libcthreads_repeating_thread.h` & `libfshfs-20240501/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcthreads/Makefile.am` & `libfshfs-20240501/libcthreads/Makefile.am`

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

### Comparing `libfshfs-20240221/libcthreads/libcthreads_support.c` & `libfshfs-20240501/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcthreads/libcthreads_mutex.c` & `libfshfs-20240501/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcthreads/libcthreads_queue.c` & `libfshfs-20240501/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcthreads/libcthreads_mutex.h` & `libfshfs-20240501/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcthreads/libcthreads_types.h` & `libfshfs-20240501/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcthreads/libcthreads_thread_attributes.h` & `libfshfs-20240501/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcthreads/libcthreads_condition.c` & `libfshfs-20240501/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcthreads/libcthreads_error.c` & `libfshfs-20240501/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcthreads/libcthreads_read_write_lock.c` & `libfshfs-20240501/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcthreads/libcthreads_libcerror.h` & `libfshfs-20240501/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcthreads/libcthreads_definitions.h` & `libfshfs-20240501/libcthreads/libcthreads_definitions.h`

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

### Comparing `libfshfs-20240221/libcthreads/libcthreads_thread_pool.c` & `libfshfs-20240501/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcthreads/libcthreads_error.h` & `libfshfs-20240501/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcthreads/libcthreads_thread_attributes.c` & `libfshfs-20240501/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcthreads/libcthreads_extern.h` & `libfshfs-20240501/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcthreads/libcthreads_repeating_thread.c` & `libfshfs-20240501/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcthreads/Makefile.in` & `libfshfs-20240501/libcthreads/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -502,14 +502,16 @@
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
@@ -574,16 +576,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -598,15 +600,16 @@
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
@@ -816,24 +819,37 @@
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
 
@@ -927,17 +943,14 @@
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

### Comparing `libfshfs-20240221/libcthreads/libcthreads_queue.h` & `libfshfs-20240501/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/test-driver` & `libfshfs-20240501/test-driver`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcpath/libcpath_support.c` & `libfshfs-20240501/libcpath/libcpath_support.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcpath/libcpath_libcerror.h` & `libfshfs-20240501/libcpath/libcpath_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcpath/libcpath_definitions.h` & `libfshfs-20240501/libcpath/libcpath_definitions.h`

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

### Comparing `libfshfs-20240221/libcpath/Makefile.am` & `libfshfs-20240501/libcpath/Makefile.am`

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

### Comparing `libfshfs-20240221/libcpath/libcpath_error.c` & `libfshfs-20240501/libcpath/libcpath_error.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcpath/libcpath_extern.h` & `libfshfs-20240501/libcpath/libcpath_extern.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcpath/libcpath_system_string.h` & `libfshfs-20240501/libcpath/libcpath_system_string.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcpath/libcpath_support.h` & `libfshfs-20240501/libcpath/libcpath_support.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcpath/libcpath_libcsplit.h` & `libfshfs-20240501/libcpath/libcpath_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcpath/libcpath_system_string.c` & `libfshfs-20240501/libcpath/libcpath_system_string.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcpath/libcpath_libclocale.h` & `libfshfs-20240501/libcpath/libcpath_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcpath/libcpath_error.h` & `libfshfs-20240501/libcpath/libcpath_error.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcpath/Makefile.in` & `libfshfs-20240501/libcpath/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -478,14 +478,16 @@
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
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -571,15 +573,16 @@
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
@@ -782,24 +785,30 @@
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
 
@@ -886,17 +895,14 @@
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

### Comparing `libfshfs-20240221/libcpath/libcpath_libuna.h` & `libfshfs-20240501/libcpath/libcpath_libuna.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcpath/libcpath_unused.h` & `libfshfs-20240501/libcpath/libcpath_unused.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcpath/libcpath_path.c` & `libfshfs-20240501/libcpath/libcpath_path.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcpath/libcpath_path.h` & `libfshfs-20240501/libcpath/libcpath_path.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/ChangeLog` & `libfshfs-20240501/ChangeLog`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/manuals/fshfsinfo.1` & `libfshfs-20240501/manuals/fshfsinfo.1`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/manuals/libfshfs.3` & `libfshfs-20240501/manuals/libfshfs.3`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/manuals/fshfsmount.1` & `libfshfs-20240501/manuals/fshfsmount.1`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/manuals/Makefile.in` & `libfshfs-20240501/manuals/Makefile.in`

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
@@ -532,15 +534,16 @@
 	libfshfs.3
 
 EXTRA_DIST = \
 	fshfsinfo.1 \
 	fshfsmount.1 \
 	libfshfs.3
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -733,23 +736,25 @@
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
@@ -831,13 +836,10 @@
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

### Comparing `libfshfs-20240221/tests/test_fshfsinfo.sh` & `libfshfs-20240501/tests/test_fshfsinfo.sh`

 * *Files 4% similar despite different names*

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
 
 PROFILES=("fshfsinfo" "fshfsinfo_fs");
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

### Comparing `libfshfs-20240221/tests/fshfs_test_directory_record.c` & `libfshfs-20240501/tests/fshfs_test_directory_record.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_types.h` & `libfshfs-20240501/tests/fshfs_test_types.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_support.c` & `libfshfs-20240501/tests/fshfs_test_support.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_btree_node_descriptor.c` & `libfshfs-20240501/tests/fshfs_test_btree_node_descriptor.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_libuna.h` & `libfshfs-20240501/tests/fshfs_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_notify.c` & `libfshfs-20240501/tests/fshfs_test_notify.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_compression.c` & `libfshfs-20240501/tests/fshfs_test_compression.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_unicode_case_folding_mappings.h` & `libfshfs-20240501/tests/fshfs_test_unicode_case_folding_mappings.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_file_system.c` & `libfshfs-20240501/tests/fshfs_test_file_system.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_btree_file.c` & `libfshfs-20240501/tests/fshfs_test_btree_file.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_extent.c` & `libfshfs-20240501/tests/fshfs_test_extent.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_file_record.c` & `libfshfs-20240501/tests/fshfs_test_file_record.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_getopt.h` & `libfshfs-20240501/tests/fshfs_test_getopt.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_memory.c` & `libfshfs-20240501/tests/fshfs_test_memory.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_libbfio.h` & `libfshfs-20240501/tests/fshfs_test_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/test_tools.sh` & `libfshfs-20240501/tests/test_tools.sh`

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

### Comparing `libfshfs-20240221/tests/fshfs_test_functions.c` & `libfshfs-20240501/tests/fshfs_test_functions.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_unicode_decomposition_mappings.h` & `libfshfs-20240501/tests/fshfs_test_unicode_decomposition_mappings.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_libcnotify.h` & `libfshfs-20240501/tests/fshfs_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_attributes_btree_key.c` & `libfshfs-20240501/tests/fshfs_test_attributes_btree_key.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_macros.h` & `libfshfs-20240501/tests/fshfs_test_macros.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_libcerror.h` & `libfshfs-20240501/tests/fshfs_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_master_directory_block.c` & `libfshfs-20240501/tests/fshfs_test_master_directory_block.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/pyfshfs_test_support.py` & `libfshfs-20240501/tests/pyfshfs_test_support.py`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_getopt.c` & `libfshfs-20240501/tests/fshfs_test_getopt.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/Makefile.am` & `libfshfs-20240501/tests/Makefile.am`

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
@@ -576,13 +576,12 @@
 	@LIBCSPLIT_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libfshfs/libfshfs.la \
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

### Comparing `libfshfs-20240221/tests/fshfs_test_unused.h` & `libfshfs-20240501/tests/fshfs_test_unused.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_btree_node.c` & `libfshfs-20240501/tests/fshfs_test_btree_node.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_thread_record.c` & `libfshfs-20240501/tests/fshfs_test_thread_record.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_fork_descriptor.c` & `libfshfs-20240501/tests/fshfs_test_fork_descriptor.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_extents_btree_key.c` & `libfshfs-20240501/tests/fshfs_test_extents_btree_key.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/test_python_module.sh` & `libfshfs-20240501/tests/test_python_module.sh`

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
 
+LIBRARY_NAME="libfshfs";
+PYTHON_MODULE="pyfshfs";
+
 test_python_function()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyfshfs_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_SCRIPT}";
 	local RESULT=$?;
 
 	return ${RESULT};
 }
 
 test_python_function_with_input()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyfshfs_test_${TEST_FUNCTION}.py";
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
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "pyfshfs");
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

### Comparing `libfshfs-20240221/tests/fshfs_test_bit_stream.c` & `libfshfs-20240501/tests/fshfs_test_bit_stream.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_attribute_record.c` & `libfshfs-20240501/tests/fshfs_test_attribute_record.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_buffer_data_handle.c` & `libfshfs-20240501/tests/fshfs_test_buffer_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_libfdata.h` & `libfshfs-20240501/tests/fshfs_test_libfdata.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_functions.h` & `libfshfs-20240501/tests/fshfs_test_functions.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_tools_signal.c` & `libfshfs-20240501/tests/fshfs_test_tools_signal.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_catalog_btree_key.c` & `libfshfs-20240501/tests/fshfs_test_catalog_btree_key.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_deflate.c` & `libfshfs-20240501/tests/fshfs_test_deflate.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_huffman_tree.c` & `libfshfs-20240501/tests/fshfs_test_huffman_tree.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/pyfshfs_test_volume.py` & `libfshfs-20240501/tests/pyfshfs_test_volume.py`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_tools_info_handle.c` & `libfshfs-20240501/tests/fshfs_test_tools_info_handle.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/test_runner.sh` & `libfshfs-20240501/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_tools_output.c` & `libfshfs-20240501/tests/fshfs_test_tools_output.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_volume.c` & `libfshfs-20240501/tests/fshfs_test_volume.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_btree_header.c` & `libfshfs-20240501/tests/fshfs_test_btree_header.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_libfshfs.h` & `libfshfs-20240501/tests/fshfs_test_libfshfs.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_file_entry.c` & `libfshfs-20240501/tests/fshfs_test_file_entry.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_error.c` & `libfshfs-20240501/tests/fshfs_test_error.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_volume_header.c` & `libfshfs-20240501/tests/fshfs_test_volume_header.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_profiler.c` & `libfshfs-20240501/tests/fshfs_test_profiler.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_libclocale.h` & `libfshfs-20240501/tests/fshfs_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/Makefile.in` & `libfshfs-20240501/tests/Makefile.in`

 * *Files 10% similar despite different names*

```diff
@@ -979,14 +979,16 @@
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
@@ -1052,16 +1054,16 @@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -1592,16 +1594,18 @@
 	@LIBCSPLIT_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libfshfs/libfshfs.la \
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
@@ -2187,24 +2191,68 @@
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
 	-rm -f ../fshfstools/$(DEPDIR)/$(am__dirstamp)
 	-rm -f ../fshfstools/$(am__dirstamp)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ../fshfstools/$(DEPDIR)/digest_hash.Po
+	-rm -f ../fshfstools/$(DEPDIR)/fshfstools_output.Po
+	-rm -f ../fshfstools/$(DEPDIR)/fshfstools_signal.Po
+	-rm -f ../fshfstools/$(DEPDIR)/info_handle.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_attribute_record.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_attributes_btree_key.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_bit_stream.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_btree_file.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_btree_header.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_btree_node.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_btree_node_descriptor.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_btree_node_record.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_buffer_data_handle.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_catalog_btree_key.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_compressed_data_handle.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_compression.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_deflate.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_directory_entry.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_directory_record.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_error.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_extent.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_extents_btree_key.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_file_entry.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_file_record.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_file_system.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_fork_descriptor.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_functions.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_getopt.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_huffman_tree.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_io_handle.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_master_directory_block.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_memory.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_name.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_notify.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_profiler.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_support.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_thread_record.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_tools_info_handle.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_tools_output.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_tools_signal.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_volume.Po
+	-rm -f ./$(DEPDIR)/fshfs_test_volume_header.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -2329,13 +2377,10 @@
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

### Comparing `libfshfs-20240221/tests/fshfs_test_memory.h` & `libfshfs-20240501/tests/fshfs_test_memory.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_btree_node_record.c` & `libfshfs-20240501/tests/fshfs_test_btree_node_record.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_compressed_data_handle.c` & `libfshfs-20240501/tests/fshfs_test_compressed_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_io_handle.c` & `libfshfs-20240501/tests/fshfs_test_io_handle.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/test_library.sh` & `libfshfs-20240501/tests/test_library.sh`

 * *Files 8% similar despite different names*

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
 
 LIBRARY_TESTS="attribute_record attributes_btree_key bit_stream btree_file btree_header btree_node btree_node_descriptor btree_node_record buffer_data_handle catalog_btree_key compressed_data_handle compression deflate directory_entry directory_record error extent extents_btree_key file_entry file_record file_system fork_descriptor huffman_tree io_handle master_directory_block name notify profiler thread_record volume_header";
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

### Comparing `libfshfs-20240221/tests/fshfs_test_directory_entry.c` & `libfshfs-20240501/tests/fshfs_test_directory_entry.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/tests/fshfs_test_name.c` & `libfshfs-20240501/tests/fshfs_test_name.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/ossfuzz/volume_fuzzer.cc` & `libfshfs-20240501/ossfuzz/volume_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/ossfuzz/Makefile.am` & `libfshfs-20240501/ossfuzz/Makefile.am`

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
 	../libfshfs/libfshfs.la \
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

### Comparing `libfshfs-20240221/ossfuzz/ossfuzz_libbfio.h` & `libfshfs-20240501/ossfuzz/ossfuzz_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/ossfuzz/file_entry_fuzzer.cc` & `libfshfs-20240501/ossfuzz/file_entry_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/ossfuzz/extended_attribute_fuzzer.cc` & `libfshfs-20240501/ossfuzz/extended_attribute_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/ossfuzz/ossfuzz_libfshfs.h` & `libfshfs-20240501/ossfuzz/ossfuzz_libfshfs.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/ossfuzz/Makefile.in` & `libfshfs-20240501/ossfuzz/Makefile.in`

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
@@ -584,16 +586,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -649,15 +651,16 @@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libfshfs/libfshfs.la \
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
@@ -909,23 +912,28 @@
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
 
@@ -1011,17 +1019,14 @@
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

### Comparing `libfshfs-20240221/ltmain.sh` & `libfshfs-20240501/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfshfs.spec` & `libfshfs-20240501/libfshfs.spec`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libfshfs
-Version: 20240221
+Version: 20240501
 Release: 1
 Summary: Library to access the Hierarchical File System (HFS) format
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libfshfs
 Requires:                zlib
@@ -36,16 +36,16 @@
 
 %description -n libfshfs-python3
 Python 3 bindings for libfshfs
 
 %package -n libfshfs-tools
 Summary: Several tools for reading Hierarchical File System (HFS) volumes
 Group: Applications/System
-Requires: libfshfs = %{version}-%{release} openssl fuse-libs 
-BuildRequires: openssl-devel fuse-devel 
+Requires: libfshfs = %{version}-%{release} openssl fuse3-libs 
+BuildRequires: openssl-devel fuse3-devel 
 
 %description -n libfshfs-tools
 Several tools for reading Hierarchical File System (HFS) volumes
 
 %prep
 %setup -q
 
@@ -91,10 +91,10 @@
 %files -n libfshfs-tools
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Wed Feb 21 2024 Joachim Metz <joachim.metz@gmail.com> 20240221-1
+* Wed May  1 2024 Joachim Metz <joachim.metz@gmail.com> 20240501-1
 - Auto-generated
```

### Comparing `libfshfs-20240221/libhmac/libhmac_sha1_context.c` & `libfshfs-20240501/libhmac/libhmac_sha1_context.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libhmac/libhmac_sha224.h` & `libfshfs-20240501/libhmac/libhmac_sha224.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libhmac/libhmac_sha512_context.c` & `libfshfs-20240501/libhmac/libhmac_sha512_context.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libhmac/libhmac_extern.h` & `libfshfs-20240501/libhmac/libhmac_extern.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libhmac/libhmac_md5.c` & `libfshfs-20240501/libhmac/libhmac_md5.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libhmac/libhmac_md5.h` & `libfshfs-20240501/libhmac/libhmac_md5.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libhmac/libhmac_error.h` & `libfshfs-20240501/libhmac/libhmac_error.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libhmac/libhmac_types.h` & `libfshfs-20240501/libhmac/libhmac_types.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libhmac/libhmac_byte_stream.h` & `libfshfs-20240501/libhmac/libhmac_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libhmac/libhmac_sha512.c` & `libfshfs-20240501/libhmac/libhmac_sha512.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libhmac/libhmac_sha256_context.c` & `libfshfs-20240501/libhmac/libhmac_sha256_context.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libhmac/libhmac_sha224.c` & `libfshfs-20240501/libhmac/libhmac_sha224.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libhmac/libhmac_definitions.h` & `libfshfs-20240501/libhmac/libhmac_definitions.h`

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

### Comparing `libfshfs-20240221/libhmac/libhmac_unused.h` & `libfshfs-20240501/libhmac/libhmac_unused.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libhmac/libhmac_sha1.h` & `libfshfs-20240501/libhmac/libhmac_sha1.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libhmac/libhmac_sha256_context.h` & `libfshfs-20240501/libhmac/libhmac_sha256_context.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libhmac/Makefile.am` & `libfshfs-20240501/libhmac/Makefile.am`

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

### Comparing `libfshfs-20240221/libhmac/libhmac_sha224_context.c` & `libfshfs-20240501/libhmac/libhmac_sha224_context.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libhmac/libhmac_md5_context.h` & `libfshfs-20240501/libhmac/libhmac_md5_context.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libhmac/libhmac_sha256.c` & `libfshfs-20240501/libhmac/libhmac_sha256.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libhmac/libhmac_sha1_context.h` & `libfshfs-20240501/libhmac/libhmac_sha1_context.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libhmac/libhmac_libcerror.h` & `libfshfs-20240501/libhmac/libhmac_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libhmac/libhmac_error.c` & `libfshfs-20240501/libhmac/libhmac_error.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libhmac/libhmac_support.h` & `libfshfs-20240501/libhmac/libhmac_support.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libhmac/Makefile.in` & `libfshfs-20240501/libhmac/Makefile.in`

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
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -600,15 +602,16 @@
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
@@ -819,24 +822,38 @@
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
 
@@ -931,17 +948,14 @@
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

### Comparing `libfshfs-20240221/libhmac/libhmac_sha256.h` & `libfshfs-20240501/libhmac/libhmac_sha256.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libhmac/libhmac_sha224_context.h` & `libfshfs-20240501/libhmac/libhmac_sha224_context.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libhmac/libhmac_sha512_context.h` & `libfshfs-20240501/libhmac/libhmac_sha512_context.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libhmac/libhmac_sha512.h` & `libfshfs-20240501/libhmac/libhmac_sha512.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libhmac/libhmac_support.c` & `libfshfs-20240501/libhmac/libhmac_support.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libhmac/libhmac_sha1.c` & `libfshfs-20240501/libhmac/libhmac_sha1.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libhmac/libhmac_md5_context.c` & `libfshfs-20240501/libhmac/libhmac_md5_context.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcsplit/libcsplit_narrow_string.c` & `libfshfs-20240501/libcsplit/libcsplit_narrow_string.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcsplit/libcsplit_definitions.h` & `libfshfs-20240501/libcsplit/libcsplit_definitions.h`

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

### Comparing `libfshfs-20240221/libcsplit/libcsplit_types.h` & `libfshfs-20240501/libcsplit/libcsplit_types.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcsplit/libcsplit_wide_split_string.c` & `libfshfs-20240501/libcsplit/libcsplit_wide_split_string.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcsplit/libcsplit_support.h` & `libfshfs-20240501/libcsplit/libcsplit_support.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcsplit/Makefile.am` & `libfshfs-20240501/libcsplit/Makefile.am`

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

### Comparing `libfshfs-20240221/libcsplit/libcsplit_libcerror.h` & `libfshfs-20240501/libcsplit/libcsplit_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcsplit/libcsplit_wide_string.c` & `libfshfs-20240501/libcsplit/libcsplit_wide_string.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcsplit/libcsplit_unused.h` & `libfshfs-20240501/libcsplit/libcsplit_unused.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcsplit/libcsplit_wide_split_string.h` & `libfshfs-20240501/libcsplit/libcsplit_wide_split_string.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcsplit/libcsplit_error.c` & `libfshfs-20240501/libcsplit/libcsplit_error.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcsplit/libcsplit_narrow_split_string.c` & `libfshfs-20240501/libcsplit/libcsplit_narrow_split_string.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcsplit/libcsplit_extern.h` & `libfshfs-20240501/libcsplit/libcsplit_extern.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcsplit/libcsplit_error.h` & `libfshfs-20240501/libcsplit/libcsplit_error.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcsplit/libcsplit_support.c` & `libfshfs-20240501/libcsplit/libcsplit_support.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcsplit/libcsplit_wide_string.h` & `libfshfs-20240501/libcsplit/libcsplit_wide_string.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcsplit/Makefile.in` & `libfshfs-20240501/libcsplit/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -488,14 +488,16 @@
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
@@ -560,16 +562,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -578,15 +580,16 @@
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
@@ -791,24 +794,32 @@
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
 
@@ -897,17 +908,14 @@
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

### Comparing `libfshfs-20240221/libcsplit/libcsplit_narrow_split_string.h` & `libfshfs-20240501/libcsplit/libcsplit_narrow_split_string.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcsplit/libcsplit_narrow_string.h` & `libfshfs-20240501/libcsplit/libcsplit_narrow_string.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/po/remove-potcdate.sin` & `libfshfs-20240501/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/po/Makefile.in.in` & `libfshfs-20240501/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/po/en@quot.header` & `libfshfs-20240501/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/po/en@boldquot.header` & `libfshfs-20240501/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/po/insert-header.sin` & `libfshfs-20240501/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/po/Makevars` & `libfshfs-20240501/po/Makevars`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/po/Makevars.in` & `libfshfs-20240501/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/po/Rules-quot` & `libfshfs-20240501/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_windows_1251.c` & `libfshfs-20240501/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_utf16_string.c` & `libfshfs-20240501/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_base16_stream.c` & `libfshfs-20240501/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_utf8_stream.h` & `libfshfs-20240501/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_iso_8859_2.h` & `libfshfs-20240501/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_windows_932.c` & `libfshfs-20240501/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_dingbats.h` & `libfshfs-20240501/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_utf8_string.c` & `libfshfs-20240501/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_base64_stream.c` & `libfshfs-20240501/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_error.h` & `libfshfs-20240501/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_turkish.h` & `libfshfs-20240501/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_unicode_character.c` & `libfshfs-20240501/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_gaelic.c` & `libfshfs-20240501/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_arabic.h` & `libfshfs-20240501/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_thai.c` & `libfshfs-20240501/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_windows_874.h` & `libfshfs-20240501/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_iso_8859_15.h` & `libfshfs-20240501/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_utf8_string.h` & `libfshfs-20240501/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_iso_8859_16.c` & `libfshfs-20240501/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_windows_1255.c` & `libfshfs-20240501/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_utf7_stream.c` & `libfshfs-20240501/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_byte_stream.h` & `libfshfs-20240501/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_koi8_u.c` & `libfshfs-20240501/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_unused.h` & `libfshfs-20240501/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_iso_8859_6.c` & `libfshfs-20240501/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_iso_8859_14.c` & `libfshfs-20240501/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_base64_stream.h` & `libfshfs-20240501/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_error.c` & `libfshfs-20240501/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_centraleurroman.h` & `libfshfs-20240501/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_romanian.c` & `libfshfs-20240501/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_iso_8859_6.h` & `libfshfs-20240501/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_iso_8859_9.c` & `libfshfs-20240501/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_russian.h` & `libfshfs-20240501/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_dingbats.c` & `libfshfs-20240501/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_iso_8859_15.c` & `libfshfs-20240501/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_windows_936.c` & `libfshfs-20240501/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_croatian.h` & `libfshfs-20240501/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_scsu.h` & `libfshfs-20240501/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/Makefile.am` & `libfshfs-20240501/libuna/Makefile.am`

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

### Comparing `libfshfs-20240221/libuna/libuna_utf32_stream.c` & `libfshfs-20240501/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_windows_936.h` & `libfshfs-20240501/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_iso_8859_10.c` & `libfshfs-20240501/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_roman.c` & `libfshfs-20240501/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_utf7_stream.h` & `libfshfs-20240501/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_iso_8859_3.h` & `libfshfs-20240501/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_thai.h` & `libfshfs-20240501/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_farsi.h` & `libfshfs-20240501/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_ukrainian.c` & `libfshfs-20240501/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_inuit.c` & `libfshfs-20240501/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_windows_932.h` & `libfshfs-20240501/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_windows_874.c` & `libfshfs-20240501/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_iso_8859_5.c` & `libfshfs-20240501/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_iso_8859_10.h` & `libfshfs-20240501/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_definitions.h` & `libfshfs-20240501/libuna/libuna_definitions.h`

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

### Comparing `libfshfs-20240221/libuna/libuna_url_stream.h` & `libfshfs-20240501/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_icelandic.h` & `libfshfs-20240501/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_koi8_u.h` & `libfshfs-20240501/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_utf16_stream.c` & `libfshfs-20240501/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_windows_1253.c` & `libfshfs-20240501/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_iso_8859_4.h` & `libfshfs-20240501/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_greek.c` & `libfshfs-20240501/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_libcerror.h` & `libfshfs-20240501/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_centraleurroman.c` & `libfshfs-20240501/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_windows_1254.c` & `libfshfs-20240501/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_iso_8859_13.h` & `libfshfs-20240501/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_iso_8859_7.h` & `libfshfs-20240501/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_windows_1255.h` & `libfshfs-20240501/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_unicode_character.h` & `libfshfs-20240501/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_iso_8859_8.h` & `libfshfs-20240501/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_iso_8859_13.c` & `libfshfs-20240501/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_windows_949.h` & `libfshfs-20240501/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_cyrillic.c` & `libfshfs-20240501/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_celtic.c` & `libfshfs-20240501/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_support.h` & `libfshfs-20240501/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_iso_8859_4.c` & `libfshfs-20240501/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_windows_949.c` & `libfshfs-20240501/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_utf16_stream.h` & `libfshfs-20240501/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_symbol.c` & `libfshfs-20240501/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_roman.h` & `libfshfs-20240501/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_windows_1257.c` & `libfshfs-20240501/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_windows_1254.h` & `libfshfs-20240501/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_windows_950.c` & `libfshfs-20240501/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_extern.h` & `libfshfs-20240501/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_windows_1256.c` & `libfshfs-20240501/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_types.h` & `libfshfs-20240501/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_base32_stream.h` & `libfshfs-20240501/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_windows_1253.h` & `libfshfs-20240501/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_iso_8859_16.h` & `libfshfs-20240501/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_utf8_stream.c` & `libfshfs-20240501/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_windows_1250.h` & `libfshfs-20240501/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_iso_8859_2.c` & `libfshfs-20240501/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_support.c` & `libfshfs-20240501/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_koi8_r.c` & `libfshfs-20240501/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_iso_8859_5.h` & `libfshfs-20240501/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_utf16_string.h` & `libfshfs-20240501/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_utf32_string.c` & `libfshfs-20240501/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_icelandic.c` & `libfshfs-20240501/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_windows_1256.h` & `libfshfs-20240501/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_utf32_string.h` & `libfshfs-20240501/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_romanian.h` & `libfshfs-20240501/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_iso_8859_8.c` & `libfshfs-20240501/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_koi8_r.h` & `libfshfs-20240501/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_cyrillic.h` & `libfshfs-20240501/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_arabic.c` & `libfshfs-20240501/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_croatian.c` & `libfshfs-20240501/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_iso_8859_9.h` & `libfshfs-20240501/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_greek.h` & `libfshfs-20240501/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_windows_1258.h` & `libfshfs-20240501/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_iso_8859_7.c` & `libfshfs-20240501/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/Makefile.in` & `libfshfs-20240501/libuna/Makefile.in`

 * *Files 8% similar despite different names*

```diff
@@ -656,14 +656,16 @@
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
@@ -728,16 +730,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -803,15 +805,16 @@
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
@@ -1073,24 +1076,89 @@
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
 
@@ -1236,17 +1304,14 @@
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

### Comparing `libfshfs-20240221/libuna/libuna_codepage_iso_8859_3.c` & `libfshfs-20240501/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_windows_1250.c` & `libfshfs-20240501/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_scsu.c` & `libfshfs-20240501/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_windows_1252.c` & `libfshfs-20240501/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_turkish.c` & `libfshfs-20240501/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_ukrainian.h` & `libfshfs-20240501/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_russian.c` & `libfshfs-20240501/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_windows_1258.c` & `libfshfs-20240501/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_celtic.h` & `libfshfs-20240501/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_byte_stream.c` & `libfshfs-20240501/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_gaelic.h` & `libfshfs-20240501/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_utf32_stream.h` & `libfshfs-20240501/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_symbol.h` & `libfshfs-20240501/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_windows_1257.h` & `libfshfs-20240501/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_inuit.h` & `libfshfs-20240501/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_mac_farsi.c` & `libfshfs-20240501/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_windows_950.h` & `libfshfs-20240501/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_url_stream.c` & `libfshfs-20240501/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_windows_1251.h` & `libfshfs-20240501/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_windows_1252.h` & `libfshfs-20240501/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_codepage_iso_8859_14.h` & `libfshfs-20240501/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_base16_stream.h` & `libfshfs-20240501/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libuna/libuna_base32_stream.c` & `libfshfs-20240501/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/Makefile.in` & `libfshfs-20240501/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -538,14 +538,16 @@
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
+	libfshfs.pc \
+	libfshfs.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libfshfs.pc
 
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
 	(cd $(srcdir)/libfmos && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfshfs && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libfshfs.pc
-	-rm -f libfshfs.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfshfs-20240221/libcnotify/libcnotify_definitions.h` & `libfshfs-20240501/libcnotify/libcnotify_definitions.h`

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

### Comparing `libfshfs-20240221/libcnotify/libcnotify_extern.h` & `libfshfs-20240501/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcnotify/libcnotify_support.c` & `libfshfs-20240501/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcnotify/libcnotify_stream.h` & `libfshfs-20240501/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcnotify/Makefile.am` & `libfshfs-20240501/libcnotify/Makefile.am`

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

### Comparing `libfshfs-20240221/libcnotify/libcnotify_unused.h` & `libfshfs-20240501/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcnotify/libcnotify_verbose.h` & `libfshfs-20240501/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcnotify/libcnotify_print.h` & `libfshfs-20240501/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcnotify/libcnotify_stream.c` & `libfshfs-20240501/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcnotify/libcnotify_support.h` & `libfshfs-20240501/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcnotify/libcnotify_verbose.c` & `libfshfs-20240501/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcnotify/Makefile.in` & `libfshfs-20240501/libcnotify/Makefile.in`

 * *Files 4% similar despite different names*

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
@@ -552,30 +554,31 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -778,24 +781,30 @@
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
 
@@ -882,17 +891,14 @@
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

### Comparing `libfshfs-20240221/libcnotify/libcnotify_libcerror.h` & `libfshfs-20240501/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcnotify/libcnotify_print.c` & `libfshfs-20240501/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcerror/libcerror_system.c` & `libfshfs-20240501/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcerror/libcerror_error.c` & `libfshfs-20240501/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcerror/libcerror_extern.h` & `libfshfs-20240501/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcerror/Makefile.am` & `libfshfs-20240501/libcerror/Makefile.am`

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

### Comparing `libfshfs-20240221/libcerror/libcerror_types.h` & `libfshfs-20240501/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcerror/libcerror_support.h` & `libfshfs-20240501/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcerror/libcerror_error.h` & `libfshfs-20240501/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcerror/libcerror_system.h` & `libfshfs-20240501/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcerror/libcerror_definitions.h` & `libfshfs-20240501/libcerror/libcerror_definitions.h`

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

### Comparing `libfshfs-20240221/libcerror/libcerror_support.c` & `libfshfs-20240501/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcerror/libcerror_unused.h` & `libfshfs-20240501/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libcerror/Makefile.in` & `libfshfs-20240501/libcerror/Makefile.in`

 * *Files 0% similar despite different names*

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
@@ -549,28 +551,29 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -772,24 +775,29 @@
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
 
@@ -875,17 +883,14 @@
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

### Comparing `libfshfs-20240221/libfshfs.spec.in` & `libfshfs-20240501/libfshfs.spec.in`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/fshfstools_libfguid.h` & `libfshfs-20240501/fshfstools/fshfstools_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/fshfstools_libcerror.h` & `libfshfs-20240501/fshfstools/fshfstools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/fshfstools_output.c` & `libfshfs-20240501/fshfstools/fshfstools_output.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/mount_dokan.c` & `libfshfs-20240501/fshfstools/mount_dokan.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/mount_file_system.h` & `libfshfs-20240501/fshfstools/mount_file_system.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/fshfstools_i18n.h` & `libfshfs-20240501/fshfstools/fshfstools_i18n.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/mount_fuse.c` & `libfshfs-20240501/fshfstools/mount_fuse.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/info_handle.h` & `libfshfs-20240501/fshfstools/info_handle.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/mount_dokan.h` & `libfshfs-20240501/fshfstools/mount_dokan.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/fshfstools_libhmac.h` & `libfshfs-20240501/fshfstools/fshfstools_libhmac.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/digest_hash.c` & `libfshfs-20240501/fshfstools/digest_hash.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/mount_file_system.c` & `libfshfs-20240501/fshfstools/mount_file_system.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/fshfstools_libbfio.h` & `libfshfs-20240501/fshfstools/fshfstools_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/Makefile.am` & `libfshfs-20240501/fshfstools/Makefile.am`

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
@@ -97,17 +97,15 @@
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libfshfs/libfshfs.la \
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
 	@echo "Running splint on fshfsinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(fshfsinfo_SOURCES)
```

### Comparing `libfshfs-20240221/fshfstools/fshfstools_libuna.h` & `libfshfs-20240501/fshfstools/fshfstools_libuna.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/fshfstools_libcpath.h` & `libfshfs-20240501/fshfstools/fshfstools_libcpath.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/mount_file_entry.c` & `libfshfs-20240501/fshfstools/mount_file_entry.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/fshfstools_getopt.h` & `libfshfs-20240501/fshfstools/fshfstools_getopt.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/info_handle.c` & `libfshfs-20240501/fshfstools/info_handle.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/mount_file_entry.h` & `libfshfs-20240501/fshfstools/mount_file_entry.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/fshfstools_libfdata.h` & `libfshfs-20240501/fshfstools/fshfstools_libfdata.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/mount_handle.h` & `libfshfs-20240501/fshfstools/mount_handle.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/fshfstools_libclocale.h` & `libfshfs-20240501/fshfstools/fshfstools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/fshfstools_libcnotify.h` & `libfshfs-20240501/fshfstools/fshfstools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/fshfsinfo.c` & `libfshfs-20240501/fshfstools/fshfsinfo.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/fshfstools_signal.c` & `libfshfs-20240501/fshfstools/fshfstools_signal.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/fshfstools_getopt.c` & `libfshfs-20240501/fshfstools/fshfstools_getopt.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/mount_handle.c` & `libfshfs-20240501/fshfstools/mount_handle.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/fshfstools_libfshfs.h` & `libfshfs-20240501/fshfstools/fshfstools_libfshfs.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/fshfstools_libfdatetime.h` & `libfshfs-20240501/fshfstools/fshfstools_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/fshfsmount.c` & `libfshfs-20240501/fshfstools/fshfsmount.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/fshfstools_libfcache.h` & `libfshfs-20240501/fshfstools/fshfstools_libfcache.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/Makefile.in` & `libfshfs-20240501/fshfstools/Makefile.in`

 * *Files 0% similar despite different names*

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
@@ -557,16 +559,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -654,15 +656,16 @@
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libfshfs/libfshfs.la \
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
@@ -919,23 +922,37 @@
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
+	-rm -f ./$(DEPDIR)/fshfsinfo.Po
+	-rm -f ./$(DEPDIR)/fshfsmount.Po
+	-rm -f ./$(DEPDIR)/fshfstools_getopt.Po
+	-rm -f ./$(DEPDIR)/fshfstools_output.Po
+	-rm -f ./$(DEPDIR)/fshfstools_signal.Po
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
 
@@ -1030,17 +1047,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on fshfsinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(fshfsinfo_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfshfs-20240221/fshfstools/fshfstools_signal.h` & `libfshfs-20240501/fshfstools/fshfstools_signal.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/digest_hash.h` & `libfshfs-20240501/fshfstools/digest_hash.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/fshfstools_unused.h` & `libfshfs-20240501/fshfstools/fshfstools_unused.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/fshfstools_output.h` & `libfshfs-20240501/fshfstools/fshfstools_output.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/fshfstools/mount_fuse.h` & `libfshfs-20240501/fshfstools/mount_fuse.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdatetime/libfdatetime_floatingtime.h` & `libfshfs-20240501/libfdatetime/libfdatetime_floatingtime.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdatetime/libfdatetime_nsf_timedate.c` & `libfshfs-20240501/libfdatetime/libfdatetime_nsf_timedate.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdatetime/libfdatetime_error.h` & `libfshfs-20240501/libfdatetime/libfdatetime_error.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdatetime/libfdatetime_floatingtime.c` & `libfshfs-20240501/libfdatetime/libfdatetime_floatingtime.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdatetime/libfdatetime_support.h` & `libfshfs-20240501/libfdatetime/libfdatetime_support.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdatetime/libfdatetime_hfs_time.h` & `libfshfs-20240501/libfdatetime/libfdatetime_hfs_time.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdatetime/libfdatetime_definitions.h` & `libfshfs-20240501/libfdatetime/libfdatetime_definitions.h`

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

### Comparing `libfshfs-20240221/libfdatetime/libfdatetime_hfs_time.c` & `libfshfs-20240501/libfdatetime/libfdatetime_hfs_time.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdatetime/Makefile.am` & `libfshfs-20240501/libfdatetime/Makefile.am`

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

### Comparing `libfshfs-20240221/libfdatetime/libfdatetime_filetime.c` & `libfshfs-20240501/libfdatetime/libfdatetime_filetime.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdatetime/libfdatetime_systemtime.h` & `libfshfs-20240501/libfdatetime/libfdatetime_systemtime.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdatetime/libfdatetime_extern.h` & `libfshfs-20240501/libfdatetime/libfdatetime_extern.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdatetime/libfdatetime_posix_time.c` & `libfshfs-20240501/libfdatetime/libfdatetime_posix_time.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdatetime/libfdatetime_unused.h` & `libfshfs-20240501/libfdatetime/libfdatetime_unused.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdatetime/libfdatetime_fat_date_time.h` & `libfshfs-20240501/libfdatetime/libfdatetime_fat_date_time.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdatetime/libfdatetime_systemtime.c` & `libfshfs-20240501/libfdatetime/libfdatetime_systemtime.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdatetime/libfdatetime_nsf_timedate.h` & `libfshfs-20240501/libfdatetime/libfdatetime_nsf_timedate.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdatetime/libfdatetime_libcerror.h` & `libfshfs-20240501/libfdatetime/libfdatetime_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdatetime/libfdatetime_support.c` & `libfshfs-20240501/libfdatetime/libfdatetime_support.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdatetime/libfdatetime_error.c` & `libfshfs-20240501/libfdatetime/libfdatetime_error.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdatetime/libfdatetime_posix_time.h` & `libfshfs-20240501/libfdatetime/libfdatetime_posix_time.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdatetime/libfdatetime_date_time_values.h` & `libfshfs-20240501/libfdatetime/libfdatetime_date_time_values.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdatetime/libfdatetime_filetime.h` & `libfshfs-20240501/libfdatetime/libfdatetime_filetime.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdatetime/libfdatetime_date_time_values.c` & `libfshfs-20240501/libfdatetime/libfdatetime_date_time_values.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdatetime/libfdatetime_types.h` & `libfshfs-20240501/libfdatetime/libfdatetime_types.h`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/libfdatetime/Makefile.in` & `libfshfs-20240501/libfdatetime/Makefile.in`

 * *Files 5% similar despite different names*

```diff
@@ -499,14 +499,16 @@
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
@@ -571,16 +573,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -593,15 +595,16 @@
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
@@ -810,24 +813,36 @@
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
 
@@ -920,17 +935,14 @@
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

### Comparing `libfshfs-20240221/libfdatetime/libfdatetime_fat_date_time.c` & `libfshfs-20240501/libfdatetime/libfdatetime_fat_date_time.c`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/aclocal.m4` & `libfshfs-20240501/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libfshfs-20240221/configure.ac` & `libfshfs-20240501/configure.ac`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libfshfs],
- [20240221],
+ [20240501],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libfshfs.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```


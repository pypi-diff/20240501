# Comparing `tmp/openlane-2.0.3.tar.gz` & `tmp/openlane-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlane-2.0.3.tar", last modified: Wed Apr 24 18:30:16 2024, max compression
+gzip compressed data, was "openlane-2.0.4.tar", last modified: Wed May  1 15:53:37 2024, max compression
```

## Comparing `openlane-2.0.3.tar` & `openlane-2.0.4.tar`

### file list

```diff
@@ -1,198 +1,198 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.427092 openlane-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-04-24 18:30:16.427092 openlane-2.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.371092 openlane-2.0.3/openlane/
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12859 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.379092 openlane-2.0.3/openlane/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/common/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/common/drc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9929 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/common/generic_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.379092 openlane-2.0.3/openlane/common/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/common/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12271 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/common/metrics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/common/metrics/library.py
--rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/common/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     9148 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/common/metrics/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    11513 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/common/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/common/ring_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/common/tcl.py
--rw-r--r--   0 runner    (1001) docker     (127)    20900 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/common/toolbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/common/tpe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/common/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.383092 openlane-2.0.3/openlane/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/config/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32144 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    15877 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/config/flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/config/pdk_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    14868 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/config/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/config/removals.py
--rw-r--r--   0 runner    (1001) docker     (127)    25394 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/config/variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     7134 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/env_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.367092 openlane-2.0.3/openlane/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.383092 openlane-2.0.3/openlane/examples/spm/
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/examples/spm/config.json
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/examples/spm/pin_order.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.387092 openlane-2.0.3/openlane/examples/spm/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/examples/spm/src/impl.sdc
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/examples/spm/src/signoff.sdc
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/examples/spm/src/spm.v
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.387092 openlane-2.0.3/openlane/examples/spm/verify/
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/examples/spm/verify/spm_tb.v
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.387092 openlane-2.0.3/openlane/examples/spm-user_project_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/examples/spm-user_project_wrapper/SPM_example.v
--rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/examples/spm-user_project_wrapper/base_sdc_file.sdc
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/examples/spm-user_project_wrapper/config-tut.json
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/examples/spm-user_project_wrapper/config.json
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/examples/spm-user_project_wrapper/defines.v
--rw-r--r--   0 runner    (1001) docker     (127)   438993 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/examples/spm-user_project_wrapper/template.def
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/examples/spm-user_project_wrapper/user_project_wrapper.v
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.391092 openlane-2.0.3/openlane/flows/
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/flows/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    10868 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/flows/classic.py
--rw-r--r--   0 runner    (1001) docker     (127)    15375 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/flows/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    33165 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/flows/flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/flows/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/flows/optimizing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10928 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/flows/sequential.py
--rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/flows/synth_explore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.391092 openlane-2.0.3/openlane/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-24 18:18:18.000000 openlane-2.0.3/openlane/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8618 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/logging/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/open_pdks_rev
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.391092 openlane-2.0.3/openlane/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/base.sdc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.395092 openlane-2.0.3/openlane/scripts/klayout/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/klayout/Readme.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     2151 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/klayout/open_design.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3833 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/klayout/render.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5867 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/klayout/stream_out.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/klayout/xml_drc_report_to_json.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3131 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/klayout/xor.drc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.395092 openlane-2.0.3/openlane/scripts/magic/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/magic/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.395092 openlane-2.0.3/openlane/scripts/magic/common/
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/magic/common/read.tcl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.395092 openlane-2.0.3/openlane/scripts/magic/def/
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/magic/def/antenna_check.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/magic/def/mag.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)     2137 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/magic/def/mag_gds.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)     2402 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/magic/drc.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/magic/extract_spice.tcl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.399092 openlane-2.0.3/openlane/scripts/magic/gds/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2198 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/magic/gds/drc_batch.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/magic/gds/erase_box.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)     1324 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/magic/gds/extras_mag.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/magic/gds/mag_with_pointers.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/magic/get_bbox.tcl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.399092 openlane-2.0.3/openlane/scripts/magic/lef/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1594 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/magic/lef/extras_maglef.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)      863 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/magic/lef/maglef.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/magic/lef.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/magic/wrapper.tcl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.399092 openlane-2.0.3/openlane/scripts/netgen/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/netgen/setup.tcl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.403092 openlane-2.0.3/openlane/scripts/odbpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/odbpy/apply_def_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/odbpy/check_antenna_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/odbpy/contextualize.py
--rw-r--r--   0 runner    (1001) docker     (127)    17754 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/odbpy/defutil.py
--rw-r--r--   0 runner    (1001) docker     (127)    11621 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/odbpy/diodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11144 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/odbpy/disconnected_pins.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/odbpy/exception_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/odbpy/filter_unannotated.py
--rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/odbpy/io_place.py
--rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/odbpy/label_macro_pins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/odbpy/lefutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/odbpy/manual_macro_place.py
--rw-r--r--   0 runner    (1001) docker     (127)    11912 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/odbpy/power_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/odbpy/random_place.py
--rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/odbpy/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/odbpy/remove_buffers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/odbpy/snap_to_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/odbpy/wire_lengths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.411092 openlane-2.0.3/openlane/scripts/openroad/
--rwxr-xr-x   0 runner    (1001) docker     (127)      810 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/antenna_check.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/antenna_repair.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)      788 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/basic_mp.tcl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.415092 openlane-2.0.3/openlane/scripts/openroad/common/
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/common/dpl.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/common/dpl_cell_pad.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/common/grt.tcl
--rw-r--r--   0 runner    (1001) docker     (127)    14029 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/common/io.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/common/pdn_cfg.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/common/resizer.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/common/set_global_connections.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/common/set_layer_adjustments.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/common/set_power_nets.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/common/set_rc.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/common/set_routing_layers.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)     2658 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/cts.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/cut_rows.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)      777 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/dpl.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)     1175 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/drt.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)      972 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/fill.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)     4849 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/floorplan.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)     2413 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/gpl.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/grt.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/gui.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/insert_buffer.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)     1893 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/ioplacer.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/irdrop.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/pdn.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/rcx.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/repair_design.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/repair_design_postgrt.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/rsz_timing_postcts.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/rsz_timing_postgrt.tcl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.415092 openlane-2.0.3/openlane/scripts/openroad/sta/
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/sta/check_macro_instances.tcl
--rw-r--r--   0 runner    (1001) docker     (127)    13662 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/sta/corner.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)      935 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/tapcell.tcl
--rwxr-xr-x   0 runner    (1001) docker     (127)      663 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/openroad/write_views.tcl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.415092 openlane-2.0.3/openlane/scripts/tclsh/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/tclsh/hello.tcl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.415092 openlane-2.0.3/openlane/scripts/yosys/
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/yosys/common.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/yosys/construct_abc_script.tcl
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/yosys/json_header.tcl
--rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/scripts/yosys/synthesize.tcl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.419092 openlane-2.0.3/openlane/state/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/state/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/state/design_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/state/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.423092 openlane-2.0.3/openlane/steps/
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12978 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/steps/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/steps/checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/steps/common_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/steps/cvc_rv.py
--rw-r--r--   0 runner    (1001) docker     (127)    16425 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/steps/klayout.py
--rw-r--r--   0 runner    (1001) docker     (127)    16589 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/steps/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/steps/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/steps/netgen.py
--rw-r--r--   0 runner    (1001) docker     (127)    29654 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/steps/odb.py
--rw-r--r--   0 runner    (1001) docker     (127)    81058 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/steps/openroad.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/steps/openroad_alerts.py
--rw-r--r--   0 runner    (1001) docker     (127)    53312 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/steps/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/steps/tclstep.py
--rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/steps/verilator.py
--rw-r--r--   0 runner    (1001) docker     (127)    23272 2024-04-24 18:18:19.000000 openlane-2.0.3/openlane/steps/yosys.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.375092 openlane-2.0.3/openlane.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-04-24 18:30:16.000000 openlane-2.0.3/openlane.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-04-24 18:30:16.000000 openlane-2.0.3/openlane.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 18:30:16.000000 openlane-2.0.3/openlane.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-24 18:30:16.000000 openlane-2.0.3/openlane.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-24 18:30:16.000000 openlane-2.0.3/openlane.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 18:30:16.000000 openlane-2.0.3/openlane.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 18:30:16.427092 openlane-2.0.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1776 2024-04-24 18:18:19.000000 openlane-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:30:16.427092 openlane-2.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-24 18:18:19.000000 openlane-2.0.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9215 2024-04-24 18:18:19.000000 openlane-2.0.3/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.871603 openlane-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-05-01 15:53:37.871603 openlane-2.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.847603 openlane-2.0.4/openlane/
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12859 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.847603 openlane-2.0.4/openlane/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/common/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/common/drc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9929 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/common/generic_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.847603 openlane-2.0.4/openlane/common/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/common/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12271 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/common/metrics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/common/metrics/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/common/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9148 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/common/metrics/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11513 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/common/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/common/ring_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/common/tcl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20900 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/common/toolbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/common/tpe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/common/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.851603 openlane-2.0.4/openlane/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/config/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32144 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15877 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/config/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/config/pdk_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14868 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/config/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/config/removals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25394 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/config/variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7134 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/env_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.843603 openlane-2.0.4/openlane/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.851603 openlane-2.0.4/openlane/examples/spm/
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/examples/spm/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/examples/spm/pin_order.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.851603 openlane-2.0.4/openlane/examples/spm/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/examples/spm/src/impl.sdc
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/examples/spm/src/signoff.sdc
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/examples/spm/src/spm.v
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.851603 openlane-2.0.4/openlane/examples/spm/verify/
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/examples/spm/verify/spm_tb.v
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.851603 openlane-2.0.4/openlane/examples/spm-user_project_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)     8423 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/examples/spm-user_project_wrapper/SPM_example.v
+-rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/examples/spm-user_project_wrapper/base_sdc_file.sdc
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/examples/spm-user_project_wrapper/config-tut.json
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/examples/spm-user_project_wrapper/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/examples/spm-user_project_wrapper/defines.v
+-rw-r--r--   0 runner    (1001) docker     (127)   438993 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/examples/spm-user_project_wrapper/template.def
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/examples/spm-user_project_wrapper/user_project_wrapper.v
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.855603 openlane-2.0.4/openlane/flows/
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/flows/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10868 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/flows/classic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15375 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/flows/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33165 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/flows/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/flows/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6080 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/flows/optimizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10928 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/flows/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/flows/synth_explore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.855603 openlane-2.0.4/openlane/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8618 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/logging/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/open_pdks_rev
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.855603 openlane-2.0.4/openlane/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/base.sdc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.855603 openlane-2.0.4/openlane/scripts/klayout/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/klayout/Readme.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2151 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/klayout/open_design.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3833 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/klayout/render.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5867 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/klayout/stream_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/klayout/xml_drc_report_to_json.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3131 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/klayout/xor.drc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.855603 openlane-2.0.4/openlane/scripts/magic/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/magic/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.855603 openlane-2.0.4/openlane/scripts/magic/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/magic/common/read.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.855603 openlane-2.0.4/openlane/scripts/magic/def/
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/magic/def/antenna_check.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/magic/def/mag.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2137 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/magic/def/mag_gds.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2402 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/magic/drc.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/magic/extract_spice.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.855603 openlane-2.0.4/openlane/scripts/magic/gds/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2198 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/magic/gds/drc_batch.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/magic/gds/erase_box.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1324 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/magic/gds/extras_mag.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/magic/gds/mag_with_pointers.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/magic/get_bbox.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.855603 openlane-2.0.4/openlane/scripts/magic/lef/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1594 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/magic/lef/extras_maglef.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      863 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/magic/lef/maglef.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/magic/lef.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/magic/wrapper.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.855603 openlane-2.0.4/openlane/scripts/netgen/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/netgen/setup.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.859603 openlane-2.0.4/openlane/scripts/odbpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/odbpy/apply_def_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/odbpy/check_antenna_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/odbpy/contextualize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17754 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/odbpy/defutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11621 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/odbpy/diodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11144 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/odbpy/disconnected_pins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/odbpy/exception_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/odbpy/filter_unannotated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/odbpy/io_place.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/odbpy/label_macro_pins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/odbpy/lefutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/odbpy/manual_macro_place.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12365 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/odbpy/power_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/odbpy/random_place.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/odbpy/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/odbpy/remove_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/odbpy/snap_to_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/odbpy/wire_lengths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.863603 openlane-2.0.4/openlane/scripts/openroad/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      810 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/antenna_check.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/antenna_repair.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      788 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/basic_mp.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.863603 openlane-2.0.4/openlane/scripts/openroad/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/common/dpl.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/common/dpl_cell_pad.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/common/grt.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)    14029 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/common/io.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/common/pdn_cfg.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/common/resizer.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/common/set_global_connections.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/common/set_layer_adjustments.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/common/set_power_nets.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/common/set_rc.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/common/set_routing_layers.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2658 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/cts.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/cut_rows.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      777 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/dpl.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1175 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/drt.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      972 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/fill.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4849 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/floorplan.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2413 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/gpl.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/grt.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/gui.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/insert_buffer.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1893 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/ioplacer.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/irdrop.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/pdn.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/rcx.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/repair_design.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/repair_design_postgrt.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/rsz_timing_postcts.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/rsz_timing_postgrt.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.863603 openlane-2.0.4/openlane/scripts/openroad/sta/
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/sta/check_macro_instances.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)    13662 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/sta/corner.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      935 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/tapcell.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (127)      663 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/openroad/write_views.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.867603 openlane-2.0.4/openlane/scripts/tclsh/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/tclsh/hello.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.867603 openlane-2.0.4/openlane/scripts/yosys/
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/yosys/common.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/yosys/construct_abc_script.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/yosys/json_header.tcl
+-rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/scripts/yosys/synthesize.tcl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.867603 openlane-2.0.4/openlane/state/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/state/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/state/design_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/state/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.871603 openlane-2.0.4/openlane/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12978 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/steps/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/steps/checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/steps/common_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/steps/cvc_rv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16425 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/steps/klayout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16589 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/steps/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/steps/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/steps/netgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29654 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/steps/odb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81058 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/steps/openroad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/steps/openroad_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53312 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/steps/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/steps/tclstep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/steps/verilator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23272 2024-05-01 15:43:06.000000 openlane-2.0.4/openlane/steps/yosys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.847603 openlane-2.0.4/openlane.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-05-01 15:53:37.000000 openlane-2.0.4/openlane.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-01 15:53:37.000000 openlane-2.0.4/openlane.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 15:53:37.000000 openlane-2.0.4/openlane.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-01 15:53:37.000000 openlane-2.0.4/openlane.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-01 15:53:37.000000 openlane-2.0.4/openlane.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 15:53:37.000000 openlane-2.0.4/openlane.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 15:53:37.871603 openlane-2.0.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1776 2024-05-01 15:43:06.000000 openlane-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:53:37.871603 openlane-2.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-01 15:43:06.000000 openlane-2.0.4/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9215 2024-05-01 15:43:06.000000 openlane-2.0.4/test/conftest.py
```

### Comparing `openlane-2.0.3/PKG-INFO` & `openlane-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlane
-Version: 2.0.3
+Version: 2.0.4
 Summary: An infrastructure for implementing chip design flows
 Home-page: UNKNOWN
 Author: Efabless Corporation and Contributors
 Author-email: donn@efabless.com
 License: UNKNOWN
 Description: <h1 align="center">OpenLane</h1>
         <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openlane Version: 2.0.3 Summary: An infrastructure
+Metadata-Version: 2.1 Name: openlane Version: 2.0.4 Summary: An infrastructure
 for implementing chip design flows Home-page: UNKNOWN Author: Efabless
 Corporation and Contributors Author-email: donn@efabless.com License: UNKNOWN
 Description:
                             ************ OOppeennLLaannee ************
   _[_L_i_c_e_n_s_e_:_ _A_p_a_c_h_e_ _2_._0_]_[_P_y_t_h_o_n_ _3_._8_ _o_r_ _h_i_g_h_e_r_]_[_C_o_d_e_ _S_t_y_l_e_:_ _b_l_a_c_k_]_[_C_h_e_c_k_e_d_ _w_i_t_h
                              _m_y_p_y_]_[_B_u_i_l_t_ _w_i_t_h_ _N_i_x_]
   _[_O_p_e_n_ _i_n_ _C_o_l_a_b_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _B_u_i_l_d_ _S_t_a_t_u_s_ _B_a_d_g_e_]_[_I_n_v_i_t_e_ _t_o_ _t_h_e_ _O_p_e_n_ _S_o_u_r_c_e
```

### Comparing `openlane-2.0.3/openlane/__init__.py` & `openlane-2.0.4/openlane/__init__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/__main__.py` & `openlane-2.0.4/openlane/__main__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/__version__.py` & `openlane-2.0.4/openlane/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "2.0.3"
+__version__ = "2.0.4"
 
 if __name__ == "__main__":
     print(__version__, end="")
```

### Comparing `openlane-2.0.3/openlane/common/__init__.py` & `openlane-2.0.4/openlane/common/__init__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/common/cli.py` & `openlane-2.0.4/openlane/common/cli.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/common/drc.py` & `openlane-2.0.4/openlane/common/drc.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/common/generic_dict.py` & `openlane-2.0.4/openlane/common/generic_dict.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/common/metrics/__init__.py` & `openlane-2.0.4/openlane/common/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/common/metrics/__main__.py` & `openlane-2.0.4/openlane/common/metrics/__main__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/common/metrics/library.py` & `openlane-2.0.4/openlane/common/metrics/library.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/common/metrics/metric.py` & `openlane-2.0.4/openlane/common/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/common/metrics/util.py` & `openlane-2.0.4/openlane/common/metrics/util.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/common/misc.py` & `openlane-2.0.4/openlane/common/misc.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/common/ring_buffer.py` & `openlane-2.0.4/openlane/common/ring_buffer.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/common/tcl.py` & `openlane-2.0.4/openlane/common/tcl.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/common/toolbox.py` & `openlane-2.0.4/openlane/common/toolbox.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/common/tpe.py` & `openlane-2.0.4/openlane/common/tpe.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/common/types.py` & `openlane-2.0.4/openlane/common/types.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/config/__init__.py` & `openlane-2.0.4/openlane/config/__init__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/config/__main__.py` & `openlane-2.0.4/openlane/config/__main__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/config/config.py` & `openlane-2.0.4/openlane/config/config.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/config/flow.py` & `openlane-2.0.4/openlane/config/flow.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/config/pdk_compat.py` & `openlane-2.0.4/openlane/config/pdk_compat.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/config/preprocessor.py` & `openlane-2.0.4/openlane/config/preprocessor.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/config/removals.py` & `openlane-2.0.4/openlane/config/removals.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/config/variable.py` & `openlane-2.0.4/openlane/config/variable.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/container.py` & `openlane-2.0.4/openlane/container.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/env_info.py` & `openlane-2.0.4/openlane/env_info.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/examples/spm/config.json` & `openlane-2.0.4/openlane/examples/spm/config.json`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/examples/spm/src/impl.sdc` & `openlane-2.0.4/openlane/examples/spm/src/impl.sdc`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/examples/spm/src/signoff.sdc` & `openlane-2.0.4/openlane/examples/spm/src/signoff.sdc`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/examples/spm/src/spm.v` & `openlane-2.0.4/openlane/examples/spm/src/spm.v`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/examples/spm/verify/spm_tb.v` & `openlane-2.0.4/openlane/examples/spm/verify/spm_tb.v`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/examples/spm-user_project_wrapper/SPM_example.v` & `openlane-2.0.4/openlane/examples/spm-user_project_wrapper/SPM_example.v`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/examples/spm-user_project_wrapper/base_sdc_file.sdc` & `openlane-2.0.4/openlane/examples/spm-user_project_wrapper/base_sdc_file.sdc`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/examples/spm-user_project_wrapper/defines.v` & `openlane-2.0.4/openlane/examples/spm-user_project_wrapper/defines.v`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/examples/spm-user_project_wrapper/template.def` & `openlane-2.0.4/openlane/examples/spm-user_project_wrapper/template.def`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/examples/spm-user_project_wrapper/user_project_wrapper.v` & `openlane-2.0.4/openlane/examples/spm-user_project_wrapper/user_project_wrapper.v`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/flows/__init__.py` & `openlane-2.0.4/openlane/flows/__init__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/flows/builtins.py` & `openlane-2.0.4/openlane/flows/builtins.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/flows/classic.py` & `openlane-2.0.4/openlane/flows/classic.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/flows/cli.py` & `openlane-2.0.4/openlane/flows/cli.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/flows/flow.py` & `openlane-2.0.4/openlane/flows/flow.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/flows/misc.py` & `openlane-2.0.4/openlane/flows/misc.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/flows/optimizing.py` & `openlane-2.0.4/openlane/flows/optimizing.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/flows/sequential.py` & `openlane-2.0.4/openlane/flows/sequential.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/flows/synth_explore.py` & `openlane-2.0.4/openlane/flows/synth_explore.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/logging/__init__.py` & `openlane-2.0.4/openlane/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/logging/logger.py` & `openlane-2.0.4/openlane/logging/logger.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/plugins.py` & `openlane-2.0.4/openlane/plugins.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/base.sdc` & `openlane-2.0.4/openlane/scripts/base.sdc`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/klayout/open_design.py` & `openlane-2.0.4/openlane/scripts/klayout/open_design.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/klayout/render.py` & `openlane-2.0.4/openlane/scripts/klayout/render.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/klayout/stream_out.py` & `openlane-2.0.4/openlane/scripts/klayout/stream_out.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/klayout/xml_drc_report_to_json.py` & `openlane-2.0.4/openlane/scripts/klayout/xml_drc_report_to_json.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/klayout/xor.drc` & `openlane-2.0.4/openlane/scripts/klayout/xor.drc`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/magic/common/read.tcl` & `openlane-2.0.4/openlane/scripts/magic/common/read.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/magic/def/antenna_check.tcl` & `openlane-2.0.4/openlane/scripts/magic/def/antenna_check.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/magic/def/mag.tcl` & `openlane-2.0.4/openlane/scripts/magic/def/mag.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/magic/def/mag_gds.tcl` & `openlane-2.0.4/openlane/scripts/magic/def/mag_gds.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/magic/drc.tcl` & `openlane-2.0.4/openlane/scripts/magic/drc.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/magic/extract_spice.tcl` & `openlane-2.0.4/openlane/scripts/magic/extract_spice.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/magic/gds/drc_batch.tcl` & `openlane-2.0.4/openlane/scripts/magic/gds/drc_batch.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/magic/gds/erase_box.tcl` & `openlane-2.0.4/openlane/scripts/magic/gds/erase_box.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/magic/gds/extras_mag.tcl` & `openlane-2.0.4/openlane/scripts/magic/gds/extras_mag.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/magic/gds/mag_with_pointers.tcl` & `openlane-2.0.4/openlane/scripts/magic/gds/mag_with_pointers.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/magic/lef/extras_maglef.tcl` & `openlane-2.0.4/openlane/scripts/magic/lef/extras_maglef.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/magic/lef/maglef.tcl` & `openlane-2.0.4/openlane/scripts/magic/lef/maglef.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/magic/lef.tcl` & `openlane-2.0.4/openlane/scripts/magic/lef.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/magic/wrapper.tcl` & `openlane-2.0.4/openlane/scripts/magic/wrapper.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/odbpy/apply_def_template.py` & `openlane-2.0.4/openlane/scripts/odbpy/apply_def_template.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/odbpy/check_antenna_properties.py` & `openlane-2.0.4/openlane/scripts/odbpy/check_antenna_properties.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/odbpy/contextualize.py` & `openlane-2.0.4/openlane/scripts/odbpy/contextualize.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/odbpy/defutil.py` & `openlane-2.0.4/openlane/scripts/odbpy/defutil.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/odbpy/diodes.py` & `openlane-2.0.4/openlane/scripts/odbpy/diodes.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/odbpy/disconnected_pins.py` & `openlane-2.0.4/openlane/scripts/odbpy/disconnected_pins.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/odbpy/exception_codes.py` & `openlane-2.0.4/openlane/scripts/odbpy/exception_codes.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/odbpy/filter_unannotated.py` & `openlane-2.0.4/openlane/scripts/odbpy/filter_unannotated.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/odbpy/io_place.py` & `openlane-2.0.4/openlane/scripts/odbpy/io_place.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/odbpy/label_macro_pins.py` & `openlane-2.0.4/openlane/scripts/odbpy/label_macro_pins.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/odbpy/lefutil.py` & `openlane-2.0.4/openlane/scripts/odbpy/lefutil.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/odbpy/manual_macro_place.py` & `openlane-2.0.4/openlane/scripts/odbpy/manual_macro_place.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/odbpy/power_utils.py` & `openlane-2.0.4/openlane/scripts/odbpy/power_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 import odb
 import utl
 
 import re
 import json
-from typing import List
+from typing import List, Optional
 from collections import namedtuple
 
 from reader import OdbReader, click_odb, click
 
 
 @click.group()
 def cli():
@@ -179,40 +179,21 @@
             )
 
         return instances
 
     def add_global_connection(
         design,
         *,
-        net_name=None,
-        inst_pattern=None,
-        pin_pattern=None,
-        power=False,
-        ground=False,
-        region=None,
+        net_name: str,
+        inst_name: str,
+        pin_name: str,
+        power: bool = False,
+        ground: bool = False,
+        region: Optional[odb.dbRegion] = None,
     ):
-        if net_name is None:
-            utl.error(
-                utl.PDN,
-                1501,
-                "The net option for the "
-                + "add_global_connection command is required.",
-            )
-
-        if inst_pattern is None:
-            inst_pattern = ".*"
-
-        if pin_pattern is None:
-            utl.error(
-                utl.PDN,
-                1502,
-                "The pin_pattern option for the "
-                + "add_global_connection command is required.",
-            )
-
         net = design.getBlock().findNet(net_name)
         if net is None:
             net = odb.dbNet_create(design.getBlock(), net_name)
 
         if power and ground:
             utl.error(utl.PDN, 1551, "Only power or ground can be specified")
         elif power:
@@ -222,16 +203,42 @@
             net.setSpecial()
             net.setSigType("GROUND")
 
         if region is not None:
             region = design.getBlock().findRegion(region)
             if region is None:
                 utl.error(utl.PDN, 1504, f"Region {region} not defined")
+                exit(-1)
+
+        inst_def_name = reader.escape_verilog_name(inst_name)
+        pin_def_name = reader.escape_verilog_name(pin_name)
+
+        for term in net.getITerms():
+            if (
+                term.getInst().getName() == inst_def_name
+                and term.getMTerm().getName() == pin_def_name
+            ):
+                print(f"{inst_name}/{pin_name} is already connected to {net.getName()}")
+                return
+
+        connected_items = design.getBlock().addGlobalConnect(
+            region,
+            re.escape(inst_def_name),
+            re.escape(pin_def_name),
+            net,
+            True,
+        )
+        print(f"Made {connected_items} connections.")
 
-        design.getBlock().addGlobalConnect(region, inst_pattern, pin_pattern, net, True)
+        assert (
+            connected_items != 0
+        ), f"Global connect failed to make any connections for '{inst_name}/{pin_name}' to {net_name}"
+        assert (
+            connected_items == 1
+        ), f"Global connect somehow made multiple connections for '{inst_name}/{pin_name}' to {net_name} -- please report this as a bug"
 
     design_str = open(input_json).read()
     design_dict = json.loads(design_str)
 
     db = reader.db
     chip = db.getChip()
     design_name = chip.getBlock().getName()
@@ -239,27 +246,27 @@
     macro_instances = extract_instances(db, design_dict, design_name)
     for instance in macro_instances:
         for pin in instance.power_connections.keys():
             net_name = instance.power_connections[pin]
             print(f"Connecting power net {net_name} to {instance.name}/{pin}…")
             add_global_connection(
                 design=chip,
-                inst_pattern=re.escape(instance.name),
+                inst_name=instance.name,
                 net_name=net_name,
-                pin_pattern=pin,
+                pin_name=pin,
                 power=True,
             )
         for pin in instance.ground_connections.keys():
             net_name = instance.ground_connections[pin]
             print(f"Connecting ground net {net_name} to {instance.name}/{pin}…")
             add_global_connection(
                 design=chip,
-                inst_pattern=re.escape(instance.name),
+                inst_name=instance.name,
                 net_name=net_name,
-                pin_pattern=pin,
+                pin_name=pin,
                 ground=True,
             )
 
 
 cli.add_command(set_power_connections)
```

### Comparing `openlane-2.0.3/openlane/scripts/odbpy/random_place.py` & `openlane-2.0.4/openlane/scripts/odbpy/random_place.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/odbpy/reader.py` & `openlane-2.0.4/openlane/scripts/odbpy/reader.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/odbpy/remove_buffers.py` & `openlane-2.0.4/openlane/scripts/odbpy/remove_buffers.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/odbpy/snap_to_grid.py` & `openlane-2.0.4/openlane/scripts/odbpy/snap_to_grid.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/odbpy/wire_lengths.py` & `openlane-2.0.4/openlane/scripts/odbpy/wire_lengths.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/antenna_check.tcl` & `openlane-2.0.4/openlane/scripts/openroad/antenna_check.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/antenna_repair.tcl` & `openlane-2.0.4/openlane/scripts/openroad/antenna_repair.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/basic_mp.tcl` & `openlane-2.0.4/openlane/scripts/openroad/basic_mp.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/common/dpl.tcl` & `openlane-2.0.4/openlane/scripts/openroad/common/dpl.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/common/dpl_cell_pad.tcl` & `openlane-2.0.4/openlane/scripts/openroad/common/dpl_cell_pad.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/common/grt.tcl` & `openlane-2.0.4/openlane/scripts/openroad/common/grt.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/common/io.tcl` & `openlane-2.0.4/openlane/scripts/openroad/common/io.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/common/pdn_cfg.tcl` & `openlane-2.0.4/openlane/scripts/openroad/common/pdn_cfg.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/common/resizer.tcl` & `openlane-2.0.4/openlane/scripts/openroad/common/resizer.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/common/set_global_connections.tcl` & `openlane-2.0.4/openlane/scripts/openroad/common/set_global_connections.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/common/set_layer_adjustments.tcl` & `openlane-2.0.4/openlane/scripts/openroad/common/set_layer_adjustments.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/common/set_power_nets.tcl` & `openlane-2.0.4/openlane/scripts/openroad/common/set_power_nets.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/common/set_rc.tcl` & `openlane-2.0.4/openlane/scripts/openroad/common/set_rc.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/common/set_routing_layers.tcl` & `openlane-2.0.4/openlane/scripts/openroad/common/set_routing_layers.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/cts.tcl` & `openlane-2.0.4/openlane/scripts/openroad/cts.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/cut_rows.tcl` & `openlane-2.0.4/openlane/scripts/openroad/cut_rows.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/dpl.tcl` & `openlane-2.0.4/openlane/scripts/openroad/dpl.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/drt.tcl` & `openlane-2.0.4/openlane/scripts/openroad/drt.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/fill.tcl` & `openlane-2.0.4/openlane/scripts/openroad/fill.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/floorplan.tcl` & `openlane-2.0.4/openlane/scripts/openroad/floorplan.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/gpl.tcl` & `openlane-2.0.4/openlane/scripts/openroad/gpl.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/grt.tcl` & `openlane-2.0.4/openlane/scripts/openroad/grt.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/gui.tcl` & `openlane-2.0.4/openlane/scripts/openroad/gui.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/insert_buffer.tcl` & `openlane-2.0.4/openlane/scripts/openroad/insert_buffer.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/ioplacer.tcl` & `openlane-2.0.4/openlane/scripts/openroad/ioplacer.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/irdrop.tcl` & `openlane-2.0.4/openlane/scripts/openroad/irdrop.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/pdn.tcl` & `openlane-2.0.4/openlane/scripts/openroad/pdn.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/rcx.tcl` & `openlane-2.0.4/openlane/scripts/openroad/rcx.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/repair_design.tcl` & `openlane-2.0.4/openlane/scripts/openroad/repair_design.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/repair_design_postgrt.tcl` & `openlane-2.0.4/openlane/scripts/openroad/repair_design_postgrt.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/rsz_timing_postcts.tcl` & `openlane-2.0.4/openlane/scripts/openroad/rsz_timing_postcts.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/rsz_timing_postgrt.tcl` & `openlane-2.0.4/openlane/scripts/openroad/rsz_timing_postgrt.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/sta/check_macro_instances.tcl` & `openlane-2.0.4/openlane/scripts/openroad/sta/check_macro_instances.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/sta/corner.tcl` & `openlane-2.0.4/openlane/scripts/openroad/sta/corner.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/tapcell.tcl` & `openlane-2.0.4/openlane/scripts/openroad/tapcell.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/openroad/write_views.tcl` & `openlane-2.0.4/openlane/scripts/openroad/write_views.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/yosys/common.tcl` & `openlane-2.0.4/openlane/scripts/yosys/common.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/yosys/construct_abc_script.tcl` & `openlane-2.0.4/openlane/scripts/yosys/construct_abc_script.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/scripts/yosys/json_header.tcl` & `openlane-2.0.4/openlane/scripts/yosys/json_header.tcl`

 * *Files 7% similar despite different names*

```diff
@@ -16,8 +16,10 @@
 
 source $::env(_DEPS_SCRIPT)
 
 yosys_ol::read_verilog_files $::env(DESIGN_NAME)
 hierarchy -check -top $::env(DESIGN_NAME) -nokeep_prints -nokeep_asserts
 yosys rename -top $::env(DESIGN_NAME)
 yosys proc
+flatten
+opt_clean -purge
 json -o $::env(SAVE_JSON_HEADER)
```

### Comparing `openlane-2.0.3/openlane/scripts/yosys/synthesize.tcl` & `openlane-2.0.4/openlane/scripts/yosys/synthesize.tcl`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/state/__init__.py` & `openlane-2.0.4/openlane/state/__init__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/state/__main__.py` & `openlane-2.0.4/openlane/state/__main__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/state/design_format.py` & `openlane-2.0.4/openlane/state/design_format.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/state/state.py` & `openlane-2.0.4/openlane/state/state.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/steps/__init__.py` & `openlane-2.0.4/openlane/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/steps/__main__.py` & `openlane-2.0.4/openlane/steps/__main__.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/steps/checker.py` & `openlane-2.0.4/openlane/steps/checker.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/steps/common_variables.py` & `openlane-2.0.4/openlane/steps/common_variables.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/steps/cvc_rv.py` & `openlane-2.0.4/openlane/steps/cvc_rv.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/steps/klayout.py` & `openlane-2.0.4/openlane/steps/klayout.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/steps/magic.py` & `openlane-2.0.4/openlane/steps/magic.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/steps/misc.py` & `openlane-2.0.4/openlane/steps/misc.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/steps/netgen.py` & `openlane-2.0.4/openlane/steps/netgen.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/steps/odb.py` & `openlane-2.0.4/openlane/steps/odb.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/steps/openroad.py` & `openlane-2.0.4/openlane/steps/openroad.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/steps/openroad_alerts.py` & `openlane-2.0.4/openlane/steps/openroad_alerts.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/steps/step.py` & `openlane-2.0.4/openlane/steps/step.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/steps/tclstep.py` & `openlane-2.0.4/openlane/steps/tclstep.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/steps/verilator.py` & `openlane-2.0.4/openlane/steps/verilator.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane/steps/yosys.py` & `openlane-2.0.4/openlane/steps/yosys.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/openlane.egg-info/PKG-INFO` & `openlane-2.0.4/openlane.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlane
-Version: 2.0.3
+Version: 2.0.4
 Summary: An infrastructure for implementing chip design flows
 Home-page: UNKNOWN
 Author: Efabless Corporation and Contributors
 Author-email: donn@efabless.com
 License: UNKNOWN
 Description: <h1 align="center">OpenLane</h1>
         <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openlane Version: 2.0.3 Summary: An infrastructure
+Metadata-Version: 2.1 Name: openlane Version: 2.0.4 Summary: An infrastructure
 for implementing chip design flows Home-page: UNKNOWN Author: Efabless
 Corporation and Contributors Author-email: donn@efabless.com License: UNKNOWN
 Description:
                             ************ OOppeennLLaannee ************
   _[_L_i_c_e_n_s_e_:_ _A_p_a_c_h_e_ _2_._0_]_[_P_y_t_h_o_n_ _3_._8_ _o_r_ _h_i_g_h_e_r_]_[_C_o_d_e_ _S_t_y_l_e_:_ _b_l_a_c_k_]_[_C_h_e_c_k_e_d_ _w_i_t_h
                              _m_y_p_y_]_[_B_u_i_l_t_ _w_i_t_h_ _N_i_x_]
   _[_O_p_e_n_ _i_n_ _C_o_l_a_b_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _B_u_i_l_d_ _S_t_a_t_u_s_ _B_a_d_g_e_]_[_I_n_v_i_t_e_ _t_o_ _t_h_e_ _O_p_e_n_ _S_o_u_r_c_e
```

### Comparing `openlane-2.0.3/openlane.egg-info/SOURCES.txt` & `openlane-2.0.4/openlane.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/setup.py` & `openlane-2.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `openlane-2.0.3/test/conftest.py` & `openlane-2.0.4/test/conftest.py`

 * *Files identical despite different names*


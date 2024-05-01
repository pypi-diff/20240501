# Comparing `tmp/cellprofiler_core_nightly-5.0.0.dev65.tar.gz` & `tmp/cellprofiler_core_nightly-5.0.0.dev69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellprofiler_core_nightly-5.0.0.dev65.tar", last modified: Tue Apr 30 22:04:46 2024, max compression
+gzip compressed data, was "cellprofiler_core_nightly-5.0.0.dev69.tar", last modified: Wed May  1 00:10:19 2024, max compression
```

## Comparing `cellprofiler_core_nightly-5.0.0.dev65.tar` & `cellprofiler_core_nightly-5.0.0.dev69.tar`

### file list

```diff
@@ -1,374 +1,374 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.302487 cellprofiler_core_nightly-5.0.0.dev65/
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5806 2024-04-30 22:04:46.302487 cellprofiler_core_nightly-5.0.0.dev65/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.242487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-30 22:04:45.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.242487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    30695 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.246487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/event/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/event/_finished.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/event/_paused.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/event/_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/event/_resumed.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/event/_started.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.246487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/reply/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/reply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/reply/_ack.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/reply/_debug_cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/reply/_dictionary_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/reply/_exception_please_debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/reply/_image_set_success.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/reply/_image_set_success_with_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/reply/_interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/reply/_no_work.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/reply/_omero_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/reply/_server_exited.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/reply/_shared_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/reply/_work.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.250487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/request/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/request/_analysis_cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/request/_debug_complete.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/request/_debug_waiting.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/request/_display.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/request/_display_post_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/request/_display_post_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/request/_exception_report.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/request/_initial_measurements.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/request/_interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/request/_measurements_report.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/request/_omero_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/request/_pipeline_preferences.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/request/_shared_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/request/_work.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.250487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/bioformats/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/bioformats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/bioformats/formatreader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/bioformats/formatwriter.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/bioformats/omexml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.250487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/commands/_pipeline_command.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/commands/_worker_command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.250487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/measurement.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.254487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/module/
--rw-r--r--   0 runner    (1001) docker     (127)    10545 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/module/_identify.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.254487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/modules/images.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/modules/load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/modules/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/modules/namesandtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/preferences.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.254487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/reader/
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/setting.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.254487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/_grayscale_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    11802 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/_image_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/_image_set_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/_rgb_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.254487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/abstract_image/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/abstract_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/abstract_image/_abstract_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/abstract_image/_callback_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/abstract_image/_vanilla_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.254487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/abstract_image/file/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/abstract_image/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14440 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/abstract_image/file/_file_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/abstract_image/file/_flex_frame_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/abstract_image/file/_movie_frame_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/abstract_image/file/_stk_frame_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.258487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/abstract_image/file/url/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/abstract_image/file/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/abstract_image/file/url/_color_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/abstract_image/file/url/_mask_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/abstract_image/file/url/_monochrome_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/abstract_image/file/url/_objects_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/abstract_image/file/url/_url_image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.258487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/measurement/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/measurement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    71601 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/measurement/_measurements.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/measurement/_metadata_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/measurement/_relationship_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.258487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/module/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/module/_identify.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/module/_image_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    38402 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/module/_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/module/_plugin_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.258487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/module/image_segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/module/image_segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/module/image_segmentation/_image_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/module/image_segmentation/_object_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.262487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30948 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/modules/align.py
--rw-r--r--   0 runner    (1001) docker     (127)    33346 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/modules/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    16864 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/modules/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/modules/inject_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/modules/injectimage.py
--rw-r--r--   0 runner    (1001) docker     (127)    62037 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/modules/loaddata.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/modules/measurementfixture.py
--rw-r--r--   0 runner    (1001) docker     (127)    60483 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/modules/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    83468 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/modules/namesandtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/modules/setting_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.262487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/object/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/object/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/object/_object_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    13565 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/object/_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/object/_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.262487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/_image_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/_image_plane.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/_image_set_channel_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)   107830 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.266487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/dependency/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/dependency/_dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/dependency/_image_dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/dependency/_measurement_dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/dependency/_object_dependency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.266487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/_end_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/_file_walk_ended.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/_file_walk_started.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/_ipd_load_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/_load_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/_module_added.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/_module_disabled.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/_module_edited.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/_module_enabled.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/_module_moved.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/_module_removed.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/_module_show_window.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/_pipeline_cleared.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/_pipeline_loaded.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/_prepare_run_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/_urls_added.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/_urls_cleared.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/_urls_removed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.270487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/run_exception/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/run_exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/run_exception/_post_run_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/run_exception/_prepare_run_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/run_exception/_run_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.270487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/io/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/io/_v5.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/io/_v6.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.270487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/preferences/
--rw-r--r--   0 runner    (1001) docker     (127)    66726 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/preferences/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/preferences/_headless_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.270487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/reader/
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/reader/_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.270487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/readers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13253 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/readers/bioformats_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/readers/gcs_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/readers/imageio_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    15122 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/readers/ngff_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.274487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_binary_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_delete_setting_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_divider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_do_things.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_figure_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)    12855 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_file_collection_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_hidden_count.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_html_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_image_plane.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_joiner.py
--rw-r--r--   0 runner    (1001) docker     (127)    13419 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_path_list_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_regexp_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_setting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_settings_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_structuring_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_tree_choice.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_validation_error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.274487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/change_setting_event/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/change_setting_event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/change_setting_event/_after_change_setting_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/change_setting_event/_before_change_setting_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/change_setting_event/_change_setting_event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.274487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/choice/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/choice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/choice/_choice.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/choice/_colormap.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/choice/_custom_choice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.278487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/do_something/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/do_something/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/do_something/_do_something.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/do_something/_image_set_display.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/do_something/_path_list_extract_button.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/do_something/_path_list_refresh_button.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/do_something/_remove_setting_button.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.278487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/filter/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/filter/_compound_filter_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/filter/_directory_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/filter/_does_not_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/filter/_does_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/filter/_extension_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/filter/_file_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10163 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/filter/_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/filter/_filter_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/filter/_image_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/filter/_metadata_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/filter/_regexp_filter_predicate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.282487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/multichoice/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/multichoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/multichoice/_image_name_subscriber_multichoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/multichoice/_measurement_multichoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/multichoice/_multichoice.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/multichoice/_object_subscriber_multichoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/multichoice/_subdirectory_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/multichoice/_subscriber_multichoice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.282487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/range/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/range/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/range/_float_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/range/_range.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.282487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/range/integer_range/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/range/integer_range/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/range/integer_range/_integer_or_unbounded_range.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/range/integer_range/_integer_range.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.282487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/subscriber/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/subscriber/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/subscriber/_grid_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/subscriber/_label_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/subscriber/_subscriber.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.282487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/subscriber/image_subscriber/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/subscriber/image_subscriber/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/subscriber/image_subscriber/_crop_image_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/subscriber/image_subscriber/_file_image_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/subscriber/image_subscriber/_image_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/subscriber/image_subscriber/_outline_image_subscriber.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.282487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/subscriber/list_subscriber/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/subscriber/list_subscriber/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/subscriber/list_subscriber/_image_list_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/subscriber/list_subscriber/_label_list_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/subscriber/list_subscriber/_list_subscriber.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.286487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8990 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/_filename.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/_text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.286487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/alphanumeric/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/alphanumeric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/alphanumeric/_alphanumeric.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/alphanumeric/_character.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.286487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/alphanumeric/name/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/alphanumeric/name/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/alphanumeric/name/_grid_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/alphanumeric/name/_label_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/alphanumeric/name/_name.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.286487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/alphanumeric/name/image_name/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/alphanumeric/name/image_name/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/alphanumeric/name/image_name/_crop_image_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/alphanumeric/name/image_name/_external_image_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/alphanumeric/name/image_name/_file_image_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/alphanumeric/name/image_name/_image_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/alphanumeric/name/image_name/_outline_image_name.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.286487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/number/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/number/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/number/_float.py
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/number/_number.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.290487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/number/integer/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/number/integer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/number/integer/_integer.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/number/integer/_odd_integer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.290487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/pathname/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/pathname/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/pathname/_pathname.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/pathname/_url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.290487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/channel_hasher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.290487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.294487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/core/module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/core/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/core/module/identify.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.294487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/core/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/core/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/core/modules/load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/core/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/core/object.py
--rw-r--r--   0 runner    (1001) docker     (127)    12001 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/core/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/core/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/core/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)   106050 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/hdf5_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    11593 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/java.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/measurement.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/pathname.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/utf16encode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.294487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/zmq/
--rw-r--r--   0 runner    (1001) docker     (127)    12392 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/zmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/zmq/_analysis_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    12488 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/zmq/_boundary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.294487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/zmq/communicable/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/zmq/communicable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/zmq/communicable/_communicable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.294487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/zmq/communicable/reply/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/zmq/communicable/reply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/zmq/communicable/reply/_lock_status_reply.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/zmq/communicable/reply/_reply.py
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/zmq/communicable/reply/_upstream_exit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.294487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/zmq/communicable/reply/upstream_exit/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/zmq/communicable/reply/upstream_exit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/zmq/communicable/reply/upstream_exit/_boundary_exited.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/zmq/communicable/reply/upstream_exit/_upstream_exit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.294487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/zmq/communicable/request/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/zmq/communicable/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/zmq/communicable/request/_analysis_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/zmq/communicable/request/_lock_status_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/zmq/communicable/request/_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.298487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/worker/
--rw-r--r--   0 runner    (1001) docker     (127)    10969 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/worker/_pipeline_event_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)    20260 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/worker/_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.298487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/workspace/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/workspace/_disposition_changed_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    21602 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/workspace/_workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 22:04:46.298487 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5806 2024-04-30 22:04:45.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15936 2024-04-30 22:04:46.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 22:04:45.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-30 22:04:45.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-30 22:04:45.000000 cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-30 22:04:19.000000 cellprofiler_core_nightly-5.0.0.dev65/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-30 22:04:29.000000 cellprofiler_core_nightly-5.0.0.dev65/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 22:04:46.302487 cellprofiler_core_nightly-5.0.0.dev65/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.932867 cellprofiler_core_nightly-5.0.0.dev69/
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-05-01 00:10:19.932867 cellprofiler_core_nightly-5.0.0.dev69/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.872867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-01 00:10:18.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.872867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30695 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.872867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/event/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/event/_finished.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/event/_paused.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/event/_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/event/_resumed.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/event/_started.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.876867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/reply/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/reply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/reply/_ack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/reply/_debug_cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/reply/_dictionary_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/reply/_exception_please_debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/reply/_image_set_success.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/reply/_image_set_success_with_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/reply/_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/reply/_no_work.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/reply/_omero_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/reply/_server_exited.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/reply/_shared_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/reply/_work.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.876867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/request/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/request/_analysis_cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/request/_debug_complete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/request/_debug_waiting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/request/_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/request/_display_post_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/request/_display_post_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/request/_exception_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/request/_initial_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/request/_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/request/_measurements_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/request/_omero_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/request/_pipeline_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/request/_shared_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/request/_work.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.880867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/bioformats/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/bioformats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/bioformats/formatreader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/bioformats/formatwriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/bioformats/omexml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.880867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/commands/_pipeline_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/commands/_worker_command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.880867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/measurement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.880867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/module/
+-rw-r--r--   0 runner    (1001) docker     (127)    10545 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/module/_identify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.880867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/modules/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/modules/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/modules/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/modules/namesandtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/preferences.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.884867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.884867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/_grayscale_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11802 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/_image_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/_image_set_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/_rgb_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.884867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/abstract_image/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/abstract_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/abstract_image/_abstract_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/abstract_image/_callback_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/abstract_image/_vanilla_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.884867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/abstract_image/file/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/abstract_image/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14440 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/abstract_image/file/_file_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/abstract_image/file/_flex_frame_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/abstract_image/file/_movie_frame_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/abstract_image/file/_stk_frame_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.884867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/abstract_image/file/url/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/abstract_image/file/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/abstract_image/file/url/_color_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/abstract_image/file/url/_mask_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/abstract_image/file/url/_monochrome_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/abstract_image/file/url/_objects_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/abstract_image/file/url/_url_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.888867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/measurement/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/measurement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71601 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/measurement/_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/measurement/_metadata_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/measurement/_relationship_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.888867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/module/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/module/_identify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/module/_image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38402 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/module/_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/module/_plugin_importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.888867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/module/image_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/module/image_segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/module/image_segmentation/_image_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/module/image_segmentation/_object_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.892867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30948 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/modules/align.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33346 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/modules/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16864 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/modules/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/modules/inject_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/modules/injectimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62037 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/modules/loaddata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/modules/measurementfixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60483 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/modules/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83468 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/modules/namesandtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/modules/setting_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.892867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/object/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/object/_object_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13565 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/object/_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/object/_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.892867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/_image_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/_image_plane.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/_image_set_channel_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)   107830 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.892867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/dependency/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/dependency/_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/dependency/_image_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/dependency/_measurement_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/dependency/_object_dependency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.896867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/_end_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/_file_walk_ended.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/_file_walk_started.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/_ipd_load_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/_load_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/_module_added.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/_module_disabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/_module_edited.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/_module_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/_module_moved.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/_module_removed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/_module_show_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/_pipeline_cleared.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/_pipeline_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/_prepare_run_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/_urls_added.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/_urls_cleared.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/_urls_removed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.900867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/run_exception/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/run_exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/run_exception/_post_run_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/run_exception/_prepare_run_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/run_exception/_run_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.900867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/io/_v5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/io/_v6.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.900867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/preferences/
+-rw-r--r--   0 runner    (1001) docker     (127)    66726 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/preferences/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/preferences/_headless_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.900867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/reader/
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/reader/_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.900867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/readers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13253 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/readers/bioformats_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/readers/gcs_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/readers/imageio_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15122 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/readers/ngff_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.904867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_binary_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_delete_setting_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_divider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_do_things.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_figure_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12855 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_file_collection_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_hidden_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_html_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_image_plane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_joiner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13419 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_path_list_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_regexp_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_setting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_settings_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_structuring_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_tree_choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_validation_error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.904867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/change_setting_event/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/change_setting_event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/change_setting_event/_after_change_setting_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/change_setting_event/_before_change_setting_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/change_setting_event/_change_setting_event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.908867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/choice/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/choice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/choice/_choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/choice/_colormap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/choice/_custom_choice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.908867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/do_something/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/do_something/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/do_something/_do_something.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/do_something/_image_set_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/do_something/_path_list_extract_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/do_something/_path_list_refresh_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/do_something/_remove_setting_button.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.908867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/filter/_compound_filter_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/filter/_directory_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/filter/_does_not_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/filter/_does_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/filter/_extension_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/filter/_file_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10163 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/filter/_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/filter/_filter_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/filter/_image_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/filter/_metadata_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/filter/_regexp_filter_predicate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.912867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/multichoice/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/multichoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/multichoice/_image_name_subscriber_multichoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/multichoice/_measurement_multichoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/multichoice/_multichoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/multichoice/_object_subscriber_multichoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/multichoice/_subdirectory_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/multichoice/_subscriber_multichoice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.912867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/range/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/range/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/range/_float_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/range/_range.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.912867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/range/integer_range/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/range/integer_range/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/range/integer_range/_integer_or_unbounded_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/range/integer_range/_integer_range.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.912867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/subscriber/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/subscriber/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/subscriber/_grid_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/subscriber/_label_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/subscriber/_subscriber.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.912867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/subscriber/image_subscriber/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/subscriber/image_subscriber/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/subscriber/image_subscriber/_crop_image_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/subscriber/image_subscriber/_file_image_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/subscriber/image_subscriber/_image_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/subscriber/image_subscriber/_outline_image_subscriber.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.916867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/subscriber/list_subscriber/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/subscriber/list_subscriber/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/subscriber/list_subscriber/_image_list_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/subscriber/list_subscriber/_label_list_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/subscriber/list_subscriber/_list_subscriber.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.916867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8990 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/_filename.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.916867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/alphanumeric/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/alphanumeric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/alphanumeric/_alphanumeric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/alphanumeric/_character.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.916867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/alphanumeric/name/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/alphanumeric/name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/alphanumeric/name/_grid_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/alphanumeric/name/_label_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/alphanumeric/name/_name.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.916867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/alphanumeric/name/image_name/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/alphanumeric/name/image_name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/alphanumeric/name/image_name/_crop_image_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/alphanumeric/name/image_name/_external_image_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/alphanumeric/name/image_name/_file_image_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/alphanumeric/name/image_name/_image_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/alphanumeric/name/image_name/_outline_image_name.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.920867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/number/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/number/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/number/_float.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/number/_number.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.920867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/number/integer/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/number/integer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/number/integer/_integer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/number/integer/_odd_integer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.920867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/pathname/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/pathname/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/pathname/_pathname.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/pathname/_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.920867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/channel_hasher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.924867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.924867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/core/module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/core/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/core/module/identify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.924867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/core/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/core/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/core/modules/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/core/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/core/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12001 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/core/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/core/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/core/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)   106050 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/hdf5_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11593 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/java.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5985 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/pathname.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/utf16encode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.924867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/zmq/
+-rw-r--r--   0 runner    (1001) docker     (127)    12392 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/zmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/zmq/_analysis_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12488 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/zmq/_boundary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.924867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/zmq/communicable/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/zmq/communicable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/zmq/communicable/_communicable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.924867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/zmq/communicable/reply/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/zmq/communicable/reply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/zmq/communicable/reply/_lock_status_reply.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/zmq/communicable/reply/_reply.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/zmq/communicable/reply/_upstream_exit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.924867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/zmq/communicable/reply/upstream_exit/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/zmq/communicable/reply/upstream_exit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/zmq/communicable/reply/upstream_exit/_boundary_exited.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/zmq/communicable/reply/upstream_exit/_upstream_exit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.928867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/zmq/communicable/request/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/zmq/communicable/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/zmq/communicable/request/_analysis_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/zmq/communicable/request/_lock_status_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/zmq/communicable/request/_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.928867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)    10969 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/worker/_pipeline_event_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20260 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/worker/_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.928867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/workspace/_disposition_changed_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21602 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/workspace/_workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 00:10:19.928867 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-05-01 00:10:18.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15936 2024-05-01 00:10:19.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 00:10:18.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-01 00:10:18.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 00:10:18.000000 cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-01 00:09:42.000000 cellprofiler_core_nightly-5.0.0.dev69/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-01 00:09:58.000000 cellprofiler_core_nightly-5.0.0.dev69/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 00:10:19.932867 cellprofiler_core_nightly-5.0.0.dev69/setup.cfg
```

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/LICENSE` & `cellprofiler_core_nightly-5.0.0.dev69/LICENSE`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/PKG-INFO` & `cellprofiler_core_nightly-5.0.0.dev69/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellprofiler-core-nightly
-Version: 5.0.0.dev65
+Version: 5.0.0.dev69
 Summary: cellprofiler-core implements the bulk of CellProfiler's non-gui functionality
 Author: Anne Carpenter, Thouis (Ray) Jones, Lee Kamentsky, Vebjorn Ljosa, David Logan, Mark Bray, Madison Swain-Bowden, Allen Goodman, Claire McQuinn, Alice Lucas, Callum Tromans-Coia
 Author-email: Beth Cimini <bcimini@broadinstitute.org>, David Stirling <dstirling@glencoesoftware.com>, Nodar Gogoberidze <ngogober@broadinstitute.org>
 Maintainer-email: Beth Cimini <bcimini@broadinstitute.org>, Nodar Gogoberidze <ngogober@broadinstitute.org>
 License: The BSD 3-Clause License
         
         Copyright © 2003 - 2021 Broad Institute, Inc. All rights reserved.
@@ -94,8 +94,8 @@
 Requires-Dist: pytest~=7.4.1; extra == "test"
 Requires-Dist: pytest-timeout~=2.1.0; extra == "test"
 Provides-Extra: wx
 Requires-Dist: wxPython==4.2.0; extra == "wx"
 
 # core
 
-This subpackage contains the code to build the `cellprofiler-core` package. It contains the critical classes and components required by the [CellProfiler](cellprofiler.org) software, whereas the [frontend](../../frontend/) contains non-essential modules and the GUI interface. This package can be used in isolation, separate from the frontend, to access CellProfiler's functionality as a Python package, see [this page](https://github.com/CellProfiler/CellProfiler/wiki/CellProfiler-as-a-Python-package) for more details.
+This subpackage contains the code to build the `cellprofiler-core` package. It contains the critical classes and components required by the [CellProfiler](https://cellprofiler.org) software, whereas the [frontend](https://github.com/CellProfiler/CellProfiler/tree/main/src/frontend) contains non-essential modules and the GUI interface. This package can be used in isolation, separate from the frontend, to access CellProfiler's functionality as a Python package, see [this page](https://github.com/CellProfiler/CellProfiler/wiki/CellProfiler-as-a-Python-package) for more details.
```

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/__main__.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/__main__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/__init__.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/_analysis.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/_analysis.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/_runner.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/_runner.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/reply/__init__.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/reply/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/request/__init__.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/request/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/analysis/request/_exception_report.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/analysis/request/_exception_report.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/bioformats/formatwriter.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/bioformats/formatwriter.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/commands/_pipeline_command.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/commands/_pipeline_command.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/image.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/measurement.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/measurement.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/module/__init__.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/module/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/module/_identify.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/module/_identify.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/modules/__init__.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/modules/load_data.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/modules/load_data.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/modules/metadata.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/modules/metadata.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/modules/namesandtypes.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/modules/namesandtypes.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/pipeline.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/pipeline.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/reader/__init__.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/constants/setting.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/constants/setting.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/__init__.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/_grayscale_image.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/_grayscale_image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/_image.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/_image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/_image_set.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/_image_set.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/_image_set_list.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/_image_set_list.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/abstract_image/_abstract_image.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/abstract_image/_abstract_image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/abstract_image/_callback_image.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/abstract_image/_callback_image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/abstract_image/_vanilla_image.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/abstract_image/_vanilla_image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/abstract_image/file/_file_image.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/abstract_image/file/_file_image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/abstract_image/file/_stk_frame_image.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/abstract_image/file/_stk_frame_image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/abstract_image/file/url/_color_image.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/abstract_image/file/url/_color_image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/abstract_image/file/url/_mask_image.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/abstract_image/file/url/_mask_image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/abstract_image/file/url/_monochrome_image.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/abstract_image/file/url/_monochrome_image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/abstract_image/file/url/_objects_image.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/abstract_image/file/url/_objects_image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/image/abstract_image/file/url/_url_image.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/image/abstract_image/file/url/_url_image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/measurement/_measurements.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/measurement/_measurements.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/measurement/_metadata_group.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/measurement/_metadata_group.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/module/_identify.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/module/_identify.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/module/_image_processing.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/module/_image_processing.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/module/_module.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/module/_module.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/module/_plugin_importer.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/module/_plugin_importer.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/module/image_segmentation/_image_segmentation.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/module/image_segmentation/_image_segmentation.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/module/image_segmentation/_object_processing.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/module/image_segmentation/_object_processing.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/modules/align.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/modules/align.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/modules/groups.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/modules/groups.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/modules/images.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/modules/images.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/modules/inject_objects.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/modules/inject_objects.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/modules/injectimage.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/modules/injectimage.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/modules/loaddata.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/modules/loaddata.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/modules/measurementfixture.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/modules/measurementfixture.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/modules/metadata.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/modules/metadata.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/modules/namesandtypes.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/modules/namesandtypes.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/modules/setting_validation.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/modules/setting_validation.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/object/_object_set.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/object/_object_set.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/object/_objects.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/object/_objects.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/object/_segmentation.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/object/_segmentation.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/__init__.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/_image_file.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/_image_file.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/_image_plane.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/_image_plane.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/_image_set_channel_descriptor.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/_image_set_channel_descriptor.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/_listener.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/_listener.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/_pipeline.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/_pipeline.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/dependency/_dependency.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/dependency/_dependency.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/dependency/_image_dependency.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/dependency/_image_dependency.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/dependency/_measurement_dependency.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/dependency/_measurement_dependency.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/dependency/_object_dependency.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/dependency/_object_dependency.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/__init__.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/_event.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/_event.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/event/run_exception/_run_exception.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/event/run_exception/_run_exception.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/io/__init__.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/io/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/io/_v5.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/io/_v5.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/pipeline/io/_v6.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/pipeline/io/_v6.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/preferences/__init__.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/preferences/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/preferences/_headless_configuration.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/preferences/_headless_configuration.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/reader/__init__.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/reader/_reader.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/reader/_reader.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/readers/bioformats_reader.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/readers/bioformats_reader.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/readers/gcs_reader.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/readers/gcs_reader.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/readers/imageio_reader.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/readers/imageio_reader.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/readers/ngff_reader.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/readers/ngff_reader.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/__init__.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_binary.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_binary.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_binary_matrix.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_binary_matrix.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_color.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_color.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_coordinates.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_coordinates.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_data_types.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_data_types.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_do_things.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_do_things.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_figure_subscriber.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_figure_subscriber.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_file_collection_display.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_file_collection_display.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_hidden_count.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_hidden_count.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_html_text.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_html_text.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_image_plane.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_image_plane.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_joiner.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_joiner.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_measurement.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_measurement.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_regexp_text.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_regexp_text.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_setting.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_setting.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_settings_group.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_settings_group.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_structuring_element.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_structuring_element.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_table.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_table.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_tree_choice.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_tree_choice.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/_validation_error.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/_validation_error.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/change_setting_event/_before_change_setting_event.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/change_setting_event/_before_change_setting_event.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/choice/_choice.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/choice/_choice.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/choice/_custom_choice.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/choice/_custom_choice.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/do_something/_do_something.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/do_something/_do_something.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/filter/__init__.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/filter/_directory_predicate.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/filter/_directory_predicate.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/filter/_extension_predicate.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/filter/_extension_predicate.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/filter/_file_predicate.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/filter/_file_predicate.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/filter/_filter.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/filter/_filter.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/filter/_filter_predicate.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/filter/_filter_predicate.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/filter/_image_predicate.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/filter/_image_predicate.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/filter/_metadata_predicate.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/filter/_metadata_predicate.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/filter/_regexp_filter_predicate.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/filter/_regexp_filter_predicate.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/multichoice/_measurement_multichoice.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/multichoice/_measurement_multichoice.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/multichoice/_multichoice.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/multichoice/_multichoice.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/multichoice/_subdirectory_filter.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/multichoice/_subdirectory_filter.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/multichoice/_subscriber_multichoice.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/multichoice/_subscriber_multichoice.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/range/_float_range.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/range/_float_range.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/range/_range.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/range/_range.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/range/integer_range/_integer_or_unbounded_range.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/range/integer_range/_integer_or_unbounded_range.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/range/integer_range/_integer_range.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/range/integer_range/_integer_range.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/subscriber/_subscriber.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/subscriber/_subscriber.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/subscriber/image_subscriber/_crop_image_subscriber.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/subscriber/image_subscriber/_crop_image_subscriber.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/subscriber/image_subscriber/_file_image_subscriber.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/subscriber/image_subscriber/_file_image_subscriber.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/subscriber/image_subscriber/_outline_image_subscriber.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/subscriber/image_subscriber/_outline_image_subscriber.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/subscriber/list_subscriber/_list_subscriber.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/subscriber/list_subscriber/_list_subscriber.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/__init__.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/_directory.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/_directory.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/_filename.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/_filename.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/alphanumeric/_alphanumeric.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/alphanumeric/_alphanumeric.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/alphanumeric/_character.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/alphanumeric/_character.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/alphanumeric/name/_label_name.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/alphanumeric/name/_label_name.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/alphanumeric/name/_name.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/alphanumeric/name/_name.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/alphanumeric/name/image_name/_external_image_name.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/alphanumeric/name/image_name/_external_image_name.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/number/_number.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/number/_number.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/setting/text/pathname/_pathname.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/setting/text/pathname/_pathname.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/analysis.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/analysis.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/channel_hasher.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/channel_hasher.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/core/module/identify.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/core/module/identify.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/core/modules/__init__.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/core/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/core/modules/load_data.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/core/modules/load_data.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/core/object.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/core/object.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/core/pipeline.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/core/plugins.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/core/plugins.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/grid.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/grid.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/hdf5_dict.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/hdf5_dict.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/image.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/image.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/java.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/java.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/legacy.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/legacy.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/measurement.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/measurement.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/pathname.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/pathname.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/utf16encode.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/utf16encode.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/zmq/__init__.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/zmq/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/zmq/_analysis_context.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/zmq/_analysis_context.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/zmq/_boundary.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/zmq/_boundary.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/zmq/communicable/_communicable.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/zmq/communicable/_communicable.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/zmq/communicable/request/_analysis_request.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/zmq/communicable/request/_analysis_request.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/utilities/zmq/communicable/request/_request.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/utilities/zmq/communicable/request/_request.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/worker/__init__.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/worker/_pipeline_event_listener.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/worker/_pipeline_event_listener.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/worker/_worker.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/worker/_worker.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core/workspace/_workspace.py` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core/workspace/_workspace.py`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core_nightly.egg-info/PKG-INFO` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core_nightly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellprofiler-core-nightly
-Version: 5.0.0.dev65
+Version: 5.0.0.dev69
 Summary: cellprofiler-core implements the bulk of CellProfiler's non-gui functionality
 Author: Anne Carpenter, Thouis (Ray) Jones, Lee Kamentsky, Vebjorn Ljosa, David Logan, Mark Bray, Madison Swain-Bowden, Allen Goodman, Claire McQuinn, Alice Lucas, Callum Tromans-Coia
 Author-email: Beth Cimini <bcimini@broadinstitute.org>, David Stirling <dstirling@glencoesoftware.com>, Nodar Gogoberidze <ngogober@broadinstitute.org>
 Maintainer-email: Beth Cimini <bcimini@broadinstitute.org>, Nodar Gogoberidze <ngogober@broadinstitute.org>
 License: The BSD 3-Clause License
         
         Copyright © 2003 - 2021 Broad Institute, Inc. All rights reserved.
@@ -94,8 +94,8 @@
 Requires-Dist: pytest~=7.4.1; extra == "test"
 Requires-Dist: pytest-timeout~=2.1.0; extra == "test"
 Provides-Extra: wx
 Requires-Dist: wxPython==4.2.0; extra == "wx"
 
 # core
 
-This subpackage contains the code to build the `cellprofiler-core` package. It contains the critical classes and components required by the [CellProfiler](cellprofiler.org) software, whereas the [frontend](../../frontend/) contains non-essential modules and the GUI interface. This package can be used in isolation, separate from the frontend, to access CellProfiler's functionality as a Python package, see [this page](https://github.com/CellProfiler/CellProfiler/wiki/CellProfiler-as-a-Python-package) for more details.
+This subpackage contains the code to build the `cellprofiler-core` package. It contains the critical classes and components required by the [CellProfiler](https://cellprofiler.org) software, whereas the [frontend](https://github.com/CellProfiler/CellProfiler/tree/main/src/frontend) contains non-essential modules and the GUI interface. This package can be used in isolation, separate from the frontend, to access CellProfiler's functionality as a Python package, see [this page](https://github.com/CellProfiler/CellProfiler/wiki/CellProfiler-as-a-Python-package) for more details.
```

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/cellprofiler_core_nightly.egg-info/SOURCES.txt` & `cellprofiler_core_nightly-5.0.0.dev69/cellprofiler_core_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellprofiler_core_nightly-5.0.0.dev65/pyproject.toml` & `cellprofiler_core_nightly-5.0.0.dev69/pyproject.toml`

 * *Files identical despite different names*


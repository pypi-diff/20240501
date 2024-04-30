# Comparing `tmp/straxen-2.2.1.tar.gz` & `tmp/straxen-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "straxen-2.2.1.tar", last modified: Wed Feb 21 14:47:24 2024, max compression
+gzip compressed data, was "straxen-2.2.2.tar", last modified: Tue Apr 30 23:26:07 2024, max compression
```

## Comparing `straxen-2.2.1.tar` & `straxen-2.2.2.tar`

### file list

```diff
@@ -1,252 +1,253 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.377797 straxen-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    48400 2024-02-21 14:47:21.000000 straxen-2.2.1/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-02-21 14:47:21.000000 straxen-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-21 14:47:21.000000 straxen-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    50816 2024-02-21 14:47:24.377797 straxen-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-02-21 14:47:21.000000 straxen-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.349797 straxen-2.2.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)    37105 2024-02-21 14:47:21.000000 straxen-2.2.1/bin/ajax
--rwxr-xr-x   0 runner    (1001) docker     (127)    67401 2024-02-21 14:47:21.000000 straxen-2.2.1/bin/bootstrax
--rwxr-xr-x   0 runner    (1001) docker     (127)     8446 2024-02-21 14:47:21.000000 straxen-2.2.1/bin/fake_daq
--rwxr-xr-x   0 runner    (1001) docker     (127)     6236 2024-02-21 14:47:21.000000 straxen-2.2.1/bin/microstrax
--rwxr-xr-x   0 runner    (1001) docker     (127)     5099 2024-02-21 14:47:21.000000 straxen-2.2.1/bin/refresh_raw_records
--rwxr-xr-x   0 runner    (1001) docker     (127)    36681 2024-02-21 14:47:21.000000 straxen-2.2.1/bin/restrax
--rwxr-xr-x   0 runner    (1001) docker     (127)      754 2024-02-21 14:47:21.000000 straxen-2.2.1/bin/straxen-print_versions
--rwxr-xr-x   0 runner    (1001) docker     (127)    12165 2024-02-21 14:47:21.000000 straxen-2.2.1/bin/straxer
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.349797 straxen-2.2.1/extra_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-21 14:47:21.000000 straxen-2.2.1/extra_requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-21 14:47:21.000000 straxen-2.2.1/extra_requirements/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-02-21 14:47:21.000000 straxen-2.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-02-21 14:47:24.377797 straxen-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-02-21 14:47:21.000000 straxen-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.349797 straxen-2.2.1/straxen/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.353797 straxen-2.2.1/straxen/analyses/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/analyses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34262 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/analyses/bokeh_waveform_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/analyses/daq_waveforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    16212 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/analyses/event_display.py
--rw-r--r--   0 runner    (1001) docker     (127)    15551 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/analyses/holoviews_waveform_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/analyses/posrec_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/analyses/pulse_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     8581 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/analyses/quick_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/analyses/records_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     9206 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/analyses/waveform_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/bokeh_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20941 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    13356 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/contexts.py
--rw-r--r--   0 runner    (1001) docker     (127)    18806 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/corrections_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/daq_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/get_corrections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.353797 straxen-2.2.1/straxen/holoviews/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/holoviews/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/holoviews/holoviews_inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)    12135 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/holoviews/holoviews_peak_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/holoviews/holoviews_pmt_array.py
--rw-r--r--   0 runner    (1001) docker     (127)    15310 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/holoviews/holoviews_tpc_event_display.py
--rw-r--r--   0 runner    (1001) docker     (127)    18651 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/holoviews_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14330 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/itp_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.353797 straxen-2.2.1/straxen/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/legacy/contexts_1t.py
--rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/legacy/hitfinder_thresholds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.353797 straxen-2.2.1/straxen/legacy/plugins_1t/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/legacy/plugins_1t/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/legacy/plugins_1t/event_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/legacy/plugins_1t/fake_daqreader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/legacy/plugins_1t/pax_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/legacy/plugins_1t/peak_positions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/legacy/plugins_1t/x1t_cuts.py
--rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/legacy/xenon1t_url_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6801 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/matplotlib_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/mini_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    12936 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/numbafied_scipy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.353797 straxen-2.2.1/straxen/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.353797 straxen-2.2.1/straxen/plugins/afterpulses/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/afterpulses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/afterpulses/afterpulse_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.357797 straxen-2.2.1/straxen/plugins/aqmon_hits/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/aqmon_hits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/aqmon_hits/aqmon_hits.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.357797 straxen-2.2.1/straxen/plugins/events/
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events/_event_s1_positions_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events/_event_s2_positions_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12104 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events/corrected_areas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events/distinct_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events/energy_estimates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events/event_ambience.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events/event_area_per_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)    16510 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events/event_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events/event_basics_som.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events/event_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events/event_info_double.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events/event_nearest_triggering.py
--rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events/event_pattern_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events/event_positions.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events/event_s1_positions_cnn.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events/event_s2_positions_cnn.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events/event_s2_positions_gcn.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events/event_s2_positions_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events/event_shadow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events/event_top_bottom_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events/event_w_bayes_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events/event_waveform.py
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events/local_minimum_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events/multi_scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events/s2_recon_pos_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events/veto_proximity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.361797 straxen-2.2.1/straxen/plugins/events_mv/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events_mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events_mv/events_mv.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events_mv/events_sync_mv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.361797 straxen-2.2.1/straxen/plugins/events_nv/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events_nv/event_positions_nv.py
--rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events_nv/events_nv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/events_nv/events_sync_nv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.361797 straxen-2.2.1/straxen/plugins/gps_syncing/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/gps_syncing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10950 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/gps_syncing/gps_syncing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.361797 straxen-2.2.1/straxen/plugins/hitlets_mv/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/hitlets_mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/hitlets_mv/hitlets_mv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.361797 straxen-2.2.1/straxen/plugins/hitlets_nv/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/hitlets_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/hitlets_nv/hitlets_nv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.361797 straxen-2.2.1/straxen/plugins/individual_peak_monitor/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/individual_peak_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/individual_peak_monitor/individual_peak_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.361797 straxen-2.2.1/straxen/plugins/led_cal/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/led_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8952 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/led_cal/led_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.361797 straxen-2.2.1/straxen/plugins/merged_s2s/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/merged_s2s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/merged_s2s/merged_s2s.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.361797 straxen-2.2.1/straxen/plugins/merged_s2s_he/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/merged_s2s_he/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/merged_s2s_he/merged_s2s_he.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.361797 straxen-2.2.1/straxen/plugins/online_monitor_mv/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/online_monitor_mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/online_monitor_mv/online_monitor_mv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.361797 straxen-2.2.1/straxen/plugins/online_monitor_nv/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/online_monitor_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/online_monitor_nv/online_monitor_nv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.361797 straxen-2.2.1/straxen/plugins/online_peak_monitor/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/online_peak_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/online_peak_monitor/online_peak_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.365797 straxen-2.2.1/straxen/plugins/peaklets/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaklets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaklets/peaklet_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaklets/peaklet_classification_som.py
--rw-r--r--   0 runner    (1001) docker     (127)    25791 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaklets/peaklets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.365797 straxen-2.2.1/straxen/plugins/peaklets_he/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaklets_he/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaklets_he/peaklet_classification_he.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaklets_he/peaklets_he.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.365797 straxen-2.2.1/straxen/plugins/peaks/
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaks/_peak_positions_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaks/_peak_s1_positions_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaks/peak_ambience.py
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaks/peak_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaks/peak_basics_som.py
--rw-r--r--   0 runner    (1001) docker     (127)     7898 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaks/peak_classification_bayes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaks/peak_corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaks/peak_nearest_triggering.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaks/peak_per_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaks/peak_positions.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaks/peak_positions_cnn.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaks/peak_positions_gcn.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaks/peak_positions_mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaks/peak_proximity.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaks/peak_s1_positions_cnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10392 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaks/peak_shadow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaks/peak_top_bottom_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaks/peaks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaks/peaks_som.py
--rw-r--r--   0 runner    (1001) docker     (127)    12877 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaks/peaks_subtyping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.369797 straxen-2.2.1/straxen/plugins/peaks_he/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaks_he/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaks_he/peak_basics_he.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/peaks_he/peaks_he.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.369797 straxen-2.2.1/straxen/plugins/raw_records/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/raw_records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16574 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/raw_records/daqreader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.369797 straxen-2.2.1/straxen/plugins/raw_records_coin_nv/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/raw_records_coin_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/raw_records_coin_nv/nveto_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.369797 straxen-2.2.1/straxen/plugins/records/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17520 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/records/records.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.369797 straxen-2.2.1/straxen/plugins/records_he/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/records_he/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/records_he/records_he.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.369797 straxen-2.2.1/straxen/plugins/records_mv/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/records_mv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/records_mv/records_mv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.369797 straxen-2.2.1/straxen/plugins/records_nv/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/records_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/records_nv/records_nv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.369797 straxen-2.2.1/straxen/plugins/ref_mon_nv/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/ref_mon_nv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/ref_mon_nv/ref_mon_nv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.369797 straxen-2.2.1/straxen/plugins/veto_intervals/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/veto_intervals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/plugins/veto_intervals/veto_intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)    26574 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/scada.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.369797 straxen-2.2.1/straxen/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14606 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/storage/mongo_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/storage/online_monitor_frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/storage/rucio_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/storage/rucio_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)    13295 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/storage/rundb.py
--rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/units.py
--rw-r--r--   0 runner    (1001) docker     (127)    26073 2024-02-21 14:47:21.000000 straxen-2.2.1/straxen/url_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.349797 straxen-2.2.1/straxen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    50816 2024-02-21 14:47:24.000000 straxen-2.2.1/straxen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-02-21 14:47:24.000000 straxen-2.2.1/straxen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 14:47:24.000000 straxen-2.2.1/straxen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 14:47:24.000000 straxen-2.2.1/straxen.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-02-21 14:47:24.000000 straxen-2.2.1/straxen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-21 14:47:24.000000 straxen-2.2.1/straxen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.373797 straxen-2.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:24.377797 straxen-2.2.1/tests/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9266 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/storage/test_database_frontends.py
--rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/storage/test_mongo_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/storage/test_mongo_interactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/storage/test_rucio_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/storage/test_rucio_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/test_1T_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/test_aqmon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/test_channel_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/test_cmt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/test_contexts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/test_count_pulses.py
--rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/test_daq_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/test_holoviews_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/test_itp_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/test_led_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14806 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/test_mini_analyses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/test_nveto_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/test_nveto_recorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/test_patternfit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/test_peaklet_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/test_peaks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/test_scada.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/test_testing_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)    15988 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/test_url_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-02-21 14:47:21.000000 straxen-2.2.1/tests/test_veto_hitlets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.269488 straxen-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    50745 2024-04-30 23:26:04.000000 straxen-2.2.2/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-30 23:26:04.000000 straxen-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-30 23:26:04.000000 straxen-2.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    53161 2024-04-30 23:26:07.269488 straxen-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-30 23:26:04.000000 straxen-2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.237488 straxen-2.2.2/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37105 2024-04-30 23:26:04.000000 straxen-2.2.2/bin/ajax
+-rwxr-xr-x   0 runner    (1001) docker     (127)    67403 2024-04-30 23:26:04.000000 straxen-2.2.2/bin/bootstrax
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8446 2024-04-30 23:26:04.000000 straxen-2.2.2/bin/fake_daq
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6236 2024-04-30 23:26:04.000000 straxen-2.2.2/bin/microstrax
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5099 2024-04-30 23:26:04.000000 straxen-2.2.2/bin/refresh_raw_records
+-rwxr-xr-x   0 runner    (1001) docker     (127)    36681 2024-04-30 23:26:04.000000 straxen-2.2.2/bin/restrax
+-rwxr-xr-x   0 runner    (1001) docker     (127)      754 2024-04-30 23:26:04.000000 straxen-2.2.2/bin/straxen-print_versions
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12167 2024-04-30 23:26:04.000000 straxen-2.2.2/bin/straxer
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.237488 straxen-2.2.2/extra_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-30 23:26:04.000000 straxen-2.2.2/extra_requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-30 23:26:04.000000 straxen-2.2.2/extra_requirements/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-30 23:26:04.000000 straxen-2.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-30 23:26:07.269488 straxen-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-30 23:26:04.000000 straxen-2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.241488 straxen-2.2.2/straxen/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.245488 straxen-2.2.2/straxen/analyses/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/analyses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34262 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/analyses/bokeh_waveform_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/analyses/daq_waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16212 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/analyses/event_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15551 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/analyses/holoviews_waveform_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/analyses/posrec_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/analyses/pulse_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8581 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/analyses/quick_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/analyses/records_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9178 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/analyses/waveform_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/bokeh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13095 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18806 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/corrections_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/daq_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/get_corrections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.245488 straxen-2.2.2/straxen/holoviews/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/holoviews/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/holoviews/holoviews_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12135 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/holoviews/holoviews_peak_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/holoviews/holoviews_pmt_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15310 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/holoviews/holoviews_tpc_event_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18651 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/holoviews_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14994 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/itp_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.245488 straxen-2.2.2/straxen/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/legacy/contexts_1t.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/legacy/hitfinder_thresholds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.245488 straxen-2.2.2/straxen/legacy/plugins_1t/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/legacy/plugins_1t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/legacy/plugins_1t/event_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/legacy/plugins_1t/fake_daqreader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6275 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/legacy/plugins_1t/pax_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/legacy/plugins_1t/peak_positions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10409 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/legacy/plugins_1t/x1t_cuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/legacy/xenon1t_url_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6801 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/matplotlib_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/mini_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17970 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/numbafied_scipy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.245488 straxen-2.2.2/straxen/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.245488 straxen-2.2.2/straxen/plugins/afterpulses/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/afterpulses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/afterpulses/afterpulse_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.245488 straxen-2.2.2/straxen/plugins/aqmon_hits/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/aqmon_hits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/aqmon_hits/aqmon_hits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.253488 straxen-2.2.2/straxen/plugins/events/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/_event_s1_positions_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/_event_s2_positions_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12324 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/corrected_areas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/distinct_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/energy_estimates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_ambience.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_area_per_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16510 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_basics_som.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_info_double.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_nearest_triggering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26370 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_pattern_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_positions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_s1_positions_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_s2_positions_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_s2_positions_gcn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_s2_positions_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_se_sensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_shadow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_top_bottom_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_w_bayes_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/event_waveform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/local_minimum_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/multi_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/s2_recon_pos_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events/veto_proximity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.253488 straxen-2.2.2/straxen/plugins/events_mv/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events_mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events_mv/events_mv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events_mv/events_sync_mv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.253488 straxen-2.2.2/straxen/plugins/events_nv/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events_nv/event_positions_nv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8230 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events_nv/events_nv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/events_nv/events_sync_nv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.253488 straxen-2.2.2/straxen/plugins/gps_syncing/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/gps_syncing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10950 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/gps_syncing/gps_syncing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.253488 straxen-2.2.2/straxen/plugins/hitlets_mv/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/hitlets_mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/hitlets_mv/hitlets_mv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.253488 straxen-2.2.2/straxen/plugins/hitlets_nv/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/hitlets_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/hitlets_nv/hitlets_nv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.253488 straxen-2.2.2/straxen/plugins/individual_peak_monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/individual_peak_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/individual_peak_monitor/individual_peak_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.253488 straxen-2.2.2/straxen/plugins/led_cal/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/led_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8952 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/led_cal/led_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.253488 straxen-2.2.2/straxen/plugins/merged_s2s/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/merged_s2s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/merged_s2s/merged_s2s.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.253488 straxen-2.2.2/straxen/plugins/merged_s2s_he/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/merged_s2s_he/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/merged_s2s_he/merged_s2s_he.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.253488 straxen-2.2.2/straxen/plugins/online_monitor_mv/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/online_monitor_mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/online_monitor_mv/online_monitor_mv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.257488 straxen-2.2.2/straxen/plugins/online_monitor_nv/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/online_monitor_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/online_monitor_nv/online_monitor_nv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.257488 straxen-2.2.2/straxen/plugins/online_peak_monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/online_peak_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/online_peak_monitor/online_peak_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.257488 straxen-2.2.2/straxen/plugins/peaklets/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaklets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaklets/peaklet_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11704 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaklets/peaklet_classification_som.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25952 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaklets/peaklets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.257488 straxen-2.2.2/straxen/plugins/peaklets_he/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaklets_he/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaklets_he/peaklet_classification_he.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaklets_he/peaklets_he.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.261488 straxen-2.2.2/straxen/plugins/peaks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/_peak_positions_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/_peak_s1_positions_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_ambience.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_basics_som.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7898 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_classification_bayes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_nearest_triggering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_per_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_positions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_positions_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_positions_gcn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_positions_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_proximity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_s1_positions_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_se_sensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10392 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_shadow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peak_top_bottom_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks/peaks_som.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.261488 straxen-2.2.2/straxen/plugins/peaks_he/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks_he/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks_he/peak_basics_he.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/peaks_he/peaks_he.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.261488 straxen-2.2.2/straxen/plugins/raw_records/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/raw_records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16574 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/raw_records/daqreader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.261488 straxen-2.2.2/straxen/plugins/raw_records_coin_nv/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/raw_records_coin_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/raw_records_coin_nv/nveto_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.261488 straxen-2.2.2/straxen/plugins/records/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17520 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/records/records.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.261488 straxen-2.2.2/straxen/plugins/records_he/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/records_he/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/records_he/records_he.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.261488 straxen-2.2.2/straxen/plugins/records_mv/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/records_mv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/records_mv/records_mv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.261488 straxen-2.2.2/straxen/plugins/records_nv/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/records_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/records_nv/records_nv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.261488 straxen-2.2.2/straxen/plugins/ref_mon_nv/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/ref_mon_nv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/ref_mon_nv/ref_mon_nv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.261488 straxen-2.2.2/straxen/plugins/veto_intervals/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/veto_intervals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/plugins/veto_intervals/veto_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26574 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/scada.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.265488 straxen-2.2.2/straxen/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14552 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/storage/mongo_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/storage/online_monitor_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/storage/rucio_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/storage/rucio_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13295 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/storage/rundb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26074 2024-04-30 23:26:04.000000 straxen-2.2.2/straxen/url_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.241488 straxen-2.2.2/straxen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    53161 2024-04-30 23:26:07.000000 straxen-2.2.2/straxen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-04-30 23:26:07.000000 straxen-2.2.2/straxen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 23:26:07.000000 straxen-2.2.2/straxen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 23:26:07.000000 straxen-2.2.2/straxen.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-30 23:26:07.000000 straxen-2.2.2/straxen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-30 23:26:07.000000 straxen-2.2.2/straxen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.269488 straxen-2.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:07.269488 straxen-2.2.2/tests/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9266 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/storage/test_database_frontends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/storage/test_mongo_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/storage/test_mongo_interactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/storage/test_rucio_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/storage/test_rucio_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_1T_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_aqmon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_channel_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_cmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_count_pulses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_daq_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_holoviews_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_itp_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_led_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14806 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_mini_analyses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_nveto_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_nveto_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_patternfit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_peaklet_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_scada.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_testing_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15988 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_url_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-30 23:26:04.000000 straxen-2.2.2/tests/test_veto_hitlets.py
```

### Comparing `straxen-2.2.1/HISTORY.md` & `straxen-2.2.2/HISTORY.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+2.2.2 / 2024-04-30
+-------------------
+* Minor change of indents by @dachengx in https://github.com/XENONnT/straxen/pull/1341
+* Remove unused `__all__` by @dachengx in https://github.com/XENONnT/straxen/pull/1342
+* Bump graphviz from 0.20.1 to 0.20.2 in /extra_requirements by @dependabot in https://github.com/XENONnT/straxen/pull/1345
+* Specifically install `lxml_html_clean` by @dachengx in https://github.com/XENONnT/straxen/pull/1352
+* Improve InterpolateAndExtrapolate performance for array valued maps by @l-althueser in https://github.com/XENONnT/straxen/pull/1347
+* Bump graphviz from 0.20.2 to 0.20.3 in /extra_requirements by @dependabot in https://github.com/XENONnT/straxen/pull/1350
+* Bump actions/setup-python from 5.0.0 to 5.1.0 by @dependabot in https://github.com/XENONnT/straxen/pull/1351
+* Add `storage_graph` to show the plugins stored or needed to be calculated in the dependency tree by @dachengx in https://github.com/XENONnT/straxen/pull/1353
+* Small bug fix of `storage_graph`, save plot into desired folder by @dachengx in https://github.com/XENONnT/straxen/pull/1356
+* Check non-positive lone_hits by @dachengx in https://github.com/XENONnT/straxen/pull/1358
+* Return the edge closer to the target in `_numeric_derivative` by @dachengx in https://github.com/XENONnT/straxen/pull/1355
+* Add a simply function to plot the dependency tree by @dachengx in https://github.com/XENONnT/straxen/pull/1363
+* Remove `PeakSubtyping` from straxen by @dachengx in https://github.com/XENONnT/straxen/pull/1365
+* Remove `xnt_simulation_config` by @dachengx in https://github.com/XENONnT/straxen/pull/1366
+* Tolerate more exceptions when can not import admix by @dachengx in https://github.com/XENONnT/straxen/pull/1367
+* Add `PeakSEDensity` and `EventSEDensity` by @dachengx in https://github.com/XENONnT/straxen/pull/1368
+* Update `se_time_search_window_left` by @dachengx in https://github.com/XENONnT/straxen/pull/1370
+* remove resource_cache from dali by @yuema137 in https://github.com/XENONnT/straxen/pull/1372
+* Add `exclude_pattern` argument to `dependency_tree` by @dachengx in https://github.com/XENONnT/straxen/pull/1373
+* Let xedocs to handle avg seg and seg partitioning by @GiovanniVolta in https://github.com/XENONnT/straxen/pull/1371
+
+**Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.2.1...v2.2.2
+
+
 2.2.1 / 2024-02-21
 -------------------
 * Loosen `save_when` of `Events` by @dachengx in https://github.com/XENONnT/straxen/pull/1327
 * Deprecate the usage of `XENONnT/ax_env` by @dachengx in https://github.com/XENONnT/straxen/pull/1329
 * `_text_formats` should include txt but not text by @dachengx in https://github.com/XENONnT/straxen/pull/1324
 * Fix numerical comparison error of `test_patternfit_stats` by @dachengx in https://github.com/XENONnT/straxen/pull/1334
 * Remove some packages requirements from `requirements-tests.txt` by @dachengx in https://github.com/XENONnT/straxen/pull/1337
```

### Comparing `straxen-2.2.1/LICENSE` & `straxen-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/PKG-INFO` & `straxen-2.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: straxen
-Version: 2.2.1
+Version: 2.2.2
 Summary: Streaming analysis for XENON
 Home-page: https://github.com/XENONnT/straxen
 Author: Straxen contributors, the XENON collaboration
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
@@ -37,14 +37,40 @@
 
 
 ## Further status
 [![Python Versions](https://img.shields.io/pypi/pyversions/straxen.svg)](https://pypi.python.org/pypi/straxen)
 [![PyPI downloads](https://img.shields.io/pypi/dm/straxen.svg)](https://pypistats.org/packages/straxen)
 
 
+2.2.2 / 2024-04-30
+-------------------
+* Minor change of indents by @dachengx in https://github.com/XENONnT/straxen/pull/1341
+* Remove unused `__all__` by @dachengx in https://github.com/XENONnT/straxen/pull/1342
+* Bump graphviz from 0.20.1 to 0.20.2 in /extra_requirements by @dependabot in https://github.com/XENONnT/straxen/pull/1345
+* Specifically install `lxml_html_clean` by @dachengx in https://github.com/XENONnT/straxen/pull/1352
+* Improve InterpolateAndExtrapolate performance for array valued maps by @l-althueser in https://github.com/XENONnT/straxen/pull/1347
+* Bump graphviz from 0.20.2 to 0.20.3 in /extra_requirements by @dependabot in https://github.com/XENONnT/straxen/pull/1350
+* Bump actions/setup-python from 5.0.0 to 5.1.0 by @dependabot in https://github.com/XENONnT/straxen/pull/1351
+* Add `storage_graph` to show the plugins stored or needed to be calculated in the dependency tree by @dachengx in https://github.com/XENONnT/straxen/pull/1353
+* Small bug fix of `storage_graph`, save plot into desired folder by @dachengx in https://github.com/XENONnT/straxen/pull/1356
+* Check non-positive lone_hits by @dachengx in https://github.com/XENONnT/straxen/pull/1358
+* Return the edge closer to the target in `_numeric_derivative` by @dachengx in https://github.com/XENONnT/straxen/pull/1355
+* Add a simply function to plot the dependency tree by @dachengx in https://github.com/XENONnT/straxen/pull/1363
+* Remove `PeakSubtyping` from straxen by @dachengx in https://github.com/XENONnT/straxen/pull/1365
+* Remove `xnt_simulation_config` by @dachengx in https://github.com/XENONnT/straxen/pull/1366
+* Tolerate more exceptions when can not import admix by @dachengx in https://github.com/XENONnT/straxen/pull/1367
+* Add `PeakSEDensity` and `EventSEDensity` by @dachengx in https://github.com/XENONnT/straxen/pull/1368
+* Update `se_time_search_window_left` by @dachengx in https://github.com/XENONnT/straxen/pull/1370
+* remove resource_cache from dali by @yuema137 in https://github.com/XENONnT/straxen/pull/1372
+* Add `exclude_pattern` argument to `dependency_tree` by @dachengx in https://github.com/XENONnT/straxen/pull/1373
+* Let xedocs to handle avg seg and seg partitioning by @GiovanniVolta in https://github.com/XENONnT/straxen/pull/1371
+
+**Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.2.1...v2.2.2
+
+
 2.2.1 / 2024-02-21
 -------------------
 * Loosen `save_when` of `Events` by @dachengx in https://github.com/XENONnT/straxen/pull/1327
 * Deprecate the usage of `XENONnT/ax_env` by @dachengx in https://github.com/XENONnT/straxen/pull/1329
 * `_text_formats` should include txt but not text by @dachengx in https://github.com/XENONnT/straxen/pull/1324
 * Fix numerical comparison error of `test_patternfit_stats` by @dachengx in https://github.com/XENONnT/straxen/pull/1334
 * Remove some packages requirements from `requirements-tests.txt` by @dachengx in https://github.com/XENONnT/straxen/pull/1337
```

### Comparing `straxen-2.2.1/README.md` & `straxen-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/bin/ajax` & `straxen-2.2.2/bin/ajax`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/bin/bootstrax` & `straxen-2.2.2/bin/bootstrax`

 * *Files 0% similar despite different names*

```diff
@@ -816,15 +816,15 @@
             )
             data_rate = float(sum([d["rate"] for d in docs]))
             if data_rate > 0:
                 break
             elif time.time() - started_looking > timeouts["max_data_rate_infer_time"]:
                 raise RuntimeError(f'Could not infer_mode for {rd["number"]}')
             log.debug(
-                f'No rate inferred for {rd["number"]} after {time.time()-started_looking:.1f} s.'
+                f'No rate inferred for {rd["number"]} after {time.time() - started_looking:.1f} s.'
             )
             time.sleep(2)
 
     except Exception as e:
         log_warning(
             f"infer_mode ran into {e}. Cannot infer datarate, using default mode.",
             run_id=f'{rd["number"]:06}',
```

### Comparing `straxen-2.2.1/bin/fake_daq` & `straxen-2.2.2/bin/fake_daq`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/bin/microstrax` & `straxen-2.2.2/bin/microstrax`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/bin/refresh_raw_records` & `straxen-2.2.2/bin/refresh_raw_records`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/bin/restrax` & `straxen-2.2.2/bin/restrax`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/bin/straxen-print_versions` & `straxen-2.2.2/bin/straxen-print_versions`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/bin/straxer` & `straxen-2.2.2/bin/straxer`

 * *Files 0% similar despite different names*

```diff
@@ -297,15 +297,15 @@
     proc_start = time.time()
     if args.multi_target:
         run_make(args.target)
     else:
         for target in strax.to_str_tuple(args.target):
             run_make(target)
     logging.info(
-        f"Straxer is done in {time.time()-proc_start :.1f} s! peak RAM usage was"
+        f"Straxer is done in {time.time() - proc_start :.1f} s! peak RAM usage was"
         f" ~{peak_ram:.1f} MB."
     )
 
 
 def register_to_context(st, module: str):
     if not os.path.exists(module):
         raise FileNotFoundError(f"No such file {module}")
```

### Comparing `straxen-2.2.1/setup.py` & `straxen-2.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     readme = file.read()
 
 with open("HISTORY.md") as file:
     history = file.read()
 
 setuptools.setup(
     name="straxen",
-    version="2.2.1",
+    version="2.2.2",
     description="Streaming analysis for XENON",
     author="Straxen contributors, the XENON collaboration",
     url="https://github.com/XENONnT/straxen",
     long_description=readme + "\n\n" + history,
     long_description_content_type="text/markdown",
     setup_requires=["pytest-runner"],
     install_requires=requires,
```

### Comparing `straxen-2.2.1/straxen/__init__.py` & `straxen-2.2.2/straxen/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # mypy: disable-error-code="no-redef"
-__version__ = "2.2.1"
+__version__ = "2.2.2"
 
 from utilix import uconfig
 from .common import *
 
 # contexts.py below
 from .corrections_services import *
 from .get_corrections import *
```

### Comparing `straxen-2.2.1/straxen/analyses/bokeh_waveform_plot.py` & `straxen-2.2.2/straxen/analyses/bokeh_waveform_plot.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/analyses/daq_waveforms.py` & `straxen-2.2.2/straxen/analyses/daq_waveforms.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/analyses/event_display.py` & `straxen-2.2.2/straxen/analyses/event_display.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/analyses/holoviews_waveform_display.py` & `straxen-2.2.2/straxen/analyses/holoviews_waveform_display.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/analyses/posrec_comparison.py` & `straxen-2.2.2/straxen/analyses/posrec_comparison.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/analyses/pulse_plots.py` & `straxen-2.2.2/straxen/analyses/pulse_plots.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/analyses/quick_checks.py` & `straxen-2.2.2/straxen/analyses/quick_checks.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/analyses/records_matrix.py` & `straxen-2.2.2/straxen/analyses/records_matrix.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/analyses/waveform_plot.py` & `straxen-2.2.2/straxen/analyses/waveform_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import straxen
 from mpl_toolkits.axes_grid1 import inset_locator
 
 from .daq_waveforms import group_by_daq
 from .records_matrix import DEFAULT_MAX_SAMPLES
 
 export, __all__ = strax.exporter()
-__all__.extend(["plot_wf"])
 
 
 @straxen.mini_analysis()
 def plot_waveform(
     context,
     deep=False,
     show_largest=100,
```

### Comparing `straxen-2.2.1/straxen/bokeh_utils.py` & `straxen-2.2.2/straxen/bokeh_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/common.py` & `straxen-2.2.2/straxen/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,15 +257,14 @@
 
     # Web resource; look first in on-disk cache
     # to prevent repeated downloads.
     cache_fn = strax.utils.deterministic_hash(html)
     cache_folders = [
         "./resource_cache",
         "/tmp/straxen_resource_cache",
-        "/dali/lgrandi/strax/resource_cache",
     ]
     for cache_folder in cache_folders:
         try:
             os.makedirs(cache_folder, exist_ok=True)
         except (PermissionError, OSError):
             continue
         cf = osp.join(cache_folder, cache_fn)
```

### Comparing `straxen-2.2.1/straxen/contexts.py` & `straxen-2.2.2/straxen/contexts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 import warnings
-from copy import deepcopy
 from typing import Dict, Any, List, Optional
 from immutabledict import immutabledict
 import socket
 
 from pandas.util._decorators import deprecate_kwarg
 import strax
 import straxen
@@ -73,22 +72,15 @@
         "resource://"
         "XnT_z_bias_map_chargeup_20230329.json.gz?"
         "fmt=json.gz"
         "&method=RegularGridInterpolator"
     ),
 )
 # these are placeholders to avoid calling cmt with non integer run_ids. Better solution pending.
-# s1,s2 and fd corrections are still problematic
-xnt_simulation_config = deepcopy(xnt_common_config)
-xnt_simulation_config.update(
-    gain_model="legacy-to-pe://to_pe_placeholder",
-    gain_model_nv="legacy-to-pe://adc_nv",
-    gain_model_mv="legacy-to-pe://adc_mv",
-    elife=1e6,
-)
+# s1, s2 and fd corrections are still problematic
 
 # Plugins in these files have nT plugins, E.g. in pulse&peak(let)
 # processing there are plugins for High Energy plugins. Therefore, do not
 # st.register_all in 1T contexts.
 xnt_common_opts = common_opts.copy()
 xnt_common_opts.update(
     {
```

### Comparing `straxen-2.2.1/straxen/corrections_services.py` & `straxen-2.2.2/straxen/corrections_services.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/daq_core.py` & `straxen-2.2.2/straxen/daq_core.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/entry_points.py` & `straxen-2.2.2/straxen/entry_points.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/get_corrections.py` & `straxen-2.2.2/straxen/get_corrections.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/holoviews/holoviews_inspector.py` & `straxen-2.2.2/straxen/holoviews/holoviews_inspector.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/holoviews/holoviews_peak_data.py` & `straxen-2.2.2/straxen/holoviews/holoviews_peak_data.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/holoviews/holoviews_pmt_array.py` & `straxen-2.2.2/straxen/holoviews/holoviews_pmt_array.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/holoviews/holoviews_tpc_event_display.py` & `straxen-2.2.2/straxen/holoviews/holoviews_tpc_event_display.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/holoviews_utils.py` & `straxen-2.2.2/straxen/holoviews_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/itp_map.py` & `straxen-2.2.2/straxen/itp_map.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,44 +26,61 @@
 
     def __init__(self, points, values, neighbours_to_use=None, array_valued=False):
         """
         :param points: array (n_points, n_dims) of coordinates
         :param values: array (n_points) of values
         :param neighbours_to_use: Number of neighbouring points to use for
         averaging. Default is 2 * dimensions of points.
+        :param array_valued: bool, if true, the results are array-valued, if false they are scalar
         """
         self.kdtree = cKDTree(points)
         self.values = values
         if neighbours_to_use is None:
             neighbours_to_use = points.shape[1] * 2
         self.neighbours_to_use = neighbours_to_use
         self.array_valued = array_valued
         if array_valued:
             self.n_dim = self.values.shape[-1]
 
     def __call__(self, points):
         points = np.asarray(points)
 
-        # kdtree doesn't grok NaNs
-        # Start with all Nans, then overwrite for the finite points
-        result = np.ones(len(points)) * float("nan")
+        # Prepare result array in order to fill with valid values and masked nan
         if self.array_valued:
-            result = np.repeat(result.reshape(-1, 1), self.n_dim, axis=1)
+            result = np.empty((len(points), self.n_dim))
+        else:
+            result = np.empty(len(points))
+
+        # kdtree doesn't grok NaNs, mask valid values
         valid = np.all(np.isfinite(points), axis=-1)
 
+        # fill non valid values with nan and compute the others
+        # fill method slightly faster than multiplication of np.ones with nan
+        result[~valid] = float("nan")
+
         # Get distances to neighbours_to_use nearest neighbours
         distances, indices = self.kdtree.query(points[valid], self.neighbours_to_use)
 
         # Get values and weights for inverse distance weighted interpolation
         values = self.values[indices]
         weights = 1 / np.clip(distances, 1e-6, float("inf"))
-        if self.array_valued:
-            weights = np.repeat(weights, self.n_dim).reshape(values.shape)
 
-        result[valid] = np.average(values, weights=weights, axis=-2 if self.array_valued else -1)
+        # Faster shortcut for large S1/S2 maps, avoids caching by direct summation
+        if (values.ndim == 3) and (self.array_valued):
+            result[valid] = np.einsum(
+                "ijk, ij->ik", values, weights / weights.sum(axis=-1)[:, np.newaxis]
+            )
+        # Default map handling
+        else:
+            if self.array_valued:
+                weights = np.repeat(weights, self.n_dim).reshape(values.shape)
+            result[valid] = np.average(
+                values, weights=weights, axis=-2 if self.array_valued else -1
+            )
+
         return result
 
 
 @export
 class InterpolatingMap:
     """Correction map that computes values using inverse-weighted distance interpolation.
```

### Comparing `straxen-2.2.1/straxen/legacy/contexts_1t.py` & `straxen-2.2.2/straxen/legacy/contexts_1t.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/legacy/hitfinder_thresholds.py` & `straxen-2.2.2/straxen/legacy/hitfinder_thresholds.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/legacy/plugins_1t/pax_interface.py` & `straxen-2.2.2/straxen/legacy/plugins_1t/pax_interface.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/legacy/plugins_1t/peak_positions.py` & `straxen-2.2.2/straxen/legacy/plugins_1t/peak_positions.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/legacy/plugins_1t/x1t_cuts.py` & `straxen-2.2.2/straxen/legacy/plugins_1t/x1t_cuts.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/legacy/xenon1t_url_configs.py` & `straxen-2.2.2/straxen/legacy/xenon1t_url_configs.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/matplotlib_utils.py` & `straxen-2.2.2/straxen/matplotlib_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/mini_analysis.py` & `straxen-2.2.2/straxen/mini_analysis.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/numbafied_scipy.py` & `straxen-2.2.2/straxen/numbafied_scipy.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/__init__.py` & `straxen-2.2.2/straxen/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/afterpulses/afterpulse_processing.py` & `straxen-2.2.2/straxen/plugins/afterpulses/afterpulse_processing.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/aqmon_hits/aqmon_hits.py` & `straxen-2.2.2/straxen/plugins/aqmon_hits/aqmon_hits.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/defaults.py` & `straxen-2.2.2/straxen/plugins/defaults.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events/__init__.py` & `straxen-2.2.2/straxen/plugins/events/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,7 +68,10 @@
 from .multi_scatter import *
 
 from . import event_basics_som
 from .event_basics_som import *
 
 from . import event_nearest_triggering
 from .event_nearest_triggering import *
+
+from . import event_se_sensity
+from .event_se_sensity import *
```

### Comparing `straxen-2.2.1/straxen/plugins/events/_event_s1_positions_base.py` & `straxen-2.2.2/straxen/plugins/events/_event_s1_positions_base.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events/_event_s2_positions_base.py` & `straxen-2.2.2/straxen/plugins/events/_event_s2_positions_base.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events/corrected_areas.py` & `straxen-2.2.2/straxen/plugins/events/corrected_areas.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         area is corrected according to the xy-position of the main S2.
         There are now 3 components of cS2s: cs2_top, cS2_bottom and cs2.
         cs2_top and cs2_bottom are corrected by the corresponding maps,
         and cs2 is the sum of the two.
 
     """
 
-    __version__ = "0.5.2"
+    __version__ = "0.5.3"
 
     depends_on: Tuple[str, ...] = ("event_basics", "event_positions")
 
     # Descriptor configs
     elife = straxen.URLConfig(
         default="cmt://elife?version=ONLINE&run_id=plugin.run_id", help="electron lifetime in [ns]"
     )
@@ -78,27 +78,25 @@
     # relative light yield
     # defaults to no correction
     rel_light_yield = straxen.URLConfig(
         default="cmt://relative_light_yield?version=ONLINE&run_id=plugin.run_id",
         help="Relative light yield (allows for time dependence)",
     )
 
-    region_linear = straxen.URLConfig(
-        default=28,
+    # Single electron gain partition
+    # AB and CD partitons distiguished based on
+    # linear and circular regions
+    # SR0 values set as default
+    # https://xe1t-wiki.lngs.infn.it/doku.php?id=jlong:sr0_2_region_se_correction
+    # https://xe1t-wiki.lngs.infn.it/doku.php?id=xenon:xenonnt:noahhood:corrections:se_gain_ee_final
+    single_electron_gain_partition = straxen.URLConfig(
+        default={"linear": 28, "circular": 60},
         help=(
-            "linear cut (cm) for ab region, check out the note"
-            " https://xe1t-wiki.lngs.infn.it/doku.php?id=jlong:sr0_2_region_se_correction"
-        ),
-    )
-
-    region_circular = straxen.URLConfig(
-        default=60,
-        help=(
-            "circular cut (cm) for ab region, check out the note"
-            " https://xe1t-wiki.lngs.infn.it/doku.php?id=jlong:sr0_2_region_se_correction"
+            "Two distinct patterns of evolution of single electron corrections between AB and CD. "
+            "Distinguish thanks to linear and circular regions"
         ),
     )
 
     # cS2 AFT correction due to photon ionization
     # https://xe1t-wiki.lngs.infn.it/doku.php?id=xenon:xenonnt:zihao:sr1_s2aft_photonionization_correction
     cs2_bottom_top_ratio_correction = straxen.URLConfig(
         default=1, help="Scaling factor for cS2 AFT correction due to photon ionization"
@@ -147,17 +145,17 @@
                         ),
                     ),
                 ]
         return dtype
 
     def ab_region(self, x, y):
         new_x, new_y = rotate_perp_wires(x, y)
-        cond = new_x < self.region_linear
-        cond &= new_x > -self.region_linear
-        cond &= new_x**2 + new_y**2 < self.region_circular**2
+        cond = new_x < self.single_electron_gain_partition["linear"]
+        cond &= new_x > -self.single_electron_gain_partition["linear"]
+        cond &= new_x**2 + new_y**2 < self.single_electron_gain_partition["circular"] ** 2
         return cond
 
     def cd_region(self, x, y):
         return ~self.ab_region(x, y)
 
     def s2_map_names(self):
         # S2 top and bottom are corrected separately, and cS2 total is the sum of the two
```

### Comparing `straxen-2.2.1/straxen/plugins/events/distinct_channels.py` & `straxen-2.2.2/straxen/plugins/events/distinct_channels.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events/energy_estimates.py` & `straxen-2.2.2/straxen/plugins/events/energy_estimates.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events/event_ambience.py` & `straxen-2.2.2/straxen/plugins/events/event_ambience.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events/event_area_per_channel.py` & `straxen-2.2.2/straxen/plugins/events/event_area_per_channel.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events/event_basics.py` & `straxen-2.2.2/straxen/plugins/events/event_basics.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events/event_basics_som.py` & `straxen-2.2.2/straxen/plugins/events/event_basics_som.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events/event_info.py` & `straxen-2.2.2/straxen/plugins/events/event_info.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events/event_info_double.py` & `straxen-2.2.2/straxen/plugins/events/event_info_double.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events/event_nearest_triggering.py` & `straxen-2.2.2/straxen/plugins/events/event_nearest_triggering.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events/event_pattern_fit.py` & `straxen-2.2.2/straxen/plugins/events/event_pattern_fit.py`

 * *Files 1% similar despite different names*

```diff
@@ -565,15 +565,19 @@
 
 
 @numba.njit(cache=True)
 def _numeric_derivative(y0, y1, err, target, x_min, x_max, x0, x1):
     """Get close to <target> by doing a numeric derivative."""
     if abs(y1 - y0) < err:
         # break by passing dx == 0
-        return 0.0, x1, x1
+        if abs(y0 - target) < abs(y1 - target):
+            x = x0
+        else:
+            x = x1
+        return 0.0, x, x
 
     x = (target - y0) / (y1 - y0) * (x1 - x0) + x0
     x = min(x, x_max)
     x = max(x, x_min)
 
     dx = abs(x - x1)
     x0 = x1
```

### Comparing `straxen-2.2.1/straxen/plugins/events/event_positions.py` & `straxen-2.2.2/straxen/plugins/events/event_positions.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events/event_s1_positions_cnn.py` & `straxen-2.2.2/straxen/plugins/events/event_s1_positions_cnn.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events/event_s2_positions_cnn.py` & `straxen-2.2.2/straxen/plugins/events/event_s2_positions_cnn.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events/event_s2_positions_gcn.py` & `straxen-2.2.2/straxen/plugins/events/event_s2_positions_gcn.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events/event_s2_positions_mlp.py` & `straxen-2.2.2/straxen/plugins/events/event_s2_positions_mlp.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events/event_shadow.py` & `straxen-2.2.2/straxen/plugins/events/event_shadow.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events/event_top_bottom_params.py` & `straxen-2.2.2/straxen/plugins/events/event_top_bottom_params.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events/event_w_bayes_class.py` & `straxen-2.2.2/straxen/plugins/events/event_w_bayes_class.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events/event_waveform.py` & `straxen-2.2.2/straxen/plugins/events/event_waveform.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events/events.py` & `straxen-2.2.2/straxen/plugins/events/events.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events/local_minimum_info.py` & `straxen-2.2.2/straxen/plugins/events/local_minimum_info.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events/multi_scatter.py` & `straxen-2.2.2/straxen/plugins/events/multi_scatter.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events/s2_recon_pos_diff.py` & `straxen-2.2.2/straxen/plugins/events/s2_recon_pos_diff.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events/veto_proximity.py` & `straxen-2.2.2/straxen/plugins/events/veto_proximity.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events_mv/events_mv.py` & `straxen-2.2.2/straxen/plugins/events_mv/events_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events_mv/events_sync_mv.py` & `straxen-2.2.2/straxen/plugins/events_mv/events_sync_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events_nv/event_positions_nv.py` & `straxen-2.2.2/straxen/plugins/events_nv/event_positions_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events_nv/events_nv.py` & `straxen-2.2.2/straxen/plugins/events_nv/events_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/events_nv/events_sync_nv.py` & `straxen-2.2.2/straxen/plugins/events_nv/events_sync_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/gps_syncing/gps_syncing.py` & `straxen-2.2.2/straxen/plugins/gps_syncing/gps_syncing.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/hitlets_mv/hitlets_mv.py` & `straxen-2.2.2/straxen/plugins/hitlets_mv/hitlets_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/hitlets_nv/hitlets_nv.py` & `straxen-2.2.2/straxen/plugins/hitlets_nv/hitlets_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/individual_peak_monitor/individual_peak_monitor.py` & `straxen-2.2.2/straxen/plugins/individual_peak_monitor/individual_peak_monitor.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/led_cal/led_calibration.py` & `straxen-2.2.2/straxen/plugins/led_cal/led_calibration.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/merged_s2s/merged_s2s.py` & `straxen-2.2.2/straxen/plugins/merged_s2s/merged_s2s.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/merged_s2s_he/merged_s2s_he.py` & `straxen-2.2.2/straxen/plugins/merged_s2s_he/merged_s2s_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/online_monitor_mv/online_monitor_mv.py` & `straxen-2.2.2/straxen/plugins/online_monitor_mv/online_monitor_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/online_monitor_nv/online_monitor_nv.py` & `straxen-2.2.2/straxen/plugins/online_monitor_nv/online_monitor_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/online_peak_monitor/online_peak_monitor.py` & `straxen-2.2.2/straxen/plugins/online_peak_monitor/online_peak_monitor.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/peaklets/peaklet_classification.py` & `straxen-2.2.2/straxen/plugins/peaklets/peaklet_classification.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/peaklets/peaklet_classification_som.py` & `straxen-2.2.2/straxen/plugins/peaklets/peaklet_classification_som.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/peaklets/peaklets.py` & `straxen-2.2.2/straxen/plugins/peaklets/peaklets.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,14 +222,16 @@
         strax.integrate_lone_hits(
             lone_hits,
             records,
             peaklets,
             save_outside_hits=(self.peak_left_extension, self.peak_right_extension),
             n_channels=len(self.to_pe),
         )
+        if np.any(lone_hits["right_integration"] - lone_hits["left_integration"] <= 0):
+            raise ValueError("Find lone_hits with non-positive length!")
 
         # Compute basic peak properties -- needed before natural breaks
         hits = hits[~is_lone_hit]
         # Define regions outside of peaks such that _find_hit_integration_bounds
         # is not extended beyond a peak.
         outside_peaks = self.create_outside_peaks_region(peaklets, start, end)
         strax.find_hit_integration_bounds(
```

### Comparing `straxen-2.2.1/straxen/plugins/peaklets_he/peaklet_classification_he.py` & `straxen-2.2.2/straxen/plugins/peaklets_he/peaklet_classification_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/peaklets_he/peaklets_he.py` & `straxen-2.2.2/straxen/plugins/peaklets_he/peaklets_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/peaks/__init__.py` & `straxen-2.2.2/straxen/plugins/peaks/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,18 +36,18 @@
 
 from . import peak_per_event
 from .peak_per_event import *
 
 from . import peak_corrections
 from .peak_corrections import *
 
-from . import peaks_subtyping
-from .peaks_subtyping import *
-
 from . import peaks_som
 from .peaks_som import *
 
 from . import peak_basics_som
 from .peak_basics_som import *
 
 from . import peak_nearest_triggering
 from .peak_nearest_triggering import *
+
+from . import peak_se_sensity
+from .peak_se_sensity import *
```

### Comparing `straxen-2.2.1/straxen/plugins/peaks/_peak_positions_base.py` & `straxen-2.2.2/straxen/plugins/peaks/_peak_positions_base.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/peaks/_peak_s1_positions_base.py` & `straxen-2.2.2/straxen/plugins/peaks/_peak_s1_positions_base.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/peaks/peak_ambience.py` & `straxen-2.2.2/straxen/plugins/peaks/peak_ambience.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/peaks/peak_basics.py` & `straxen-2.2.2/straxen/plugins/peaks/peak_basics.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/peaks/peak_basics_som.py` & `straxen-2.2.2/straxen/plugins/peaks/peak_basics_som.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/peaks/peak_classification_bayes.py` & `straxen-2.2.2/straxen/plugins/peaks/peak_classification_bayes.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/peaks/peak_corrections.py` & `straxen-2.2.2/straxen/plugins/peaks/peak_corrections.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/peaks/peak_nearest_triggering.py` & `straxen-2.2.2/straxen/plugins/peaks/peak_nearest_triggering.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/peaks/peak_per_event.py` & `straxen-2.2.2/straxen/plugins/peaks/peak_per_event.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/peaks/peak_positions.py` & `straxen-2.2.2/straxen/plugins/peaks/peak_positions.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/peaks/peak_positions_cnn.py` & `straxen-2.2.2/straxen/plugins/peaks/peak_positions_cnn.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/peaks/peak_positions_gcn.py` & `straxen-2.2.2/straxen/plugins/peaks/peak_positions_gcn.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/peaks/peak_positions_mlp.py` & `straxen-2.2.2/straxen/plugins/peaks/peak_positions_mlp.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/peaks/peak_proximity.py` & `straxen-2.2.2/straxen/plugins/peaks/peak_proximity.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/peaks/peak_s1_positions_cnn.py` & `straxen-2.2.2/straxen/plugins/peaks/peak_s1_positions_cnn.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/peaks/peak_shadow.py` & `straxen-2.2.2/straxen/plugins/peaks/peak_shadow.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/peaks/peak_top_bottom_params.py` & `straxen-2.2.2/straxen/plugins/peaks/peak_top_bottom_params.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/peaks/peaks.py` & `straxen-2.2.2/straxen/plugins/peaks/peaks.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/peaks/peaks_som.py` & `straxen-2.2.2/straxen/plugins/peaks/peaks_som.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/peaks_he/peaks_he.py` & `straxen-2.2.2/straxen/plugins/peaks_he/peaks_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/raw_records/daqreader.py` & `straxen-2.2.2/straxen/plugins/raw_records/daqreader.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/raw_records_coin_nv/nveto_recorder.py` & `straxen-2.2.2/straxen/plugins/raw_records_coin_nv/nveto_recorder.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/records/records.py` & `straxen-2.2.2/straxen/plugins/records/records.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/records_he/records_he.py` & `straxen-2.2.2/straxen/plugins/records_he/records_he.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/records_mv/records_mv.py` & `straxen-2.2.2/straxen/plugins/records_mv/records_mv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/records_nv/records_nv.py` & `straxen-2.2.2/straxen/plugins/records_nv/records_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/ref_mon_nv/ref_mon_nv.py` & `straxen-2.2.2/straxen/plugins/ref_mon_nv/ref_mon_nv.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/plugins/veto_intervals/veto_intervals.py` & `straxen-2.2.2/straxen/plugins/veto_intervals/veto_intervals.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/scada.py` & `straxen-2.2.2/straxen/scada.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/storage/mongo_storage.py` & `straxen-2.2.2/straxen/storage/mongo_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,15 +257,14 @@
         super().__init__(*args, **kwargs)
 
         # We are going to set a place where to store the files. It's
         # either specified by the user or we use these defaults:
         if store_files_at is None:
             store_files_at = (
                 "/tmp/straxen_resource_cache/",
-                "/dali/lgrandi/strax/resource_cache",
                 "./resource_cache",
             )
         elif not isinstance(store_files_at, (tuple, str, list)):
             raise ValueError(f"{store_files_at} should be tuple of paths!")
         elif isinstance(store_files_at, str):
             store_files_at = to_str_tuple(store_files_at)
```

### Comparing `straxen-2.2.1/straxen/storage/online_monitor_frontend.py` & `straxen-2.2.2/straxen/storage/online_monitor_frontend.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/storage/rucio_local.py` & `straxen-2.2.2/straxen/storage/rucio_local.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/storage/rucio_remote.py` & `straxen-2.2.2/straxen/storage/rucio_remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from utilix import xent_collection
 
 try:
     import admix
     from rucio.common.exception import DataIdentifierNotFound
 
     HAVE_ADMIX = True
-except ImportError:
+except (ImportError, AttributeError):
     HAVE_ADMIX = False
 
 export, __all__ = strax.exporter()
 
 __all__.extend(["HAVE_ADMIX"])
```

### Comparing `straxen-2.2.1/straxen/storage/rundb.py` & `straxen-2.2.2/straxen/storage/rundb.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/test_utils.py` & `straxen-2.2.2/straxen/test_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/units.py` & `straxen-2.2.2/straxen/units.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/straxen/url_config.py` & `straxen-2.2.2/straxen/url_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -738,15 +738,15 @@
 
     global WARN
 
     if isinstance(url, str) and URLConfig.SCHEME_SEP in url:
         if url != URLConfig.format_url_kwargs(url) and WARN:
             warnings.warn(
                 "From straxen version 2.1.0 onward, URLConfig parameters"
-                "will be sorted alphabetically before being passed to the plugins,"
+                " will be sorted alphabetically before being passed to the plugins,"
                 " this will change the lineage hash for non-sorted URLs. To load"
                 " data processed with non-sorted URLs, you will need to use an"
                 " older version."
             )
             WARN = False
         return URLConfig.format_url_kwargs(url)
     return url
```

### Comparing `straxen-2.2.1/straxen.egg-info/PKG-INFO` & `straxen-2.2.2/straxen.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: straxen
-Version: 2.2.1
+Version: 2.2.2
 Summary: Streaming analysis for XENON
 Home-page: https://github.com/XENONnT/straxen
 Author: Straxen contributors, the XENON collaboration
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
@@ -37,14 +37,40 @@
 
 
 ## Further status
 [![Python Versions](https://img.shields.io/pypi/pyversions/straxen.svg)](https://pypi.python.org/pypi/straxen)
 [![PyPI downloads](https://img.shields.io/pypi/dm/straxen.svg)](https://pypistats.org/packages/straxen)
 
 
+2.2.2 / 2024-04-30
+-------------------
+* Minor change of indents by @dachengx in https://github.com/XENONnT/straxen/pull/1341
+* Remove unused `__all__` by @dachengx in https://github.com/XENONnT/straxen/pull/1342
+* Bump graphviz from 0.20.1 to 0.20.2 in /extra_requirements by @dependabot in https://github.com/XENONnT/straxen/pull/1345
+* Specifically install `lxml_html_clean` by @dachengx in https://github.com/XENONnT/straxen/pull/1352
+* Improve InterpolateAndExtrapolate performance for array valued maps by @l-althueser in https://github.com/XENONnT/straxen/pull/1347
+* Bump graphviz from 0.20.2 to 0.20.3 in /extra_requirements by @dependabot in https://github.com/XENONnT/straxen/pull/1350
+* Bump actions/setup-python from 5.0.0 to 5.1.0 by @dependabot in https://github.com/XENONnT/straxen/pull/1351
+* Add `storage_graph` to show the plugins stored or needed to be calculated in the dependency tree by @dachengx in https://github.com/XENONnT/straxen/pull/1353
+* Small bug fix of `storage_graph`, save plot into desired folder by @dachengx in https://github.com/XENONnT/straxen/pull/1356
+* Check non-positive lone_hits by @dachengx in https://github.com/XENONnT/straxen/pull/1358
+* Return the edge closer to the target in `_numeric_derivative` by @dachengx in https://github.com/XENONnT/straxen/pull/1355
+* Add a simply function to plot the dependency tree by @dachengx in https://github.com/XENONnT/straxen/pull/1363
+* Remove `PeakSubtyping` from straxen by @dachengx in https://github.com/XENONnT/straxen/pull/1365
+* Remove `xnt_simulation_config` by @dachengx in https://github.com/XENONnT/straxen/pull/1366
+* Tolerate more exceptions when can not import admix by @dachengx in https://github.com/XENONnT/straxen/pull/1367
+* Add `PeakSEDensity` and `EventSEDensity` by @dachengx in https://github.com/XENONnT/straxen/pull/1368
+* Update `se_time_search_window_left` by @dachengx in https://github.com/XENONnT/straxen/pull/1370
+* remove resource_cache from dali by @yuema137 in https://github.com/XENONnT/straxen/pull/1372
+* Add `exclude_pattern` argument to `dependency_tree` by @dachengx in https://github.com/XENONnT/straxen/pull/1373
+* Let xedocs to handle avg seg and seg partitioning by @GiovanniVolta in https://github.com/XENONnT/straxen/pull/1371
+
+**Full Changelog**: https://github.com/XENONnT/straxen/compare/v2.2.1...v2.2.2
+
+
 2.2.1 / 2024-02-21
 -------------------
 * Loosen `save_when` of `Events` by @dachengx in https://github.com/XENONnT/straxen/pull/1327
 * Deprecate the usage of `XENONnT/ax_env` by @dachengx in https://github.com/XENONnT/straxen/pull/1329
 * `_text_formats` should include txt but not text by @dachengx in https://github.com/XENONnT/straxen/pull/1324
 * Fix numerical comparison error of `test_patternfit_stats` by @dachengx in https://github.com/XENONnT/straxen/pull/1334
 * Remove some packages requirements from `requirements-tests.txt` by @dachengx in https://github.com/XENONnT/straxen/pull/1337
```

### Comparing `straxen-2.2.1/straxen.egg-info/SOURCES.txt` & `straxen-2.2.2/straxen.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 straxen/plugins/events/event_nearest_triggering.py
 straxen/plugins/events/event_pattern_fit.py
 straxen/plugins/events/event_positions.py
 straxen/plugins/events/event_s1_positions_cnn.py
 straxen/plugins/events/event_s2_positions_cnn.py
 straxen/plugins/events/event_s2_positions_gcn.py
 straxen/plugins/events/event_s2_positions_mlp.py
+straxen/plugins/events/event_se_sensity.py
 straxen/plugins/events/event_shadow.py
 straxen/plugins/events/event_top_bottom_params.py
 straxen/plugins/events/event_w_bayes_class.py
 straxen/plugins/events/event_waveform.py
 straxen/plugins/events/events.py
 straxen/plugins/events/local_minimum_info.py
 straxen/plugins/events/multi_scatter.py
@@ -144,19 +145,19 @@
 straxen/plugins/peaks/peak_per_event.py
 straxen/plugins/peaks/peak_positions.py
 straxen/plugins/peaks/peak_positions_cnn.py
 straxen/plugins/peaks/peak_positions_gcn.py
 straxen/plugins/peaks/peak_positions_mlp.py
 straxen/plugins/peaks/peak_proximity.py
 straxen/plugins/peaks/peak_s1_positions_cnn.py
+straxen/plugins/peaks/peak_se_sensity.py
 straxen/plugins/peaks/peak_shadow.py
 straxen/plugins/peaks/peak_top_bottom_params.py
 straxen/plugins/peaks/peaks.py
 straxen/plugins/peaks/peaks_som.py
-straxen/plugins/peaks/peaks_subtyping.py
 straxen/plugins/peaks_he/__init__.py
 straxen/plugins/peaks_he/peak_basics_he.py
 straxen/plugins/peaks_he/peaks_he.py
 straxen/plugins/raw_records/__init__.py
 straxen/plugins/raw_records/daqreader.py
 straxen/plugins/raw_records_coin_nv/__init__.py
 straxen/plugins/raw_records_coin_nv/nveto_recorder.py
```

### Comparing `straxen-2.2.1/tests/storage/test_database_frontends.py` & `straxen-2.2.2/tests/storage/test_database_frontends.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/tests/storage/test_mongo_downloader.py` & `straxen-2.2.2/tests/storage/test_mongo_downloader.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/tests/storage/test_mongo_interactions.py` & `straxen-2.2.2/tests/storage/test_mongo_interactions.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/tests/storage/test_rucio_local.py` & `straxen-2.2.2/tests/storage/test_rucio_local.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/tests/storage/test_rucio_remote.py` & `straxen-2.2.2/tests/storage/test_rucio_remote.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/tests/test_1T_plugins.py` & `straxen-2.2.2/tests/test_1T_plugins.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/tests/test_aqmon.py` & `straxen-2.2.2/tests/test_aqmon.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/tests/test_basics.py` & `straxen-2.2.2/tests/test_basics.py`

 * *Files 21% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         st = self.st
         # Ignore strax-internal warnings
         st.set_context_config({"free_options": tuple(st.config.keys())})
 
         run_df = st.select_runs(available="raw_records")
         print(run_df)
         run_id = run_df.iloc[0]["name"]
-        assert run_id == test_run_id_1T
+        assert run_id == self.run_id
 
     def test_mini_analysis(self):
         @straxen.mini_analysis(requires=("raw_records",))
         def count_rr(raw_records):
             return len(raw_records)
 
         n = self.st.count_rr(self.run_id)
@@ -77,7 +77,17 @@
         self.test_extract_latest_comment_nt(test_for_target="lone_hits")
 
     @unittest.skipIf(not straxen.utilix_is_configured(), "No db access, cannot test!")
     def test_raw_records_lineage(self):
         """The raw records lineage may NEVER change, if you ever do, doom ensures."""
         st = straxen.contexts.xenonnt_online()
         self.assertTrue(st.key_for("0", "raw_records").lineage_hash == "rfzvpzj4mf")
+
+    def test_storage_graph(self):
+        """Test the storage graph."""
+        self.st.storage_graph(self.run_id, "event_info")
+        self.st.storage_graph(self.run_id, "event_info", include_class=True)
+
+    def test_dependency_tree(self):
+        """Test the dependency tree."""
+        self.st.dependency_tree("event_info")
+        self.st.dependency_tree("event_info", include_class=True, exclude_pattern="raw_records_*")
```

### Comparing `straxen-2.2.1/tests/test_channel_split.py` & `straxen-2.2.2/tests/test_channel_split.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/tests/test_cmt.py` & `straxen-2.2.2/tests/test_cmt.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/tests/test_common.py` & `straxen-2.2.2/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/tests/test_contexts.py` & `straxen-2.2.2/tests/test_contexts.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         try:
             xenonnt(global_version)
             success_for.append(global_version)
         except straxen.CMTVersionError:
             pass
     print(
         f"This straxen version works with {success_for} but is "
-        f"incompatible with {set(cmt_versions)-set(success_for)}"
+        f"incompatible with {set(cmt_versions) - set(success_for)}"
     )
 
     test = unittest.TestCase()
     # We should always work for one offline and the online version
     test.assertTrue(len(success_for) >= 2)
```

### Comparing `straxen-2.2.1/tests/test_count_pulses.py` & `straxen-2.2.2/tests/test_count_pulses.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/tests/test_daq_reader.py` & `straxen-2.2.2/tests/test_daq_reader.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/tests/test_holoviews_utils.py` & `straxen-2.2.2/tests/test_holoviews_utils.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/tests/test_itp_map.py` & `straxen-2.2.2/tests/test_itp_map.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/tests/test_led_calibration.py` & `straxen-2.2.2/tests/test_led_calibration.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/tests/test_mini_analyses.py` & `straxen-2.2.2/tests/test_mini_analyses.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/tests/test_misc.py` & `straxen-2.2.2/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/tests/test_nveto_events.py` & `straxen-2.2.2/tests/test_nveto_events.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/tests/test_nveto_recorder.py` & `straxen-2.2.2/tests/test_nveto_recorder.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/tests/test_patternfit.py` & `straxen-2.2.2/tests/test_patternfit.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/tests/test_peaklet_processing.py` & `straxen-2.2.2/tests/test_peaklet_processing.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/tests/test_peaks.py` & `straxen-2.2.2/tests/test_peaks.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/tests/test_scada.py` & `straxen-2.2.2/tests/test_scada.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/tests/test_url_config.py` & `straxen-2.2.2/tests/test_url_config.py`

 * *Files identical despite different names*

### Comparing `straxen-2.2.1/tests/test_veto_hitlets.py` & `straxen-2.2.2/tests/test_veto_hitlets.py`

 * *Files identical despite different names*


# Comparing `tmp/pygmt-0.8.0.tar.gz` & `tmp/pygmt-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmt-0.8.0.tar", last modified: Thu Dec 29 22:52:05 2022, max compression
+gzip compressed data, was "pygmt-0.9.0.tar", last modified: Fri Mar 31 21:13:26 2023, max compression
```

## Comparing `pygmt-0.8.0.tar` & `pygmt-0.9.0.tar`

### file list

```diff
@@ -1,355 +1,374 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 22:52:05.831999 pygmt-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2022-12-29 22:51:56.000000 pygmt-0.8.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2022-12-29 22:51:56.000000 pygmt-0.8.0/AUTHORSHIP.md
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2022-12-29 22:51:56.000000 pygmt-0.8.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)      188 2022-12-29 22:51:56.000000 pygmt-0.8.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2022-12-29 22:51:56.000000 pygmt-0.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2022-12-29 22:51:56.000000 pygmt-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13626 2022-12-29 22:52:05.831999 pygmt-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12503 2022-12-29 22:51:56.000000 pygmt-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 22:52:05.791999 pygmt-0.8.0/pygmt/
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/accessors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 22:52:05.791999 pygmt-0.8.0/pygmt/clib/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/clib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10015 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/clib/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/clib/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)    57311 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/clib/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 22:52:05.795999 pygmt-0.8.0/pygmt/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/datasets/earth_age.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/datasets/earth_free_air_anomaly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/datasets/earth_geoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/datasets/earth_magnetic_anomaly.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/datasets/earth_relief.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/datasets/earth_vertical_gravity_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)    11817 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/datasets/load_remote_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14156 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/datasets/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20662 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/figure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 22:52:05.795999 pygmt-0.8.0/pygmt/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34770 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/helpers/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/helpers/tempfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/helpers/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10799 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/helpers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/session_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/sphinx_gallery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 22:52:05.799999 pygmt-0.8.0/pygmt/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/basemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/binstats.py
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/blockm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/coast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/colorbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/dimfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/filter1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9475 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/grd2cpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7626 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/grd2xyz.py
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/grdclip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/grdcontour.py
--rw-r--r--   0 runner    (1001) docker     (123)     4367 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/grdcut.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/grdfill.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/grdfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/grdgradient.py
--rw-r--r--   0 runner    (1001) docker     (123)    12607 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/grdhisteq.py
--rw-r--r--   0 runner    (1001) docker     (123)     8427 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/grdimage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/grdinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/grdlandmask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/grdproject.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/grdsample.py
--rw-r--r--   0 runner    (1001) docker     (123)    17240 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/grdtrack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/grdview.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/grdvolume.py
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/inset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/legend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/logo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7928 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/makecpt.py
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/meca.py
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/nearneighbor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10503 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9188 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/plot3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    11076 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/rose.py
--rw-r--r--   0 runner    (1001) docker     (123)     7130 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/solar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/sph2grd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/sphdistance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/sphinterpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10457 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/subplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/ternary.py
--rw-r--r--   0 runner    (1001) docker     (123)     8370 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    14374 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/triangulate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11860 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/velo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/which.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/wiggle.py
--rw-r--r--   0 runner    (1001) docker     (123)     9595 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/x2sys_cross.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/x2sys_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/src/xyz2grd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 22:52:05.811999 pygmt-0.8.0/pygmt/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 22:52:05.831999 pygmt-0.8.0/pygmt/tests/baseline/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_basemap.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_basemap_compass.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_basemap_loglog.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_basemap_map_scale.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_basemap_polar.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       96 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_basemap_power_axis.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_basemap_required_args.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       90 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_basemap_rose.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       99 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_basemap_utm_projection.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       99 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_basemap_winkel_tripel.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_coast_dcw_list.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       94 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_coast_dcw_single.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       90 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_coast_region.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       99 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_coast_world_mercator.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       89 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_colorbar_box.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       99 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_colorbar_box_with_fill.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      101 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_colorbar_scaled_z_values.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      102 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_colorbar_shading_boolean.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       99 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_colorbar_shading_list.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      109 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_colorbar_truncated_to_zlow_zhigh.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       84 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_config.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_config_font_annot.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_config_font_one.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       99 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_config_format_date_map.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       99 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_config_format_time_map.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_config_map_annot_offset.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_config_map_grid_cross_size.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       97 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_config_map_grid_pen.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_config_map_tick_length.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       97 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_config_map_tick_pen.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_contour_from_file.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_contour_matrix.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       89 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_contour_vec.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       96 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_figure_shift_origin.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      107 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_geopandas_plot3d_default_cube.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_geopandas_plot3d_non_default_circle.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      106 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_geopandas_plot_default_square.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      110 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_geopandas_plot_non_default_circle.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       85 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_grd2cpt.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       89 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_grdcontour.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      112 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_grdcontour_interval_file_full_opts.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       96 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_grdcontour_labels.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       94 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_grdcontour_slice.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       87 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_grdimage.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_grdimage_file.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_grdimage_global_subset.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_grdimage_over_dateline.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_grdimage_slice.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_grdview_drapegrid_dataarray.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       99 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_grdview_grid_dataarray.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       96 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_grdview_on_a_plane.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      118 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_grdview_on_a_plane_styled_with_facadepen.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      124 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_grdview_on_a_plane_with_colored_frontal_facade.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      123 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_grdview_surface_mesh_plot_styled_with_meshpen.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      121 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_grdview_surface_plot_styled_with_contourpen.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      111 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_grdview_with_cmap_for_image_plot.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      124 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_grdview_with_cmap_for_perspective_surface_plot.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      123 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_grdview_with_cmap_for_surface_monochrome_plot.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      102 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_grdview_with_perspective.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      118 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_grdview_with_perspective_and_zaxis_frame.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_grdview_with_perspective_and_zscale.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      112 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_grdview_with_perspective_and_zsize.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       87 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_histogram.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       83 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_image.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_inset_aliases.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       99 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_inset_context_manager.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      101 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_legend_default_position.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_legend_entries.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_legend_position.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_legend_specfile.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       82 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_logo.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_logo_on_a_map.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       96 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_makecpt_categorical.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_makecpt_continuous.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_makecpt_cyclic.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_makecpt_plot_colorbar.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      117 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_makecpt_plot_colorbar_scaled_with_series.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       97 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_makecpt_plot_points.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_makecpt_reverse_color_and_zsign.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_makecpt_reverse_color_only.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_makecpt_truncated_zlow_zhigh.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       97 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_meca_dict_eventname.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       94 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_meca_dict_offset.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_meca_dict_offset_eventname.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       97 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_meca_gcmt_convention.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_meca_loc_array.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_meca_spec_1d_array.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_meca_spec_2d_array.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       96 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_meca_spec_dataframe.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       97 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_meca_spec_dict_list.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_meca_spec_dictionary.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_meca_spec_file.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot3d_colors.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       97 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot3d_colors_sizes.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      102 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot3d_colors_sizes_proj.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       94 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot3d_from_file.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot3d_matrix.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       97 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot3d_matrix_color.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      121 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot3d_ogrgmt_file_multipoint_default_style.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      125 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot3d_ogrgmt_file_multipoint_non_default_style.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot3d_projection.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot3d_red_circles_zscale.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      102 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot3d_red_circles_zsize.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot3d_scalar_xyz.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       90 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot3d_sizes.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      112 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot3d_sizes_colors_transparencies.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       97 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot3d_transparency.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      102 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot3d_varying_intensity.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot3d_varying_transparency.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot3d_vectors.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       89 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot_colors.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot_colors_sizes.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot_colors_sizes_proj.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot_dataframe_incols.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot_datetime.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot_from_file.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot_lines_with_arrows.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       89 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot_matrix.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot_matrix_color.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      118 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot_ogrgmt_file_multipoint_default_style.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      122 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot_ogrgmt_file_multipoint_non_default_style.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot_projection.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       94 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot_red_circles.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot_scalar_xy.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot_shapefile.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot_sizes.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      110 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot_sizes_colors_transparencies.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot_transparency.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       99 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot_varying_intensity.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot_varying_transparency.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       90 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_plot_vectors.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_rose_2d_array_multiple.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_rose_2d_array_single.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_rose_bools.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_rose_data_file.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       94 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_rose_no_sectors.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      102 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_rose_plot_data_using_cpt.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_rose_plot_with_transparency.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      107 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_solar_set_terminator_datetime.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_solar_terminators.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      109 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_subplot_autolabel_margins_title.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       96 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_subplot_basic_frame.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      120 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_subplot_clearance_and_shared_xy_axis_layout.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_subplot_direct.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       85 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_ternary.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_ternary_1_label.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       94 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_ternary_3_labels.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       90 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_text_angle_30.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      114 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_text_angle_font_justify_from_textfile.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       86 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_text_fill.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_text_font_bold.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      107 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_text_input_multiple_filenames.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_text_input_remote_filename.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_text_input_single_filename.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      115 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_text_justify_bottom_right_and_top_left.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      111 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_text_justify_parsed_from_textfile.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_text_multiple_lines_of_text.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       94 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_text_nonstr_text.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       85 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_text_pen.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       90 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_text_position.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      107 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_text_position_offset_with_line.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       97 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_text_round_clearance.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      101 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_text_single_line_of_text.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       95 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_text_transparency.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_text_varying_transparency.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)      107 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_velo_numpy_array_numeric_only.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       99 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_velo_pandas_dataframe.png.dvc
--rw-r--r--   0 runner    (1001) docker     (123)       83 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/baseline/test_wiggle.png.dvc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 22:52:05.831999 pygmt-0.8.0/pygmt/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/data/cities.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/data/contours.txt
--rw-r--r--   0 runner    (1001) docker     (123)      444 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/data/points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/data/track.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_basemap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_binstats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_blockm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_blockmedian.py
--rw-r--r--   0 runner    (1001) docker     (123)    31427 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_clib.py
--rw-r--r--   0 runner    (1001) docker     (123)    11895 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_clib_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_clib_put_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_clib_put_strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_clib_put_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_coast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_colorbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_datasets_earth_age.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_datasets_earth_free_air_anomaly.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_datasets_earth_geoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_datasets_earth_magnetic_anomaly.py
--rw-r--r--   0 runner    (1001) docker     (123)     8848 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_datasets_earth_relief.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_datasets_earth_vertical_gravity_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_datasets_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_dimfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9299 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_figure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_filter1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_geopandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_grd2cpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_grd2xyz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_grdclip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_grdcontour.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_grdcut.py
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_grdfill.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_grdfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_grdgradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_grdhisteq.py
--rw-r--r--   0 runner    (1001) docker     (123)     7611 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_grdimage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_grdinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_grdlandmask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_grdproject.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_grdsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_grdtrack.py
--rw-r--r--   0 runner    (1001) docker     (123)     7077 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_grdview.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_grdvolume.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_inset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_legend.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_logo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_makecpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     9200 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_meca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_nearneighbor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12664 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    11606 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_plot3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_psconvert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_rose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_session_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_solar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_sph2grd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_sphdistance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_sphinterpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_sphinx_gallery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_subplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_ternary.py
--rw-r--r--   0 runner    (1001) docker     (123)     9571 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_triangulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_velo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_which.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_wiggle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8831 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_x2sys_cross.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_x2sys_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2022-12-29 22:51:56.000000 pygmt-0.8.0/pygmt/tests/test_xyz2grd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 22:52:05.791999 pygmt-0.8.0/pygmt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13626 2022-12-29 22:52:05.000000 pygmt-0.8.0/pygmt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14015 2022-12-29 22:52:05.000000 pygmt-0.8.0/pygmt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-29 22:52:05.000000 pygmt-0.8.0/pygmt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2022-12-29 22:52:05.000000 pygmt-0.8.0/pygmt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-29 22:52:05.000000 pygmt-0.8.0/pygmt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2022-12-29 22:51:56.000000 pygmt-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-29 22:52:05.831999 pygmt-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:13:26.865235 pygmt-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-03-31 21:13:15.000000 pygmt-0.9.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-03-31 21:13:15.000000 pygmt-0.9.0/AUTHORSHIP.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-03-31 21:13:15.000000 pygmt-0.9.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-31 21:13:15.000000 pygmt-0.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-03-31 21:13:15.000000 pygmt-0.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-31 21:13:15.000000 pygmt-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14555 2023-03-31 21:13:26.865235 pygmt-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-03-31 21:13:15.000000 pygmt-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:13:26.805235 pygmt-0.9.0/pygmt/
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/accessors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:13:26.805235 pygmt-0.9.0/pygmt/clib/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/clib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/clib/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/clib/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58798 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/clib/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:13:26.809235 pygmt-0.9.0/pygmt/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/datasets/earth_age.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/datasets/earth_free_air_anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/datasets/earth_geoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/datasets/earth_magnetic_anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/datasets/earth_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/datasets/earth_relief.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/datasets/earth_vertical_gravity_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/datasets/load_remote_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10274 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/datasets/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/datasets/tile_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22140 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/figure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:13:26.809235 pygmt-0.9.0/pygmt/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35032 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/helpers/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/helpers/tempfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/helpers/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11243 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/helpers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/session_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/sphinx_gallery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:13:26.821235 pygmt-0.9.0/pygmt/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/basemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/binstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/blockm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/coast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/colorbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/dimfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/filter1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/grd2cpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7626 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/grd2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/grdclip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/grdcontour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/grdcut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/grdfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/grdfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/grdgradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/grdhisteq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/grdimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/grdinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/grdlandmask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/grdproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/grdsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16129 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/grdtrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/grdview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/grdvolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/inset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/legend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/logo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/makecpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/meca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/nearneighbor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10496 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/plot3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/rose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/solar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/sph2grd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/sphdistance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/sphinterpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10760 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/subplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/ternary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/tilemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14373 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/triangulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11849 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/velo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/which.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/wiggle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/x2sys_cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/x2sys_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/src/xyz2grd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:13:26.833235 pygmt-0.9.0/pygmt/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:13:26.865235 pygmt-0.9.0/pygmt/tests/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_basemap.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_basemap_compass.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_basemap_loglog.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_basemap_map_scale.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_basemap_polar.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_basemap_power_axis.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_basemap_rose.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_basemap_subplot.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_basemap_utm_projection.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_basemap_winkel_tripel.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_coast_dcw_list.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_coast_dcw_single.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_coast_region.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_coast_world_mercator.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_colorbar_box.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_colorbar_box_with_fill.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_colorbar_scaled_z_values.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_colorbar_shading_boolean.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_colorbar_shading_list.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_colorbar_truncated_to_zlow_zhigh.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_config.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_config_font_annot.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_config_font_one.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_config_format_date_map.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_config_format_time_map.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_config_map_annot_offset.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_config_map_grid_cross_size.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_config_map_grid_pen.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_config_map_tick_length.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_config_map_tick_pen.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_contour_from_file.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_contour_matrix.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_contour_vec.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_figure_shift_origin.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_geopandas_plot3d_default_cube.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_geopandas_plot3d_non_default_circle.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_geopandas_plot_default_square.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_geopandas_plot_non_default_circle.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_grd2cpt.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_grdcontour.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_grdcontour_interval_file_full_opts.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_grdcontour_labels.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_grdcontour_slice.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_grdimage.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_grdimage_file.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_grdimage_global_subset.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_grdimage_over_dateline.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_grdimage_slice.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_grdview_drapegrid_dataarray.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_grdview_grid_dataarray.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_grdview_on_a_plane.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_grdview_on_a_plane_styled_with_facadepen.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_grdview_on_a_plane_with_colored_frontal_facade.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_grdview_surface_mesh_plot_styled_with_meshpen.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_grdview_surface_plot_styled_with_contourpen.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_grdview_with_cmap_for_image_plot.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_grdview_with_cmap_for_perspective_surface_plot.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_grdview_with_cmap_for_surface_monochrome_plot.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_grdview_with_perspective.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_grdview_with_perspective_and_zaxis_frame.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_grdview_with_perspective_and_zscale.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_grdview_with_perspective_and_zsize.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_histogram.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_image.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_inset_aliases.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_inset_context_manager.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_legend_default_position.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_legend_entries.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_legend_position.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_legend_specfile.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_logo.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_logo_on_a_map.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_makecpt_categorical.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_makecpt_continuous.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_makecpt_cyclic.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_makecpt_plot_colorbar.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_makecpt_plot_colorbar_scaled_with_series.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_makecpt_plot_points.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_makecpt_reverse_color_and_zsign.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_makecpt_reverse_color_only.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_makecpt_truncated_zlow_zhigh.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_meca_dict_eventname.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_meca_dict_offset.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_meca_dict_offset_eventname.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_meca_gcmt_convention.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_meca_loc_array.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_meca_spec_1d_array.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_meca_spec_2d_array.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_meca_spec_dataframe.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_meca_spec_dict_list.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_meca_spec_dictionary.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_meca_spec_file.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot3d_colors.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot3d_colors_sizes.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot3d_colors_sizes_proj.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot3d_from_file.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot3d_matrix.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot3d_matrix_color.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot3d_ogrgmt_file_multipoint_default_style.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot3d_ogrgmt_file_multipoint_non_default_style.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot3d_projection.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot3d_red_circles_zscale.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot3d_red_circles_zsize.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot3d_scalar_xyz.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot3d_sizes.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot3d_sizes_colors_transparencies.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot3d_transparency.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot3d_varying_intensity.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot3d_varying_transparency.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot3d_vectors.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot_colors.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot_colors_sizes.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot_colors_sizes_proj.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot_dataframe_incols.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot_datetime.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot_from_file.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot_lines_with_arrows.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot_matrix.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot_matrix_color.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot_ogrgmt_file_multipoint_default_style.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot_ogrgmt_file_multipoint_non_default_style.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot_projection.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot_red_circles.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot_scalar_xy.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot_shapefile.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot_sizes.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot_sizes_colors_transparencies.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot_transparency.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot_varying_intensity.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot_varying_transparency.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_plot_vectors.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_rose_2d_array_multiple.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_rose_2d_array_single.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_rose_bools.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_rose_data_file.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_rose_no_sectors.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_rose_plot_data_using_cpt.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_rose_plot_with_transparency.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_solar_set_terminator_datetime.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_solar_terminators.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_subplot_autolabel_margins_title.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_subplot_basic_frame.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_subplot_clearance_and_shared_xy_axis_layout.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_subplot_direct.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_subplot_outside_plotting_positioning.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_ternary.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_ternary_1_label.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_ternary_3_labels.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_text_angle_30.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_text_angle_font_justify_from_textfile.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_text_fill.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_text_font_bold.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_text_input_multiple_filenames.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_text_input_remote_filename.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_text_input_single_filename.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_text_justify_bottom_right_and_top_left.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_text_justify_parsed_from_textfile.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_text_multiple_lines_of_text.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_text_nonstr_text.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_text_pen.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_text_position.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_text_position_offset_with_line.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_text_round_clearance.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_text_single_line_of_text.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_text_transparency.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_text_varying_transparency.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_tilemap_no_clip_False.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_tilemap_no_clip_True.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_tilemap_ogc_wgs84.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_tilemap_web_mercator.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_timestamp.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_timestamp_font.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_timestamp_justification.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_timestamp_label.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_timestamp_offset.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_timestamp_text_truncated.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_velo_numpy_array_numeric_only.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_velo_pandas_dataframe.png.dvc
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/baseline/test_wiggle.png.dvc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:13:26.865235 pygmt-0.9.0/pygmt/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/data/cities.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/data/contours.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/data/points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/data/track.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_basemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_binstats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_blockm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_blockmedian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31432 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_clib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_clib_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_clib_put_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_clib_put_strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_clib_put_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_coast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_colorbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_datasets_earth_age.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_datasets_earth_free_air_anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_datasets_earth_geoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_datasets_earth_magnetic_anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_datasets_earth_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8848 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_datasets_earth_relief.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_datasets_earth_vertical_gravity_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_datasets_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_dimfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_figure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_filter1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_geopandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_grd2cpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_grd2xyz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_grdclip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_grdcontour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_grdcut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_grdfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_grdfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_grdgradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_grdhisteq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_grdimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_grdinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_grdlandmask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_grdproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_grdsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_grdtrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_grdview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_grdvolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_inset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_legend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_logo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_makecpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_meca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_nearneighbor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12703 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11613 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_plot3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_psconvert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_rose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_session_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_solar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_sph2grd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_sphdistance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_sphinterpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_sphinx_gallery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_subplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_ternary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9571 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_tilemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_triangulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_velo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_which.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_wiggle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_x2sys_cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_x2sys_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-03-31 21:13:15.000000 pygmt-0.9.0/pygmt/tests/test_xyz2grd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:13:26.805235 pygmt-0.9.0/pygmt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14555 2023-03-31 21:13:26.000000 pygmt-0.9.0/pygmt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14822 2023-03-31 21:13:26.000000 pygmt-0.9.0/pygmt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 21:13:26.000000 pygmt-0.9.0/pygmt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-31 21:13:26.000000 pygmt-0.9.0/pygmt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-31 21:13:26.000000 pygmt-0.9.0/pygmt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-03-31 21:13:15.000000 pygmt-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 21:13:26.865235 pygmt-0.9.0/setup.cfg
```

### Comparing `pygmt-0.8.0/AUTHORS.md` & `pygmt-0.9.0/AUTHORS.md`

 * *Files 10% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 (alphabetical by name) and are considered to be "PyGMT Developers":
 
 * [Abhishek Anant](https://twitter.com/itsabhianant) | [0000-0002-5751-2010](https://orcid.org/0000-0002-5751-2010) | Unaffiliated
 * [Andre L. Belem](https://github.com/andrebelem) | [0000-0002-8865-6180](https://orcid.org/0000-0002-8865-6180) | Fluminense Federal University, Brazil
 * [Dongdong Tian](https://seisman.info/) | [0000-0001-7967-1197](https://orcid.org/0000-0001-7967-1197) | China University of Geosciences, China
 * [Jamie Quinn](http://jamiejquinn.com) | [0000-0002-0268-7032](https://orcid.org/0000-0002-0268-7032) | University College London, United Kingdom
 * [Jiayuan Yao](https://github.com/core-man) | [0000-0001-7036-4238](https://orcid.org/0000-0001-7036-4238) | Nanyang Technological University, Singapore
+* [Jing-Hui Tong](https://github.com/JingHuiTong) | [0009-0002-7195-3071](https://orcid.org/0009-0002-7195-3071) | National Taiwan Normal University, Taiwan
 * [Kathryn Materna](https://github.com/kmaterna) | [0000-0002-6687-980X](https://orcid.org/0000-0002-6687-980X) | US Geological Survey, USA
 * [Leonardo Uieda](http://www.leouieda.com/) | [0000-0001-6123-9515](https://orcid.org/0000-0001-6123-9515) | University of Liverpool, United Kingdom
 * [Liam Toney](https://liam.earth/) | [0000-0003-0167-9433](https://orcid.org/0000-0003-0167-9433) | University of Alaska Fairbanks, USA
 * [Malte Ziebarth](https://github.com/mjziebarth) | [0000-0002-5190-4478](https://orcid.org/0000-0002-5190-4478) | GFZ German Research Centre for Geosciences, Germany
 * [Max Jones](https://github.com/maxrjones) | [0000-0003-0180-8928](https://orcid.org/0000-0003-0180-8928) | University of Hawai'i at Mānoa, USA
 * [Michael Grund](https://github.com/michaelgrund) | [0000-0001-8759-2018](https://orcid.org/0000-0001-8759-2018) | Innoplexia GmbH, Germany
 * [Tyler Newton](http://www.tnewton.com/) | [0000-0002-1560-6553](https://orcid.org/0000-0002-1560-6553) | University of Oregon, USA
-* [Wei Ji Leong](https://github.com/weiji14) | [0000-0003-2354-1988](https://orcid.org/0000-0003-2354-1988) | The Ohio State University, USA
+* [Wei Ji Leong](https://github.com/weiji14) | [0000-0003-2354-1988](https://orcid.org/0000-0003-2354-1988) | Development Seed, USA
 * [William Schlitzer](https://github.com/willschlitzer) | [0000-0002-5843-2282](https://orcid.org/0000-0002-5843-2282) | Unaffiliated
 * [Yohai Magen](https://github.com/yohaimagen) | [0000-0002-4892-4013](https://orcid.org/0000-0002-4892-4013) | Tel Aviv University, Israel
 * [Yvonne Fröhlich](https://github.com/yvonnefroehlich) | [0000-0002-8566-0619](https://orcid.org/0000-0002-8566-0619) | Karlsruhe Institute of Technology, Germany
```

### Comparing `pygmt-0.8.0/AUTHORSHIP.md` & `pygmt-0.9.0/AUTHORSHIP.md`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/CITATION.cff` & `pygmt-0.9.0/CITATION.cff`

 * *Files 9% similar despite different names*

```diff
@@ -10,44 +10,48 @@
   orcid: https://orcid.org/0000-0001-6123-9515
 - given-names: Dongdong
   family-names: Tian
   affiliation: China University of Geosciences, China
   orcid: https://orcid.org/0000-0001-7967-1197
 - given-names: Wei Ji
   family-names: Leong
-  affiliation: The Ohio State University, USA
+  affiliation: Development Seed, USA
   orcid: https://orcid.org/0000-0003-2354-1988
-- given-names: Max
-  family-names: Jones
-  affiliation: University of Hawai'i at Mānoa, USA
-  orcid: https://orcid.org/0000-0003-0180-8928
 - given-names: William
   family-names: Schlitzer
   affiliation: Unaffiliated
   orcid: https://orcid.org/0000-0002-5843-2282
 - given-names: Michael
   family-names: Grund
   affiliation: Innoplexia GmbH, Germany
   orcid: https://orcid.org/0000-0001-8759-2018
-- given-names: Liam
-  family-names: Toney
-  affiliation: University of Alaska Fairbanks, USA
-  orcid: https://orcid.org/0000-0003-0167-9433
+- given-names: Max
+  family-names: Jones
+  affiliation: University of Hawai'i at Mānoa, USA
+  orcid: https://orcid.org/0000-0003-0180-8928
 - given-names: Yvonne
   family-names: Fröhlich
   affiliation: Karlsruhe Institute of Technology, Germany
   orcid: https://orcid.org/0000-0002-8566-0619
+- given-names: Liam
+  family-names: Toney
+  affiliation: University of Alaska Fairbanks, USA
+  orcid: https://orcid.org/0000-0003-0167-9433
 - given-names: Jiayuan
   family-names: Yao
   affiliation: Nanyang Technological University, Singapore
   orcid: https://orcid.org/0000-0001-7036-4238
 - given-names: Yohai
   family-names: Magen
   affiliation: Tel Aviv University, Israel
   orcid: https://orcid.org/0000-0002-4892-4013
+- given-names: Tong
+  family-names: Jing-Hui
+  affiliation: National Taiwan Normal University, Taiwan
+  orcid: https://orcid.org/0009-0002-7195-3071
 - given-names: Kathryn
   family-names: Materna
   affiliation: US Geological Survey, USA
   orcid: https://orcid.org/0000-0002-6687-980X
 - given-names: Andre
   family-names: Belem
   affiliation: Fluminense Federal University, Brazil
@@ -68,13 +72,13 @@
   family-names: Quinn
   affiliation: University College London, United Kingdom
   orcid: https://orcid.org/0000-0002-0268-7032
 - given-names: Paul
   family-names: Wessel
   affiliation: University of Hawai'i at Mānoa, USA
   orcid: https://orcid.org/0000-0001-5708-7336
-date-released: 2022-12-30
-doi: 10.5281/zenodo.7481934
+date-released: 2023-03-31
+doi: 10.5281/zenodo.7772533
 license: BSD-3-Clause
 repository-code: https://github.com/GenericMappingTools/pygmt
 type: software
-version: 0.8.0
+version: 0.9.0
```

### Comparing `pygmt-0.8.0/LICENSE.txt` & `pygmt-0.9.0/LICENSE.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2017-2022 The PyGMT Developers
+Copyright (c) 2017-2023 The PyGMT Developers
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice,
   this list of conditions and the following disclaimer.
```

### Comparing `pygmt-0.8.0/PKG-INFO` & `pygmt-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: pygmt
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Python interface for the Generic Mapping Tools
 Author-email: The PyGMT Developers <pygmt.team@gmail.com>
 License: BSD License
 Project-URL: homepage, https://www.pygmt.org
 Project-URL: documentation, https://www.pygmt.org
 Project-URL: repository, https://github.com/GenericMappingTools/pygmt
 Project-URL: changelog, https://www.pygmt.org/latest/changes.html
+Keywords: cartography,geodesy,geology,geophysics,geospatial,oceanography,seismology
 Platform: Any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
@@ -80,30 +81,31 @@
 ----------
 
 A beautiful map is worth a thousand words.
 To truly understand how powerful PyGMT is, play with it online on `Binder <https://github.com/GenericMappingTools/try-gmt>`__!
 For a quicker introduction, check out our `3 minute overview <https://youtu.be/4iPnITXrxVU>`__!
 
 Afterwards, feel free to look at our `Tutorials <https://www.pygmt.org/latest/tutorials>`__,
-visit the `PyGMT Gallery <https://www.pygmt.org/latest/gallery>`__, and check out
+visit the `Gallery <https://www.pygmt.org/latest/gallery>`__, and check out
 some `external PyGMT examples <https://www.pygmt.org/latest/external_resources.html>`__!
 
 .. image:: https://user-images.githubusercontent.com/14077947/155809878-48b8f235-141b-460a-80ec-08bbf6c36e40.png
     :alt: Quick Introduction to PyGMT YouTube Video
     :align: center
     :target: https://youtu.be/4iPnITXrxVU
     :width: 80%
 
 About
 -----
 
 PyGMT is a library for processing geospatial and geophysical data and making
-publication quality maps and figures. It provides a Pythonic interface for the
+publication-quality maps and figures. It provides a Pythonic interface for the
 `Generic Mapping Tools (GMT) <https://github.com/GenericMappingTools/gmt>`__, a
-command-line program widely used in the Earth Sciences.
+command-line program widely used across the Earth, Ocean, and Planetary sciences
+and beyond.
 
 Project goals
 -------------
 
 * Make GMT more accessible to new users.
 * Build a Pythonic API for GMT.
 * Interface with the GMT C API directly using ctypes (no system calls).
@@ -116,24 +118,38 @@
 
 Quickstart
 ----------
 
 Installation
 ++++++++++++
 
-Simple installation using `conda <https://docs.conda.io/projects/conda/en/latest/user-guide/index.html>`__::
+Simple installation using `mamba <https://mamba.readthedocs.org/>`__::
 
-    conda install --channel conda-forge pygmt
+    mamba install --channel conda-forge pygmt
 
-If you use `mamba <https://mamba.readthedocs.org/>`__::
+If you use `conda <https://docs.conda.io/projects/conda/en/latest/user-guide/index.html>`__::
 
-    mamba install --channel conda-forge pygmt
+    conda install --channel conda-forge pygmt
 
 For other ways to install ``pygmt``, see `full installation instructions <https://www.pygmt.org/latest/install.html>`__.
 
+Getting started
++++++++++++++++
+
+As a starting point, you can open a `Python interpreter <https://docs.python.org/3/tutorial/interpreter.html>`__
+or a `Jupyter notebook <https://docs.jupyter.org/en/latest/running.html>`__, and try the following example::
+
+    import pygmt
+    fig = pygmt.Figure()
+    fig.coast(projection="H10c", region="g", frame=True, land="gray")
+    fig.show()
+
+For more examples, please have a look at the `Gallery <https://www.pygmt.org/latest/gallery/index.html>`__
+and `Tutorials <https://www.pygmt.org/latest/tutorials/index.html>`__.
+
 
 Contacting Us
 -------------
 
 * Most discussion happens `on GitHub
   <https://github.com/GenericMappingTools/pygmt>`__. Feel free to `open an issue
   <https://github.com/GenericMappingTools/pygmt/issues/new>`__ or comment on any
@@ -190,47 +206,49 @@
 PyGMT is a community developed project. See the
 `AUTHORS.md <https://github.com/GenericMappingTools/pygmt/blob/main/AUTHORS.md>`__
 file on GitHub for a list of the people involved and a definition of the term "PyGMT
 Developers". Feel free to cite our work in your research using the following BibTeX:
 
 .. code-block::
 
-    @software{pygmt_2022_7481934,
+    @software{pygmt_2023_7772533,
       author       = {Uieda, Leonardo and
                       Tian, Dongdong and
                       Leong, Wei Ji and
-                      Jones, Max and
                       Schlitzer, William and
                       Grund, Michael and
-                      Toney, Liam and
+                      Jones, Max and
                       Fröhlich, Yvonne and
+                      Toney, Liam and
                       Yao, Jiayuan and
                       Magen, Yohai and
+                      Tong, Jing-Hui and
                       Materna, Kathryn and
                       Belem, Andre and
                       Newton, Tyler and
                       Anant, Abhishek and
                       Ziebarth, Malte and
                       Quinn, Jamie and
                       Wessel, Paul},
       title        = {{PyGMT: A Python interface for the Generic Mapping Tools}},
-      month        = dec,
-      year         = 2022,
+      month        = mar,
+      year         = 2023,
       publisher    = {Zenodo},
-      version      = {0.8.0},
-      doi          = {10.5281/zenodo.7481934},
-      url          = {https://doi.org/10.5281/zenodo.7481934}
+      version      = {0.9.0},
+      doi          = {10.5281/zenodo.7772533},
+      url          = {https://doi.org/10.5281/zenodo.7772533}
     }
 
 To cite a specific version of PyGMT, go to our Zenodo page at
 https://doi.org/10.5281/zenodo.3781524 and use the "Export to BibTeX" function there.
 It is also strongly recommended to cite the
 `GMT6 paper <https://doi.org/10.1029/2019GC008515>`__ (which PyGMT wraps around).
-Note that some modules like ``surface`` and ``x2sys`` also have their dedicated citation.
-Further information for all these can be found at https://www.generic-mapping-tools.org/cite.
+Note that some modules like ``dimfilter``, ``surface``, and ``x2sys`` also have their
+dedicated citations. Further information for all these can be found at
+https://www.generic-mapping-tools.org/cite.
 
 
 License
 -------
 
 PyGMT is free software: you can redistribute it and/or modify it under the terms of
 the **BSD 3-clause License**. A copy of this license is provided in
@@ -271,16 +289,21 @@
       - GMT
       - Python
       - NumPy
     * - `Dev <https://github.com/GenericMappingTools/pygmt/milestones>`_ (upcoming release)
       - `Dev Documentation <https://www.pygmt.org/dev>`_ (reflects `main branch <https://github.com/GenericMappingTools/pygmt>`_)
       - >=6.3.0
       - >=3.8
-      - >=1.20
-    * - `v0.8.0 <https://github.com/GenericMappingTools/pygmt/releases/tag/v0.8.0>`_ (latest release)
+      - >=1.21
+    * - `v0.9.0 <https://github.com/GenericMappingTools/pygmt/releases/tag/v0.9.0>`_ (latest release)
+      - `v0.9.0 Documentation <https://www.pygmt.org/v0.9.0>`_
+      - >=6.3.0
+      - >=3.8
+      - >=1.21
+    * - `v0.8.0 <https://github.com/GenericMappingTools/pygmt/releases/tag/v0.8.0>`_
       - `v0.8.0 Documentation <https://www.pygmt.org/v0.8.0>`_
       - >=6.3.0
       - >=3.8
       - >=1.20
     * - `v0.7.0 <https://github.com/GenericMappingTools/pygmt/releases/tag/v0.7.0>`_
       - `v0.7.0 Documentation <https://www.pygmt.org/v0.7.0>`_
       - >=6.3.0
```

### Comparing `pygmt-0.8.0/README.rst` & `pygmt-0.9.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -51,30 +51,31 @@
 ----------
 
 A beautiful map is worth a thousand words.
 To truly understand how powerful PyGMT is, play with it online on `Binder <https://github.com/GenericMappingTools/try-gmt>`__!
 For a quicker introduction, check out our `3 minute overview <https://youtu.be/4iPnITXrxVU>`__!
 
 Afterwards, feel free to look at our `Tutorials <https://www.pygmt.org/latest/tutorials>`__,
-visit the `PyGMT Gallery <https://www.pygmt.org/latest/gallery>`__, and check out
+visit the `Gallery <https://www.pygmt.org/latest/gallery>`__, and check out
 some `external PyGMT examples <https://www.pygmt.org/latest/external_resources.html>`__!
 
 .. image:: https://user-images.githubusercontent.com/14077947/155809878-48b8f235-141b-460a-80ec-08bbf6c36e40.png
     :alt: Quick Introduction to PyGMT YouTube Video
     :align: center
     :target: https://youtu.be/4iPnITXrxVU
     :width: 80%
 
 About
 -----
 
 PyGMT is a library for processing geospatial and geophysical data and making
-publication quality maps and figures. It provides a Pythonic interface for the
+publication-quality maps and figures. It provides a Pythonic interface for the
 `Generic Mapping Tools (GMT) <https://github.com/GenericMappingTools/gmt>`__, a
-command-line program widely used in the Earth Sciences.
+command-line program widely used across the Earth, Ocean, and Planetary sciences
+and beyond.
 
 Project goals
 -------------
 
 * Make GMT more accessible to new users.
 * Build a Pythonic API for GMT.
 * Interface with the GMT C API directly using ctypes (no system calls).
@@ -87,24 +88,38 @@
 
 Quickstart
 ----------
 
 Installation
 ++++++++++++
 
-Simple installation using `conda <https://docs.conda.io/projects/conda/en/latest/user-guide/index.html>`__::
+Simple installation using `mamba <https://mamba.readthedocs.org/>`__::
 
-    conda install --channel conda-forge pygmt
+    mamba install --channel conda-forge pygmt
 
-If you use `mamba <https://mamba.readthedocs.org/>`__::
+If you use `conda <https://docs.conda.io/projects/conda/en/latest/user-guide/index.html>`__::
 
-    mamba install --channel conda-forge pygmt
+    conda install --channel conda-forge pygmt
 
 For other ways to install ``pygmt``, see `full installation instructions <https://www.pygmt.org/latest/install.html>`__.
 
+Getting started
++++++++++++++++
+
+As a starting point, you can open a `Python interpreter <https://docs.python.org/3/tutorial/interpreter.html>`__
+or a `Jupyter notebook <https://docs.jupyter.org/en/latest/running.html>`__, and try the following example::
+
+    import pygmt
+    fig = pygmt.Figure()
+    fig.coast(projection="H10c", region="g", frame=True, land="gray")
+    fig.show()
+
+For more examples, please have a look at the `Gallery <https://www.pygmt.org/latest/gallery/index.html>`__
+and `Tutorials <https://www.pygmt.org/latest/tutorials/index.html>`__.
+
 
 Contacting Us
 -------------
 
 * Most discussion happens `on GitHub
   <https://github.com/GenericMappingTools/pygmt>`__. Feel free to `open an issue
   <https://github.com/GenericMappingTools/pygmt/issues/new>`__ or comment on any
@@ -161,47 +176,49 @@
 PyGMT is a community developed project. See the
 `AUTHORS.md <https://github.com/GenericMappingTools/pygmt/blob/main/AUTHORS.md>`__
 file on GitHub for a list of the people involved and a definition of the term "PyGMT
 Developers". Feel free to cite our work in your research using the following BibTeX:
 
 .. code-block::
 
-    @software{pygmt_2022_7481934,
+    @software{pygmt_2023_7772533,
       author       = {Uieda, Leonardo and
                       Tian, Dongdong and
                       Leong, Wei Ji and
-                      Jones, Max and
                       Schlitzer, William and
                       Grund, Michael and
-                      Toney, Liam and
+                      Jones, Max and
                       Fröhlich, Yvonne and
+                      Toney, Liam and
                       Yao, Jiayuan and
                       Magen, Yohai and
+                      Tong, Jing-Hui and
                       Materna, Kathryn and
                       Belem, Andre and
                       Newton, Tyler and
                       Anant, Abhishek and
                       Ziebarth, Malte and
                       Quinn, Jamie and
                       Wessel, Paul},
       title        = {{PyGMT: A Python interface for the Generic Mapping Tools}},
-      month        = dec,
-      year         = 2022,
+      month        = mar,
+      year         = 2023,
       publisher    = {Zenodo},
-      version      = {0.8.0},
-      doi          = {10.5281/zenodo.7481934},
-      url          = {https://doi.org/10.5281/zenodo.7481934}
+      version      = {0.9.0},
+      doi          = {10.5281/zenodo.7772533},
+      url          = {https://doi.org/10.5281/zenodo.7772533}
     }
 
 To cite a specific version of PyGMT, go to our Zenodo page at
 https://doi.org/10.5281/zenodo.3781524 and use the "Export to BibTeX" function there.
 It is also strongly recommended to cite the
 `GMT6 paper <https://doi.org/10.1029/2019GC008515>`__ (which PyGMT wraps around).
-Note that some modules like ``surface`` and ``x2sys`` also have their dedicated citation.
-Further information for all these can be found at https://www.generic-mapping-tools.org/cite.
+Note that some modules like ``dimfilter``, ``surface``, and ``x2sys`` also have their
+dedicated citations. Further information for all these can be found at
+https://www.generic-mapping-tools.org/cite.
 
 
 License
 -------
 
 PyGMT is free software: you can redistribute it and/or modify it under the terms of
 the **BSD 3-clause License**. A copy of this license is provided in
@@ -242,16 +259,21 @@
       - GMT
       - Python
       - NumPy
     * - `Dev <https://github.com/GenericMappingTools/pygmt/milestones>`_ (upcoming release)
       - `Dev Documentation <https://www.pygmt.org/dev>`_ (reflects `main branch <https://github.com/GenericMappingTools/pygmt>`_)
       - >=6.3.0
       - >=3.8
-      - >=1.20
-    * - `v0.8.0 <https://github.com/GenericMappingTools/pygmt/releases/tag/v0.8.0>`_ (latest release)
+      - >=1.21
+    * - `v0.9.0 <https://github.com/GenericMappingTools/pygmt/releases/tag/v0.9.0>`_ (latest release)
+      - `v0.9.0 Documentation <https://www.pygmt.org/v0.9.0>`_
+      - >=6.3.0
+      - >=3.8
+      - >=1.21
+    * - `v0.8.0 <https://github.com/GenericMappingTools/pygmt/releases/tag/v0.8.0>`_
       - `v0.8.0 Documentation <https://www.pygmt.org/v0.8.0>`_
       - >=6.3.0
       - >=3.8
       - >=1.20
     * - `v0.7.0 <https://github.com/GenericMappingTools/pygmt/releases/tag/v0.7.0>`_
       - `v0.7.0 Documentation <https://www.pygmt.org/v0.7.0>`_
       - >=6.3.0
```

### Comparing `pygmt-0.8.0/pygmt/__init__.py` & `pygmt-0.9.0/pygmt/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 """
 PyGMT is a library for processing geospatial and geophysical data and making
-publication quality maps and figures. It provides a Pythonic interface for the
-Generic Mapping Tools (GMT), a command-line program widely used in the Earth
-Sciences. Besides making GMT more accessible to new users, PyGMT aims to
-provide integration with the PyData ecosystem as well as support for rich
-display in Jupyter notebooks.
+publication-quality maps and figures. It provides a Pythonic interface for the
+Generic Mapping Tools (GMT), a command-line program widely used across the
+Earth, Ocean, and Planetary sciences and beyond. Besides making GMT more
+accessible to new users, PyGMT aims to provide integration with the PyData
+ecosystem as well as support for rich display in Jupyter notebooks.
 
 Main Features
 -------------
 Here are just a few of the things that PyGMT does well:
 
   - Easy handling of individual types of data like Cartesian, geographic, or
     time-series data.
   - Processing of (geo)spatial data including gridding, filtering, and masking.
-  - Allows plotting of a large spectrum of objects on figures including
+  - Plotting of a large spectrum of objects on figures including
     lines, vectors, polygons, and symbols (pre-defined and customized).
-  - Generate publication-quality illustrations and make animations.
+  - Generating publication-quality illustrations and making animations.
 """
-
 import atexit as _atexit
+import sys
 from importlib.metadata import version
 
+from pygmt import clib
+
+# Get semantic version through setuptools-scm
+__version__ = f'v{version("pygmt")}'  # e.g. v0.1.2.dev3+g0ab3cd78
+__commit__ = __version__.split("+g")[-1] if "+g" in __version__ else ""  # 0ab3cd78
+with clib.Session() as lib:
+    __gmt_version__ = lib.info["version"]
+
 # Import modules to make the high-level GMT Python API
 from pygmt import datasets
 from pygmt.accessors import GMTDataArrayAccessor
 from pygmt.figure import Figure, set_display
 from pygmt.io import load_dataarray
 from pygmt.session_management import begin as _begin
 from pygmt.session_management import end as _end
@@ -62,55 +70,52 @@
     triangulate,
     which,
     x2sys_cross,
     x2sys_init,
     xyz2grd,
 )
 
-# Get semantic version through setuptools-scm
-__version__ = f'v{version("pygmt")}'  # e.g. v0.1.2.dev3+g0ab3cd78
-__commit__ = __version__.split("+g")[-1] if "+g" in __version__ else ""  # 0ab3cd78
-
 # Start our global modern mode session
 _begin()
 # Tell Python to run _end when shutting down
 _atexit.register(_end)
 
 
-def print_clib_info():
+def print_clib_info(file=sys.stdout):
     """
     Print information about the GMT shared library that we can find.
 
     Includes the GMT version, default values for parameters, the path to the
     ``libgmt`` shared library, and GMT directories.
     """
     from pygmt.clib import Session  # pylint: disable=import-outside-toplevel
 
     lines = ["GMT library information:"]
     with Session() as ses:
         for key in sorted(ses.info):
             lines.append(f"  {key}: {ses.info[key]}")
-    print("\n".join(lines))
+    print("\n".join(lines), file=file)
 
 
-def show_versions():
+def show_versions(file=sys.stdout):
     """
-    Prints various dependency versions useful when submitting bug reports. This
-    includes information about:
+    Print various dependency versions which are useful when submitting bug
+    reports.
+
+    This includes information about:
 
     - PyGMT itself
     - System information (Python version, Operating System)
     - Core dependency versions (NumPy, Pandas, Xarray, etc)
     - GMT library information
     """
     # pylint: disable=import-outside-toplevel
     import importlib
     import platform
     import subprocess
-    import sys
 
     def _get_module_version(modname):
         """
         Get version information of a Python module.
         """
         try:
             if modname in sys.modules:
@@ -148,42 +153,50 @@
 
     sys_info = {
         "python": sys.version.replace("\n", " "),
         "executable": sys.executable,
         "machine": platform.platform(),
     }
 
-    deps = ["numpy", "pandas", "xarray", "netCDF4", "packaging", "geopandas"]
+    deps = [
+        "numpy",
+        "pandas",
+        "xarray",
+        "netCDF4",
+        "packaging",
+        "contextily",
+        "geopandas",
+    ]
 
-    print("PyGMT information:")
-    print(f"  version: {__version__}")
+    print("PyGMT information:", file=file)
+    print(f"  version: {__version__}", file=file)
 
-    print("System information:")
+    print("System information:", file=file)
     for key, val in sys_info.items():
-        print(f"  {key}: {val}")
+        print(f"  {key}: {val}", file=file)
 
-    print("Dependency information:")
+    print("Dependency information:", file=file)
     for modname in deps:
-        print(f"  {modname}: {_get_module_version(modname)}")
-    print(f"  ghostscript: {_get_ghostscript_version()}")
+        print(f"  {modname}: {_get_module_version(modname)}", file=file)
+    print(f"  ghostscript: {_get_ghostscript_version()}", file=file)
 
-    print_clib_info()
+    print_clib_info(file=file)
 
 
 def test(doctest=True, verbose=True, coverage=False, figures=True):
     """
     Run the test suite.
 
     Uses `pytest <http://pytest.org/>`__ to discover and run the tests. If you
-    haven't already, you can install it with `conda
-    <http://conda.pydata.org/>`__ or `pip <https://pip.pypa.io/en/stable/>`__.
+    haven't already, you can install it with `mamba
+    <https://mamba.readthedocs.org/>`__ or `pip
+    <https://pip.pypa.io/en/stable/>`__.
 
     Parameters
     ----------
-
     doctest : bool
         If ``True``, will run the doctests as well (code examples that start
         with a ``>>>`` in the docs).
     verbose : bool
         If ``True``, will print extra information during the test run.
     coverage : bool
         If ``True``, will run test coverage analysis on the code as well.
```

### Comparing `pygmt-0.8.0/pygmt/clib/conversion.py` & `pygmt-0.9.0/pygmt/clib/conversion.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import numpy as np
 import pandas as pd
 from pygmt.exceptions import GMTInvalidInput
 
 
 def dataarray_to_matrix(grid):
     """
-    Transform an xarray.DataArray into a data 2D array and metadata.
+    Transform an xarray.DataArray into a data 2-D array and metadata.
 
     Use this to extract the underlying numpy array of data and the region and
     increment for the grid.
 
     Only allows grids with two dimensions and constant grid spacing (GMT
     doesn't allow variable grid spacing). If the latitude and/or longitude
     increments of the input grid are negative, the output matrix will be
@@ -27,16 +27,16 @@
     ----------
     grid : xarray.DataArray
         The input grid as a DataArray instance. Information is retrieved from
         the coordinate arrays, not from headers.
 
     Returns
     -------
-    matrix : 2d-array
-        The 2D array of data from the grid.
+    matrix : 2-D array
+        The 2-D array of data from the grid.
     region : list
         The West, East, South, North boundaries of the grid.
     inc : list
         The grid spacing in East-West and North-South, respectively.
 
     Raises
     ------
@@ -123,32 +123,32 @@
 
     matrix = as_c_contiguous(grid[::-1].values)
     return matrix, region, inc
 
 
 def vectors_to_arrays(vectors):
     """
-    Convert 1d vectors (lists, arrays or pandas.Series) to C contiguous 1d
+    Convert 1-D vectors (lists, arrays, or pandas.Series) to C contiguous 1-D
     arrays.
 
     Arrays must be in C contiguous order for us to pass their memory pointers
     to GMT. If any are not, convert them to C order (which requires copying the
-    memory). This usually happens when vectors are columns of a 2d array or
+    memory). This usually happens when vectors are columns of a 2-D array or
     have been sliced.
 
     If a vector is a list or pandas.Series, get the underlying numpy array.
 
     Parameters
     ----------
-    vectors : list of lists, 1d arrays or pandas.Series
+    vectors : list of lists, 1-D arrays, or pandas.Series
         The vectors that must be converted.
 
     Returns
     -------
-    arrays : list of 1d arrays
+    arrays : list of 1-D arrays
         The converted numpy arrays
 
     Examples
     --------
 
     >>> import numpy as np
     >>> import pandas as pd
@@ -175,20 +175,20 @@
     """
     Ensure a numpy array is C contiguous in memory.
 
     If the array is not C contiguous, a copy will be necessary.
 
     Parameters
     ----------
-    array : 1d array
+    array : 1-D array
         The numpy array
 
     Returns
     -------
-    array : 1d array
+    array : 1-D array
         Array is C contiguous order.
 
     Examples
     --------
 
     >>> import numpy as np
     >>> data = np.array([[1, 2], [3, 4], [5, 6]])
@@ -248,35 +248,35 @@
     if argument in kwargs:
         return dtype(*kwargs[argument])
     return None
 
 
 def array_to_datetime(array):
     """
-    Convert an 1d datetime array from various types into pandas.DatetimeIndex
+    Convert an 1-D datetime array from various types into pandas.DatetimeIndex
     (i.e., numpy.datetime64).
 
     If the input array is not in legal datetime formats, raise a "ParseError"
     exception.
 
     Parameters
     ----------
-    array : list or 1d array
+    array : list or 1-D array
         The input datetime array in various formats.
 
         Supported types:
 
         - str
         - numpy.datetime64
         - pandas.DateTimeIndex
         - datetime.datetime and datetime.date
 
     Returns
     -------
-    array : 1d datetime array in pandas.DatetimeIndex (i.e., numpy.datetime64)
+    array : 1-D datetime array in pandas.DatetimeIndex (i.e., numpy.datetime64)
 
     Examples
     --------
     >>> import datetime
     >>> # numpy.datetime64 array
     >>> x = np.array(
     ...     ["2010-06-01", "2011-06-01T12", "2012-01-01T12:34:56"],
```

### Comparing `pygmt-0.8.0/pygmt/clib/loading.py` & `pygmt-0.9.0/pygmt/clib/loading.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/clib/session.py` & `pygmt-0.9.0/pygmt/clib/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,33 +24,46 @@
     GMTCLibNoSessionError,
     GMTInvalidInput,
     GMTVersionError,
 )
 from pygmt.helpers import data_kind, dummy_context, fmt_docstring, tempfile_from_geojson
 
 FAMILIES = [
-    "GMT_IS_DATASET",
-    "GMT_IS_GRID",
-    "GMT_IS_PALETTE",
-    "GMT_IS_MATRIX",
-    "GMT_IS_VECTOR",
+    "GMT_IS_DATASET",  # Entity is a data table
+    "GMT_IS_GRID",  # Entity is a grid
+    "GMT_IS_IMAGE",  # Entity is a 1- or 3-band unsigned char image
+    "GMT_IS_PALETTE",  # Entity is a color palette table
+    "GMT_IS_POSTSCRIPT",  # Entity is a PostScript content struct
+    "GMT_IS_MATRIX",  # Entity is a user matrix
+    "GMT_IS_VECTOR",  # Entity is a set of user vectors
+    "GMT_IS_CUBE",  # Entity is a 3-D data cube
 ]
 
-VIAS = ["GMT_VIA_MATRIX", "GMT_VIA_VECTOR"]
+VIAS = [
+    "GMT_VIA_MATRIX",  # dataset is passed as a matrix
+    "GMT_VIA_VECTOR",  # dataset is passed as a set of vectors
+]
 
 GEOMETRIES = [
-    "GMT_IS_NONE",
-    "GMT_IS_POINT",
-    "GMT_IS_LINE",
-    "GMT_IS_POLYGON",
-    "GMT_IS_PLP",
-    "GMT_IS_SURFACE",
+    "GMT_IS_NONE",  # items without geometry (e.g., CPT)
+    "GMT_IS_POINT",  # items are points
+    "GMT_IS_LINE",  # items are lines
+    "GMT_IS_POLY",  # items are polygons
+    "GMT_IS_LP",  # items could be any one of LINE or POLY
+    "GMT_IS_PLP",  # items could be any one of POINT, LINE, or POLY
+    "GMT_IS_SURFACE",  # items are 2-D grid
+    "GMT_IS_VOLUME",  # items are 3-D grid
+]
+
+METHODS = [
+    "GMT_IS_DUPLICATE",  # tell GMT the data are read-only
+    "GMT_IS_REFERENCE",  # tell GMT to duplicate the data
 ]
 
-METHODS = ["GMT_IS_DUPLICATE", "GMT_IS_REFERENCE"]
+DIRECTIONS = ["GMT_IN", "GMT_OUT"]
 
 MODES = ["GMT_CONTAINER_ONLY", "GMT_IS_OUTPUT"]
 
 REGISTRATIONS = ["GMT_GRID_PIXEL_REG", "GMT_GRID_NODE_REG"]
 
 DTYPES = {
     np.int8: "GMT_CHAR",
@@ -162,18 +175,24 @@
                 # "binary dir": self.get_default("API_BINDIR"),
                 "share dir": self.get_default("API_SHAREDIR"),
                 # This segfaults for some reason
                 # 'data dir': self.get_default("API_DATADIR"),
                 "plugin dir": self.get_default("API_PLUGINDIR"),
                 "library path": self.get_default("API_LIBRARY"),
                 "cores": self.get_default("API_CORES"),
-                # API_IMAGE_LAYOUT not defined if GMT is not compiled with GDAL
-                # "image layout": self.get_default("API_IMAGE_LAYOUT"),
                 "grid layout": self.get_default("API_GRID_LAYOUT"),
             }
+            # For GMT<6.4.0, API_IMAGE_LAYOUT is not defined if GMT is not
+            # compiled with GDAL. Since GMT 6.4.0, GDAL is a required GMT
+            # dependency. The try-except block can be refactored after we bump
+            # the minimum required GMT version to 6.4.0.
+            try:
+                self._info["image layout"] = self.get_default("API_IMAGE_LAYOUT")
+            except GMTCLibError:
+                pass
             # API_BIN_VERSION is new in GMT 6.4.0.
             if Version(self._info["version"]) >= Version("6.4.0"):
                 self._info["binary version"] = self.get_default("API_BIN_VERSION")
         return self._info
 
     def __enter__(self):
         """
@@ -426,24 +445,25 @@
 
     def get_default(self, name):
         """
         Get the value of a GMT default parameter (library version, paths, etc).
 
         Possible default parameter names include:
 
-        * ``"API_VERSION"``: The GMT version
+        * ``"API_VERSION"``: The GMT API version
         * ``"API_PAD"``: The grid padding setting
         * ``"API_BINDIR"``: The binary file directory
         * ``"API_SHAREDIR"``: The share directory
         * ``"API_DATADIR"``: The data directory
         * ``"API_PLUGINDIR"``: The plugin directory
         * ``"API_LIBRARY"``: The core library path
         * ``"API_CORES"``: The number of cores
         * ``"API_IMAGE_LAYOUT"``: The image/band layout
         * ``"API_GRID_LAYOUT"``: The grid layout
+        * ``"API_BIN_VERSION"``: The GMT binary version (with git information)
 
         Parameters
         ----------
         name : str
             The name of the default parameter (e.g., ``"API_VERSION"``)
 
         Returns
@@ -673,34 +693,34 @@
                 f"Invalid constant modifier '{parts[1]}'. Must be one of {str(valid_modifiers)}."
             )
         integer_value = sum(self[part] for part in parts)
         return integer_value
 
     def _check_dtype_and_dim(self, array, ndim):
         """
-        Check that a numpy array has the given dimensions and is a valid data
-        type.
+        Check that a numpy array has the given number of dimensions and is a
+        valid data type.
 
         Parameters
         ----------
-        array : numpy array
+        array : numpy.ndarray
             The array to be tested.
         ndim : int
-            The desired dimension of the array.
+            The desired number of array dimensions.
 
         Returns
         -------
         gmt_type : int
             The GMT constant value representing this data type.
 
         Raises
         ------
-        GMTCLibError
-            If the array has the wrong dimensions or is an unsupported data
-            type.
+        GMTInvalidInput
+            If the array has the wrong number of dimensions or
+            is an unsupported data type.
 
         Examples
         --------
 
         >>> import numpy as np
         >>> data = np.array([1, 2, 3], dtype="float64")
         >>> with Session() as ses:
@@ -711,64 +731,66 @@
         >>> data = np.ones((5, 2), dtype="float32")
         >>> with Session() as ses:
         ...     gmttype = ses._check_dtype_and_dim(data, ndim=2)
         ...     gmttype == ses["GMT_FLOAT"]
         ...
         True
         """
-        # check the array has the given dimension
+        # Check that the array has the given number of dimensions
         if array.ndim != ndim:
-            raise GMTInvalidInput(f"Expected a numpy 1d array, got {array.ndim}d.")
+            raise GMTInvalidInput(
+                f"Expected a numpy {ndim}-D array, got {array.ndim}-D."
+            )
 
-        # check the array has a valid/known data type
+        # Check that the array has a valid/known data type
         if array.dtype.type not in DTYPES:
             try:
                 # Try to convert any unknown numpy data types to np.datetime64
                 array = np.asarray(array, dtype=np.datetime64)
             except ValueError as e:
                 raise GMTInvalidInput(
                     f"Unsupported numpy data type '{array.dtype.type}'."
                 ) from e
         return self[DTYPES[array.dtype.type]]
 
     def put_vector(self, dataset, column, vector):
         r"""
-        Attach a numpy 1D array as a column on a GMT dataset.
+        Attach a numpy 1-D array as a column on a GMT dataset.
 
         Use this function to attach numpy array data to a GMT dataset and pass
         it to GMT modules. Wraps ``GMT_Put_Vector``.
 
         The dataset must be created by :meth:`pygmt.clib.Session.create_data`
         first. Use ``family='GMT_IS_DATASET|GMT_VIA_VECTOR'``.
 
         Not all numpy dtypes are supported, only: int8, int16, int32, int64,
-        uint8, uint16, uint32, uint64, float32, float64, str\_ and datetime64.
+        uint8, uint16, uint32, uint64, float32, float64, str\_, and datetime64.
 
         .. warning::
             The numpy array must be C contiguous in memory. If it comes from a
-            column slice of a 2d array, for example, you will have to make a
+            column slice of a 2-D array, for example, you will have to make a
             copy. Use :func:`numpy.ascontiguousarray` to make sure your vector
             is contiguous (it won't copy if it already is).
 
         Parameters
         ----------
         dataset : :class:`ctypes.c_void_p`
             The ctypes void pointer to a ``GMT_Dataset``. Create it with
             :meth:`pygmt.clib.Session.create_data`.
         column : int
             The column number of this vector in the dataset (starting from 0).
-        vector : numpy 1d-array
-            The array that will be attached to the dataset. Must be a 1d C
+        vector : numpy 1-D array
+            The array that will be attached to the dataset. Must be a 1-D C
             contiguous array.
 
         Raises
         ------
         GMTCLibError
-            If given invalid input or ``GMT_Put_Vector`` exits with status !=
-            0.
+            If given invalid input or ``GMT_Put_Vector`` exits with
+            status != 0.
         """
         c_put_vector = self.get_libgmt_func(
             "GMT_Put_Vector",
             argtypes=[ctp.c_void_p, ctp.c_void_p, ctp.c_uint, ctp.c_uint, ctp.c_void_p],
             restype=ctp.c_int,
         )
 
@@ -792,45 +814,45 @@
                     f"Failed to put vector of type {vector.dtype} "
                     f"in column {column} of dataset."
                 )
             )
 
     def put_strings(self, dataset, family, strings):
         """
-        Attach a numpy 1D array of dtype str as a column on a GMT dataset.
+        Attach a numpy 1-D array of dtype str as a column on a GMT dataset.
 
         Use this function to attach string type numpy array data to a GMT
         dataset and pass it to GMT modules. Wraps ``GMT_Put_Strings``.
 
         The dataset must be created by :meth:`pygmt.clib.Session.create_data`
         first.
 
         .. warning::
             The numpy array must be C contiguous in memory. If it comes from a
-            column slice of a 2d array, for example, you will have to make a
+            column slice of a 2-D array, for example, you will have to make a
             copy. Use :func:`numpy.ascontiguousarray` to make sure your vector
             is contiguous (it won't copy if it already is).
 
         Parameters
         ----------
         dataset : :class:`ctypes.c_void_p`
             The ctypes void pointer to a ``GMT_Dataset``. Create it with
             :meth:`pygmt.clib.Session.create_data`.
         family : str
             The family type of the dataset. Can be either ``GMT_IS_VECTOR`` or
             ``GMT_IS_MATRIX``.
-        strings : numpy 1d-array
-            The array that will be attached to the dataset. Must be a 1d C
+        strings : numpy 1-D array
+            The array that will be attached to the dataset. Must be a 1-D C
             contiguous array.
 
         Raises
         ------
         GMTCLibError
-            If given invalid input or ``GMT_Put_Strings`` exits with status !=
-            0.
+            If given invalid input or ``GMT_Put_Strings`` exits with
+            status != 0.
         """
         c_put_strings = self.get_libgmt_func(
             "GMT_Put_Strings",
             argtypes=[
                 ctp.c_void_p,
                 ctp.c_uint,
                 ctp.c_void_p,
@@ -852,47 +874,47 @@
         if status != 0:
             raise GMTCLibError(
                 f"Failed to put strings of type {strings.dtype} into dataset"
             )
 
     def put_matrix(self, dataset, matrix, pad=0):
         """
-        Attach a numpy 2D array to a GMT dataset.
+        Attach a numpy 2-D array to a GMT dataset.
 
         Use this function to attach numpy array data to a GMT dataset and pass
         it to GMT modules. Wraps ``GMT_Put_Matrix``.
 
         The dataset must be created by :meth:`pygmt.clib.Session.create_data`
         first. Use ``|GMT_VIA_MATRIX'`` in the family.
 
         Not all numpy dtypes are supported, only: int8, int16, int32, int64,
-        uint8, uint16, uint32, uint64, float32 and float64.
+        uint8, uint16, uint32, uint64, float32, and float64.
 
         .. warning::
             The numpy array must be C contiguous in memory. Use
             :func:`numpy.ascontiguousarray` to make sure your vector is
             contiguous (it won't copy if it already is).
 
         Parameters
         ----------
         dataset : :class:`ctypes.c_void_p`
             The ctypes void pointer to a ``GMT_Dataset``. Create it with
             :meth:`pygmt.clib.Session.create_data`.
-        matrix : numpy 2d-array
-            The array that will be attached to the dataset. Must be a 2d C
+        matrix : numpy 2-D array
+            The array that will be attached to the dataset. Must be a 2-D C
             contiguous array.
         pad : int
             The amount of padding that should be added to the matrix. Use when
             creating grids for modules that require padding.
 
         Raises
         ------
         GMTCLibError
-            If given invalid input or ``GMT_Put_Matrix`` exits with status !=
-            0.
+            If given invalid input or ``GMT_Put_Matrix`` exits with
+            status != 0.
         """
         c_put_matrix = self.get_libgmt_func(
             "GMT_Put_Matrix",
             argtypes=[ctp.c_void_p, ctp.c_void_p, ctp.c_uint, ctp.c_int, ctp.c_void_p],
             restype=ctp.c_int,
         )
 
@@ -972,52 +994,53 @@
         )
         if status != 0:
             raise GMTCLibError(f"Failed to write dataset to '{output}'")
 
     @contextmanager
     def open_virtual_file(self, family, geometry, direction, data):
         """
-        Open a GMT Virtual File to pass data to and from a module.
+        Open a GMT virtual file to pass data to and from a module.
 
-        GMT uses a virtual file scheme to pass in data to API modules. Use it
-        to pass in your GMT data structure (created using
+        GMT uses a virtual file scheme to pass in data or get data from API
+        modules. Use it to pass in your GMT data structure (created using
         :meth:`pygmt.clib.Session.create_data`) to a module that expects an
-        input or output file.
+        input file, or get the output from a module that writes to a file.
 
         Use in a ``with`` block. Will automatically close the virtual file when
         leaving the ``with`` block. Because of this, no wrapper for
         ``GMT_Close_VirtualFile`` is provided.
 
         Parameters
         ----------
         family : str
-            A valid GMT data family name (e.g., ``'GMT_IS_DATASET'``). Should
+            A valid GMT data family name (e.g., ``"GMT_IS_DATASET"``). Should
             be the same as the one you used to create your data structure.
         geometry : str
-            A valid GMT data geometry name (e.g., ``'GMT_IS_POINT'``). Should
+            A valid GMT data geometry name (e.g., ``"GMT_IS_POINT"``). Should
             be the same as the one you used to create your data structure.
         direction : str
-            Either ``'GMT_IN'`` or ``'GMT_OUT'`` to indicate if passing data to
+            Either ``"GMT_IN"`` or ``"GMT_OUT"`` to indicate if passing data to
             GMT or getting it out of GMT, respectively.
             By default, GMT can modify the data you pass in. Add modifier
-            ``'GMT_IS_REFERENCE'`` to tell GMT the data are read-only, or
-            ``'GMT_IS_DUPLICATE'`` to tell GMT to duplicate the data.
-        data : int
-            The ctypes void pointer to your GMT data structure.
+            ``"GMT_IS_REFERENCE"`` to tell GMT the data are read-only, or
+            ``"GMT_IS_DUPLICATE"`` to tell GMT to duplicate the data.
+        data : int or None
+            The ctypes void pointer to your GMT data structure. For output
+            (i.e., ``direction="GMT_OUT"``), it can be ``None`` to have GMT
+            automatically allocate the output GMT data structure.
 
         Yields
         ------
         vfname : str
             The name of the virtual file that you can pass to a GMT module.
 
         Examples
         --------
 
         >>> from pygmt.helpers import GMTTempFile
-        >>> import os
         >>> import numpy as np
         >>> x = np.array([0, 1, 2, 3, 4])
         >>> y = np.array([5, 6, 7, 8, 9])
         >>> with Session() as lib:
         ...     family = "GMT_IS_DATASET|GMT_VIA_VECTOR"
         ...     geometry = "GMT_IS_POINT"
         ...     dataset = lib.create_data(
@@ -1057,59 +1080,56 @@
             argtypes=[ctp.c_void_p, ctp.c_char_p],
             restype=ctp.c_int,
         )
 
         family_int = self._parse_constant(family, valid=FAMILIES, valid_modifiers=VIAS)
         geometry_int = self._parse_constant(geometry, valid=GEOMETRIES)
         direction_int = self._parse_constant(
-            direction, valid=["GMT_IN", "GMT_OUT"], valid_modifiers=METHODS
+            direction, valid=DIRECTIONS, valid_modifiers=METHODS
         )
 
         buff = ctp.create_string_buffer(self["GMT_VF_LEN"])
-
         status = c_open_virtualfile(
             self.session_pointer, family_int, geometry_int, direction_int, data, buff
         )
-
         if status != 0:
             raise GMTCLibError("Failed to create a virtual file.")
 
         vfname = buff.value.decode()
-
         try:
             yield vfname
         finally:
             status = c_close_virtualfile(self.session_pointer, vfname.encode())
             if status != 0:
                 raise GMTCLibError(f"Failed to close virtual file '{vfname}'.")
 
     @contextmanager
     def virtualfile_from_vectors(self, *vectors):
         """
-        Store 1d arrays as columns of a table inside a virtual file.
+        Store 1-D arrays as columns of a table inside a virtual file.
 
         Use the virtual file name to pass in the data in your vectors to a GMT
         module.
 
         Context manager (use in a ``with`` block). Yields the virtual file name
         that you can pass as an argument to a GMT module call. Closes the
         virtual file upon exit of the ``with`` block.
 
         Use this instead of creating the data container and virtual file by
         hand with :meth:`pygmt.clib.Session.create_data`,
         :meth:`pygmt.clib.Session.put_vector`, and
         :meth:`pygmt.clib.Session.open_virtual_file`.
 
         If the arrays are C contiguous blocks of memory, they will be passed
-        without copying to GMT. If they are not (e.g., they are columns of a 2D
-        array), they will need to be copied to a contiguous block.
+        without copying to GMT. If they are not (e.g., they are columns of a
+        2-D array), they will need to be copied to a contiguous block.
 
         Parameters
         ----------
-        vectors : 1d arrays
+        vectors : 1-D arrays
             The vectors that will be included in the array. All must be of the
             same size.
 
         Yields
         ------
         fname : str
             The name of virtual file. Pass this as a file name argument to a
@@ -1185,15 +1205,15 @@
             family, geometry, "GMT_IN|GMT_IS_REFERENCE", dataset
         ) as vfile:
             yield vfile
 
     @contextmanager
     def virtualfile_from_matrix(self, matrix):
         """
-        Store a 2d array as a table inside a virtual file.
+        Store a 2-D array as a table inside a virtual file.
 
         Use the virtual file name to pass in the data in your matrix to a GMT
         module.
 
         Context manager (use in a ``with`` block). Yields the virtual file name
         that you can pass as an argument to a GMT module call. Closes the
         virtual file upon exit of the ``with`` block.
@@ -1211,15 +1231,15 @@
         :meth:`pygmt.clib.Session.open_virtual_file`
 
         The matrix must be C contiguous in memory. If it is not (e.g., it is a
         slice of a larger array), the array will be copied to make sure it is.
 
         Parameters
         ----------
-        matrix : 2d array
+        matrix : 2-D array
             The matrix that will be included in the GMT data container.
 
         Yields
         ------
         fname : str
             The name of virtual file. Pass this as a file name argument to a
             GMT module.
@@ -1371,24 +1391,24 @@
         into it, and produces a virtualfile that can be passed into GMT later
         on.
 
         Parameters
         ----------
         check_kind : str
             Used to validate the type of data that can be passed in. Choose
-            from 'raster', 'vector' or None. Default is None (no validation).
+            from 'raster', 'vector', or None. Default is None (no validation).
         data : str or pathlib.Path or xarray.DataArray or {table-like} or None
             Any raster or vector data format. This could be a file name or
             path, a raster grid, a vector matrix/arrays, or other supported
             data input.
-        x/y/z : 1d arrays or None
-            x, y and z columns as numpy arrays.
-        extra_arrays : list of 1d arrays
-            Optional. A list of numpy arrays in addition to x, y and z. All
-            of these arrays must be of the same size as the x/y/z arrays.
+        x/y/z : 1-D arrays or None
+            x, y, and z columns as numpy arrays.
+        extra_arrays : list of 1-D arrays
+            Optional. A list of numpy arrays in addition to x, y, and z.
+            All of these arrays must be of the same size as the x/y/z arrays.
         required_z : bool
             State whether the 'z' column is required.
 
         Returns
         -------
         file_context : contextlib._GeneratorContextManager
             The virtual file stored inside a context manager. Access the file
@@ -1449,30 +1469,31 @@
             _data = (str(data),)
         elif kind == "vectors":
             _data = [np.atleast_1d(x), np.atleast_1d(y)]
             if z is not None:
                 _data.append(np.atleast_1d(z))
             if extra_arrays:
                 _data.extend(extra_arrays)
-        elif kind == "matrix":  # turn 2D arrays into list of vectors
+        elif kind == "matrix":  # turn 2-D arrays into list of vectors
             try:
-                # pandas.Series will be handled below like a 1d numpy ndarray
+                # pandas.Series will be handled below like a 1-D numpy.ndarray
                 assert not hasattr(data, "to_frame")
                 # pandas.DataFrame and xarray.Dataset types
                 _data = [array for _, array in data.items()]
             except (AttributeError, AssertionError):
                 try:
-                    # Just use virtualfile_from_matrix for 2D numpy.ndarray
+                    # Just use virtualfile_from_matrix for 2-D numpy.ndarray
                     # which are signed integer (i), unsigned integer (u) or
                     # floating point (f) types
                     assert data.ndim == 2 and data.dtype.kind in "iuf"
                     _virtualfile_from = self.virtualfile_from_matrix
                     _data = (data,)
                 except (AssertionError, AttributeError):
-                    # Python list, tuple, numpy ndarray and pandas.Series types
+                    # Python list, tuple, numpy.ndarray, and pandas.Series
+                    # types
                     _data = np.atleast_2d(np.asanyarray(data).T)
 
         # Finally create the virtualfile from the data, to be passed into GMT
         file_context = _virtualfile_from(*_data)
 
         return file_context
 
@@ -1481,16 +1502,16 @@
         Extract the WESN bounding box of the currently active figure.
 
         Retrieves the information from the PostScript file, so it works for
         country codes as well.
 
         Returns
         -------
-        * wesn : 1d array
-            A 1D numpy array with the west, east, south, and north dimensions
+        * wesn : 1-D array
+            A numpy 1-D array with the west, east, south, and north dimensions
             of the current figure.
 
         Examples
         --------
 
         >>> import pygmt
         >>> fig = pygmt.Figure()
```

### Comparing `pygmt-0.8.0/pygmt/datasets/__init__.py` & `pygmt-0.9.0/pygmt/datasets/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,17 @@
-# pylint: disable=missing-docstring
-#
-# Load sample data included with GMT (downloaded from the GMT cache server).
+"""
+Functions to load GMT remote data and sample data.
+
+Data are downloaded from the GMT data server.
+"""
 
 from pygmt.datasets.earth_age import load_earth_age
 from pygmt.datasets.earth_free_air_anomaly import load_earth_free_air_anomaly
 from pygmt.datasets.earth_geoid import load_earth_geoid
 from pygmt.datasets.earth_magnetic_anomaly import load_earth_magnetic_anomaly
+from pygmt.datasets.earth_mask import load_earth_mask
 from pygmt.datasets.earth_relief import load_earth_relief
 from pygmt.datasets.earth_vertical_gravity_gradient import (
     load_earth_vertical_gravity_gradient,
 )
-from pygmt.datasets.samples import (
-    list_sample_data,
-    load_fractures_compilation,
-    load_hotspots,
-    load_japan_quakes,
-    load_mars_shape,
-    load_ocean_ridge_points,
-    load_sample_bathymetry,
-    load_sample_data,
-    load_usgs_quakes,
-)
+from pygmt.datasets.samples import list_sample_data, load_sample_data
+from pygmt.datasets.tile_map import load_tile_map
```

### Comparing `pygmt-0.8.0/pygmt/datasets/earth_age.py` & `pygmt-0.9.0/pygmt/datasets/earth_age.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,17 +50,22 @@
     -------
     grid : :class:`xarray.DataArray`
         The Earth seafloor crustal age grid. Coordinates are latitude and
         longitude in degrees. Age is in millions of years (Myr).
 
     Note
     ----
-    The :class:`xarray.DataArray` grid doesn't support slice operation, for
-    Earth seafloor crustal age with resolutions of 5 arc-minutes or higher,
-    which are stored as smaller tiles.
+    The registration and coordinate system type of the returned
+    :class:`xarray.DataArray` grid can be accessed via the GMT accessors
+    (i.e., ``grid.gmt.registration`` and ``grid.gmt.gtype`` respectively).
+    However, these properties may be lost after specific grid operations (such
+    as slicing) and will need to be manually set before passing the grid to any
+    PyGMT data processing or plotting functions. Refer to
+    :class:`pygmt.GMTDataArrayAccessor` for detailed explanations and
+    workarounds.
 
     Examples
     --------
 
     >>> from pygmt.datasets import load_earth_age
     >>> # load the default grid (gridline-registered 1 arc-degree grid)
     >>> grid = load_earth_age()
@@ -69,17 +74,15 @@
     >>> # load high-resolution (5 arc-minutes) grid for a specific region
     >>> grid = load_earth_age(
     ...     resolution="05m",
     ...     region=[120, 160, 30, 60],
     ...     registration="gridline",
     ... )
     """
-    dataset_prefix = "earth_age_"
-    dataset_name = "earth_age"
     grid = _load_remote_dataset(
-        dataset_name=dataset_name,
-        dataset_prefix=dataset_prefix,
+        dataset_name="earth_age",
+        dataset_prefix="earth_age_",
         resolution=resolution,
         region=region,
         registration=registration,
     )
     return grid
```

### Comparing `pygmt-0.8.0/pygmt/datasets/earth_free_air_anomaly.py` & `pygmt-0.9.0/pygmt/datasets/earth_vertical_gravity_gradient.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 """
-Function to download the IGPP Global Earth Free-Air Anomaly datasets from the
+Function to download the IGPP Global Earth Vertical Gravity Gradient from the
 GMT data server, and load as :class:`xarray.DataArray`.
 
 The grids are available in various resolutions.
 """
 from pygmt.datasets.load_remote_dataset import _load_remote_dataset
 from pygmt.helpers import kwargs_to_strings
 
-__doctest_skip__ = ["load_earth_free_air_anomaly"]
+__doctest_skip__ = ["load_earth_vertical_gravity_gradient"]
 
 
 @kwargs_to_strings(region="sequence")
-def load_earth_free_air_anomaly(resolution="01d", region=None, registration=None):
+def load_earth_vertical_gravity_gradient(
+    resolution="01d", region=None, registration=None
+):
     r"""
-    Load an Earth Free-Air Anomaly grid in various resolutions.
+    Load the IGPP Global Earth Vertical Gravity Gradient in various
+    resolutions.
 
     The grids are downloaded to a user data directory
-    (usually ``~/.gmt/server/earth/earth_faa/``) the first time you invoke
+    (usually ``~/.gmt/server/earth/earth_vgg/``) the first time you invoke
     this function. Afterwards, it will load the grid from the data directory.
     So you'll need an internet connection the first time around.
 
     These grids can also be accessed by passing in the file name
-    **@earth_faa**\_\ *res*\[_\ *reg*] to any grid plotting/processing
+    **@earth_vgg**\_\ *res*\[_\ *reg*] to any grid plotting/processing
     function. *res* is the grid resolution (see below), and *reg* is grid
     registration type (**p** for pixel registration or **g** for gridline
     registration).
 
-    Refer to :gmt-datasets:`earth-faa.html` for more details.
+    Refer to :gmt-datasets:`earth-vgg.html` for more details.
 
     Parameters
     ----------
     resolution : str
         The grid resolution. The suffix ``d`` and ``m`` stand for
         arc-degrees and arc-minutes. It can be ``"01d"``, ``"30m"``,
         ``"20m"``, ``"15m"``, ``"10m"``, ``"06m"``, ``"05m"``, ``"04m"``,
@@ -46,41 +49,46 @@
         Grid registration type. Either ``"pixel"`` for pixel registration or
         ``"gridline"`` for gridline registration. Default is ``"gridline"``
         for all resolutions except ``"01m"`` which is ``"pixel"`` only.
 
     Returns
     -------
     grid : :class:`xarray.DataArray`
-        The Earth free-air anomaly grid. Coordinates are latitude and
-        longitude in degrees. Units are in mGal.
+        The Earth vertical gravity gradient grid. Coordinates are latitude and
+        longitude in degrees. Units are in Eotvos.
 
     Note
     ----
-    The :class:`xarray.DataArray` grid doesn't support slice operation, for
-    Earth free-air anomaly with resolutions of 5 arc-minutes or higher,
-    which are stored as smaller tiles.
+    The registration and coordinate system type of the returned
+    :class:`xarray.DataArray` grid can be accessed via the GMT accessors
+    (i.e., ``grid.gmt.registration`` and ``grid.gmt.gtype`` respectively).
+    However, these properties may be lost after specific grid operations (such
+    as slicing) and will need to be manually set before passing the grid to any
+    PyGMT data processing or plotting functions. Refer to
+    :class:`pygmt.GMTDataArrayAccessor` for detailed explanations and
+    workarounds.
 
     Examples
     --------
 
-    >>> from pygmt.datasets import load_earth_free_air_anomaly
+    >>> from pygmt.datasets import load_earth_vertical_gravity_gradient
     >>> # load the default grid (gridline-registered 1 arc-degree grid)
-    >>> grid = load_earth_free_air_anomaly()
+    >>> grid = load_earth_vertical_gravity_gradient()
     >>> # load the 30 arc-minutes grid with "gridline" registration
-    >>> grid = load_earth_free_air_anomaly(
+    >>> grid = load_earth_vertical_gravity_gradient(
     ...     resolution="30m", registration="gridline"
     ... )
     >>> # load high-resolution (5 arc-minutes) grid for a specific region
-    >>> grid = load_earth_free_air_anomaly(
+    >>> grid = load_earth_vertical_gravity_gradient(
     ...     resolution="05m",
     ...     region=[120, 160, 30, 60],
     ...     registration="gridline",
     ... )
     """
     grid = _load_remote_dataset(
-        dataset_name="earth_free_air_anomaly",
-        dataset_prefix="earth_faa_",
+        dataset_name="earth_vgg",
+        dataset_prefix="earth_vgg_",
         resolution=resolution,
         region=region,
         registration=registration,
     )
     return grid
```

### Comparing `pygmt-0.8.0/pygmt/datasets/earth_geoid.py` & `pygmt-0.9.0/pygmt/datasets/earth_geoid.py`

 * *Files 18% similar despite different names*

```diff
@@ -50,17 +50,22 @@
     -------
     grid : :class:`xarray.DataArray`
         The Earth geoid grid. Coordinates are latitude and
         longitude in degrees. Units are in meters.
 
     Note
     ----
-    The :class:`xarray.DataArray` grid doesn't support slice operation, for
-    Earth geoid grids with resolutions of 5 arc-minutes or higher,
-    which are stored as smaller tiles.
+    The registration and coordinate system type of the returned
+    :class:`xarray.DataArray` grid can be accessed via the GMT accessors
+    (i.e., ``grid.gmt.registration`` and ``grid.gmt.gtype`` respectively).
+    However, these properties may be lost after specific grid operations (such
+    as slicing) and will need to be manually set before passing the grid to any
+    PyGMT data processing or plotting functions. Refer to
+    :class:`pygmt.GMTDataArrayAccessor` for detailed explanations and
+    workarounds.
 
     Examples
     --------
 
     >>> from pygmt.datasets import load_earth_geoid
     >>> # load the default grid (gridline-registered 1 arc-degree grid)
     >>> grid = load_earth_geoid()
```

### Comparing `pygmt-0.8.0/pygmt/datasets/earth_magnetic_anomaly.py` & `pygmt-0.9.0/pygmt/datasets/earth_magnetic_anomaly.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,54 +38,59 @@
 
     Parameters
     ----------
     resolution : str
         The grid resolution. The suffix ``d`` and ``m`` stand for
         arc-degrees and arc-minutes. It can be ``"01d"``, ``"30m"``,
         ``"20m"``, ``"15m"``, ``"10m"``, ``"06m"``, ``"05m"``, ``"04m"``,
-        ``"03m"``, or ``"02m"``.
+        ``"03m"``, or ``"02m"``. The ``"02m"`` resolution is not available for
+        ``data_source="wdmam"``.
 
     region : str or list
         The subregion of the grid to load, in the form of a list
         [*xmin*, *xmax*, *ymin*, *ymax*] or a string *xmin/xmax/ymin/ymax*.
         Required for grids with resolutions higher than 5
         arc-minutes (i.e., ``"05m"``).
 
     registration : str
         Grid registration type. Either ``"pixel"`` for pixel registration or
         ``"gridline"`` for gridline registration. Default is ``"gridline"``
-        for all resolutions except ``"02m"`` which is ``"pixel"`` only.
+        for all resolutions except ``"02m"`` for ``data_source="emag2"`` or
+        ``data_source="emag2_4km"``, which are ``"pixel"`` only.
 
     data_source : str
-        Select the source of the magnetic anomaly data.
+        Select the source of the magnetic anomaly data. Available options are:
 
-        Available options:
-
-        - **emag2** : EMAG2 Global Earth Magnetic Anomaly Model [Default
-          option]. Only includes data is observed from sea level over
+        - ``"emag2"``: EMAG2 Global Earth Magnetic Anomaly Model [Default
+          option]. It only includes data observed at sea level over
           oceanic regions. See :gmt-datasets:`earth-mag.html`.
 
-        - **emag2_4km** : Use a version of EMAG2 where all observations
+        - ``"emag2_4km"``: Use a version of EMAG2 where all observations
           are relative to an altitude of 4 km above the geoid and include
           data over land.
 
-        - **wdmam** : World Digital Magnetic Anomaly Map (WDMAM).
-          See :gmt-datasets:`earth-wdmam.html`
+        - ``"wdmam"``: World Digital Magnetic Anomaly Map (WDMAM).
+          See :gmt-datasets:`earth-wdmam.html`.
 
     Returns
     -------
     grid : :class:`xarray.DataArray`
         The Earth magnetic anomaly grid. Coordinates are latitude and
-        longitude in degrees. Units are in nano Teslas (nT).
+        longitude in degrees. Units are in nano Tesla (nT).
 
     Note
     ----
-    The :class:`xarray.DataArray` grid doesn't support slice operation, for
-    Earth magnetic anomaly with resolutions of 5 arc-minutes or higher,
-    which are stored as smaller tiles.
+    The registration and coordinate system type of the returned
+    :class:`xarray.DataArray` grid can be accessed via the GMT accessors
+    (i.e., ``grid.gmt.registration`` and ``grid.gmt.gtype`` respectively).
+    However, these properties may be lost after specific grid operations (such
+    as slicing) and will need to be manually set before passing the grid to any
+    PyGMT data processing or plotting functions. Refer to
+    :class:`pygmt.GMTDataArrayAccessor` for detailed explanations and
+    workarounds.
 
     Examples
     --------
 
     >>> from pygmt.datasets import load_earth_magnetic_anomaly
     >>> # load the default grid (gridline-registered 1 arc-degree grid)
     >>> grid = load_earth_magnetic_anomaly()
@@ -111,16 +116,16 @@
     magnetic_anomaly_sources = {
         "emag2": "earth_mag_",
         "emag2_4km": "earth_mag4km_",
         "wdmam": "earth_wdmam_",
     }
     if data_source not in magnetic_anomaly_sources:
         raise GMTInvalidInput(
-            f"Invalid earth magnetic anomaly 'data_source' {data_source}, "
-            "valid values are 'emag2', 'emag2_4km', and 'wdmam'."
+            f"Invalid earth magnetic anomaly data source '{data_source}'. "
+            "Valid values are 'emag2', 'emag2_4km', and 'wdmam'."
         )
     dataset_prefix = magnetic_anomaly_sources[data_source]
     if data_source == "wdmam":
         dataset_name = "earth_wdmam"
     else:
         dataset_name = "earth_magnetic_anomaly"
     grid = _load_remote_dataset(
```

### Comparing `pygmt-0.8.0/pygmt/datasets/earth_relief.py` & `pygmt-0.9.0/pygmt/datasets/earth_relief.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,17 @@
     data_source="igpp",
     use_srtm=False,
 ):
     r"""
     Load Earth relief grids (topography and bathymetry) in various resolutions.
 
     The grids are downloaded to a user data directory
-    (usually a subdirectory under ~/.gmt/server/earth/) the first time you
+    (usually ``~/.gmt/server/earth/earth_relief``,
+    ``~/.gmt/server/earth/earth_gebco``, ``~/.gmt/server/earth/earth_gebcosi``,
+    or ``~/.gmt/server/earth/earth_synbath``) the first time you
     invoke this function. Afterwards, it will load the grid from the data
     directory. So you'll need an internet connection the first time around.
 
     This module downloads the grids that can also be accessed by
     passing in the file name **@**\ *earth_relief_type*\_\ *res*\[_\ *reg*] to
     any grid plotting/processing function. *earth_relief_type* is the GMT name
     for the dataset. The available options are **earth_relief**\,
@@ -55,30 +57,28 @@
 
     registration : str
         Grid registration type. Either ``"pixel"`` for pixel registration or
         ``"gridline"`` for gridline registration. Default is ``"gridline"``
         for all resolutions except ``"15s"`` which is ``"pixel"`` only.
 
     data_source : str
-        Select the source for the Earth relief data.
+        Select the source for the Earth relief data. Available options are:
 
-        Available options:
-
-        - **igpp** : IGPP Global Earth Relief [Default option]. See
+        - ``"igpp"``: IGPP Global Earth Relief [Default option]. See
           :gmt-datasets:`earth-relief.html`.
 
-        - **synbath** : IGPP Global Earth Relief dataset that uses
-          stastical properties of young seafloor to provide more realistic
+        - ``"synbath"``: IGPP Global Earth Relief dataset that uses
+          stastical properties of young seafloor to provide a more realistic
           relief of young areas with small seamounts.
 
-        - **gebco** : GEBCO Global Earth Relief with only observed relief and
+        - ``"gebco"``: GEBCO Global Earth Relief with only observed relief and
           inferred relief via altimetric gravity. See
           :gmt-datasets:`earth-gebco.html`.
 
-        - **gebcosi** : GEBCO Global Earth Relief that gives sub-ice (si)
+        - ``"gebcosi"``: GEBCO Global Earth Relief that gives sub-ice (si)
           elevations.
 
     use_srtm : bool
         By default, the land-only SRTM tiles from NASA are used to generate the
         ``"03s"`` and ``"01s"`` grids, and the missing ocean values are filled
         by up-sampling the SRTM15 tiles which have a resolution of 15
         arc-seconds (i.e., ``"15s"``). If True, will only load the original
@@ -88,17 +88,22 @@
     -------
     grid : :class:`xarray.DataArray`
         The Earth relief grid. Coordinates are latitude and longitude in
         degrees. Relief is in meters.
 
     Note
     ----
-    The :class:`xarray.DataArray` grid doesn't support slice operation, for
-    Earth relief data with resolutions of 5 arc-minutes or higher, which are
-    stored as smaller tiles.
+    The registration and coordinate system type of the returned
+    :class:`xarray.DataArray` grid can be accessed via the GMT accessors
+    (i.e., ``grid.gmt.registration`` and ``grid.gmt.gtype`` respectively).
+    However, these properties may be lost after specific grid operations (such
+    as slicing) and will need to be manually set before passing the grid to any
+    PyGMT data processing or plotting functions. Refer to
+    :class:`pygmt.GMTDataArrayAccessor` for detailed explanations and
+    workarounds.
 
     Examples
     --------
 
     >>> from pygmt.datasets import load_earth_relief
     >>> # load the default grid (gridline-registered 1 arc-degree grid)
     >>> grid = load_earth_relief()
@@ -125,31 +130,30 @@
         "igpp": "earth_relief_",
         "gebco": "earth_gebco_",
         "gebcosi": "earth_gebcosi_",
         "synbath": "earth_synbath_",
     }
     if data_source not in earth_relief_sources:
         raise GMTInvalidInput(
-            f"Invalid earth relief 'data_source' {data_source}, "
-            "valid values are 'igpp', 'gebco', 'gebcosi' and 'synbath'."
+            f"Invalid earth relief data source '{data_source}'. "
+            "Valid values are 'igpp', 'gebco', 'gebcosi' and 'synbath'."
         )
     # Choose earth relief data prefix
     if use_srtm and resolution in land_only_srtm_resolutions:
         if data_source == "igpp":
             dataset_prefix = "srtm_relief_"
         else:
             raise GMTInvalidInput(
-                f"The {data_source} option is not available if 'use_srtm=True'."
-                " Set data_source to 'igpp'."
+                f"Option 'use_srtm=True' doesn't work with data source '{data_source}'."
+                " Please set 'data_source' to 'igpp'."
             )
     else:
         dataset_prefix = earth_relief_sources[data_source]
 
-    dataset_name = "earth_relief"
     grid = _load_remote_dataset(
-        dataset_name=dataset_name,
+        dataset_name="earth_relief",
         dataset_prefix=dataset_prefix,
         resolution=resolution,
         region=region,
         registration=registration,
     )
     return grid
```

### Comparing `pygmt-0.8.0/pygmt/datasets/load_remote_dataset.py` & `pygmt-0.9.0/pygmt/datasets/load_remote_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     ----------
     registrations : list
         A list of the accepted registrations for a given resolution.
         Can be either "pixel" or "gridline".
 
     tiled : bool
         States if the given resolution is tiled, which requires an
-        argument for ``region``."
+        argument for ``region``.
     """
 
     registrations: list
     tiled: bool
 
 
 class GMTRemoteDataset(NamedTuple):
@@ -139,14 +139,36 @@
             "06m": Resolution(["gridline", "pixel"], False),
             "05m": Resolution(["gridline", "pixel"], True),
             "04m": Resolution(["gridline", "pixel"], True),
             "03m": Resolution(["gridline", "pixel"], True),
             "02m": Resolution(["pixel"], True),
         },
     ),
+    "earth_mask": GMTRemoteDataset(
+        title="Earth mask",
+        name="earth_mask",
+        long_name="Mask of land and water features",
+        units=None,
+        extra_attributes={"horizontal_datum": "WGS84"},
+        resolutions={
+            "01d": Resolution(["gridline", "pixel"], False),
+            "30m": Resolution(["gridline", "pixel"], False),
+            "20m": Resolution(["gridline", "pixel"], False),
+            "15m": Resolution(["gridline", "pixel"], False),
+            "10m": Resolution(["gridline", "pixel"], False),
+            "06m": Resolution(["gridline", "pixel"], False),
+            "05m": Resolution(["gridline", "pixel"], False),
+            "04m": Resolution(["gridline", "pixel"], False),
+            "03m": Resolution(["gridline", "pixel"], False),
+            "02m": Resolution(["gridline", "pixel"], False),
+            "01m": Resolution(["gridline", "pixel"], False),
+            "30s": Resolution(["gridline", "pixel"], False),
+            "15s": Resolution(["gridline", "pixel"], False),
+        },
+    ),
     "earth_relief": GMTRemoteDataset(
         title="Earth relief",
         name="elevation",
         long_name="Earth elevation relative to the geoid",
         units="meters",
         extra_attributes={"vertical_datum": "EGM96", "horizontal_datum": "WGS84"},
         resolutions={
@@ -231,77 +253,76 @@
         The subregion of the grid to load, in the form of a list
         [*xmin*, *xmax*, *ymin*, *ymax*] or a string *xmin/xmax/ymin/ymax*.
         Required for tiled grids.
 
     registration : str
         Grid registration type. Either ``"pixel"`` for pixel registration or
         ``"gridline"`` for gridline registration. Default is ``None``, where
-        a pixel-registered grid is returned unless only the
-        gridline-registered grid is available.
+        a gridline-registered grid is returned unless only the
+        pixel-registered grid is available.
 
     Returns
     -------
     grid : :class:`xarray.DataArray`
         The GMT remote dataset grid.
 
     Note
     ----
     The returned :class:`xarray.DataArray` doesn't support slice operation for
     tiled grids.
     """
     dataset = datasets[dataset_name]
+
+    # check resolution
     if resolution not in dataset.resolutions.keys():
         raise GMTInvalidInput(f"Invalid resolution '{resolution}'.")
+
+    # check registration
     if registration is None:
-        # Check if "gridline" is an available registration for the resolution
-        if "gridline" in dataset.resolutions[resolution].registrations:
-            # Use default of gridline registration if available
-            registration = "gridline"
-        else:
+        # use gridline registration unless only pixel registration is available
+        registration = "gridline"
+        if "gridline" not in dataset.resolutions[resolution].registrations:
             registration = "pixel"
-    if registration in ("pixel", "gridline"):
-        reg = f"_{registration[0]}"
+    elif registration in ("pixel", "gridline"):
+        if registration not in dataset.resolutions[resolution].registrations:
+            raise GMTInvalidInput(
+                f"{registration} registration is not available for the "
+                f"{resolution} {dataset.title} dataset. Only "
+                f"{dataset.resolutions[resolution].registrations[0]}"
+                " registration is available."
+            )
     else:
         raise GMTInvalidInput(
             f"Invalid grid registration: '{registration}', should be either "
             "'pixel', 'gridline' or None. Default is None, where a "
             "gridline-registered grid is returned unless only the "
             "pixel-registered grid is available."
         )
-
-    if registration and (
-        registration not in dataset.resolutions[resolution].registrations
-    ):
-        raise GMTInvalidInput(
-            f"{registration} registration is not available for the "
-            f"{resolution} {dataset.title} dataset. Only "
-            f"{dataset.resolutions[resolution].registrations[0]}"
-            " registration is available."
-        )
+    reg = f"_{registration[0]}"
 
     # different ways to load tiled and non-tiled grids.
     # Known issue: tiled grids don't support slice operation
     # See https://github.com/GenericMappingTools/pygmt/issues/524
     if region is None:
         if dataset.resolutions[resolution].tiled:
             raise GMTInvalidInput(
-                f"'region' is required for {dataset.title}"
-                f"resolution '{resolution}'."
+                f"'region' is required for {dataset.title} resolution '{resolution}'."
             )
         fname = which(f"@{dataset_prefix}{resolution}{reg}", download="a")
         grid = load_dataarray(fname, engine="netcdf4")
     else:
         grid = grdcut(f"@{dataset_prefix}{resolution}{reg}", region=region)
 
     # Add some metadata to the grid
     grid.name = dataset.name
     grid.attrs["long_name"] = dataset.long_name
-    grid.attrs["units"] = dataset.units
+    if dataset.units:
+        grid.attrs["units"] = dataset.units
     for key, value in dataset.extra_attributes.items():
         grid.attrs[key] = value
     # Remove the actual range because it gets outdated when indexing the grid,
     # which causes problems when exporting it to netCDF for usage on the
     # command-line.
-    grid.attrs.pop("actual_range")
+    grid.attrs.pop("actual_range", None)
     for coord in grid.coords:
-        grid[coord].attrs.pop("actual_range")
+        grid[coord].attrs.pop("actual_range", None)
     return grid
```

### Comparing `pygmt-0.8.0/pygmt/exceptions.py` & `pygmt-0.9.0/pygmt/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# pylint: disable=missing-docstring
-#
-# Custom exception types used throughout the library. All exceptions derive
-# from GMTError.
+"""
+Custom exception types used throughout the library.
+
+All exceptions derive from GMTError.
+"""
 
 
 class GMTError(Exception):
     """
     Base class for all GMT related errors.
     """
```

### Comparing `pygmt-0.8.0/pygmt/figure.py` & `pygmt-0.9.0/pygmt/figure.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import base64
 import os
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
 try:
     import IPython
-except ModuleNotFoundError:
+except ImportError:
     IPython = None  # pylint: disable=invalid-name
 
 
 from pygmt.clib import Session
 from pygmt.exceptions import GMTError, GMTInvalidInput
 from pygmt.helpers import (
     build_arg_string,
@@ -205,18 +205,18 @@
             [*pen*] to draw the BoundingBox outline (append a pen or accept
             the default pen of 0.25p,black). **Note**: If both **+g** and
             **+f** are used then we use paint as the fade color instead of
             black. Append **+i** to enforce gray-shades by using ICC profiles.
         anti_aliasing : str
             [**g**\|\ **p**\|\ **t**\][**1**\|\ **2**\|\ **4**].
             Set the anti-aliasing options for **g**\ raphics or **t**\ ext.
-            Append the size of the subsample box (1, 2, or 4) [4]. [Default is
-            no anti-aliasing (same as bits = 1)].
+            Append the size of the subsample box (1, 2, or 4) [Default is
+            ``"4"``]. [Default is no anti-aliasing (same as bits = 1).]
         fmt : str
-            Sets the output format, where **b** means BMP, **e** means EPS,
+            Set the output format, where **b** means BMP, **e** means EPS,
             **E** means EPS with PageSize command, **f** means PDF, **F** means
             multi-page PDF, **j** means JPEG, **g** means PNG, **G** means
             transparent PNG (untouched regions are transparent), **m** means
             PPM, and **t** means TIFF [Default is JPEG]. To
             **b**\|\ **j**\|\ **g**\|\ **t**\ , optionally append **+m** in
             order to get a monochrome (grayscale) image. The EPS format can be
             combined with any of the other formats. For example, **ef** creates
@@ -269,36 +269,44 @@
 
         Parameters
         ----------
         fname : str
             The desired figure file name, including the extension. See the list
             of supported formats and their extensions above.
         transparent : bool
-            If True, will use a transparent background for the figure. Only
-            valid for PNG format.
+            If ``True``, will use a transparent background for the figure.
+            Only valid for PNG format.
         crop : bool
-            If True, will crop the figure canvas (page) to the plot area.
+            If ``True``, will crop the figure canvas (page) to the plot area.
         anti_alias: bool
-            If True, will use anti aliasing when creating raster images (PNG,
-            JPG, TIFF). More specifically, it passes arguments ``t2``
+            If ``True``, will use anti-aliasing when creating raster images
+            (PNG, JPG, TIFF). More specifically, it passes arguments ``t2``
             and ``g2`` to the ``anti_aliasing`` parameter of
             :meth:`pygmt.Figure.psconvert`. Ignored if creating vector
             graphics.
         show: bool
-            If True, will open the figure in an external viewer.
+            If ``True``, will open the figure in an external viewer.
         dpi : int
-            Set raster resolution in dpi. Default is 720 for PDF, 300 for
-            others.
+            Set raster resolution in dpi [Default is ``720`` for PDF, ``300``
+            for others].
         **kwargs : dict
             Additional keyword arguments passed to
             :meth:`pygmt.Figure.psconvert`. Valid parameters are ``gs_path``,
             ``gs_option``, ``resize``, ``bb_style``, and ``verbose``.
         """
         # All supported formats
-        fmts = dict(png="g", pdf="f", jpg="j", bmp="b", eps="e", tif="t", kml="g")
+        fmts = {
+            "png": "g",
+            "pdf": "f",
+            "jpg": "j",
+            "bmp": "b",
+            "eps": "e",
+            "tif": "t",
+            "kml": "g",
+        }
 
         prefix, ext = os.path.splitext(fname)
         ext = ext[1:]  # Remove the .
         if ext not in fmts:
             if ext == "ps":
                 raise GMTInvalidInput(
                     "Extension '.ps' is not supported. "
@@ -327,15 +335,15 @@
         Display a preview of the figure.
 
         Inserts the preview in the Jupyter notebook output if available,
         otherwise opens it in the default viewer for your operating system
         (falls back to the default web browser).
 
         :func:`pygmt.set_display` can select the default display method
-        (**notebook**, **external**, or **none**).
+        (``"notebook"``, ``"external"``, ``"none"`` or ``None``).
 
         The ``method`` parameter can also override the default display method
         for the current figure. Parameters ``dpi`` and ``width`` can be used
         to control the resolution and dimension of the figure in the notebook.
 
         **Note**: The external viewer can be disabled by setting the
         PYGMT_USE_EXTERNAL_DISPLAY environment variable to **false**.
@@ -350,20 +358,25 @@
 
         Parameters
         ----------
         dpi : int
             The image resolution (dots per inch) in Jupyter notebooks.
         width : int
             The image width (in pixels) in Jupyter notebooks.
-        method : str
-            How the current figure will be displayed. Options are
+        method : str or None
+            How the current figure will be displayed. Choose from:
 
-            - **external**: PDF preview in an external program [Default]
-            - **notebook**: PNG preview [Default in Jupyter notebooks]
-            - **none**: Disable image preview
+            - ``"external"``: External PDF preview using the default PDF viewer
+            - ``"notebook"``: Inline PNG preview in the current notebook
+            - ``"none"``: Disable image preview
+            - ``None``: Reset to the default display method
+
+            The default display method is ``"external"`` in Python consoles or
+            ``"notebook"`` in Jupyter notebooks, but can be changed by
+            :func:`pygmt.set_display`.
         waiting : float
             Suspend the execution of the current process for a given number of
             seconds after launching an external viewer.
             Only works if ``method="external"``.
         **kwargs : dict
             Additional keyword arguments passed to
             :meth:`pygmt.Figure.psconvert`. Valid parameters are ``gs_path``,
@@ -381,15 +394,15 @@
             raise GMTInvalidInput(
                 (
                     f"Invalid display method '{method}', "
                     "should be either 'notebook', 'external', or 'none'."
                 )
             )
 
-        if method in ["notebook", "none"]:
+        if method == "notebook":
             if IPython is None:
                 raise GMTError(
                     (
                         "Notebook display is selected, but IPython is not available. "
                         "Make sure you have IPython installed, "
                         "or run the script in a Jupyter notebook."
                     )
@@ -506,34 +519,61 @@
         plot3d,
         rose,
         set_panel,
         solar,
         subplot,
         ternary,
         text,
+        tilemap,
+        timestamp,
         velo,
         wiggle,
     )
 
 
 def set_display(method=None):
     """
-    Set the display method.
+    Set the display method when calling :meth:`pygmt.Figure.show`.
 
     Parameters
     ----------
     method : str or None
-        The method to display an image. Choose from:
+        The method to display an image preview. Choose from:
+
+        - ``"external"``: External PDF preview using the default PDF viewer
+        - ``"notebook"``: Inline PNG preview in the current notebook
+        - ``"none"``: Disable image preview
+        - ``None``: Reset to the default display method
 
-        - **external**: PDF preview in an external program [Default]
-        - **notebook**: PNG preview [Default in Jupyter notebooks]
-        - **none**: Disable image preview
+        The default display method is ``"external"`` in Python consoles or
+        ``"notebook"`` in Jupyter notebooks.
+
+    Examples
+    --------
+    Let's assume that you're using a Jupyter Notebook:
+
+    >>> import pygmt
+    >>> fig = pygmt.Figure()
+    >>> fig.basemap(region=[0, 10, 0, 10], projection="X10c/5c", frame=True)
+    >>> fig.show()  # will display a PNG image in the current notebook
+    >>>
+    >>> # set the display method to "external"
+    >>> pygmt.set_display(method="external")  # doctest: +SKIP
+    >>> fig.show()  # will display a PDF image using the default PDF viewer
+    >>>
+    >>> # set the display method to "none"
+    >>> pygmt.set_display(method="none")
+    >>> fig.show()  # will not show any image
+    >>>
+    >>> # reset to the default display method
+    >>> pygmt.set_display(method=None)
+    >>> fig.show()  # again, will show a PNG image in the current notebook
     """
     if method in ["notebook", "external", "none"]:
         SHOW_CONFIG["method"] = method
     elif method is not None:
         raise GMTInvalidInput(
             (
                 f"Invalid display mode '{method}', "
-                "should be either 'notebook', 'external' or 'none'."
+                "should be either 'notebook', 'external', 'none' or None."
             )
         )
```

### Comparing `pygmt-0.8.0/pygmt/helpers/decorators.py` & `pygmt-0.9.0/pygmt/helpers/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,36 +25,29 @@
             Select map :doc:`projection </projections/index>`.""",
     "area_thresh": r"""
         area_thresh : int or float or str
             *min_area*\ [/*min_level*/*max_level*][**+a**\[**g**\|\ **i**]\
             [**s**\|\ **S**]][**+l**\|\ **r**][**+p**\ *percent*].
             Features with an area smaller than *min_area* in km\ :sup:`2` or of
             hierarchical level that is lower than *min_level* or higher than
-            *max_level* will not be plotted [Default is 0/0/4 (all
+            *max_level* will not be plotted [Default is ``"0/0/4"`` (all
             features)].""",
     "frame": r"""
         frame : bool or str or list
             Set map boundary
             :doc:`frame and axes attributes </tutorials/basics/frames>`. """,
-    "timestamp": """\
-        timestamp : bool or str
-            Draw GMT time stamp logo on plot.""",
     "cmap": r"""
         cmap : str
            File name of a CPT file or a series of comma-separated colors
            (e.g., *color1*,\ *color2*,\ *color3*) to build a linear continuous
            CPT from those colors automatically.""",
-    "color": """\
-        color : str or 1-D array
-            Select color or pattern for filling of symbols or polygons [Default
-            is no fill].""",
-    "fill": """\
+    "fill": r"""
         fill : str
-            Select color or pattern for filling of symbols or polygons [Default
-            is no fill].""",
+            Set color or pattern for filling symbols or polygons
+            [Default is no fill].""",
     "spacing": r"""
         spacing : str
             *x_inc*\ [**+e**\|\ **n**][/\ *y_inc*\ [**+e**\|\ **n**]].
             *x_inc* [and optionally *y_inc*] is the grid spacing.
 
             - **Geographical (degrees) coordinates**: Optionally, append an
               increment unit. Choose among **m** to indicate arc-minutes or
@@ -78,27 +71,27 @@
               depends on whether you have selected a gridline-registered or
               pixel-registered grid; see :gmt-docs:`GMT File Formats
               <cookbook/file-formats.html#gmt-file-formats>` for details.
 
             **Note**: If ``region=grdfile`` is used then the grid spacing and
             the registration have already been initialized; use ``spacing`` and
             ``registration`` to override these values.""",
-    "verbose": """\
+    "verbose": r"""
         verbose : bool or str
             Select verbosity level [Default is **w**], which modulates the messages
             written to stderr. Choose among 7 levels of verbosity:
 
             - **q** - Quiet, not even fatal error messages are produced
             - **e** - Error messages only
             - **w** - Warnings [Default]
             - **t** - Timings (report runtimes for time-intensive algorithms)
             - **i** - Informational messages (same as ``verbose=True``)
             - **c** - Compatibility warnings
             - **d** - Debugging messages""",
-    "pen": """\
+    "pen": r"""
         pen : str
             Set pen attributes for lines or the outline of symbols.""",
     "aspatial": r"""
         aspatial : bool or str
             [*col*\ =]\ *name*\ [,...].
             Control how aspatial data are handled during input and output.
             Full documentation is at :gmt-docs:`gmt.html#aspatial-full`.
@@ -308,21 +301,21 @@
               used then the columns given to ``outcols`` correspond to the
               order after the ``incols`` selection has taken place.""",
     "perspective": r"""
         perspective : list or str
             [**x**\|\ **y**\|\ **z**]\ *azim*\[/*elev*\[/*zlevel*]]\
             [**+w**\ *lon0*/*lat0*\[/*z0*]][**+v**\ *x0*/*y0*].
             Select perspective view and set the azimuth and elevation angle of
-            the viewpoint. Default is [180, 90]. Full documentation is at
+            the viewpoint [Default is ``[180, 90]``]. Full documentation is at
             :gmt-docs:`gmt.html#perspective-full`.
         """,
     "registration": r"""
         registration : str
             **g**\|\ **p**.
-            Force gridline (**g**) or pixel (**p**) node registration.
+            Force gridline (**g**) or pixel (**p**) node registration
             [Default is **g**\ (ridline)].
         """,
     "skiprows": r"""
         skiprows : bool or str
             [*cols*][**+a**][**+r**].
             Suppress output for records whose *z*-value equals NaN [Default
             outputs all records]. Optionally, supply a comma-separated list of
@@ -333,18 +326,18 @@
             supported:
 
                 - **+r** to reverse the suppression, i.e., only output the
                   records whose *z*-value equals NaN.
                 - **+a** to suppress the output of the record if just one or
                   more of the columns equal NaN [Default skips record only
                   if values in all specified *cols* equal NaN].""",
-    "transparency": """\
+    "transparency": r"""
         transparency : int or float
             Set transparency level, in [0-100] percent range
-            [Default is 0, i.e., opaque].
+            [Default is ``0``, i.e., opaque].
             Only visible when PDF or raster format output is selected.
             Only the PNG format selection adds a transparency layer
             in the image (for further processing). """,
     "wrap": r"""
         wrap : str
             **y**\|\ **a**\|\ **w**\|\ **d**\|\ **h**\|\ **m**\|\ **s**\|\
             **c**\ *period*\ [/*phase*][**+c**\ *col*].
@@ -565,14 +558,25 @@
                 elif short_param in kwargs:
                     msg = (
                         f"Short-form parameter ({short_param}) is not recommended. "
                         f"Use long-form parameter '{long_alias}' instead."
                     )
                     warnings.warn(msg, category=SyntaxWarning, stacklevel=2)
 
+            # timestamp (U) is deprecated since v0.9.0.
+            if "U" in kwargs or "timestamp" in kwargs:
+                if "timestamp" in kwargs:
+                    kwargs["U"] = kwargs.pop("timestamp")
+                msg = (
+                    "Parameters 'U' and 'timestamp' are deprecated since v0.9.0 "
+                    "and will be removed in v0.12.0. "
+                    "Use Figure.timestamp() instead."
+                )
+                warnings.warn(msg, category=SyntaxWarning, stacklevel=2)
+
             # xshift (X) is deprecated since v0.8.0.
             if "X" in kwargs or "xshift" in kwargs:
                 if "xshift" in kwargs:
                     kwargs["X"] = kwargs.pop("xshift")
                 msg = (
                     "Parameters 'X' and 'xshift' are deprecated since v0.8.0 "
                     "and will be removed in v0.12.0. "
```

### Comparing `pygmt-0.8.0/pygmt/helpers/tempfile.py` & `pygmt-0.9.0/pygmt/helpers/tempfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,15 @@
     0.0 1.0 2.0
     0.0 1.0 2.0
     <BLANKLINE>
     [0. 0. 0.] [1. 1. 1.] [2. 2. 2.]
     """
 
     def __init__(self, prefix="pygmt-", suffix=".txt"):
-        args = dict(prefix=prefix, suffix=suffix, delete=False)
-        with NamedTemporaryFile(**args) as tmpfile:
+        with NamedTemporaryFile(prefix=prefix, suffix=suffix, delete=False) as tmpfile:
             self.name = tmpfile.name
 
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         if os.path.exists(self.name):
@@ -124,15 +123,15 @@
     ------
     tmpfilename : str
         A temporary OGR_GMT format file holding the geographical data.
         E.g. '1a2b3c4d5e6.gmt'.
     """
     with GMTTempFile(suffix=".gmt") as tmpfile:
         os.remove(tmpfile.name)  # ensure file is deleted first
-        ogrgmt_kwargs = dict(filename=tmpfile.name, driver="OGR_GMT", mode="w")
+        ogrgmt_kwargs = {"filename": tmpfile.name, "driver": "OGR_GMT", "mode": "w"}
         try:
             # Using geopandas.to_file to directly export to OGR_GMT format
             geojson.to_file(**ogrgmt_kwargs)
         except AttributeError:
             # pylint: disable=import-outside-toplevel
             # Other 'geo' formats which implement __geo_interface__
             import json
```

### Comparing `pygmt-0.8.0/pygmt/helpers/testing.py` & `pygmt-0.9.0/pygmt/helpers/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,14 +185,17 @@
         # Earth geoid grids
         "@earth_geoid_01d_g",
         "@N00W030.earth_geoid_01m_g.nc",  # Specific grid for 01m test
         # Earth magnetic anomaly grids
         "@earth_mag_01d_g",
         "@S30W060.earth_mag_02m_p.nc",  # Specific grid for 02m test
         "@earth_mag4km_01d_g",
+        "@S30W120.earth_mag4km_02m_p.nc",  # Specific grid for 02m test
+        # Earth mask grid
+        "@earth_mask_01d_g",
         # Earth free-air anomaly grids
         "@earth_faa_01d_g",
         "@N00W030.earth_faa_01m_p.nc",  # Specific grid for 01m test
         # Earth vertical gravity gradient grids
         "@earth_vgg_01d_g",
         "@N00W030.earth_vgg_01m_p.nc",  # Specific grid for 01m test
         # Earth WDMAM grids
```

### Comparing `pygmt-0.8.0/pygmt/helpers/utils.py` & `pygmt-0.9.0/pygmt/helpers/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,46 +115,51 @@
     ...     print(temp)
     ...
     some argument
     """
     yield arg
 
 
-def build_arg_string(kwdict, infile=None, outfile=None):
+def build_arg_string(kwdict, confdict=None, infile=None, outfile=None):
     r"""
-    Convert a dict and optional input/output files into a GMT argument string.
+    Convert keyword dictionaries and input/output files into a GMT argument
+    string.
 
     Make sure all values in ``kwdict`` have been previously converted to a
     string representation using the ``kwargs_to_strings`` decorator. The only
     exceptions are True, False and None.
 
     Any lists or tuples left will be interpreted as multiple entries for the
-    same command line argument. For example, the kwargs entry ``'B': ['xa',
+    same command line option. For example, the kwargs entry ``'B': ['xa',
     'yaf']`` will be converted to ``-Bxa -Byaf`` in the argument string.
 
     Note that spaces `` `` in arguments are converted to the equivalent octal
     code ``\040``, except in the case of -J (projection) arguments where PROJ4
     strings (e.g. "+proj=longlat +datum=WGS84") will have their spaces removed.
     See https://github.com/GenericMappingTools/pygmt/pull/1487 for more info.
 
     Parameters
     ----------
     kwdict : dict
-        A dict containing parsed keyword arguments.
+        A dictionary containing parsed keyword arguments.
+    confdict : dict
+        A dictionary containing configurable GMT parameters.
     infile : str or pathlib.Path
         The input file.
     outfile : str or pathlib.Path
         The output file.
 
     Returns
     -------
     args : str
         The space-delimited argument string with '-' inserted before each
-        keyword. The arguments are sorted alphabetically, with optional input
-        file at the beginning and optional output file at the end.
+        keyword, or '--' inserted before GMT configuration key-value pairs.
+        The keyword arguments are sorted alphabetically, followed by GMT
+        configuration key-value pairs, with optional input file at the
+        beginning and optional output file at the end.
 
     Examples
     --------
 
     >>> print(
     ...     build_arg_string(
     ...         dict(
@@ -195,19 +200,20 @@
     ...         ),
     ...     )
     ... )
     -BWSne+tBlank\040Space -Baf -F+t"Empty\040\040Spaces" -l'Void\040Space'
     >>> print(
     ...     build_arg_string(
     ...         dict(A="0", B=True, C="rainbow"),
+    ...         confdict=dict(FORMAT_DATE_MAP="o dd"),
     ...         infile="input.txt",
     ...         outfile="output.txt",
     ...     )
     ... )
-    input.txt -A0 -B -Crainbow ->output.txt
+    input.txt -A0 -B -Crainbow --FORMAT_DATE_MAP="o dd" ->output.txt
     """
     gmt_args = []
 
     for key in kwdict:
         if len(key) > 2:  # raise an exception for unrecognized options
             raise GMTInvalidInput(f"Unrecognized parameter '{key}'.")
         if kwdict[key] is None or kwdict[key] is False:
@@ -223,14 +229,18 @@
                 _value = str(kwdict[key]).replace(" ", r"\040")
             else:
                 # special handling if key == "J" (projection)
                 # remove any spaces in PROJ4 string
                 _value = str(kwdict[key]).replace(" ", "")
             gmt_args.append(rf"-{key}{_value}")
     gmt_args = sorted(gmt_args)
+
+    if confdict:
+        gmt_args.extend(f'--{key}="{value}"' for key, value in confdict.items())
+
     if infile:
         gmt_args = [str(infile)] + gmt_args
     if outfile:
         gmt_args.append("->" + str(outfile))
     return " ".join(gmt_args)
 
 
@@ -279,15 +289,18 @@
     Parameters
     ----------
     fname : str
         The file name of the file (preferably a full path).
     """
     # Redirect stdout and stderr to devnull so that the terminal isn't filled
     # with noise
-    run_args = dict(stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+    run_args = {
+        "stdout": subprocess.DEVNULL,
+        "stderr": subprocess.DEVNULL,
+    }
 
     # Open the file with the default viewer.
     # Fall back to the browser if can't recognize the operating system.
     os_name = sys.platform
     if os_name.startswith(("linux", "freebsd")) and shutil.which("xdg-open"):
         subprocess.run(["xdg-open", fname], check=False, **run_args)
     elif os_name == "darwin":  # Darwin is macOS
```

### Comparing `pygmt-0.8.0/pygmt/io.py` & `pygmt-0.9.0/pygmt/io.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/session_management.py` & `pygmt-0.9.0/pygmt/session_management.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/sphinx_gallery.py` & `pygmt-0.9.0/pygmt/sphinx_gallery.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/src/__init__.py` & `pygmt-0.9.0/pygmt/src/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,16 @@
 from pygmt.src.sph2grd import sph2grd
 from pygmt.src.sphdistance import sphdistance
 from pygmt.src.sphinterpolate import sphinterpolate
 from pygmt.src.subplot import set_panel, subplot
 from pygmt.src.surface import surface
 from pygmt.src.ternary import ternary
 from pygmt.src.text import text_ as text  # "text" is an argument within "text_"
+from pygmt.src.tilemap import tilemap
+from pygmt.src.timestamp import timestamp
 from pygmt.src.triangulate import triangulate
 from pygmt.src.velo import velo
 from pygmt.src.which import which
 from pygmt.src.wiggle import wiggle
 from pygmt.src.x2sys_cross import x2sys_cross
 from pygmt.src.x2sys_init import x2sys_init
 from pygmt.src.xyz2grd import xyz2grd
```

### Comparing `pygmt-0.8.0/pygmt/src/basemap.py` & `pygmt-0.9.0/pygmt/src/basemap.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,26 @@
 """
 basemap - Plot base maps and frames for the figure.
 """
 
 from pygmt.clib import Session
-from pygmt.helpers import (
-    args_in_kwargs,
-    build_arg_string,
-    fmt_docstring,
-    kwargs_to_strings,
-    use_alias,
-)
+from pygmt.helpers import build_arg_string, fmt_docstring, kwargs_to_strings, use_alias
 
 
 @fmt_docstring
 @use_alias(
     R="region",
     J="projection",
     Jz="zscale",
     JZ="zsize",
     B="frame",
     L="map_scale",
     F="box",
     Td="rose",
     Tm="compass",
-    U="timestamp",
     V="verbose",
     c="panel",
     f="coltypes",
     p="perspective",
     t="transparency",
 )
 @kwargs_to_strings(R="sequence", c="sequence_comma", p="sequence")
@@ -36,14 +29,17 @@
     Plot base maps and frames for the figure.
 
     Creates a basic or fancy basemap with axes, fill, and titles. Several
     map projections are available, and the user may specify separate
     tick-mark intervals for boundary annotation, ticking, and [optionally]
     gridlines. A simple map scale or directional rose may also be plotted.
 
+    At least one of the parameters ``frame``, ``map_scale``, ``rose``, or
+    ``compass`` must be specified if not in subplot mode.
+
     Full option list at :gmt-docs:`basemap.html`
 
     {aliases}
 
     Parameters
     ----------
     {projection}
@@ -51,44 +47,41 @@
         Set z-axis scaling or z-axis size.
     {region}
         *Required if this is the first plot command.*
     {frame}
     map_scale : str
         [**g**\|\ **j**\|\ **J**\|\ **n**\|\ **x**]\ *refpoint*\
         **+w**\ *length*.
-        Draws a simple map scale centered on the reference point specified.
+        Draw a simple map scale centered on the reference point specified.
     box : bool or str
         [**+c**\ *clearances*][**+g**\ *fill*][**+i**\ [[*gap*/]\ *pen*]]\
         [**+p**\ [*pen*]][**+r**\ [*radius*]][**+s**\ [[*dx*/*dy*/][*shade*]]].
-        If set to ``True``, draws a rectangular border around the
+        If set to ``True``, draw a rectangular border around the
         map scale or rose. Alternatively, specify a different pen with
         **+p**\ *pen*. Add **+g**\ *fill* to fill the scale panel [Default is
         no fill]. Append **+c**\ *clearance* where *clearance* is either gap,
         xgap/ygap, or lgap/rgap/bgap/tgap where these items are uniform,
         separate in x- and y-direction, or individual side spacings between
         scale and border. Append **+i** to draw a secondary, inner border as
         well. We use a uniform gap between borders of 2p and the
         :gmt-term:`MAP_DEFAULTS_PEN` unless other values are specified. Append
         **+r** to draw rounded rectangular borders instead, with a 6p corner
         radius. You can override this radius by appending another value.
         Finally, append **+s** to draw an offset background shaded region.
         Here, *dx/dy* indicates the shift relative to the foreground frame
-        [Default is 4p/-4p] and shade sets the fill style to use for shading
-        [Default is gray50].
+        [Default is ``"4p/-4p"``] and shade sets the fill style to use for
+        shading [Default is ``"gray50"``].
     rose : str
-        Draws a map directional rose on the map at the location defined by
+        Draw a map directional rose on the map at the location defined by
         the reference and anchor points.
     compass : str
-        Draws a map magnetic rose on the map at the location defined by the
-        reference and anchor points
-    {timestamp}
+        Draw a map magnetic rose on the map at the location defined by the
+        reference and anchor points.
     {verbose}
     {panel}
     {coltypes}
     {perspective}
     {transparency}
     """
     kwargs = self._preprocess(**kwargs)  # pylint: disable=protected-access
-    if not args_in_kwargs(args=["B", "L", "Td", "Tm", "c"], kwargs=kwargs):
-        kwargs["B"] = True  # Plotting frames if required arguments not given
     with Session() as lib:
         lib.call_module(module="basemap", args=build_arg_string(kwargs))
```

### Comparing `pygmt-0.8.0/pygmt/src/binstats.py` & `pygmt-0.9.0/pygmt/src/binstats.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         - **z** for the sum
     empty : float or int
         Set the value assigned to empty nodes [Default is NaN].
     normalize : bool
         Normalize the resulting grid values by the area represented by the
         search *radius* [no normalization].
     search_radius : float or str
-        Sets the *search_radius* that determines which data points are
+        Set the *search_radius* that determines which data points are
         considered close to a node. Append the distance unit.
         Not compatible with ``tiling``.
     weight : str
         Input data have an extra column containing observation point weight.
         If weights are given then weighted statistical quantities will be
         computed while the count will be the sum of the weights instead of
         number of points. If the weights are actually uncertainties
```

### Comparing `pygmt-0.8.0/pygmt/src/blockm.py` & `pygmt-0.9.0/pygmt/src/blockm.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/src/coast.py` & `pygmt-0.9.0/pygmt/src/coast.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     E="dcw",
     I="rivers",
     L="map_scale",
     N="borders",
     W="shorelines",
     G="land",
     S="water",
-    U="timestamp",
     V="verbose",
     c="panel",
     p="perspective",
     t="transparency",
 )
 @kwargs_to_strings(R="sequence", c="sequence_comma", p="sequence")
 def coast(self, **kwargs):
@@ -73,15 +72,15 @@
         Set the shade, color, or pattern for lakes and river-lakes. The
         default is the fill chosen for wet areas set by the ``water``
         parameter. Optionally, specify separate fills by appending
         **+l** for lakes or **+r** for river-lakes, and passing multiple
         strings in a list.
     resolution : str
         **f**\|\ **h**\|\ **i**\|\ **l**\|\ **c**.
-        Selects the resolution of the data set to: (**f**\ )ull,
+        Select the resolution of the data set to: (**f**\ )ull,
         (**h**\ )igh, (**i**\ )ntermediate, (**l**\ )ow,
         and (**c**\ )rude.
     land : str
         Select filling or clipping of "dry" areas.
     rivers : int or str or list
         *river*\ [/*pen*].
         Draw rivers. Specify the type of rivers and [optionally] append
@@ -124,15 +123,15 @@
 
         i = All intermittent rivers (5-7)
 
         c = All canals (8-10)
     map_scale : str
         [**g**\|\ **j**\|\ **J**\|\ **n**\|\ **x**]\ *refpoint*\
         **+w**\ *length*.
-        Draws a simple map scale centered on the reference point specified.
+        Draw a simple map scale centered on the reference point specified.
     borders : int or str or list
         *border*\ [/*pen*].
         Draw political boundaries. Specify the type of boundary and
         [optionally] append pen attributes
         [Default is ``"0.25p,black,solid"``].
 
         Choose from the list of boundaries below. Pass a list to
@@ -143,15 +142,14 @@
         2 = State boundaries within the Americas
 
         3 = Marine boundaries
 
         a = All boundaries (1-3)
     water : str
         Select filling or clipping of "wet" areas.
-    {timestamp}
     shorelines : int or str or list
         [*level*\ /]\ *pen*.
         Draw shorelines [Default is no shorelines]. Append pen attributes
         [Default is ``"0.25p,black,solid"``] which
         apply to all four levels. To set the pen for a single level,
         pass a string with *level*\ /*pen*\ , where level is
         1-4 and represent coastline, lakeshore, island-in-lake shore, and
```

### Comparing `pygmt-0.8.0/pygmt/src/config.py` & `pygmt-0.9.0/pygmt/src/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,11 +203,11 @@
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         # revert to initial values
         arg_str = " ".join(
-            [f"{key}={value}" for key, value in self.old_defaults.items()]
+            [f'{key}="{value}"' for key, value in self.old_defaults.items()]
         )
         with Session() as lib:
             lib.call_module(module="set", args=arg_str)
```

### Comparing `pygmt-0.8.0/pygmt/src/contour.py` & `pygmt-0.9.0/pygmt/src/contour.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     C="levels",
     G="label_placement",
     J="projection",
     L="triangular_mesh_pen",
     N="no_clip",
     R="region",
     S="skip",
-    U="timestamp",
     V="verbose",
     W="pen",
     b="binary",
     c="panel",
     d="nodata",
     e="find",
     f="coltypes",
@@ -80,33 +79,32 @@
         [**d**\|\ **f**\|\ **n**\|\ **l**\|\ **L**\|\ **x**\|\ **X**]\ *args*.
         Control the placement of labels along the quoted lines. It supports
         five controlling algorithms. See :gmt-docs:`contour.html#g` for
         details.
     I : bool
         Color the triangles using CPT.
     triangular_mesh_pen : str
-        Pen to draw the underlying triangulation [Default is None].
+        Pen to draw the underlying triangulation [Default is ``None``].
     no_clip : bool
-        Do NOT clip contours or image at the boundaries [Default will clip
-        to fit inside region].
+        Do **not** clip contours or image at the frame boundaries
+        [Default is ``False`` to fit inside ``region``].
     Q : float or str
         [*cut*][**+z**].
-        Do not draw contours with less than cut number of points.
+        Do not draw contours with less than *cut* number of points.
     skip : bool or str
         [**p**\|\ **t**].
         Skip input points outside region.
     {pen}
     label : str
         Add a legend entry for the contour being plotted. Normally, the
         annotated contour is selected for the legend. You can select the
         regular contour instead, or both of them, by considering the label
         to be of the format [*annotcontlabel*][/*contlabel*]. If either
         label contains a slash (/) character then use ``|`` as the
         separator for the two labels instead.
-    {timestamp}
     {verbose}
     {binary}
     {panel}
     {nodata}
     {find}
     {coltypes}
     {header}
```

### Comparing `pygmt-0.8.0/pygmt/src/dimfilter.py` & `pygmt-0.9.0/pygmt/src/dimfilter.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     Spherical geometries. The output grid can optionally be generated as a
     subregion of the input and/or with a new increment using ``spacing``,
     which may add an "extra space" in the input data to prevent edge
     effects for the output grid. If the filter is low-pass, then the output
     may be less frequently sampled than the input. :func:`pygmt.dimfilter`
     will not produce a smooth output as other spatial filters
     do because it returns a minimum median out of *N* medians of *N*
-    sectors. The output can be rough unless the input data is noise-free.
+    sectors. The output can be rough unless the input data are noise-free.
     Thus, an additional filtering (e.g., Gaussian via :func:`pygmt.grdfilter`)
     of the DiM-filtered data is generally recommended.
 
     Full option list at :gmt-docs:`dimfilter.html`
 
     {aliases}
 
@@ -73,15 +73,15 @@
 
         - **3**\ : grid (x,y) in degrees, *width* in km, dx scaled by
           cosine(y), Cartesian distance calculation.
         - **4**\ : grid (x,y) in degrees, *width* in km, Spherical distance
           calculation.
     filter : str
         **x**\ *width*\ [**+l**\|\ **u**].
-        Sets the primary filter type. Choose among convolution and
+        Set the primary filter type. Choose among convolution and
         non-convolution filters. Use the filter code **x** followed by
         the full diameter *width*. Available convolution filters are:
 
         - (**b**) Boxcar: All weights are equal.
         - (**c**) Cosine Arch: Weights follow a cosine arch curve.
         - (**g**) Gaussian: Weights are given by the Gaussian function.
 
@@ -90,36 +90,36 @@
         - (**m**) Median: Returns median value.
         - (**p**) Maximum likelihood probability (a mode estimator): Return
           modal value. If more than one mode is found we return their average
           value. Append **+l** or **+h** to the filter width if you want
           to return the smallest or largest of each sector's modal values.
     sectors : str
         **x**\ *sectors*\ [**+l**\|\ **u**]
-        Sets the secondary filter type **x** and the number of bow-tie sectors.
+        Set the secondary filter type **x** and the number of bow-tie sectors.
         *sectors* must be integer and larger than 0. When *sectors* is
         set to 1, the secondary filter is not effective. Available secondary
         filters **x** are:
 
         - (**l**) Lower: Return the minimum of all filtered values.
         - (**u**) Upper: Return the maximum of all filtered values.
         - (**a**) Average: Return the mean of all filtered values.
         - (**m**) Median: Return the median of all filtered values.
         - (**p**) Mode: Return the mode of all filtered values:
           If more than one mode is found we return their average
           value. Append **+l** or **+h** to the sectors if you rather want to
           return the smallest or largest of the modal values.
     spacing : str or list
-        *x_inc* [and optionally *y_inc*] is the output Increment. Append
+        *x_inc* [and optionally *y_inc*] is the output increment. Append
         **m** to indicate minutes, or **c** to indicate seconds. If the new
         *x_inc*, *y_inc* are NOT integer multiples of the old ones (in the
-        input data), filtering will be considerably slower. [Default: Same
+        input data), filtering will be considerably slower. [Default is same
         as input.]
     region : str or list
         [*xmin*, *xmax*, *ymin*, *ymax*].
-        Defines the region of the output points. [Default: Same as input.]
+        Define the region of the output points [Default is same as input].
     {verbose}
 
     Returns
     -------
     ret: xarray.DataArray or None
         Return type depends on whether the ``outgrid`` parameter is set:
```

### Comparing `pygmt-0.8.0/pygmt/src/filter1d.py` & `pygmt-0.9.0/pygmt/src/filter1d.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     {aliases}
 
     Parameters
     ----------
     filter_type : str
         **type**\ *width*\ [**+h**].
-        Sets the filter **type**. Choose among convolution and non-convolution
+        Set the filter **type**. Choose among convolution and non-convolution
         filters. Append the filter code followed by the full filter
         *width* in same units as time column. By default, this
         performs a low-pass filtering; append **+h** to select high-pass
         filtering. Some filters allow for optional arguments and a modifier.
 
         Available convolution filter types are:
 
@@ -78,17 +78,17 @@
         segments.
 
     end : bool
         Include ends of time series in output. The default [False] loses
         half the filter-width of data at each end.
 
     time_col : int
-        Indicates which column contains the independent variable (time). The
+        Indicate which column contains the independent variable (time). The
         left-most column is 0, while the right-most is (*n_cols* - 1)
-        [Default is 0].
+        [Default is ``0``].
 
     output_type : str
         Determine the format the xyz data will be returned in [Default is
         ``pandas``]:
 
             - ``numpy`` - :class:`numpy.ndarray`
             - ``pandas``- :class:`pandas.DataFrame`
```

### Comparing `pygmt-0.8.0/pygmt/src/grd2cpt.py` & `pygmt-0.9.0/pygmt/src/grd2cpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,19 +74,19 @@
     {aliases}
 
     Parameters
     ----------
     grid : str or xarray.DataArray
         The file name of the input grid or the grid loaded as a DataArray.
     transparency : int or float or str
-        Sets a constant level of transparency (0-100) for all color slices.
+        Set a constant level of transparency (0-100) for all color slices.
         Append **+a** to also affect the foreground, background, and NaN
-        colors [Default is no transparency, i.e., 0 (opaque)].
+        colors [Default is no transparency, i.e., ``0`` (opaque)].
     cmap : str
-        Selects the master color palette table (CPT) to use in the
+        Select the master color palette table (CPT) to use in the
         interpolation. Full list of built-in color palette tables can be found
         at :gmt-docs:`cookbook/cpts.html#built-in-color-palette-tables-cpt`.
     background : bool or str
         Select the back- and foreground colors to match the colors for lowest
         and highest *z*-values in the output CPT [Default (``background=True``
         or ``background="o"``) uses the colors specified in the master file, or
         those defined by the parameters :gmt-term:`COLOR_BACKGROUND`,
@@ -107,18 +107,18 @@
         build ranges *start*-*start+1* instead.
     nlevels : bool or int or str
         Set to ``True`` to create a linear color table by using the grid
         z-range as the new limits in the CPT. Alternatively, set *nlevels*
         to resample the color table into *nlevels* equidistant slices.
     series : list or str
         [*min/max/inc*\ [**+b**\|\ **l**\|\ **n**\]|\ *file*\|\ *list*\].
-        Defines the range of the new CPT by giving the lowest and highest
+        Define the range of the new CPT by giving the lowest and highest
         z-value (and optionally an interval). If this is not given, the
         existing range in the master CPT will be used intact. The values
-        produced defines the color slice boundaries.  If **+n** is used it
+        produced defines the color slice boundaries. If **+n** is used it
         refers to the number of such boundaries and not the number of slices.
         For details on array creation, see
         :gmt-docs:`makecpt.html#generate-1d-array`.
     truncate : list or str
         *zlo/zhi*.
         Truncate the incoming CPT so that the lowest and highest z-levels are
         to *zlo* and *zhi*. If one of these equal NaN then we leave that end of
```

### Comparing `pygmt-0.8.0/pygmt/src/grd2xyz.py` & `pygmt-0.9.0/pygmt/src/grd2xyz.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/src/grdclip.py` & `pygmt-0.9.0/pygmt/src/grdclip.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     Sa="sequence",
     Sb="sequence",
     Si="sequence",
     Sr="sequence",
 )
 def grdclip(grid, **kwargs):
     r"""
-    Sets values in a grid that meet certain criteria to a new value.
+    Set values in a grid that meet certain criteria to a new value.
 
     Produce a clipped ``outgrid`` or :class:`xarray.DataArray` version of the
     input ``grid`` file.
 
     The parameters ``above`` and ``below`` allow for a given value to be set
     for values above or below a set amount, respectively. This allows for
     extreme values in a grid, such as points below a certain depth when
```

### Comparing `pygmt-0.8.0/pygmt/src/grdcontour.py` & `pygmt-0.9.0/pygmt/src/grdcontour.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     C="interval",
     G="label_placement",
     J="projection",
     L="limit",
     Q="cut",
     R="region",
     S="resample",
-    U="timestamp",
     V="verbose",
     W="pen",
     l="label",
     c="panel",
     f="coltypes",
     p="perspective",
     t="transparency",
@@ -76,15 +75,14 @@
     {frame}
     label_placement : str
         [**d**\|\ **f**\|\ **n**\|\ **l**\|\ **L**\|\ **x**\|\ **X**]\
         *args*.
         Control the placement of labels along the quoted lines. It supports
         five controlling algorithms. See :gmt-docs:`grdcontour.html#g` for
         details.
-    {timestamp}
     {verbose}
     {pen}
     {panel}
     {coltypes}
     label : str
         Add a legend entry for the contour being plotted. Normally, the
         annotated contour is selected for the legend. You can select the
```

### Comparing `pygmt-0.8.0/pygmt/src/grdcut.py` & `pygmt-0.9.0/pygmt/src/grdcut.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/src/grdfill.py` & `pygmt-0.9.0/pygmt/src/grdfill.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/src/grdfilter.py` & `pygmt-0.9.0/pygmt/src/grdfilter.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     -------
     >>> import os
     >>> import pygmt
 
     >>> # Apply a filter of 600km (full width) to the @earth_relief_30m file
     >>> # and return a filtered field (saved as netcdf)
     >>> pygmt.grdfilter(
-    ...     grid="@earth_relief_30m",
+    ...     grid="@earth_relief_30m_g",
     ...     filter="m600",
     ...     distance="4",
     ...     region=[150, 250, 10, 40],
     ...     spacing=0.5,
     ...     outgrid="filtered_pacific.nc",
     ... )
     >>> os.remove("filtered_pacific.nc")  # cleanup file
```

### Comparing `pygmt-0.8.0/pygmt/src/grdgradient.py` & `pygmt-0.9.0/pygmt/src/grdgradient.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,23 +121,23 @@
           using the L2 norm of :math:`(g - \mbox{{offset}})` if it is not
           given.
 
         As a final option, you may add **+a**\ *ambient* to add *ambient* to
         all nodes after gradient calculations are completed.
     tiles : str
         **c**\|\ **r**\|\ **R**.
-        Controls how normalization via ``normalize`` is carried out.  When
-        multiple  grids should be normalized the same way (i.e., with the same
-        *offset*  and/or *sigma*),
-        we must pass these values via ``normalize``.  However, this is
-        inconvenient if we compute these values from a grid.  Use **c** to
-        save  the results  of *offset* and *sigma* to a statistics file; if
-        grid output is not  needed for this run then do not specify
-        ``outgrid``. For  subsequent runs,  just use **r** to read these
-        values.  Using **R**  will read then delete the statistics file.
+        Control how normalization via ``normalize`` is carried out. When
+        multiple grids should be normalized the same way (i.e., with the same
+        *offset* and/or *sigma*),
+        we must pass these values via ``normalize``. However, this is
+        inconvenient if we compute these values from a grid. Use **c** to
+        save the results of *offset* and *sigma* to a statistics file; if
+        grid output is not needed for this run then do not specify
+        ``outgrid``. For subsequent runs, just use **r** to read these
+        values. Using **R** will read then delete the statistics file.
     {region}
     slope_file : str
         Name of output grid file with scalar magnitudes of gradient vectors.
         Requires ``direction`` but makes ``outgrid`` optional.
     {verbose}
     {coltypes}
     {interpolation}
```

### Comparing `pygmt-0.8.0/pygmt/src/grdhisteq.py` & `pygmt-0.9.0/pygmt/src/grdhisteq.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,18 +80,18 @@
         outgrid : str or bool or None
             The name of the output netCDF file with extension .nc to store the
             grid in.
         outfile : str or bool or None
             The name of the output ASCII file to store the results of the
             histogram equalization in.
         output_type: str
-            Determines the output type. Use "file", "xarray", "pandas", or
+            Determine the output type. Use "file", "xarray", "pandas", or
             "numpy".
         divisions : int
-            Set the number of divisions of the data range [Default is 16].
+            Set the number of divisions of the data range [Default is ``16``].
 
         {region}
         {verbose}
         {header}
 
         Returns
         -------
```

### Comparing `pygmt-0.8.0/pygmt/src/grdimage.py` & `pygmt-0.9.0/pygmt/src/grdimage.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     G="bit_color",
     I="shading",
     J="projection",
     M="monochrome",
     N="no_clip",
     Q="nan_transparent",
     R="region",
-    U="timestamp",
     V="verbose",
     n="interpolation",
     c="panel",
     f="coltypes",
     p="perspective",
     t="transparency",
     x="cores",
@@ -109,19 +108,20 @@
         specifies that the grid is in fact an image file to be read via
         GDAL. Append **r** to assign the region specified by ``region``
         to the image. For example, if you have used ``region="d"`` then
         the image will be assigned a global domain. This mode allows you
         to project a raw image (an image without referencing coordinates).
     dpi : int
         [**i**\|\ *dpi*].
-        Sets the resolution of the projected grid that will be created if a
-        map projection other than Linear or Mercator was selected [100]. By
-        default, the projected grid will be of the same size (rows and
-        columns) as the input file. Specify **i** to use the PostScript
-        image operator to interpolate the image at the device resolution.
+        Set the resolution of the projected grid that will be created if a
+        map projection other than Linear or Mercator was selected [Default
+        is ``100`` dpi]. By default, the projected grid will be of the
+        same size (rows and columns) as the input file. Specify **i** to
+        use the PostScript image operator to interpolate the image at the
+        device resolution.
     bit_color : str
         *color*\ [**+b**\|\ **f**\].
         This parameter only applies when a resulting 1-bit image otherwise
         would consist of only two colors: black (0) and white (255). If so,
         this parameter will instead use the image as a transparent mask and
         paint the mask with the given color. Append **+b** to paint the
         background pixels (1) or **+f** for the foreground pixels
@@ -142,20 +142,24 @@
         input data is an *image* then an *intensfile* or constant *intensity*
         must be provided.
     {projection}
     monochrome : bool
         Force conversion to monochrome image using the (television) YIQ
         transformation. Cannot be used with ``nan_transparent``.
     no_clip : bool
-        Do not clip the image at the map boundary (only relevant for
-        non-rectangular maps).
-    nan_transparent : bool
+        Do **not** clip the image at the frame boundaries (only relevant
+        for non-rectangular maps) [Default is ``False``].
+    nan_transparent : bool or str
+        [**+z**\ *value*][*color*]
         Make grid nodes with z = NaN transparent, using the color-masking
         feature in PostScript Level 3 (the PS device must support PS Level
-        3).
+        3). If the input is a grid, use **+z** with a *value* to select
+        another grid value than NaN. If the input is instead an image,
+        append an alternate *color* to select another pixel value to be
+        transparent [Default is ``"black"``].
     {region}
     {verbose}
     {panel}
     {coltypes}
     {interpolation}
     {perspective}
     {transparency}
```

### Comparing `pygmt-0.8.0/pygmt/src/grdinfo.py` & `pygmt-0.9.0/pygmt/src/grdinfo.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     ----------
     grid : str or xarray.DataArray
         The file name of the input grid or the grid loaded as a DataArray.
         This is the only required parameter.
     {region}
     per_column : str or bool
         **n**\|\ **t**.
-        Formats the report using tab-separated fields on a single line. The
+        Format the report using tab-separated fields on a single line. The
         output is name *w e s n z0 z1 dx dy nx ny* [ *x0 y0 x1 y1* ]
         [ *med scale* ] [ *mean std rms* ] [ *n_nan* ] *registration gtype*.
         The data in brackets are outputted depending on the ``force_scan``
         and ``minmax_pos`` parameters. Use **t** to place file name at the end
         of the output record or, **n** or ``True`` to only output numerical
         columns. The registration is either 0 (gridline) or 1 (pixel), while
         gtype is either 0 (Cartesian) or 1 (geographic). The default value is
@@ -76,35 +76,36 @@
         grid region instead). If no argument is given then we report the grid
         increment in the form *xinc*\ [/*yinc*]. If **b** is given we write
         each grid's bounding box polygon instead. Finally, if ``tiles`` is in
         effect then *dx* and *dy* are the dimensions of the desired tiles.
     force_scan : int or str
         **0**\|\ **1**\|\ **2**\|\ **p**\|\ **a**.
 
-        **0**\ : Report range of z after actually scanning the data, not just
-        reporting what the header says.
-        **1**\ : Report median and L1 scale of z (L1 scale = 1.4826 * Median
-        Absolute Deviation (MAD)).
-        **2**\ : Report mean, standard deviation, and root-mean-square (rms)
-        of z.
-        **p**\ : Report mode (LMS) and LMS scale of z.
-        **a**\ : Include all of the above.
-    minxmax_pos : bool
+        - **0**: Report range of z after actually scanning the data, not just
+          reporting what the header says.
+        - **1**: Report median and L1 scale of z (L1 scale = 1.4826 * Median
+          Absolute Deviation (MAD)).
+        - **2**: Report mean, standard deviation, and root-mean-square (rms)
+          of z.
+        - **p**: Report mode (LMS) and LMS scale of z.
+        - **a**: Include all of the above.
+    minmax_pos : bool
         Include the x/y values at the location of the minimum and maximum
         z-values.
     nearest_multiple : str
         [*dz*]\ [**+a**\ [*alpha*]]\ [**+s**].
-        Determine min and max z-value. If *dz* is provided then we first round
-        these values off to multiples of *dz*. To exclude the two tails of the
-        distribution when determining the min and max you can add **+a** to
-        set the *alpha* value (in percent): We then sort the grid, exclude the
-        data in the 0.5*\ *alpha* and 100 - 0.5*\ *alpha* tails, and revise
-        the min and max. To force a symmetrical range about zero, using
-        minus/plus the max absolute value of the two extremes, append **+s**\ .
-        We report the result via the text string *zmin/zmax* or *zmin/zmax/dz*
+        Determine minimum and maximum z-values. If *dz* is provided then we
+        first round these values off to multiples of *dz*. To exclude the
+        two tails of the distribution when determining the minimum and
+        maximum you can add **+a** to set the *alpha* value (in percent):
+        We then sort the grid, exclude the data in the 0.5*\ *alpha* and
+        100 - 0.5*\ *alpha* tails, and revise the minimum and maximum. To
+        force a symmetrical range about zero, using minus/plus the maximum
+        absolute value of the two extremes, append **+s**. We report the
+        result via the text string *zmin/zmax* or *zmin/zmax/dz*
         (if *dz* was given) as expected by :func:`pygmt.makecpt`.
     {verbose}
     {coltypes}
 
     Returns
     -------
     info : str
```

### Comparing `pygmt-0.8.0/pygmt/src/grdlandmask.py` & `pygmt-0.9.0/pygmt/src/grdlandmask.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     outgrid : str or None
         The name of the output netCDF file with extension .nc to store the grid
         in.
     {spacing}
     {region}
     {area_thresh}
     resolution : str
-        *res*\[\ **+f**\]. Selects the resolution of the data set to use
+        *res*\[\ **+f**\]. Select the resolution of the data set to use
         ((**f**)ull, (**h**)igh, (**i**)ntermediate, (**l**)ow, or
         (**c**)rude). The resolution drops off by ~80% between data sets.
         [Default is **l**]. Append **+f** to automatically select a lower
         resolution should the one requested not be available
         [abort if not found]. Alternatively, choose (**a**)uto to automatically
         select the best resolution given the chosen region. Note that because
         the coastlines differ in details a node in a mask file using one
@@ -73,15 +73,15 @@
         node values for all cells traversed by a line to the corresponding
         border value. Here, *cborder* is used for cells traversed by the
         coastline, *lborder* for cells traversed by a lake outline, *iborder*
         for islands-in-lakes outlines, and *pborder* for
         ponds-in-islands-in-lakes outlines [Default is no line tracing].
     maskvalues : str or list
         [*wet*, *dry*] or [*ocean*, *land*, *lake*, *island*, *pond*].
-        Sets the values that will be assigned to nodes. Values can
+        Set the values that will be assigned to nodes. Values can
         be any number, including the textstring NaN
         [Default is [0, 1, 0, 1, 0] (i.e., [0, 1])]. Also select
         ``bordervalues`` to let nodes exactly on feature boundaries be
         considered outside [Default is inside].
     {verbose}
     {registration}
```

### Comparing `pygmt-0.8.0/pygmt/src/grdproject.py` & `pygmt-0.9.0/pygmt/src/grdproject.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,21 +75,23 @@
         northings for particular projection zones [0/0].
     {spacing}
     dpi : int
         Set the resolution for the new grid in dots per inch.
     scaling : str
         [**c**\|\ **i**\|\ **p**\|\ **e**\|\ **f**\|\
         **k**\|\ **M**\|\ **n**\|\ **u**].
-        Force 1:1 scaling, i.e., output or output data are in actual projected
-        meters [**e**]. To specify other units, append **f** (foot),
-        **k** (km), **M** (statute mile), **n** (nautical mile), **u**
-        (US survey foot), **i** (inch), **c** (cm), or **p** (point).
+        Force 1:1 scaling, i.e., output or input data are in actual projected
+        meters [**e**]. To specify other units, append **f** (feet),
+        **k** (kilometers), **M** (statute miles), **n** (nautical miles),
+        **u** (US survey feet), **i** (inches), **c** (centimeters), or
+        **p** (points).
     unit : str
-        Append **c**, **i**, or **p** to indicate that cm, inch, or point
-        should be the projected measure unit. Cannot be used with ``scaling``.
+        Append **c**, **i**, or **p** to indicate that centimeters, inches, or
+        points should be the projected measure unit. Cannot be used with
+        ``scaling``.
     {verbose}
     {interpolation}
     {registration}
 
     Returns
     -------
     ret: xarray.DataArray or None
```

### Comparing `pygmt-0.8.0/pygmt/src/grdsample.py` & `pygmt-0.9.0/pygmt/src/grdsample.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/src/grdtrack.py` & `pygmt-0.9.0/pygmt/src/grdtrack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 """
 grdtrack - Sample grids at specified (x,y) locations.
 """
-import warnings
-
 import pandas as pd
-import xarray as xr
 from pygmt.clib import Session
 from pygmt.exceptions import GMTInvalidInput
 from pygmt.helpers import (
     GMTTempFile,
     build_arg_string,
     fmt_docstring,
     kwargs_to_strings,
     use_alias,
 )
-from pygmt.src.which import which
 
 __doctest_skip__ = ["grdtrack"]
 
 
 @fmt_docstring
 @use_alias(
     A="resample",
@@ -115,16 +111,16 @@
         as we look in the direction of the input line segment). Append **+a**
         to alternate the direction of cross-profiles, or **v** to enforce
         either a "west-to-east" or "south-to-north" view. By default the entire
         profiles are output. Choose to only output the left or right halves
         of the profiles by appending **+l** or **+r**, respectively.  Append
         suitable units to *length*; it sets the unit used for *ds* [and
         *spacing*] (See :gmt-docs:`Units <grdtrack.html#units>`). The default
-        unit for geographic grids is meter while Cartesian grids implies the
-        user unit.  The output columns will be *lon*, *lat*, *dist*, *azimuth*,
+        unit for geographic grids is meters while Cartesian grids implies the
+        user unit. The output columns will be *lon*, *lat*, *dist*, *azimuth*,
         *z1*, *z2*, ..., *zn* (The *zi* are the sampled values for each of the
         *n* grids).
     dfile : str
         In concert with ``crossprofile`` we can save the (possibly resampled)
         original lines to *dfile* [Default only saves the cross-profiles]. The
         columns will be *lon*, *lat*, *dist*, *azimuth*, *z1*, *z2*, ...
         (sampled value for each grid).
@@ -293,37 +289,14 @@
 
     if points is None and kwargs.get("E") is None:
         raise GMTInvalidInput("Must give 'points' or set 'profile'.")
 
     if hasattr(points, "columns") and newcolname is None:
         raise GMTInvalidInput("Please pass in a str to 'newcolname'")
 
-    # Backward compatibility with old parameter order "points, grid".
-    # deprecated_version="0.7.0", remove_version="v0.9.0"
-    is_a_grid = True
-    if not isinstance(grid, (xr.DataArray, str)):
-        is_a_grid = False
-    elif isinstance(grid, str):
-        try:
-            xr.open_dataarray(which(grid, download="a"), engine="netcdf4").close()
-            is_a_grid = True
-        except (ValueError, OSError):
-            is_a_grid = False
-    if not is_a_grid:
-        msg = (
-            "Positional parameters 'points, grid' of pygmt.grdtrack() has changed "
-            "to 'grid, points=None' since v0.7.0. It's likely that you're NOT "
-            "passing a valid grid as the first positional argument or "
-            "are passing an invalid grid to the 'grid' parameter. "
-            "Please check the order of arguments with the latest documentation. "
-            "This warning will be removed in v0.9.0."
-        )
-        grid, points = points, grid
-        warnings.warn(msg, category=FutureWarning, stacklevel=1)
-
     with GMTTempFile(suffix=".csv") as tmpfile:
         with Session() as lib:
             # Store the xarray.DataArray grid in virtualfile
             grid_context = lib.virtualfile_from_data(check_kind="raster", data=grid)
 
             with grid_context as grdfile:
                 kwargs.update({"G": grdfile})
```

### Comparing `pygmt-0.8.0/pygmt/src/grdview.py` & `pygmt-0.9.0/pygmt/src/grdview.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,14 +9,16 @@
     build_arg_string,
     data_kind,
     fmt_docstring,
     kwargs_to_strings,
     use_alias,
 )
 
+__doctest_skip__ = ["grdview"]
+
 
 @fmt_docstring
 @use_alias(
     R="region",
     J="projection",
     Jz="zscale",
     JZ="zsize",
@@ -73,19 +75,19 @@
         The file name or a DataArray of the image grid to be draped on top
         of the relief provided by grid. [Default determines colors from
         grid]. Note that ``zscale`` and ``plane`` always refers to the grid.
         The drapegrid only provides the information pertaining to colors, which
         (if drapegrid is a grid) will be looked-up via the CPT (see ``cmap``).
     plane : float or str
         *level*\ [**+g**\ *fill*].
-        Draws a plane at this z-level. If the optional color is provided
+        Draw a plane at this z-level. If the optional color is provided
         via the **+g** modifier, and the projection is not oblique, the frontal
         facade between the plane and the data perimeter is colored.
     surftype : str
-        Specifies cover type of the grid.
+        Specify cover type of the grid.
         Select one of following settings:
 
         - **m** - mesh plot [Default].
         - **mx** or **my** - waterfall plots (row or column profiles).
         - **s** - surface plot, and optionally append **m** to have mesh lines
           drawn on top of the surface.
         - **i** - image plot.
@@ -93,18 +95,18 @@
 
         For any of these choices, you may force a monochrome image by
         appending the modifier **+m**.
     contourpen : str
         Draw contour lines on top of surface or mesh (not image). Append
         pen attributes used for the contours.
     meshpen : str
-        Sets the pen attributes used for the mesh. You must also select
+        Set the pen attributes used for the mesh. You must also select
         ``surftype`` of **m** or **sm** for meshlines to be drawn.
     facadepen :str
-        Sets the pen attributes used for the facade. You must also select
+        Set the pen attributes used for the facade. You must also select
         ``plane`` for the facade outline to be drawn.
     shading : str
         Provide the name of a grid file with intensities in the (-1,+1)
         range, or a constant intensity to apply everywhere (affects the
         ambient light). Alternatively, derive an intensity grid from the
         input data grid reliefgrid via a call to :func:`pygmt.grdgradient`;
         append **+a**\ *azimuth*, **+n**\ *args*, and **+m**\ *ambient* to
@@ -113,14 +115,47 @@
         [Default is **+a**\ -45\ **+nt**\ 1\ **+m**\ 0].
     {verbose}
     {panel}
     {coltypes}
     {interpolation}
     {perspective}
     {transparency}
+
+    Example
+    -------
+    >>> import pygmt
+    >>> # load the 30 arc-minutes grid with "gridline" registration
+    >>> # in a specified region
+    >>> grid = pygmt.datasets.load_earth_relief(
+    ...     resolution="30m",
+    ...     region=[-92.5, -82.5, -3, 7],
+    ...     registration="gridline",
+    ... )
+    >>> # create a new figure instance with pygmt.Figure()
+    >>> fig = pygmt.Figure()
+    >>> # create the contour plot
+    >>> fig.grdview(
+    ...     # pass in the grid downloaded above
+    ...     grid=grid,
+    ...     # set the perspective to an azimuth of 130° and an elevation of 30°
+    ...     perspective=[130, 30],
+    ...     # add a frame to the x- and y-axes
+    ...     # specify annotations on the south and east borders of the plot
+    ...     frame=["xa", "ya", "wSnE"],
+    ...     # set the projection of the 2-D map to Mercator with a 10 cm width
+    ...     projection="M10c",
+    ...     # set the vertical scale (z-axis) to 2 cm
+    ...     zsize="2c",
+    ...     # set "surface plot" to color the surface via a CPT
+    ...     surftype="s",
+    ...     # specify CPT to "geo"
+    ...     cmap="geo",
+    ... )
+    >>> # show the plot
+    >>> fig.show()
     """
     kwargs = self._preprocess(**kwargs)  # pylint: disable=protected-access
     with Session() as lib:
         file_context = lib.virtualfile_from_data(check_kind="raster", data=grid)
 
         with contextlib.ExitStack() as stack:
             if kwargs.get("G") is not None:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pygmt-0.8.0/pygmt/src/grdvolume.py` & `pygmt-0.9.0/pygmt/src/grdvolume.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/src/histogram.py` & `pygmt-0.9.0/pygmt/src/histogram.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     J="projection",
     L="extreme",
     N="distribution",
     Q="cumulative",
     R="region",
     S="stairs",
     T="series",
-    U="timestamp",
     V="verbose",
     W="pen",
     Z="histtype",
     b="binary",
     c="panel",
     d="nodata",
     e="find",
@@ -37,75 +36,75 @@
     w="wrap",
 )
 @kwargs_to_strings(
     R="sequence", T="sequence", c="sequence_comma", i="sequence_comma", p="sequence"
 )
 def histogram(self, data, **kwargs):
     r"""
-    Plots a histogram, and can read data from a file or list, array, or
-    dataframe.
+    Plot Cartesian histograms.
 
     Full option list at :gmt-docs:`histogram.html`
 
     {aliases}
 
     Parameters
     ----------
     data : str or list or {table-like}
         Pass in either a file name to an ASCII data table, a Python list, a 2-D
         {table-classes}.
     {projection}
     {region}
     {frame}
     {cmap}
-    {fill}
+    fill : str
+         Set color or pattern for filling bars [Default is no fill].
     {pen}
     {panel}
     annotate : bool or str
         [**+b**][**+f**\ *font*][**+o**\ *off*][**+r**].
-        Annotate each bar with the count it represents.  Append any of the
+        Annotate each bar with the count it represents. Append any of the
         following modifiers: Use **+b** to place the labels beneath the bars
         instead of above; use **+f** to change to another font than the default
         annotation font; use **+o** to change the offset between bar and
-        label [6p]; use **+r** to rotate the labels from horizontal to
-        vertical.
+        label [Default is ``"6p"``]; use **+r** to rotate the labels from
+        horizontal to vertical.
     barwidth : int or float or str
         *width*\ [**+o**\ *offset*].
         Use an alternative histogram bar width than the default set via
-        ``series``, and optionally shift all bars by an *offset*.  Here
+        ``series``, and optionally shift all bars by an *offset*. Here
         *width* is either an alternative width in data units, or the user may
         append a valid plot dimension unit (**c**\|\ **i**\|\ **p**) for a
         fixed dimension instead. Optionally, all bins may be shifted along the
         axis by *offset*. As for *width*, it may be given in data units of
         plot dimension units by appending the relevant unit.
     center : bool
         Center bin on each value. [Default is left edge].
     distribution : bool or int or float or str
         [*mode*][**+p**\ *pen*].
         Draw the equivalent normal distribution; append desired
-        *pen* [Default is 0.25p,black].
+        *pen* [Default is ``"0.25p,black,solid"``].
         The *mode* selects which central location and scale to use:
 
         * 0 = mean and standard deviation [Default];
         * 1 = median and L1 scale (1.4826 \* median absolute deviation; MAD);
         * 2 = LMS (least median of squares) mode and scale.
     cumulative : bool or str
         [**r**].
         Draw a cumulative histogram by passing ``True``. Use **r** to display
         a reverse cumulative histogram.
     extreme : str
         **l**\|\ **h**\|\ **b**.
         The modifiers specify the handling of extreme values that fall outside
-        the range set by ``series``.  By default these values are ignored.
+        the range set by ``series``. By default, these values are ignored.
         Append **b** to let these values be included in the first or last
         bins. To only include extreme values below first bin into the first
         bin, use **l**, and to only include extreme values above the last bin
         into that last bin, use **h**.
     stairs : bool
-        Draws a stairs-step diagram which does not include the internal bars
+        Draw a stairs-step diagram which does not include the internal bars
         of the default histogram.
     horizontal : bool
         Plot the histogram using horizontal bars instead of the
         default vertical bars.
     series : int or str or list
         [*min*\ /*max*\ /]\ *inc*\ [**+n**\ ].
         Set the interval for the width of each bar in the histogram.
@@ -118,15 +117,14 @@
         * 2 = log (1.0 + count)
         * 3 = log (1.0 + frequency_percent)
         * 4 = log10 (1.0 + count)
         * 5 = log10 (1.0 + frequency_percent).
 
         To use weights provided as a second data column instead of pure counts,
         append **+w**.
-    {timestamp}
     {verbose}
     {binary}
     {nodata}
     {find}
     {header}
     {incols}
     {label}
```

### Comparing `pygmt-0.8.0/pygmt/src/image.py` & `pygmt-0.9.0/pygmt/src/image.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 @fmt_docstring
 @use_alias(
     R="region",
     J="projection",
     D="position",
     F="box",
     M="monochrome",
-    U="timestamp",
     V="verbose",
     c="panel",
     p="perspective",
     t="transparency",
 )
 @kwargs_to_strings(R="sequence", c="sequence_comma", p="sequence")
 def image(self, imagefile, **kwargs):
@@ -40,24 +39,23 @@
         then only EPS files are supported.
     {projection}
     {region}
     position : str
         [**g**\|\ **j**\|\ **J**\|\ **n**\|\ **x**]\ *refpoint*\ **+r**\ *dpi*\
         **+w**\ [**-**]\ *width*\ [/*height*]\ [**+j**\ *justify*]\
         [**+n**\ *nx*\ [/*ny*] ]\ [**+o**\ *dx*\ [/*dy*]].
-        Sets reference point on the map for the image.
+        Set reference point on the map for the image.
     box : bool or str
         [**+c**\ *clearances*][**+g**\ *fill*][**+i**\ [[*gap*/]\ *pen*]]\
         [**+p**\ [*pen*]][**+r**\ [*radius*]][**+s**\ [[*dx*/*dy*/][*shade*]]].
-        Without further arguments, draws a rectangular border around the image
+        If set to ``True``, draw a rectangular border around the image
         using :gmt-term:`MAP_FRAME_PEN`.
     monochrome : bool
         Convert color image to monochrome grayshades using the (television)
         YIQ-transformation.
-    {timestamp}
     {verbose}
     {panel}
     {perspective}
     {transparency}
     """
     kwargs = self._preprocess(**kwargs)  # pylint: disable=protected-access
     with Session() as lib:
```

### Comparing `pygmt-0.8.0/pygmt/src/info.py` & `pygmt-0.9.0/pygmt/src/info.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/src/inset.py` & `pygmt-0.9.0/pygmt/src/inset.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,73 +43,72 @@
 
         *This is the only required parameter.*
         Define the map inset rectangle on the map. Specify the rectangle
         in one of three ways:
 
         Append **g**\ *lon*/*lat* for map (user) coordinates,
         **j**\ *code* or **J**\ *code* for setting the *refpoint* via a
-        2-char justification code that refers to the (invisible)
+        2-character justification code that refers to the (invisible)
         projected map bounding box, **n**\ *xn*/*yn* for normalized (0-1)
         bounding box coordinates, or **x**\ *x*/*y* for plot
-        coordinates (inches, cm, points, append unit).
+        coordinates (inches, centimeters, points, append unit).
         All but **x** requires both ``region`` and ``projection`` to be
         specified. You can offset the reference point via
         **+o**\ *dx*/*dy* in the direction implied by *code* or
         **+j**\ *justify*.
 
         Alternatively, give *west/east/south/north* of geographic
         rectangle bounded by parallels and meridians; append **+r** if the
         coordinates instead are the lower left and upper right corners of
         the desired rectangle. (Or, give *xmin/xmax/ymin/ymax* of bounding
         rectangle in projected coordinates and optionally
-        append **+u**\ *unit* [Default coordinate unit is meter (e)].
+        append **+u**\ *unit* [Default coordinate unit is meters (**e**)].
 
         Append **+w**\ *width*\ [/*height*] of bounding rectangle or box
-        in plot coordinates (inches, cm, etc.). By default, the anchor
-        point on the scale is assumed to be the bottom left corner (**BL**),
-        but this can be changed by appending **+j** followed by a 2-char
-        justification code *justify*.
+        in plot coordinates (inches, centimeters, etc.). By default, the
+        anchor point on the scale is assumed to be the bottom left corner
+        (**BL**), but this can be changed by appending **+j** followed by
+        a 2-character justification code *justify*.
         **Note**: If **j** is used then *justify* defaults to the same
         as *refpoint*, if **J** is used then *justify* defaults to the
         mirror opposite of *refpoint*. Specify inset box attributes via
         the ``box`` parameter [Default is outline only].
     box : str or bool
         [**+c**\ *clearances*][**+g**\ *fill*][**+i**\ [[*gap*/]\
         *pen*]][**+p**\ [*pen*]][**+r**\ [*radius*]][**+s**\
         [[*dx*/*dy*/][*shade*]]].
-
-        If passed ``True``, this draws a rectangular box around the map
+        If set to ``True``, draw a rectangular box around the map
         inset using the default pen; specify a different pen
         with **+p**\ *pen*. Add **+g**\ *fill* to fill the logo box
         [Default is no fill].
         Append **+c**\ *clearance*  where *clearance* is either
         *gap*, *xgap*\ /\ *ygap*, or *lgap*\ /\ *rgap*\ /\ *bgap*\ /\
         *tgap* where these items are uniform, separate in x- and
         y-direction, or individual side spacings between logo and border.
         Append **+i** to draw a secondary, inner border as well. We use a
         uniform *gap* between borders of 2\ **p** and the default pen
         unless other values are specified. Append **+r** to draw rounded
         rectangular borders instead, with a 6p corner radius. You
         can override this radius by appending another value. Append
         **+s** to draw an offset background shaded region. Here, *dx*/*dy*
-        indicates the shift relative to the foreground frame
-        [4p/-4p] and ``shade`` sets the fill style to use for
-        shading [Default is gray50].
+        indicates the shift relative to the foreground frame [Default is
+        ``"4p/-4p"``] and ``shade`` sets the fill style to use for
+        shading [Default is ``"gray50"``].
     margin : int or str or list
         This is clearance that is added around the inside of the inset.
         Plotting will take place within the inner region only. The margins
         can be a single value, a pair of values separated (for setting
         separate horizontal and vertical margins), or the full set of four
         margins (for setting separate left, right, bottom, and top
         margins). When passing multiple values, it can be either a list or
         a string with the values separated by forward
         slashes [Default is no margins].
     no_clip : bool
-        Do NOT clip features extruding outside map inset boundaries [Default
-        is clip].
+        Do **not** clip features extruding outside the inset frame
+        boundaries [Default is ``False``].
     {region}
     {projection}
     {verbose}
 
     Examples
     --------
     >>> import pygmt
@@ -127,16 +126,15 @@
     ...         land="gray",
     ...         water="white",
     ...         dcw="MG+gred",
     ...     )
     ...
     >>> # Map elements outside the "with" block are plotted in the main figure
     >>> fig.logo(position="jBR+o0.2c+w3c")
-    >>> fig.show()  # doctest: +SKIP
-    <IPython.core.display.Image object>
+    >>> fig.show()
     """
     kwargs = self._preprocess(**kwargs)  # pylint: disable=protected-access
     with Session() as lib:
         try:
             lib.call_module(module="inset", args=f"begin {build_arg_string(kwargs)}")
             yield
         finally:
```

### Comparing `pygmt-0.8.0/pygmt/src/legend.py` & `pygmt-0.9.0/pygmt/src/legend.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 @fmt_docstring
 @use_alias(
     R="region",
     J="projection",
     D="position",
     F="box",
-    U="timestamp",
     V="verbose",
     c="panel",
     p="perspective",
     t="transparency",
 )
 @kwargs_to_strings(R="sequence", c="sequence_comma", p="sequence")
 def legend(self, spec=None, position="JTR+jTR+o0.2c", box="+gwhite+p1p", **kwargs):
@@ -48,26 +47,25 @@
         specification file.
     {projection}
     {region}
     position : str
         [**g**\|\ **j**\|\ **J**\|\ **n**\|\ **x**]\ *refpoint*\
         **+w**\ *width*\ [/*height*]\ [**+j**\ *justify*]\ [**+l**\ *spacing*]\
         [**+o**\ *dx*\ [/*dy*]].
-        Defines the reference point on the map for the
+        Define the reference point on the map for the
         legend. By default, uses **JTR**\ **+jTR**\ **+o**\ 0.2c which
         places the legend at the top-right corner inside the map frame, with a
         0.2 cm offset.
     box : bool or str
         [**+c**\ *clearances*][**+g**\ *fill*][**+i**\ [[*gap*/]\ *pen*]]\
         [**+p**\ [*pen*]][**+r**\ [*radius*]][**+s**\ [[*dx*/*dy*/][*shade*]]].
-        Without further arguments, draws a rectangular border around the legend
+        If set to ``True``, draw a rectangular border around the legend
         using :gmt-term:`MAP_FRAME_PEN`. By default, uses
         **+g**\ white\ **+p**\ 1p which draws a box around the legend using a
         1p black pen and adds a white background.
-    {timestamp}
     {verbose}
     {panel}
     {perspective}
     {transparency}
     """
     kwargs = self._preprocess(**kwargs)  # pylint: disable=protected-access
```

### Comparing `pygmt-0.8.0/pygmt/src/logo.py` & `pygmt-0.9.0/pygmt/src/logo.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 @fmt_docstring
 @use_alias(
     R="region",
     J="projection",
     D="position",
     F="box",
     S="style",
-    U="timestamp",
     V="verbose",
     c="panel",
     t="transparency",
 )
 @kwargs_to_strings(R="sequence", c="sequence_comma", p="sequence")
 def logo(self, **kwargs):
     r"""
@@ -35,27 +34,26 @@
     Parameters
     ----------
     {projection}
     {region}
     position : str
         [**g**\|\ **j**\|\ **J**\|\ **n**\|\ **x**]\ *refpoint*\
         **+w**\ *width*\ [**+j**\ *justify*]\ [**+o**\ *dx*\ [/*dy*]].
-        Sets reference point on the map for the image.
+        Set reference point on the map for the image.
     box : bool or str
-        Without further arguments, draws a rectangular border around the
+        If set to ``True``, draw a rectangular border around the
         GMT logo.
     style : str
         [**l**\|\ **n**\|\ **u**].
         Control what is written beneath the map portion of the logo.
 
         - **l** to plot the text label "The Generic Mapping Tools"
           [Default]
         - **n** to skip the label placement
         - **u** to place the URL to the GMT site
-    {timestamp}
     {verbose}
     {panel}
     {transparency}
     """
     kwargs = self._preprocess(**kwargs)  # pylint: disable=protected-access
     with Session() as lib:
         lib.call_module(module="logo", args=build_arg_string(kwargs))
```

### Comparing `pygmt-0.8.0/pygmt/src/makecpt.py` & `pygmt-0.9.0/pygmt/src/makecpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,19 +61,19 @@
     Full option list at :gmt-docs:`makecpt.html`
 
     {aliases}
 
     Parameters
     ----------
     transparency : str
-        Sets a constant level of transparency (0-100) for all color slices.
+        Set a constant level of transparency (0-100) for all color slices.
         Append **+a** to also affect the foreground, background, and NaN
-        colors [Default is no transparency, i.e., 0 (opaque)].
+        colors [Default is no transparency, i.e., ``0`` (opaque)].
     cmap : str
-        Selects the master color palette table (CPT) to use in the
+        Select the master color palette table (CPT) to use in the
         interpolation. Full list of built-in color palette tables can be found
         at :gmt-docs:`cookbook/cpts.html#built-in-color-palette-tables-cpt`.
     background : bool or str
         Select the back- and foreground colors to match the colors for lowest
         and highest *z*-values in the output CPT [Default (``background=True``
         or ``background="o"``) uses the colors specified in the master file, or
         those defined by the parameters :gmt-term:`COLOR_BACKGROUND`,
@@ -90,15 +90,15 @@
         CPT is plotted. The *label* may be a comma-separated list of category
         names (you can skip a category by not giving a name), or give
         *start*\[**-**], where we automatically build monotonically increasing
         labels from *start* (a single letter or an integer). Append **-** to
         build ranges *start*-*start+1* instead.
     series : list or str
         [*min/max/inc*\[**+b**\|\ **l**\|\ **n**]\|\ *file*\|\ *list*].
-        Defines the range of the new CPT by giving the lowest and highest
+        Define the range of the new CPT by giving the lowest and highest
         z-value (and optionally an interval). If this is not given, the
         existing range in the master CPT will be used intact. The values
         produced defines the color slice boundaries.  If **+n** is used it
         refers to the number of such boundaries and not the number of slices.
         For details on array creation, see
         :gmt-docs:`makecpt.html#generate-1d-array`.
     truncate : list or str
```

### Comparing `pygmt-0.8.0/pygmt/src/meca.py` & `pygmt-0.9.0/pygmt/src/meca.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,20 +71,24 @@
     if convention in ["a", "c", "m", "d", "z", "p", "x", "y", "t"]:
         return convention
     raise GMTInvalidInput(f"Invalid convention '{convention}'.")
 
 
 @fmt_docstring
 @use_alias(
-    R="region",
-    J="projection",
     A="offset",
     B="frame",
+    C="cmap",
+    E="extensionfill",
+    G="compressionfill",
+    J="projection",
     N="no_clip",
+    R="region",
     V="verbose",
+    W="pen",
     c="panel",
     p="perspective",
     t="transparency",
 )
 @kwargs_to_strings(R="sequence", c="sequence_comma", p="sequence")
 def meca(
     self,
@@ -105,15 +109,15 @@
 
     Full option list at :gmt-docs:`supplements/seis/meca.html`
 
     {aliases}
 
     Parameters
     ----------
-    spec: str, 1-D array, 2-D array, dict, or pd.DataFrame
+    spec : str, 1-D array, 2-D array, dict, or pd.DataFrame
         Data that contains focal mechanism parameters.
 
         ``spec`` can be specified in either of the following types:
 
         - *str*: a file name containing focal mechanism parameters as
           columns. The meaning of each column is:
 
@@ -128,96 +132,112 @@
             ``offset=True`` to take effect].
           - Text string to appear near the beachball [optional].
 
         - *1-D array*: focal mechanism parameters of a single event.
           The meanings of columns are the same as above.
         - *2-D array*: focal mechanim parameters of multiple events.
           The meanings of columns are the same as above.
-        - *dict or pd.DataFrame*: The dict keys or pd.DataFrame column names
-          determine the focal mechanims convention. For different conventions,
-          the following combination of keys are allowed:
+        - *dictionary or pd.DataFrame*: The dictionary keys or pd.DataFrame
+          column names determine the focal mechanims convention. For
+          different conventions, the following combination of keys are allowed:
 
           - ``"aki"``: *strike, dip, rake, magnitude*
           - ``"gcmt"``: *strike1, dip1, rake1, strike2, dip2, rake2, mantissa,*
             *exponent*
           - ``"mt"``: *mrr, mtt, mff, mrt, mrf, mtf, exponent*
           - ``"partial"``: *strike1, dip1, strike2, fault_type, magnitude*
           - ``"principal_axis"``: *t_value, t_azimuth, t_plunge, n_value,
             n_azimuth, n_plunge, p_value, p_azimuth, p_plunge, exponent*
 
-          A dict may contain values for a single focal mechanism or lists of
-          values for multiple focal mechanisms.
+          A dictionary may contain values for a single focal mechanism or
+          lists of values for multiple focal mechanisms.
 
-          Both dict and pd.DataFrame may optionally contain keys/column names:
-          ``latitude``, ``longitude``, ``depth``, ``plot_longitude``,
-          ``plot_latitude``, and/or ``event_name``.
+          Both dictionary and pd.DataFrame may optionally contain
+          keys/column names: ``latitude``, ``longitude``, ``depth``,
+          ``plot_longitude``, ``plot_latitude``, and/or ``event_name``.
 
           If ``spec`` is either a str, a 1-D array or a 2-D array, the
           ``convention`` parameter is required so we know how to interpret the
-          columns. If ``spec`` is a dict or a pd.DataFrame, ``convention`` is
-          not needed and is ignored if specified.
+          columns. If ``spec`` is a dictionary or a pd.DataFrame,
+          ``convention`` is not needed and is ignored if specified.
 
-    scale: str
-        Adjusts the scaling of the radius of the beachball, which is
+    scale : str
+        Adjust the scaling of the radius of the beachball, which is
         proportional to the magnitude. *scale* defines the size for
         magnitude = 5 (i.e. scalar seismic moment M0 = 4.0E23 dynes-cm).
-    convention: str
+    convention : str
         Focal mechanism convention. Choose from:
 
         - ``"aki"`` (Aki & Richards)
         - ``"gcmt"`` (global CMT)
         - ``"mt"`` (seismic moment tensor)
         - ``"partial"`` (partial focal mechanism)
         - ``"principal_axis"`` (principal axis)
 
         Ignored if ``spec`` is a dictionary or pd.DataFrame.
-    component: str
+    component : str
         The component of the seismic moment tensor to plot.
 
         - ``"full"``: the full seismic moment tensor
         - ``"dc"``: the closest double couple defined from the moment tensor
           (zero trace and zero determinant)
         - ``"deviatoric"``: deviatoric part of the moment tensor (zero trace)
-    longitude: int, float, list, or 1-D numpy array
-        Longitude(s) of event location. Must be the same length as the
+    longitude : int, float, list, or 1-D numpy array
+        Longitude(s) of event location(s). Must be the same length as the
         number of events. Will override the ``longitude`` values
-        in ``spec`` if ``spec`` is a dict or pd.DataFrame.
-    latitude: int, float, list, or 1-D numpy array
-        Latitude(s) of event location. Must be the same length as the
+        in ``spec`` if ``spec`` is a dictionary or pd.DataFrame.
+    latitude : int, float, list, or 1-D numpy array
+        Latitude(s) of event location(s). Must be the same length as the
         number of events. Will override the ``latitude`` values
-        in ``spec`` if ``spec`` is a dict or pd.DataFrame.
-    depth: int, float, list, or 1-D numpy array
-        Depth(s) of event location in kilometers. Must be the same length as
-        the number of events. Will override the ``depth`` values in ``spec``
-        if ``spec`` is a dict or pd.DataFrame.
-    plot_longitude: int, float, str, list, or 1-D numpy array
-        Longitude(s) at which to place beachball. Must be the same length as
-        the number of events. Will override the ``plot_longitude`` values in
-        ``spec`` if ``spec`` is a dict or pd.DataFrame.
-    plot_latitude: int, float, str, list, or 1-D numpy array
-        Latitude(s) at which to place beachball. List must be the same length
-        as the number of events. Will override the ``plot_latitude`` values in
-        ``spec`` if ``spec`` is a dict or pd.DataFrame.
+        in ``spec`` if ``spec`` is a dictionary or pd.DataFrame.
+    depth : int, float, list, or 1-D numpy array
+        Depth(s) of event location(s) in kilometers. Must be the same length
+        as the number of events. Will override the ``depth`` values in ``spec``
+        if ``spec`` is a dictionary or pd.DataFrame.
+    plot_longitude : int, float, str, list, or 1-D numpy array
+        Longitude(s) at which to place beachball(s). Must be the same length
+        as the number of events. Will override the ``plot_longitude`` values
+        in ``spec`` if ``spec`` is a dictionary or pd.DataFrame.
+    plot_latitude : int, float, str, list, or 1-D numpy array
+        Latitude(s) at which to place beachball(s). List must be the same
+        length as the number of events. Will override the ``plot_latitude``
+        values in ``spec`` if ``spec`` is a dictionary or pd.DataFrame.
     event_name : str or list of str, or 1-D numpy array
-        Text strings (e.g., event names) to appear near the beachball. List
-        must be the same length as the number of events. Will override the
-        ``event_name`` values in ``spec`` if ``spec`` is a dict or
-        pd.DataFrame.
-    offset: bool or str
+        Text string(s), e.g., event name(s) to appear near the beachball(s).
+        List must be the same length as the number of events. Will override
+        the ``event_name`` values in ``spec`` if ``spec`` is a dictionary
+        or pd.DataFrame.
+    offset : bool or str
         [**+p**\ *pen*][**+s**\ *size*].
-        Offsets beachballs to the longitude, latitude specified in the last two
-        columns of the input file or array, or by ``plot_longitude`` and
-        ``plot_latitude`` if provided. A small circle is plotted at the initial
-        location and a line connects the beachball to the circle. Use
-        **+s**\ *size* to set the diameter of the circle [Default is
-        no circle]. Use **+p**\ *pen* to set the line pen attributes [Default
-        is 0.25p].
+        Offset beachball(s) to longitude(s) and latitude(s) specified in the
+        the last two columns of the input file or array, or by
+        ``plot_longitude`` and ``plot_latitude`` if provided. A small circle
+        is plotted at the initial location and a line connects the beachball
+        to the circle. Use **+s**\ *size* to set the diameter of the circle
+        [Default is no circle]. Use **+p**\ *pen* to set the line pen
+        attributes [Default is ``"0.25p"``].
+    compressionfill : str
+        Set color or pattern for filling compressive quadrants
+        [Default is ``"black"``].
+    extensionfill : str
+        Set color or pattern for filling extensive quadrants
+        [Default is ``"white"``].
+    pen : str
+        Set pen attributes for outline of beachball
+        [Default is ``"0.25p,black,solid"``].
+    cmap : str
+        File name of a CPT file or a series of comma-separated colors (e.g.,
+        *color1,color2,color3*) to build a linear continuous CPT from those
+        colors automatically. The color of the compressive quadrants is
+        determined by the z-value (i.e., event depth or the third column for
+        an input file).
     no_clip : bool
-        Does NOT skip symbols that fall outside frame boundary specified by
-        ``region`` [Default is False, i.e. plot symbols inside map frame only].
+        Do **not** skip symbols that fall outside the frame boundaries
+        [Default is ``False``, i.e., plot symbols inside the frame
+        boundaries only].
     {projection}
     {region}
     {frame}
     {verbose}
     {panel}
     {perspective}
     {transparency}
```

### Comparing `pygmt-0.8.0/pygmt/src/nearneighbor.py` & `pygmt-0.9.0/pygmt/src/nearneighbor.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         Arrays of x and y coordinates and values z of the data points.
 
     {spacing}
 
     {region}
 
     search_radius : str
-        Sets the search radius that determines which data points are considered
+        Set the search radius that determines which data points are considered
         close to a node.
 
     outgrid : str
         Optional. The file name for the output netcdf file with extension .nc
         to store the grid in.
 
     empty : str
```

### Comparing `pygmt-0.8.0/pygmt/src/plot.py` & `pygmt-0.9.0/pygmt/src/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     G="fill",
     I="intensity",
     J="projection",
     L="close",
     N="no_clip",
     R="region",
     S="style",
-    U="timestamp",
     V="verbose",
     W="pen",
     Z="zvalue",
     a="aspatial",
     b="binary",
     c="panel",
     d="nodata",
@@ -165,29 +164,29 @@
     close : str
         [**+b**\|\ **d**\|\ **D**][**+xl**\|\ **r**\|\ *x0*]\
         [**+yl**\|\ **r**\|\ *y0*][**+p**\ *pen*].
         Force closed polygons. Full documentation is at
         :gmt-docs:`plot.html#l`.
     no_clip : bool or str
         [**c**\|\ **r**].
-        Do NOT clip symbols that fall outside map border [Default plots
-        points whose coordinates are strictly inside the map border only].
+        Do **not** clip symbols that fall outside the frame boundaries
+        [Default plots points whose coordinates are strictly inside the
+        frame boundaries only].
         The parameter does not apply to lines and polygons which are always
         clipped to the map region. For periodic (360-longitude) maps we
         must plot all symbols twice in case they are clipped by the
         repeating boundary. ``no_clip=True`` will turn off clipping and not
         plot repeating symbols. Use ``no_clip="r"`` to turn off clipping
         but retain the plotting of such repeating symbols, or use
         ``no_clip="c"`` to retain clipping but turn off plotting of
         repeating symbols.
     style : str
         Plot symbols (including vectors, pie slices, fronts, decorated or
         quoted lines).
     {pen}
-    {timestamp}
     {verbose}
     zvalue : str
         *value*\|\ *file*.
         Instead of specifying a symbol or polygon fill and outline color
         via ``fill`` and ``pen``, give both a *value* via ``zvalue`` and a
         color lookup table via ``cmap``.  Alternatively, give the name of a
         *file* with one z-value (read from the last column) for each
```

### Comparing `pygmt-0.8.0/pygmt/src/plot3d.py` & `pygmt-0.9.0/pygmt/src/plot3d.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     ----------
     data : str or {table-like}
         Either a data file name, a 2-D {table-classes}.
         Optionally, use parameter ``incols`` to specify which columns are x, y,
         z, fill, and size, respectively.
     x/y/z : float or 1-D arrays
         The x, y, and z coordinates, or arrays of x, y and z coordinates of
-        the data points
+        the data points.
     size : 1-D array
         The size of the data points in units specified in ``style``.
         Only valid if using ``x``/``y``/``z``.
     direction : list of two 1-D arrays
         If plotting vectors (using ``style="V"`` or ``style="v"``), then
         should be a list of two 1-D arrays with the vector directions. These
         can be angle and length, azimuth and length, or x and y components,
@@ -131,31 +131,31 @@
     close : str
         [**+b**\|\ **d**\|\ **D**][**+xl**\|\ **r**\|\ *x0*]\
         [**+yl**\|\ **r**\|\ *y0*][**+p**\ *pen*].
         Force closed polygons. Full documentation is at
         :gmt-docs:`plot3d.html#l`.
     no_clip : bool or str
         [**c**\|\ **r**].
-        Do NOT clip symbols that fall outside map border [Default plots
-        points whose coordinates are strictly inside the map border only].
+        Do **not** clip symbols that fall outside the frame boundaries
+        [Default plots points whose coordinates are strictly inside the
+        frame boundaries only].
         This parameter does not apply to lines and polygons which are always
-        clipped to the map region. For periodic (360-longitude) maps we
+        clipped to the map region. For periodic (360° longitude) maps we
         must plot all symbols twice in case they are clipped by the
         repeating boundary. ``no_clip=True`` will turn off clipping and not
         plot repeating symbols. Use ``no_clip="r"`` to turn off clipping
         but retain the plotting of such repeating symbols, or use
         ``no_clip="c"`` to retain clipping but turn off plotting of
         repeating symbols.
     no_sort : bool
         Turn off the automatic sorting of items based on their distance
         from the viewer. The default is to sort the items so that items in
         the foreground are plotted after items in the background.
     style : str
         Plot symbols. Full documentation is at :gmt-docs:`plot3d.html#s`.
-    {timestamp}
     {verbose}
     {pen}
     zvalue : str
         *value*\|\ *file*.
         Instead of specifying a symbol or polygon fill and outline color
         via ``fill`` and ``pen``, give both a *value* via **zvalue** and a
         color lookup table via ``cmap``.  Alternatively, give the name of a
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pygmt-0.8.0/pygmt/src/project.py` & `pygmt-0.9.0/pygmt/src/project.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/src/rose.py` & `pygmt-0.9.0/pygmt/src/rose.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     JX="diameter",
     L="labels",
     M="vector_params",
     Q="alpha",
     R="region",
     S="norm",
     T="orientation",
-    U="timestamp",
     V="verbose",
     W="pen",
     Z="scale",
     b="binary",
     d="nodata",
     e="find",
     h="header",
@@ -72,37 +71,37 @@
         azimuth, respectively. If a file with only azimuths is given, use
         ``incols`` to indicate the single column with azimuths; then all
         lengths are set to unity (see ``scale="u"`` to set actual
         lengths to unity as well).
 
     length/azimuth : float or 1-D arrays
         Length and azimuth values, or arrays of length and azimuth
-        values
+        values.
 
     orientation : bool
-        Specifies that the input data are orientation data (i.e., have a
+        Specify that the input data are orientation data (i.e., have a
         180 degree ambiguity) instead of true 0-360 degree directions
         [Default is 0-360 degrees]. We compensate by counting each record
         twice: First as azimuth and second as azimuth +180. Ignored if
         ``region`` is given as (-90, 90) or (0, 180).
 
     region : str or list
         *r0/r1/az0/az1* or [*r0*, *r1*, *az0*, *az1*].
         *Required if this is the first plot command*.
-        Specifies the ``region`` of interest in (*r*, *azimuth*) space.
+        Specify the ``region`` of interest in (*r*, *azimuth*) space.
         Here, *r0* is 0 and *r1* is the maximal length in units.
         For *az0* and *az1*, specify either (-90, 90) or (0, 180) for
         half circle plot or (0, 360) for full circle.
 
     diameter : str
-         Sets the diameter of the rose diagram. If not given,
+         Set the diameter of the rose diagram. If not given,
          then we default to a diameter of 7.5 cm.
 
     sector : float or str
-         Gives the sector width in degrees for sector and rose diagram.
+         Give the sector width in degrees for sector and rose diagram.
          Default ``0`` means windrose diagram. Append **+r** to draw rose
          diagram instead of sector diagram (e.g. ``"10+r"``).
 
     norm : bool
          Normalize input radii (or bin counts if ``sector`` is used)
          by the largest value so all radii (or bin counts) range from 0
          to 1.
@@ -116,16 +115,15 @@
     scale : float or str
          Multiply the data radii by scale. E.g., use ``scale=0.001`` to
          convert your data from m to km. To exclude the radii from
          consideration, set them all to unity with ``scale="u"``
          [Default is no scaling].
 
     fill : str
-         Selects shade, color or pattern for filling the sectors [Default
-         is no fill].
+         Set color or pattern for filling sectors [Default is no fill].
 
     cmap : str
         Give a CPT. The *r*-value for each sector is used to look-up the
         sector color. Cannot be used with a rose diagram.
 
     pen : str
         Set pen attributes for sector outline or rose plot, e.g.
@@ -173,27 +171,26 @@
         line]. See :gmt-docs:`rose.html#vector-attributes` for
         specifying additional attributes. If ``vectors`` is not
         given and the current plot mode is to draw a windrose diagram
         then using ``vector_params`` will add vector heads to all
         individual directions using the supplied attributes.
 
     alpha : float or str
-        Sets the confidence level used to determine if the mean
+        Set the confidence level used to determine if the mean
         resultant is significant (i.e., Lord Rayleigh test for
         uniformity) [Default is ``alpha=0.05``]. **Note**: The
         critical values are approximated [Berens, 2009] and requires
         at least 10 points; the critical resultants are accurate to
         at least 3 significant digits. For smaller data sets you
         should consult exact statistical tables.
 
         Berens, P., 2009, CircStat: A MATLAB Toolbox for Circular
         Statistics, *J. Stat. Software*, 31(10), 1-21,
         https://doi.org/10.18637/jss.v031.i10.
 
-    {timestamp}
     {verbose}
     {binary}
     {panel}
     {nodata}
     {find}
     {header}
     {incols}
```

### Comparing `pygmt-0.8.0/pygmt/src/select.py` & `pygmt-0.9.0/pygmt/src/select.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         it is not guaranteed that a point will remain inside [or outside] when
         a different resolution is selected.
     gridmask : str
         Pass all locations that are inside the valid data area of the grid
         *gridmask*. Nodes that are outside are either NaN or zero.
     reverse : str
         [**cflrsz**].
-        Reverses the sense of the test for each of the criteria specified:
+        Reverse the sense of the test for each of the criteria specified:
 
         - **c** select records NOT inside any point's circle of influence.
         - **f** select records NOT inside any of the polygons.
         - **g** will pass records inside the cells with z equal zero of the
           grid mask in ``gridmask``.
         - **l** select records NOT within the specified distance of any line.
         - **r** select records NOT inside the specified rectangular region.
```

### Comparing `pygmt-0.8.0/pygmt/src/solar.py` & `pygmt-0.9.0/pygmt/src/solar.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 @fmt_docstring
 @use_alias(
     B="frame",
     G="fill",
     J="projection",
     R="region",
-    U="timestamp",
     V="verbose",
     W="pen",
     c="panel",
     p="perspective",
     t="transparency",
 )
 @kwargs_to_strings(R="sequence", c="sequence_comma", p="sequence")
@@ -35,32 +34,31 @@
 
     {aliases}
 
     Parameters
     ----------
     terminator : str
         Set the type of terminator displayed. Valid arguments are
-        **day_night**, **civil**, **nautical**, and **astronomical**, which
-        can be set with either the full name or the first letter of the name
-        [Default is **day_night**].
+        ``"day_night"``, ``"civil"``, ``"nautical"``, and ``"astronomical"``,
+        which can be set with either the full name or the first letter of the
+        name [Default is ``"day_night"``].
 
         Refer to https://en.wikipedia.org/wiki/Twilight for the definitions of
         different types of twilight.
     terminator_datetime : str or datetime object
         Set the UTC date and time of the displayed terminator
         [Default is the current UTC date and time]. It can be
         passed as a string or Python datetime object.
     {region}
     {projection}
     {frame}
     fill : str
-        Color or pattern for filling of terminators.
+        Set color or pattern for filling terminators [Default is no fill].
     pen : str
         Set pen attributes for lines [Default is ``"0.25p,black,solid"``].
-    {timestamp}
     {verbose}
     {panel}
     {perspective}
     {transparency}
 
     Example
     -------
@@ -71,15 +69,15 @@
     >>> date = datetime.datetime(
     ...     year=1997, month=6, day=24, hour=8, minute=52, second=18
     ... )
     >>> # create a new plot with pygmt.Figure()
     >>> fig = pygmt.Figure()
     >>> # create a map of the Earth with the coast method
     >>> fig.coast(
-    ...     land="lightgreen", water="lightblue", projection="W10c", region="d"
+    ...     land="darkgreen", water="lightblue", projection="W10c", region="d"
     ... )
     >>> fig.solar(
     ...     # set the terminator to "day_night"
     ...     terminator="day_night",
     ...     # pass the datetime object
     ...     terminator_datetime=date,
     ...     # fill the night-section with navyblue at 75% transparency
```

### Comparing `pygmt-0.8.0/pygmt/src/sph2grd.py` & `pygmt-0.9.0/pygmt/src/sph2grd.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/src/sphdistance.py` & `pygmt-0.9.0/pygmt/src/sphdistance.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,16 +78,16 @@
         - **z** - assign all nodes inside the polygon the z-value of the center
           node for a natural nearest-neighbor grid.
 
         Optionally, append the resampling interval along Voronoi arcs in
         spherical degrees.
     unit : str
         Specify the unit used for distance calculations. Choose among **d**
-        (spherical degree), **e** (m), **f** (feet), **k** (km), **M**
-        (mile), **n** (nautical mile) or **u** survey foot.
+        (spherical degrees), **e** (meters), **f** (feet), **k** (kilometers),
+        **M** (miles), **n** (nautical miles), or **u** (survey feet).
     node_table : str
         Read the information pertaining to each Voronoi
         polygon (the unique node lon, lat and polygon area) from a separate
         file [Default acquires this information from the ASCII segment
         headers of the output file]. Required if binary input via `voronoi`
         is used.
     voronoi : str
```

### Comparing `pygmt-0.8.0/pygmt/src/sphinterpolate.py` & `pygmt-0.9.0/pygmt/src/sphinterpolate.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/src/subplot.py` & `pygmt-0.9.0/pygmt/src/subplot.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,20 +150,25 @@
     if nrows < 1 or ncols < 1:
         raise GMTInvalidInput("Please ensure that both 'nrows'>=1 and 'ncols'>=1.")
     if kwargs.get("Ff") and kwargs.get("Fs"):
         raise GMTInvalidInput(
             "Please provide either one of 'figsize' or 'subsize' only."
         )
 
-    with Session() as lib:
-        try:
+    # Need to use separate sessions for "subplot begin" and "subplot end".
+    # Otherwise, "subplot end" will use the last session, which may cause
+    # strange positioning issues for later plotting calls.
+    # See https://github.com/GenericMappingTools/pygmt/issues/2426.
+    try:
+        with Session() as lib:
             arg_str = " ".join(["begin", f"{nrows}x{ncols}", build_arg_string(kwargs)])
             lib.call_module(module="subplot", args=arg_str)
             yield
-        finally:
+    finally:
+        with Session() as lib:
             v_arg = build_arg_string({"V": kwargs.get("V")})
             lib.call_module(module="subplot", args=f"end {v_arg}")
 
 
 @fmt_docstring
 @contextlib.contextmanager
 @use_alias(A="fixedlabel", C="clearance", V="verbose")
```

### Comparing `pygmt-0.8.0/pygmt/src/ternary.py` & `pygmt-0.9.0/pygmt/src/ternary.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 """
 ternary - Plot data on ternary diagrams.
 """
 import pandas as pd
 from packaging.version import Version
+from pygmt import __gmt_version__
 from pygmt.clib import Session
 from pygmt.helpers import build_arg_string, fmt_docstring, kwargs_to_strings, use_alias
 
 
 @fmt_docstring
 @use_alias(
     B="frame",
     C="cmap",
     G="fill",
     JX="width",
     R="region",
     S="style",
-    U="timestamp",
     V="verbose",
     W="pen",
     c="panel",
     p="perspective",
     t="transparency",
 )
 @kwargs_to_strings(R="sequence", c="sequence_comma", p="sequence")
 def ternary(self, data, alabel=None, blabel=None, clabel=None, **kwargs):
     r"""
+    Plot ternary diagrams.
+
     Reads (*a*,\ *b*,\ *c*\ [,\ *z*]) records from *data* and plots symbols at
     those locations on a ternary diagram. If a symbol is selected and no symbol
     size given, then we will interpret the fourth column of the input data as
     symbol size. Symbols whose *size* is <= 0 are skipped. If no symbols are
     specified then the symbol code (see ``style`` below) must be present as
     last column in the input.  If ``style`` is not specified then we instead
     plot lines or polygons.
@@ -62,34 +64,32 @@
         Set the label for the *b* vertex where the component is 100%.
     clabel : str
         Set the label for the *c* vertex where the component is 100%.
     style : str
         *symbol*\[\ *size*].
         Plot individual symbols in a ternary diagram.
     {pen}
-    {timestamp}
     {verbose}
     {panel}
     {perspective}
     {transparency}
     """
     kwargs = self._preprocess(**kwargs)  # pylint: disable=protected-access
 
     if alabel or blabel or clabel:
         alabel = str(alabel) if alabel is not None else "-"
         blabel = str(blabel) if blabel is not None else "-"
         clabel = str(clabel) if clabel is not None else "-"
         kwargs["L"] = "/".join([alabel, blabel, clabel])
 
+    # Patch for GMT < 6.5.0.
+    # See https://github.com/GenericMappingTools/pygmt/pull/2138
+    if Version(__gmt_version__) < Version("6.5.0") and isinstance(data, pd.DataFrame):
+        data = data.to_numpy()
+
     with Session() as lib:
-        # Patch for GMT < 6.5.0.
-        # See https://github.com/GenericMappingTools/pygmt/pull/2138
-        if Version(lib.info["version"]) < Version("6.5.0") and isinstance(
-            data, pd.DataFrame
-        ):
-            data = data.to_numpy()
         file_context = lib.virtualfile_from_data(check_kind="vector", data=data)
         with file_context as infile:
             lib.call_module(
                 module="ternary",
                 args=build_arg_string(kwargs, infile=infile),
             )
```

### Comparing `pygmt-0.8.0/pygmt/src/text.py` & `pygmt-0.9.0/pygmt/src/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     R="region",
     J="projection",
     B="frame",
     C="clearance",
     D="offset",
     G="fill",
     N="no_clip",
-    U="timestamp",
     V="verbose",
     W="pen",
     a="aspatial",
     c="panel",
     e="find",
     f="coltypes",
     h="header",
@@ -77,15 +76,15 @@
     textfiles : str or list
         A text data file name, or a list of file names containing 1 or more
         records with (x, y[, angle, font, justify], text).
     x/y : float or 1-D arrays
         The x and y coordinates, or an array of x and y coordinates to plot
         the text.
     position : str
-        Sets reference point on the map for the text by using x, y
+        Set reference point on the map for the text by using x, y
         coordinates extracted from ``region`` instead of providing them
         through ``x``/``y``. Specify with a two-letter (order independent)
         code, chosen from:
 
         * Horizontal: **L**\ (eft), **C**\ (entre), **R**\ (ight)
         * Vertical: **T**\ (op), **M**\ (iddle), **B**\ (ottom)
 
@@ -116,44 +115,43 @@
         this as a column.
     {projection}
     {region}
         *Required if this is the first plot command.*
     clearance : str
         [*dx/dy*][**+to**\|\ **O**\|\ **c**\|\ **C**].
         Adjust the clearance between the text and the surrounding box
-        [Default is 15% of the font size]. Only used if ``pen`` or ``fill`` are
-        specified. Append the unit you want (*c* for cm, *i* for inch, or *p*
-        for point; if not given we consult :gmt-term:`PROJ_LENGTH_UNIT`)
-        or *%* for a percentage of the font size. Optionally, use modifier
-        **+t** to set the shape of the text box when using ``fill`` and/or
-        ``pen``. Append lower case **o** to get a straight rectangle
-        [Default is **o**]. Append upper case **O** to get a rounded
-        rectangle. In paragraph mode (*paragraph*) you can also append lower
-        case **c** to get a concave rectangle or append upper case **C**
-        to get a convex rectangle.
+        [Default is 15% of the font size]. Only used if ``pen`` or ``fill``
+        are specified. Append the unit you want (*c* for centimeters,
+        *i* for inches, or *p* for points; if not given we consult
+        :gmt-term:`PROJ_LENGTH_UNIT`) or *%* for a percentage of the font
+        size. Optionally, use modifier **+t** to set the shape of the text
+        box when using ``fill`` and/or ``pen``. Append lower case **o**
+        to get a straight rectangle [Default is **o**]. Append upper case
+        **O** to get a rounded rectangle. In paragraph mode (*paragraph*)
+        you can also append lower case **c** to get a concave rectangle or
+        append upper case **C** to get a convex rectangle.
     fill : str
-        Sets the shade or color used for filling the text box [Default is
-        no fill].
+        Set color for filling text boxes [Default is no fill].
     offset : str
         [**j**\|\ **J**]\ *dx*\[/*dy*][**+v**\[*pen*]].
-        Offsets the text from the projected (x, y) point by *dx*/\ *dy*
+        Offset the text from the projected (x, y) point by *dx*/\ *dy*
         [Default is ``"0/0"``].
         If *dy* is not specified then it is set equal to *dx*. Use **j** to
         offset the text away from the point instead (i.e., the text
         justification will determine the direction of the shift). Using
         **J** will shorten diagonal offsets at corners by sqrt(2).
         Optionally, append **+v** which will draw a line from the original
         point to the shifted point; append a pen to change the attributes
         for this line.
     pen : str
-        Sets the pen used to draw a rectangle around the text string
+        Set the pen used to draw a rectangle around the text string
         (see ``clearance``) [Default is ``"0.25p,black,solid"``].
     no_clip : bool
-        Do NOT clip text at map boundaries [Default is with clip].
-    {timestamp}
+        Do **not** clip text at the frame boundaries [Default is
+        ``False``].
     {verbose}
     {aspatial}
     {panel}
     {find}
     {coltypes}
     {header}
     use_word : int
```

### Comparing `pygmt-0.8.0/pygmt/src/triangulate.py` & `pygmt-0.9.0/pygmt/src/triangulate.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             better off projecting all data to a local coordinate system before
             using ``triangulate`` (this is true of all gridding routines) or
             instead select :gmt-docs:`sphtriangulate <sphtriangulate.html>`.
         outfile : str or bool or None
             The name of the output ASCII file to store the results of the
             histogram equalization in.
         output_type: str
-            Determines the output type. Use "file", "xarray", "pandas", or
+            Determine the output type. Use "file", "xarray", "pandas", or
             "numpy".
         {verbose}
         {binary}
         {nodata}
         {find}
         {coltypes}
         {header}
```

### Comparing `pygmt-0.8.0/pygmt/src/velo.py` & `pygmt-0.9.0/pygmt/src/velo.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     H="scale",
     I="shading",
     J="projection",
     L="line",
     N="no_clip",
     R="region",
     S="spec",
-    U="timestamp",
     V="verbose",
     W="pen",
     Z="zvalue",
     c="panel",
     d="nodata",
     e="find",
     h="header",
@@ -68,15 +67,15 @@
     data : str or {table-like}
         Pass in either a file name to an ASCII data table, a 2-D
         {table-classes}.
         Note that text columns are only supported with file or
         :class:`pandas.DataFrame` inputs.
 
     spec: str
-        Selects the meaning of the columns in the data file and the figure to
+        Select the meaning of the columns in the data file and the figure to
         be plotted. In all cases, the scales are in data units per length unit
         and sizes are in length units (default length unit is controlled by
         :gmt-term:`PROJ_LENGTH_UNIT` unless **c**, **i**, or **p** is
         appended).
 
         - **e**\ [*velscale*/]\ *confidence*\ [**+f**\ *font*]
 
@@ -168,30 +167,30 @@
         Modify vector parameters. For vector heads, append vector head *size*
         [Default is 9p]. See
         :gmt-docs:`supplements/geodesy/velo.html#vector-attributes` for
         specifying additional attributes.
     {frame}
     {cmap}
     rescale : str
-        can be used to rescale the uncertainties of velocities (``spec="e"``
+        Can be used to rescale the uncertainties of velocities (``spec="e"``
         and ``spec="r"``) and rotations (``spec="w"``). Can be combined with
         the ``confidence`` variable.
     uncertaintyfill : str
-        Sets the color or shade used for filling uncertainty wedges
-        (``spec="w"``) or velocity error ellipses (``spec="e"`` or
-        ``spec="r"``). If ``uncertaintyfill`` is not specified, the
-        uncertainty regions will be transparent. **Note**: Using ``cmap`` and
-        ``zvalue="+e"`` will update the uncertainty fill color based on the
-        selected measure in ``zvalue`` [magnitude error]. More details at
+        Set color or pattern for filling uncertainty wedges (``spec="w"``)
+        or velocity error ellipses (``spec="e"`` or ``spec="r"``).
+        If ``uncertaintyfill`` is not specified, the uncertainty regions
+        will be transparent. **Note**: Using ``cmap`` and ``zvalue="+e"``
+        will update the uncertainty fill color based on the selected measure
+        in ``zvalue`` [Default is magnitude error]. More details at
         :gmt-docs:`cookbook/features.html#gfill-attrib`.
     fill : str
-        Select color or pattern for filling of symbols [Default is no fill].
+        Set color or pattern for filling symbols [Default is no fill].
         **Note**: Using ``cmap`` (and optionally ``zvalue``) will update the
         symbol fill color based on the selected measure in ``zvalue``
-        [magnitude]. More details at
+        [Default is magnitude]. More details at
         :gmt-docs:`cookbook/features.html#gfill-attrib`.
     scale : float or bool
         [*scale*].
         Scale symbol sizes and pen widths on a per-record basis using the
         *scale* read from the data set, given as the first column after the
         (optional) *z* and *size* columns [Default is no scaling]. The symbol
         size is either provided by ``spec`` or via the input *size* column.
@@ -209,18 +208,18 @@
         Draw lines. Ellipses and rotational wedges will have their outlines
         drawn using the current pen (see ``pen``).  Alternatively, append a
         separate pen to use for the error outlines. If the modifier **+cl** is
         appended then the color of the pen is updated from the CPT (see
         ``cmap``). If instead modifier **+cf** is appended then the color from
         the cpt file is applied to error fill only [Default]. Use just **+c**
         to set both pen and fill color.
-    no_clip: bool or str
-        Do NOT skip symbols that fall outside the frame boundary specified
-        by ``region`` [Default plots symbols inside frame only].
-    {timestamp}
+    no_clip: bool
+        Do **not** skip symbols that fall outside the frame boundaries
+        [Default is ``False``, i.e., plot symbols inside the frame
+        boundaries only].
     {verbose}
     pen : str
         [*pen*][**+c**\ [**f**\|\ **l**]].
         Set pen attributes for velocity arrows, ellipse circumference and fault
         plane edges [Default is ``"0.25p,black,solid"``].
         If the modifier **+cl** is appended then the color of the pen is
         updated from the CPT (see ``cmap``). If instead modifier **+cf** is
```

### Comparing `pygmt-0.8.0/pygmt/src/which.py` & `pygmt-0.9.0/pygmt/src/which.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/src/wiggle.py` & `pygmt-0.9.0/pygmt/src/wiggle.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 @use_alias(
     B="frame",
     D="position",
     G="color",
     J="projection",
     R="region",
     T="track",
-    U="timestamp",
     V="verbose",
     W="pen",
     Z="scale",
     b="binary",
     c="panel",
     d="nodata",
     e="find",
@@ -37,15 +36,15 @@
     self,
     data=None,
     x=None,
     y=None,
     z=None,
     fillpositive=None,
     fillnegative=None,
-    **kwargs
+    **kwargs,
 ):
     r"""
     Plot z=f(x,y) anomalies along tracks.
 
     Takes a matrix, (x, y, z) triplets, or a file name as input and plots z
     as a function of distance along track.
 
@@ -63,34 +62,33 @@
         Pass in either a file name to an ASCII data table, a 2-D
         {table-classes}.
         Use parameter ``incols`` to choose which columns are x, y, z,
         respectively.
     {projection}
     {region}
     scale : str or float
-        Gives anomaly scale in data-units/distance-unit. Append **c**, **i**,
-        or **p** to indicate the distance unit (cm, inch, or point); if no unit
-        is given we use the default unit that is controlled by
-        :gmt-term:`PROJ_LENGTH_UNIT`.
+        Give anomaly scale in data-units/distance-unit. Append **c**, **i**,
+        or **p** to indicate the distance unit (centimeters, inches, or
+        points); if no unit is given we use the default unit that is
+        controlled by :gmt-term:`PROJ_LENGTH_UNIT`.
     {frame}
     position : str
         [**g**\|\ **j**\|\ **J**\|\ **n**\|\ **x**]\ *refpoint*\
         **+w**\ *length*\ [**+j**\ *justify*]\ [**+al**\|\ **r**]\
         [**+o**\ *dx*\ [/*dy*]][**+l**\ [*label*]].
-        Defines the reference point on the map for the vertical scale bar.
+        Define the reference point on the map for the vertical scale bar.
     fillpositive : str
-        Set fill shade, color, or pattern for positive wiggles [Default is no
-        fill].
+        Set color or pattern for filling positive wiggles
+        [Default is no fill].
     fillnegative : str
-        Set fill shade, color, or pattern for negative wiggles [Default is no
-        fill].
+        Set color or pattern for filling negative wiggles
+        [Default is no fill].
     track : str
         Draw track [Default is no track]. Append pen attributes to use
         [Default is ``"0.25p,black,solid"``].
-    {timestamp}
     {verbose}
     pen : str
         Specify outline pen attributes [Default is no outline].
     {binary}
     {panel}
     {nodata}
     {find}
```

### Comparing `pygmt-0.8.0/pygmt/src/x2sys_cross.py` & `pygmt-0.9.0/pygmt/src/x2sys_cross.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/src/x2sys_init.py` & `pygmt-0.9.0/pygmt/src/x2sys_init.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,45 +56,45 @@
         - **gmt** (for old mgg supplement binary files)
         - **xy** (for plain ASCII x, y tables)
         - **xyz** (same, with one z-column)
         - **geo** (for plain ASCII longitude, latitude files)
         - **geoz** (same, with one z-column).
 
     suffix : str
-        Specifies the file extension (suffix) for these data files. If not
+        Specify the file extension (suffix) for these data files. If not
         given we use the format definition file prefix as the suffix (see
         ``fmtfile``).
 
     discontinuity : str
         **d**\|\ **g**.
-        Selects geographical coordinates. Append **d** for discontinuity at the
-        Dateline (makes longitude go from -180 to +180) or **g** for
-        discontinuity at Greenwich (makes longitude go from 0 to 360
+        Select geographical coordinates. Append **d** for discontinuity at the
+        Dateline (makes longitude go from -180° to +180°) or **g** for
+        discontinuity at Greenwich (makes longitude go from 0° to 360°
         [Default]). If not given we assume the data are Cartesian.
 
     spacing : str or list
          *dx*\[/*dy*].
          *dx* and optionally *dy* is the grid spacing. Append **m** to
          indicate minutes or **s** to indicate seconds for geographic data.
          These spacings refer to the binning used in the track bin-index data
          base.
 
     units : str or list
         **d**\|\ **s**\ *unit*.
-        Sets the units used for distance and speed when requested by other
+        Set the units used for distance and speed when requested by other
         programs. Append **d** for distance or **s** for speed, then give the
         desired *unit* as:
 
         - **c** - Cartesian userdist or userdist/usertime
         - **e** - meters or m/s
-        - **f** - feet or feet/s
-        - **k** - km or km/hr
-        - **m** - miles or miles/hr
+        - **f** - feet or ft/s
+        - **k** - kilometers or km/hr
+        - **m** - miles or mi/hr
         - **n** - nautical miles or knots
-        - **u** - survey feet or survey feet/s
+        - **u** - survey feet or sft/s
 
         [Default is ``units=["dk", "se"]`` (km and m/s) if ``discontinuity`` is
         set, and ``units=["dc", "sc"]`` otherwise (e.g., for Cartesian units)].
 
     {region}
     {verbose}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pygmt-0.8.0/pygmt/src/xyz2grd.py` & `pygmt-0.9.0/pygmt/src/xyz2grd.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_accessor.py` & `pygmt-0.9.0/pygmt/tests/test_accessor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """
 Test the behaviour of the GMTDataArrayAccessor class.
 """
 import os
 import sys
+from pathlib import Path
 
 import pytest
 import xarray as xr
 from packaging.version import Version
-from pygmt import clib, which
+from pygmt import __gmt_version__, which
+from pygmt.datasets import load_earth_relief
 from pygmt.exceptions import GMTInvalidInput
 
-with clib.Session() as _lib:
-    gmt_version = Version(_lib.info["version"])
-
 
 def test_accessor_gridline_cartesian():
     """
     Check that a grid returns a registration value of 0 when Gridline
     registered, and a gtype value of 1 when using Geographic coordinates.
     """
     fname = which(fname="@test.dat.nc", download="a")
@@ -72,15 +71,15 @@
         grid.gmt.registration = "2"
 
     with pytest.raises(GMTInvalidInput):
         grid.gmt.gtype = 2
 
 
 @pytest.mark.skipif(
-    gmt_version < Version("6.4.0"),
+    Version(__gmt_version__) < Version("6.4.0"),
     reason="Upstream bug fixed in https://github.com/GenericMappingTools/gmt/pull/6615",
 )
 @pytest.mark.xfail(
     condition=sys.platform == "win32",
     reason="PermissionError on Windows when deleting eraint_uvz.nc file; "
     "see https://github.com/GenericMappingTools/pygmt/pull/2073",
 )
@@ -100,7 +99,36 @@
         with xr.open_dataset(fname) as dataset:
             grid = dataset.sel(level=500, month=1, drop=True).z
 
         assert grid.gmt.registration == 0  # gridline registration
         assert grid.gmt.gtype == 1  # geographic coordinate type
     finally:
         os.remove(fname)
+
+
+def test_accessor_grid_source_file_not_exist():
+    """
+    Check that the accessor fallbacks to the default registration and gtype
+    when the grid source file (i.e., grid.encoding["source"]) doesn't exist.
+    """
+    # Load the 05m earth relief grid, which is stored as tiles
+    grid = load_earth_relief(
+        resolution="05m", region=[0, 5, -5, 5], registration="pixel"
+    )
+    # Registration and gtype are correct
+    assert grid.gmt.registration == 1
+    assert grid.gmt.gtype == 1
+    # The source grid file is defined but doesn't exist
+    assert grid.encoding["source"].endswith(".nc")
+    assert not Path(grid.encoding["source"]).exists()
+
+    # For a sliced grid, fallback to default registration and gtype,
+    # because the source grid file doesn't exist.
+    sliced_grid = grid[1:3, 1:3]
+    assert sliced_grid.gmt.registration == 0
+    assert sliced_grid.gmt.gtype == 0
+
+    # Still possible to manually set registration and gtype
+    sliced_grid.gmt.registration = 1
+    sliced_grid.gmt.gtype = 1
+    assert sliced_grid.gmt.registration == 1
+    assert sliced_grid.gmt.gtype == 1
```

### Comparing `pygmt-0.8.0/pygmt/tests/test_basemap.py` & `pygmt-0.9.0/pygmt/tests/test_basemap.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,14 @@
 Tests Figure.basemap.
 """
 import pytest
 from pygmt import Figure
 
 
 @pytest.mark.mpl_image_compare
-def test_basemap_required_args():
-    """
-    Automatically set `frame=True` when required arguments are not given.
-    """
-    fig = Figure()
-    fig.basemap(region=[10, 70, -3, 8], projection="X8c/6c")
-    return fig
-
-
-@pytest.mark.mpl_image_compare
 def test_basemap():
     """
     Create a simple basemap plot.
     """
     fig = Figure()
     fig.basemap(region=[10, 70, -3, 8], projection="X8c/6c", frame="afg")
     return fig
@@ -132,7 +122,22 @@
     fig.basemap(
         region=[127.5, 128.5, 26, 27],
         projection="H15c",
         frame=True,
         map_scale="jMC+c26.5+w10k+f+l",
     )
     return fig
+
+
+@pytest.mark.mpl_image_compare
+def test_basemap_subplot():
+    """
+    Test in subplot mode for the case that the frame parameter of basemap is
+    not specified.
+    """
+    fig = Figure()
+    with fig.subplot(nrows=1, ncols=2, figsize=("10c", "5c")):
+        with fig.set_panel(panel=0):
+            fig.basemap(region=[0, 10, 0, 10], projection="X?")
+        with fig.set_panel(panel=1):
+            fig.basemap(region=[0, 10, 0, 10], projection="X?")
+    return fig
```

### Comparing `pygmt-0.8.0/pygmt/tests/test_binstats.py` & `pygmt-0.9.0/pygmt/tests/test_binstats.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_blockm.py` & `pygmt-0.9.0/pygmt/tests/test_blockm.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_blockmedian.py` & `pygmt-0.9.0/pygmt/tests/test_blockmedian.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_clib.py` & `pygmt-0.9.0/pygmt/tests/test_clib.py`

 * *Files 1% similar despite different names*

```diff
@@ -635,19 +635,19 @@
 def test_virtualfile_from_vectors_pandas(dtypes):
     """
     Pass vectors to a dataset using pandas Series.
     """
     size = 13
     for dtype in dtypes:
         data = pd.DataFrame(
-            data=dict(
-                x=np.arange(size, dtype=dtype),
-                y=np.arange(size, size * 2, 1, dtype=dtype),
-                z=np.arange(size * 2, size * 3, 1, dtype=dtype),
-            )
+            data={
+                "x": np.arange(size, dtype=dtype),
+                "y": np.arange(size, size * 2, 1, dtype=dtype),
+                "z": np.arange(size * 2, size * 3, 1, dtype=dtype),
+            }
         )
         with clib.Session() as lib:
             with lib.virtualfile_from_vectors(data.x, data.y, data.z) as vfile:
                 with GMTTempFile() as outfile:
                     lib.call_module("info", f"{vfile} ->{outfile.name}")
                     output = outfile.read(keep_tabs=True)
             bounds = "\t".join(
```

### Comparing `pygmt-0.8.0/pygmt/tests/test_clib_loading.py` & `pygmt-0.9.0/pygmt/tests/test_clib_loading.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_clib_put_matrix.py` & `pygmt-0.9.0/pygmt/tests/test_clib_put_matrix.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_clib_put_strings.py` & `pygmt-0.9.0/pygmt/tests/test_clib_put_strings.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_clib_put_vector.py` & `pygmt-0.9.0/pygmt/tests/test_clib_put_vector.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_coast.py` & `pygmt-0.9.0/pygmt/tests/test_coast.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_colorbar.py` & `pygmt-0.9.0/pygmt/tests/test_colorbar.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_config.py` & `pygmt-0.9.0/pygmt/tests/test_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,16 +68,21 @@
 def test_config_format_date_map():
     """
     Test that setting FORMAT_DATE_MAP config changes how the output date string
     is plotted.
 
     Note the space in 'o dd', this acts as a regression test for
     https://github.com/GenericMappingTools/pygmt/issues/247.
+
+    Setting FORMAT_DATE_MAP="yyyy mm dd" as a regression test for
+    https://github.com/GenericMappingTools/pygmt/issues/2298.
     """
     fig = Figure()
+    # Set FORMAT_DATE_MAP to "yyyy mm dd" which contains whitespaces.
+    config(FORMAT_DATE_MAP="yyyy mm dd")
     with config(FORMAT_DATE_MAP="o dd"):
         fig.basemap(
             region=["1969-7-21T", "1969-7-23T", 0, 1],
             projection="X2.5c/0.1c",
             frame=["sxa1D", "S"],
         )
     return fig
```

### Comparing `pygmt-0.8.0/pygmt/tests/test_contour.py` & `pygmt-0.9.0/pygmt/tests/test_contour.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 @pytest.fixture(scope="module", name="data")
 def fixture_data():
     """
     Load the point data from the test file.
     """
-    return pd.read_table(POINTS_DATA, header=None, sep=r"\s+")
+    return pd.read_table(POINTS_DATA, header=None, delim_whitespace=True)
 
 
 @pytest.fixture(scope="module", name="region")
 def fixture_region():
     """
     The data region.
     """
```

### Comparing `pygmt-0.8.0/pygmt/tests/test_datasets_earth_age.py` & `pygmt-0.9.0/pygmt/tests/test_datasets_earth_age.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_datasets_earth_free_air_anomaly.py` & `pygmt-0.9.0/pygmt/tests/test_datasets_earth_free_air_anomaly.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_datasets_earth_geoid.py` & `pygmt-0.9.0/pygmt/tests/test_datasets_earth_geoid.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_datasets_earth_magnetic_anomaly.py` & `pygmt-0.9.0/pygmt/tests/test_datasets_earth_magnetic_anomaly.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,14 +76,30 @@
             resolution="02m",
             region=[0, 1, 3, 5],
             registration="gridline",
             data_source="emag2_4km",
         )
 
 
+def test_earth_mag_02m_default_registration():
+    """
+    Test that the grid returned by default for the 2 arc-minute resolution has
+    a "pixel" registration.
+    """
+    data = load_earth_magnetic_anomaly(resolution="02m", region=[-10, -9, 3, 5])
+    assert data.shape == (60, 30)
+    assert data.gmt.registration == 1
+    npt.assert_allclose(data.coords["lat"].data.min(), 3.016666667)
+    npt.assert_allclose(data.coords["lat"].data.max(), 4.983333333)
+    npt.assert_allclose(data.coords["lon"].data.min(), -9.98333333)
+    npt.assert_allclose(data.coords["lon"].data.max(), -9.01666667)
+    npt.assert_allclose(data.min(), -231)
+    npt.assert_allclose(data.max(), 131.79999)
+
+
 def test_earth_mag4km_01d():
     """
     Test some properties of the magnetic anomaly 4km 01d data.
     """
     data = load_earth_magnetic_anomaly(resolution="01d", data_source="emag2_4km")
     assert data.name == "magnetic_anomaly"
     assert data.attrs["long_name"] == "Earth magnetic anomaly"
@@ -110,42 +126,32 @@
     assert data.shape == (11, 21)
     npt.assert_allclose(data.lat, np.arange(-5, 6, 1))
     npt.assert_allclose(data.lon, np.arange(-10, 11, 1))
     npt.assert_allclose(data.min(), -153.19995)
     npt.assert_allclose(data.max(), 113.59985)
 
 
-def test_earth_mag_02m_default_registration():
+def test_earth_mag4km_02m_default_registration():
     """
     Test that the grid returned by default for the 2 arc-minute resolution has
     a "pixel" registration.
     """
-    data = load_earth_magnetic_anomaly(resolution="02m", region=[-10, -9, 3, 5])
-    assert data.shape == (60, 30)
-    assert data.gmt.registration == 1
-    npt.assert_allclose(data.coords["lat"].data.min(), 3.016666667)
-    npt.assert_allclose(data.coords["lat"].data.max(), 4.983333333)
-    npt.assert_allclose(data.coords["lon"].data.min(), -9.98333333)
-    npt.assert_allclose(data.coords["lon"].data.max(), -9.01666667)
-    npt.assert_allclose(data.min(), -231)
-    npt.assert_allclose(data.max(), 131.79999)
-
     data = load_earth_magnetic_anomaly(
-        resolution="05m",
+        resolution="02m",
         region=[-115, -112, 4, 6],
-        registration="gridline",
         data_source="emag2_4km",
     )
-    assert data.shape == (25, 37)
-    assert data.lat.min() == 4
-    assert data.lat.max() == 6
-    assert data.lon.min() == -115
-    assert data.lon.max() == -112
-    npt.assert_allclose(data.min(), -128.40015)
-    npt.assert_allclose(data.max(), 76.80005)
+    assert data.shape == (60, 90)
+    assert data.gmt.registration == 1
+    npt.assert_allclose(data.coords["lat"].data.min(), 4.01666667)
+    npt.assert_allclose(data.coords["lat"].data.max(), 5.98333333)
+    npt.assert_allclose(data.coords["lon"].data.min(), -114.98333333)
+    npt.assert_allclose(data.coords["lon"].data.max(), -112.01666667)
+    npt.assert_allclose(data.min(), -132.80005)
+    npt.assert_allclose(data.max(), 79.59985)
 
 
 def test_earth_mag_01d_wdmam():
     """
     Test some properties of the WDMAM 01d data.
     """
     data = load_earth_magnetic_anomaly(
@@ -192,21 +198,21 @@
     assert data.lat.max() == -58
     assert data.lon.min() == 10
     assert data.lon.max() == 13
     npt.assert_allclose(data.min(), -639.7001)
     npt.assert_allclose(data.max(), 629.6)
 
 
-def test_earth_mag_05m_wdmam_without_region():
+def test_earth_mag_03m_wdmam_without_region():
     """
     Test loading a high-resolution WDMAM grid without passing 'region'.
     """
     with pytest.raises(GMTInvalidInput):
         load_earth_magnetic_anomaly(
-            resolution="05m", registration="gridline", data_source="wdmam"
+            resolution="03m", registration="gridline", data_source="wdmam"
         )
 
 
 def test_earth_mag_wdmam_incorrect_resolution_registration():
     """
     Test that an error is raised when trying to load a WDMAM grid registration
     with an unavailable resolution.
```

### Comparing `pygmt-0.8.0/pygmt/tests/test_datasets_earth_relief.py` & `pygmt-0.9.0/pygmt/tests/test_datasets_earth_relief.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_datasets_earth_vertical_gravity_gradient.py` & `pygmt-0.9.0/pygmt/tests/test_datasets_earth_vertical_gravity_gradient.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_datasets_samples.py` & `pygmt-0.9.0/pygmt/tests/test_datasets_samples.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,33 @@
 """
 Test basic functionality for loading sample datasets.
 """
 import numpy.testing as npt
 import pandas as pd
 import pytest
-from pygmt.datasets import (
-    load_fractures_compilation,
-    load_hotspots,
-    load_japan_quakes,
-    load_mars_shape,
-    load_ocean_ridge_points,
-    load_sample_bathymetry,
-    load_sample_data,
-    load_usgs_quakes,
-)
+from pygmt.datasets import list_sample_data, load_sample_data
 from pygmt.exceptions import GMTInvalidInput
 
 
 def test_load_sample_invalid():
     """
     Check that the function raises error for unsupported filenames.
     """
     with pytest.raises(GMTInvalidInput):
         load_sample_data(name="bad.filename")
 
 
-def test_japan_quakes():
+def test_list_sample_data():
     """
-    Check that the dataset loads without errors.
+    Check that the list_sample_data function returns a dictionary.
     """
-    with pytest.warns(expected_warning=FutureWarning) as record:
-        data = load_japan_quakes()
-        assert len(record) == 1
-    assert data.shape == (115, 7)
-    assert data["year"].min() == 1987
-    assert data["year"].max() == 1988
-    assert data["month"].min() == 1
-    assert data["month"].max() == 12
-    assert data["day"].min() == 1
-    assert data["day"].max() == 31
+    assert isinstance(list_sample_data(), dict)
 
 
-def test_load_sample_data():
+def test_japan_quakes():
     """
     Check that the dataset loads without errors.
     """
     data = load_sample_data(name="japan_quakes")
     assert data.shape == (115, 7)
     assert data["year"].min() == 1987
     assert data["year"].max() == 1988
@@ -55,95 +37,137 @@
     assert data["day"].max() == 31
 
 
 def test_ocean_ridge_points():
     """
     Check that the @ridge.txt dataset loads without errors.
     """
-    with pytest.warns(expected_warning=FutureWarning) as record:
-        data = load_ocean_ridge_points()
-        assert len(record) == 1
+    data = load_sample_data(name="ocean_ridge_points")
     assert data.shape == (4146, 2)
     assert data["longitude"].min() == -179.9401
     assert data["longitude"].max() == 179.935
     assert data["latitude"].min() == -65.6182
     assert data["latitude"].max() == 86.8
 
 
 def test_sample_bathymetry():
     """
     Check that the @tut_ship.xyz dataset loads without errors.
     """
-    with pytest.warns(expected_warning=FutureWarning) as record:
-        data = load_sample_bathymetry()
-        assert len(record) == 1
+    data = load_sample_data(name="bathymetry")
     assert data.shape == (82970, 3)
     assert data["longitude"].min() == 245.0
     assert data["longitude"].max() == 254.705
     assert data["latitude"].min() == 20.0
     assert data["latitude"].max() == 29.99131
     assert data["bathymetry"].min() == -7708.0
     assert data["bathymetry"].max() == -9.0
 
 
 def test_usgs_quakes():
     """
-    Check that the dataset loads without errors.
+    Check that the @usgs_quakes_22.txt dataset loads without errors.
     """
-    with pytest.warns(expected_warning=FutureWarning) as record:
-        data = load_usgs_quakes()
-        assert len(record) == 1
+    data = load_sample_data(name="usgs_quakes")
     assert data.shape == (1197, 22)
+    assert list(data.columns) == [
+        "time",
+        "latitude",
+        "longitude",
+        "depth",
+        "mag",
+        "magType",
+        "nst",
+        "gap",
+        "dmin",
+        "rms",
+        "net",
+        "id",
+        "updated",
+        "place",
+        "type",
+        "horizontalError",
+        "depthError",
+        "magError",
+        "magNst",
+        "status",
+        "locationSource",
+        "magSource",
+    ]
+    npt.assert_allclose(data["latitude"].min(), -60.6819)
+    npt.assert_allclose(data["latitude"].max(), 72.6309)
+    npt.assert_allclose(data["longitude"].min(), -179.9953)
+    npt.assert_allclose(data["longitude"].max(), 179.9129)
+    npt.assert_allclose(data["depth"].min(), -0.21)
+    npt.assert_allclose(data["depth"].max(), 640.49)
+    npt.assert_allclose(data["mag"].min(), 3)
+    npt.assert_allclose(data["mag"].max(), 8.1)
+    npt.assert_allclose(data["nst"].min(), 3)
+    npt.assert_allclose(data["nst"].max(), 167)
+    npt.assert_allclose(data["gap"].min(), 10.0)
+    npt.assert_allclose(data["gap"].max(), 353.0)
+    npt.assert_allclose(data["dmin"].min(), 0.006421)
+    npt.assert_allclose(data["dmin"].max(), 39.455)
+    npt.assert_allclose(data["rms"].min(), 0.02)
+    npt.assert_allclose(data["rms"].max(), 1.76)
+    npt.assert_allclose(data["horizontalError"].min(), 0.09)
+    npt.assert_allclose(data["horizontalError"].max(), 36.8)
+    npt.assert_allclose(data["depthError"].min(), 0)
+    npt.assert_allclose(data["depthError"].max(), 65.06)
+    npt.assert_allclose(data["magError"].min(), 0.02)
+    npt.assert_allclose(data["magError"].max(), 0.524)
+    npt.assert_allclose(data["magNst"].min(), 1)
+    npt.assert_allclose(data["magNst"].max(), 944)
 
 
 def test_fractures_compilation():
     """
     Check that the @fractures_06.txt dataset loads without errors.
     """
-    with pytest.warns(expected_warning=FutureWarning) as record:
-        data = load_fractures_compilation()
-        assert len(record) == 1
+    data = load_sample_data(name="fractures")
     assert data.shape == (361, 2)
     assert data["length"].min() == 98.6561
     assert data["length"].max() == 984.652
     assert data["azimuth"].min() == 0.0
     assert data["azimuth"].max() == 360.0
 
 
 def test_mars_shape():
     """
     Check that the @mars370d.txt dataset loads without errors.
     """
-    with pytest.warns(expected_warning=FutureWarning) as record:
-        data = load_mars_shape()
-        assert len(record) == 1
+    data = load_sample_data(name="mars_shape")
     assert data.shape == (370, 3)
     assert data["longitude"].min() == 0.008
     assert data["longitude"].max() == 359.983
     assert data["latitude"].min() == -79.715
     assert data["latitude"].max() == 85.887
-    assert data["radius(m)"].min() == -6930
-    assert data["radius(m)"].max() == 15001
+    assert data["radius_m"].min() == -6930
+    assert data["radius_m"].max() == 15001
 
 
 def test_hotspots():
     """
     Check that the @hotspots.txt dataset loads without errors.
     """
-    with pytest.warns(expected_warning=FutureWarning) as record:
-        data = load_hotspots()
-        assert len(record) == 1
+    data = load_sample_data(name="hotspots")
     assert data.shape == (55, 4)
     assert list(data.columns) == [
         "longitude",
         "latitude",
         "symbol_size",
         "place_name",
     ]
     assert isinstance(data, pd.DataFrame)
+    assert data["longitude"].min() == -169.6
+    assert data["longitude"].max() == 167
+    assert data["latitude"].min() == -78
+    assert data["latitude"].max() == 64
+    assert data["symbol_size"].min() == 0.25
+    assert data["symbol_size"].max() == 0.5
 
 
 def test_load_notre_dame_topography():
     """
     Check that the @Table_5_11.txt dataset loads without errors.
     """
     data = load_sample_data(name="notre_dame_topography")
```

### Comparing `pygmt-0.8.0/pygmt/tests/test_dimfilter.py` & `pygmt-0.9.0/pygmt/tests/test_dimfilter.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,18 +28,18 @@
         data=[
             [346.0, 344.5, 349.0, 349.0],
             [344.5, 318.5, 344.5, 394.0],
             [344.5, 356.5, 345.5, 352.5],
             [367.5, 349.0, 385.5, 349.0],
             [435.0, 385.5, 413.5, 481.5],
         ],
-        coords=dict(
-            lon=[-54.5, -53.5, -52.5, -51.5],
-            lat=[-23.5, -22.5, -21.5, -20.5, -19.5],
-        ),
+        coords={
+            "lon": [-54.5, -53.5, -52.5, -51.5],
+            "lat": [-23.5, -22.5, -21.5, -20.5, -19.5],
+        },
         dims=["lat", "lon"],
     )
 
 
 def test_dimfilter_outgrid(grid, expected_grid):
     """
     Test the required parameters for dimfilter with a set outgrid.
```

### Comparing `pygmt-0.8.0/pygmt/tests/test_figure.py` & `pygmt-0.9.0/pygmt/tests/test_figure.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Doesn't include the plotting commands which have their own test files.
 """
 import os
 from pathlib import Path
 
 try:
     import IPython
-except ModuleNotFoundError:
+except ImportError:
     IPython = None  # pylint: disable=invalid-name
 
 
 import numpy as np
 import numpy.testing as npt
 import pytest
 from pygmt import Figure, set_display
@@ -170,33 +170,62 @@
     fig = Figure()
     fig.psconvert = mock_psconvert
 
     prefix = "test_figure_savefig"
 
     fname = ".".join([prefix, "png"])
     fig.savefig(fname)
-    assert kwargs_saved[-1] == dict(prefix=prefix, fmt="g", crop=True, Qt=2, Qg=2)
+    assert kwargs_saved[-1] == {
+        "prefix": prefix,
+        "fmt": "g",
+        "crop": True,
+        "Qt": 2,
+        "Qg": 2,
+    }
 
     fname = ".".join([prefix, "pdf"])
     fig.savefig(fname)
-    assert kwargs_saved[-1] == dict(prefix=prefix, fmt="f", crop=True, Qt=2, Qg=2)
+    assert kwargs_saved[-1] == {
+        "prefix": prefix,
+        "fmt": "f",
+        "crop": True,
+        "Qt": 2,
+        "Qg": 2,
+    }
 
     fname = ".".join([prefix, "png"])
     fig.savefig(fname, transparent=True)
-    assert kwargs_saved[-1] == dict(prefix=prefix, fmt="G", crop=True, Qt=2, Qg=2)
+    assert kwargs_saved[-1] == {
+        "prefix": prefix,
+        "fmt": "G",
+        "crop": True,
+        "Qt": 2,
+        "Qg": 2,
+    }
 
     fname = ".".join([prefix, "eps"])
     fig.savefig(fname)
-    assert kwargs_saved[-1] == dict(prefix=prefix, fmt="e", crop=True, Qt=2, Qg=2)
+    assert kwargs_saved[-1] == {
+        "prefix": prefix,
+        "fmt": "e",
+        "crop": True,
+        "Qt": 2,
+        "Qg": 2,
+    }
 
     fname = ".".join([prefix, "kml"])
     fig.savefig(fname)
-    assert kwargs_saved[-1] == dict(
-        prefix=prefix, fmt="g", crop=True, Qt=2, Qg=2, W="+k"
-    )
+    assert kwargs_saved[-1] == {
+        "prefix": prefix,
+        "fmt": "g",
+        "crop": True,
+        "Qt": 2,
+        "Qg": 2,
+        "W": "+k",
+    }
 
 
 @pytest.mark.skipif(IPython is None, reason="run when IPython is installed")
 def test_figure_show():
     """
     Test that show creates the correct file name and deletes the temp dir.
     """
@@ -206,15 +235,15 @@
 
 
 @pytest.mark.mpl_image_compare
 def test_figure_shift_origin():
     """
     Test if fig.shift_origin works.
     """
-    kwargs = dict(region=[0, 3, 0, 5], projection="X3c/5c", frame=0)
+    kwargs = {"region": [0, 3, 0, 5], "projection": "X3c/5c", "frame": 0}
     fig = Figure()
     # First call shift_origin without projection and region.
     # Test issue https://github.com/GenericMappingTools/pygmt/issues/514
     fig.shift_origin(xshift="2c", yshift="3c")
     fig.basemap(**kwargs)
     fig.shift_origin(xshift="4c")
     fig.basemap(**kwargs)
```

### Comparing `pygmt-0.8.0/pygmt/tests/test_filter1d.py` & `pygmt-0.9.0/pygmt/tests/test_filter1d.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_geopandas.py` & `pygmt-0.9.0/pygmt/tests/test_geopandas.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_grd2cpt.py` & `pygmt-0.9.0/pygmt/tests/test_grd2cpt.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_grd2xyz.py` & `pygmt-0.9.0/pygmt/tests/test_grd2xyz.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_grdclip.py` & `pygmt-0.9.0/pygmt/tests/test_grdclip.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     """
     return xr.DataArray(
         data=[
             [1000.0, 570.5, -1000.0, -1000.0],
             [1000.0, 1000.0, 571.5, 638.5],
             [555.5, 556.0, 580.0, 1000.0],
         ],
-        coords=dict(lon=[-52.5, -51.5, -50.5, -49.5], lat=[-18.5, -17.5, -16.5]),
+        coords={"lon": [-52.5, -51.5, -50.5, -49.5], "lat": [-18.5, -17.5, -16.5]},
         dims=["lat", "lon"],
     )
 
 
 def test_grdclip_outgrid(grid, expected_grid):
     """
     Test the below and above parameters for grdclip and creates a test outgrid.
```

### Comparing `pygmt-0.8.0/pygmt/tests/test_grdcontour.py` & `pygmt-0.9.0/pygmt/tests/test_grdcontour.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_grdcut.py` & `pygmt-0.9.0/pygmt/tests/test_grdcut.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     """
     return xr.DataArray(
         data=[
             [446.5, 481.5, 439.5, 553.0],
             [757.0, 570.5, 538.5, 524.0],
             [796.0, 886.0, 571.5, 638.5],
         ],
-        coords=dict(lon=[-52.5, -51.5, -50.5, -49.5], lat=[-19.5, -18.5, -17.5]),
+        coords={"lon": [-52.5, -51.5, -50.5, -49.5], "lat": [-19.5, -18.5, -17.5]},
         dims=["lat", "lon"],
     )
 
 
 def test_grdcut_dataarray_in_file_out(grid, expected_grid, region):
     """
     grdcut an input DataArray, and output to a grid file.
```

### Comparing `pygmt-0.8.0/pygmt/tests/test_grdfill.py` & `pygmt-0.9.0/pygmt/tests/test_grdfill.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,22 +3,19 @@
 """
 from pathlib import Path
 
 import numpy as np
 import pytest
 import xarray as xr
 from packaging.version import Version
-from pygmt import clib, grdfill, load_dataarray
+from pygmt import __gmt_version__, grdfill, load_dataarray
 from pygmt.exceptions import GMTInvalidInput
 from pygmt.helpers import GMTTempFile
 from pygmt.helpers.testing import load_static_earth_relief
 
-with clib.Session() as _lib:
-    gmt_version = Version(_lib.info["version"])
-
 
 @pytest.fixture(scope="module", name="grid")
 def fixture_grid():
     """
     Load the grid data from the static_earth_relief file and set value(s) to
     NaN and inf.
     """
@@ -46,17 +43,17 @@
             [601.0, 526.5, 535.0, 299.0, 398.5, 645.0, 797.5, 964.0],
             [494.5, 488.5, 357.0, 254.5, 286.0, 484.5, 653.5, 930.0],
             [450.5, 395.5, 366.0, 248.0, 250.0, 354.5, 550.0, 797.5],
             [345.5, 320.0, 335.0, 292.0, 207.5, 247.0, 325.0, 346.5],
             [349.0, 313.0, 325.5, 247.0, 191.0, 225.0, 260.0, 452.5],
             [347.5, 331.5, 309.0, 282.0, 190.0, 208.0, 299.5, 348.0],
         ],
-        coords=dict(
-            lon=[-54.5, -53.5, -52.5, -51.5, -50.5, -49.5, -48.5, -47.5],
-            lat=[
+        coords={
+            "lon": [-54.5, -53.5, -52.5, -51.5, -50.5, -49.5, -48.5, -47.5],
+            "lat": [
                 -23.5,
                 -22.5,
                 -21.5,
                 -20.5,
                 -19.5,
                 -18.5,
                 -17.5,
@@ -64,15 +61,15 @@
                 -15.5,
                 -14.5,
                 -13.5,
                 -12.5,
                 -11.5,
                 -10.5,
             ],
-        ),
+        },
         dims=["lat", "lon"],
     )
 
 
 def test_grdfill_dataarray_out(grid, expected_grid):
     """
     Test grdfill with a DataArray output.
@@ -83,15 +80,15 @@
     assert result.gmt.gtype == 1  # Geographic grid
     assert result.gmt.registration == 1  # Pixel registration
     # check information of the output grid
     xr.testing.assert_allclose(a=result, b=expected_grid)
 
 
 @pytest.mark.skipif(
-    gmt_version < Version("6.4.0"),
+    Version(__gmt_version__) < Version("6.4.0"),
     reason="Upstream bug/crash fixed in https://github.com/GenericMappingTools/gmt/pull/6418.",
 )
 def test_grdfill_asymmetric_pad(grid, expected_grid):
     """
     Test grdfill using a region that includes the edge of the grid.
 
     Regression test for
```

### Comparing `pygmt-0.8.0/pygmt/tests/test_grdfilter.py` & `pygmt-0.9.0/pygmt/tests/test_grdfilter.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,18 +27,18 @@
     """
     return xr.DataArray(
         data=[
             [502.61914, 488.27576, 494.10657, 559.06244],
             [614.6496, 601.4992, 569.9743, 606.0966],
             [661.41003, 656.9681, 625.1668, 664.40204],
         ],
-        coords=dict(
-            lon=[-52.5, -51.5, -50.5, -49.5],
-            lat=[-19.5, -18.5, -17.5],
-        ),
+        coords={
+            "lon": [-52.5, -51.5, -50.5, -49.5],
+            "lat": [-19.5, -18.5, -17.5],
+        },
         dims=["lat", "lon"],
     )
 
 
 def test_grdfilter_dataarray_in_dataarray_out(grid, expected_grid):
     """
     Test grdfilter with an input DataArray, and output as DataArray.
```

### Comparing `pygmt-0.8.0/pygmt/tests/test_grdgradient.py` & `pygmt-0.9.0/pygmt/tests/test_grdgradient.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,18 +26,18 @@
     """
     return xr.DataArray(
         data=[
             [-1.5974800e-03, -9.9056680e-04, -6.1276241e-04, -3.6172546e-04],
             [-1.5880326e-03, -1.6113354e-03, -5.4624723e-04, -5.0047837e-04],
             [7.2569086e-04, 2.4801277e-04, 1.8859128e-05, -1.2269041e-03],
         ],
-        coords=dict(
-            lon=[-52.5, -51.5, -50.5, -49.5],
-            lat=[-19.5, -18.5, -17.5],
-        ),
+        coords={
+            "lon": [-52.5, -51.5, -50.5, -49.5],
+            "lat": [-19.5, -18.5, -17.5],
+        },
         dims=["lat", "lon"],
     )
 
 
 def test_grdgradient_outgrid(grid, expected_grid):
     """
     Test the azimuth and direction parameters for grdgradient with a set
```

### Comparing `pygmt-0.8.0/pygmt/tests/test_grdhisteq.py` & `pygmt-0.9.0/pygmt/tests/test_grdhisteq.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,18 @@
 @pytest.fixture(scope="module", name="expected_grid")
 def fixture_expected_grid():
     """
     Load the expected grdhisteq grid result.
     """
     return xr.DataArray(
         data=[[0, 0, 0, 1], [0, 0, 0, 1], [0, 0, 1, 1], [1, 1, 1, 1]],
-        coords=dict(lon=[-51.5, -50.5, -49.5, -48.5], lat=[-21.5, -20.5, -19.5, -18.5]),
+        coords={
+            "lon": [-51.5, -50.5, -49.5, -48.5],
+            "lat": [-21.5, -20.5, -19.5, -18.5],
+        },
         dims=["lat", "lon"],
     )
 
 
 @pytest.fixture(scope="module", name="expected_df")
 def fixture_expected_df():
     """
```

### Comparing `pygmt-0.8.0/pygmt/tests/test_grdimage.py` & `pygmt-0.9.0/pygmt/tests/test_grdimage.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,22 +115,21 @@
     The ``shading`` can be True, a constant intensity, some modifiers, or
     a grid with modifiers.
 
     See https://github.com/GenericMappingTools/pygmt/issues/364 and
     https://github.com/GenericMappingTools/pygmt/issues/618.
     """
     fig_ref, fig_test = Figure(), Figure()
-    kwargs = dict(
-        region=[-180, 180, -90, 90],
-        frame=True,
-        projection="Cyl_stere/6i",
-        cmap="geo",
-        shading=shading,
-    )
-
+    kwargs = {
+        "region": [-180, 180, -90, 90],
+        "frame": True,
+        "projection": "Cyl_stere/6i",
+        "cmap": "geo",
+        "shading": shading,
+    }
     fig_ref.grdimage("@earth_relief_01d_g", **kwargs)
     fig_test.grdimage(grid, **kwargs)
     return fig_ref, fig_test
 
 
 @check_figures_equal()
 def test_grdimage_grid_and_shading_with_xarray(grid, xrgrid):
```

### Comparing `pygmt-0.8.0/pygmt/tests/test_grdinfo.py` & `pygmt-0.9.0/pygmt/tests/test_grdinfo.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_grdlandmask.py` & `pygmt-0.9.0/pygmt/tests/test_grdlandmask.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,18 @@
             [0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
             [0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
             [0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
             [0.0, 0.0, 0.0, 0.0, 0.0, 1.0],
             [0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
             [0.0, 0.0, 1.0, 1.0, 0.0, 0.0],
         ],
-        coords=dict(
-            lon=[125.0, 126.0, 127.0, 128.0, 129.0, 130.0],
-            lat=[30.0, 31.0, 32.0, 33.0, 34.0, 35.0],
-        ),
+        coords={
+            "lon": [125.0, 126.0, 127.0, 128.0, 129.0, 130.0],
+            "lat": [30.0, 31.0, 32.0, 33.0, 34.0, 35.0],
+        },
         dims=["lat", "lon"],
     )
 
 
 def test_grdlandmask_outgrid(expected_grid):
     """
     Creates a grid land mask with an outgrid argument.
```

### Comparing `pygmt-0.8.0/pygmt/tests/test_grdproject.py` & `pygmt-0.9.0/pygmt/tests/test_grdproject.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,18 @@
         data=[
             [427.85062, 431.05698, 452.34268],
             [563.92957, 540.5212, 501.46896],
             [740.80133, 679.1116, 554.78534],
             [794.233, 829.4449, 764.12225],
             [749.37445, 834.55994, 831.2627],
         ],
-        coords=dict(
-            x=[1.666667, 5.0, 8.333333],
-            y=[1.572432, 4.717295, 7.862158, 11.007022, 14.151885],
-        ),
+        coords={
+            "x": [1.666667, 5.0, 8.333333],
+            "y": [1.572432, 4.717295, 7.862158, 11.007022, 14.151885],
+        },
         dims=["y", "x"],
     )
 
 
 def test_grdproject_file_out(grid, expected_grid):
     """
     grdproject with an outgrid set.
```

### Comparing `pygmt-0.8.0/pygmt/tests/test_grdsample.py` & `pygmt-0.9.0/pygmt/tests/test_grdsample.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,18 +43,18 @@
         data=[
             [460.84375, 482.78125, 891.09375],
             [680.46875, 519.09375, 764.9375],
             [867.75, 579.03125, 852.53125],
             [551.75, 666.6875, 958.21875],
             [411.3125, 518.4375, 931.28125],
         ],
-        coords=dict(
-            lon=[-52, -50, -48],
-            lat=[-19.5, -18.5, -17.5, -16.5, -15.5],
-        ),
+        coords={
+            "lon": [-52, -50, -48],
+            "lat": [-19.5, -18.5, -17.5, -16.5, -15.5],
+        },
         dims=["lat", "lon"],
     )
 
 
 def test_grdsample_file_out(grid, expected_grid, region, spacing):
     """
     Test grdsample with an outgrid set and the spacing is changed.
```

### Comparing `pygmt-0.8.0/pygmt/tests/test_grdtrack.py` & `pygmt-0.9.0/pygmt/tests/test_grdtrack.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 @pytest.fixture(scope="module", name="dataframe")
 def fixture_dataframe():
     """
     Load a pandas DataFrame with points.
     """
     return pd.read_csv(
-        POINTS_DATA, sep=r"\s+", header=None, names=["longitude", "latitude"]
+        POINTS_DATA, delim_whitespace=True, header=None, names=["longitude", "latitude"]
     )
 
 
 def test_grdtrack_input_dataframe_and_dataarray(dataarray, dataframe, expected_array):
     """
     Run grdtrack by passing in a pandas.DataFrame and xarray.DataArray as
     inputs.
@@ -173,22 +173,7 @@
 
 def test_grdtrack_set_points_and_profile(dataarray, dataframe):
     """
     Run grdtrack but set both 'points' and 'profile'.
     """
     with pytest.raises(GMTInvalidInput):
         grdtrack(grid=dataarray, points=dataframe, profile="BL/TR")
-
-
-def test_grdtrack_old_parameter_order(dataframe, dataarray, expected_array):
-    """
-    Run grdtrack with the old parameter order 'points, grid'.
-
-    This test should be removed in v0.9.0.
-    """
-    for points in (POINTS_DATA, dataframe):
-        for grid in ("@static_earth_relief.nc", dataarray):
-            with pytest.warns(expected_warning=FutureWarning) as record:
-                output = grdtrack(points, grid)
-                assert len(record) == 1
-                assert isinstance(output, pd.DataFrame)
-                npt.assert_allclose(np.array(output), expected_array)
```

### Comparing `pygmt-0.8.0/pygmt/tests/test_grdview.py` & `pygmt-0.9.0/pygmt/tests/test_grdview.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_grdvolume.py` & `pygmt-0.9.0/pygmt/tests/test_grdvolume.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_helpers.py` & `pygmt-0.9.0/pygmt/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_histogram.py` & `pygmt-0.9.0/pygmt/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_info.py` & `pygmt-0.9.0/pygmt/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_inset.py` & `pygmt-0.9.0/pygmt/tests/test_inset.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_io.py` & `pygmt-0.9.0/pygmt/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_legend.py` & `pygmt-0.9.0/pygmt/tests/test_legend.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_logo.py` & `pygmt-0.9.0/pygmt/tests/test_logo.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_makecpt.py` & `pygmt-0.9.0/pygmt/tests/test_makecpt.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_meca.py` & `pygmt-0.9.0/pygmt/tests/test_meca.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     """
     Test supplying a dictionary containing a single focal mechanism to the spec
     parameter.
     """
     fig = Figure()
     # Right lateral strike slip focal mechanism
     fig.meca(
-        spec=dict(strike=0, dip=90, rake=0, magnitude=5),
+        spec={"strike": 0, "dip": 90, "rake": 0, "magnitude": 5},
         longitude=0,
         latitude=5,
         depth=0,
         scale="2.5c",
         region=[-1, 1, 4, 6],
         projection="M14c",
         frame=2,
@@ -33,17 +33,20 @@
 def test_meca_spec_dict_list():
     """
     Test supplying a dictionary containing a list of focal mechanism to the
     spec parameter.
     """
     fig = Figure()
     # supply focal mechanisms as a dict of lists
-    focal_mechanisms = dict(
-        strike=[330, 350], dip=[30, 50], rake=[90, 90], magnitude=[3, 2]
-    )
+    focal_mechanisms = {
+        "strike": [330, 350],
+        "dip": [30, 50],
+        "rake": [90, 90],
+        "magnitude": [3, 2],
+    }
     fig.meca(
         spec=focal_mechanisms,
         longitude=[-123.5, -124.5],
         latitude=[47.5, 48.5],
         depth=[12.0, 11.0],
         region=[-125, -122, 47, 49],
         scale="2c",
@@ -57,25 +60,24 @@
 def test_meca_spec_dataframe():
     """
     Test supplying a pandas.DataFrame containing focal mechanisms and locations
     to the spec parameter.
     """
 
     fig = Figure()
-
     # supply focal mechanisms to meca as a dataframe
-    focal_mechanisms = dict(
-        strike=[324, 353],
-        dip=[20.6, 40],
-        rake=[83, 90],
-        magnitude=[3.4, 2.9],
-        longitude=[-124, -124.4],
-        latitude=[48.1, 48.2],
-        depth=[12, 11.0],
-    )
+    focal_mechanisms = {
+        "strike": [324, 353],
+        "dip": [20.6, 40],
+        "rake": [83, 90],
+        "magnitude": [3.4, 2.9],
+        "longitude": [-124, -124.4],
+        "latitude": [48.1, 48.2],
+        "depth": [12, 11.0],
+    }
     fig.meca(
         spec=pd.DataFrame(data=focal_mechanisms),
         region=[-125, -122, 47, 49],
         scale="2c",
         projection="M14c",
     )
     return fig
@@ -177,17 +179,20 @@
 def test_meca_loc_array():
     """
     Test supplying lists and np.ndarrays as the event location (longitude,
     latitude, and depth).
     """
     fig = Figure()
     # specify focal mechanisms
-    focal_mechanisms = dict(
-        strike=[327, 350], dip=[41, 50], rake=[68, 90], magnitude=[3, 2]
-    )
+    focal_mechanisms = {
+        "strike": [327, 350],
+        "dip": [41, 50],
+        "rake": [68, 90],
+        "magnitude": [3, 2],
+    }
     # longitude, latitude, and depth may be specified as an int, float,
     # list, or 1-D numpy array
     longitude = np.array([-123.3, -124.4])
     latitude = np.array([48.4, 48.2])
     depth = [12.0, 11.0]  # to test mixed data types as inputs
     scale = "2c"
     fig.meca(
@@ -205,24 +210,24 @@
 @pytest.mark.mpl_image_compare
 def test_meca_gcmt_convention():
     """
     Test plotting beachballs using the global CMT convention.
     """
     fig = Figure()
     # specify focal mechanisms
-    focal_mechanisms = dict(
-        strike1=180,
-        dip1=18,
-        rake1=-88,
-        strike2=0,
-        dip2=72,
-        rake2=-90,
-        mantissa=5.5,
-        exponent=0,
-    )
+    focal_mechanisms = {
+        "strike1": 180,
+        "dip1": 18,
+        "rake1": -88,
+        "strike2": 0,
+        "dip2": 72,
+        "rake2": -90,
+        "mantissa": 5.5,
+        "exponent": 0,
+    }
     fig.meca(
         spec=focal_mechanisms,
         scale="1c",
         longitude=239.384,
         latitude=34.556,
         depth=12,
         convention="gcmt",
@@ -235,15 +240,15 @@
 
 @pytest.mark.mpl_image_compare
 def test_meca_dict_offset():
     """
     Test offsetting beachballs for a dict input.
     """
     fig = Figure()
-    focal_mechanism = dict(strike=330, dip=30, rake=90, magnitude=3)
+    focal_mechanism = {"strike": 330, "dip": 30, "rake": 90, "magnitude": 3}
     fig.basemap(region=[-125, -122, 47, 49], projection="M6c", frame=True)
     fig.meca(
         spec=focal_mechanism,
         scale="1c",
         longitude=-124,
         latitude=48,
         depth=12.0,
@@ -258,22 +263,22 @@
     """
     Test offsetting beachballs for a dict input with offset parameters in the
     dict.
 
     See https://github.com/GenericMappingTools/pygmt/issues/2016.
     """
     fig = Figure()
-    focal_mechanism = dict(
-        strike=330,
-        dip=30,
-        rake=90,
-        magnitude=3,
-        plot_longitude=-124.5,
-        plot_latitude=47.5,
-    )
+    focal_mechanism = {
+        "strike": 330,
+        "dip": 30,
+        "rake": 90,
+        "magnitude": 3,
+        "plot_longitude": -124.5,
+        "plot_latitude": 47.5,
+    }
     fig.basemap(region=[-125, -122, 47, 49], projection="M6c", frame=True)
     fig.meca(
         spec=focal_mechanism,
         scale="1c",
         longitude=-124,
         latitude=48,
         depth=12.0,
@@ -283,15 +288,15 @@
 
 @pytest.mark.mpl_image_compare
 def test_meca_dict_eventname():
     """
     Test offsetting beachballs for a dict input.
     """
     fig = Figure()
-    focal_mechanism = dict(strike=330, dip=30, rake=90, magnitude=3)
+    focal_mechanism = {"strike": 330, "dip": 30, "rake": 90, "magnitude": 3}
     fig.basemap(region=[-125, -122, 47, 49], projection="M6c", frame=True)
     fig.meca(
         spec=focal_mechanism,
         scale="1c",
         longitude=-124,
         latitude=48,
         depth=12.0,
@@ -302,15 +307,15 @@
 
 @pytest.mark.mpl_image_compare
 def test_meca_dict_offset_eventname():
     """
     Test offsetting beachballs for a dict input.
     """
     fig = Figure()
-    focal_mechanism = dict(strike=330, dip=30, rake=90, magnitude=3)
+    focal_mechanism = {"strike": 330, "dip": 30, "rake": 90, "magnitude": 3}
     fig.basemap(region=[-125, -122, 47, 49], projection="M6c", frame=True)
     fig.meca(
         spec=focal_mechanism,
         scale="1c",
         longitude=-124,
         latitude=48,
         depth=12.0,
@@ -328,20 +333,20 @@
 
     This is a regression test for
     https://github.com/GenericMappingTools/pygmt/pull/2174
     """
     fig = Figure()
     fig.basemap(region=[-125, -122, 47, 49], projection="M6c", frame=True)
     fig.meca(
-        spec=dict(
-            strike=330,
-            dip=30,
-            rake=90,
-            magnitude=3,
-            longitude=-124,
-            latitude=48,
-            depth=12.0,
-            event_name="Event20220311",
-        ),
+        spec={
+            "strike": 330,
+            "dip": 30,
+            "rake": 90,
+            "magnitude": 3,
+            "longitude": -124,
+            "latitude": 48,
+            "depth": 12.0,
+            "event_name": "Event20220311",
+        },
         scale="1c",
     )
     return fig
```

### Comparing `pygmt-0.8.0/pygmt/tests/test_nearneighbor.py` & `pygmt-0.9.0/pygmt/tests/test_nearneighbor.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_plot.py` & `pygmt-0.9.0/pygmt/tests/test_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
 def test_plot_fail_1d_array_with_data(data, region):
     """
     Should raise an exception if array fill, size, intensity and transparency
     are used with matrix.
     """
     fig = Figure()
-    kwargs = dict(data=data, region=region, projection="X10c", frame="afg")
+    kwargs = {"data": data, "region": region, "projection": "X10c", "frame": "afg"}
     with pytest.raises(GMTInvalidInput):
         fig.plot(style="c0.2c", fill=data[:, 2], **kwargs)
     with pytest.raises(GMTInvalidInput):
         fig.plot(style="cc", size=data[:, 2], fill="red", **kwargs)
     with pytest.raises(GMTInvalidInput):
         fig.plot(style="c0.2c", fill="red", intensity=data[:, 2], **kwargs)
     with pytest.raises(GMTInvalidInput):
@@ -511,14 +511,15 @@
     datasets = ["@RidgeTest" + suffix for suffix in [".shp", ".shx", ".dbf", ".prj"]]
     which(fname=datasets, download="a")
     fig = Figure()
     fig.plot(data="@RidgeTest.shp", pen="1p", frame=True)
     return fig
 
 
+@pytest.mark.mpl_image_compare
 def test_plot_dataframe_incols():
     """
     Make sure that the incols parameter works for pandas.DataFrame.
 
     See https://github.com/GenericMappingTools/pygmt/issues/1440.
     """
     data = pd.DataFrame(data={"col1": [-0.5, 0, 0.5], "col2": [-0.75, 0, 0.75]})
```

### Comparing `pygmt-0.8.0/pygmt/tests/test_plot3d.py` & `pygmt-0.9.0/pygmt/tests/test_plot3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
 def test_plot3d_fail_1d_array_with_data(data, region):
     """
     Should raise an exception if array fill, size, intensity and transparency
     are used with matrix.
     """
     fig = Figure()
-    kwargs = dict(data=data, region=region, projection="X10c", frame="afg")
+    kwargs = {"data": data, "region": region, "projection": "X10c", "frame": "afg"}
     with pytest.raises(GMTInvalidInput):
         fig.plot3d(style="c0.2c", fill=data[:, 2], **kwargs)
     with pytest.raises(GMTInvalidInput):
         fig.plot3d(style="cc", size=data[:, 2], fill="red", **kwargs)
     with pytest.raises(GMTInvalidInput):
         fig.plot3d(style="cc", intensity=data[:, 2], fill="red", **kwargs)
     with pytest.raises(GMTInvalidInput):
@@ -100,15 +100,15 @@
     fig.plot3d(
         x=data[:, 0],
         y=data[:, 1],
         z=data[:, 2],
         zscale=5,
         perspective=[225, 30],
         region=region,
-        projection="R270/10c",
+        projection="R40/10c",
         style="s1c",
         fill="green",
         frame=["ag", "zag"],
     )
     return fig
```

### Comparing `pygmt-0.8.0/pygmt/tests/test_project.py` & `pygmt-0.9.0/pygmt/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_psconvert.py` & `pygmt-0.9.0/pygmt/tests/test_psconvert.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_rose.py` & `pygmt-0.9.0/pygmt/tests/test_rose.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_select.py` & `pygmt-0.9.0/pygmt/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_session_management.py` & `pygmt-0.9.0/pygmt/tests/test_session_management.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_solar.py` & `pygmt-0.9.0/pygmt/tests/test_solar.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_sph2grd.py` & `pygmt-0.9.0/pygmt/tests/test_sph2grd.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_sphdistance.py` & `pygmt-0.9.0/pygmt/tests/test_sphdistance.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_sphinterpolate.py` & `pygmt-0.9.0/pygmt/tests/test_sphinterpolate.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_sphinx_gallery.py` & `pygmt-0.9.0/pygmt/tests/test_sphinx_gallery.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_subplot.py` & `pygmt-0.9.0/pygmt/tests/test_subplot.py`

 * *Files 21% similar despite different names*

```diff
@@ -96,7 +96,25 @@
     """
     Check that an error is raised when nrows or ncols is less than one.
     """
     fig = Figure()
     with pytest.raises(GMTInvalidInput):
         with fig.subplot(nrows=0, ncols=-1, figsize=("2c", "1c")):
             pass
+
+
+# Increase tolerance for compatibility with GMT 6.3 and 6.4, see
+# https://github.com/GenericMappingTools/pygmt/pull/2454
+@pytest.mark.mpl_image_compare(tolerance=4.0)
+def test_subplot_outside_plotting_positioning():
+    """
+    Plotting calls are correctly positioned after exiting subplot.
+
+    This is a regression test for
+    https://github.com/GenericMappingTools/pygmt/issues/2426.
+    """
+    fig = Figure()
+    with fig.subplot(nrows=1, ncols=2, figsize=(10, 5)):
+        fig.basemap(region=[0, 10, 0, 10], projection="X?", panel=True)
+        fig.basemap(region=[0, 10, 0, 10], projection="X?", panel=True)
+    fig.colorbar(position="JBC+w5c+h", cmap="turbo", frame=True)
+    return fig
```

### Comparing `pygmt-0.8.0/pygmt/tests/test_surface.py` & `pygmt-0.9.0/pygmt/tests/test_surface.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 @pytest.fixture(scope="module", name="data")
 def fixture_data():
     """
     Load Table 5.11 in Davis: Statistics and Data Analysis in Geology.
     """
     fname = which("@Table_5_11_mean.xyz", download="c")
     return pd.read_csv(
-        fname, sep=r"\s+", header=None, names=["x", "y", "z"], skiprows=1
+        fname, delim_whitespace=True, header=None, names=["x", "y", "z"], skiprows=1
     )
 
 
 @pytest.fixture(scope="module", name="region")
 def fixture_region():
     """
     Define the region.
@@ -51,18 +51,18 @@
             [878.5973, 851.71, 814.6884, 812.1127, 819.9591],
             [842.0522, 815.2896, 788.2292, 777.0031, 785.6345],
             [854.2515, 813.3035, 781, 742.3641, 735.6497],
             [882.972, 818.4636, 773.611, 718.7798, 685.4824],
             [897.4532, 822.9642, 756.4472, 687.594, 626.2299],
             [910.2932, 823.3307, 737.9952, 651.4994, 565.9981],
         ],
-        coords=dict(
-            y=[0, 1, 2, 3, 4, 5, 6, 7, 8],
-            x=[0, 1, 2, 3, 4],
-        ),
+        coords={
+            "y": [0, 1, 2, 3, 4, 5, 6, 7, 8],
+            "x": [0, 1, 2, 3, 4],
+        },
         dims=[
             "y",
             "x",
         ],
     )
```

### Comparing `pygmt-0.8.0/pygmt/tests/test_ternary.py` & `pygmt-0.9.0/pygmt/tests/test_ternary.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_text.py` & `pygmt-0.9.0/pygmt/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_triangulate.py` & `pygmt-0.9.0/pygmt/tests/test_triangulate.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 @pytest.fixture(scope="module", name="dataframe")
 def fixture_dataframe():
     """
     Load the table data from the sample bathymetry dataset.
     """
     fname = which("@Table_5_11_mean.xyz", download="c")
     return pd.read_csv(
-        fname, sep=r"\s+", header=None, names=["x", "y", "z"], skiprows=1
+        fname, delim_whitespace=True, header=None, names=["x", "y", "z"], skiprows=1
     )[:10]
 
 
 @pytest.fixture(scope="module", name="expected_dataframe")
 def fixture_expected_dataframe():
     """
     Load the expected triangulate dataframe result.
@@ -50,15 +50,15 @@
 @pytest.fixture(scope="module", name="expected_grid")
 def fixture_expected_grid():
     """
     Load the expected triangulate grid result.
     """
     return xr.DataArray(
         data=[[779.6264, 752.1539, 749.38776], [771.2882, 726.9792, 722.1368]],
-        coords=dict(y=[5, 6], x=[2, 3, 4]),
+        coords={"y": [5, 6], "x": [2, 3, 4]},
         dims=["y", "x"],
     )
 
 
 @pytest.mark.parametrize("array_func", [np.array, xr.Dataset])
 def test_delaunay_triples_input_table_matrix(array_func, dataframe, expected_dataframe):
     """
```

### Comparing `pygmt-0.8.0/pygmt/tests/test_velo.py` & `pygmt-0.9.0/pygmt/tests/test_velo.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_which.py` & `pygmt-0.9.0/pygmt/tests/test_which.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_wiggle.py` & `pygmt-0.9.0/pygmt/tests/test_wiggle.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_x2sys_cross.py` & `pygmt-0.9.0/pygmt/tests/test_x2sys_cross.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_x2sys_init.py` & `pygmt-0.9.0/pygmt/tests/test_x2sys_init.py`

 * *Files identical despite different names*

### Comparing `pygmt-0.8.0/pygmt/tests/test_xyz2grd.py` & `pygmt-0.9.0/pygmt/tests/test_xyz2grd.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,18 +27,18 @@
     """
     return xr.DataArray(
         data=[
             [-3651.0608, -3015.214, -2320.1033],
             [-2546.2512, -1977.8754, -963.23303],
             [-352.3795, -1025.4508, np.nan],
         ],
-        coords=dict(
-            x=[245.0, 250.0, 255.0],
-            y=[20.0, 25.0, 30.0],
-        ),
+        coords={
+            "x": [245.0, 250.0, 255.0],
+            "y": [20.0, 25.0, 30.0],
+        },
         dims=["y", "x"],
     )
 
 
 @pytest.mark.parametrize("array_func", [np.array, xr.Dataset])
 def test_xyz2grd_input_array(array_func, ship_data, expected_grid):
     """
```

### Comparing `pygmt-0.8.0/pygmt.egg-info/PKG-INFO` & `pygmt-0.9.0/pygmt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: pygmt
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Python interface for the Generic Mapping Tools
 Author-email: The PyGMT Developers <pygmt.team@gmail.com>
 License: BSD License
 Project-URL: homepage, https://www.pygmt.org
 Project-URL: documentation, https://www.pygmt.org
 Project-URL: repository, https://github.com/GenericMappingTools/pygmt
 Project-URL: changelog, https://www.pygmt.org/latest/changes.html
+Keywords: cartography,geodesy,geology,geophysics,geospatial,oceanography,seismology
 Platform: Any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
@@ -80,30 +81,31 @@
 ----------
 
 A beautiful map is worth a thousand words.
 To truly understand how powerful PyGMT is, play with it online on `Binder <https://github.com/GenericMappingTools/try-gmt>`__!
 For a quicker introduction, check out our `3 minute overview <https://youtu.be/4iPnITXrxVU>`__!
 
 Afterwards, feel free to look at our `Tutorials <https://www.pygmt.org/latest/tutorials>`__,
-visit the `PyGMT Gallery <https://www.pygmt.org/latest/gallery>`__, and check out
+visit the `Gallery <https://www.pygmt.org/latest/gallery>`__, and check out
 some `external PyGMT examples <https://www.pygmt.org/latest/external_resources.html>`__!
 
 .. image:: https://user-images.githubusercontent.com/14077947/155809878-48b8f235-141b-460a-80ec-08bbf6c36e40.png
     :alt: Quick Introduction to PyGMT YouTube Video
     :align: center
     :target: https://youtu.be/4iPnITXrxVU
     :width: 80%
 
 About
 -----
 
 PyGMT is a library for processing geospatial and geophysical data and making
-publication quality maps and figures. It provides a Pythonic interface for the
+publication-quality maps and figures. It provides a Pythonic interface for the
 `Generic Mapping Tools (GMT) <https://github.com/GenericMappingTools/gmt>`__, a
-command-line program widely used in the Earth Sciences.
+command-line program widely used across the Earth, Ocean, and Planetary sciences
+and beyond.
 
 Project goals
 -------------
 
 * Make GMT more accessible to new users.
 * Build a Pythonic API for GMT.
 * Interface with the GMT C API directly using ctypes (no system calls).
@@ -116,24 +118,38 @@
 
 Quickstart
 ----------
 
 Installation
 ++++++++++++
 
-Simple installation using `conda <https://docs.conda.io/projects/conda/en/latest/user-guide/index.html>`__::
+Simple installation using `mamba <https://mamba.readthedocs.org/>`__::
 
-    conda install --channel conda-forge pygmt
+    mamba install --channel conda-forge pygmt
 
-If you use `mamba <https://mamba.readthedocs.org/>`__::
+If you use `conda <https://docs.conda.io/projects/conda/en/latest/user-guide/index.html>`__::
 
-    mamba install --channel conda-forge pygmt
+    conda install --channel conda-forge pygmt
 
 For other ways to install ``pygmt``, see `full installation instructions <https://www.pygmt.org/latest/install.html>`__.
 
+Getting started
++++++++++++++++
+
+As a starting point, you can open a `Python interpreter <https://docs.python.org/3/tutorial/interpreter.html>`__
+or a `Jupyter notebook <https://docs.jupyter.org/en/latest/running.html>`__, and try the following example::
+
+    import pygmt
+    fig = pygmt.Figure()
+    fig.coast(projection="H10c", region="g", frame=True, land="gray")
+    fig.show()
+
+For more examples, please have a look at the `Gallery <https://www.pygmt.org/latest/gallery/index.html>`__
+and `Tutorials <https://www.pygmt.org/latest/tutorials/index.html>`__.
+
 
 Contacting Us
 -------------
 
 * Most discussion happens `on GitHub
   <https://github.com/GenericMappingTools/pygmt>`__. Feel free to `open an issue
   <https://github.com/GenericMappingTools/pygmt/issues/new>`__ or comment on any
@@ -190,47 +206,49 @@
 PyGMT is a community developed project. See the
 `AUTHORS.md <https://github.com/GenericMappingTools/pygmt/blob/main/AUTHORS.md>`__
 file on GitHub for a list of the people involved and a definition of the term "PyGMT
 Developers". Feel free to cite our work in your research using the following BibTeX:
 
 .. code-block::
 
-    @software{pygmt_2022_7481934,
+    @software{pygmt_2023_7772533,
       author       = {Uieda, Leonardo and
                       Tian, Dongdong and
                       Leong, Wei Ji and
-                      Jones, Max and
                       Schlitzer, William and
                       Grund, Michael and
-                      Toney, Liam and
+                      Jones, Max and
                       Fröhlich, Yvonne and
+                      Toney, Liam and
                       Yao, Jiayuan and
                       Magen, Yohai and
+                      Tong, Jing-Hui and
                       Materna, Kathryn and
                       Belem, Andre and
                       Newton, Tyler and
                       Anant, Abhishek and
                       Ziebarth, Malte and
                       Quinn, Jamie and
                       Wessel, Paul},
       title        = {{PyGMT: A Python interface for the Generic Mapping Tools}},
-      month        = dec,
-      year         = 2022,
+      month        = mar,
+      year         = 2023,
       publisher    = {Zenodo},
-      version      = {0.8.0},
-      doi          = {10.5281/zenodo.7481934},
-      url          = {https://doi.org/10.5281/zenodo.7481934}
+      version      = {0.9.0},
+      doi          = {10.5281/zenodo.7772533},
+      url          = {https://doi.org/10.5281/zenodo.7772533}
     }
 
 To cite a specific version of PyGMT, go to our Zenodo page at
 https://doi.org/10.5281/zenodo.3781524 and use the "Export to BibTeX" function there.
 It is also strongly recommended to cite the
 `GMT6 paper <https://doi.org/10.1029/2019GC008515>`__ (which PyGMT wraps around).
-Note that some modules like ``surface`` and ``x2sys`` also have their dedicated citation.
-Further information for all these can be found at https://www.generic-mapping-tools.org/cite.
+Note that some modules like ``dimfilter``, ``surface``, and ``x2sys`` also have their
+dedicated citations. Further information for all these can be found at
+https://www.generic-mapping-tools.org/cite.
 
 
 License
 -------
 
 PyGMT is free software: you can redistribute it and/or modify it under the terms of
 the **BSD 3-clause License**. A copy of this license is provided in
@@ -271,16 +289,21 @@
       - GMT
       - Python
       - NumPy
     * - `Dev <https://github.com/GenericMappingTools/pygmt/milestones>`_ (upcoming release)
       - `Dev Documentation <https://www.pygmt.org/dev>`_ (reflects `main branch <https://github.com/GenericMappingTools/pygmt>`_)
       - >=6.3.0
       - >=3.8
-      - >=1.20
-    * - `v0.8.0 <https://github.com/GenericMappingTools/pygmt/releases/tag/v0.8.0>`_ (latest release)
+      - >=1.21
+    * - `v0.9.0 <https://github.com/GenericMappingTools/pygmt/releases/tag/v0.9.0>`_ (latest release)
+      - `v0.9.0 Documentation <https://www.pygmt.org/v0.9.0>`_
+      - >=6.3.0
+      - >=3.8
+      - >=1.21
+    * - `v0.8.0 <https://github.com/GenericMappingTools/pygmt/releases/tag/v0.8.0>`_
       - `v0.8.0 Documentation <https://www.pygmt.org/v0.8.0>`_
       - >=6.3.0
       - >=3.8
       - >=1.20
     * - `v0.7.0 <https://github.com/GenericMappingTools/pygmt/releases/tag/v0.7.0>`_
       - `v0.7.0 Documentation <https://www.pygmt.org/v0.7.0>`_
       - >=6.3.0
```

### Comparing `pygmt-0.8.0/pygmt.egg-info/SOURCES.txt` & `pygmt-0.9.0/pygmt.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 AUTHORSHIP.md
 CITATION.cff
 CODE_OF_CONDUCT.md
 LICENSE.txt
 MANIFEST.in
 README.rst
 pyproject.toml
-setup.cfg
 pygmt/__init__.py
 pygmt/accessors.py
 pygmt/exceptions.py
 pygmt/figure.py
 pygmt/io.py
 pygmt/session_management.py
 pygmt/sphinx_gallery.py
@@ -24,18 +23,20 @@
 pygmt/clib/loading.py
 pygmt/clib/session.py
 pygmt/datasets/__init__.py
 pygmt/datasets/earth_age.py
 pygmt/datasets/earth_free_air_anomaly.py
 pygmt/datasets/earth_geoid.py
 pygmt/datasets/earth_magnetic_anomaly.py
+pygmt/datasets/earth_mask.py
 pygmt/datasets/earth_relief.py
 pygmt/datasets/earth_vertical_gravity_gradient.py
 pygmt/datasets/load_remote_dataset.py
 pygmt/datasets/samples.py
+pygmt/datasets/tile_map.py
 pygmt/helpers/__init__.py
 pygmt/helpers/decorators.py
 pygmt/helpers/tempfile.py
 pygmt/helpers/testing.py
 pygmt/helpers/utils.py
 pygmt/src/__init__.py
 pygmt/src/basemap.py
@@ -82,14 +83,16 @@
 pygmt/src/sph2grd.py
 pygmt/src/sphdistance.py
 pygmt/src/sphinterpolate.py
 pygmt/src/subplot.py
 pygmt/src/surface.py
 pygmt/src/ternary.py
 pygmt/src/text.py
+pygmt/src/tilemap.py
+pygmt/src/timestamp.py
 pygmt/src/triangulate.py
 pygmt/src/velo.py
 pygmt/src/which.py
 pygmt/src/wiggle.py
 pygmt/src/x2sys_cross.py
 pygmt/src/x2sys_init.py
 pygmt/src/xyz2grd.py
@@ -108,14 +111,15 @@
 pygmt/tests/test_colorbar.py
 pygmt/tests/test_config.py
 pygmt/tests/test_contour.py
 pygmt/tests/test_datasets_earth_age.py
 pygmt/tests/test_datasets_earth_free_air_anomaly.py
 pygmt/tests/test_datasets_earth_geoid.py
 pygmt/tests/test_datasets_earth_magnetic_anomaly.py
+pygmt/tests/test_datasets_earth_mask.py
 pygmt/tests/test_datasets_earth_relief.py
 pygmt/tests/test_datasets_earth_vertical_gravity_gradient.py
 pygmt/tests/test_datasets_samples.py
 pygmt/tests/test_dimfilter.py
 pygmt/tests/test_figure.py
 pygmt/tests/test_filter1d.py
 pygmt/tests/test_geopandas.py
@@ -136,14 +140,15 @@
 pygmt/tests/test_grdtrack.py
 pygmt/tests/test_grdview.py
 pygmt/tests/test_grdvolume.py
 pygmt/tests/test_helpers.py
 pygmt/tests/test_histogram.py
 pygmt/tests/test_image.py
 pygmt/tests/test_info.py
+pygmt/tests/test_init.py
 pygmt/tests/test_inset.py
 pygmt/tests/test_io.py
 pygmt/tests/test_legend.py
 pygmt/tests/test_logo.py
 pygmt/tests/test_makecpt.py
 pygmt/tests/test_meca.py
 pygmt/tests/test_nearneighbor.py
@@ -159,29 +164,31 @@
 pygmt/tests/test_sphdistance.py
 pygmt/tests/test_sphinterpolate.py
 pygmt/tests/test_sphinx_gallery.py
 pygmt/tests/test_subplot.py
 pygmt/tests/test_surface.py
 pygmt/tests/test_ternary.py
 pygmt/tests/test_text.py
+pygmt/tests/test_tilemap.py
+pygmt/tests/test_timestamp.py
 pygmt/tests/test_triangulate.py
 pygmt/tests/test_velo.py
 pygmt/tests/test_which.py
 pygmt/tests/test_wiggle.py
 pygmt/tests/test_x2sys_cross.py
 pygmt/tests/test_x2sys_init.py
 pygmt/tests/test_xyz2grd.py
 pygmt/tests/baseline/test_basemap.png.dvc
 pygmt/tests/baseline/test_basemap_compass.png.dvc
 pygmt/tests/baseline/test_basemap_loglog.png.dvc
 pygmt/tests/baseline/test_basemap_map_scale.png.dvc
 pygmt/tests/baseline/test_basemap_polar.png.dvc
 pygmt/tests/baseline/test_basemap_power_axis.png.dvc
-pygmt/tests/baseline/test_basemap_required_args.png.dvc
 pygmt/tests/baseline/test_basemap_rose.png.dvc
+pygmt/tests/baseline/test_basemap_subplot.png.dvc
 pygmt/tests/baseline/test_basemap_utm_projection.png.dvc
 pygmt/tests/baseline/test_basemap_winkel_tripel.png.dvc
 pygmt/tests/baseline/test_coast_dcw_list.png.dvc
 pygmt/tests/baseline/test_coast_dcw_single.png.dvc
 pygmt/tests/baseline/test_coast_region.png.dvc
 pygmt/tests/baseline/test_coast_world_mercator.png.dvc
 pygmt/tests/baseline/test_colorbar_box.png.dvc
@@ -310,14 +317,15 @@
 pygmt/tests/baseline/test_rose_plot_with_transparency.png.dvc
 pygmt/tests/baseline/test_solar_set_terminator_datetime.png.dvc
 pygmt/tests/baseline/test_solar_terminators.png.dvc
 pygmt/tests/baseline/test_subplot_autolabel_margins_title.png.dvc
 pygmt/tests/baseline/test_subplot_basic_frame.png.dvc
 pygmt/tests/baseline/test_subplot_clearance_and_shared_xy_axis_layout.png.dvc
 pygmt/tests/baseline/test_subplot_direct.png.dvc
+pygmt/tests/baseline/test_subplot_outside_plotting_positioning.png.dvc
 pygmt/tests/baseline/test_ternary.png.dvc
 pygmt/tests/baseline/test_ternary_1_label.png.dvc
 pygmt/tests/baseline/test_ternary_3_labels.png.dvc
 pygmt/tests/baseline/test_text_angle_30.png.dvc
 pygmt/tests/baseline/test_text_angle_font_justify_from_textfile.png.dvc
 pygmt/tests/baseline/test_text_fill.png.dvc
 pygmt/tests/baseline/test_text_font_bold.png.dvc
@@ -331,14 +339,24 @@
 pygmt/tests/baseline/test_text_pen.png.dvc
 pygmt/tests/baseline/test_text_position.png.dvc
 pygmt/tests/baseline/test_text_position_offset_with_line.png.dvc
 pygmt/tests/baseline/test_text_round_clearance.png.dvc
 pygmt/tests/baseline/test_text_single_line_of_text.png.dvc
 pygmt/tests/baseline/test_text_transparency.png.dvc
 pygmt/tests/baseline/test_text_varying_transparency.png.dvc
+pygmt/tests/baseline/test_tilemap_no_clip_False.png.dvc
+pygmt/tests/baseline/test_tilemap_no_clip_True.png.dvc
+pygmt/tests/baseline/test_tilemap_ogc_wgs84.png.dvc
+pygmt/tests/baseline/test_tilemap_web_mercator.png.dvc
+pygmt/tests/baseline/test_timestamp.png.dvc
+pygmt/tests/baseline/test_timestamp_font.png.dvc
+pygmt/tests/baseline/test_timestamp_justification.png.dvc
+pygmt/tests/baseline/test_timestamp_label.png.dvc
+pygmt/tests/baseline/test_timestamp_offset.png.dvc
+pygmt/tests/baseline/test_timestamp_text_truncated.png.dvc
 pygmt/tests/baseline/test_velo_numpy_array_numeric_only.png.dvc
 pygmt/tests/baseline/test_velo_pandas_dataframe.png.dvc
 pygmt/tests/baseline/test_wiggle.png.dvc
 pygmt/tests/data/cities.txt
 pygmt/tests/data/contours.txt
 pygmt/tests/data/points.txt
 pygmt/tests/data/track.txt
```

### Comparing `pygmt-0.8.0/pyproject.toml` & `pygmt-0.9.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -5,41 +5,51 @@
 [project]
 name = "pygmt"
 description = "A Python interface for the Generic Mapping Tools"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {text = "BSD License"}
 authors = [{name = "The PyGMT Developers", email = "pygmt.team@gmail.com"}]
-keywords = []
+keywords = [
+    "cartography",
+    "geodesy",
+    "geology",
+    "geophysics",
+    "geospatial",
+    "oceanography",
+    "seismology",
+]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development :: Libraries",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: BSD License",
 ]
 dependencies = [
-    "numpy>=1.20",
+    "numpy>=1.21",
     "pandas",
     "xarray",
     "netCDF4",
-    "packaging"
+    "packaging",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 all = [
+    "contextily",
     "geopandas",
-    "ipython"
+    "ipython",
+    "rioxarray",
 ]
 
 [project.urls]
 homepage = "https://www.pygmt.org"
 documentation = "https://www.pygmt.org"
 repository = "https://github.com/GenericMappingTools/pygmt"
 changelog = "https://www.pygmt.org/latest/changes.html"
```


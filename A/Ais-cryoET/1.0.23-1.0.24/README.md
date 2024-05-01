# Comparing `tmp/Ais-cryoET-1.0.23.tar.gz` & `tmp/Ais-cryoET-1.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Ais-cryoET-1.0.23.tar", last modified: Thu Mar 28 11:32:11 2024, max compression
+gzip compressed data, was "Ais-cryoET-1.0.24.tar", last modified: Wed May  1 07:35:45 2024, max compression
```

## Comparing `Ais-cryoET-1.0.23.tar` & `Ais-cryoET-1.0.24.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 11:32:11.352032 Ais-cryoET-1.0.23/
-drwxrwxrwx   0        0        0        0 2024-03-28 11:32:11.128874 Ais-cryoET-1.0.23/Ais/
--rw-rw-rw-   0        0        0    36025 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/LICENSE.txt
--rw-rw-rw-   0        0        0        0 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 11:32:11.195081 Ais-cryoET-1.0.23/Ais/core/
--rw-rw-rw-   0        0        0        0 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/core/__init__.py
--rw-rw-rw-   0        0        0     5069 2024-03-28 11:32:03.000000 Ais-cryoET-1.0.23/Ais/core/config.py
--rw-rw-rw-   0        0        0     1637 2024-01-02 08:48:51.000000 Ais-cryoET-1.0.23/Ais/core/extract.py
--rw-rw-rw-   0        0        0     2640 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/core/open_in_blender.py
--rw-rw-rw-   0        0        0      625 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/core/open_in_chimerax.py
--rw-rw-rw-   0        0        0    17600 2023-12-13 11:43:47.000000 Ais-cryoET-1.0.23/Ais/core/opengl_classes.py
--rw-rw-rw-   0        0        0    33046 2024-02-08 12:56:17.000000 Ais-cryoET-1.0.23/Ais/core/se_frame.py
--rw-rw-rw-   0        0        0    24255 2024-03-26 11:05:39.000000 Ais-cryoET-1.0.23/Ais/core/se_model.py
--rw-rw-rw-   0        0        0   192280 2024-03-28 11:17:34.000000 Ais-cryoET-1.0.23/Ais/core/segmentation_editor.py
--rw-rw-rw-   0        0        0      331 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/core/settings.py
--rw-rw-rw-   0        0        0      130 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/core/settings.txt
--rw-rw-rw-   0        0        0       98 2024-01-02 10:33:08.000000 Ais-cryoET-1.0.23/Ais/core/start.py
--rw-rw-rw-   0        0        0    22298 2024-03-28 11:18:29.000000 Ais-cryoET-1.0.23/Ais/core/util.py
--rw-rw-rw-   0        0        0     2572 2023-12-21 15:04:18.000000 Ais-cryoET-1.0.23/Ais/core/widgets.py
--rw-rw-rw-   0        0        0     7894 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/core/window.py
-drwxrwxrwx   0        0        0        0 2024-03-28 11:32:11.239023 Ais-cryoET-1.0.23/Ais/icons/
--rw-rw-rw-   0        0        0  1098617 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/icons/LOGO_Pom_1024.png
--rw-rw-rw-   0        0        0    19430 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/icons/LOGO_Pom_128.png
--rw-rw-rw-   0        0        0  2960366 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/icons/LOGO_Pom_2048.png
--rw-rw-rw-   0        0        0   134990 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/icons/LOGO_Pom_256.png
--rw-rw-rw-   0        0        0   401274 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/icons/LOGO_Pom_512.png
--rw-rw-rw-   0        0        0        0 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/icons/__init__.py
--rw-rw-rw-   0        0        0     8843 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/icons/icon_blender_256.png
--rw-rw-rw-   0        0        0    30131 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/icons/icon_chimerax_256.png
--rw-rw-rw-   0        0        0     1563 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/icons/icon_close_256.png
--rw-rw-rw-   0        0        0      954 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/icons/icon_crop_256.png
--rw-rw-rw-   0        0        0     5113 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/icons/icon_obj_256.png
--rw-rw-rw-   0        0        0      784 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/icons/icon_stop_256.png
--rw-rw-rw-   0        0        0     2001 2024-01-02 08:48:51.000000 Ais-cryoET-1.0.23/Ais/main.py
-drwxrwxrwx   0        0        0        0 2024-03-28 11:32:11.280130 Ais-cryoET-1.0.23/Ais/models/
--rw-rw-rw-   0        0        0       15 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/models/__init__.py
--rw-rw-rw-   0        0        0      819 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/models/eman2.py
--rw-rw-rw-   0        0        0     1359 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/models/inceptionnet.py
--rw-rw-rw-   0        0        0     2149 2024-02-06 08:17:58.000000 Ais-cryoET-1.0.23/Ais/models/model_template.py
--rw-rw-rw-   0        0        0     7759 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/models/pix2pix.py
--rw-rw-rw-   0        0        0     1562 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/models/resnet.py
--rw-rw-rw-   0        0        0     1166 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/models/unet_deep.py
--rw-rw-rw-   0        0        0      973 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/models/unet_dropout.py
--rw-rw-rw-   0        0        0      889 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/models/unet_lite.py
--rw-rw-rw-   0        0        0     1559 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/models/vggnet.py
--rw-rw-rw-   0        0        0     1568 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/models/vggnet_plus.py
--rw-rw-rw-   0        0        0      207 2024-01-02 08:48:52.000000 Ais-cryoET-1.0.23/Ais/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-03-28 11:32:11.332069 Ais-cryoET-1.0.23/Ais/shaders/
--rw-rw-rw-   0        0        0        0 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/shaders/__init__.py
--rw-rw-rw-   0        0        0      372 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/shaders/ce_line_shader.glsl
--rw-rw-rw-   0        0        0      725 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/shaders/se_binary_segmentation_shader.glsl
--rw-rw-rw-   0        0        0      424 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/shaders/se_border_shader.glsl
--rw-rw-rw-   0        0        0      929 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/shaders/se_compute_kernel_filter.glsl
--rw-rw-rw-   0        0        0      808 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/shaders/se_compute_mix.glsl
--rw-rw-rw-   0        0        0      487 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/shaders/se_depth_mask_shader.glsl
--rw-rw-rw-   0        0        0      696 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/shaders/se_float_segmentation_shader.glsl
--rw-rw-rw-   0        0        0      649 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/shaders/se_icon_shader.glsl
--rw-rw-rw-   0        0        0      286 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/shaders/se_line_3d_shader.glsl
--rw-rw-rw-   0        0        0      449 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/shaders/se_overlay_blend_shader.glsl
--rw-rw-rw-   0        0        0     3359 2023-11-30 12:28:22.000000 Ais-cryoET-1.0.23/Ais/shaders/se_overlay_ray_trace_shader.glsl
--rw-rw-rw-   0        0        0     1188 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/shaders/se_overlay_shader.glsl
--rw-rw-rw-   0        0        0      454 2024-01-02 13:56:12.000000 Ais-cryoET-1.0.23/Ais/shaders/se_particle_shader.glsl
--rw-rw-rw-   0        0        0      827 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/shaders/se_quad_3d_shader.glsl
--rw-rw-rw-   0        0        0     1019 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.23/Ais/shaders/se_quad_shader.glsl
--rw-rw-rw-   0        0        0     1950 2023-12-03 15:17:59.000000 Ais-cryoET-1.0.23/Ais/shaders/se_surface_model_shader.glsl
-drwxrwxrwx   0        0        0        0 2024-03-28 11:32:11.348038 Ais-cryoET-1.0.23/Ais_cryoET.egg-info/
--rw-rw-rw-   0        0        0     5068 2024-03-28 11:32:10.000000 Ais-cryoET-1.0.23/Ais_cryoET.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1861 2024-03-28 11:32:11.000000 Ais-cryoET-1.0.23/Ais_cryoET.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 11:32:10.000000 Ais-cryoET-1.0.23/Ais_cryoET.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-03-28 11:32:11.000000 Ais-cryoET-1.0.23/Ais_cryoET.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      196 2024-03-28 11:32:11.000000 Ais-cryoET-1.0.23/Ais_cryoET.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-03-28 11:32:11.000000 Ais-cryoET-1.0.23/Ais_cryoET.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-10-23 08:03:57.000000 Ais-cryoET-1.0.23/MANIFEST.in
--rw-rw-rw-   0        0        0     5068 2024-03-28 11:32:11.348038 Ais-cryoET-1.0.23/PKG-INFO
--rw-rw-rw-   0        0        0     4706 2023-12-14 16:04:51.000000 Ais-cryoET-1.0.23/README.md
--rw-rw-rw-   0        0        0       42 2024-03-28 11:32:11.352032 Ais-cryoET-1.0.23/setup.cfg
--rw-rw-rw-   0        0        0     1396 2024-03-28 11:31:06.000000 Ais-cryoET-1.0.23/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 07:35:45.539061 Ais-cryoET-1.0.24/
+drwxrwxrwx   0        0        0        0 2024-05-01 07:35:45.259590 Ais-cryoET-1.0.24/Ais/
+-rw-rw-rw-   0        0        0    36025 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/LICENSE.txt
+-rw-rw-rw-   0        0        0        0 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 07:35:45.371909 Ais-cryoET-1.0.24/Ais/core/
+-rw-rw-rw-   0        0        0        0 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/core/__init__.py
+-rw-rw-rw-   0        0        0     5069 2024-05-01 07:35:39.000000 Ais-cryoET-1.0.24/Ais/core/config.py
+-rw-rw-rw-   0        0        0     1637 2024-01-02 08:48:51.000000 Ais-cryoET-1.0.24/Ais/core/extract.py
+-rw-rw-rw-   0        0        0     2640 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/core/open_in_blender.py
+-rw-rw-rw-   0        0        0      625 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/core/open_in_chimerax.py
+-rw-rw-rw-   0        0        0    17600 2023-12-13 11:43:47.000000 Ais-cryoET-1.0.24/Ais/core/opengl_classes.py
+-rw-rw-rw-   0        0        0    33047 2024-04-15 16:00:16.000000 Ais-cryoET-1.0.24/Ais/core/se_frame.py
+-rw-rw-rw-   0        0        0    24255 2024-03-26 11:05:39.000000 Ais-cryoET-1.0.24/Ais/core/se_model.py
+-rw-rw-rw-   0        0        0   192280 2024-03-28 11:17:34.000000 Ais-cryoET-1.0.24/Ais/core/segmentation_editor.py
+-rw-rw-rw-   0        0        0      331 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/core/settings.py
+-rw-rw-rw-   0        0        0      130 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/core/settings.txt
+-rw-rw-rw-   0        0        0       98 2024-01-02 10:33:08.000000 Ais-cryoET-1.0.24/Ais/core/start.py
+-rw-rw-rw-   0        0        0    22298 2024-03-28 11:18:29.000000 Ais-cryoET-1.0.24/Ais/core/util.py
+-rw-rw-rw-   0        0        0     2572 2023-12-21 15:04:18.000000 Ais-cryoET-1.0.24/Ais/core/widgets.py
+-rw-rw-rw-   0        0        0     7961 2024-05-01 07:34:37.000000 Ais-cryoET-1.0.24/Ais/core/window.py
+drwxrwxrwx   0        0        0        0 2024-05-01 07:35:45.423770 Ais-cryoET-1.0.24/Ais/icons/
+-rw-rw-rw-   0        0        0  1098617 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/icons/LOGO_Pom_1024.png
+-rw-rw-rw-   0        0        0    19430 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/icons/LOGO_Pom_128.png
+-rw-rw-rw-   0        0        0  2960366 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/icons/LOGO_Pom_2048.png
+-rw-rw-rw-   0        0        0   134990 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/icons/LOGO_Pom_256.png
+-rw-rw-rw-   0        0        0   401274 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/icons/LOGO_Pom_512.png
+-rw-rw-rw-   0        0        0        0 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/icons/__init__.py
+-rw-rw-rw-   0        0        0     8843 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/icons/icon_blender_256.png
+-rw-rw-rw-   0        0        0    30131 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/icons/icon_chimerax_256.png
+-rw-rw-rw-   0        0        0     1563 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/icons/icon_close_256.png
+-rw-rw-rw-   0        0        0      954 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/icons/icon_crop_256.png
+-rw-rw-rw-   0        0        0     5113 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/icons/icon_obj_256.png
+-rw-rw-rw-   0        0        0      784 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/icons/icon_stop_256.png
+-rw-rw-rw-   0        0        0     2001 2024-01-02 08:48:51.000000 Ais-cryoET-1.0.24/Ais/main.py
+drwxrwxrwx   0        0        0        0 2024-05-01 07:35:45.471504 Ais-cryoET-1.0.24/Ais/models/
+-rw-rw-rw-   0        0        0       15 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/models/__init__.py
+-rw-rw-rw-   0        0        0      819 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/models/eman2.py
+-rw-rw-rw-   0        0        0     1359 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/models/inceptionnet.py
+-rw-rw-rw-   0        0        0     2149 2024-02-06 08:17:58.000000 Ais-cryoET-1.0.24/Ais/models/model_template.py
+-rw-rw-rw-   0        0        0     7759 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/models/pix2pix.py
+-rw-rw-rw-   0        0        0     1562 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/models/resnet.py
+-rw-rw-rw-   0        0        0     1166 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/models/unet_deep.py
+-rw-rw-rw-   0        0        0      973 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/models/unet_dropout.py
+-rw-rw-rw-   0        0        0      889 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/models/unet_lite.py
+-rw-rw-rw-   0        0        0     1559 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/models/vggnet.py
+-rw-rw-rw-   0        0        0     1568 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/models/vggnet_plus.py
+-rw-rw-rw-   0        0        0      207 2024-01-02 08:48:52.000000 Ais-cryoET-1.0.24/Ais/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 07:35:45.522431 Ais-cryoET-1.0.24/Ais/shaders/
+-rw-rw-rw-   0        0        0        0 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/shaders/__init__.py
+-rw-rw-rw-   0        0        0      372 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/shaders/ce_line_shader.glsl
+-rw-rw-rw-   0        0        0      725 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/shaders/se_binary_segmentation_shader.glsl
+-rw-rw-rw-   0        0        0      424 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/shaders/se_border_shader.glsl
+-rw-rw-rw-   0        0        0      929 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/shaders/se_compute_kernel_filter.glsl
+-rw-rw-rw-   0        0        0      808 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/shaders/se_compute_mix.glsl
+-rw-rw-rw-   0        0        0      487 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/shaders/se_depth_mask_shader.glsl
+-rw-rw-rw-   0        0        0      696 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/shaders/se_float_segmentation_shader.glsl
+-rw-rw-rw-   0        0        0      649 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/shaders/se_icon_shader.glsl
+-rw-rw-rw-   0        0        0      286 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/shaders/se_line_3d_shader.glsl
+-rw-rw-rw-   0        0        0      449 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/shaders/se_overlay_blend_shader.glsl
+-rw-rw-rw-   0        0        0     3359 2023-11-30 12:28:22.000000 Ais-cryoET-1.0.24/Ais/shaders/se_overlay_ray_trace_shader.glsl
+-rw-rw-rw-   0        0        0     1188 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/shaders/se_overlay_shader.glsl
+-rw-rw-rw-   0        0        0      454 2024-01-02 13:56:12.000000 Ais-cryoET-1.0.24/Ais/shaders/se_particle_shader.glsl
+-rw-rw-rw-   0        0        0      827 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/shaders/se_quad_3d_shader.glsl
+-rw-rw-rw-   0        0        0     1019 2023-11-29 15:57:43.000000 Ais-cryoET-1.0.24/Ais/shaders/se_quad_shader.glsl
+-rw-rw-rw-   0        0        0     1950 2023-12-03 15:17:59.000000 Ais-cryoET-1.0.24/Ais/shaders/se_surface_model_shader.glsl
+drwxrwxrwx   0        0        0        0 2024-05-01 07:35:45.523436 Ais-cryoET-1.0.24/Ais_cryoET.egg-info/
+-rw-rw-rw-   0        0        0     5068 2024-05-01 07:35:44.000000 Ais-cryoET-1.0.24/Ais_cryoET.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1861 2024-05-01 07:35:44.000000 Ais-cryoET-1.0.24/Ais_cryoET.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 07:35:44.000000 Ais-cryoET-1.0.24/Ais_cryoET.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-05-01 07:35:44.000000 Ais-cryoET-1.0.24/Ais_cryoET.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      196 2024-05-01 07:35:44.000000 Ais-cryoET-1.0.24/Ais_cryoET.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-01 07:35:44.000000 Ais-cryoET-1.0.24/Ais_cryoET.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-10-23 08:03:57.000000 Ais-cryoET-1.0.24/MANIFEST.in
+-rw-rw-rw-   0        0        0     5068 2024-05-01 07:35:45.523436 Ais-cryoET-1.0.24/PKG-INFO
+-rw-rw-rw-   0        0        0     4706 2023-12-14 16:04:51.000000 Ais-cryoET-1.0.24/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-01 07:35:45.539061 Ais-cryoET-1.0.24/setup.cfg
+-rw-rw-rw-   0        0        0     1396 2024-05-01 07:35:39.000000 Ais-cryoET-1.0.24/setup.py
```

### Comparing `Ais-cryoET-1.0.23/Ais/LICENSE.txt` & `Ais-cryoET-1.0.24/Ais/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/core/config.py` & `Ais-cryoET-1.0.24/Ais/core/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import platform
 
 # TODO: .tif files as input
 
 frozen = False
 root = os.path.dirname(os.path.dirname(__file__))
 app_name = "Ais"
-version = "1.0.23"
+version = "1.0.24"
 license = "GNU GPL v3"
 log_title = "Ais.log"
 log_path = os.path.join(root, log_title)
 
 filetype_segmentation = ".scns"
 filetype_traindata = ".scnt"
 filetype_semodel = ".scnm"
```

### Comparing `Ais-cryoET-1.0.23/Ais/core/extract.py` & `Ais-cryoET-1.0.24/Ais/core/extract.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/core/open_in_blender.py` & `Ais-cryoET-1.0.24/Ais/core/open_in_blender.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/core/open_in_chimerax.py` & `Ais-cryoET-1.0.24/Ais/core/open_in_chimerax.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/core/opengl_classes.py` & `Ais-cryoET-1.0.24/Ais/core/opengl_classes.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/core/se_frame.py` & `Ais-cryoET-1.0.24/Ais/core/se_frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -492,15 +492,15 @@
                 mrc.set_data(np.array([image, annotation]))
                 mrc.voxel_size = self.parent.pixel_size * 10.0
             print(f"Slice saved to: {fpath}")
         except Exception as e:
             cfg.set_error(e, "Could not save current slice, see details below.")
 
     def save_volume(self):
-        fpath = os.path.splitext(self.parent.path)[0] + self.title + f"__annotations.mrc"
+        fpath = os.path.splitext(self.parent.path)[0] + "__" + self.title + f"_manual.mrc"
         try:
             with mrcfile.new(fpath, overwrite=True) as outf:
                 vol = np.zeros((self.parent.n_slices, self.parent.height, self.parent.width), dtype=np.uint8)
                 for i in self.edited_slices:
                     vol[i] = self.slices[i]
                 outf.set_data(vol * 255)
                 outf.voxel_size = self.parent.pixel_size * 10.0
```

### Comparing `Ais-cryoET-1.0.23/Ais/core/se_model.py` & `Ais-cryoET-1.0.24/Ais/core/se_model.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/core/segmentation_editor.py` & `Ais-cryoET-1.0.24/Ais/core/segmentation_editor.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/core/util.py` & `Ais-cryoET-1.0.24/Ais/core/util.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/core/widgets.py` & `Ais-cryoET-1.0.24/Ais/core/widgets.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/core/window.py` & `Ais-cryoET-1.0.24/Ais/core/window.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import glfw
-from platform import system
-from OpenGL.GL import *
+
+from OpenGL.GL import (
+    glBlendFunc, glEnable, glClearColor, glClear, glViewport,
+    GL_TRUE, GL_SRC_ALPHA, GL_ONE_MINUS_SRC_ALPHA, GL_BLEND,
+    GL_MULTISAMPLE, GL_COLOR_BUFFER_BIT, GL_DEPTH_BUFFER_BIT,
+)
 
 
 class Window:
     def __init__(self, width, height, title):
         self.width = width
         self.height = height
         self.title = title
         self.clear_color = (0.0, 0.0, 0.0, 1.0)
         glfw.window_hint(glfw.CONTEXT_VERSION_MAJOR, 3)
         glfw.window_hint(glfw.CONTEXT_VERSION_MINOR, 3)
         glfw.window_hint(glfw.OPENGL_PROFILE, glfw.OPENGL_CORE_PROFILE)
-        glfw.window_hint(glfw.OPENGL_FORWARD_COMPAT, OpenGL.GL.GL_TRUE)
-        glfw.window_hint(glfw.RESIZABLE, glfw.TRUE)  ## in order to avoid an issue with pyimgui multiple contexts, window sizes are fixed.
+        glfw.window_hint(glfw.OPENGL_FORWARD_COMPAT, GL_TRUE)
+        glfw.window_hint(glfw.RESIZABLE, glfw.TRUE)
         glfw.window_hint(glfw.SAMPLES, 4)
         self.glfw_window = glfw.create_window(self.width, self.height, self.title, None, None)
         self.focused = True
         glfw.make_context_current(self.glfw_window)
         glBlendFunc(GL_SRC_ALPHA, GL_ONE_MINUS_SRC_ALPHA)
         glEnable(GL_BLEND)
         glEnable(GL_MULTISAMPLE)
```

### Comparing `Ais-cryoET-1.0.23/Ais/icons/LOGO_Pom_1024.png` & `Ais-cryoET-1.0.24/Ais/icons/LOGO_Pom_1024.png`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/icons/LOGO_Pom_128.png` & `Ais-cryoET-1.0.24/Ais/icons/LOGO_Pom_128.png`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/icons/LOGO_Pom_2048.png` & `Ais-cryoET-1.0.24/Ais/icons/LOGO_Pom_2048.png`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/icons/LOGO_Pom_256.png` & `Ais-cryoET-1.0.24/Ais/icons/LOGO_Pom_256.png`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/icons/LOGO_Pom_512.png` & `Ais-cryoET-1.0.24/Ais/icons/LOGO_Pom_512.png`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/icons/icon_blender_256.png` & `Ais-cryoET-1.0.24/Ais/icons/icon_blender_256.png`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/icons/icon_chimerax_256.png` & `Ais-cryoET-1.0.24/Ais/icons/icon_chimerax_256.png`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/icons/icon_close_256.png` & `Ais-cryoET-1.0.24/Ais/icons/icon_close_256.png`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/icons/icon_crop_256.png` & `Ais-cryoET-1.0.24/Ais/icons/icon_crop_256.png`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/icons/icon_obj_256.png` & `Ais-cryoET-1.0.24/Ais/icons/icon_obj_256.png`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/icons/icon_stop_256.png` & `Ais-cryoET-1.0.24/Ais/icons/icon_stop_256.png`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/main.py` & `Ais-cryoET-1.0.24/Ais/main.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/models/eman2.py` & `Ais-cryoET-1.0.24/Ais/models/eman2.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/models/inceptionnet.py` & `Ais-cryoET-1.0.24/Ais/models/inceptionnet.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/models/model_template.py` & `Ais-cryoET-1.0.24/Ais/models/model_template.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/models/pix2pix.py` & `Ais-cryoET-1.0.24/Ais/models/pix2pix.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/models/resnet.py` & `Ais-cryoET-1.0.24/Ais/models/resnet.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/models/unet_deep.py` & `Ais-cryoET-1.0.24/Ais/models/unet_deep.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/models/unet_dropout.py` & `Ais-cryoET-1.0.24/Ais/models/unet_dropout.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/models/unet_lite.py` & `Ais-cryoET-1.0.24/Ais/models/unet_lite.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/models/vggnet.py` & `Ais-cryoET-1.0.24/Ais/models/vggnet.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/models/vggnet_plus.py` & `Ais-cryoET-1.0.24/Ais/models/vggnet_plus.py`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/shaders/se_binary_segmentation_shader.glsl` & `Ais-cryoET-1.0.24/Ais/shaders/se_binary_segmentation_shader.glsl`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/shaders/se_compute_kernel_filter.glsl` & `Ais-cryoET-1.0.24/Ais/shaders/se_compute_kernel_filter.glsl`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/shaders/se_compute_mix.glsl` & `Ais-cryoET-1.0.24/Ais/shaders/se_compute_mix.glsl`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/shaders/se_float_segmentation_shader.glsl` & `Ais-cryoET-1.0.24/Ais/shaders/se_float_segmentation_shader.glsl`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/shaders/se_icon_shader.glsl` & `Ais-cryoET-1.0.24/Ais/shaders/se_icon_shader.glsl`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/shaders/se_overlay_ray_trace_shader.glsl` & `Ais-cryoET-1.0.24/Ais/shaders/se_overlay_ray_trace_shader.glsl`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/shaders/se_overlay_shader.glsl` & `Ais-cryoET-1.0.24/Ais/shaders/se_overlay_shader.glsl`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/shaders/se_quad_3d_shader.glsl` & `Ais-cryoET-1.0.24/Ais/shaders/se_quad_3d_shader.glsl`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/shaders/se_quad_shader.glsl` & `Ais-cryoET-1.0.24/Ais/shaders/se_quad_shader.glsl`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais/shaders/se_surface_model_shader.glsl` & `Ais-cryoET-1.0.24/Ais/shaders/se_surface_model_shader.glsl`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/Ais_cryoET.egg-info/PKG-INFO` & `Ais-cryoET-1.0.24/Ais_cryoET.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Ais-cryoET
-Version: 1.0.23
+Version: 1.0.24
 Summary: Segmentation of cryo-electron tomography data - https://ais-cryoet.readthedocs.org/ https://aiscryoet.org/
 Home-page: https://github.com/bionanopatterning/Ais
 Author: mgflast
 Author-email: m.g.f.last@lumc.nl
 License: GPL v3
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `Ais-cryoET-1.0.23/Ais_cryoET.egg-info/SOURCES.txt` & `Ais-cryoET-1.0.24/Ais_cryoET.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/PKG-INFO` & `Ais-cryoET-1.0.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Ais-cryoET
-Version: 1.0.23
+Version: 1.0.24
 Summary: Segmentation of cryo-electron tomography data - https://ais-cryoet.readthedocs.org/ https://aiscryoet.org/
 Home-page: https://github.com/bionanopatterning/Ais
 Author: mgflast
 Author-email: m.g.f.last@lumc.nl
 License: GPL v3
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `Ais-cryoET-1.0.23/README.md` & `Ais-cryoET-1.0.24/README.md`

 * *Files identical despite different names*

### Comparing `Ais-cryoET-1.0.23/setup.py` & `Ais-cryoET-1.0.24/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # twine upload dist/*
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='Ais-cryoET',
-    version='1.0.23',
+    version='1.0.24',
     packages=find_packages(),
     entry_points={'console_scripts': ['ais=Ais.main:main', 'ais-cryoet=Ais.main:main']},
     url='https://github.com/bionanopatterning/Ais',
     license='GPL v3',
     author='mgflast',
     author_email='m.g.f.last@lumc.nl',
     description='Segmentation of cryo-electron tomography data - https://ais-cryoet.readthedocs.org/ https://aiscryoet.org/',
```


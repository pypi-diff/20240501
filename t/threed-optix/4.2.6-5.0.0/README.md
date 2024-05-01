# Comparing `tmp/threed_optix-4.2.6.tar.gz` & `tmp/threed_optix-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threed_optix-4.2.6.tar", last modified: Sun Mar 24 14:40:39 2024, max compression
+gzip compressed data, was "threed_optix-5.0.0.tar", last modified: Wed May  1 11:16:46 2024, max compression
```

## Comparing `threed_optix-4.2.6.tar` & `threed_optix-5.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-03-24 14:40:39.407388 threed_optix-4.2.6/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      148 2024-03-24 13:38:50.000000 threed_optix-4.2.6/.gitignore
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1064 2024-02-20 12:16:48.000000 threed_optix-4.2.6/LICENSE.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2377 2024-03-24 14:40:39.407388 threed_optix-4.2.6/PKG-INFO
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2077 2024-03-24 13:38:50.000000 threed_optix-4.2.6/README.md
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-03-24 14:40:39.397388 threed_optix-4.2.6/help/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    36113 2024-03-24 13:38:50.000000 threed_optix-4.2.6/help/SDK help text.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    39791 2024-03-24 13:50:05.000000 threed_optix-4.2.6/help/SDK help.md
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      107 2024-03-24 14:40:39.407388 threed_optix-4.2.6/setup.cfg
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1051 2024-03-24 14:40:34.000000 threed_optix-4.2.6/setup.py
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-03-24 14:40:39.397388 threed_optix-4.2.6/src/
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-03-24 14:40:39.407388 threed_optix-4.2.6/src/threed_optix/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      283 2024-03-24 14:39:51.000000 threed_optix-4.2.6/src/threed_optix/__init__.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    15030 2024-03-24 14:35:27.000000 threed_optix-4.2.6/src/threed_optix/analyses.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     4172 2024-03-24 13:38:50.000000 threed_optix-4.2.6/src/threed_optix/beams.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    21224 2024-03-24 14:36:09.000000 threed_optix-4.2.6/src/threed_optix/client.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)       29 2024-03-24 13:38:50.000000 threed_optix-4.2.6/src/threed_optix/optimize.py
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-03-24 14:40:39.407388 threed_optix-4.2.6/src/threed_optix/package_utils/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)       16 2024-03-24 13:38:50.000000 threed_optix-4.2.6/src/threed_optix/package_utils/__init__.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     8984 2024-03-24 14:38:42.000000 threed_optix-4.2.6/src/threed_optix/package_utils/api.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2256 2024-03-24 14:35:14.000000 threed_optix-4.2.6/src/threed_optix/package_utils/general.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1515 2024-03-24 13:38:50.000000 threed_optix-4.2.6/src/threed_optix/package_utils/math.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)       70 2024-03-24 13:38:50.000000 threed_optix-4.2.6/src/threed_optix/package_utils/matlab.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    10164 2024-03-24 13:38:50.000000 threed_optix-4.2.6/src/threed_optix/package_utils/vars.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    46605 2024-03-24 13:38:50.000000 threed_optix-4.2.6/src/threed_optix/parts.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)    14149 2024-03-24 14:40:19.000000 threed_optix-4.2.6/src/threed_optix/simulations.py
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     4290 2024-03-24 14:40:21.000000 threed_optix-4.2.6/src/threed_optix/utils.py
-drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-03-24 14:40:39.407388 threed_optix-4.2.6/src/threed_optix.egg-info/
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2377 2024-03-24 14:40:39.000000 threed_optix-4.2.6/src/threed_optix.egg-info/PKG-INFO
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      756 2024-03-24 14:40:39.000000 threed_optix-4.2.6/src/threed_optix.egg-info/SOURCES.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)        1 2024-03-24 14:40:39.000000 threed_optix-4.2.6/src/threed_optix.egg-info/dependency_links.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)      116 2024-03-24 14:40:39.000000 threed_optix-4.2.6/src/threed_optix.egg-info/requires.txt
--rw-r--r--   0 ereztep   (1000) ereztep   (1000)       13 2024-03-24 14:40:39.000000 threed_optix-4.2.6/src/threed_optix.egg-info/top_level.txt
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-01 11:16:46.290742 threed_optix-5.0.0/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      148 2024-03-24 13:38:50.000000 threed_optix-5.0.0/.gitignore
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1064 2024-02-20 12:16:48.000000 threed_optix-5.0.0/LICENSE.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2377 2024-05-01 11:16:46.290742 threed_optix-5.0.0/PKG-INFO
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2077 2024-03-24 13:38:50.000000 threed_optix-5.0.0/README.md
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-01 11:16:46.290742 threed_optix-5.0.0/help/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    46819 2024-05-01 11:13:46.000000 threed_optix-5.0.0/help/SDK help text.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    46929 2024-05-01 11:13:46.000000 threed_optix-5.0.0/help/SDK help.md
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      107 2024-05-01 11:16:46.290742 threed_optix-5.0.0/setup.cfg
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1242 2024-05-01 11:13:46.000000 threed_optix-5.0.0/setup.py
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-01 11:16:46.290742 threed_optix-5.0.0/src/
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-01 11:16:46.290742 threed_optix-5.0.0/src/threed_optix/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      832 2024-05-01 11:13:46.000000 threed_optix-5.0.0/src/threed_optix/__init__.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    23682 2024-05-01 11:13:46.000000 threed_optix-5.0.0/src/threed_optix/analyses.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     4172 2024-03-24 13:38:50.000000 threed_optix-5.0.0/src/threed_optix/beams.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    43188 2024-05-01 11:13:46.000000 threed_optix-5.0.0/src/threed_optix/client.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)       29 2024-03-24 13:38:50.000000 threed_optix-5.0.0/src/threed_optix/optimize.py
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-01 11:16:46.290742 threed_optix-5.0.0/src/threed_optix/package_utils/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)       16 2024-03-24 13:38:50.000000 threed_optix-5.0.0/src/threed_optix/package_utils/__init__.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    15563 2024-05-01 11:13:46.000000 threed_optix-5.0.0/src/threed_optix/package_utils/api.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     3247 2024-05-01 11:13:46.000000 threed_optix-5.0.0/src/threed_optix/package_utils/general.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     1582 2024-05-01 11:13:46.000000 threed_optix-5.0.0/src/threed_optix/package_utils/math.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)       70 2024-03-24 13:38:50.000000 threed_optix-5.0.0/src/threed_optix/package_utils/matlab.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    19082 2024-05-01 11:13:46.000000 threed_optix-5.0.0/src/threed_optix/package_utils/vars.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    59842 2024-05-01 11:13:46.000000 threed_optix-5.0.0/src/threed_optix/parts.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)    14858 2024-05-01 11:13:46.000000 threed_optix-5.0.0/src/threed_optix/simulations.py
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     4718 2024-05-01 11:13:46.000000 threed_optix-5.0.0/src/threed_optix/utils.py
+drwxr-xr-x   0 ereztep   (1000) ereztep   (1000)        0 2024-05-01 11:16:46.290742 threed_optix-5.0.0/src/threed_optix.egg-info/
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)     2377 2024-05-01 11:16:46.000000 threed_optix-5.0.0/src/threed_optix.egg-info/PKG-INFO
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      756 2024-05-01 11:16:46.000000 threed_optix-5.0.0/src/threed_optix.egg-info/SOURCES.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)        1 2024-05-01 11:16:46.000000 threed_optix-5.0.0/src/threed_optix.egg-info/dependency_links.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)      116 2024-05-01 11:16:46.000000 threed_optix-5.0.0/src/threed_optix.egg-info/requires.txt
+-rw-r--r--   0 ereztep   (1000) ereztep   (1000)       13 2024-05-01 11:16:46.000000 threed_optix-5.0.0/src/threed_optix.egg-info/top_level.txt
```

### Comparing `threed_optix-4.2.6/LICENSE.txt` & `threed_optix-5.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `threed_optix-4.2.6/PKG-INFO` & `threed_optix-5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threed_optix
-Version: 4.2.6
+Version: 5.0.0
 Home-page: https://3doptix.com
 Author: 3DOptix
 Author-email: ereztep@3doptix.com
 License: MIT
 Keywords: Optics,Optical Design,Optical Simulation,Optical Design Software,3DOptix
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `threed_optix-4.2.6/README.md` & `threed_optix-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `threed_optix-4.2.6/help/SDK help text.txt` & `threed_optix-5.0.0/help/SDK help text.txt`

 * *Files 18% similar despite different names*

```diff
@@ -54,15 +54,27 @@
 ```python
 #'setups' will be a list of your simulation setups as a `tdo.Setup` objects
 setups = client.get_setups()
 ```
 
 #### Create a `tdo.Setup`
 
-Creating a new setup is not supported at the moment, but we're working on it.
+You could create a new setup with `client.create_setup` method. The method has the following arguments:
+- `name`: str, The name of the setup.
+- `description`: str, The description of the setup.
+- `labels`: list[str], the labels of the setup. Can be anything from `tdo.SETUP_LABELS`.
+- `units`: str, 'mm' or 'inch'. Default to 'mm'.
+- `private`: bool, `True` for private setup and `False` for a public one. Default to `False`.
+
+```python
+setup = client.create_setup(name = name,
+                            description = description,
+                            labels = labels,
+                            private = True)
+```
 
 #### Find a setup:
 
 First, we need to identify the setup we want to work on:
 
 ```python
 #Examine the setups:
@@ -109,14 +121,16 @@
 `tdo.Part` are the objects that represent your setup parts in the SDK.
 You could access their information:
 
 - `part.label` is the label of the part. It is not neceseraliy unique.
 - `part.id` is the id of the setup. It is unique.
 - `part.surfaces` is a list of `tdo.Surface` objects that the part has.
 - `part.pose` is a list of 6 floats representing the part's position and rotation relative to their associated coordinate system.
+- `part.db_id` is the id of the part in our database (not in the setup). For example, two lenses in the setup can be the same database object. They will have different ids, but the same db_id.
+- `part.optical_data` in the case that the part is `tdo.Optic` part.
 
 > **Warning**
 > Setups with parts that were loaded from a CAD file are not supported fully at the moment.
 > These CAD parts will not lead to an error, but they might lead to unexpected behavior.
 
 `tdo.Detector` is the object used to represent detectors. It inherits all properties and functionalities from `tdo.Part` while also introducing specific attributes tailored for representing detectors within the SDK.
 `tdo.Detector` has the following additional information:
@@ -135,17 +149,34 @@
 - `ls.opacity`
 - `ls.color`
 - `ls.source_type`
 - And information that changes with respect to `source_type`.
 
 **You could see a full description of these objects, as well as how to modify them, later on this document**.
 
-#### Create or add a `tdo.Part`:
+#### Add a `tdo.Part`:
+To add a detector to the setup:
+```python
+detector = setup.add_detector(label = label,
+                              pose = pose)
+```
+
+To add a light source to the setup:
+```python
+ls = setup.add_light_source(label = label,
+                              pose = pose)
+```
 
-Creating a new part, light source or detector is not supported at the moment, but we're working on it.
+To add optic to the setup, we will have to find its `db_id` from the product catalog or take the number id of the created optic from `client.create_xxx` methods.
+```python
+ls = setup.add_optics(db_id = db_id,
+                            label = label,
+                            pose = pose)
+```
+You could get the part number id in the `ID` column in the product catalog, or take the number id of the part you created.
 
 #### Find a part:
 
 Almost identical to finding a setup.
 
 ```python
 #Examine the parts of the setup
@@ -183,14 +214,22 @@
     if p.id == part_id:
        part = p
        break
 
 assert part is not None, "Part was not found"
 ```
 
+#### Delete a part from the setup:
+In order to remove a part from the setup, we simply use `setup.delete_part` method as follows:
+```python
+part_to_delete = setup.get('<part_to_delete_label')
+setup.delete_part(part_to_delete)
+```
+And that's it! The part is removed from the setup.
+
 ### Surface
 
 `tdo.Surface` are the objects that represent the surfaces of the part in the SDK.
 You could access their information:
 
 - `surface.name` is the name of the surface. It is not neceseraliy unique.
 - `surface.id` is the id of the setup. It is unique.
@@ -236,40 +275,131 @@
     if s.id == surface_id:
       surface = s
       break
 
 assert surface is not None, "Surface was not found"
 ```
 
-### Analysis
+### Scattering
+Each surface of `tdo.Optic` part can have scattering properties.
+To examine them, check `surface.scattering` property.
+If the surface does not have scattering, it will return `False`.
+#### Disable Surface Scattering
+If a surface has a scattering that you want to disable, simply use `surface.disable_scatterin` method.
+```python
+surface.diasble_scattering()
+if not surface.scattering:
+    print('Success!')
+```
+#### Add Or Change Scattering
+Scattering can be added or changed with `surface.XXX_scattering` methods.
+Each of them acccepts the following arguments:
+- `transmittance`, `absorption`, `reflection`: float, The relative part of transmittance, absorption and reflection of the scattering.
+- `num_of_rays`: int,
+- `relative_power_threshold`: float,
+##### Cos-nth
+Requires also `n` parameter, which defaults to 1.5.
+```python
+surface.cos_scattering(transmittance = 0.5,
+                        reflection = 0.3,
+                        absorption = 0.1,
+                        num_of_rays = 10,
+                        relative_power_threshold = 5,
+                        n = 2)
+```
+##### Gaussian
+Requires also `sigma_x`, `sigma_y` and `azimuth_theta` parameters.
+```python
+surface.gaussian_scattering(transmittance = 0.99,
+                            reflection = 0.01,
+                            absorption = 0,
+                            num_of_rays = 5,
+                            relative_power_threshold = 2
+                            sigma_x = 10,
+                            sigma_y = 15,
+                            azimuth_theta = 0)
+```
+
+##### ABG
+Requires also `a`, `b` and `g` parameters.
+```python
+surface.abg_scattering(transmittance = 0.95,
+                            reflection = 0.025,
+                            absorption = 0.025,
+                            num_of_rays = 7,
+                            relative_power_threshold = 4
+                            a = 1,
+                            b = 2,
+                            g = 2)
+```
+
+##### Lambertian
+Does not require unique parameters.
+```python
+surface.lembertian_scattering(transmittance = 0.97,
+                            reflection = 0.03,
+                            absorption = 0.01,
+                            num_of_rays = 10,
+                            relative_power_threshold = 5,
+                            )
+```
+
+### Coordinate Systems
+#### Part Coordinate System
+You can see all of the coordinate systems that a part has in `part.cs` list.
+Every `CoordinateSystem` object has `name`, `pose`, and `id` properties.
+The local coordinate system is accesible with `part.lcs`, and the reference coordinate system is accesible with `part.rcs` (with the relevant part).
+```python
+for cs in part.cs:
+    print(cs.name, cs.id, cs.pose)
+
+lcs = part.lcs
+rcs, reference_part = part.rcs
+```
+#### The World Coordinate System
+The world coordinate system is stored in `tdo.WORLD` object. You can use it as a coordinate system.
+
+#### Change lcs and rcs
+You can change lcs and rcs with `part.change_cs` method. It accepts the following arguments:
+- `lcs`: CoordinateSystem, if defined, it will be the new local coordinate system of the part.
+- `rcs`: CoordinateSystem, if defined, it will be the new reference coordinate system of the part.
+```python
+lens.change_cs(lcs = lens.cs[1])
+detector.change_cs(rcs = lens.cs[0])
+ls.change_cs(lcs = ls.cs[0], rcs = tdo.WORLD)
+```
+
+### Materials
+#### Find Materials From Database
+Some mmethods require specific materials from our database. In order to find them, use `client.search_materials` method.
+```python
+materials = client.search_materials('N-BK7')
+```
+`materials` is now a list of `Material` object.
+```python
+for m in materials:
+    print(m.id, m.name, m.company)
+```
+Finally, you can use the chosen material object of directly in the material id.
 
+### Analysis
 `tdo.Analysis` are the objects that represent analyses that can be performed on a surface.
 They are defined by:
 
 - `id`: The unique id of the analysis.
 - `surface`: The `tdo.Surface` object on which the analysis will be made.
 - `resolution`: The analysis surface resolution, in the format of `[pixels_x, pixels_y]` (up to 1e4)
 - `rays`: A dictionary that maps how many rays to shoot from each light source (up to 1e9), in the format of `{ls_object: num_rays, ls_object: num_rays, ...}` where light source object is a `tdo.LightSource` object. The rays are distributed equally between the light source wavelengths.
-- `name`: A string represents the analysis type. Currently supported:
-  - "Spot (Incoherent Irradiance)",
-  - "Spot (Coherent Irradiance)",
-  - "Coherent Phase",
-  - "Spot (Coherent Irradiance) Huygens",
-  - "Coherent Phase Huygens",
-  - "Spot (Coherent Irradiance) Polarized",
-  - "Coherent Phase Polarized",
-  - "Spot (Incoherent Irradiance) Polarized"
+- `name`: str, one of `tdo.ANALYSIS_NAMES`.
 
 A surface can contain several analysis with identical properties and different ids.
 However, each analysis consumes your account resources, since analysis id holds its results.
 When you run the analysis again, the last result is deleted from 3DOptix systems.
 So, we reccomend storing iterations of the same analysis locally and use duplicated analyses only when you think it's necessary.
 
-You can always get a reminder of the possible analyses with `tdo.analysis_names` variable.
-
 #### Find existing analysis
 
 Every new analysis consumes storage resources for you account.
 So, we reccomend sticking to the same analysis if they have the same properties instead of creating new ones.
 You could get a list of the `tdo.Analysis` of the surface like this:
 
 ```python
@@ -315,28 +445,36 @@
                         resolution = [500, 500],
                         rays = {laser: 1e5},
                         name = "Spot (Incoherent Irradiance)"
                         )
 ```
 
 > **Reminder**
-> You can always access all the possible analysis names with `tdo.analysis_names`
+> You can always access all the possible analysis names with `tdo.ANALYSIS_NAMES`
 
 After we created an analysis, we need to add it to the surface and setup to be able to run it.
 
 ```python
 # In case the surface doesn't have analysis with this parameter
 surface.add_analysis(analysis)
 
 # In case that the surface has an analysis with these parameter, and we want to add a new one anyway
 surface.add_analysis(analysis, force = True)
 ```
 
 **If the analysis is duplicated**, you have to use `force = True` to indicate that you understand that you are adding a duplicated analysis that will use more storage.
 Otherwise, you will get an error.
+#### Delete Analysis
+You can delete analysis from the surface with `surface.delete_analysis(analysis)` method.
+This can help manage memory as well as creating more smooth workflows.
+```python
+results = setup.run(analysis)
+analysis.show()
+surface.delete_analysis(analysis)
+```
 
 ## Make Changes
 
 #### Backup
 
 Before making any changes, we reccomend storing the original part or setup, before any changes:
 
@@ -365,14 +503,15 @@
 ```
 
 #### Transformations
 
 You could move and rotate part using `part.change_pose()` method that moves the part to a location on the three axis (x, y, z) and rotates it in respect to them (alpha, beta, gamma).
 
 All six numbers indicating absolute future value in respect to the part's coordinate system, **not** change and **not** with respect to the global coordinate system.
+if you want to change coordinate systems, please check `part.change_cs` method.
 
 ```python
 #Define the rotation
 new_pose = [x, y, z, alpha, beta, gamma]
 
 #Apply on the part
 part.change_pose(new_pose)
@@ -798,23 +937,14 @@
 results = setup.run(analysis)
 ```
 
 > **Reminder**
 > If you would try to add analysis with exactly the same parameters as one that you already have, you should use **`force = True`** argument to make sure that you are interested with duplicated analysis.
 > Otherwise, choose the existing analysis and run it instead. This helps optimizing your system memory credits usage.
 
-If we want to run multiple analyses with the same command, you can do that by passing `tdo.Analysis` list:
-
-```python
-analyses = detector_front.analyses[1:4]
-results = setup.run(analyses)
-```
-
-The recieved results will be a list of results in the same order of the analyses list, so that `results[i]` is the result of analysis `analyses[i]`.
-
 #### Results
 
 Even if we didn't store it in another variable, we can view and analize the latest results in a raw form:
 
 ```python
 print(analysis.results)
 ```
@@ -861,53 +991,130 @@
 ```python
 analysis.show_interactive(upscale = True,
                           polarizations = ['Y', 'Z'],
                           wavelengths = [500, 700],
                           figsize = (20, 20))
 ```
 
-## Advanced
-
-#### Versioning
-
-We can use the backup options to create versions of the parts and setups and manage them.
-In order to do that, we give the back a name:
-
-```python
-# For part
-part.backup(name = '10z')
-# Some code
-part.restore(name = '10z')
-
-# For entire setup
-setup.backup(name = 'system phase 1')
-# Some code
-setup.restore(name = 'system phase 1')
-```
-
-The same backup name for both setup and part overrides those backups, also for individual parts inside the setup.
-
-#### Ask questions
-
-If you have any questions about the SDK, you can send them to `client.ask()` and get a response from OptiChat, our optics copilot.
-
-```python
-client.ask('How can I get the front surface of my detector object?')
-```
-
-```python
-client.ask('How can I define a uniform distribution between 500 nm and 600 nm to my light source?')
-```
+## Create a new `tdo.Optics` in your product catalog
+As for now, the SDK supports creating spherical and conic lenses.
+### Create Lenses
+#### Spherical Lenses
+To create spherical lens, we can use `client.create_spherical_lens` method. The arguments are:
+- `name`: str, the name of the created lens.
+- `material`: Union[str, tdo.Material], the desired material id or material object of the lens. Can be found using `client.search_materials(material_name)` method.
+- `diameter`: float, the diameter of the lens.
+- `thickness`: float, the central thickness of the lens.
+- `r1`: float, the first radius of curvature.
+- `r2`: float, the second radius of curvature.
+
+The method returns the number id of the created element.
+```python
+lens_db_id = client.create_spherical_lens(name = name,
+                                              material = material,
+                                              diameter = diameter,
+                                              thickness = thickness,
+                                              r1 = r1,
+                                              r2 = r2)
+```
+
+#### Conic Lenses
+To create conic lens, we can use `client.create_conic_lens` method. The arguments are:
+- `name`: str, the name of the created lens.
+- `material`: Union[str, tdo.Material], the desired material id or material object of the lens. Can be found using `client.search_materials(material_name)` method.
+- `diameter`: float, the diameter of the lens.
+- `thickness`: float, the central thickness of the lens.
+- `r1`: float, the first radius of curvature.
+- `r2`: float, the second radius of curvature.
+- `k1`, `k2`: float, the conic coefficients of the lens. Default to 0.
+
+The method returns the number id of the created element.
+```python
+lens_db_id = client.create_spherical_lens(name = name,
+                                              material = material,
+                                              diameter = diameter,
+                                              thickness = thickness,
+                                              r1 = r1,
+                                              r2 = r2,
+                                              k1 = k1,
+                                              k2 = k2)
+```
+
+#### Biconic Lenses
+To create conic lens, we can use `client.create_conic_lens` method. The arguments are:
+- `name`: str, the name of the created lens.
+- `material`: Union[str, tdo.Material], the desired material id or material object of the lens. Can be found using `client.search_materials(material_name)` method.
+- `diameter`: float, the diameter of the lens.
+- `thickness`: float, the central thickness of the lens.
+- `r1_x`, `r1_y`: float, the first radius of curvature.
+- `r2_x`, `r2_y`: float, the second radius of curvature.
+- `k1_x`, `k1_y`, `k2_x`, `k2_y`: float, the conic coefficients of the lens. Default to 0.
+
+The method returns the number id of the created element.
+```python
+lens_db_id = client.create_spherical_lens(name = name,
+                                              material = material,
+                                              diameter = diameter,
+                                              thickness = thickness,
+                                              r1_x = r1_x,
+                                              r1_y = r1_y,
+                                              r2_x = r2_x,
+                                              r2_y = r2_y,
+                                              k1_x = k1_x,
+                                              k1_y = k1_y,
+                                              k2_x = k2_x,
+                                              k2_y = k2_y)
+```
+### Create Grating
+You can create a new grating in the database with `client.create_grating` method.
+It requires the following arguments:
+- `name`: str, The name of the grating in the database.
+- `material`: Union[str, tdo.Material], the desired material id or material object of the lens. Can be found using `client.search_materials(material_name)` method.
+- `grooves`: int, Number of grooves on the grating.
+- `order`: int, order of diffraction.
+- `orientation_vector`: iter, a 3 floats iterable representing the normalized orientation vector of the grooves.
+- `gating_side`: `"Front"` or `"Back"`, the surface of the grating element onto which the grating structure would apply. Default to `"Front"`
+- `thickness`: float, the thickness of the grating.
+- `shape`: 'cir' or 'rec', representing circular or rectangular grating.
+    - if `shape` is `"cir"`, then `diameter` must to be specified.
+    - if `shape` is `"rec"`, then `height`, `width` must to be specified.
+- `subtype`: str, one of `tdo.GRATING_SUBTYPES`.
+    - if `subtype` is one of `"Blazed Ruled Reflective Grating"`, `"Echelle Grating"`, `"Transmission Grating"`: `blaze_angle` and `blaze_wavelength` must also be specified.
 
+For example:
 ```python
-client.ask('Why do I need to add the `force` argument when I want to add a duplicated analysis?')
+circular_grating_id = client.create_grating(name = 'example circular grating',
+                                            material = material,
+                                            orientation_vector = [1, 0, 0],
+                                            shape = 'cir',
+                                            thickness = 3,
+                                            diameter = 5,
+                                            subtype = 'Reflective Grating',
+                                            grooves = 200,
+                                            order = 2,
+                                            )
+```
+```python
+rectangular_transmission_grating_id = client.create_grating(name = 'example circular grating',
+                                                            material = material2,
+                                                            orientation_vector = [0, 1, 0],
+                                                            shape = 'rec',
+                                                            thickness = 3,
+                                                            height = 2,
+                                                            width = 1.5,
+                                                            subtype = 'Transmission Grating',
+                                                            grooves = 200,
+                                                            order = 2,
+                                                            blaze_angle = 20,
+                                                            blaze_wavelength = 450
+                                                            )
 ```
 
+## Advanced
 ### Utils Module
-
 #### Get spot size
 
 `tdo.utils.calculate_spot_size(matrix)` calculates the diameter of the blocking circle of the biggest contours of the matrix, in pixels.
 
 ```python
 import threed_optix.utils as tu
```

### Comparing `threed_optix-4.2.6/help/SDK help.md` & `threed_optix-5.0.0/help/SDK help.md`

 * *Files 12% similar despite different names*

```diff
@@ -57,26 +57,15 @@
 ```
 
 #### Create a `tdo.Setup`
 
 You could create a new setup with `client.create_setup` method. The method has the following arguments:
 - `name`: str, The name of the setup.
 - `description`: str, The description of the setup.
-- `labels`: list[str], the labels of the setup. Can be:
-    - "General"
-    - "Microscopy"
-    - "Telescopy"
-    - "Spectroscopy"
-    - "Imaging"
-    - "Non-linear optics"
-    - "Fiber"
-    - "Illumination"
-    - "Light sources"
-    - "Laser Optics"
-    - "Diffractive Optics"
+- `labels`: list[str], the labels of the setup. Can be anything from `tdo.SETUP_LABELS`.
 - `units`: str, 'mm' or 'inch'. Default to 'mm'.
 - `private`: bool, `True` for private setup and `False` for a public one. Default to `False`.
 
 ```python
 setup = client.create_setup(name = name,
                             description = description,
                             labels = labels,
@@ -132,14 +121,16 @@
 `tdo.Part` are the objects that represent your setup parts in the SDK.
 You could access their information:
 
 - `part.label` is the label of the part. It is not neceseraliy unique.
 - `part.id` is the id of the setup. It is unique.
 - `part.surfaces` is a list of `tdo.Surface` objects that the part has.
 - `part.pose` is a list of 6 floats representing the part's position and rotation relative to their associated coordinate system.
+- `part.db_id` is the id of the part in our database (not in the setup). For example, two lenses in the setup can be the same database object. They will have different ids, but the same db_id.
+- `part.optical_data` in the case that the part is `tdo.Optic` part.
 
 > **Warning**
 > Setups with parts that were loaded from a CAD file are not supported fully at the moment.
 > These CAD parts will not lead to an error, but they might lead to unexpected behavior.
 
 `tdo.Detector` is the object used to represent detectors. It inherits all properties and functionalities from `tdo.Part` while also introducing specific attributes tailored for representing detectors within the SDK.
 `tdo.Detector` has the following additional information:
@@ -171,22 +162,25 @@
 
 To add a light source to the setup:
 ```python
 ls = setup.add_light_source(label = label,
                               pose = pose)
 ```
 
-To add optic to the setup, we will have to find its `number_id` from the product catalog or take the number id of the created optic from `client.create_xxx` methods.
+To add optic to the setup, we will have to find its `db_id` from the product catalog or take the number id of the created optic from `client.create_xxx` methods.
 ```python
-ls = setup.add_optics(number_id = number_id,
+ls = setup.add_optics(db_id = db_id,
                             label = label,
                             pose = pose)
 ```
 You could get the part number id in the `ID` column in the product catalog, or take the number id of the part you created.
 
+>> **Note**
+>> You can add parts with any keywords from part.change_config to add and change properties with the same command.
+
 #### Find a part:
 
 Almost identical to finding a setup.
 
 ```python
 #Examine the parts of the setup
 for part in setup:
@@ -284,40 +278,131 @@
     if s.id == surface_id:
       surface = s
       break
 
 assert surface is not None, "Surface was not found"
 ```
 
-### Analysis
+### Scattering
+Each surface of `tdo.Optic` part can have scattering properties.
+To examine them, check `surface.scattering` property.
+If the surface does not have scattering, it will return `False`.
+#### Disable Surface Scattering
+If a surface has a scattering that you want to disable, simply use `surface.disable_scatterin` method.
+```python
+surface.diasble_scattering()
+if not surface.scattering:
+    print('Success!')
+```
+#### Add Or Change Scattering
+Scattering can be added or changed with `surface.XXX_scattering` methods.
+Each of them acccepts the following arguments:
+- `transmittance`, `absorption`, `reflection`: float, The relative part of transmittance, absorption and reflection of the scattering.
+- `num_of_rays`: int,
+- `relative_power_threshold`: float,
+##### Cos-nth
+Requires also `n` parameter, which defaults to 1.5.
+```python
+surface.cos_scattering(transmittance = 0.5,
+                        reflection = 0.3,
+                        absorption = 0.1,
+                        num_of_rays = 10,
+                        relative_power_threshold = 5,
+                        n = 2)
+```
+##### Gaussian
+Requires also `sigma_x`, `sigma_y` and `azimuth_theta` parameters.
+```python
+surface.gaussian_scattering(transmittance = 0.99,
+                            reflection = 0.01,
+                            absorption = 0,
+                            num_of_rays = 5,
+                            relative_power_threshold = 2
+                            sigma_x = 10,
+                            sigma_y = 15,
+                            azimuth_theta = 0)
+```
+
+##### ABG
+Requires also `a`, `b` and `g` parameters.
+```python
+surface.abg_scattering(transmittance = 0.95,
+                            reflection = 0.025,
+                            absorption = 0.025,
+                            num_of_rays = 7,
+                            relative_power_threshold = 4
+                            a = 1,
+                            b = 2,
+                            g = 2)
+```
+
+##### Lambertian
+Does not require unique parameters.
+```python
+surface.lembertian_scattering(transmittance = 0.97,
+                            reflection = 0.03,
+                            absorption = 0.01,
+                            num_of_rays = 10,
+                            relative_power_threshold = 5,
+                            )
+```
+
+### Coordinate Systems
+#### Part Coordinate System
+You can see all of the coordinate systems that a part has in `part.cs` list.
+Every `CoordinateSystem` object has `name`, `pose`, and `id` properties.
+The local coordinate system is accesible with `part.lcs`, and the reference coordinate system is accesible with `part.rcs` (with the relevant part).
+```python
+for cs in part.cs:
+    print(cs.name, cs.id, cs.pose)
+
+lcs = part.lcs
+rcs, reference_part = part.rcs
+```
+#### The World Coordinate System
+The world coordinate system is stored in `tdo.WORLD` object. You can use it as a coordinate system.
+
+#### Change lcs and rcs
+You can change lcs and rcs with `part.change_cs` method. It accepts the following arguments:
+- `lcs`: CoordinateSystem, if defined, it will be the new local coordinate system of the part.
+- `rcs`: CoordinateSystem, if defined, it will be the new reference coordinate system of the part.
+```python
+lens.change_cs(lcs = lens.cs[1])
+detector.change_cs(rcs = lens.cs[0])
+ls.change_cs(lcs = ls.cs[0], rcs = tdo.WORLD)
+```
+
+### Materials
+#### Find Materials From Database
+Some mmethods require specific materials from our database. In order to find them, use `client.search_materials` method.
+```python
+materials = client.search_materials('N-BK7')
+```
+`materials` is now a list of `Material` object.
+```python
+for m in materials:
+    m.describe()
+```
+Finally, you can use the chosen material object or directly in the material id.
 
+### Analysis
 `tdo.Analysis` are the objects that represent analyses that can be performed on a surface.
 They are defined by:
 
 - `id`: The unique id of the analysis.
 - `surface`: The `tdo.Surface` object on which the analysis will be made.
 - `resolution`: The analysis surface resolution, in the format of `[pixels_x, pixels_y]` (up to 1e4)
 - `rays`: A dictionary that maps how many rays to shoot from each light source (up to 1e9), in the format of `{ls_object: num_rays, ls_object: num_rays, ...}` where light source object is a `tdo.LightSource` object. The rays are distributed equally between the light source wavelengths.
-- `name`: A string represents the analysis type. Currently supported:
-  - "Spot (Incoherent Irradiance)",
-  - "Spot (Coherent Irradiance)",
-  - "Coherent Phase",
-  - "Spot (Coherent Irradiance) Huygens",
-  - "Coherent Phase Huygens",
-  - "Spot (Coherent Irradiance) Polarized",
-  - "Coherent Phase Polarized",
-  - "Spot (Incoherent Irradiance) Polarized"
+- `name`: str, one of `tdo.ANALYSIS_NAMES`.
 
 A surface can contain several analysis with identical properties and different ids.
 However, each analysis consumes your account resources, since analysis id holds its results.
 When you run the analysis again, the last result is deleted from 3DOptix systems.
 So, we reccomend storing iterations of the same analysis locally and use duplicated analyses only when you think it's necessary.
 
-You can always get a reminder of the possible analyses with `tdo.analysis_names` variable.
-
 #### Find existing analysis
 
 Every new analysis consumes storage resources for you account.
 So, we reccomend sticking to the same analysis if they have the same properties instead of creating new ones.
 You could get a list of the `tdo.Analysis` of the surface like this:
 
 ```python
@@ -363,28 +448,36 @@
                         resolution = [500, 500],
                         rays = {laser: 1e5},
                         name = "Spot (Incoherent Irradiance)"
                         )
 ```
 
 > **Reminder**
-> You can always access all the possible analysis names with `tdo.analysis_names`
+> You can always access all the possible analysis names with `tdo.ANALYSIS_NAMES`
 
 After we created an analysis, we need to add it to the surface and setup to be able to run it.
 
 ```python
 # In case the surface doesn't have analysis with this parameter
 surface.add_analysis(analysis)
 
 # In case that the surface has an analysis with these parameter, and we want to add a new one anyway
 surface.add_analysis(analysis, force = True)
 ```
 
 **If the analysis is duplicated**, you have to use `force = True` to indicate that you understand that you are adding a duplicated analysis that will use more storage.
 Otherwise, you will get an error.
+#### Delete Analysis
+You can delete analysis from the surface with `surface.delete_analysis(analysis)` method.
+This can help manage memory as well as creating more smooth workflows.
+```python
+results = setup.run(analysis)
+analysis.show()
+surface.delete_analysis(analysis)
+```
 
 ## Make Changes
 
 #### Backup
 
 Before making any changes, we reccomend storing the original part or setup, before any changes:
 
@@ -413,14 +506,15 @@
 ```
 
 #### Transformations
 
 You could move and rotate part using `part.change_pose()` method that moves the part to a location on the three axis (x, y, z) and rotates it in respect to them (alpha, beta, gamma).
 
 All six numbers indicating absolute future value in respect to the part's coordinate system, **not** change and **not** with respect to the global coordinate system.
+if you want to change coordinate systems, please check `part.change_cs` method.
 
 ```python
 #Define the rotation
 new_pose = [x, y, z, alpha, beta, gamma]
 
 #Apply on the part
 part.change_pose(new_pose)
@@ -906,92 +1000,124 @@
 
 ## Create a new `tdo.Optics` in your product catalog
 As for now, the SDK supports creating spherical and conic lenses.
 ### Create Lenses
 #### Spherical Lenses
 To create spherical lens, we can use `client.create_spherical_lens` method. The arguments are:
 - `name`: str, the name of the created lens.
-- `material`: str, the desired material id of the lens. Can be fetched from name and company with `client.get_material_id` method (**Which is not released yet**).
+- `material`: Union[str, tdo.Material], the desired material id or material object of the lens. Can be found using `client.search_materials(material_name)` method.
 - `diameter`: float, the diameter of the lens.
 - `thickness`: float, the central thickness of the lens.
 - `r1`: float, the first radius of curvature.
 - `r2`: float, the second radius of curvature.
 
 The method returns the number id of the created element.
 ```python
-lens_number_id = client.create_spherical_lens(name = name,
+lens_db_id = client.create_spherical_lens(name = name,
                                               material = material,
                                               diameter = diameter,
                                               thickness = thickness,
                                               r1 = r1,
                                               r2 = r2)
 ```
 
 #### Conic Lenses
 To create conic lens, we can use `client.create_conic_lens` method. The arguments are:
 - `name`: str, the name of the created lens.
-- `material`: str, the desired material id of the lens. Can be fetched from name and company with `client.get_material_id` method (**Which is not released yet**).
+- `material`: Union[str, tdo.Material], the desired material id or material object of the lens. Can be found using `client.search_materials(material_name)` method.
+- `diameter`: float, the diameter of the lens.
+- `thickness`: float, the central thickness of the lens.
+- `r1`: float, the first radius of curvature.
+- `r2`: float, the second radius of curvature.
+- `k1`, `k2`: float, the conic coefficients of the lens. Default to 0.
+
+The method returns the number id of the created element.
+```python
+lens_db_id = client.create_spherical_lens(name = name,
+                                              material = material,
+                                              diameter = diameter,
+                                              thickness = thickness,
+                                              r1 = r1,
+                                              r2 = r2,
+                                              k1 = k1,
+                                              k2 = k2)
+```
+
+#### Biconic Lenses
+To create conic lens, we can use `client.create_conic_lens` method. The arguments are:
+- `name`: str, the name of the created lens.
+- `material`: Union[str, tdo.Material], the desired material id or material object of the lens. Can be found using `client.search_materials(material_name)` method.
 - `diameter`: float, the diameter of the lens.
 - `thickness`: float, the central thickness of the lens.
 - `r1_x`, `r1_y`: float, the first radius of curvature.
 - `r2_x`, `r2_y`: float, the second radius of curvature.
 - `k1_x`, `k1_y`, `k2_x`, `k2_y`: float, the conic coefficients of the lens. Default to 0.
 
 The method returns the number id of the created element.
 ```python
-lens_number_id = client.create_spherical_lens(name = name,
+lens_db_id = client.create_spherical_lens(name = name,
                                               material = material,
                                               diameter = diameter,
                                               thickness = thickness,
                                               r1_x = r1_x,
                                               r1_y = r1_y,
                                               r2_x = r2_x,
                                               r2_y = r2_y,
                                               k1_x = k1_x,
+                                              k1_y = k1_y,
+                                              k2_x = k2_x,
                                               k2_y = k2_y)
 ```
+### Create Grating
+You can create a new grating in the database with `client.create_grating` method.
+It requires the following arguments:
+- `name`: str, The name of the grating in the database.
+- `material`: Union[str, tdo.Material], the desired material id or material object of the lens. Can be found using `client.search_materials(material_name)` method.
+- `grooves`: int, Number of grooves on the grating.
+- `order`: int, order of diffraction.
+- `orientation_vector`: iter, a 3 floats iterable representing the normalized orientation vector of the grooves.
+- `gating_side`: `"Front"` or `"Back"`, the surface of the grating element onto which the grating structure would apply. Default to `"Front"`
+- `thickness`: float, the thickness of the grating.
+- `shape`: 'cir' or 'rec', representing circular or rectangular grating.
+    - if `shape` is `"cir"`, then `diameter` must to be specified.
+    - if `shape` is `"rec"`, then `height`, `width` must to be specified.
+- `subtype`: str, one of `tdo.GRATING_SUBTYPES`.
+    - if `subtype` is one of `"Blazed Ruled Reflective Grating"`, `"Echelle Grating"`, `"Transmission Grating"`: `blaze_angle` and `blaze_wavelength` must also be specified.
 
-## Advanced
-#### Versioning
-
-We can use the backup options to create versions of the parts and setups and manage them.
-In order to do that, we give the back a name:
-
-```python
-# For part
-part.backup(name = '10z')
-# Some code
-part.restore(name = '10z')
-
-# For entire setup
-setup.backup(name = 'system phase 1')
-# Some code
-setup.restore(name = 'system phase 1')
-```
-
-The same backup name for both setup and part overrides those backups, also for individual parts inside the setup.
-
-#### Ask questions
-
-If you have any questions about the SDK, you can send them to `client.ask()` and get a response from OptiChat, our optics copilot.
-
-```python
-client.ask('How can I get the front surface of my detector object?')
-```
-
-```python
-client.ask('How can I define a uniform distribution between 500 nm and 600 nm to my light source?')
-```
-
+For example:
 ```python
-client.ask('Why do I need to add the `force` argument when I want to add a duplicated analysis?')
+circular_grating_id = client.create_grating(name = 'example circular grating',
+                                            material = material,
+                                            orientation_vector = [1, 0, 0],
+                                            shape = 'cir',
+                                            thickness = 3,
+                                            diameter = 5,
+                                            subtype = 'Reflective Grating',
+                                            grooves = 200,
+                                            order = 2,
+                                            )
+```
+```python
+rectangular_transmission_grating_id = client.create_grating(name = 'example circular grating',
+                                                            material = material2,
+                                                            orientation_vector = [0, 1, 0],
+                                                            shape = 'rec',
+                                                            thickness = 3,
+                                                            height = 2,
+                                                            width = 1.5,
+                                                            subtype = 'Transmission Grating',
+                                                            grooves = 200,
+                                                            order = 2,
+                                                            blaze_angle = 20,
+                                                            blaze_wavelength = 450
+                                                            )
 ```
 
+## Advanced
 ### Utils Module
-
 #### Get spot size
 
 `tdo.utils.calculate_spot_size(matrix)` calculates the diameter of the blocking circle of the biggest contours of the matrix, in pixels.
 
 ```python
 import threed_optix.utils as tu
```

### Comparing `threed_optix-4.2.6/setup.py` & `threed_optix-5.0.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 from setuptools import setup, find_packages
 from setuptools.command.develop import develop
 from setuptools.command.install import install
 import subprocess
 import os
 
-
 with open('README.md') as f:
     long_description = f.read()
 
+with open('src/threed_optix/package_utils/vars.py', 'r') as f:
+    for line in f:
+        if 'VERSION' in line:
+            version = line.split('=')[1].strip().strip('"')
+            break
+
+
 setup(
     name='threed_optix',
-    version='4.2.6',
+    version=version,
     license='MIT',
     author="3DOptix",
     author_email='ereztep@3doptix.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages('src'),
     package_dir={'': 'src'},
```

### Comparing `threed_optix-4.2.6/src/threed_optix/analyses.py` & `threed_optix-5.0.0/src/threed_optix/package_utils/api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,415 +1,517 @@
-import zipfile
 import requests
-import random
+from colorama import init, Fore, Style
 import time
 import json
-import copy
-import os
-from typing import List, Dict, Union, Tuple
-import pandas as pd
-import io
-import struct
-
-import pandas as pd
-import plotly.express as px
+import math
 import numpy as np
-from io import BytesIO
+from threed_optix.package_utils import vars as v
+import pandas as pd
+import threed_optix.package_utils.math as mu
+import copy
 
-import matplotlib.pyplot as plt
-from matplotlib.colors import LinearSegmentedColormap
-from plotly.graph_objs.layout import Colorscale
-
-import threed_optix.package_utils.api as au
-import threed_optix.package_utils.general as gu
-import threed_optix.package_utils.vars as v
-
-class RayTable(pd.DataFrame):
-
-    def __init__(self, ray_table_url, maps_url, setup_object):
-        df = au._map_ray_table(ray_table_url, maps_url)
-        super().__init__(df)
-        self.attrs['setup'] = setup_object
-        return None
-
-    @property
-    def setup(self):
-        return self.attrs['setup']
-
-class Analysis:
-
-    def __init__(self,
-                 surface,
-                 resolution: Union[Tuple[int, int], List[int]],
-                 rays: Union[dict, int],
-                 name: str,
-                 fast: bool=False):
-        """
-        Initializes a new instance of the Analysis class.
-
-        Args:
-            surface (Surface): The surface of the analysis.
-            resolution (tuple): The resolution of the analysis surface in the form (x, y).
-            rays (dict): A dictionary of lasers and the number of rays for each laser.
-            name (str): The name of the analysis.
-            fast (bool, optional): Specifies if the analysis is fast or advanced. Defaults to False.
-
-        Returns:
-            tdo.Analysis: The created Analysis object.
-
-        Raises:
-            AssertionError: If the name or rays are not valid for 'fast' choice.
-        """
-
-        def verify(fast, name, rays, surface):
-            '''
-            Private.
-            '''
-
-            if surface.__class__.__name__ != 'Surface':
-                raise TypeError(f'surface must be of type Surface, got {surface.__class__.__name__}')
-
-            errors = []
-
-            if fast:
-                #Check if the name of the analysis is valid for fast analysis
-                if not name in v.FAST_ANALYSIS_NAMES:
-                    errors.append(f"Valid names for fast analysis are {v.FAST_ANALYSIS_NAMES}")
-                if not all([num <= 200 for num in rays]):
-                    errors.append(f'Number of rays must be less than 200 for fast analysis')
-            else:
-                #Check if the name of the analysis is valid for advanced analysis
-                if not name in v.ANALYSIS_NAMES:
-                    errors.append(f"Valid names for advanced analysis are {v.ANALYSIS_NAMES}")
-
-            #res is 2 floats tuple
-            if len(resolution) != 2:
-                errors.append(f'Resolution must be a tuple of 2 integers, got len {len(resolution)}')
-
-            #Res in range
-            if not all([v.ANALYSIS_RES_RANGE[0] < num <= v.ANALYSIS_RES_RANGE[1] for num in resolution]):
-                errors.append(f'Resolution must be between {v.ANALYSIS_RES_RANGE[0]} and {v.ANALYSIS_RES_RANGE[1]} for analysis')
-
-            # Rays in range
-            if not all([v.ANALYSIS_RAYS_RANGE[0] <= num <= v.ANALYSIS_RAYS_RANGE[1] for num in rays.values()]):
-                errors.append(f'Number of rays must be between {v.ANALYSIS_RAYS_RANGE[0]} and {v.ANALYSIS_RAYS_RANGE[1]} for analysis')
-
-            # Rays values are integers
-            # Trust me, Don't check for ints, because 1e8 is a float, for example
-            if not all([int(num) == num for num in rays.values()]):
-                errors.append(f'Number of rays must be an integer')
-
-            # Rays keys are LightSource
-            if not all([key.__class__.__name__ == 'LightSource' for key in rays.keys()]):
-                errors.append(f'Keys of rays must be of type LightSource')
-
-            if isinstance(rays, dict):
-                if not all([laser in rays for laser in surface._part._setup.light_sources]):
-                    errors.append(f'If rays is a dict, all lasers in the setup must be included in the rays dictionary')
-            return errors
-
-
-        if isinstance(rays, float):
-            rays = {laser: rays for laser in surface._part._setup.light_sources}
-
-        errors = verify(fast=fast, name=name, rays=rays, surface = surface)
-        if errors:
-            raise AssertionError(v.argument_repair_message(errors))
-
-
-        self._added = False
-        self._urls = []
-        self._fail_message = None
-        self._raw_results = {}
-        self.results = {}
-        self.surface = surface
-        self.name = name
-        self.rays = rays
-        self.resolution = resolution
-        self.id = Analysis._generate_id()
-        self.fast = fast
-
-
-    @classmethod
-    def _new(cls, surface, resolution, num_rays, name, type, id):
-        '''
-        Private.
-        Past analysis are stored within the setup.
-        When the setup is fetched, the past analysis are created using this method.
-        '''
-
-        analysis = object.__new__(cls)
-        analysis.surface = surface
-        analysis.resolution = list(resolution.values())
-        analysis.rays = {surface._part._setup[laser_id]: num for laser_id, num in num_rays.items()}
-        analysis.name = name
-        analysis.fast = False if type == '1' else True
-        analysis.id = id
-        analysis._added = True
-        analysis._urls = []
-        analysis._fail_message = None
-        analysis._raw_results = {}
-        analysis.results = {}
-
-        return analysis
-
-    @property
-    def wls(self):
-        '''
-        Returns a sorted list of the analysis wavelengths.
-        '''
-        return self._analysis_wls()
-
-    @classmethod
-    def _generate_id(cls):
-        '''
-        Private
-        Generates a unique id for the analysis.
-        '''
-        int_time = int(time.time())
-        enc_36_time = np.base_repr(int_time, 36)
-        randint = np.base_repr(random.randint(0, 36**5), 36)[2:5]
-        id_ = enc_36_time + randint
-        return id_
-
-    def _analysis_wls(self):
-        '''
-        Private.
-        Returns a sorted list of the wavelengths of the analysis
-        '''
-        analysis_wls = []
-        setup = self.surface._part._setup
-        laser_objects = [setup[laser.id] for laser in self.rays.keys()]
-        for laser in laser_objects:
-            wls_dicts = laser.data['light_source']['wavelengths_data']
-            wls = [wls_dict['wavelength'] for wls_dict in wls_dicts]
-            analysis_wls += wls
-        analysis_wls = sorted(list(set(analysis_wls)))
-        return analysis_wls
-
-    def _extract_file(self,url, destination):
-        ''''
-        Private.
-        Extracts a zip file from a url to a destination folder
-        '''
-        response = requests.get(url)
-        if response.status_code == 200:
-            zip_data = BytesIO(response.content)
-            with zipfile.ZipFile(zip_data, 'r') as zip_ref:
-                zip_ref.extractall(destination)
-
-        file_name = url.split('/')[-1].replace(f'{self.id}_', '').replace('.zip', '')
-        file_path = f'{destination}/{file_name}'
-        return file_path
-
-    def _unpack(self):
-        '''
-        Private.
-        Unpacks the results of the analysis to a folder
-        '''
-        setup = self.surface._part._setup.id
-        destination_path = f'.analysis-files/{setup}/{self.surface.id}/{self.id}'
-        if not os.path.exists(destination_path):
-            os.makedirs(destination_path)
-        for url in self._urls:
-            self._extract_file(url, destination_path)
-
-        return destination_path
-
-    def _read_file(self, file_path):
-        '''
-        Private.
-        Reads the results of the analysis from a file
-        '''
-        # with open(file_path, 'rb') as f:
-        #     content = f.read()
-
-        with open(file_path, 'rb') as f:
-            content = f.read().strip()
-
-
-        header = np.frombuffer(content[:v.HEADER_BYTES], dtype=v.ANALYSIS_HEADER_DTYPES)
-        data = np.frombuffer(content[v.HEADER_BYTES:], dtype=v.ANALYSIS_MATRIX_DTYPES)
-        return header, data
-
-    def _process_results(self):
-        '''
-        Private.
-        Processes the results of the analysis
-        '''
-        directory = self._unpack()
-        for file in os.listdir(directory):
-            file_results = {}
-            file_path = f'{directory}/{file}'
-            headers_nums, data = self._read_file(file_path)
-            headers = gu.process_headers(headers_nums)
-            file_results['metadata'] = headers
-
-            if headers['data_kind'] not in v.SUPPORTED_DATA_KINDS_NAMES:
-                continue
-            if data.shape[0] != len(self.wls)*self.resolution[0]*self.resolution[1]:
-                continue
-            data_matrices = data.reshape(len(self.wls), self.resolution[0], self.resolution[1])
-            file_results['data'] = {}
-            for i, wl in enumerate(self.wls):
-                matrix = data_matrices[i]
-                file_results['data'][wl] = matrix
-            file_name = file.split('.')[0]
-            self._raw_results[file_name] = file_results
-
-            polarized_dict = gu.reorganize_analysis_results_dict(self._raw_results.values())
-        self.results = polarized_dict
-        #delete directory and all subdirectories
-        os.system(f'rm -rf {directory}')
-        return self.results
-
-    def __str__(self):
-        json_dict = {
-            "id": self.id,
-            "name": self.name,
-            "surface": self.surface.id,
-            "rays": {laser.id: num for laser, num in self.rays.items()},
-            "resolution": tuple(self.resolution),
-        }
-        string = json.dumps(json_dict, indent=4)
-        return string
-
-    def __eq__(self, other):
-        '''
-        Equal analyses are analyses with the same parameters of rays, name, resolution and surface.
-        '''
-        if not isinstance(other, Analysis):
-            return False
-
-        is_rays_equal = self.rays == other.rays
-        is_name_equal = self.name == other.name
-        is_resolution_x_equal = self.resolution[0] == other.resolution[0]
-        is_resolution_y_equal = self.resolution[1] == other.resolution[1]
-        is_surface_equal = self.surface.id == other.surface.id
-
-        if is_rays_equal and is_name_equal and is_surface_equal and is_resolution_x_equal and is_resolution_y_equal:
-            return True
-
-        return False
-
-    @property
-    def data(self):
-        return self.results
-
-    def show(self, polarizations: list = None, wavelengths: list = None, figsize: Tuple[int, int] = (20, 20), upscale: bool = False):
-        '''
-        Shows a static figure of the analysis results.
-        Args:
-            figsize (tuple): The size of the figure.
-            upscale (bool): If True, smoothes the pixels over, if the analysis resolution is lower than the figure resolution.
-
-        Returns:
-            None
-
-        Shows:
-            A figure of the analysis results.
-
-        Raises:
-            Exception: If the analysis was not run yet.
-        '''
-        #3DOptix color scale
-        cmap = LinearSegmentedColormap.from_list('custom', v.COLOR_SCALE)
-
-        if not self.results:
-            raise Exception('Analysis was not run yet')
-
-        if not polarizations:
-            one_wl_data = list(self.results.values())[0]
-            polarizations = list(one_wl_data.keys())
-        if not wavelengths:
-            wavelengths = list(self.results.keys())
-
-        #Check if the analysis was run
-        if not self.results:
-            raise Exception('Analysis was not run yet')
-
-        #Get the number of polarizations and wavelengths of the analysis- polarizations are the rows and wavelengths are the columns of the presented figure
-        num_polarizations = len(self.results)
-        num_wavelengths = len(self.wls)
-        fig = plt.figure(constrained_layout=True, figsize=figsize)
-        subfigs = fig.subfigures(nrows=num_polarizations, ncols=1)
-
-        if num_polarizations == 1:
-            subfigs = [subfigs]
-
-        for polarization, subfig in zip(polarizations, subfigs):
-
-            subfig.suptitle(f'Polarization {polarization}')
-            axs = subfig.subplots(nrows=1, ncols=num_wavelengths)
-
-            if num_wavelengths == 1:
-                axs = [axs]
-
-            for wavelength, ax in zip(wavelengths, axs):
-                data = self.results[wavelength][polarization]
-                if upscale:
-                    dpi = plt.rcParams['figure.dpi']
-                    data = gu.upscale(data, figsize[0]*dpi, figsize[1]*dpi)
-                ax.imshow(data, cmap=cmap)
-
-                ax.set_title(f'Wavelength {wavelength} nm')
-
-        #Show the figure
-        plt.show()
-        return None
-
-    def show_interactive(self, polarizations: list = None, wavelengths: list = None, figsize: Tuple[int, int] = (20, 20), upscale: bool = False):
-        '''
-        Shows an interactive figure of the analysis results.
-        Args:
-            polarizations (list): The polarizations to present. If None, all polarizations are presented.
-            wavelengths (list): The wavelengths to present. If None, all wavelengths are presented.
-            height (int): The height of the each figure.
-            width (int): The width of each figure.
-            upscale (bool): If True, smoothes the pixels over, if the analysis resolution is lower than the figure resolution.
-        Returns:
-            None
-
-        Shows:
-            An interactive figure of the analysis results.
-
-        Raises:
-            Exception: If the analysis was not run yet.
-        '''
-        dpi = plt.rcParams['figure.dpi']
-        height = figsize[0]*dpi
-        width = figsize[1]*dpi
-
-        if not self.results:
-            raise Exception('Analysis was not run yet')
-
-        if not polarizations:
-            one_wl_data = list(self.results.values())[0]
-            polarizations = list(one_wl_data.keys())
-        if not wavelengths:
-            wavelengths = list(self.results.keys())
-
-        for polarization in polarizations:
-            for wavelength in wavelengths:
-                data = self.results[wavelength][polarization]
-                if upscale:
-                    data = gu.upscale(data, height, width)
-
-                fig = px.imshow(data, title=f'Polarization {polarization} Wavelength {wavelength} nm', color_continuous_scale = v.COLOR_SCALE)
-                fig.update_layout(height=height, width=width)
-                fig.show()
-
-    def copy(self):
-        '''
-        Copies the analysis to a different analysis object with a different id.
-        Returns:
-        tdo.Analysis: The copied analysis.
-        '''
-        copied = copy.deepcopy(self)
-        copied.id = Analysis._generate_id()
-        copied._added = False
-        return copied
-
-    # def __call__(self, auto_add = False, force = False):
-    #     self.surface._part._setup._api.run_analysis(self, force = force, auto_add = auto_add)
-    #     results = copy.deepcopy(self.results)
-    #     return results
+def verify_response(response):
+    '''
+    This function checkes if the response is valid.
+    '''
+
+    #If the response status code is not in the valid response codes, raise an exception.
+    if int(response.status_code) not in v.VALID_RESPONSE_CODES:
+        raise Exception(f'Error: {response.status_code} - {response.text}')
+    return None
+
+
+#General Purpose
+def _healthcheck():
+    """
+    Checks if the server is up and well.
+    """
+    url = f'{v.API_URL}/healthcheck'
+
+    r = requests.get(url)
+    verify_response(r)
+    r = r.json()
+    return (r['status'] == 'SUCCESS', r['message'])
+
+def _get(
+    endpoint: str,
+    api_key: str,
+    #payload: dict = {}
+    ):
+    """
+    Sends a GET request to the endpoint with the API key.
+
+    Args:
+        endpoint (str): The endpoint to send the request to.
+        api_key (str): The API key.
+
+    Returns:
+        tuple: The data and message from the response.
+    """
+
+    url = f'{v.API_URL}/{endpoint}'
+    headers = {'X-API-KEY': api_key,
+               'Content-Type': 'application/json',
+               "sdk-version": v.VERSION}
+
+    if v.DEBUG:
+        print(f'GET {url}')
+        print(f'Headers: {headers}')
+
+    r = requests.get(url, headers=headers)
+    verify_response(r)
+    r = r.json()
+
+    if v.DEBUG:
+        print(f'Response: {r}')
+
+    # Return the data if the status is SUCCESS, otherwise return None, and the message.
+    return (r['data'] if 'status' in r and r['status'] == 'SUCCESS' else None, r['message'])
+
+def _put(endpoint: str, api_key: str, json_data: dict = None):
+    """
+    Sends a PUT request to the endpoint.
+
+    Args:
+        endpoint (str): The endpoint to send the request to.
+        json_data (dict): The JSON payload for the request.
+        api_key (str): The API key.
+
+    Returns:
+        tuple: The data and message from the response.
+    """
+    url = f'{v.API_URL}/{endpoint}'
+    headers =  {'X-API-KEY': api_key,
+               'Content-Type': 'application/json',
+               "sdk-version": v.VERSION}
+
+    if v.DEBUG:
+        print(f'PUT {url}')
+        print(f'Headers: {headers}')
+        print(f'Payload: {json_data}')
+
+    r = requests.put(url, headers=headers, json=json_data)
+    verify_response(r)
+    r = r.json()
+
+    if v.DEBUG:
+        print(f'Response: {r}')
+
+    # Return the data if the status is SUCCESS, otherwise return None, and the message.
+    return (r['data'] if 'status' in r and r['status'] == 'SUCCESS' else None, r['message'])
+
+def _set(endpoint, data, api_key):
+    '''
+    Sends a POST request to the endpoint with the data and the API key.
+    tbh, I don't know why it's seperated from the _post function.
+
+    Args:
+        endpoint (str): The endpoint to send the request to.
+        data (dict): The data to send.
+        api_key (str): The API key.
+
+    Returns:
+        tuple: The data and message from the response.
+    '''
+    url = f'{v.API_URL}/{endpoint}'
+    headers =  {'X-API-KEY': api_key,
+               'Content-Type': 'application/json',
+               "sdk-version": v.VERSION}
+
+    if v.DEBUG:
+        print(f'SET {url}')
+        print(f'Headers: {headers}')
+        print(f'Payload: {data}')
+
+
+    r = requests.post(url, headers=headers, json=data)
+
+    verify_response(r)
+    r = r.json()
+
+    if v.DEBUG:
+        print(f'Response: {r}')
+
+    return ('status' in r and r['status'] == 'SUCCESS', r['message'])
+
+def _post(endpoint, data, api_key):
+    '''
+    Sends a POST request to the endpoint with the data and the API key.
+
+    Args:
+        endpoint (str): The endpoint to send the request to.
+        data (dict): The data to send.
+        api_key (str): The API key.
+
+    Returns:
+        tuple: The status, message, and data from the response.
+    '''
+    url = f'{v.API_URL}/{endpoint}'
+    headers =  {'X-API-KEY': api_key,
+               'Content-Type': 'application/json',
+               "sdk-version": v.VERSION}
+
+    if v.DEBUG:
+        print(f'POST {url}')
+        print(f'Headers: {headers}')
+        print(f'Payload: {data}')
+
+    r = requests.post(url, headers=headers, json=data)
+    verify_response(r)
+    r = r.json()
+
+    if v.DEBUG:
+        print(f'Response: {r}')
+
+    return ('status' in r and r['status'] == 'SUCCESS', r['message'], r.get('data', None))
+
+def _delete(endpoint, api_key):
+    '''
+    Sends a DELETE request to the endpoint with the API key.
+
+    Args:
+        endpoint (str): The endpoint to send the request to.
+        api_key (str): The API key.
+
+    Returns:
+        tuple: The status and message from the response.
+    '''
+    url = f'{v.API_URL}/{endpoint}'
+    headers =  {'X-API-KEY': api_key,
+               'Content-Type': 'application/json',
+               "sdk-version": v.VERSION}
+
+    if v.DEBUG:
+        print(f'DELETE {url}')
+        print(f'Headers: {headers}')
+
+    r = requests.delete(url, headers=headers)
+    verify_response(r)
+    r = r.json()
+
+    if v.DEBUG:
+        print(f'Response: {r}')
+
+    return ('status' in r and r['status'] == 'SUCCESS', r['message'])
+
+def _create_setup(parameters, api_key):
+    '''
+    This function accesses the API create setup endpoint.
+    '''
+    endpoint = v.POST_CREATE_SETUP_ENDPOINT
+    response = _post(endpoint, parameters, api_key)
+    if not response[0]:
+        raise Exception(response[1])
+    return response[2]
+
+def _delete_part(setup_id, part_id, api_key):
+    '''
+    This function accesses the API delete part endpoint.
+    '''
+    endpoint = v.DELETE_PART_ENDPOINT.format(setup_id=setup_id, part_id=part_id)
+    return _delete(endpoint, api_key)
+
+def _add_part(setup_id, data, api_key):
+    '''
+    This function accesses the API add part endpoint.
+    '''
+    endpoint = v.POST_ADD_PART_ENDPOINT.format(setup_id=setup_id)
+    response = _post(endpoint,data,api_key)
+    if not response[0]:
+        raise Exception(response[1])
+    return response[2]
+
+def _get_setups(api_key: str):
+    """
+    Returns the list of setup names and ids of the user.
+
+    Args:
+        api_key (str): The API key.
+
+    Returns:
+        list: A list of setup names and ids.
+    """
+    endpoint = v.GET_SETUPS_ENDPOINT
+    response = _get(endpoint, api_key)
+
+    return response
+
+def _get_setup(
+    setup_id: str,
+    api_key: str
+    ):
+    """
+    Returns the opt file for the specified setup id.
+
+    Args:
+        setup_id (str): The setup id.
+        api_key (str): The API key.
+
+    Returns:
+        str: The opt file content.
+    """
+
+    endpoint = v.GET_SETUP_ENDPOINT.format(setup_id=setup_id)
+
+    return _get(endpoint, api_key)
+
+def _get_surface(api_key, setup_id, surface_id, part_id):
+    '''
+    This function fetches the information of a surface.
+    '''
+    endpoint = v.Endpoints.GET_SURFACE_DATA.format(setup_id=setup_id, surface_id=surface_id, part_id=part_id)
+    return _get(endpoint, api_key)
+
+def _create_part(parameters, api_key):
+    '''
+    This function accesses the API create part endpoint.
+    '''
+    endpoint = v.POST_CREATE_OPTICS_ENDPOINT
+    response = _post(endpoint, parameters, api_key)
+    if not response[0]:
+        raise Exception(response[1])
+    return response[2]
+
+def _get_part(setup_id: str, part_id: str, api_key: str):
+    '''
+    This function fetches the information of a part.
+    '''
+    endpoint = v.GET_PART_ENDPOINT.format(setup_id=setup_id, part_id=part_id)
+    part =  _get(endpoint, api_key)
+    return part
+
+def _change_part(setup_id, part_id, data, api_key):
+    '''
+    This function accesses the API change part endpoint.
+    '''
+
+    # Copy the data to avoid changing the original data.
+    data_copy = copy.deepcopy(data)
+
+    # Convert the rotation to radians.
+    if data.get('pose'):
+        data_copy['pose']['rotation'] =[mu.deg_to_rad(x) for x in data_copy['pose']['rotation']]
+    endpoint = v.PUT_PART_ENDPOINT.format(setup_id=setup_id, part_id=part_id)
+    r = _put(endpoint=endpoint, api_key=api_key, json_data=data_copy)
+    return r
+
+def _delete_analysis(setup_id, part_id, surface_id,analysis_id, api_key):
+    '''
+    This function accesses the API delete analysis endpoint.
+    '''
+    endpoint = v.Endpoints.DELETE_ANALYSIS.format(setup_id=setup_id,
+                                                 part_id=part_id,
+                                                 analysis_id=analysis_id,
+                                                 surface_id = surface_id)
+    return _delete(endpoint, api_key)
+
+def _run_async(setup_id, api_key):
+    '''
+    Not suppoerted anymore.
+    '''
+    endpoint =  v.PUT_SIMULATION_ENDPOINT.format(setup_id=setup_id)
+    json_data = {
+        "gpu_type": v.GPU_TYPE,
+    }
+    r = _put(endpoint = endpoint, json_data=json_data, api_key= api_key)
+    return r
+
+def _run_batch(
+    setup_id: str,
+    configuration: dict,
+    api_key: str):
+    """
+    Not supported anymore.
+    Puts the batch run request.
+
+    Args:
+        setup_id (str): The setup id.
+        configuration (dict): The batch configuration.
+        api_key (str): The API key.
+    """
+    endpoint = v.PUT_BATCH_CHANGES_ENDPOINT.format(setup_id=setup_id)
+    return _put(endpoint = endpoint, api_key= api_key, json_data = configuration)
+
+def _run_simulation(setup_id, api_key, is_sync = True):
+    '''
+    This function accesses the API run simulation endpoint for propagation.
+    '''
+    endpoint =  v.PUT_SIMULATION_ENDPOINT.format(setup_id=setup_id)
+    json_data = {
+        "gpu_type": v.GPU_TYPE,
+        "is_sync": is_sync,
+    }
+    r = _put(endpoint = endpoint, json_data=json_data, api_key= api_key)
+    return r
+
+def _add_analyses(setup_id, part_id, surface_id, data, api_key):
+    '''
+    This function accesses the API add analysis endpoint.
+    '''
+    endpoint = v.POST_ADD_ANALYSIS_ENDPOINT.format(setup_id=setup_id, part_id=part_id, surface_id = surface_id)
+    return _post(endpoint = endpoint,data=data, api_key = api_key)
+
+def _run_analysis(setup_id: str, api_key: str, analysis_id: str):
+    '''
+    This function accesses the API run simulation endpoint to run an analysis.
+    '''
+    endpoint = v.PUT_SIMULATION_ENDPOINT.format(setup_id=setup_id)
+
+    json_data = {
+        "gpu_type": v.GPU_TYPE,
+        "is_sync": True,
+        "analysis_id": analysis_id,
+    }
+
+    return _put(endpoint = endpoint, json_data = json_data, api_key = api_key)
+
+def _change_scattering(setup_id, part_id, surface_id, data, api_key):
+    '''
+    This function accesses the API change scattering endpoint.
+    '''
+    endpoint = v.Endpoints.SCATTERING.format(setup_id=setup_id, part_id=part_id, surface_id=surface_id)
+    return _put(endpoint=endpoint, api_key=api_key, json_data=data)
+
+def _get_optics_data(api_key, db_id):
+    '''
+    This function fetches the optics data.
+    '''
+    endpoint = v.Endpoints.GET_OPTICS_DATA.format(number_id=db_id)
+    return _get(endpoint, api_key)
+
+def _change_cs_data(setup_id, part_id, data, api_key):
+    '''
+    This function accesses the API change cs endpoint.
+    '''
+    endpoint = v.Endpoints.CHANGE_CS.format(setup_id=setup_id, part_id=part_id)
+    return _put(endpoint=endpoint, api_key=api_key, json_data=data)
+
+def _ask(conversation, api_key):
+    '''
+    Not implemented yet.
+    This function accesses the API ask endpoint.
+    It allows the user to ask questions to the SDK Assistant
+    '''
+    endpoint = v.GET_ANSWER_ENDPOINT
+    headers = {'X-API-KEY': api_key}
+    params = {'threed_optix_key': api_key, "conversation": json.dumps(conversation)}
+    r = requests.get(endpoint, headers=headers, params=params)
+    verify_response(r)
+    r = r.json()
+    return r['answer']
+
+def _set_api_url(url, are_you_sure=False):
+    '''
+    Private.
+    This function sets the API URL.
+    It should be used internally to switch the API URL to dev or release.
+    '''
+
+    if not are_you_sure:
+        raise Exception(v.SET_API_URL_WARNING)
+
+    print(v.SET_API_URL_WARNING)
+    print('Previous API URL was', v.API_URL)
+    print('Setting API URL to', url)
+    v.API_URL = url
+
+def _get_materials(api_key, material_name):
+    '''
+    This function fetches the materials data based on the material name.
+    '''
+    endpoint = v.Endpoints.GET_MATERIALS_ENDPOINT.format(material_name=material_name)
+    data, message = _get(endpoint, api_key)
+    if data is None:
+        raise Exception(message)
+    return data
+
+def _set_ask_url(url, are_you_sure=False):
+    '''
+    Not implemented yet.
+    This function sets the ASK URL.
+    It should be used internally to switch the ASK URL to dev or release.
+    '''
+    if not are_you_sure:
+        raise Exception(v.SET_API_URL_WARNING)
+
+    print(v.SET_API_URL_WARNING)
+    print('Previous ASK URL was', v.ASK_URL)
+    print('Setting ASK URL to', url)
+    v.ASK_URL = url
+
+def _welcome():
+    '''
+    Private.
+    This is the function that prints the welcome message, when the client object is created.
+    '''
+    init(autoreset=True)
+    color = Fore.WHITE
+    print('******************')
+    for i, char in enumerate(v.WELCOME_MESSAGE):
+        print(f"{color}{char}", end="")
+        time.sleep(0.01)  # Adjust the delay for the desired speed
+
+    print(Style.RESET_ALL)  # Reset the style after the rainbow effect
+    print('******************')
+
+def _print_getting_parts():
+    '''
+    Deprecated.
+    This function used to print a message when we fetched the parts information of the setup.
+    It is no longer needed since we are not fetching the parts information all at once anymore.
+    '''
+    init(autoreset=True)
+    color = Fore.WHITE
+    print('******************')
+    for i, char in enumerate(v.GETTING_PARTS_MESSAGE):
+        print(f"{color}{char}", end="")
+        time.sleep(0.01)  # Adjust the delay for the desired speed
+
+    print(Style.RESET_ALL)  # Reset the style after the rainbow effect
+    print('******************')
+
+def _map_ray_table(rays_url, maps_url):
+    '''
+    This function creates a pandas dataframe from the rays data and maps the indices to the actual values.
+    Args:
+        rays_url (str): The URL to the rays data, recieved from the simulation results.
+        maps_url (str): The URL to the maps data, recieved from the simulation results.
+
+    Returns:
+        pandas.DataFrame: The rays data with the indices mapped to actual values.
+    '''
+
+    # Fetch the rays data and the maps data.
+    rays_df = pd.read_csv(rays_url)
+
+    # This is probably useless, but I'm documenting when I don't have time to examine changes.
+    rays_df = rays_df.copy()
+
+    # Fetch the maps data.
+    maps_json = requests.get(maps_url).json()
+
+    # Map the indices to the actual values.
+    rays_df = rays_df.apply(lambda row: _map_ray_row(row, maps_json), axis=1)
+
+    # Set the index to the idx column.
+    rays_df.set_index('idx', inplace=True)
+    return rays_df
+
+def _map_ray_row(row, map):
+    '''
+    This is a helper function to map the indices to the actual values in the rays data per each row of the ray dataframe.
+    '''
+
+    # Map the surface from indices to the actual id.
+    row['surface'] = map['surfaces'][int(row['hit_surface_idx'])]
+
+    # Map the wavelength from indices to the actual value.
+    row['wavelength'] = map['wavelengths'][int(row['wavelength_idx'])]
+
+    # Map the light source from indices to the actual light source id.
+    row['light_source'] = map['sources'][int(row['source_idx'])]
+
+    # Drop the indices columns.
+    del row['hit_surface_idx']
+    del row['wavelength_idx']
+    del row['source_idx']
+    return row
```

### Comparing `threed_optix-4.2.6/src/threed_optix/beams.py` & `threed_optix-5.0.0/src/threed_optix/beams.py`

 * *Files identical despite different names*

### Comparing `threed_optix-4.2.6/src/threed_optix/package_utils/math.py` & `threed_optix-5.0.0/src/threed_optix/package_utils/math.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import math
 import numpy as np
 
+def is_normalized(vector):
+    return np.linalg.norm(vector) == 1
+
 def _3d_distance(a, b):
 
     a = np.array(a)
     b = np.array(b)
 
     return np.linalg.norm(a - b)
```

### Comparing `threed_optix-4.2.6/src/threed_optix/parts.py` & `threed_optix-5.0.0/src/threed_optix/parts.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,41 @@
 import threed_optix.package_utils.vars as v
 import threed_optix.beams as bm
 from typing import Union
 import copy
 import json
 import re
 
+class CoordinateSystem:
+    def __init__(self):
+        raise TypeError("Cannot directly create an instance of coordinate system.")
+
+    @classmethod
+    def _new(cls, id, _data, part):
+        cs = object.__new__(cls)
+        cs._data = _data
+        cs.id = id
+        cs._part = part
+        return cs
+
+    @property
+    def pose(self):
+        return self._data['ref_pose']['position'] + self._data['ref_pose']['rotation']
+
+    @property
+    def name(self):
+        return self._data.get('name', '')
+
+class WorldCS(CoordinateSystem):
+    @classmethod
+    def _new(cls):
+        return super()._new(id = v.CoordinateSystems.WORLD, _data = v.CoordinateSystems.WORLD_DATA, part = None)
+
+WORLD = WorldCS._new()
+
 class Surface:
     def __init__(self):
         '''
         Private
         '''
         raise TypeError("Cannot directly create an instance of Surface.")
 
@@ -19,38 +46,239 @@
         '''
         Private
         '''
         surface = object.__new__(cls)
         surface.name = _data['name']
         surface.id = _data['id']
         surface._part = _part
-        surface.analyses = [an.Analysis._new(surface = surface, **analysis) for analysis in _data['analyses']]
+        surface._analyses = None
+        surface._data = None
         return surface
 
+    @property
+    def data(self):
+        if self._data is None:
+            self._data = self._part._get_surface(surface_id = self.id).get(self.id)
+        return self._data
+
+    @property
+    def analyses(self):
+        if self._analyses is None:
+            analysis_data = self.data.get('analyses', {})
+            self._analyses = [
+                an.Analysis._new(surface = self,
+                                 id=id,
+                                 resolution=analysis['resolution'],
+                                 num_rays=analysis.get('num_rays', {laser: v.Analyses.DEFAULT_NUM_RAYS for laser in self._part._setup.light_sources}),
+                                 type = analysis['type'],
+                                 name = analysis['name'],
+                                 )
+                for id, analysis in analysis_data.items()
+                ]
+        return self._analyses
+
+
+
     def __str__(self):
         '''
         Returns a string representation of the surface: name, id, part id, and part label.
         '''
         string = f'Surface with {len(self.analyses)} analyses:\n'
         for analysis in self.analyses:
             string += f'''{analysis.name} ({analysis.id})\n'''
         return string
 
-    def find_analysis(self, name: str, rays: dict, resolution: Union[tuple, list]):
+    def find_analysis(self, name: str, rays: Union[dict, int], resolution: Union[tuple, list]):
+
+        if isinstance(rays, int):
+            rays = {ls: rays for ls in self._part._setup.light_sources}
+
         wanted_analysis = an.Analysis(surface = self, resolution = resolution, name = name, rays = rays)
         for analysis in self.analyses:
             if analysis == wanted_analysis:
                 return analysis
         return None
 
     def add_analysis(self, analysis: an.Analysis, force = False):
-        return self._part._setup._api._add_analysis(analysis, force = force)
+        data = self._part._setup._api._add_analysis(analysis, force = force)
+        analysis._added = True
+        analysis.id = data['id']
+        self.analyses.append(analysis)
+        return
+
+    def delete_analysis(self, analysis: Union[str, an.Analysis]):
+
+        analysis_id = analysis
+        if isinstance(analysis, an.Analysis):
+            analysis_id = analysis.id
+
+        if not any([(a.id == analysis_id) or (a is analysis) for a in self.analyses]):
+            raise Exception(f"Analysis with id {analysis} not found in surface.")
+
+        self._part._setup._api._delete_analysis(analysis_id = analysis_id,
+                                              setup_id = self._part._setup.id,
+                                              part_id = self._part.id,
+                                              surface_id = self.id,
+                                              )
+
+        self._analyses = [a for a in self.analyses if a.id != analysis_id]
+
+        return None
+
+class OpticSurface(Surface):
+    @classmethod
+    def _new(cls, _part, _data):
+        '''
+        Private
+        '''
+        surface = object.__new__(cls)
+        surface.name = _data['name']
+        surface.id = _data['id']
+        surface._part = _part
+        surface._analyses = None
+        surface._data = None
+        return surface
+
+    @property
+    def scattering(self):
+        return self.data['scattering'] if self.data['scattering']['enabled'] else False
+
+    def disable_scattering(self):
+        scattering = {
+            "enabled": False
+        }
+        self._part._change_scattering(surface_id = self.id, scattering = scattering)
+        self.data['scattering'] = scattering
+
+    def change_scattering(self,
+                          transmittance,
+                          reflectance,
+                          absorption,
+                          num_of_rays,
+                          relative_power_threshold,
+                          scatter_model,
+                          bsdf = None
+                          ):
+
+        parameters = {
+            "transmittance": transmittance,
+            "reflectance": reflectance,
+            "absorption": absorption,
+            "numberOfRays": num_of_rays,
+            "relativePowerThreshold": relative_power_threshold,
+            "scatterModel": scatter_model,
+        }
+
+        if bsdf is not None:
+            parameters['bsdfParams'] = bsdf
+
+        scattering_data = {
+            "parameters": parameters
+        }
+
+        scattering = {
+            "enabled": True,
+            "scatteringData": scattering_data
+        }
+        self._part._change_scattering(surface_id = self.id, scattering = scattering)
+        self.data['scattering'] = scattering
+        return None
 
-    # def __call__(self):
-    #     return {analysis: analysis() for analysis in self.analyses}
+    def lambartian_scattering(self,
+                          transmittance = v.Scattering.DEFAULT_TRANS,
+                          reflectance = v.Scattering.DEFAULT_REF,
+                          absorption = v.Scattering.DEFAULT_ABS,
+                          num_of_rays = v.Scattering.DEFAULT_NUMBER_OF,
+                          relative_power_threshold = v.Scattering.DEFAULT_RELATIVE_POWER,
+                          ):
+
+        scatter_model = v.ScatteringModels.LAMBERTIAN
+        self.change_scattering(transmittance = transmittance,
+                               reflectance = reflectance,
+                               absorption = absorption,
+                               num_of_rays = num_of_rays,
+                               relative_power_threshold = relative_power_threshold,
+                               scatter_model = scatter_model,
+                               )
+
+    def abg_scattering(self,
+                          transmittance = v.Scattering.DEFAULT_TRANS,
+                          reflectance = v.Scattering.DEFAULT_REF,
+                          absorption = v.Scattering.DEFAULT_ABS,
+                          num_of_rays = v.Scattering.DEFAULT_NUMBER_OF,
+                          relative_power_threshold = v.Scattering.DEFAULT_RELATIVE_POWER,
+                          a = v.Scattering.DEFAULT_A,
+                          b  =v.Scattering.DEFAULT_B,
+                          g = v.Scattering.DEFAULT_G
+                          ):
+
+        scatter_model = v.ScatteringModels.ABG
+        bsdf = {
+            "a": a,
+            "b": b,
+            "g": g
+        }
+        self.change_scattering(transmittance = transmittance,
+                               reflectance = reflectance,
+                               absorption = absorption,
+                               num_of_rays = num_of_rays,
+                               relative_power_threshold = relative_power_threshold,
+                               scatter_model = scatter_model,
+                               bsdf=bsdf
+                               )
+
+    def gaussian_scattering(self,
+                          transmittance = v.Scattering.DEFAULT_TRANS,
+                          reflectance = v.Scattering.DEFAULT_REF,
+                          absorption = v.Scattering.DEFAULT_ABS,
+                          num_of_rays = v.Scattering.DEFAULT_NUMBER_OF,
+                          relative_power_threshold = v.Scattering.DEFAULT_RELATIVE_POWER,
+                        sigma_x = v.Scattering.DEFAULT_SIGMAX,
+                        sigma_y = v.Scattering.DEFAULT_SIGMAY,
+                        azimuth_theta = v.Scattering.DEFAULT_AZIMUTH_THETA
+                        ):
+
+        scatter_model = v.ScatteringModels.GAUSSIAN
+        bsdf = {
+            "sigmaX": sigma_x,
+            "sigmaY": sigma_y,
+            "azimuth_theta": azimuth_theta
+            }
+
+        self.change_scattering(transmittance = transmittance,
+                               reflectance = reflectance,
+                               absorption = absorption,
+                               num_of_rays = num_of_rays,
+                               relative_power_threshold = relative_power_threshold,
+                               scatter_model = scatter_model,
+                               bsdf=bsdf
+                               )
+
+    def cos_scattering(self,
+                        transmittance = v.Scattering.DEFAULT_TRANS,
+                        reflectance = v.Scattering.DEFAULT_REF,
+                        absorption = v.Scattering.DEFAULT_ABS,
+                        num_of_rays = v.Scattering.DEFAULT_NUMBER_OF,
+                        relative_power_threshold = v.Scattering.DEFAULT_RELATIVE_POWER,
+                        n = v.Scattering.DEFAULT_N
+                        ):
+
+        scatter_model = v.ScatteringModels.COS_NTH
+        bsdf = {
+            "n": n
+            }
+
+        self.change_scattering(transmittance = transmittance,
+                               reflectance = reflectance,
+                               absorption = absorption,
+                               num_of_rays = num_of_rays,
+                               relative_power_threshold = relative_power_threshold,
+                               scatter_model = scatter_model,
+                               bsdf=bsdf
+                               )
 
 class Part:
 
     def __init__(self):
         '''
         Private
         '''
@@ -73,14 +301,17 @@
         part = object.__new__(cls)
         part._setup = _setup
         part.id = id
         part._data = _data
         part._surfaces = None
         part._changes = {}
         part._errors = []
+        part._cs = None
+        part._rcs = None
+        part._lcs = None
         part.backup_data = None
         part._user_backup = {v.BASE_BACKUP: copy.deepcopy(_data)}
         return part
 
     def __str__(self) -> str:
         '''
         Returns a string representation of the part: label, id, position, and rotation.
@@ -129,19 +360,107 @@
         '''
         if self._data is None:
             self._data = self._setup._get_part(self.id).get(self.id)
         data = self._data
         return data
 
     @property
+    def cs_data(self):
+        return self.data['cs_data']
+
+
+    @property
+    def cs(self):
+        if self._cs is None:
+            self._cs = [CoordinateSystem._new(id=id, _data=data, part=self) for id, data in self.cs_data['coordinate_systems'].items()]
+        return self._cs
+
+    @property
+    def lcs(self):
+        if self._lcs is None:
+            for cs in self.cs:
+                if cs.id == self.cs_data['lcs']:
+                    self._lcs = cs
+        return self._lcs
+
+    @property
+    def rcs(self):
+        if self._rcs is None:
+
+            if self.cs_data.get('rcs') is None:
+                self._rcs = (WORLD, None)
+
+            else:
+                for part in self._setup:
+                    for cs in part.cs:
+                        if cs.id == self.cs_data['rcs']:
+                            self._rcs = (cs, cs._part)
+                            break
+
+                    if self._rcs is not None:
+                        break
+        return self._rcs
+
+    def change_cs(self, lcs = None, rcs = None):
+        if lcs is None and rcs is None:
+            raise Exception("At least one of lcs or rcs must be specified.")
+        if lcs is None:
+            lcs = self.lcs
+        if rcs is None:
+            rcs = self.rcs[0]
+
+        if isinstance(lcs, CoordinateSystem):
+            if lcs not in self.cs:
+                raise Exception(f"lcs with id {lcs} not found in part.")
+            lcs_id = lcs.id
+        elif isinstance(lcs, str):
+            if lcs not in [cs.id for cs in self.cs]:
+                raise Exception(f"lcs with id {lcs} not found in part.")
+            lcs_id = lcs
+
+        if v.DEBUG:
+            print(f'RCS type and class: {type(rcs)} {rcs}')
+
+        if isinstance(rcs, CoordinateSystem) or isinstance(rcs, WorldCS):
+
+            ## Takes too much time, Eliav should do it (getting the cs data of each part)
+            # if rcs not in [cs for part in self._setup for cs in part.cs] or isinstance(rcs, WorldCS):
+            #     raise Exception(f"rcs with id {rcs} not found in setup.")
+
+            rcs_id = rcs.id
+        elif isinstance(rcs, str):
+
+            ## Takes too much time, Eliav should do it (getting the cs data of each part)
+            # if rcs not in [cs.id for part in self._setup for cs in part.cs] + [WORLD.id]:
+            #     raise Exception(f"rcs with id {rcs} not found in setup.")
+            rcs_id = rcs
+
+        r = self._setup._change_cs(part_id = self.id, lcs_id = lcs_id, rcs_id = rcs_id)
+
+        if r[0] is None:
+            raise Exception(r[1])
+        self._lcs = lcs
+        self._rcs = (rcs, rcs._part)
+
+        for p in self._setup:
+            if p.rcs[1] == self:
+                if v.DEBUG:
+                    print(f'Resetting part {p.id} data')
+                p._data = None
+        self._data = None
+
+
+        return None
+
+    @property
     def material(self):
         '''
         Returns the part's material.
         '''
-        return self.data['material']
+        return self._parameters['materialID']
 
     @property
     def surfaces(self):
         '''
         Returns a list of the part's surfaces as tdo.Surface objects.
         '''
         if self._surfaces is None:
@@ -156,14 +475,17 @@
     def material(self, value):
         raise AttributeError("Cannot set material directly.")
 
     @data.setter
     def data(self, value):
         raise AttributeError("Cannot set data directly.")
 
+    def _get_surface(self, surface_id):
+        return self._setup._get_surface(part_id = self.id, surface_id = surface_id)
+
     def get(self,
             name: str
             ):
         """
         Returns the surface object with the specified name.
 
         Args:
@@ -282,15 +604,15 @@
         '''
         if self._errors:
             errors = self._errors.copy()
             self.reset()
             raise Exception(v.argument_repair_message(errors))
 
         r = self._setup._update_part(self)
-        if not r[0]:
+        if r[0] is None:
             self.reset()
             raise Exception(f"Error updating part: {r[1]}")
 
         self.backup_data = None
         self.update_data(a = self._data, b = self._changes)
 
         for part in self._setup:
@@ -1153,37 +1475,97 @@
     @classmethod
     def _new(cls, _setup, id, _data):
         optics = super(cls, cls)._new(_setup, id, _data)
         optics._setup = _setup
         optics.id = id
         optics._data = _data
         optics._surfaces = None
+        optics._optical_data = None
         optics._changes = {}
         optics._errors = []
         return optics
 
+    @property
+    def surfaces(self):
+        if self._surfaces is None:
+            self._surfaces = [OpticSurface._new(self, surface)
+                              for surface in self.data.get('surfaces', [])
+                              if 'name' in surface
+                              ]
+        return self._surfaces
+
+
+    @property
+    def db_id(self):
+        return self.data.get('number_id', None)
+
+    @property
+    def optical_data(self):
+        if self._optical_data is None:
+            self._optical_data = self._setup._api.optics_data(self.db_id)
+        return self._optical_data
+
+    @property
+    def physical_data(self):
+        return self._parameters.get('physical_data', {})
+
+    @property
+    def db_name(self):
+        return self.optical_data['name']
+
+    @property
+    def _parameters(self):
+        return self.optical_data['parameters']
+
+    @property
+    def geometry(self):
+        return self._parameters['geometry']
+
+    @property
+    def brand(self):
+        return self._parameters['info']['brand']
+
+    @property
+    def base_shape(self):
+        return self._parameters['baseShape']
+
+    @property
+    def shape(self):
+        return self._parameters['shape']
+
+    def _change_scattering(self, surface_id, scattering):
+        return self._setup._change_scattering(surface_id=surface_id, scattering=scattering, part_id = self.id)
+
 def create_part(_setup, id, type_):
     '''
     Private
     '''
     # part = _setup._get_part(id)
     # _data = part.get(id)
     # if _data.get('detector_data'):
     #     part = Detector._new(_setup, id, _data)
     # elif _data.get('light_source'):
     #     part = LightSource._new(_setup, id, _data)
     # else:
     #     part = Part._new(_setup, id, _data)
     # return part
     type_ = int(type_)
+
+    if v.DEBUG:
+        print(f"Creating part with id: {id}, type: {type_}")
+
     if type_ == v.OPTICS_ADD_PART_TYPE:
         part = Optics._new(_setup = _setup, id = id, _data= None)
 
     elif type_ == v.DETECTOR_ADD_PART_TYPE:
         part = Detector._new(_setup = _setup, id = id, _data= None)
 
     elif type_ == v.LIGHT_SOURCE_ADD_PART_TYPE:
         part = LightSource._new(_setup = _setup, id = id, _data= None)
 
     else:
         part = Part._new(_setup = _setup, id = id, _data= None)
+
+    if v.DEBUG:
+        print(f"Part created: {type(part)}")
+
     return part
```

### Comparing `threed_optix-4.2.6/src/threed_optix/simulations.py` & `threed_optix-5.0.0/src/threed_optix/simulations.py`

 * *Files 10% similar despite different names*

```diff
@@ -143,17 +143,17 @@
         """
         Property to access the list of part objects of the setup.
         Returns:
             list: The list of Part objects.
         """
         if self._parts is None:
             self._get_parts()
-            self._user_backup[v.BASE_BACKUP] = {part.id: copy.deepcopy(part.data) for part in self}
-        parts = self._parts
-        return parts
+            self._user_backup[v.BASE_BACKUP] = {part.id: copy.deepcopy(part._data) for part in self}
+
+        return self._parts
 
     def _retrieve_parts(self):
         try:
             setup_data = self._api._get_setup_parts(self.id)
             parts = setup_data.get(self.id).get('parts')
 
             self._parts = [tdo_parts.create_part(_setup=self, id=part['id']) for part in parts]
@@ -173,29 +173,34 @@
         self._parts = []
 
         setup_data = self._api._get_setup_parts(self.id)
         parts = setup_data.get(self.id).get('parts')
         self._part_creation_errors = []
 
         for part in parts:
-                part = tdo_parts.create_part(_setup=self, id=part['id'], type_ = part['type'])
-                self._parts.append(part)
+                create_part(id=part['id'], type_ = part['type'])
 
         if len(self._part_creation_errors) > 0:
             raise self._part_creation_errors[0]
 
+        if v.DEBUG:
+            print(f"Parts retrieved: {len(self._parts)}")
+
         return None
 
     def _get_part(self, part_id):
         '''
         Private.
         '''
         part = self._api._get_part(part_id, self.id)
         return part
 
+    def _get_surface(self, part_id, surface_id):
+        return self._api._get_surface(setup_id = self.id, part_id=part_id, surface_id=surface_id)
+
     def get(self,
             part_label: str,
             all: bool = False):
         """
         Returns the part object with the specified label.
 
         Args:
@@ -345,61 +350,64 @@
         return results
 
     def delete_part(self, part: tdo_parts.Part):
         '''
         Deletes the part from the setup.
         '''
         self._api._delete_part(self.id, part.id)
-
+        self._parts = [p for p in self.parts if p.id != part.id]
         if isinstance(part, tdo_parts.LightSource):
-            self.light_sources.remove(part)
             for part in self:
                 for surface in part.surfaces:
                     for analysis in surface.analyses:
                         # if the laser id in the analysis rays attribute as key, delete the entry
                         if part.id in analysis.rays:
                             del analysis.rays[part.id]
 
-        if isinstance(part, tdo_parts.Detector):
-            self.detectors.remove(part)
-        if isinstance(part, tdo_parts.Optics):
-            self.optics.remove(part)
-
         return
 
-    def add_optics(self, number_id, label = None, pose = None):
-        part_id = self._api._add_part(self.id, v.OPTICS_ADD_PART_TYPE, number_id)
-        part = tdo_parts.create_part(_setup=self, id=part_id, type_ = v.OPTICS_ADD_PART_TYPE)
-        self.parts.append(part)
-        if pose:
-            part.change_pose(pose)
-        if label:
-            part.change_label(label)
-        return part
+    def add_optics(self, db_id, **kwargs):
+        if not all([key in v.AddParts.VALID_OPTICS_ARGUMENTS for key in kwargs.keys()]):
+            raise Exception(f'Invalid arguments for optics. Valid arguments are {v.AddParts.VALID_OPTICS_ARGUMENTS}')
+        return self._add_part(type_ = v.OPTICS_ADD_PART_TYPE, db_id = db_id, **kwargs)
+
+    def add_light_source(self, **kwargs):
+        if not all([key in v.AddParts.VALID_LIGHT_SOURCE_ARGUMENTS for key in kwargs.keys()]):
+            raise Exception(f'Invalid arguments for light source. Valid arguments are {v.AddParts.VALID_LIGHT_SOURCE_ARGUMENTS}')
+        return self._add_part(type_ = v.LIGHT_SOURCE_ADD_PART_TYPE, **kwargs)
+
+    def add_detector(self, **kwargs):
+        if not all([key in v.AddParts.VALID_DETECTOR_ARGUMENTS for key in kwargs.keys()]):
+            raise Exception(f'Invalid arguments for detector. Valid arguments are {v.AddParts.VALID_DETECTOR_ARGUMENTS}')
+        return self._add_part(type_ = v.DETECTOR_ADD_PART_TYPE, **kwargs)
+
+    def _add_part(self, type_, db_id=None, **kwargs):
+
+
+        part_id = self._api._add_part(setup_id=self.id,
+                                      type_=type_,
+                                      db_id=db_id
+                                      )
+
+        part = tdo_parts.create_part(_setup=self,
+                                     id=part_id,
+                                     type_ = type_
+                                     )
 
-    def add_light_source(self, label = None, pose = None):
-        part_id = self._api._add_part(self.id, v.LIGHT_SOURCE_ADD_PART_TYPE)
-        part = tdo_parts.create_part(_setup=self, id=part_id, type_ = v.LIGHT_SOURCE_ADD_PART_TYPE)
         self.parts.append(part)
-        if pose:
-            part.change_pose(pose)
-        if label:
-            part.change_label(label)
-        return part
 
-    def add_detector(self, label = None, pose = None):
-        part_id = self._api._add_part(self.id, v.DETECTOR_ADD_PART_TYPE)
-        part = tdo_parts.create_part(_setup=self, id=part_id, type_ = v.DETECTOR_ADD_PART_TYPE)
-        self.parts.append(part)
-        if pose:
-            part.change_pose(pose)
-        if label:
-            part.change_label(label)
+        part.change_config(**kwargs)
+
         return part
 
+    def _change_cs(self, part_id, lcs_id, rcs_id):
+        return self._api._change_cs(setup_id = self.id, part_id = part_id, lcs_id = lcs_id, rcs_id = rcs_id)
+
+    def _change_scattering(self, part_id, surface_id, scattering):
+        return self._api._change_scattering(setup_id = self.id, part_id = part_id, surface_id = surface_id, scattering = scattering)
 
 class Job:
     """
     Private.
     Contains information about a batch job.
 
     Attributes:
```

### Comparing `threed_optix-4.2.6/src/threed_optix/utils.py` & `threed_optix-5.0.0/src/threed_optix/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from scipy.stats import norm
 import cv2
 import threed_optix.package_utils.vars as v
 # import matlabparser as mpars
 # import threed_optix.package_utils.matlab as mt
 import re
 import matplotlib.pyplot as plt
+import plotly.express as px
 
 def wavelengths_normal_distribution(mean_wavelength, std_dev, num_wavelengths):
     wavelengths = {}
     wavelengths_list = np.linspace(mean_wavelength - 3 * std_dev, mean_wavelength + 3 * std_dev, num_wavelengths)
     weights =  norm.pdf(wavelengths_list, mean_wavelength, std_dev)
     sum_of_weights = np.sum(weights)
 
@@ -100,7 +101,21 @@
 
 def visualize_spot(matrix, center_point, radius):
     plt.figure(figsize=(10, 10))
     plt.imshow(matrix)
     plt.scatter(center_point[1], center_point[0], marker='x', color='red')
     plt.gca().add_patch(plt.Circle((center_point[1], center_point[0]), radius, color='red', fill=False))
     plt.show()
+
+def visualize_matrix(matrix, interactive = False, title = None):
+    if not interactive:
+        plt.figure(figsize=(10, 10))
+        plt.imshow(matrix)
+        if title:
+            plt.title(title)
+        plt.show()
+
+    if interactive:
+        fig = px.imshow(matrix, color_continuous_scale = v.COLOR_SCALE)
+        if title:
+            fig.update_layout(title_text = title)
+        fig.show()
```

### Comparing `threed_optix-4.2.6/src/threed_optix.egg-info/PKG-INFO` & `threed_optix-5.0.0/src/threed_optix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threed-optix
-Version: 4.2.6
+Version: 5.0.0
 Home-page: https://3doptix.com
 Author: 3DOptix
 Author-email: ereztep@3doptix.com
 License: MIT
 Keywords: Optics,Optical Design,Optical Simulation,Optical Design Software,3DOptix
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `threed_optix-4.2.6/src/threed_optix.egg-info/SOURCES.txt` & `threed_optix-5.0.0/src/threed_optix.egg-info/SOURCES.txt`

 * *Files identical despite different names*


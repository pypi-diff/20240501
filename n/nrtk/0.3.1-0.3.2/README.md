# Comparing `tmp/nrtk-0.3.1.tar.gz` & `tmp/nrtk-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrtk-0.3.1.tar", max compression
+gzip compressed data, was "nrtk-0.3.2.tar", max compression
```

## Comparing `nrtk-0.3.1.tar` & `nrtk-0.3.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    10173 2024-04-23 20:29:58.628306 nrtk-0.3.1/LICENSE
--rw-r--r--   0        0        0      554 2024-04-23 20:29:58.628306 nrtk-0.3.1/NOTICE
--rw-r--r--   0        0        0     2006 2024-04-23 20:29:58.628306 nrtk-0.3.1/README.md
--rw-r--r--   0        0        0      246 2024-04-23 20:29:58.684306 nrtk-0.3.1/nrtk/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 20:29:58.776306 nrtk-0.3.1/nrtk/impls/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 20:29:58.776306 nrtk-0.3.1/nrtk/impls/gen_object_detector_blackbox_response/__init__.py
--rw-r--r--   0        0        0     1986 2024-04-23 20:29:58.684306 nrtk-0.3.1/nrtk/impls/gen_object_detector_blackbox_response/simple_generic_generator.py
--rw-r--r--   0        0        0     3302 2024-04-23 20:29:58.684306 nrtk-0.3.1/nrtk/impls/gen_object_detector_blackbox_response/simple_pybsm_generator.py
--rw-r--r--   0        0        0        0 2024-04-23 20:29:58.776306 nrtk-0.3.1/nrtk/impls/perturb_image/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 20:29:58.776306 nrtk-0.3.1/nrtk/impls/perturb_image/generic/PIL/__init__.py
--rw-r--r--   0        0        0     4474 2024-04-23 20:29:58.684306 nrtk-0.3.1/nrtk/impls/perturb_image/generic/PIL/enhance.py
--rw-r--r--   0        0        0        0 2024-04-23 20:29:58.776306 nrtk-0.3.1/nrtk/impls/perturb_image/generic/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 20:29:58.776306 nrtk-0.3.1/nrtk/impls/perturb_image/generic/cv2/__init__.py
--rw-r--r--   0        0        0     2702 2024-04-23 20:29:58.684306 nrtk-0.3.1/nrtk/impls/perturb_image/generic/cv2/blur.py
--rw-r--r--   0        0        0      706 2024-04-23 20:29:58.684306 nrtk-0.3.1/nrtk/impls/perturb_image/generic/nop_perturber.py
--rw-r--r--   0        0        0        0 2024-04-23 20:29:58.776306 nrtk-0.3.1/nrtk/impls/perturb_image/generic/skimage/__init__.py
--rw-r--r--   0        0        0     6560 2024-04-23 20:29:58.684306 nrtk-0.3.1/nrtk/impls/perturb_image/generic/skimage/random_noise.py
--rw-r--r--   0        0        0        0 2024-04-23 20:29:58.776306 nrtk-0.3.1/nrtk/impls/perturb_image/pybsm/__init__.py
--rw-r--r--   0        0        0     2897 2024-04-23 20:29:58.684306 nrtk-0.3.1/nrtk/impls/perturb_image/pybsm/perturber.py
--rw-r--r--   0        0        0     4587 2024-04-23 20:29:58.684306 nrtk-0.3.1/nrtk/impls/perturb_image/pybsm/scenario.py
--rw-r--r--   0        0        0     8051 2024-04-23 20:29:58.684306 nrtk-0.3.1/nrtk/impls/perturb_image/pybsm/sensor.py
--rw-r--r--   0        0        0        0 2024-04-23 20:29:58.776306 nrtk-0.3.1/nrtk/impls/perturb_image_factory/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 20:29:58.776306 nrtk-0.3.1/nrtk/impls/perturb_image_factory/generic/__init__.py
--rw-r--r--   0        0        0     1656 2024-04-23 20:29:58.688306 nrtk-0.3.1/nrtk/impls/perturb_image_factory/generic/step.py
--rw-r--r--   0        0        0     3111 2024-04-23 20:29:58.688306 nrtk-0.3.1/nrtk/impls/perturb_image_factory/pybsm.py
--rw-r--r--   0        0        0        0 2024-04-23 20:29:58.776306 nrtk-0.3.1/nrtk/impls/score_detections/__init__.py
--rw-r--r--   0        0        0     2661 2024-04-23 20:29:58.688306 nrtk-0.3.1/nrtk/impls/score_detections/class_agnostic_pixelwise_iou_scorer.py
--rw-r--r--   0        0        0     4277 2024-04-23 20:29:58.688306 nrtk-0.3.1/nrtk/impls/score_detections/coco_scorer.py
--rw-r--r--   0        0        0     1346 2024-04-23 20:29:58.688306 nrtk-0.3.1/nrtk/impls/score_detections/nop_scorer.py
--rw-r--r--   0        0        0     1617 2024-04-23 20:29:58.688306 nrtk-0.3.1/nrtk/impls/score_detections/random_scorer.py
--rw-r--r--   0        0        0        0 2024-04-23 20:29:58.776306 nrtk-0.3.1/nrtk/interfaces/__init__.py
--rw-r--r--   0        0        0     2836 2024-04-23 20:29:58.688306 nrtk-0.3.1/nrtk/interfaces/gen_blackbox_response.py
--rw-r--r--   0        0        0     5401 2024-04-23 20:29:58.688306 nrtk-0.3.1/nrtk/interfaces/gen_classifier_blackbox_response.py
--rw-r--r--   0        0        0     5394 2024-04-23 20:29:58.688306 nrtk-0.3.1/nrtk/interfaces/gen_object_detector_blackbox_response.py
--rw-r--r--   0        0        0     1121 2024-04-23 20:29:58.688306 nrtk-0.3.1/nrtk/interfaces/perturb_image.py
--rw-r--r--   0        0        0     2750 2024-04-23 20:29:58.688306 nrtk-0.3.1/nrtk/interfaces/perturb_image_factory.py
--rw-r--r--   0        0        0     1345 2024-04-23 20:29:58.688306 nrtk-0.3.1/nrtk/interfaces/score_classifications.py
--rw-r--r--   0        0        0     1572 2024-04-23 20:29:58.688306 nrtk-0.3.1/nrtk/interfaces/score_detections.py
--rw-r--r--   0        0        0        0 2024-04-23 20:29:58.776306 nrtk-0.3.1/nrtk/interop/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 20:29:58.776306 nrtk-0.3.1/nrtk/py.typed
--rw-r--r--   0        0        0        0 2024-04-23 20:29:58.776306 nrtk-0.3.1/nrtk/utils/__init__.py
--rw-r--r--   0        0        0     2694 2024-04-23 20:29:58.692306 nrtk-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3285 1970-01-01 00:00:00.000000 nrtk-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    10173 2024-05-01 21:45:55.704154 nrtk-0.3.2/LICENSE
+-rw-r--r--   0        0        0      554 2024-05-01 21:45:55.704154 nrtk-0.3.2/NOTICE
+-rw-r--r--   0        0        0     2006 2024-05-01 21:45:55.704154 nrtk-0.3.2/README.md
+-rw-r--r--   0        0        0      246 2024-05-01 21:45:55.732154 nrtk-0.3.2/nrtk/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/impls/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/impls/gen_object_detector_blackbox_response/__init__.py
+-rw-r--r--   0        0        0     1986 2024-05-01 21:45:55.732154 nrtk-0.3.2/nrtk/impls/gen_object_detector_blackbox_response/simple_generic_generator.py
+-rw-r--r--   0        0        0     3302 2024-05-01 21:45:55.732154 nrtk-0.3.2/nrtk/impls/gen_object_detector_blackbox_response/simple_pybsm_generator.py
+-rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/impls/perturb_image/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/impls/perturb_image/generic/PIL/__init__.py
+-rw-r--r--   0        0        0     4774 2024-05-01 21:45:55.732154 nrtk-0.3.2/nrtk/impls/perturb_image/generic/PIL/enhance.py
+-rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/impls/perturb_image/generic/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/impls/perturb_image/generic/cv2/__init__.py
+-rw-r--r--   0        0        0     2702 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/impls/perturb_image/generic/cv2/blur.py
+-rw-r--r--   0        0        0      706 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/impls/perturb_image/generic/nop_perturber.py
+-rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/impls/perturb_image/generic/skimage/__init__.py
+-rw-r--r--   0        0        0     6560 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/impls/perturb_image/generic/skimage/random_noise.py
+-rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/impls/perturb_image/pybsm/__init__.py
+-rw-r--r--   0        0        0     3449 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/impls/perturb_image/pybsm/perturber.py
+-rw-r--r--   0        0        0     5051 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/impls/perturb_image/pybsm/scenario.py
+-rw-r--r--   0        0        0     8599 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/impls/perturb_image/pybsm/sensor.py
+-rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/impls/perturb_image_factory/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/impls/perturb_image_factory/generic/__init__.py
+-rw-r--r--   0        0        0     1656 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/impls/perturb_image_factory/generic/step.py
+-rw-r--r--   0        0        0     3160 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/impls/perturb_image_factory/pybsm.py
+-rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/impls/score_detections/__init__.py
+-rw-r--r--   0        0        0     2661 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/impls/score_detections/class_agnostic_pixelwise_iou_scorer.py
+-rw-r--r--   0        0        0     4277 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/impls/score_detections/coco_scorer.py
+-rw-r--r--   0        0        0     1346 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/impls/score_detections/nop_scorer.py
+-rw-r--r--   0        0        0     1617 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/impls/score_detections/random_scorer.py
+-rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/interfaces/__init__.py
+-rw-r--r--   0        0        0     2836 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/interfaces/gen_blackbox_response.py
+-rw-r--r--   0        0        0     5401 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/interfaces/gen_classifier_blackbox_response.py
+-rw-r--r--   0        0        0     5394 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/interfaces/gen_object_detector_blackbox_response.py
+-rw-r--r--   0        0        0     1121 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/interfaces/perturb_image.py
+-rw-r--r--   0        0        0     2750 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/interfaces/perturb_image_factory.py
+-rw-r--r--   0        0        0     1345 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/interfaces/score_classifications.py
+-rw-r--r--   0        0        0     1572 2024-05-01 21:45:55.736154 nrtk-0.3.2/nrtk/interfaces/score_detections.py
+-rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/interop/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/py.typed
+-rw-r--r--   0        0        0        0 2024-05-01 21:51:32.599870 nrtk-0.3.2/nrtk/utils/__init__.py
+-rw-r--r--   0        0        0     2667 2024-05-01 21:45:55.740154 nrtk-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3287 1970-01-01 00:00:00.000000 nrtk-0.3.2/PKG-INFO
```

### Comparing `nrtk-0.3.1/LICENSE` & `nrtk-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.1/NOTICE` & `nrtk-0.3.2/NOTICE`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.1/README.md` & `nrtk-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.1/nrtk/impls/gen_object_detector_blackbox_response/simple_generic_generator.py` & `nrtk-0.3.2/nrtk/impls/gen_object_detector_blackbox_response/simple_generic_generator.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.1/nrtk/impls/gen_object_detector_blackbox_response/simple_pybsm_generator.py` & `nrtk-0.3.2/nrtk/impls/gen_object_detector_blackbox_response/simple_pybsm_generator.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.1/nrtk/impls/perturb_image/generic/PIL/enhance.py` & `nrtk-0.3.2/nrtk/impls/perturb_image/generic/PIL/enhance.py`

 * *Files 7% similar despite different names*

```diff
@@ -79,16 +79,16 @@
         additional_params: Dict[str, Any] = {}
     ) -> np.ndarray:
         """
         Return image stimulus with adjusted brightness.
         """
 
         enhancement = ImageEnhance.Brightness
-        if TYPE_CHECKING:  # pragma: no cover
-            assert isinstance(enhancement, _Enhancement)
+        if TYPE_CHECKING and not isinstance(enhancement, _Enhancement):  # pragma: no cover
+            raise ValueError("enhancement does not conform to _Enhancement protocol")
         return self._perturb(enhancement=enhancement, image=image)
 
 
 class ColorPerturber(_PILEnhancePerturber):
     """
     Adjusts image stimulus color balance.
     """
@@ -99,16 +99,16 @@
         additional_params: Dict[str, Any] = {}
     ) -> np.ndarray:
         """
         Return image stimulus with adjusted color balance.
         """
 
         enhancement = ImageEnhance.Color
-        if TYPE_CHECKING:  # pragma: no cover
-            assert isinstance(enhancement, _Enhancement)
+        if TYPE_CHECKING and not isinstance(enhancement, _Enhancement):  # pragma: no cover
+            raise ValueError("enhancement does not conform to _Enhancement protocol")
         return self._perturb(enhancement=enhancement, image=image)
 
 
 class ContrastPerturber(_PILEnhancePerturber):
     """
     Adjusts image stimulus contrast.
     """
@@ -119,16 +119,16 @@
         additional_params: Dict[str, Any] = {}
     ) -> np.ndarray:
         """
         Return image stimulus with adjusted contrast.
         """
 
         enhancement = ImageEnhance.Contrast
-        if TYPE_CHECKING:  # pragma: no cover
-            assert isinstance(enhancement, _Enhancement)
+        if TYPE_CHECKING and not isinstance(enhancement, _Enhancement):  # pragma: no cover
+            raise ValueError("enhancement does not conform to _Enhancement protocol")
         return self._perturb(enhancement=enhancement, image=image)
 
 
 class SharpnessPerturber(_PILEnhancePerturber):
     """
     Adjusts image stimulus sharpness.
     """
@@ -152,10 +152,10 @@
         additional_params: Dict[str, Any] = {}
     ) -> np.ndarray:
         """
         Return image stimulus with adjusted sharpness.
         """
 
         enhancement = ImageEnhance.Sharpness
-        if TYPE_CHECKING:  # pragma: no cover
-            assert isinstance(enhancement, _Enhancement)
+        if TYPE_CHECKING and not isinstance(enhancement, _Enhancement):  # pragma: no cover
+            raise ValueError("enhancement does not conform to _Enhancement protocol")
         return self._perturb(enhancement=enhancement, image=image)
```

### Comparing `nrtk-0.3.1/nrtk/impls/perturb_image/generic/cv2/blur.py` & `nrtk-0.3.2/nrtk/impls/perturb_image/generic/cv2/blur.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.1/nrtk/impls/perturb_image/generic/nop_perturber.py` & `nrtk-0.3.2/nrtk/impls/perturb_image/generic/nop_perturber.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.1/nrtk/impls/perturb_image/generic/skimage/random_noise.py` & `nrtk-0.3.2/nrtk/impls/perturb_image/generic/skimage/random_noise.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.1/nrtk/impls/perturb_image/pybsm/perturber.py` & `nrtk-0.3.2/nrtk/impls/perturb_image/pybsm/perturber.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,43 +18,52 @@
             **kwargs: Any
             ) -> None:
 
         """
         :param sensor: pyBSM sensor object.
         :param scenario: pyBSM scenario object.
         :param reflectance_range: Array of reflectances that correspond to pixel values.
+
+        :raises: ValueError if reflectance_range length != 2
+        :raises: ValueError if reflectance_range not strictly ascending
         """
         self.sensor = copy.deepcopy(sensor)
         self.scenario = copy.deepcopy(scenario)
 
         for k in kwargs:
             if hasattr(self.sensor, k):
                 setattr(self.sensor, k, kwargs[k])
             elif hasattr(self.scenario, k):
                 setattr(self.scenario, k, kwargs[k])
 
         self.metrics = pybsm.niirs(self.sensor, self.scenario)
 
-        assert reflectance_range.shape[0] == 2
-        assert reflectance_range[0] < reflectance_range[1]
+        if reflectance_range.shape[0] != 2:
+            raise ValueError(f"Reflectance range array must have length of 2, got {reflectance_range.shape[0]}")
+        if reflectance_range[0] >= reflectance_range[1]:
+            raise ValueError(f"Reflectance range array values must be strictly ascending, got {reflectance_range}")
         self.reflectance_range = reflectance_range
 
         # this is key:value record of the thetas use for perturbing
         self.thetas = copy.deepcopy(kwargs)
 
     @property
     def params(self) -> Dict:
         return self.thetas
 
     def perturb(
             self,
             image: np.ndarray,
             additional_params: Dict[str, Any] = {}
             ) -> np.ndarray:
-        assert 'img_gsd' in additional_params
+        """
+        :raises: ValueError if 'img_gsd' not present in additional_params
+        """
+        if 'img_gsd' not in additional_params:
+            raise ValueError("'img_gsd' must be present in image metadata for this perturber")
 
         perturbed = pybsm.metrics2image(
                     self.metrics,
                     image,
                     additional_params['img_gsd'],
                     np.array([image.min(), image.max()]),
                     self.reflectance_range)[-1]
```

### Comparing `nrtk-0.3.1/nrtk/impls/perturb_image/pybsm/scenario.py` & `nrtk-0.3.2/nrtk/impls/perturb_image/pybsm/scenario.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,18 @@
     backgroundTemperature:
         background temperature (Kelvin)
     haWindspeed:
         the high altitude windspeed (m/s).  Used to calculate the turbulence profile.
     cn2at1m:
         the refractive index structure parameter "near the ground" (e.g. at h = 1 m).
         Used to calculate the turbulence profile.
+
+    :raises: ValueError if ihaze not in acceptable ihaze values
+    :raises: ValueError if altitude not in acceptable altitude values
+    :raises: ValueError if ground range not in acceptable ground range values
     """
 
     ihaze_values = [1, 2]
     altitude_values = [2, 32.55, 75, 150, 225, 500] + \
         list(range(1000, 12001, 1000)) + \
         list(range(14000, 20001, 2000)) + [24500]
     groundRange_values = [0, 100, 500] + \
@@ -58,17 +62,20 @@
                  targetReflectance: Optional[float] = 0.15,
                  targetTemperature: Optional[float] = 295.0,
                  backgroundReflectance: Optional[float] = 0.07,
                  backgroundTemperature: Optional[float] = 293.0,
                  haWindspeed: Optional[float] = 21.0,
                  cn2at1m: Optional[float] = 1.7e-14
                  ):
-        assert ihaze in PybsmScenario.ihaze_values
-        assert altitude in PybsmScenario.altitude_values
-        assert groundRange in PybsmScenario.groundRange_values
+        if ihaze not in PybsmScenario.ihaze_values:
+            raise ValueError(f"Invalid ihaze value ({ihaze}) must be in {PybsmScenario.ihaze_values}")
+        if altitude not in PybsmScenario.altitude_values:
+            raise ValueError(f"Invalid altitude value ({altitude})")
+        if groundRange not in PybsmScenario.groundRange_values:
+            raise ValueError(f"Invalid ground range value ({groundRange})")
 
         # required parameters
         self.name = name
         self.ihaze = ihaze
         self.altitude = altitude
         self.groundRange = groundRange
```

### Comparing `nrtk-0.3.1/nrtk/impls/perturb_image/pybsm/sensor.py` & `nrtk-0.3.2/nrtk/impls/perturb_image/pybsm/sensor.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         effective aperture diameter (m)
     f :
         focal length (m)
     px and py :
         detector center-to-center spacings (pitch) in the x and y directions (m)
     optTransWavelengths :
         numpy array specifying the spectral bandpass of the camera (m).  At
-        minimum, and start and end wavelength should be specified.
+        minimum, start and end wavelength should be specified.
     opticsTransmission :
         full system in-band optical transmission (unitless).  Loss due to any
         telescope obscuration should *not* be included in with this optical transmission
         array.
     eta :
         relative linear obscuration (unitless)
     wx and wy :
@@ -83,14 +83,18 @@
         (read noise, photon noise, dark current, quantization noise are
         all already included)
     filterKernel:
          2-D filter kernel (for sharpening or whatever).  Note that
          the kernel is assumed to sum to one.
     framestacks:
          the number of frames to be added together for improved SNR.
+
+    :raises: ValueError if optTransWavelengths length < 2
+    :raises: ValueError if optTransWavelengths is not ascending
+    :raises: ValueError if optTransWavelengths and (if provided) opticsTransmission lengths are different
     """
     def __init__(self,
                  name: str,
                  D: float,
                  f: float,
                  px: float,
                  optTransWavelengths: np.ndarray,
@@ -107,29 +111,33 @@
                  sx: Optional[float] = 0.0,
                  sy: Optional[float] = 0.0,
                  dax: Optional[float] = 0.0,
                  day: Optional[float] = 0.0,
                  qewavelengths: Optional[np.ndarray] = None,
                  qe: Optional[np.ndarray] = None
                  ):
-        assert optTransWavelengths.shape[0] >= 2
-        assert optTransWavelengths[0] < optTransWavelengths[-1]
+        if optTransWavelengths.shape[0] < 2:
+            raise ValueError("At minimum, at least the start and end wavelengths"
+                             " must be specified for optTransWavelengths")
+        if optTransWavelengths[0] >= optTransWavelengths[-1]:
+            raise ValueError("optTransWavelengths must be ascending")
 
         # required parameters
         self.name = name
         self.D = D
         self.f = f
         self.px = px
         self.optTransWavelengths = optTransWavelengths
 
         # optional parameters
         if opticsTransmission is None:
             self.opticsTransmission = np.ones(optTransWavelengths.shape[0])
         else:
-            assert opticsTransmission.shape[0] == optTransWavelengths.shape[0]
+            if opticsTransmission.shape[0] != optTransWavelengths.shape[0]:
+                raise ValueError("opticsTransmission and optTransWavelengths must have the same length")
             self.opticsTransmission = opticsTransmission
         self.eta = eta
         self.py = px
         self.wx = px if wx is None else wx
         self.wy = px if wy is None else wy
         self.intTime = intTime
         self.darkCurrent = darkCurrent
```

### Comparing `nrtk-0.3.1/nrtk/impls/perturb_image_factory/generic/step.py` & `nrtk-0.3.2/nrtk/impls/perturb_image_factory/generic/step.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.1/nrtk/impls/perturb_image_factory/pybsm.py` & `nrtk-0.3.2/nrtk/impls/perturb_image_factory/pybsm.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,16 @@
             func = PybsmPerturber(self.sensor, self.scenario, **kwargs)
             self.n += 1
             return func
         else:
             raise StopIteration
 
     def __getitem__(self, idx: int) -> PerturbImage:
-        assert idx < len(self.sets)
+        if idx >= len(self.sets):
+            raise IndexError("Index out of range")
         kwargs = {
             k: self.thetas[i][self.sets[idx][i]]
             for i, k in enumerate(self.theta_keys)
             }
         func = PybsmPerturber(self.sensor, self.scenario, **kwargs)
         return func
```

### Comparing `nrtk-0.3.1/nrtk/impls/score_detections/class_agnostic_pixelwise_iou_scorer.py` & `nrtk-0.3.2/nrtk/impls/score_detections/class_agnostic_pixelwise_iou_scorer.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.1/nrtk/impls/score_detections/coco_scorer.py` & `nrtk-0.3.2/nrtk/impls/score_detections/coco_scorer.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.1/nrtk/impls/score_detections/nop_scorer.py` & `nrtk-0.3.2/nrtk/impls/score_detections/nop_scorer.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.1/nrtk/impls/score_detections/random_scorer.py` & `nrtk-0.3.2/nrtk/impls/score_detections/random_scorer.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.1/nrtk/interfaces/gen_blackbox_response.py` & `nrtk-0.3.2/nrtk/interfaces/gen_blackbox_response.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.1/nrtk/interfaces/gen_classifier_blackbox_response.py` & `nrtk-0.3.2/nrtk/interfaces/gen_classifier_blackbox_response.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.1/nrtk/interfaces/gen_object_detector_blackbox_response.py` & `nrtk-0.3.2/nrtk/interfaces/gen_object_detector_blackbox_response.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.1/nrtk/interfaces/perturb_image.py` & `nrtk-0.3.2/nrtk/interfaces/perturb_image.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.1/nrtk/interfaces/perturb_image_factory.py` & `nrtk-0.3.2/nrtk/interfaces/perturb_image_factory.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.1/nrtk/interfaces/score_classifications.py` & `nrtk-0.3.2/nrtk/interfaces/score_classifications.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.1/nrtk/interfaces/score_detections.py` & `nrtk-0.3.2/nrtk/interfaces/score_detections.py`

 * *Files identical despite different names*

### Comparing `nrtk-0.3.1/pyproject.toml` & `nrtk-0.3.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ###############################################################################
 [tool.poetry]
 name = "nrtk"
 # REMEMBER: `distutils.version.*Version` types can be used to compare versions
 # from strings like this.
 # This package prefers to use the strict numbering standard when possible.
-version = "0.3.1"
+version = "0.3.2"
 description = ""
 license = "Apache-2.0"
 authors = ["Kitware, Inc. <nrtk@kitware.com>"]
 readme = "README.md"
 packages = [{include = "nrtk"}]
 documentation = "https://nrtk.readthedocs.io/"
 classifiers = [
@@ -29,15 +29,15 @@
     'Programming Language :: Python :: 3.11',
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 numpy = ">=1.18"
 opencv-python = ">=4.6"
-Pillow = ">=10.0"
+Pillow = ">=10.2.0"
 scikit-image = ">=0.21"
 smqtk-classifier = ">=0.19.0"
 smqtk-core = ">=0.19"
 smqtk-detection = ">=0.19.0"
 smqtk-image-io = ">=0.17.1"
 tqdm = ">=4.64"
 pybsm = "<0.2.0"
@@ -56,23 +56,21 @@
 types-setuptools = ">=65.6.0.1"
 types-tqdm = ">=4.64"
 # Testing
 coverage = ">=6.5.0"
 pytest = ">=7.2.0"
 pytest-cov = ">=4.0.0"
 # Jupyter notebook testing
-jupyter = ">=1.0.0"
+notebook = ">=7.0.7"
 papermill = ">=2.4.0"
 # Docs
 Sphinx = ">=5.3.0"
 sphinx-rtd-theme = ">=1.1.1"
 sphinx-prompt = ">=1.5.0"
 livereload = ">=2.6.3"
-# Utility
-ipython = ">=8.6.0"
 
 
 [tool.poetry.scripts]
 
 [tool.poetry.plugins."smqtk_plugins"]
```

### Comparing `nrtk-0.3.1/PKG-INFO` & `nrtk-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nrtk
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 License: Apache-2.0
 Author: Kitware, Inc.
 Author-email: nrtk@kitware.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -14,15 +14,15 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
-Requires-Dist: Pillow (>=10.0)
+Requires-Dist: Pillow (>=10.2.0)
 Requires-Dist: numpy (>=1.18)
 Requires-Dist: opencv-python (>=4.6)
 Requires-Dist: pybsm (<0.2.0)
 Requires-Dist: pycocotools (>=2.0.6)
 Requires-Dist: scikit-image (>=0.21)
 Requires-Dist: setuptools (>=65.6.1)
 Requires-Dist: smqtk-classifier (>=0.19.0)
```


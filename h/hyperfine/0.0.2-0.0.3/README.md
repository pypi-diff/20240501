# Comparing `tmp/hyperfine-0.0.2.tar.gz` & `tmp/hyperfine-0.0.3.tar.gz`

## Comparing `hyperfine-0.0.2.tar` & `hyperfine-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 hyperfine-0.0.2/hyperfine/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hyperfine-0.0.2/hyperfine/_version.py
--rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 hyperfine-0.0.2/hyperfine/demagnetization.py
--rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 hyperfine-0.0.2/hyperfine/distributions.py
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 hyperfine-0.0.2/hyperfine/dpass.py
--rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 hyperfine-0.0.2/hyperfine/minuit.py
--rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 hyperfine-0.0.2/hyperfine/srf.py
--rw-r--r--   0        0        0    10872 2020-02-02 00:00:00.000000 hyperfine-0.0.2/hyperfine/srim.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 hyperfine-0.0.2/hyperfine/bnmr/__init__.py
--rw-r--r--   0        0        0    14249 2020-02-02 00:00:00.000000 hyperfine-0.0.2/hyperfine/bnmr/lineshape.py
--rw-r--r--   0        0        0    18998 2020-02-02 00:00:00.000000 hyperfine-0.0.2/hyperfine/bnmr/meissner.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 hyperfine-0.0.2/hyperfine/bnmr/nlme.py
--rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 hyperfine-0.0.2/hyperfine/bnmr/susceptibility.py
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 hyperfine-0.0.2/hyperfine/musr/__init__.py
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 hyperfine-0.0.2/hyperfine/musr/_meissner.py
--rw-r--r--   0        0        0    19756 2020-02-02 00:00:00.000000 hyperfine-0.0.2/hyperfine/musr/meissner.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 hyperfine-0.0.2/hyperfine/superconductivity/__init__.py
--rw-r--r--   0        0        0     6126 2020-02-02 00:00:00.000000 hyperfine-0.0.2/hyperfine/superconductivity/bcs.py
--rw-r--r--   0        0        0    12048 2020-02-02 00:00:00.000000 hyperfine-0.0.2/hyperfine/superconductivity/gle.py
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 hyperfine-0.0.2/hyperfine/superconductivity/interpolation.py
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 hyperfine-0.0.2/hyperfine/superconductivity/intertype.py
--rw-r--r--   0        0        0    10438 2020-02-02 00:00:00.000000 hyperfine-0.0.2/hyperfine/superconductivity/pippard.py
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 hyperfine-0.0.2/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 hyperfine-0.0.2/LICENSE
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 hyperfine-0.0.2/README.md
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 hyperfine-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 hyperfine-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/_version.py
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/demagnetization.py
+-rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/distributions.py
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/dpass.py
+-rw-r--r--   0        0        0     6037 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/minuit.py
+-rw-r--r--   0        0        0    13475 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/srim.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/bnmr/__init__.py
+-rw-r--r--   0        0        0    14249 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/bnmr/lineshape.py
+-rw-r--r--   0        0        0    18998 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/bnmr/meissner.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/bnmr/nlme.py
+-rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/bnmr/susceptibility.py
+-rw-r--r--   0        0        0     8229 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/musr/__init__.py
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/musr/_meissner.py
+-rw-r--r--   0        0        0    26336 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/musr/meissner.py
+-rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/superconductivity/__init__.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/superconductivity/_muhlschlegel.py
+-rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/superconductivity/bcs.py
+-rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/superconductivity/ccf.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/superconductivity/interpolation.py
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/superconductivity/intertype.py
+-rw-r--r--   0        0        0    18362 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/superconductivity/london.py
+-rw-r--r--   0        0        0    15737 2020-02-02 00:00:00.000000 hyperfine-0.0.3/hyperfine/superconductivity/pippard.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 hyperfine-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 hyperfine-0.0.3/LICENSE
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 hyperfine-0.0.3/README.md
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 hyperfine-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 hyperfine-0.0.3/PKG-INFO
```

### Comparing `hyperfine-0.0.2/hyperfine/demagnetization.py` & `hyperfine-0.0.3/hyperfine/demagnetization.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.2/hyperfine/distributions.py` & `hyperfine-0.0.3/hyperfine/distributions.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.2/hyperfine/dpass.py` & `hyperfine-0.0.3/hyperfine/dpass.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.2/hyperfine/minuit.py` & `hyperfine-0.0.3/hyperfine/minuit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,29 @@
+"""Utilities for interacting with the ``iminuit`` package.
+"""
+
 import json
 import numpy as np
 import iminuit
 from iminuit import Minuit
 from typing import Callable
 from joblib import Parallel, delayed, cpu_count
 
 
 def minos2dict(minuit: Minuit) -> dict:
-    """
-    Convert the MINOS errors to a dictionary (e.g., for serialization).
+    """Convert the MINOS errors to a dictionary.
+
+    Convert the MINOS (i.e., asymmetric) errors determined by the MINUIT2
+    minimizer to a dictionary (e.g., for serialization).
+
+    Args:
+        minuit: The ``iminuit.Minuit`` object.
+
+    Returns:
+        A dictionary containing the MINOS errors.
     """
 
     # empty dictionary to hold the results
     minos = {}
 
     # loop over all fit parameters
     for item in minuit.merrors.items():
@@ -31,16 +42,19 @@
         minos[par] = mdict
 
     # return the filled minos dictionary
     return minos
 
 
 def minuit2json(minuit: Minuit, filename: str) -> None:
-    """
-    Serialize fitting results from an `iminuit.Minuit` object to a JSON file.
+    """Serialize fitting results from an `iminuit.Minuit` object to a JSON file.
+
+    Args:
+        minuit: The ``iminuit.Minuit`` object.
+        filename: Name of JSON file to save the serialized fit results.
     """
 
     # convert the results to a dictionary
     results = {
         "values": minuit.values.to_dict(),
         "errors": minuit.errors.to_dict(),
         "limits": minuit.limits.to_dict(),
@@ -50,16 +64,19 @@
 
     # write the results dictionary to a file
     with open(filename, "w") as fh:
         json.dump(results, fh, indent="\t")
 
 
 def json2minuit(minuit: Minuit, filename: str) -> None:
-    """
-    De-serialize fitting results from a JSON file to an `iminuit.Minuit` object.
+    """De-serialize fitting results from a JSON file to an `iminuit.Minuit` object.
+
+    Args:
+        minuit: The ``iminuit.Minuit`` object.
+        filename: Name of JSON file containing the serialized fit results.
     """
 
     # read the results into a dictionary
     with open(filename, "r") as fh:
         results = json.load(fh)
 
     # restore the fit quantities
@@ -68,16 +85,15 @@
             for key, value in results[quantity].items():
                 minuit.__getattribute__(quantity)[key] = value
 
     # TODO: restore the minos errors
 
 
 class GenericLeastSquares3D:
-    """
-    Generic 3D least-squares cost function with error.
+    """Generic 3D least-squares cost function with error.
 
     https://iminuit.readthedocs.io/en/stable/tutorial/generic_least_squares.html
     """
 
     # for Minuit to compute errors correctly
     errordef = iminuit.Minuit.LEAST_SQUARES
```

### Comparing `hyperfine-0.0.2/hyperfine/srim.py` & `hyperfine-0.0.3/hyperfine/srim.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,57 @@
+"""Facilities for creating/parsing SRIM input/output files.
+
+The Stopping and Range of Ions in Matter (SRIM) is a suite of programs for
+calculating and simulating projectile-matter interactions during
+ion-implantation.
+
+http://srim.org/
+"""
+
 import string
 import warnings
 import numpy as np
 
 
 def get_line_number(
     filename: str = "RANGE_3D.txt",
     phrase: str = "-------  ----------- ----------- -----------",
     encoding: str = "gbk",
 ) -> int:
-    """
-    Deduce where the data columns start in the `RANGE_3D.txt` file output by SRIM.
+    """Deduce where the data columns start in the ``RANGE_3D.txt`` file output by ``TRIM.exe``.
 
     Args:
-        filename: Name of the `RANGE_3D.txt` file output from SRIM
-        phrase: Character sequence to find in the file
-        encoding: Encoding of the `RANGE_3D.txt` file
+        filename: Name of the ``RANGE_3D.txt`` file output from ``SRIM``.
+        phrase: Character sequence to find in the file.
+        encoding: Encoding of the ``RANGE_3D.txt`` file.
 
     Returns:
-        The line number in `RANGE_3D.txt.` that matches `phrase`.
+        The line number in ``RANGE_3D.txt`` that matches ``phrase``.
     """
 
     # https://stackoverflow.com/a/3961303
     with open(filename, "r", encoding=encoding) as fh:
         for i, line in enumerate(fh, 1):
             if phrase in line:
                 return i
     # return a negative index if the phrase is not found
     return -1
 
 
 def _unix2dos(filename: str) -> None:
-    """
-    Convenience method replicating the functionality of unix2dos.
+    """Convenience method replicating the functionality of ``unix2dos``.
+
+    ``unix2dos`` is a non-standard Unix program for converting line breaks in a
+    text file from Unix format (Line feed) to DOS format (carriage return +
+    Line feed).
+
+    See: https://en.wikipedia.org/wiki/Unix2dos
+
+    Args:
+        filename: Name of the file run ``unix2dos`` on.
     """
 
     with open(filename, "rb") as input_file:
         input_string = input_file.read()
 
     # systematically replace & harmonize all line breaks
     output_string = (
@@ -60,16 +76,23 @@
     atomic_number: int,
     energy_eV: float,
     angle_mean_deg: float = 0.0,
     angle_sigma_deg: float = np.finfo(float).eps,
     description: str = "",
     total_ions: int = 99999,
 ) -> None:
-    """
-    Create a TRIM.DAT file for use in an advanced TRIM calculation.
+    """Create a ``TRIM.DAT`` file for use in an advanced ``TRIM.exe`` calculation.
+
+    Args:
+        atomic_number: Atomic number of the projectile.
+        energy_eV: Energy of the projectile (eV).
+        angle_mean_deg: Mean angle of incidence with respect to the surface normal (degrees).
+        angle_sigma_deg: Standard deviation of the angle of incidence (degrees).
+        description: Description of simulation.
+        total_ions: Total number of ions to generate.
     """
 
     assert (atomic_number >= 1) & (atomic_number <= 92)
     assert energy_eV >= 0.0
     assert angle_sigma_deg > 0.0
 
     with open("TRIM.dat", "w", encoding="gbk") as fh:
@@ -162,21 +185,36 @@
     a: float = 1.0,
     b: float = 1.0,
     c: float = 1.0,
     e_x_0: float = 0.0,
     e_y_0: float = 0.0,
     e_z_0: float = 0.0,
 ) -> np.array:
+    """Calculate the unit vector normal to the surface of an ellipsoid at point :math:`p = (x, y, z)`.
+
+    Args:
+        x: Spatial position :math:`x`.
+        y: Spatial position :math:`y`.
+        z: Spatial position :math:`z`.
+        a: Ellipsoid semi-axis :math:`a`.
+        b: Ellipsoid semi-axis :math:`b`.
+        c: Ellipsoid semi-axis :math:`c`.
+        e_x_0: Ellipsoid :math:`x`-coordinate centre.
+        e_y_0: Ellipsoid :math:`y`-coordinate centre.
+        e_z_0: Ellipsoid :math:`z`-coordinate centre.
+
+    Returns:
+        The unit vector normal to the ellipsoid surface at :math:`p`.
     """
-    Calculate the unit vector normal to the surface of an ellipsoid at point p = (x, y, z).
-    """
+
     df_dx = 2.0 * (x - e_x_0) / np.square(a)
     df_dy = 2.0 * (y - e_y_0) / np.square(b)
     df_dz = 2.0 * (z - e_z_0) / np.square(c)
     magnitude = np.sqrt(np.square(df_dx) + np.square(df_dy) + np.square(df_dz))
+
     return np.array([df_dx, df_dy, df_dz]) / magnitude
 
 
 def create_trim_dat_ellipsoid(
     beam_atomic_number: int,
     beam_energy_eV: float,
     beam_fwhm_y_mm: float = 3.0,
@@ -188,18 +226,37 @@
     ellipsoid_semiaxis_c_mm: float = 2.0,
     ellipsoid_position_x_mm: float = 0.0,
     ellipsoid_position_y_mm: float = 0.0,
     ellipsoid_position_z_mm: float = 0.0,
     description: str = "",
     total_ions: int = 99999,
 ) -> None:
-    """
-    Create a TRIM.DAT file for use in an advanced TRIM calculation.
+    """Create a ``TRIM.DAT`` file for use in an advanced ``TRIM.exe`` calculation.
+
+    In a standard TRIM calculation, the program assumes a flat target with
+    infinite lateral dimensions. Within this constraint, this function attempts
+    to transform the projectile ion trajectories to approximate incidence with
+    an ellipsoid-shaped target.
 
-    This function is specific to an ellipsoid target.
+    As with all TRIM calculations, the beam/projectile direction is initially
+    parallel the :math:`x`-axis.
+
+    Args:
+        beam_atomic_number: Projectile atomic number.
+        beam_energy_eV: Projectile energy (eV).
+        beam_fwhm_y_mm: FWHM of the projectile beam's lateral spread in the :math:`y`-direction.
+        beam_fwhm_z_mm: FWHM of the projectile beam's lateral spread in the :math:`z`-direction.
+        ellipsoid_semiaxis_a_mm: Ellipsoid semi-axis :math:`a`.
+        ellipsoid_semiaxis_b_mm: Ellipsoid semi-axis :math:`b`.
+        ellipsoid_semiaxis_c_mm: Ellipsoid semi-axis :math:`c`.
+        ellipsoid_position_x_mm: Ellipsoid :math:`x`-coordinate centre.
+        ellipsoid_position_y_mm: Ellipsoid :math:`y`-coordinate centre.
+        ellipsoid_position_z_mm: Ellipsoid :math:`z`-coordinate centre.
+        description: Description of simulation.
+        total_ions: Total number of ions to generate.
     """
 
     assert (beam_atomic_number >= 1) & (beam_atomic_number <= 92)
     assert beam_energy_eV >= 0.0
     assert (
         (ellipsoid_semiaxis_a_mm > 0.0)
         & (ellipsoid_semiaxis_b_mm > 0.0)
```

### Comparing `hyperfine-0.0.2/hyperfine/bnmr/lineshape.py` & `hyperfine-0.0.3/hyperfine/bnmr/lineshape.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.2/hyperfine/bnmr/meissner.py` & `hyperfine-0.0.3/hyperfine/bnmr/meissner.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.2/hyperfine/bnmr/nlme.py` & `hyperfine-0.0.3/hyperfine/bnmr/nlme.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.2/hyperfine/bnmr/susceptibility.py` & `hyperfine-0.0.3/hyperfine/bnmr/susceptibility.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.2/hyperfine/musr/_meissner.py` & `hyperfine-0.0.3/hyperfine/musr/_meissner.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.2/hyperfine/musr/meissner.py` & `hyperfine-0.0.3/hyperfine/musr/meissner.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 
 from typing import Annotated, Sequence, override
 import numpy as np
 import pandas as pd
 from scipy import constants, integrate, interpolate, special
 from .. import distributions
-from ..superconductivity import pippard
+from ..superconductivity import london, pippard
 
 
 class DepthAveragingCalculator:
     """Calculator for convolving a Meissner screening profile with a muon stopping distribution.
 
     Class for handling the details required for calculating the mean magnetic
     field at a given muon implantation energy by convolving a Meissner
@@ -350,16 +350,15 @@
             mean_free_path_nm: Electron mean-free-path (nm).
             demagnetization_factor: Effective demagnetization factor.
             temperature_K: Absolute temperature (K).
             critical_temperature_K: Superconducting transition temperature (K).
             gap_0K_eV: Superconducting gap energy at 0 K (eV).
 
         Returns:
-            The field screening profile at a given depth.
-
+            The field screening profile at a given depth (G).
         """
 
         return (
             # nonlocal field screening model
             pippard.specular_profile_dl(
                 depth_nm,
                 temperature_K,
@@ -402,16 +401,15 @@
             mean_free_path_nm: Electron mean-free-path (nm).
             demagnetization_factor: Effective demagnetization factor.
             temperature_K: Absolute temperature (K).
             critical_temperature_K: Superconducting transition temperature (K).
             gap_0K_eV: Superconducting gap energy at 0 K (eV).
 
         Returns:
-            Integrand for the average magnetic field at a given implantation energy.
-
+            Integrand for the average magnetic field at a given implantation energy (G).
         """
 
         return self.pippard_ms(
             z,
             applied_field_G,
             dead_layer_nm,
             london_penetration_depth_nm,
@@ -448,16 +446,15 @@
             mean_free_path_nm: Electron mean-free-path (nm).
             demagnetization_factor: Effective demagnetization factor.
             temperature_K: Absolute temperature (K).
             critical_temperature_K: Superconducting transition temperature (K).
             gap_0K_eV: Superconducting gap energy at 0 K (eV).
 
         Returns:
-            The average magnetic field at a given implantation energy.
-
+            The average magnetic field at a given implantation energy (G).
         """
 
         # do the numeric integration using adaptive Gaussian quadrature
         # https://docs.scipy.org/doc/scipy/reference/generated/scipy.integrate.quad.html
         result, _ = integrate.quad(
             self.mean_field_integrand,
             0.0,  # lower integration limit
@@ -488,25 +485,25 @@
         )
 
         return result
 
     @override
     def __call__(
         self,
-        energy_keV: float,
+        energy_keV: Sequence[float],
         applied_field_G: Annotated[float, 0:None],
         dead_layer_nm: Annotated[float, 0:None],
         london_penetration_depth_nm: Annotated[float, 0:None],
         bcs_coherence_length_nm: Annotated[float, 0:None],
         mean_free_path_nm: Annotated[float, 0:None],
         demagnetization_factor: Annotated[float, 0:1],
         temperature_K: Annotated[float, 0:None],
         critical_temperature_K: Annotated[float, 0:None],
         gap_0K_eV: Annotated[float, 0:None],
-    ) -> float:
+    ) -> Sequence[float]:
         """Calculate average magnetic field at a given implantation energy.
 
         Functor version!
 
         Args:
             energy_keV: Implantation energy (keV).
             applied_field_G: Applied magnetic field (G).
@@ -517,15 +514,14 @@
             demagnetization_factor: Effective demagnetization factor.
             temperature_K: Absolute temperature (K).
             critical_temperature_K: Superconducting transition temperature (K).
             gap_0K_eV: Superconducting gap energy at 0 K (eV).
 
         Returns:
             The average magnetic field at a given implantation energy.
-
         """
 
         # make everything numpy arrays
         energy_keV = np.asarray(energy_keV)
         results = np.empty(energy_keV.size)
 
         for i, e_keV in enumerate(energy_keV):
@@ -538,7 +534,174 @@
                 mean_free_path_nm,
                 demagnetization_factor,
                 temperature_K,
                 critical_temperature_K,
                 gap_0K_eV,
             )
         return results
+
+
+class DepthAveragingCalculatorGLE(DepthAveragingCalculator):
+    """Calculator for convolving a Meissner screening profile with a muon stopping distribution.
+
+    Class for handling the details required for calculating the mean magnetic
+    field at a given muon implantation energy by convolving a Meissner
+    screening profile with the corresponding stopping distribution.
+
+    This instance assumes local electrodynamics following the generalized
+    London equation (GLE).
+    """
+
+    def __init__(
+        self,
+        file_name: str,
+        interpolation: str = "linear",
+    ) -> None:
+        """Constructor.
+
+        Args:
+            file_name: Name of the CSV containing the stopping profile coefficients.
+            interpolation: Type of interpolation scheme used for the stopping profile coefficients.
+        """
+
+        # generalized London equation (GLE) solver
+        self.gle = london.GLESolver()
+
+        # initialize from the base class
+        super().__init__(file_name, interpolation)
+
+    def mean_field_integrand(
+        self,
+        z: float,
+        energy_keV: float,
+        applied_field_G: Annotated[float, 0:None],
+        dead_layer_nm: Annotated[float, 0:None],
+        surface_penetration_depth_nm: Annotated[float, 0:None],
+        bulk_penetration_depth_nm: Annotated[float, 0:None],
+        diffusion_length_nm: Annotated[float, 0:None],
+        demagnetization_factor: Annotated[float, 0:1] = 0.0,
+    ) -> float:
+        """Integrand for calculating the mean magnetic field at a given implantation energy.
+
+        Args:
+            z: Depth (nm).
+            energy_keV: Implantation energy (keV).
+            applied_field_G: Applied magnetic field (G).
+            dead_layer_nm: Non-superconducting dead layer (nm).
+            surface_penetration_depth_nm: Magnetic penetration depth at the surface (nm).
+            bulk_penetration_depth_nm: Magnetic penetration depth in the bulk (nm).
+            diffusion_length_nm: Length of inhomogenous defect region (nm).
+            demagnetization_factor: Effective demagnetization factor.
+
+        Returns:
+            Integrand for the average magnetic field at a given implantation energy (G).
+        """
+
+        return self.gle.screening_profile(
+            z,
+            applied_field_G,
+            dead_layer_nm,
+            surface_penetration_depth_nm,
+            bulk_penetration_depth_nm,
+            diffusion_length_nm,
+            demagnetization_factor,
+        ) * self.stopping_distribution(z, energy_keV)
+
+    @override
+    def calculate_mean_field(
+        self,
+        energy_keV: float,
+        applied_field_G: Annotated[float, 0:None],
+        dead_layer_nm: Annotated[float, 0:None],
+        surface_penetration_depth_nm: Annotated[float, 0:None],
+        bulk_penetration_depth_nm: Annotated[float, 0:None],
+        diffusion_length_nm: Annotated[float, 0:None],
+        demagnetization_factor: Annotated[float, 0:1] = 0.0,
+    ) -> float:
+        """Calculate average magnetic field at a given implantation energy.
+
+        Args:
+            energy_keV: Implantation energy (keV).
+            applied_field_G: Applied magnetic field (G).
+            dead_layer_nm: Non-superconducting dead layer (nm).
+            surface_penetration_depth_nm: Magnetic penetration depth at the surface (nm).
+            bulk_penetration_depth_nm: Magnetic penetration depth in the bulk (nm).
+            diffusion_length_nm: Length of inhomogenous defect region (nm).
+            demagnetization_factor: Effective demagnetization factor.
+
+        Returns:
+            The average magnetic field at a given implantation energy (G).
+        """
+
+        # do the numeric integration using adaptive Gaussian quadrature
+        # https://docs.scipy.org/doc/scipy/reference/generated/scipy.integrate.quad.html
+        result, _ = integrate.quad(
+            self.mean_field_integrand,
+            0.0,  # lower integration limit
+            max(  # upper integration limit
+                np.max(self.z_max_1(energy_keV)), np.max(self.z_max_2(energy_keV))
+            ),
+            args=(
+                energy_keV,
+                applied_field_G,
+                dead_layer_nm,
+                surface_penetration_depth_nm,
+                bulk_penetration_depth_nm,
+                diffusion_length_nm,
+                demagnetization_factor,
+            ),
+            epsabs=np.sqrt(np.finfo(float).eps),  # absolute error tolerance
+            epsrel=np.sqrt(np.finfo(float).eps),  # relative error tolerance
+            limit=np.iinfo(np.int32).max,  # maximum number of subintervals
+            points=[  # potential singularities/discontinuities in the integrand
+                0.0,
+                dead_layer_nm,
+                self.z_max_1(energy_keV),
+                self.z_max_2(energy_keV),
+            ],
+        )
+
+        return result
+
+    @override
+    def __call__(
+        self,
+        energy_keV: Sequence[float],
+        applied_field_G: Annotated[float, 0:None],
+        dead_layer_nm: Annotated[float, 0:None],
+        surface_penetration_depth_nm: Annotated[float, 0:None],
+        bulk_penetration_depth_nm: Annotated[float, 0:None],
+        diffusion_length_nm: Annotated[float, 0:None],
+        demagnetization_factor: Annotated[float, 0:1] = 0.0,
+    ) -> float:
+        """Calculate average magnetic field at a given implantation energy.
+
+        Functor version!
+
+        Args:
+            energy_keV: Implantation energy (keV).
+            applied_field_G: Applied magnetic field (G).
+            dead_layer_nm: Non-superconducting dead layer (nm).
+            surface_penetration_depth_nm: Magnetic penetration depth at the surface (nm).
+            bulk_penetration_depth_nm: Magnetic penetration depth in the bulk (nm).
+            diffusion_length_nm: Length of inhomogenous defect region (nm).
+            demagnetization_factor: Effective demagnetization factor.
+
+        Returns:
+            The average magnetic field at a given implantation energy (G).
+        """
+
+        # make everything numpy arrays
+        energy_keV = np.asarray(energy_keV)
+        results = np.empty(energy_keV.size)
+
+        for i, e_keV in enumerate(energy_keV):
+            results[i] = self.calculate_mean_field(
+                e_keV,
+                applied_field_G,
+                dead_layer_nm,
+                surface_penetration_depth_nm,
+                bulk_penetration_depth_nm,
+                diffusion_length_nm,
+                demagnetization_factor,
+            )
+        return results
```

### Comparing `hyperfine-0.0.2/hyperfine/superconductivity/__init__.py` & `hyperfine-0.0.3/hyperfine/superconductivity/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from . import bcs, pippard, interpolation, intertype, gle
+"""Superconductivity-related formulas.
+"""
+
+from . import bcs, pippard, interpolation, intertype, london, ccf
 import numpy as np
 
 
 def get_penetration_depth_at_0K(
     penetration_depth_nm: float,
     penetration_depth_error_nm: float,
     temperature_K: float,
```

### Comparing `hyperfine-0.0.2/hyperfine/superconductivity/bcs.py` & `hyperfine-0.0.3/hyperfine/superconductivity/bcs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+"""Expressions from Bardeen-Cooper-Schrieffer (BCS) theory for nonlocal field screening.
+
+J. Bardeen, L. N. Cooper, and J. R. Schrieffer,
+Theory of Superconductivity,
+Phys. Rev. 108, 1175 (1957).
+https://doi.org/10.1103/PhysRev.108.1175
+
+J. Halbritter,
+On the penetration of the magnetic field into a superconductor,
+Z. Physik 243, 201–219 (1971).
+https://doi.org/10.1007/BF01394851
+"""
+
 from typing import Annotated, Callable, Optional, Sequence
 import numpy as np
 from scipy import constants, integrate
 from .interpolation import gap_cos_eV
 
 
 def _a(
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hyperfine-0.0.2/hyperfine/superconductivity/interpolation.py` & `hyperfine-0.0.3/hyperfine/superconductivity/interpolation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""Interpolation formulas.
+
+Common interpolation formulas used in superconductivity as:
+* Phenomenological models describing (universal) data trends.
+* Analytic approximations for theoretical expressions whose solutions must be derived numerically.
+"""
+
 from typing import Annotated, Callable, Optional, Sequence
 import numpy as np
 
 
 def gap_cos_eV(
     T: Annotated[Sequence[float], 0.0:None],
     T_c: Annotated[float, 0.0:None],
```

### Comparing `hyperfine-0.0.2/hyperfine/superconductivity/intertype.py` & `hyperfine-0.0.3/hyperfine/superconductivity/intertype.py`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.2/.gitignore` & `hyperfine-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.2/LICENSE` & `hyperfine-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.2/README.md` & `hyperfine-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.2/pyproject.toml` & `hyperfine-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hyperfine-0.0.2/PKG-INFO` & `hyperfine-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hyperfine
-Version: 0.0.2
+Version: 0.0.3
 Project-URL: Homepage, https://github.com/rmlmcfadden/hyperfine
 Project-URL: Documentation, https://hyperfine.readthedocs.io/
 Project-URL: Repository, https://github.com/rmlmcfadden/hyperfine.git
 Project-URL: Issues, https://github.com/rmlmcfadden/hyperfine/issues
 Author-email: "Ryan M. L. McFadden" <rmlm@triumf.ca>
 License-Expression: MIT
 License-File: LICENSE
```


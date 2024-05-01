# Comparing `tmp/salamander_learn-0.3.2.tar.gz` & `tmp/salamander_learn-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salamander_learn-0.3.2.tar", max compression
+gzip compressed data, was "salamander_learn-0.4.0.tar", max compression
```

## Comparing `salamander_learn-0.3.2.tar` & `salamander_learn-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,22 @@
--rw-r--r--   0        0        0     1091 2023-10-08 04:31:09.634064 salamander_learn-0.3.2/LICENSE
--rw-r--r--   0        0        0     2147 2023-12-21 02:00:44.373048 salamander_learn-0.3.2/README.md
--rw-r--r--   0        0        0      973 2024-01-03 16:17:18.698101 salamander_learn-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      513 2024-01-03 16:17:18.698101 salamander_learn-0.3.2/src/salamander/__init__.py
--rw-r--r--   0        0        0     3166 2023-10-10 17:36:04.452813 salamander_learn-0.3.2/src/salamander/consts.py
--rw-r--r--   0        0        0        3 2023-09-26 18:20:20.939787 salamander_learn-0.3.2/src/salamander/nmf_framework/__init__.py
--rw-r--r--   0        0        0     9203 2024-01-03 11:55:39.653124 salamander_learn-0.3.2/src/salamander/nmf_framework/_utils_corrnmf.py
--rw-r--r--   0        0        0     9002 2023-10-30 04:20:35.646783 salamander_learn-0.3.2/src/salamander/nmf_framework/_utils_klnmf.py
--rw-r--r--   0        0        0    18631 2024-01-03 16:17:18.698101 salamander_learn-0.3.2/src/salamander/nmf_framework/corrnmf.py
--rw-r--r--   0        0        0     9519 2024-01-03 16:17:18.698101 salamander_learn-0.3.2/src/salamander/nmf_framework/corrnmf_det.py
--rw-r--r--   0        0        0     5820 2023-10-31 18:41:05.591631 salamander_learn-0.3.2/src/salamander/nmf_framework/initialization.py
--rw-r--r--   0        0        0     8388 2024-01-03 16:17:18.698101 salamander_learn-0.3.2/src/salamander/nmf_framework/klnmf.py
--rwxr-xr-x   0        0        0    25809 2024-01-03 16:17:18.698101 salamander_learn-0.3.2/src/salamander/nmf_framework/multimodal_corrnmf.py
--rw-r--r--   0        0        0     7599 2023-12-21 02:00:44.373048 salamander_learn-0.3.2/src/salamander/nmf_framework/mvnmf.py
--rw-r--r--   0        0        0     8454 2024-01-03 16:17:18.698101 salamander_learn-0.3.2/src/salamander/nmf_framework/nmf.py
--rw-r--r--   0        0        0    16357 2024-01-03 16:17:18.698101 salamander_learn-0.3.2/src/salamander/nmf_framework/signature_nmf.py
--rw-r--r--   0        0        0    19700 2023-12-21 03:37:16.906965 salamander_learn-0.3.2/src/salamander/plot.py
--rw-r--r--   0        0        0     3129 2023-10-31 18:26:07.377838 salamander_learn-0.3.2/src/salamander/utils.py
--rw-r--r--   0        0        0     3145 1970-01-01 00:00:00.000000 salamander_learn-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-10-08 04:31:09.634064 salamander_learn-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2147 2023-12-21 02:00:44.373048 salamander_learn-0.4.0/README.md
+-rw-r--r--   0        0        0     1075 2024-05-01 04:04:13.076830 salamander_learn-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      361 2024-05-01 03:58:25.637316 salamander_learn-0.4.0/src/salamander/__init__.py
+-rw-r--r--   0        0        0     3166 2023-10-10 17:36:04.452813 salamander_learn-0.4.0/src/salamander/consts.py
+-rw-r--r--   0        0        0        3 2023-09-26 18:20:20.939787 salamander_learn-0.4.0/src/salamander/initialization/__init__.py
+-rw-r--r--   0        0        0    15419 2024-04-30 20:56:45.838201 salamander_learn-0.4.0/src/salamander/initialization/initialize.py
+-rw-r--r--   0        0        0     4345 2024-04-23 20:18:44.627278 salamander_learn-0.4.0/src/salamander/initialization/methods.py
+-rw-r--r--   0        0        0      251 2024-04-29 19:11:36.770386 salamander_learn-0.4.0/src/salamander/models/__init__.py
+-rw-r--r--   0        0        0    12338 2024-04-29 21:31:58.001850 salamander_learn-0.4.0/src/salamander/models/_utils_corrnmf.py
+-rw-r--r--   0        0        0     9270 2024-04-23 22:15:45.379682 salamander_learn-0.4.0/src/salamander/models/_utils_klnmf.py
+-rw-r--r--   0        0        0     7977 2024-05-01 03:11:23.599717 salamander_learn-0.4.0/src/salamander/models/corrnmf.py
+-rw-r--r--   0        0        0     6012 2024-04-29 21:55:04.012896 salamander_learn-0.4.0/src/salamander/models/corrnmf_det.py
+-rw-r--r--   0        0        0     5005 2024-04-29 19:15:29.940852 salamander_learn-0.4.0/src/salamander/models/klnmf.py
+-rw-r--r--   0        0        0    25340 2024-05-01 03:11:23.599717 salamander_learn-0.4.0/src/salamander/models/mmcorrnmf.py
+-rw-r--r--   0        0        0     6502 2024-04-29 19:15:29.944852 salamander_learn-0.4.0/src/salamander/models/mvnmf.py
+-rw-r--r--   0        0        0    20245 2024-04-30 20:50:17.794896 salamander_learn-0.4.0/src/salamander/models/signature_nmf.py
+-rw-r--r--   0        0        0     3073 2024-04-30 20:58:47.519140 salamander_learn-0.4.0/src/salamander/models/standard_nmf.py
+-rw-r--r--   0        0        0    23831 2024-04-30 21:10:02.971940 salamander_learn-0.4.0/src/salamander/plot.py
+-rw-r--r--   0        0        0     5137 2024-04-30 19:28:21.403318 salamander_learn-0.4.0/src/salamander/tools.py
+-rw-r--r--   0        0        0     5788 2024-04-30 19:28:21.403318 salamander_learn-0.4.0/src/salamander/utils.py
+-rw-r--r--   0        0        0     3226 1970-01-01 00:00:00.000000 salamander_learn-0.4.0/PKG-INFO
```

### Comparing `salamander_learn-0.3.2/LICENSE` & `salamander_learn-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `salamander_learn-0.3.2/README.md` & `salamander_learn-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `salamander_learn-0.3.2/pyproject.toml` & `salamander_learn-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 [tool.poetry]
 name = "salamander-learn"
-version = "0.3.2"
+version = "0.4.0"
 description = "Salamander is a non-negative matrix factorization framework for signature analysis"
 license = "MIT"
 authors = ["Benedikt Geiger"]
 maintainers = [
     "Benedikt Geiger <benedikt_geiger@hms.harvard.edu>",
 ]
 packages = [{ include = "salamander", from = "src" }]
 
 
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 adjustText = "^0.8"
+anndata = "^0.10.5"
 fastcluster = "^1.2.6"
 matplotlib = "^3.7.1"
-numba = "^0.57"
+mudata = "^0.2.3"
+numba = "^0.59"
 numpy = "^1.24.3"
 pandas = "^1.5.3"
 scikit-learn = "^1.3.0"
 scipy = "^1.10.1"
 seaborn = "^0.13.0"
 umap-learn = "^0.5.4"
 
 [tool.poetry.group.dev.dependencies]
+mypy = "^1.9"
+pandas-stubs = "^2.2.1"
 pytest = "^7.4.2"
 pre-commit = "^3.4.0"
 tox = "^4.11.3"
+types-seaborn = "^0.13.2"
 
 [tool.pytest.ini_options]
 # /site-packages/umap/__init__.py:36: DeprecationWarning: pkg_resources is deprecated as an API.
 filterwarnings = [
     "ignore::DeprecationWarning:umap.*:",
 ]
```

### Comparing `salamander_learn-0.3.2/src/salamander/consts.py` & `salamander_learn-0.4.0/src/salamander/consts.py`

 * *Files identical despite different names*

### Comparing `salamander_learn-0.3.2/src/salamander/nmf_framework/_utils_klnmf.py` & `salamander_learn-0.4.0/src/salamander/models/_utils_klnmf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,21 @@
+from __future__ import annotations
+
 import numpy as np
 from numba import njit
 from scipy.special import gammaln
 
 EPSILON = np.finfo(np.float32).eps
+GIVEN_PARAMETERS_ALLOWED = ["asignatures"]
 
 
 @njit(fastmath=True)
-def kl_divergence(X: np.ndarray, W: np.ndarray, H: np.ndarray, weights=None) -> float:
+def kl_divergence(
+    X: np.ndarray, W: np.ndarray, H: np.ndarray, weights: np.ndarray | None = None
+) -> float:
     r"""
     The generalized Kullback-Leibler divergence
     D_KL(X || WH) = \sum_vd X_vd * ln(X_vd / (WH)_vd) - \sum_vd X_vd + \sum_vd (WH)_vd.
 
     Parameters
     ----------
     X : np.ndarray of shape (n_features, n_samples)
@@ -47,15 +52,15 @@
 
         result += summand_sample
 
     return result
 
 
 def samplewise_kl_divergence(
-    X: np.ndarray, W: np.ndarray, H: np.ndarray, weights=None
+    X: np.ndarray, W: np.ndarray, H: np.ndarray, weights: np.ndarray | None = None
 ) -> np.ndarray:
     """
     Per sample (weighted) generalized Kullback-Leibler divergence D_KL(x || Wh).
 
     Parameters
     ----------
     X : np.ndarray of shape (n_features, n_samples)
@@ -157,15 +162,15 @@
 
 
 @njit
 def update_W(
     X: np.ndarray,
     W: np.ndarray,
     H: np.ndarray,
-    weights_kl=None,
+    weights_kl: np.ndarray | None = None,
     n_given_signatures: int = 0,
 ) -> np.ndarray:
     """
     The multiplicative update rule of the signature matrix W
     under the constraint of normalized signatures. It can be shown
     that the generalized KL-divegence D_KL(X || WH) is decreasing
     under the implemented update rule.
@@ -210,15 +215,19 @@
     W_updated[:, n_given_signatures:] = W_updated[:, n_given_signatures:].clip(EPSILON)
 
     return W_updated
 
 
 @njit
 def update_H(
-    X: np.ndarray, W: np.ndarray, H: np.ndarray, weights_kl=None, weights_l_half=None
+    X: np.ndarray,
+    W: np.ndarray,
+    H: np.ndarray,
+    weights_kl: np.ndarray | None = None,
+    weights_l_half: np.ndarray | None = None,
 ) -> np.ndarray:
     """
     The multiplicative update rule of the exposure matrix H
     under the constraint of normalized signatures.
 
     Clipping the matrix avoids floating point errors.
 
@@ -270,18 +279,18 @@
 
 
 @njit
 def update_WH(
     X: np.ndarray,
     W: np.ndarray,
     H: np.ndarray,
-    weights_kl=None,
-    weights_l_half=None,
+    weights_kl: np.ndarray | None = None,
+    weights_l_half: np.ndarray | None = None,
     n_given_signatures: int = 0,
-) -> np.ndarray:
+) -> tuple[np.ndarray, np.ndarray]:
     """
     A joint update rule for the signature matrix W and
     the exposure matrix H under the constraint of normalized
     signatures.
 
     Clipping the matrix avoids floating point errors.
```

### Comparing `salamander_learn-0.3.2/src/salamander/nmf_framework/multimodal_corrnmf.py` & `salamander_learn-0.4.0/src/salamander/models/mmcorrnmf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,794 +1,739 @@
 """
-Multimodal correlated NMF (MultiCorrNMF) fits multiple correlated NMF (CorrNMF)
-models jointly in the following manner:
-Assuming that the input data for each modality originates from the identical samples,
-MultiCorrNMF fixes the sample embeddings accross modalities and learns signature
-embeddings for all modalities in the same embedding space.
+Multimodal correlated NMF fits multiple correlated NMF models jointly.
+
+Assuming that the input data of each modality originates from the identical samples,
+multimodal correlated NMF fixes the sample embeddings accross modalities and learns
+signature embeddings of all modalities in a shared embedding space.
 """
-# This implementation heavily relies on the implementaion of CorrNMF in
-# corrnmf_det.py. In particular, CorrNMFDet methods with a leading '_'
-# are accessed.
-# pylint: disable=protected-access
 
+from __future__ import annotations
+
+import warnings
+from typing import TYPE_CHECKING, Any, Iterable, Literal
+
+import anndata as ad
 import matplotlib.pyplot as plt
+import mudata as md
 import numpy as np
 import pandas as pd
-from scipy import optimize
-from scipy.spatial.distance import squareform
 
-from ..plot import (
-    _get_sample_order,
-    corr_plot,
-    embeddings_plot,
-    history_plot,
-    signatures_plot,
-)
-from ..utils import type_checker, value_checker
+from .. import plot as pl
+from .. import tools as tl
+from ..initialization.initialize import EPSILON, _Init_methods, initialize_mmcorrnmf
+from ..utils import dict_checker, type_checker, value_checker
 from . import _utils_corrnmf
-from .corrnmf_det import CorrNMFDet
+from ._utils_klnmf import samplewise_kl_divergence, update_W
 
-EPSILON = np.finfo(np.float32).eps
+if TYPE_CHECKING:
+    from matplotlib.axes import Axes
+    from matplotlib.typing import ColorType
+    from seaborn.matrix import ClusterGrid
+
+    from .signature_nmf import _Dim_reduction_methods
 
 
 class MultimodalCorrNMF:
     def __init__(
         self,
-        n_modalities,
-        ns_signatures=None,
-        dim_embeddings=None,
-        init_method="nndsvd",
-        min_iterations=500,
-        max_iterations=10000,
-        conv_test_freq=10,
-        tol=1e-7,
+        ns_signatures: list[int],
+        dim_embeddings: int | None = None,
+        init_method: _Init_methods = "nndsvd",
+        min_iterations: int = 500,
+        max_iterations: int = 10000,
+        conv_test_freq: int = 10,
+        tol: float = 1e-7,
     ):
-        self.n_modalities = n_modalities
-
-        if ns_signatures is None:
-            ns_signatures = np.ones(n_modalities, dtype=int)
-
         self.ns_signatures = ns_signatures
 
         if dim_embeddings is None:
             dim_embeddings = np.max(ns_signatures)
 
         self.dim_embeddings = dim_embeddings
         self.init_method = init_method
         self.min_iterations = min_iterations
         self.max_iterations = max_iterations
         self.conv_test_freq = conv_test_freq
         self.tol = tol
-        self.models = [
-            CorrNMFDet(n_signatures, dim_embeddings, init_method)
-            for n_signatures in ns_signatures
-        ]
+        self.variance = 1.0
 
         # initialize data/fitting dependent attributes
-        self.modality_names = np.empty(n_modalities, dtype=str)
-        self.n_samples = 0
-        self.history = {}
+        mod_names_default = [f"mod{n}" for n in range(1, len(ns_signatures) + 1)]
+        self.mdata = md.MuData(
+            {mod_name: ad.AnnData() for mod_name in mod_names_default}
+        )
+        self.asignatures = {mod_name: ad.AnnData() for mod_name in mod_names_default}
+        self.history: dict[str, Any] = {}
+        self.signature_correlation = np.empty((sum(ns_signatures), sum(ns_signatures)))
+        self.signature_correlation[:] = np.nan
 
     @property
-    def signatures(self) -> dict:
-        return {
-            name: model.signatures
-            for name, model in zip(self.modality_names, self.models)
-        }
+    def mod_names(self) -> list[str]:
+        return list(self.mdata.mod.keys())
 
     @property
-    def exposures(self) -> dict:
+    def mutation_types(self) -> dict[str, list[str]]:
         return {
-            name: model.exposures
-            for name, model in zip(self.modality_names, self.models)
+            mod_name: list(adata.var_names)
+            for mod_name, adata in self.mdata.mod.items()
         }
 
     @property
-    def data_reconstructed(self) -> dict:
+    def signature_names(self) -> dict[str, list[str]]:
         return {
-            name: model.data_reconstructred
-            for name, model in zip(self.modality_names, self.models)
+            mod_name: list(asigs.obs_names)
+            for mod_name, asigs in self.asignatures.items()
         }
 
     @property
-    def Xs_reconstructed(self) -> np.ndarray:
-        return {
-            name: model.X_reconstructed
-            for name, model in zip(self.modality_names, self.models)
-        }
+    def sample_names(self) -> list[str]:
+        return list(self.mdata.obs_names)
 
     @property
-    def reconstruction_errors(self) -> float:
-        return {
-            name: model.reconstruction_error
-            for name, model in zip(self.modality_names, self.models)
-        }
+    def signatures(self) -> dict[str, pd.DataFrame]:
+        return {mod_name: asigs.to_df() for mod_name, asigs in self.asignatures.items()}
+
+    @property
+    def exposures(self) -> dict[str, pd.DataFrame]:
+        exposures_all = {}
+        for mod_name in self.mod_names:
+            exposures_all[mod_name] = pd.DataFrame(
+                self.mdata[mod_name].obsm["exposures"],
+                index=self.sample_names,
+                columns=self.asignatures[mod_name].obs_names,
+            )
+        return exposures_all
+
+    def compute_exposures(self) -> None:
+        for mod_name in self.mod_names:
+            adata = self.mdata[mod_name]
+            asigs = self.asignatures[mod_name]
+            adata.obsm["exposures"] = _utils_corrnmf.compute_exposures(
+                asigs.obs["scalings"].values,
+                adata.obs["scalings"].values,
+                asigs.obsm["embeddings"],
+                self.mdata.obsm["embeddings"],
+            )
+
+    def compute_reconstruction(self) -> None:
+        for mod_name in self.mod_names:
+            adata = self.mdata[mod_name]
+            asigs = self.asignatures[mod_name]
+            adata.obsm["X_reconstructed"] = adata.obsm["exposures"] @ asigs.X
+
+    @property
+    def data_reconstructed(self) -> dict[str, pd.DataFrame]:
+        for adata in self.mdata.mod.values():
+            if "X_reconstructed" not in adata.obsm:
+                self.compute_reconstruction()
+
+        data_reconstructed_all = {}
+        for mod_name, adata in self.mdata.mod.items():
+            data_reconstructed_all[mod_name] = pd.DataFrame(
+                adata.obsm["X_reconstructed"],
+                index=adata.obs_names,
+                columns=adata.var_names,
+            )
+        return data_reconstructed_all
+
+    def compute_reconstruction_errors(self) -> None:
+        self.compute_exposures()
+
+        for mod_name in self.mod_names:
+            adata = self.mdata[mod_name]
+            asigs = self.asignatures[mod_name]
+            errors = samplewise_kl_divergence(
+                adata.X.T, asigs.X.T, adata.obsm["exposures"].T
+            )
+            adata.obs["reconstruction_error"] = errors
+
+        self.mdata.update()
 
     @property
-    def samplewise_reconstruction_errors(self) -> np.ndarray:
+    def reconstruction_errors(self) -> dict[str, float]:
+        if any(
+            "reconstruction_error" not in self.mdata[mod_name].obs
+            for mod_name in self.mod_names
+        ):
+            self.compute_reconstruction_errors()
+
         return {
-            name: model.samplewise_reconstruction_error
-            for name, model in zip(self.modality_names, self.models)
+            mod_name: np.sum(adata.obs["reconstruction_error"])
+            for mod_name, adata in self.mdata.mod.items()
         }
 
+    @property
+    def reconstruction_error(self) -> float:
+        return np.sum(list(self.reconstruction_errors.values()))
+
     def objective_function(self) -> float:
         """
-        The objective function to be optimized during fitting.
+        The ELBO of multimodal correlated NMF.
         """
-        elbo = np.sum(
-            [
-                model.objective_function(penalize_sample_embeddings=False)
-                for model in self.models
-            ]
-        )
+        elbo = 0.0
+
+        for mod_name in self.mod_names:
+            adata = self.mdata[mod_name]
+            asigs = self.asignatures[mod_name]
+            elbo += _utils_corrnmf.elbo_corrnmf(
+                adata.X,
+                asigs.X,
+                adata.obsm["exposures"],
+                asigs.obsm["embeddings"],
+                self.mdata.obsm["embeddings"],
+                self.variance,
+                penalize_sample_embeddings=False,
+            )
+
         elbo -= (
             0.5
             * self.dim_embeddings
-            * self.n_samples
-            * np.log(2 * np.pi * self.models[0].sigma_sq)
+            * self.mdata.n_obs
+            * np.log(2 * np.pi * self.variance)
         )
-        elbo -= np.sum(self.models[0].U ** 2) / (2 * self.models[0].sigma_sq)
+        elbo -= np.sum(self.mdata.obsm["embeddings"] ** 2) / (2 * self.variance)
         return elbo
 
     @property
-    def objective(self) -> str:
+    def objective(self) -> Literal["minimize", "maximize"]:
         return "maximize"
 
-    def _surrogate_objective_function(self) -> float:
-        """
-        The surrogate lower bound of the ELBO.
-        """
-        ps = self._update_ps()
-        sof_value = np.sum(
-            [
-                model._surrogate_objective_function(penalize_sample_embeddings=False)
-                for model, p in zip(self.models, ps)
-            ]
-        )
-        sof_value -= (
-            0.5
-            * self.dim_embeddings
-            * self.n_samples
-            * np.log(2 * np.pi * self.models[0].sigma_sq)
-        )
-        sof_value -= np.sum(self.models[0].U ** 2) / (2 * self.models[0].sigma_sq)
-        return sof_value
-
-    def loglikelihood(self) -> float:
-        """
-        The log-likelihood of the underlying generative model.
-        """
-        return self.objective_function()
+    def _setup_mdata(self, mdata: md.MuData):
+        type_checker("mdata", mdata, md.MuData)
+        n_mod_expected = len(self.ns_signatures)
 
-    @property
-    def _n_parameters(self) -> int:
-        n_parameters_signatures = np.sum(
-            [model.n_features * model.n_signatures for model in self.models]
-        )
-        n_parameters_embeddings = self.dim_embeddings * (
-            np.sum(self.ns_signatures) + self.n_samples
-        )
-        n_parameters_biases = self.n_modalities * self.n_samples + np.sum(
-            self.ns_signatures
-        )
-        n_parameters_exposures = n_parameters_embeddings + n_parameters_biases
-        n_parameters = n_parameters_signatures + n_parameters_exposures + 1
+        if mdata.n_mod != n_mod_expected:
+            raise ValueError(f"The data has to have {n_mod_expected} many modalities.")
 
-        return n_parameters
+        sample_names_expected = list(mdata.mod.values())[0].obs_names
 
-    @property
-    def bic(self) -> float:
-        return self._n_parameters * np.log(self.n_samples) - 2 * self.loglikelihood()
-
-    def _update_alphas(self, given_sample_biases):
-        for model, given_sam_biases in zip(self.models, given_sample_biases):
-            model._update_alpha(given_sam_biases)
-
-    def _update_betas(self, ps, given_signature_biases):
-        for model, p, given_sig_biases in zip(self.models, ps, given_signature_biases):
-            model._update_beta(p, given_sig_biases)
-
-    def _update_sigma_sq(self, given_variance):
-        if given_variance is None:
-            Ls = np.concatenate([model.L for model in self.models], axis=1)
-            embeddings = np.concatenate([Ls, self.models[0].U], axis=1)
-            sigma_sq = np.mean(embeddings**2)
-            sigma_sq = np.clip(sigma_sq, EPSILON, None)
-
-            for model in self.models:
-                model.sigma_sq = sigma_sq
-
-    def _update_Ws(self):
-        for model in self.models:
-            if model.n_given_signatures < model.n_signatures:
-                model._update_W()
-
-    def _update_ps(self):
-        return [model._update_p() for model in self.models]
-
-    def _objective_fun_u(self, u, index, aux_cols):
-        sigma_sq = self.models[0].sigma_sq
-        s = -np.sum(
-            [
-                _utils_corrnmf.objective_function_embedding(
-                    u,
-                    model.L,
-                    model.alpha[index],
-                    model.beta,
-                    sigma_sq,
-                    aux_col,
-                    add_penalty=False,
-                )
-                for model, aux_col in zip(self.models, aux_cols)
-            ]
-        )
-        s -= np.dot(u, u) / (2 * sigma_sq)
-        return -s
-
-    def _gradient_u(self, u, index, s_grads):
-        sigma_sq = self.models[0].sigma_sq
-        s = -np.sum(
-            [
-                _utils_corrnmf.gradient_embedding(
-                    u,
-                    model.L,
-                    model.alpha[index],
-                    model.beta,
-                    sigma_sq,
-                    s_grad,
-                    add_penalty=False,
-                )
-                for model, s_grad in zip(self.models, s_grads)
-            ],
-            axis=0,
-        )
-        s -= u / sigma_sq
-        return -s
-
-    def _hessian_u(self, u, index, outer_prods_Ls):
-        sigma_sq = self.models[0].sigma_sq
-        s = -np.sum(
-            [
-                _utils_corrnmf.hessian_embedding(
-                    u,
-                    model.L,
-                    model.alpha[index],
-                    model.beta,
-                    sigma_sq,
-                    outer_prods_L,
-                    add_penalty=False,
+        for adata in mdata.mod.values():
+            if not all(adata.obs_names == sample_names_expected):
+                raise ValueError(
+                    "The sample names of the different modalities are not identical."
                 )
-                for model, outer_prods_L in zip(self.models, outer_prods_Ls)
-            ],
-            axis=0,
-        )
-        s -= np.diag(np.full(self.dim_embeddings, 1 / sigma_sq))
-        return -s
-
-    def _update_u(self, index, aux_cols, outer_prods_Ls):
-        def objective_fun(u):
-            return self._objective_fun_u(u, index, aux_cols)
-
-        s_grads = np.array(
-            [
-                np.sum(aux_col * model.L, axis=1)
-                for model, aux_col in zip(self.models, aux_cols)
-            ]
-        )
 
-        def gradient(u):
-            return self._gradient_u(u, index, s_grads)
+        self.mdata = mdata
 
-        def hessian(u):
-            return self._hessian_u(u, index, outer_prods_Ls)
-
-        u = optimize.minimize(
-            fun=objective_fun,
-            x0=self.models[0].U[:, index],
-            method="Newton-CG",
-            jac=gradient,
-            hess=hessian,
-            options={"maxiter": 3},
-        ).x
-        u[(0 < u) & (u < EPSILON)] = EPSILON
-        u[(-EPSILON < u) & (u < 0)] = -EPSILON
-
-        for model in self.models:
-            model.U[:, index] = u
-
-    def _update_U(self, auxs):
-        outer_prods_Ls = [
-            np.einsum("mK,nK->Kmn", model.L, model.L) for model in self.models
-        ]
-
-        for d in range(self.n_samples):
-            aux_cols = [aux[:, d] for aux in auxs]
-            self._update_u(d, aux_cols, outer_prods_Ls)
-
-    def _update_Ls(self, auxs, outer_prods_U, given_signature_embeddings):
-        for model, aux, given_sig_embs in zip(
-            self.models, auxs, given_signature_embeddings
-        ):
-            if given_sig_embs is None:
-                model._update_L(aux, outer_prods_U)
-
-    def _update_LsU(self, ps, given_signature_embeddings, given_sample_embeddings):
-        auxs = [
-            np.einsum("vd,vkd->kd", model.X, p) for model, p in zip(self.models, ps)
-        ]
-        outer_prods_U = np.einsum("mD,nD->Dmn", self.models[0].U, self.models[0].U)
-        self._update_Ls(auxs, outer_prods_U, given_signature_embeddings)
+    def _initialize(
+        self,
+        given_parameters: dict[str, Any] | None = None,
+        init_kwargs: dict[str, Any] | None = None,
+    ) -> None:
+        init_kwargs = {} if init_kwargs is None else init_kwargs.copy()
+        self.asignatures, self.variance = initialize_mmcorrnmf(
+            self.mdata,
+            self.ns_signatures,
+            self.dim_embeddings,
+            self.init_method,
+            given_parameters,
+            **init_kwargs,
+        )
+        self.compute_exposures()
+
+    def _compute_auxs(self) -> dict[str, np.ndarray]:
+        r"""
+        auxs: dict[str, np.ndarray]
+            For every modality
+                aux_kd = \sum_v X_vd * p_vkd
+            is used for updating the signatures and the sample embeddidngs.
+        """
+        auxs = {}
+        for mod_name in self.mod_names:
+            adata = self.mdata[mod_name]
+            asigs = self.asignatures[mod_name]
+            auxs[mod_name] = _utils_corrnmf.compute_aux(
+                adata.X, asigs.X, adata.obsm["exposures"]
+            )
+        return auxs
 
-        if given_sample_embeddings is None:
-            self._update_U(auxs)
+    def update_sample_scalings_mod(
+        self, mod_name: str, given_parameters_mod: dict[str, Any]
+    ) -> None:
+        if "sample_scalings" not in given_parameters_mod:
+            adata = self.mdata[mod_name]
+            asigs = self.asignatures[mod_name]
+            adata.obs["scalings"] = _utils_corrnmf.update_sample_scalings(
+                adata.X,
+                asigs.obs["scalings"].values,
+                asigs.obsm["embeddings"],
+                self.mdata.obsm["embeddings"],
+            )
 
-    def _setup_data_parameters(self, data: list):
-        type_checker("data", data, list)
+    def update_sample_scalings(
+        self,
+        given_parameters: dict[str, Any] | None = None,
+    ) -> None:
+        if given_parameters is None:
+            given_parameters = {}
+
+        for mod_name in self.mod_names:
+            if mod_name in given_parameters:
+                given_parameters_mod = given_parameters[mod_name]
+            else:
+                given_parameters_mod = {}
+            self.update_sample_scalings_mod(mod_name, given_parameters_mod)
 
-        if len(data) != self.n_modalities:
-            raise ValueError(
-                f"The input data has to be {self.n_modalities} "
-                "many named pandas dataframes."
+    def update_signature_scalings_mod(
+        self, mod_name: str, aux: np.ndarray, given_parameters_mod: dict[str, Any]
+    ) -> None:
+        if "signature_scalings" not in given_parameters_mod:
+            asigs = self.asignatures[mod_name]
+            asigs.obs["scalings"] = _utils_corrnmf.update_signature_scalings(
+                aux,
+                self.mdata[mod_name].obs["scalings"].values,
+                asigs.obsm["embeddings"],
+                self.mdata.obsm["embeddings"],
             )
 
-        for df in data:
-            type_checker("input dataframe", df, pd.DataFrame)
+    def update_signature_scalings(
+        self,
+        auxs: dict[str, np.ndarray],
+        given_parameters: dict[str, Any] | None = None,
+    ) -> None:
+        if given_parameters is None:
+            given_parameters = {}
+
+        for mod_name in self.mod_names:
+            if mod_name in given_parameters:
+                given_parameters_mod = given_parameters[mod_name]
+            else:
+                given_parameters_mod = {}
+            self.update_signature_scalings_mod(
+                mod_name, auxs[mod_name], given_parameters_mod
+            )
 
-            if df.index.name is None:
-                raise ValueError(
-                    "You have to set 'df.index.name' to a "
-                    "meaningful name for every input dataframe."
-                )
+    def update_variance(self, given_parameters: dict[str, Any] | None = None) -> None:
+        if given_parameters is None:
+            given_parameters = {}
+
+        if "variance" not in given_parameters:
+            signature_embeddings = np.concatenate(
+                [asigs.obsm["embeddings"] for asigs in self.asignatures.values()]
+            )
+            embeddings = np.concatenate(
+                [signature_embeddings, self.mdata.obsm["embeddings"]]
+            )
+            variance = np.mean(embeddings**2)
+            self.variance = np.clip(variance, EPSILON, None)
 
-        self.modality_names = np.array([df.index.name for df in data])
-        self.n_samples = data[0].shape[1]
+    def update_signatures_mod(
+        self, mod_name: str, given_parameters_mod: dict[str, Any]
+    ) -> None:
+        if "asignatures" in given_parameters_mod:
+            n_given_signatures = given_parameters_mod["asignatures"].n_obs
+        else:
+            n_given_signatures = 0
 
-        for model, df in zip(self.models, data):
-            model._setup_data_parameters(df)
+        asigs = self.asignatures[mod_name]
+        W = update_W(
+            self.mdata[mod_name].X.T,
+            asigs.X.T,
+            self.mdata[mod_name].obsm["exposures"].T,
+            n_given_signatures=n_given_signatures,
+        )
+        asigs.X = W.T
+
+    def update_signatures(self, given_parameters: dict[str, Any] | None = None) -> None:
+        if given_parameters is None:
+            given_parameters = {}
+
+        for mod_name in self.mod_names:
+            if mod_name in given_parameters:
+                given_parameters_mod = given_parameters[mod_name]
+            else:
+                given_parameters_mod = {}
+            self.update_signatures_mod(mod_name, given_parameters_mod)
 
-    def _initialize(
+    def update_signature_embeddings_mod(
         self,
-        given_signatures=None,
-        given_signature_biases=None,
-        given_signature_embeddings=None,
-        given_sample_biases=None,
-        given_sample_embeddings=None,
-        given_variance=None,
-        init_kwargs=None,
-    ):
-        if given_signatures is None:
-            given_signatures = [None for _ in range(self.n_modalities)]
-
-        if given_variance is None:
-            variance = 1.0
-        else:
-            variance = given_variance
-
-        if given_signature_biases is None:
-            given_signature_biases = [None for _ in range(self.n_modalities)]
+        mod_name: str,
+        aux: np.ndarray,
+        outer_prods_sample_embeddings: np.ndarray,
+        given_parameters_mod: dict[str, Any],
+    ) -> None:
+        if "signature_embeddings" not in given_parameters_mod:
+            asigs = self.asignatures[mod_name]
+            for k, aux_row in enumerate(aux):
+                embedding_init = asigs.obsm["embeddings"][k, :]
+                asigs.obsm["embeddings"][k, :] = _utils_corrnmf.update_embedding(
+                    embedding_init,
+                    self.mdata.obsm["embeddings"],
+                    asigs.obs["scalings"][k],
+                    self.mdata[mod_name].obs["scalings"].values,
+                    self.variance,
+                    aux_row,
+                    outer_prods_sample_embeddings,
+                )
 
-        if given_signature_embeddings is None:
-            given_signature_embeddings = [None for _ in range(self.n_modalities)]
+    def update_signature_embeddings(
+        self,
+        auxs: dict[str, np.ndarray],
+        given_parameters: dict[str, Any] | None = None,
+    ) -> None:
+        """
+        Update all signature embeddings by optimizing
+        the surrogate objective function using scipy.optimize.minimize
+        with the 'Newton-CG' method.
+        """
+        if given_parameters is None:
+            given_parameters = {}
+
+        outer_prods_sample_embeddings = np.einsum(
+            "Dm,Dn->Dmn",
+            self.mdata.obsm["embeddings"],
+            self.mdata.obsm["embeddings"],
+        )
+        for mod_name in self.mod_names:
+            if mod_name in given_parameters:
+                given_parameters_mod = given_parameters[mod_name]
+            else:
+                given_parameters_mod = {}
+            self.update_signature_embeddings_mod(
+                mod_name,
+                auxs[mod_name],
+                outer_prods_sample_embeddings,
+                given_parameters_mod,
+            )
 
-        if given_sample_biases is None:
-            given_sample_biases = [None for _ in range(self.n_modalities)]
-
-        if given_sample_embeddings is None:
-            U = np.random.multivariate_normal(
-                np.zeros(self.dim_embeddings),
-                variance * np.identity(self.dim_embeddings),
-                size=self.n_samples,
-            ).T
-        else:
-            U = given_sample_embeddings
+    def update_sample_embeddings(self, auxs: dict[str, np.ndarray]) -> None:
+        sig_embeddings = np.concatenate(
+            [asigs.obsm["embeddings"] for asigs in self.asignatures.values()]
+        )
+        outer_prods_sig_embeddings = np.einsum(
+            "Km,Kn->Kmn", sig_embeddings, sig_embeddings
+        )
+        sig_scalings = np.concatenate(
+            [asigs.obs["scalings"] for asigs in self.asignatures.values()]
+        )
+        aux = np.concatenate([aux for aux in auxs.values()])
+
+        for d, aux_col in enumerate(aux.T):
+            embedding_init = self.mdata.obsm["embeddings"][d, :]
+            scalings = [
+                np.repeat(adata.obs["scalings"][d], n_signatures)
+                for adata, n_signatures in zip(
+                    self.mdata.mod.values(), self.ns_signatures
+                )
+            ]
+            scalings = np.concatenate(scalings)
+            self.mdata.obsm["embeddings"][d, :] = _utils_corrnmf.update_embedding(
+                embedding_init,
+                sig_embeddings,
+                scalings,
+                sig_scalings,
+                self.variance,
+                aux_col,
+                outer_prods_sig_embeddings,
+                options={"maxiter": 3},
+            )
 
-        for (
-            model,
-            modality_name,
-            given_sigs,
-            given_sig_biases,
-            given_sig_embs,
-            given_sam_biases,
-        ) in zip(
-            self.models,
-            self.modality_names,
-            given_signatures,
-            given_signature_biases,
-            given_signature_embeddings,
-            given_sample_biases,
-        ):
-            model._initialize(
-                given_signatures=given_sigs,
-                given_signature_biases=given_sig_biases,
-                given_signature_embeddings=given_sig_embs,
-                given_sample_biases=given_sam_biases,
-                given_sample_embeddings=U,
-                given_variance=variance,
-                init_kwargs=init_kwargs,
-            )
-            model.signature_names = np.concatenate(
-                [
-                    model.signature_names[: model.n_given_signatures],
-                    np.char.add(
-                        modality_name + " ",
-                        model.signature_names[model.n_given_signatures :],
-                    ),
-                ]
-            )
-        return (
-            given_signature_biases,
-            given_signature_embeddings,
-            given_sample_biases,
-        )
+    def update_embeddings(
+        self,
+        auxs: dict[str, np.ndarray],
+        given_parameters: dict[str, Any] | None = None,
+    ) -> None:
+        if given_parameters is None:
+            given_parameters = {}
+
+        self.update_signature_embeddings(auxs, given_parameters)
+
+        if "sample_embeddings" not in given_parameters:
+            self.update_sample_embeddings(auxs)
+
+    def _update_parameters(self, given_parameters: dict[str, Any] | None = None):
+        if given_parameters is None:
+            given_parameters = {}
+
+        self.update_sample_scalings(given_parameters)
+        self.compute_exposures()
+        auxs = self._compute_auxs()
+        self.update_signature_scalings(auxs, given_parameters)
+        self.update_embeddings(auxs, given_parameters)
+        self.update_variance(given_parameters)
+        self.update_signatures(given_parameters)
 
     def fit(
         self,
-        data: list,
-        given_signatures=None,
-        given_signature_biases=None,
-        given_signature_embeddings=None,
-        given_sample_biases=None,
-        given_sample_embeddings=None,
-        given_variance=None,
-        init_kwargs=None,
-        history=False,
-        verbose=0,
-    ):
-        self._setup_data_parameters(data)
-        (
-            given_signature_biases,
-            given_signature_embeddings,
-            given_sample_biases,
-        ) = self._initialize(
-            given_signatures=given_signatures,
-            given_signature_biases=given_signature_biases,
-            given_signature_embeddings=given_signature_embeddings,
-            given_sample_biases=given_sample_biases,
-            given_sample_embeddings=given_sample_embeddings,
-            given_variance=given_variance,
-            init_kwargs=init_kwargs,
-        )
+        mdata: md.MuData,
+        given_parameters: dict[str, Any] | None = None,
+        init_kwargs: dict[str, Any] | None = None,
+        history: bool = True,
+        verbose: Literal[0, 1] = 0,
+        verbosity_freq: int = 100,
+    ) -> MultimodalCorrNMF:
+        self._setup_mdata(mdata)
+        self._initialize(given_parameters, init_kwargs)
         of_values = [self.objective_function()]
         n_iteration = 0
         converged = False
 
         while not converged:
             n_iteration += 1
 
-            if verbose and n_iteration % 100 == 0:
+            if verbose and n_iteration % verbosity_freq == 0:
                 print(f"iteration: {n_iteration}; objective: {of_values[-1]:.2f}")
 
-            self._update_alphas(given_sample_biases)
-            ps = self._update_ps()
-            self._update_betas(ps, given_signature_biases)
-            self._update_LsU(ps, given_signature_embeddings, given_sample_embeddings)
-            self._update_sigma_sq(given_variance)
-            self._update_Ws()
+            self._update_parameters(given_parameters)
 
             if n_iteration % self.conv_test_freq == 0:
                 prev_of_value = of_values[-1]
                 of_values.append(self.objective_function())
-                rel_change = (of_values[-1] - prev_of_value) / np.abs(prev_of_value)
+                rel_change_nominator = np.abs(prev_of_value - of_values[-1])
+                rel_change = rel_change_nominator / np.abs(prev_of_value)
                 converged = rel_change < self.tol and n_iteration >= self.min_iterations
 
             converged |= n_iteration >= self.max_iterations
 
         if history:
             self.history["objective_function"] = of_values[1:]
 
+        self.mdata.update()
         return self
 
-    def plot_history(self, ax=None, min_iteration=0, outfile=None, **kwargs):
+    def plot_history(self, outfile: str | None = None, **kwargs) -> Axes:
         if not self.history:
             raise ValueError(
                 "No history available, the model has to be fitted first. "
                 "Remember to set 'history' to 'True' when calling 'fit()'."
             )
 
-        history_plot(
-            self.history["objective_function"],
-            self.conv_test_freq,
-            min_iteration=min_iteration,
-            ax=ax,
+        ax = pl.history(
+            values=self.history["objective_function"],
+            conv_test_freq=self.conv_test_freq,
             **kwargs,
         )
-
         if outfile is not None:
             plt.savefig(outfile, bbox_inches="tight")
 
         return ax
 
     def plot_signatures(
         self,
-        colors=None,
-        annotate_mutation_types=False,
-        figsize=None,
-        outfile=None,
+        colors: dict[str, ColorType | list[ColorType]] | None = None,
+        annotate_mutation_types: bool = False,
+        figsize: tuple[float, float] | None = None,
+        outfile: str | None = None,
         **kwargs,
     ):
-        if colors is None:
-            colors = [None for _ in range(self.n_modalities)]
-
+        colors = {} if colors is None else colors.copy()
+        dict_checker("colors", colors, self.mod_names)
         max_n_signatures = np.max(self.ns_signatures)
 
         if figsize is None:
-            figsize = (8 * self.n_modalities, 2 * max_n_signatures)
+            figsize = (4 * self.mdata.n_mod, max_n_signatures)
 
-        fig, axes = plt.subplots(max_n_signatures, self.n_modalities, figsize=figsize)
+        fig, axes = plt.subplots(max_n_signatures, self.mdata.n_mod, figsize=figsize)
 
-        for axs, model, cols in zip(axes.T, self.models, colors):
-            model.plot_signatures(
+        for mod_name, axs in zip(self.mod_names, axes.T):
+            sigs = self.asignatures[mod_name]
+            cols = colors[mod_name] if mod_name in colors else None
+            n_sigs = sigs.n_obs
+            pl.barplot(
+                sigs,
                 colors=cols,
-                annotate_mutation_types=annotate_mutation_types,
-                axes=axs[: model.n_signatures],
+                annotate_vars=annotate_mutation_types,
+                axes=axs[:n_sigs],
                 **kwargs,
             )
-
-            for ax in axs[model.n_signatures :]:
+            for ax in axs[n_sigs:]:
                 fig.delaxes(ax)
 
         plt.tight_layout()
 
         if outfile is not None:
             plt.savefig(outfile, bbox_inches="tight")
 
         return axes
 
     def plot_exposures(
         self,
-        sample_order=None,
-        reorder_signatures=True,
-        annotate_samples=True,
-        colors=None,
-        ncol_legend=1,
-        axes=None,
-        outfile=None,
+        sample_order: np.ndarray | None = None,
+        reorder_signatures: bool = True,
+        annotate_samples: bool = True,
+        colors: dict[str, Iterable[ColorType]] | None = None,
+        axes: Iterable[Axes] | None = None,
+        outfile: str | None = None,
         **kwargs,
-    ):
+    ) -> Iterable[Axes]:
         """
         Visualize the exposures as a stacked bar chart,
         see plot.py for the implementation.
 
         Input:
         ------
         **kwargs:
             arguments to be passed to exposure_plot
         """
         if axes is None:
-            _, axes = plt.subplots(
-                self.n_modalities, figsize=(20, 3 * self.n_modalities)
-            )
+            _, axes = plt.subplots(self.mdata.n_mod, figsize=(20, 3 * self.mdata.n_mod))
 
-        if colors is None:
-            colors = [None for _ in range(self.n_modalities)]
+        colors = {} if colors is None else colors.copy()
+        dict_checker("colors", colors, self.mod_names)
+        exposures = self.exposures
 
         if sample_order is None:
-            all_exposures = [model.exposures for model in self.models]
-            all_exposures_normalized = pd.concat(
-                [df / df.sum(axis=0) for df in all_exposures]
+            exposures_all_normalized = pd.concat(
+                [df.div(df.sum(axis=1), axis=0) for df in exposures.values()], axis=1
             )
-            sample_order = _get_sample_order(all_exposures_normalized)
+            sample_order = pl.get_obs_order(exposures_all_normalized)
 
-        for n, (ax, model, cols) in enumerate(zip(axes, self.models, colors)):
-            if n < self.n_modalities - 1:
+        for n, (mod_name, ax) in enumerate(zip(self.mod_names, axes)):
+            expos = exposures[mod_name]
+            cols = colors[mod_name] if mod_name in colors else None
+
+            if n < self.mdata.n_mod - 1:
                 annotate = False
             else:
                 annotate = annotate_samples
 
-            ax = model.plot_exposures(
-                sample_order=sample_order,
-                reorder_signatures=reorder_signatures,
-                annotate_samples=annotate,
+            ax = pl.stacked_barplot(
+                data=expos,
+                obs_order=sample_order,
+                reorder_dimensions=reorder_signatures,
+                annotate_obs=annotate,
                 colors=cols,
-                ncol_legend=ncol_legend,
                 ax=ax,
                 **kwargs,
             )
-            ax.set_title(f"{self.modality_names[n]} signature exposures")
+            ax.set_title(f"{self.mod_names[n]} signature exposures")
 
         plt.tight_layout()
 
         if outfile is not None:
             plt.savefig(outfile, bbox_inches="tight")
 
         return axes
 
-    @property
-    def corr_signatures(self) -> pd.DataFrame:
-        Ls = np.concatenate([model.L for model in self.models], axis=1)
-        signature_names = np.concatenate(
-            [model.signature_names for model in self.models]
-        )
-        norms = np.sqrt(np.sum(Ls**2, axis=0))
-
-        corr_vector = np.array(
-            [
-                np.dot(l1, l2) / (norms[k1] * norms[k1 + k2 + 1])
-                for k1, l1 in enumerate(Ls.T)
-                for k2, l2 in enumerate(Ls[:, k1 + 1 :].T)
-            ]
+    def compute_correlation(
+        self, data: Literal["samples", "signatures"] = "signatures", **kwargs
+    ) -> None:
+        """
+        Compute the signature or sample correlation. The signature
+        correlation is stored as a new model attribute, the sample correlation
+        is stored in mdata.
+        """
+        value_checker("data", data, ["samples", "signatures"])
+
+        for adata in self.mdata.mod.values():
+            assert "exposures" in adata.obsm, (
+                "Computing the sample or signature correlation "
+                "requires fitting the NMF model."
+            )
+
+        values = np.concatenate(
+            [adata.obsm["exposures"] for adata in self.mdata.mod.values()], axis=1
         )
-        corr_matrix = squareform(corr_vector) + np.identity(np.sum(self.ns_signatures))
-        corr = pd.DataFrame(corr_matrix, index=signature_names, columns=signature_names)
 
-        return corr
+        if data == "signatures":
+            values = values.T
 
-    @property
-    def corr_samples(self) -> pd.DataFrame:
-        return self.models[0].corr_samples
+        correlation = tl.correlation_numpy(values, **kwargs)
 
-    def plot_correlation(self, data="signatures", annot=False, outfile=None, **kwargs):
-        """
-        Plot the correlation matrix of the signatures or samples.
-        See plot.py for the implementation of corr_plot.
+        if data == "samples":
+            self.mdata.obsp["X_correlation"] = correlation
+        else:
+            self.signature_correlation = correlation
 
-        Input:
-        ------
-        *args, **kwargs:
-            arguments to be passed to corr_plot
+    def correlation(
+        self, data: Literal["samples", "signatures"] = "signatures"
+    ) -> pd.DataFrame:
         """
-        value_checker("data", data, ["signatures", "samples"])
+        Dataframe of the signature or sample correlation.
+        """
+        value_checker("data", data, ["samples", "signatures"])
 
-        if data == "signatures":
-            corr = self.corr_signatures
+        if data == "samples":
+            if "X_correlation" not in self.mdata.obsp:
+                self.compute_correlation("samples")
+            values = self.mdata.obsp["X_correlation"]
+            names = self.sample_names
 
         else:
-            corr = self.corr_samples
+            if np.isnan(self.signature_correlation).all():
+                self.compute_correlation("signatures")
+            values = self.signature_correlation
+            names = sum(self.signature_names.values(), [])
 
-        clustergrid = corr_plot(corr, annot=annot, **kwargs)
+        correlation_df = pd.DataFrame(values, index=names, columns=names)
+        return correlation_df
 
-        if outfile is not None:
-            plt.savefig(outfile, bbox_inches="tight")
-
-        return clustergrid
-
-    def plot_embeddings(self, annotations=None, outfile=None, **kwargs):
+    def plot_correlation(
+        self,
+        data: Literal["samples", "signatures"] = "signatures",
+        annot: bool | None = None,
+        outfile: str | None = None,
+        **kwargs,
+    ) -> ClusterGrid:
         """
-        Plot the signature and sample embeddings. If the embedding dimension
-        is two, the embeddings will be plotted directly, ignoring the chosen method.
-        See plot.py for the implementation of 'embeddings_plot'.
-
-        Parameters
-        ----------
-        annotations : list[str], default=None
-            Annotations per data point, e.g. the sample names. If None,
-            all signatures are annotated.
-            Note that there are sum('ns_signatures') + 'n_samples' data points,
-            i.e. the first sum('ns_signatures') elements in 'annotations'
-            are the signature annotations, not any sample annotations.
-
-        outfile : str, default=None
-            If not None, the figure will be saved in the specified file path.
-
-        **kwargs :
-            keyword arguments to pass to seaborn's scatterplot
-
-        Returns
-        -------
-        ax : matplotlib.axes.Axes
-            The matplotlib axes containing the plot.
+        Plot the signature or sample correlation.
         """
-        Ls = np.concatenate([model.L for model in self.models], axis=1)
-        embedding_data = np.concatenate([Ls, self.models[0].U], axis=1).T.copy()
+        value_checker("data", data, ["samples", "signatures"])
+        corr = self.correlation(data=data)
 
-        if annotations is None:
-            annotations = np.concatenate(
-                [model.signature_names for model in self.models]
-            )
+        if annot is None:
+            annot = False if data == "samples" else True
 
-        ax = embeddings_plot(data=embedding_data, annotations=annotations, **kwargs)
+        clustergrid = pl.correlation_pandas(corr, annot=annot, **kwargs)
 
         if outfile is not None:
             plt.savefig(outfile, bbox_inches="tight")
 
-        return ax
-
-    def feature_change(self, in_modality=None, out_modalities="all", normalize=True):
-        if in_modality is None:
-            in_modality = self.modality_names[0]
-
-        in_model = self.models[list(self.modality_names).index(in_modality)]
-
-        if out_modalities == "all":
-            out_modalities = self.modality_names
-
-        if type(out_modalities) is str:
-            out_modalities = [out_modalities]
-
-        out_modalities = [name for name in out_modalities if name != in_modality]
-        out_modalities_indices = [
-            n for n, name in enumerate(self.modality_names) if name in out_modalities
-        ]
-        results = [in_model.signatures]
-
-        for n in out_modalities_indices:
-            result = self.models[n].signatures @ np.exp(self.models[n].L.T @ in_model.L)
-            result.columns = in_model.signature_names
-
-            if normalize:
-                result = result / result.sum(axis=0)
-
-            results.append(result)
-
-        return results
+        return clustergrid
 
-    def plot_feature_change(
+    def plot_embeddings(
         self,
-        in_modality=None,
-        out_modalities="all",
-        colors=None,
-        annotate_mutation_types=False,
-        figsize=None,
-        outfile=None,
+        method: _Dim_reduction_methods = "umap",
+        n_components: int = 2,
+        dimensions: tuple[int, int] = (0, 1),
+        color: str | None = None,
+        zorder: str | None = None,
+        annotations: Iterable[str] | None = None,
+        outfile: str | None = None,
         **kwargs,
-    ):
-        """
-        For the signatures of one modality, plot the co-occuring spectra
-        in other modalities. This is achieved by interpreting a signature
-        embedding as a sample embedding and using the resulting exposures to
-        compute distributions over mutation types in different modalities.
-
-        Parameters
-        ----------
-        in_modality : str
-            The modality name of the signatures of interest, e.g. "SBS".
-
-        out_modalities : list or str, default="all"
-            A list of modalities to convert the 'in_modality' signatures
-            into, e.g. ["Indel", "SV"]. A single string can also be provided
-            to select only one 'out_modality'. By default, all modalities
-            other than the 'in_modality' are selected.
-
-        colors : list, default=None
-            A list of length '1 + len(out_modalities)' of colors to use
-            for the signature plots of the input modalitiy signatures
-            and the co-occuring spectra in the output modalites.
-
-        annotate_mutation_types : bool, default=False
-            If True, the x-axis of the spectra plots will be annotated
-            with the mutation types of the respective modalities.
-
-        figsize : tuple, default=None
-            The size of the matplotlib figure. If None, the figure size
-            is computed internally based on the number of input
-            signatures and output modalities.
-
-        outfile : str, default=None
-            If not None, the figure will be saved to the provided path.
-
-        kwargs : dict
-            Any keyword arguments to be passed to matplotlibs ax.bar.
-
-        Returns
-        -------
-        axes : np.ndarray
-            An array of matplotlib axes containing the plots.
-        """
-        # result[0] are the 'in_modality' signatures
-        results = self.feature_change(in_modality, out_modalities)
-        n_signatures = results[0].shape[1]
-        n_feature_spaces = len(results)
-
-        if colors is None:
-            colors = [None for _ in range(n_feature_spaces)]
-
-        if figsize is None:
-            figsize = (4 * n_feature_spaces, n_signatures)
-
-        fig, axes = plt.subplots(n_signatures, n_feature_spaces, figsize=figsize)
-        fig.suptitle("Signature feature change")
-
-        for axs, result, cols in zip(axes.T, results, colors):
-            signatures_plot(
-                result,
-                colors=cols,
-                annotate_mutation_types=annotate_mutation_types,
-                axes=axs,
-                **kwargs,
+    ) -> Axes:
+        adatas = list(self.asignatures.values()) + [self.mdata]
+        tl.reduce_dimension_multiple(
+            adatas=adatas,
+            basis="embeddings",
+            method=method,
+            n_components=n_components,
+        )
+        if self.dim_embeddings <= 2:
+            warnings.warn(
+                f"The embedding dimension is {self.dim_embeddings}. "
+                "The embeddings are plotted without an additional "
+                "dimensionality reduction.",
+                UserWarning,
             )
+            basis = "embeddings"
+        else:
+            basis = method
 
-        plt.tight_layout()
+        if color is None:
+            color = "color_embeddings"
+            for asigs in self.asignatures.values():
+                asigs.obs[color] = asigs.n_obs * ["black"]
+            self.mdata.obs[color] = self.mdata.n_obs * ["#1f77b4"]  # default blue
+
+        if zorder is None:
+            zorder = "zorder_embeddings"
+            for asigs in self.asignatures.values():
+                asigs.obs[zorder] = asigs.n_obs * [2]
+            self.mdata.obs[zorder] = self.mdata.n_obs * [1]
+
+        if annotations is None:
+            annotations = sum(self.signature_names.values(), [])
 
+        ax = pl.embedding_multiple(
+            adatas=adatas,
+            basis=basis,
+            dimensions=dimensions,
+            color=color,
+            zorder=zorder,
+            annotations=annotations,
+            **kwargs,
+        )
         if outfile is not None:
             plt.savefig(outfile, bbox_inches="tight")
 
-        return axes
+        return ax
```

### Comparing `salamander_learn-0.3.2/src/salamander/nmf_framework/signature_nmf.py` & `salamander_learn-0.4.0/src/salamander/models/signature_nmf.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,503 +1,617 @@
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
+from typing import TYPE_CHECKING, Any, Iterable, Literal, get_args
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
+from anndata import AnnData
 
-from ..plot import (
-    corr_plot,
-    embeddings_plot,
-    exposures_plot,
-    history_plot,
-    signatures_plot,
-)
-from ..utils import type_checker, value_checker
-
-EPSILON = np.finfo(np.float32).eps
+from .. import plot as pl
+from .. import tools as tl
+from ..initialization.initialize import EPSILON
+from ..initialization.methods import _INIT_METHODS
+from ..utils import match_signatures_pair, type_checker, value_checker
+
+if TYPE_CHECKING:
+    from matplotlib.axes import Axes
+    from seaborn.matrix import ClusterGrid
+
+    from ..initialization.methods import _Init_methods
+
+_Dim_reduction_methods = Literal[
+    "pca",
+    "tsne",
+    "umap",
+]
+_DIM_REDUCTION_METHODS = get_args(_Dim_reduction_methods)
 
 
 class SignatureNMF(ABC):
     """
     The abstract class SignatureNMF unifies the structure of
     multiple NMF algorithms used for signature analysis.
 
     Common properties and methods of all algorithms are indicated,
     i.e. have to be implemented by child classes, or implemented. Overview:
 
     Every child class has to implement the following attributes:
 
-        - signatures: pd.DataFrame
-            The signature matrix including mutation type names and signature names
+        - objective: Literal["minimize", "maximize"]
+            Whether the NMF algorithm minimize or maximize the objective function.
+            Some algorithms maximize a likelihood, others minimize a distance.
 
-        - exposures: pd.DataFrames
-            The exposure matrix including the signature names and sample names
+    Every child class has to implement the following methods:
 
-        - _n_parameters: int
-            The number of parameters fitted by the NMF algorithm.
-            This is needed to compute the Bayesian Information Criterion (BIC)
+        - compute_reconstruction_errors:
+            Add the samplewise reconstruction errors to adata.obs with the key
+            'reconstruction_error'.
 
-        - reconstruction_error: float
-            The reconstruction error between the count matrix and
-            the reconstructed count matrix.
+        - objective_fuction:
+            The objective function to optimize during model training.
 
-        - samplewise_reconstruction_error: np.ndarray
-            The samplewise reconstruction error between the sample counts and
-            the reconstructed sample counts.
-
-        - objective: str
-            "minimize" or "maximize". Whether the NMF algorithm maximizes or
-            minimizes the objective function. Some algorithms maximize a likelihood,
-            others minimize a distance. The distinction is useful for filtering NMF runs
-            based on the fitted objective function value downstream.
+        - _initialize:
+            Initialize all model parameters before model training.
 
-        - corr_signatures: pd.DataFrame
-            The signature correlation matrix
+        - _setup_fitting_parameters:
+            Initialize any additional and parameters required to fit
+            the NMF model.
 
-        - corr_samples: pd.DataFrame
-            The sample correlation matrix
+        - _update_parameters:
+            Update all model parameters.
 
+        - reorder:
+            Reorder the model parameters to match the order of another
+            collection of signatures.
 
-    Every child class has to implement the following methods:
+        - reduce_dimension_embeddings:
+            Reduce the dimension of the canonical model embeddings.
+            These are typically the sample exposures.
 
-        - objective_fuction:
-            The objective function to optimize when running the algorithm
+        - _get_embedding_plot_adata:
+            A helper function for the embedding plot.
 
-        - loglikelihood:
-            The loglikelihood of the underyling generative model
+        - _get_default_embedding_plot_annotations:
+            A helper function for the embedding plot.
 
-        - _initialize:
-            A method to initialize all model parameters before fitting
+    The following attributes and methods are implemented in SignatureNMF:
 
-        - fit:
-            Run the NMF algorithm for a given mutation count data. Every
-            fit method should also implement a version that allows fixing
-            arbitrary many a priori known signatures.
+        - mutation_types: np.ndarray
+            Wrapper around the var_names of the count data.
 
-        - _get_embedding_data:
-            A helper function for the embedding plot
+        - signature_names: np.ndarray
+            Wrapper around the obs_names of the signatures AnnData object.
 
-        - _get_default_embedding_annotations:
-            A helper function for the embedding plot
+        - sample_names: np.ndarrray
+            Wrapper around the obs_names of the count data.
 
+        - signatures: pd.DataFrame
+            Wrapper around the signatures AnnData object to return
+            the signatures as a dataframe.
 
-    The following attributes and methods are implemented in SignatureNMF:
+        - exposures: pd.DataFrame
+            Wrapper around adata.obsm to return the signature exposures
+            as a dataframe.
+
+        - compute_reconstruction: None
+            Add the reconstrcuted counts to adata.obsm with key 'X_reconstructed'.
 
         - data_reconstructed: pd.DataFrame
-            The recovered mutation count data given
-            the current signatures and exposures.
+            The recovered mutation count data as a dataframe.
+
+        - reconstruction_error: float
+            The sum of the samplewise reconstruction errors.
+
+        - _setup_adata:
+            Perform parameter checks on the input AnnData count object and clip zeros.
 
-        - X_reconstructed: np.ndarray
-            The recovered mutation count matrix given
-            the current signatures and exposures
+        - _check_given_asignatures:
+            Perform parameter checks on the optial input AnnData signature object.
 
-        - bic: float
-            The value of the Bayesian Information Criterion (BIC)
+        - fit:
+            Fit all model parameters.
+
+        - compute_correlation:
+            Add sample or signature correlations to the AnnData objects.
 
-        - _setup_data_parameters:
-            Perform parameter checks on the input data and add attributes
+        - correlation:
+            The sample or signature correlation as a dataframe.
 
         - plot_history:
             Plot the history of the objective function values after fitting the model
 
         - plot_signatures:
-            Plot the signatures using the signatures_plot function implemented in
-            the plot module
+            Plot the signatures as a barplot.
+
+        - plot_exposures:
+            Plot the exposures as a stacked barplot.
 
         - plot_correlation:
-            Plot the correlation of either the signatures or exposures
-            using the corr_plot function implemented in the plot module
+            Plot the correlation of either the signatures or exposures.
 
         - plot_embeddings:
             Plot the sample (and potentially the signature) embeddings in 2D
-            using PCA, tSNE or UMAP
+            using PCA, tSNE or UMAP.
     """
 
     def __init__(
         self,
-        n_signatures=1,
-        init_method="nndsvd",
-        min_iterations=500,
-        max_iterations=10000,
-        conv_test_freq=10,
-        tol=1e-7,
+        n_signatures: int = 1,
+        init_method: _Init_methods = "nndsvd",
+        min_iterations: int = 500,
+        max_iterations: int = 10000,
+        conv_test_freq: int = 10,
+        tol: float = 1e-7,
     ):
         """
-        Input:
+        Inputs
         ------
         n_signatures: int
-            The number of underlying signatures that are assumed to
-            have generated the mutation count data
+            The number of signatures that are assumed to
+            have generated the mutation count data.
 
-        init_method: str
-            The initialization method for the NMF algorithm
+        init_method: str, default='nndsvd'
+            The model parameter initialization method.
 
-        min_iterations: int
+        min_iterations: int, default=500
             The minimum number of iterations to perform by the NMF algorithm
 
-        max_iterations: int
+        max_iterations: int, default=10000
             The maximum number of iterations to perform by the NMF algorithm
 
-        conv_test_freq: int
+        conv_test_freq: int, default=10
             The frequency at which the algorithm is tested for convergence.
             The objective function value is only computed every 'conv_test_freq'
-            many iterations, which also affects a potentially saved history of
-            the objective function values.
+            many iterations.
 
         tol: float
-            The NMF algorithm is converged when the relative change of
-            the objective function of one iteration is smaller
-            than the tolerance 'tol'.
-        """
-        init_methods = [
-            "custom",
-            "flat",
-            "hierarchical_cluster",
-            "nndsvd",
-            "nndsvda",
-            "nndsvdar",
-            "random",
-            "separableNMF",
-        ]
-        value_checker("init_method", init_method, init_methods)
+            The convergence tolerance. The NMF algorithm is converged
+            when the relative change of the objective function is smaller
+            than 'tol'.
+        """
+        value_checker("init_method", init_method, _INIT_METHODS)
 
         self.n_signatures = n_signatures
-        self.signature_names = None
         self.init_method = init_method
         self.min_iterations = min_iterations
         self.max_iterations = max_iterations
         self.conv_test_freq = conv_test_freq
         self.tol = tol
 
         # initialize data/fitting dependent attributes
-        self.X = None
-        self.n_features = 0
-        self.n_given_signatures = 0
-        self.n_samples = 0
-        self.mutation_types = np.empty(0, dtype=str)
-        self.sample_names = np.empty(0, dtype=str)
-        self.history = {}
+        self.adata = AnnData()
+        self.asignatures = AnnData()
+        self.history: dict[str, Any] = {}
+
+    @property
+    def mutation_types(self) -> list[str]:
+        return list(self.adata.var_names)
+
+    @property
+    def signature_names(self) -> list[str]:
+        return list(self.asignatures.obs_names)
+
+    @property
+    def sample_names(self) -> list[str]:
+        return list(self.adata.obs_names)
 
     @property
-    @abstractmethod
     def signatures(self) -> pd.DataFrame:
         """
         Extract the mutational signatures as a pandas dataframe.
         """
-        pass
+        return self.asignatures.to_df()
 
     @property
-    @abstractmethod
     def exposures(self) -> pd.DataFrame:
         """
-        Extract the signature exposures of samples as a pandas dataframe.
+        Extract the signature exposures as a pandas dataframe.
         """
-        pass
+        assert (
+            "exposures" in self.adata.obsm
+        ), "Learning the sample exposures requires fitting the NMF model."
+        exposures_df = pd.DataFrame(
+            self.adata.obsm["exposures"],
+            index=self.sample_names,
+            columns=self.signature_names,
+        )
+        return exposures_df
+
+    def compute_reconstruction(self) -> None:
+        self.adata.obsm["X_reconstructed"] = (
+            self.adata.obsm["exposures"] @ self.asignatures.X
+        )
 
     @property
     def data_reconstructed(self) -> pd.DataFrame:
-        return (self.signatures @ self.exposures).astype(int)
+        if "X_reconstructed" not in self.adata.obsm:
+            self.compute_reconstruction()
 
-    @property
-    def X_reconstructed(self) -> np.ndarray:
-        return self.data_reconstructed.values
+        return pd.DataFrame(
+            self.adata.obsm["X_reconstructed"],
+            index=self.sample_names,
+            columns=self.mutation_types,
+        )
 
-    @property
     @abstractmethod
+    def compute_reconstruction_errors(self) -> None:
+        """
+        The samplewise reconstruction errors between the data
+        and the reconstructed data.
+        """
+
+    @property
     def reconstruction_error(self) -> float:
         """
-        The reconstruction error between the count matrix and
-        the reconstructed count matrix.
+        The total reconstruction error between the data and
+        the reconstructed data.
         """
-        pass
+        if "reconstruction_error" not in self.adata.obs:
+            self.compute_reconstruction_errors()
+
+        return np.sum(self.adata.obs["reconstruction_error"])
 
     @property
     @abstractmethod
-    def samplewise_reconstruction_error(self) -> np.ndarray:
+    def objective(self) -> Literal["minimize", "maximize"]:
         """
-        The samplewise reconstruction error between the sample counts and
-        the reconstructed sample counts.
+        Whether the NMF algorithm minimizes or maximizes its objective
+        function.
         """
-        pass
 
     @abstractmethod
     def objective_function(self) -> float:
         """
         The objective function to be optimized during fitting.
         """
-        pass
 
-    @abstractmethod
-    def loglikelihood(self) -> float:
+    def _setup_adata(self, adata: AnnData) -> None:
         """
-        The log-likelihood of the underlying generative model.
+        Check the type of the input counts and clip them to
+        avoid floating point errors.
+
+        Inputs
+        ------
+        data: AnnData
+            The AnnData object with the mutation count matrix.
         """
-        pass
+        type_checker("adata", adata, AnnData)
+        self.adata = adata
+        self.adata.X = self.adata.X.clip(EPSILON)
 
-    @property
     @abstractmethod
-    def _n_parameters(self) -> int:
-        """
-        Every child class has to implement a function returning
-        the number of parameters estimated by the respective model.
-        This is allows to, for example, implement the BIC
-        (Bayesian information criterion). The BIC can be used to
-        estimate the optimal number of signatures.
+    def _initialize(
+        self,
+        given_parameters: dict[str, Any] | None = None,
+        init_kwargs: dict[str, Any] | None = None,
+    ) -> None:
         """
-        pass
+        Initialize the NMF model parameters.
 
-    @property
-    def bic(self) -> float:
+        Example:
+            Before running the Lee & Seung NMF multiplicative update rules to
+            decompose the mutation count matrix into a signature matrix and
+            an exposure matrix, both matrices have to be initialized.
         """
-        Bayesian information criterion (BIC).
-        Can only be called after the _setup_parameters_fitting function as it
-        requires the number of samples be an attribute.
-        """
-        return self._n_parameters * np.log(self.n_samples) - 2 * self.loglikelihood()
-
-    def _check_given_signatures(self, given_signatures: pd.DataFrame):
-        """
-        Check if the given signatures are compatible with the
-        number of signatures of the algorithm and the
-        mutation types of the input data.
-
-        given_signatures: pd.DataFrame
-            Known signatures that should be fixed by the algorithm.
-            The number of known signatures can be less or equal to the
-            number of signatures specified in the algorithm instance.
-        """
-        type_checker("given_signatures", given_signatures, pd.DataFrame)
-        given_mutation_types = given_signatures.index.to_numpy(dtype=str)
-        compatible = (
-            np.array_equal(given_mutation_types, self.mutation_types)
-            and given_signatures.shape[1] <= self.n_signatures
-        )
-
-        if not compatible:
-            raise ValueError(
-                f"You have to provide at most {self.n_signatures} signatures with "
-                f"mutation types matching to your data."
-            )
 
     @abstractmethod
-    def _initialize(self):
+    def _setup_fitting_parameters(
+        self, fitting_kwargs: dict[str, Any] | None = None
+    ) -> None:
+        """
+        Initialize any additional and parameters required to fit
+        the NMF model.
         """
-        Initialize model parameters and attributes before fitting.
-        Enforcing the existence of _initialize unifies the implementation of
-        the NMF algorithms.
-
-        Example:
 
-            Before running the Lee & Seung NMF multiplicative update rules to
-            decompose the mutation count matrix X into a signature matrix W and
-            an exposure matrix H, both W and H have to be initialized.
+    @abstractmethod
+    def _update_parameters(
+        self, given_parameters: dict[str, Any] | None = None
+    ) -> None:
+        """
+        Update all model parameters.
         """
 
-    def _setup_data_parameters(self, data: pd.DataFrame):
+    def fit(
+        self,
+        adata: AnnData,
+        given_parameters: dict[str, Any] | None = None,
+        init_kwargs: dict[str, Any] | None = None,
+        fitting_kwargs: dict[str, Any] | None = None,
+        history: bool = True,
+        verbose: Literal[0, 1] = 0,
+        verbosity_freq: int = 1000,
+    ) -> SignatureNMF:
         """
-        Perform parameter checks before running the fit method.
+        Fit the model parameters. NMF models are expected to handle
+        'given_parameters' appropriately.
 
-        Input:
+        Inputs
         ------
-        data: pd.DataFrame
-            The mutation count pandas dataframe with indices and column names.
-            Samples are expected to corresponding to columns.
-        """
-        type_checker("data", data, pd.DataFrame)
-        self.X = data.values.clip(EPSILON)
-        self.n_features, self.n_samples = data.shape
-        self.mutation_types = data.index.values.astype(str)
-        self.sample_names = data.columns.values.astype(str)
+        adata: AnnData
+            The mutation count matrix as an AnnData object.
 
-    @abstractmethod
-    def fit(self, data: pd.DataFrame, given_signatures=None):
+        given_parameters: dict, optional
+            A priori known parameters. The key is expected to be the parameter
+            name.
+
+        init_kwargs: dict, optional
+            Keyword arguments to pass to the model parameter initialization, e.g.,
+            a seed when a stochastic initialization method is used.
+
+        fitting_kwargs: dict, optional
+            Keyword arguments to pass to the initialization of additional fitting
+            parameters, e.g., sample-specific loss function weights.
+
+        history: bool, default=True
+            If True, the objective function values computed during model training
+            will be stored.
+
+        verbose: Literal[0, 1], default=0
+            If True, intermediate objective function values obtained during model
+            training are printed.
+
+        verbosity_freq: int, default=1000
+            The objective function values after every 'verbosity_freq' many
+            iterations are printed. Only applies if 'verbose' is set to 1.
         """
-        Fit the model parameters. Child classes are expected to handle
-        'given_signatures' appropriately.
+        self._setup_adata(adata)
+        self._initialize(given_parameters, init_kwargs)
+        self._setup_fitting_parameters(fitting_kwargs)
+        of_values = [self.objective_function()]
+        n_iteration = 0
+        converged = False
 
-        Input:
-        ------
-        data: pd.DataFrame
-            The named mutation count data of shape (n_features, n_samples).
+        while not converged:
+            n_iteration += 1
 
-        given_signatures: pd.DataFrame, by default None
-            A priori known signatures. The number of given signatures has
-            to be less or equal to the number of signatures of NMF
-            algorithm instance, and the mutation type names have to match
-            the mutation types of the count data.
-        """
-
-    def plot_history(self, ax=None, min_iteration=0, outfile=None, **kwargs):
-        if not self.history:
-            raise ValueError(
-                "No history available, the model has to be fitted first. "
-                "Remember to set 'history' to 'True' when calling 'fit()'."
-            )
-
-        history_plot(
-            self.history["objective_function"],
-            self.conv_test_freq,
-            min_iteration=min_iteration,
-            ax=ax,
-            **kwargs,
+            if verbose and n_iteration % verbosity_freq == 0:
+                print(f"iteration: {n_iteration}; objective: {of_values[-1]:.2f}")
+
+            self._update_parameters(given_parameters)
+
+            if n_iteration % self.conv_test_freq == 0:
+                prev_of_value = of_values[-1]
+                of_values.append(self.objective_function())
+                rel_change_nominator = np.abs(prev_of_value - of_values[-1])
+                rel_change = rel_change_nominator / np.abs(prev_of_value)
+                converged = rel_change < self.tol and n_iteration >= self.min_iterations
+
+            converged |= n_iteration >= self.max_iterations
+
+        if history:
+            self.history["objective_function"] = of_values[1:]
+
+        return self
+
+    def reorder(
+        self,
+        asignatures_other: AnnData,
+        metric: str = "cosine",
+    ) -> None:
+        """
+        Reorder the model parameters to match the order of another
+        collection of signatures.
+        """
+        reordered_indices = match_signatures_pair(
+            asignatures_other.to_df().T, self.asignatures.to_df().T, metric=metric
         )
+        self.asignatures = self.asignatures[reordered_indices, :].copy()
+        self.adata.obsm["exposures"] = self.adata.obsm["exposures"][
+            :, reordered_indices
+        ]
 
+    def plot_history(self, outfile: str | None = None, **kwargs) -> Axes:
+        """
+        Plot the history of the objective function values. See
+        the implemenation of 'history' in the plotting module.
+        """
+        assert "objective_function" in self.history, (
+            "No history available, the model has to be fitted first. "
+            "Remember to set 'history' to 'True' when calling 'fit()'."
+        )
+        ax = pl.history(
+            values=self.history["objective_function"],
+            conv_test_freq=self.conv_test_freq,
+            **kwargs,
+        )
         if outfile is not None:
             plt.savefig(outfile, bbox_inches="tight")
 
         return ax
 
     def plot_signatures(
         self,
-        catalog=None,
-        colors=None,
-        annotate_mutation_types=False,
-        axes=None,
-        outfile=None,
+        annotate_mutation_types: bool = False,
+        outfile: str | None = None,
         **kwargs,
-    ):
+    ) -> Axes | Iterable[Axes]:
         """
-        Plot the signatures, see plot.py for the implementation of signatures_plot.
+        Plot the signatures, see the implementation of 'barplot' in
+        the plotting module.
         """
-        axes = signatures_plot(
-            self.signatures,
-            catalog=catalog,
-            colors=colors,
-            annotate_mutation_types=annotate_mutation_types,
-            axes=axes,
+        axes = pl.barplot(
+            self.asignatures,
+            annotate_vars=annotate_mutation_types,
             **kwargs,
         )
-
         if outfile is not None:
             plt.savefig(outfile, bbox_inches="tight")
 
         return axes
 
     def plot_exposures(
         self,
-        sample_order=None,
-        reorder_signatures=True,
-        annotate_samples=True,
-        colors=None,
-        ncol_legend=1,
-        ax=None,
-        outfile=None,
+        sample_order: np.ndarray | None = None,
+        reorder_signatures: bool = True,
+        annotate_samples: bool = True,
+        outfile: str | None = None,
         **kwargs,
-    ):
+    ) -> Axes:
         """
-        Visualize the exposures as a stacked bar chart,
-        see plot.py for the implementation.
+        Visualize the exposures as a stacked bar chart, see
+        the implementation of 'stacked_barplot' in the plotting
+        module.
+
+        Inputs
+        ------
+        sample_order: np.ndarray, optional
+            A pre-defined order of the samples along the x-axis.
+
+        reorder_signatures: bool, default=True
+            If True, the signatures are ordered by their total
+            relative contributions.
+
+        annotate_samples: bool, default=True
+            If True, the x-axis is annotated with the sample names.
+
+        outfile : str, default=None
+            If not None, the figure will be saved in the specified file path.
+
+        **kwargs:
+            Any further keyword arguments to pass to 'stacked_barplot'.
+
+        Returns
+        -------
+        ax : matplotlib.axes.Axes
+            The matplotlib axes containing the plot.
         """
-        ax = exposures_plot(
-            exposures=self.exposures,
-            sample_order=sample_order,
-            reorder_signatures=reorder_signatures,
-            annotate_samples=annotate_samples,
-            colors=colors,
-            ncol_legend=ncol_legend,
-            ax=ax,
+        ax = pl.stacked_barplot(
+            data=self.exposures,
+            obs_order=sample_order,
+            reorder_dimensions=reorder_signatures,
+            annotate_obs=annotate_samples,
             **kwargs,
         )
         if outfile is not None:
             plt.savefig(outfile, bbox_inches="tight")
 
         return ax
 
-    @property
-    @abstractmethod
-    def corr_signatures(self) -> pd.DataFrame:
-        """
-        Every child class of SignatureNMF has to implement a function that
-        returns the signature correlation matrix as a pandas dataframe.
-        """
+    def compute_correlation(
+        self, data: Literal["samples", "signatures"] = "signatures", **kwargs
+    ) -> None:
+        """
+        Compute the signature or sample correlation and store it in the
+        respective anndata object.
+        """
+        value_checker("data", data, ["samples", "signatures"])
+        assert "exposures" in self.adata.obsm, (
+            "Computing the sample or signature correlation "
+            "requires fitting the NMF model."
+        )
+        values = self.adata.obsm["exposures"]
 
-    @property
-    @abstractmethod
-    def corr_samples(self) -> pd.DataFrame:
-        """
-        Every child class of SignatureNMF has to implement a function that
-        returns the sample correlation matrix as a pandas dataframe.
-        """
+        if data == "signatures":
+            values = values.T
 
-    def plot_correlation(self, data="signatures", annot=False, outfile=None, **kwargs):
-        """
-        Plot the correlation matrix of the signatures or samples.
-        See plot.py for the implementation of corr_plot.
+        correlation = tl.correlation_numpy(values, **kwargs)
 
-        Input:
-        ------
-        *args, **kwargs:
-            arguments to be passed to corr_plot
+        if data == "samples":
+            self.adata.obsp["X_correlation"] = correlation
+        else:
+            self.asignatures.obsp["correlation"] = correlation
+
+    def correlation(
+        self, data: Literal["samples", "signatures"] = "signatures"
+    ) -> pd.DataFrame:
         """
-        value_checker("data", data, ["signatures", "samples"])
+        Dataframe of the signature or sample correlation.
+        """
+        value_checker("data", data, ["samples", "signatures"])
 
-        if data == "signatures":
-            corr = self.corr_signatures
+        if data == "samples":
+            if "X_correlation" not in self.adata.obsp:
+                self.compute_correlation("samples")
+            values = self.adata.obsp["X_correlation"]
+            names = self.sample_names
 
         else:
-            corr = self.corr_samples
+            if "correlation" not in self.asignatures.obsp:
+                self.compute_correlation("signatures")
+            values = self.asignatures.obsp["correlation"]
+            names = self.signature_names
+
+        correlation_df = pd.DataFrame(values, index=names, columns=names)
+        return correlation_df
+
+    def plot_correlation(
+        self,
+        data: Literal["samples", "signatures"] = "signatures",
+        annot: bool | None = None,
+        outfile: str | None = None,
+        **kwargs,
+    ) -> ClusterGrid:
+        """
+        Plot the signature or sample correlation.
+        """
+        value_checker("data", data, ["samples", "signatures"])
+        corr = self.correlation(data=data)
+
+        if annot is None:
+            annot = False if data == "samples" else True
 
-        clustergrid = corr_plot(corr, annot=annot, **kwargs)
+        clustergrid = pl.correlation_pandas(corr, annot=annot, **kwargs)
 
         if outfile is not None:
             plt.savefig(outfile, bbox_inches="tight")
 
         return clustergrid
 
     @abstractmethod
-    def _get_embedding_data(self) -> np.ndarray:
-        """
-        Get the data points for the dimensionality reduction / embedding plot.
-        One data point corresponds to a row of the embedding data.
-        Usually, these are the transposed exposures.
-        """
-
-    @abstractmethod
-    def _get_default_embedding_annotations(self) -> np.ndarray:
-        """
-        Get the annotations of the data points in the embedding plot.
-        """
-
-    def plot_embeddings(self, annotations=None, outfile=None, **kwargs):
+    def plot_embeddings(
+        self,
+        method: _Dim_reduction_methods = "umap",
+        n_components: int = 2,
+        dimensions: tuple[int, int] = (0, 1),
+        color: str | None = None,
+        zorder: str | None = None,
+        annotations: Iterable[str] | None = None,
+        outfile: str | None = None,
+        **kwargs,
+    ) -> Axes:
         """
         Plot a dimensionality reduction of the exposure representation.
         In most NMF algorithms, this is just the exposures of the samples.
         In CorrNMF, the exposures matrix is refactored, and there are both
         sample and signature embeddings in a shared embedding space.
 
         If the embedding dimension is one or two, the embeddings are be plotted
-        directly, ignoring the chosen method.
-        See plot.py for the implementation of 'embeddings_plot'.
+        directly, ignoring the chosen dimensionality reduction method.
+
+        Inputs
+        ------
+        method: str, default='umap'
+            The dimensionality reduction method. One of ['pca', 'tsne', 'umap'].
+
+        n_components: int, default=2
+            The target dimension of the dimensionality reduction.
+
+        dimensions: tuple[int, int], default=(0,1)
+            The indices of the dimensions to plot.
 
-        Parameters
-        ----------
-        annotations : list[str], default=None
+        color: str, default=None
+            Optional annotation key to use for the colors.
+
+        zorder: str, default=None
+            Optional annotation key to use for the drawing order.
+
+        annotations : Iterable[str], optional, default=None
             Annotations per data point, e.g. the sample names. If None,
             the algorithm-specific default annotations are used.
             For example, CorrNMF annotates the signature embeddings by default.
             Note that there are 'n_signatures' + 'n_samples' data points in CorrNMF,
             i.e. the first 'n_signatures' elements in 'annotations'
             are the signature annotations, not any sample annotations.
 
         outfile : str, default=None
             If not None, the figure will be saved in the specified file path.
 
         **kwargs :
-            keyword arguments to pass to seaborn's scatterplot
+            keyword arguments to pass to the scatterplot implementation.
 
         Returns
         -------
         ax : matplotlib.axes.Axes
             The matplotlib axes containing the plot.
         """
-        # one data point corresponds to a row of embedding_data
-        embedding_data = self._get_embedding_data()
-
-        if annotations is None:
-            annotations = self._get_default_embedding_annotations()
-
-        ax = embeddings_plot(data=embedding_data, annotations=annotations, **kwargs)
-
-        if outfile is not None:
-            plt.savefig(outfile, bbox_inches="tight")
-
-        return ax
```

### Comparing `salamander_learn-0.3.2/src/salamander/plot.py` & `salamander_learn-0.4.0/src/salamander/plot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,58 @@
-import warnings
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Any, Iterable
 
 import fastcluster
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
-import umap
 from adjustText import adjust_text
+from matplotlib.axes import Axes
 from scipy.cluster import hierarchy
 from scipy.spatial.distance import pdist
-from sklearn.decomposition import PCA
-from sklearn.manifold import TSNE
 
 from .consts import COLORS_INDEL83, COLORS_SBS96, INDEL_TYPES_83, SBS_TYPES_96
-from .utils import match_to_catalog, value_checker
+from .utils import _concat_light, _get_basis_obsm, _get_basis_obsp, match_to_catalog
+
+if TYPE_CHECKING:
+    from anndata import AnnData
+    from matplotlib.colors import Colormap
+    from matplotlib.typing import ColorType
+    from mudata import MuData
+    from seaborn.matrix import ClusterGrid
 
 
 def set_salamander_style():
     sns.set_context("notebook")
     sns.set_style("ticks")
     params = {
         "axes.edgecolor": "black",
-        "axes.labelsize": 14,
+        "axes.labelsize": "medium",
         "axes.spines.top": False,
         "axes.spines.right": False,
-        "axes.titlesize": 16,
-        "errorbar.capsize": 3,
+        "axes.titlesize": "large",
         "font.family": "DejaVu Sans",
-        "legend.fontsize": 12,
-        "lines.markersize": 8,
+        "legend.fontsize": "medium",
         "pdf.fonttype": 42,
-        "xtick.labelsize": 12,
-        "ytick.labelsize": 12,
+        "xtick.labelsize": "small",
+        "ytick.labelsize": "small",
     }
     mpl.rcParams.update(params)
 
 
-def history_plot(values, conv_test_freq, min_iteration=0, ax=None, **kwargs):
+def history(
+    values: np.ndarray,
+    conv_test_freq: int,
+    min_iteration: int = 0,
+    ax: Axes | None = None,
+    **kwargs,
+) -> Axes:
     n_values = len(values)
     ns_iteration = np.arange(
         conv_test_freq, n_values * conv_test_freq + 1, conv_test_freq
     )
 
     if min_iteration > ns_iteration[-1]:
         raise ValueError(
@@ -58,612 +69,771 @@
         if n_iteration >= min_iteration
     )
     ax.plot(ns_iteration[min_index:], values[min_index:], **kwargs)
     return ax
 
 
 def _annotate_plot(
-    ax,
-    data,
-    annotations,
-    ha="left",
-    fontsize="medium",
-    color="black",
-    adjust_annotations=True,
-    adjust_kwargs=None,
+    ax: Axes,
+    data: np.ndarray,
+    annotations: Iterable[str],
+    fontsize: float | str = "small",
+    color: ColorType = "black",
+    adjust_annotations: bool = True,
+    adjust_kwargs: dict[str, Any] | None = None,
     **kwargs,
-):
+) -> None:
     for data_point, annotation in zip(data, annotations):
         ax.text(
             data_point[0],
             data_point[1],
             annotation,
-            ha=ha,
             fontsize=fontsize,
             color=color,
             **kwargs,
         )
     if adjust_annotations:
-        if adjust_kwargs is None:
-            adjust_kwargs = {} if adjust_kwargs is None else adjust_kwargs.copy()
-
-        annotations = [
+        adjust_kwargs = {} if adjust_kwargs is None else adjust_kwargs.copy()
+        texts = [
             child for child in ax.get_children() if isinstance(child, mpl.text.Text)
         ]
-        annotations = [
-            annotation for annotation in annotations if annotation.get_text()
-        ]
-        adjust_text(annotations, **adjust_kwargs)
+        texts_nonempty = [annotation for annotation in texts if annotation.get_text()]
+        adjust_text(texts_nonempty, **adjust_kwargs)
 
 
-def _scatter_1d(data: np.ndarray, ax=None, **kwargs):
+def _scatter_1d(
+    data: np.ndarray,
+    xlabel: str | None = None,
+    color: list[ColorType] | None = None,
+    zorder: list[int] | None = None,
+    ax: Axes | None = None,
+    **kwargs,
+) -> Axes:
     if data.ndim != 1:
-        raise ValueError(f"The datapoints of {data} (rows) have to be one-dimensional.")
+        raise ValueError("The data have to be one-dimensional.")
 
     if ax is None:
-        _, ax = plt.subplots(figsize=(6, 1))
+        _, ax = plt.subplots(figsize=(4, 1))
+
+    if zorder is None:
+        zorder = len(data) * [1]
 
     ax.spines[["left", "bottom"]].set_visible(False)
     ax.get_yaxis().set_visible(False)
-    ax.axhline(y=0, color="black", zorder=1)
-    data_2d = np.vstack([data, np.zeros_like(data)]).T
-    sns.scatterplot(x=data_2d[:, 0], y=data_2d[:, 1], ax=ax, zorder=2, **kwargs)
-    return data_2d, ax
+    ax.axhline(y=0, color="black", zorder=np.min(zorder) - 1)
 
+    for zord in np.unique(zorder):
+        subgroup = np.where(zorder == zord)[0]
+        subdata = data[subgroup]
+        subgroup_color = [color[d] for d in subgroup] if color is not None else None
+        sns.scatterplot(
+            x=subdata,
+            y=np.zeros_like(subdata),
+            color=subgroup_color,
+            zorder=zord,
+            ax=ax,
+            **kwargs,
+        )
 
-def _scatter_2d(data, ax=None, **kwargs):
-    """
-    The rows (!) of 'data' are assumed to be the data points.
-    """
-    if data.shape[1] != 2:
-        raise ValueError(f"The datapoints of {data} (rows) have to be two-dimensional.")
+    if xlabel:
+        ax.set_xlabel(xlabel)
 
-    if ax is None:
-        _, ax = plt.subplots(figsize=(6, 6))
-
-    ax.set(xlabel="x", ylabel="y")
-    sns.scatterplot(x=data[:, 0], y=data[:, 1], ax=ax, **kwargs)
-    return data, ax
+    return ax
 
 
-def _pca_2d(data, ax=None, **kwargs):
+def _scatter_2d(
+    data: np.ndarray,
+    xlabel: str | None = None,
+    ylabel: str | None = None,
+    ticks: bool = True,
+    color: list[ColorType] | None = None,
+    zorder: list[int] | None = None,
+    ax: Axes | None = None,
+    **kwargs,
+) -> Axes:
     """
     The rows (!) of 'data' are assumed to be the data points.
     """
-    if ax is None:
-        _, ax = plt.subplots(figsize=(6, 6))
-
-    data_2d = PCA(n_components=2).fit_transform(data)
-    ax.set(xlabel="PC1", ylabel="PC2")
-    sns.scatterplot(x=data_2d[:, 0], y=data_2d[:, 1], ax=ax, **kwargs)
-    return data_2d, ax
-
+    if data.shape[1] != 2:
+        raise ValueError("The datapoints (rows) have to be two-dimensional.")
 
-def _tsne_2d(data, perplexity=30, ax=None, **kwargs):
-    """
-    The rows (!) of 'data' are assumed to be the single data points.
-    """
     if ax is None:
-        _, ax = plt.subplots(figsize=(6, 6))
+        _, ax = plt.subplots(figsize=(4, 4))
 
-    with warnings.catch_warnings():
-        warnings.simplefilter("ignore")
-        perplexity = min(perplexity, len(data) - 1)
-        data_2d = TSNE(perplexity=perplexity).fit_transform(data)
+    if zorder is None:
+        zorder = len(data) * [1]
 
-    ax.set(xlabel="t-SNE1", xticks=[], ylabel="t-SNE2", yticks=[])
-    sns.scatterplot(x=data_2d[:, 0], y=data_2d[:, 1], ax=ax, **kwargs)
-    return data_2d, ax
+    for zord in np.unique(zorder):
+        subgroup = np.where(zorder == zord)[0]
+        subdata = data[subgroup]
+        subgroup_color = [color[d] for d in subgroup] if color is not None else None
+        sns.scatterplot(
+            x=subdata[:, 0],
+            y=subdata[:, 1],
+            color=subgroup_color,
+            zorder=zord,
+            ax=ax,
+            **kwargs,
+        )
 
+    if xlabel:
+        ax.set_xlabel(xlabel)
 
-def _umap_2d(data, n_neighbors=15, min_dist=0.1, ax=None, **kwargs):
-    """
-    The rows (!) of 'data' are assumed to be the single data points.
-    """
-    if ax is None:
-        _, ax = plt.subplots(figsize=(6, 6))
+    if ylabel:
+        ax.set_ylabel(ylabel)
 
-    n_neighbors = min(n_neighbors, len(data) - 1)
-    data_2d = umap.UMAP(n_neighbors=n_neighbors, min_dist=min_dist).fit_transform(data)
+    if not ticks:
+        ax.set(xticks=[], yticks=[])
 
-    ax.set(xlabel="UMAP1", xticks=[], ylabel="UMAP2", yticks=[])
-    sns.scatterplot(x=data_2d[:, 0], y=data_2d[:, 1], ax=ax, **kwargs)
-    return data_2d, ax
+    return ax
 
 
-def embeddings_plot(
+def scatter_numpy(
     data: np.ndarray,
-    method="umap",
-    normalize=False,
-    annotations=None,
-    annotation_kwargs=None,
-    adjust_annotations=True,
-    adjust_kwargs=None,
-    ax=None,
-    **kwargs,
-):
-    """
-    Plot a dimensionality reduction of high-dimensional data.
-    If the dimension of the data is one or two, it is plotted
-    directly, ignoring the chosen method.
-
-    Parameters
-    ----------
-    data : np.ndarray
-        The rows (!) are assumed to be the data points.
-
-    method : str, default='umap'
-        Either 'tsne', 'pca' or 'umap'. The respective dimensionality reduction
-        is applied to plot the data in 2D. If the dimensionality of the data is
-        less or equal to two, the points are plotted directly.
-
-    normalize : bool, default=False
-        If True, the data points are normalized to have a Euclidean norm of
-        one before applying the dimensionality reduction.
-
-    annotations : list[str], default=None
-        Annotations of the projected data points. The length of the list has to match
-        the number of data points.
-
-    annotation_kwargs : dict, default=None
-        keyword arguments to pass to matplotlibs plt.txt()
-
-    adjust_annotations : bool, default=True
-        If True, the annotations are adjusted to prevent them from overlapping.
-
-    adjust_kwargs : dict, default=None
-        keyword arguments to pass to adjustText's adjust_text.
-        This is for example useful when arrows connecting the projected
-        data points and the adjusted positions of the annotations
-        should be added.
-
-    ax : matplotlib.axes.Axes, default=None
-        Pre-existing axes for the plot. Otherwise, an axes is created.
-
-    **kwargs :
-        keyword arguments to pass to seaborn's scatterplot
-
-    Returns
-    -------
-    ax : matplotlib.axes.Axes
-        The matplotlib axes containing the plot.
-    """
-    value_checker("method", method, ["pca", "tsne", "umap"])
-
-    if normalize:
-        data /= np.sqrt(np.sum(data**2, axis=1))[:, np.newaxis]
-
-    n_dimensions = data.shape[1]
-
-    if n_dimensions in [1, 2]:
-        warnings.warn(
-            f"The dimension of the data points is {n_dimensions}. "
-            f"The method argument '{method}' will be ignored "
-            "and the embeddings are plotted directly.",
-            UserWarning,
-        )
-
-    if n_dimensions == 1:
-        data_2d, ax = _scatter_1d(data[:, 0], ax=ax, **kwargs)
-    elif n_dimensions == 2:
-        data_2d, ax = _scatter_2d(data, ax=ax, **kwargs)
-    elif method == "tsne":
-        data_2d, ax = _tsne_2d(data, ax=ax, **kwargs)
-    elif method == "pca":
-        data_2d, ax = _pca_2d(data, ax=ax, **kwargs)
+    xlabel: str | None = None,
+    ylabel: str | None = None,
+    ticks: bool = True,
+    color: list[ColorType] | None = None,
+    zorder: list[int] | None = None,
+    annotations: Iterable[str] | None = None,
+    annotation_kwargs: dict[str, Any] | None = None,
+    adjust_annotations: bool = True,
+    adjust_kwargs: dict[str, Any] | None = None,
+    ax: Axes | None = None,
+    **kwargs,
+) -> Axes:
+    if data.ndim == 1 or data.shape[1] == 1:
+        ax = _scatter_1d(data, xlabel, color, zorder, ax, **kwargs)
+        data_2d = np.vstack([data.flatten(), np.zeros_like(data.flatten())]).T
+    elif data.ndim == 2 and data.shape[1] == 2:
+        ax = _scatter_2d(data, xlabel, ylabel, ticks, color, zorder, ax, **kwargs)
+        data_2d = data
     else:
-        data_2d, ax = _umap_2d(data, ax=ax, **kwargs)
+        raise ValueError(
+            "Scatterplots are only supported for one- or two-dimensional data."
+        )
 
     if annotations is not None:
         annotation_kwargs = (
             {} if annotation_kwargs is None else annotation_kwargs.copy()
         )
         _annotate_plot(
             ax,
             data_2d,
             annotations,
             adjust_annotations=adjust_annotations,
             adjust_kwargs=adjust_kwargs,
             **annotation_kwargs,
         )
+    return ax
+
+
+def scatter(
+    adata: AnnData | MuData,
+    x: str,
+    y: str | None = None,
+    ticks: bool = True,
+    color: str | None = None,
+    zorder: str | None = None,
+    **kwargs,
+) -> Axes:
+    if y is None:
+        data = adata.obs[x].to_numpy()
+    else:
+        data = adata.obs[[x, y]].to_numpy()
+
+    col = list(adata.obs[color]) if color is not None else None
+    zord = list(adata.obs[zorder]) if zorder is not None else None
+    ax = scatter_numpy(
+        data, xlabel=x, ylabel=y, ticks=ticks, color=col, zorder=zord, **kwargs
+    )
+    return ax
+
+
+def scatter_multiple(
+    adatas: Iterable[AnnData | MuData],
+    x: str,
+    y: str | None = None,
+    ticks: bool = True,
+    color: str | None = None,
+    zorder: str | None = None,
+    **kwargs,
+) -> Axes:
+    obs_keys = [x, y, color, zorder]
+    obs_keys = [key for key in obs_keys if key is not None]
+    combined = _concat_light(adatas, obs_keys=obs_keys)
+    ax = scatter(
+        adata=combined, x=x, y=y, ticks=ticks, color=color, zorder=zorder, **kwargs
+    )
+    return ax
+
+
+def embedding_numpy(
+    data: np.ndarray,
+    dimensions: tuple[int, int] = (0, 1),
+    xlabel: str | None = None,
+    ylabel: str | None = None,
+    ticks: bool = True,
+    color: list[ColorType] | None = None,
+    zorder: list[int] | None = None,
+    **kwargs,
+) -> Axes:
+    if data.ndim == 2 and data.shape[1] > 2:
+        data = data[:, dimensions]
 
+    ax = scatter_numpy(data, xlabel, ylabel, ticks, color, zorder, **kwargs)
     return ax
 
 
-def corr_plot(
-    corr: pd.DataFrame, figsize=(6, 6), cmap="vlag", annot=True, fmt=".2f", **kwargs
-):
+# fmt: off
+def _basisobsm2name(basis: str) -> str:
+    name = (
+        "PC" if basis == "pca"
+        else "tSNE" if basis == "tsne"
+        else "UMAP" if basis == "umap"
+        else basis
+    )
+    return name
+# fmt: on
+
+
+def embedding(
+    adata: AnnData | MuData,
+    basis: str,
+    dimensions: tuple[int, int] = (0, 1),
+    xlabel: str | None = None,
+    ylabel: str | None = None,
+    ticks: bool | None = None,
+    color: str | None = None,
+    zorder: str | None = None,
+    **kwargs,
+) -> Axes:
+    data = _get_basis_obsm(adata, basis)
+    name = _basisobsm2name(basis)
+    labels = [f"{name}{d+1}" for d in dimensions]
+
+    if xlabel is None:
+        xlabel = labels[0]
+
+    if ylabel is None:
+        ylabel = labels[1]
+
+    if ticks is None:
+        ticks = False if basis in ["tsne", "umap"] else True
+
+    col = list(adata.obs[color]) if color is not None else None
+    zord = list(adata.obs[zorder]) if zorder is not None else None
+    ax = embedding_numpy(
+        data,
+        dimensions=dimensions,
+        xlabel=xlabel,
+        ylabel=ylabel,
+        ticks=ticks,
+        color=col,
+        zorder=zord,
+        **kwargs,
+    )
+    return ax
+
+
+def embedding_multiple(
+    adatas: Iterable[AnnData | MuData],
+    basis: str,
+    dimensions: tuple[int, int] = (0, 1),
+    xlabel: str | None = None,
+    ylabel: str | None = None,
+    ticks: bool | None = None,
+    color: str | None = None,
+    zorder: str | None = None,
+    **kwargs,
+) -> Axes:
+    obs_keys = [color, zorder]
+    obs_keys = [key for key in obs_keys if key is not None]
+    combined = _concat_light(adatas, obs_keys=obs_keys, obsm_keys=[basis])
+    ax = embedding(
+        adata=combined,
+        basis=basis,
+        dimensions=dimensions,
+        xlabel=xlabel,
+        ylabel=ylabel,
+        ticks=ticks,
+        color=color,
+        zorder=zorder,
+        **kwargs,
+    )
+    return ax
+
+
+def pca(adata: AnnData, **kwargs) -> Axes:
+    return embedding(adata, basis="pca", **kwargs)
+
+
+def pca_multiple(adatas: Iterable[AnnData | MuData], **kwargs) -> Axes:
+    return embedding_multiple(adatas, basis="pca", **kwargs)
+
+
+def tsne(adata: AnnData, **kwargs) -> Axes:
+    return embedding(adata, basis="tsne", **kwargs)
+
+
+def tsne_multiple(adatas: Iterable[AnnData | MuData], **kwargs) -> Axes:
+    return embedding_multiple(adatas, basis="tsne", **kwargs)
+
+
+def umap(adata: AnnData, **kwargs) -> Axes:
+    return embedding(adata, basis="umap", **kwargs)
+
+
+def umap_multiple(adatas: Iterable[AnnData | MuData], **kwargs) -> Axes:
+    return embedding_multiple(adatas, basis="umap", **kwargs)
+
+
+def correlation_pandas(
+    corr: pd.DataFrame,
+    figsize: tuple[float, float] = (4.0, 4.0),
+    cmap: Colormap | str | None = "vlag",
+    fmt: str = ".2f",
+    **kwargs,
+) -> ClusterGrid:
     linkage = hierarchy.linkage(corr)
     clustergrid = sns.clustermap(
         corr,
         row_linkage=linkage,
         figsize=figsize,
         vmin=-1,
         vmax=1,
         cmap=cmap,
-        annot=annot,
         fmt=fmt,
         **kwargs,
     )
-
     return clustergrid
 
 
-def _get_colors_signature_plot(mutation_types, colors=None):
+def correlation(adata: AnnData, **kwargs) -> ClusterGrid:
+    corr = pd.DataFrame(
+        _get_basis_obsp(adata, "correlation"),
+        index=adata.obs_names,
+        columns=adata.obs_names,
+    )
+    return correlation_pandas(corr, **kwargs)
+
+
+def _get_colors_barplot(var_names, colors=None):
     """
-    Given the mutation types and the colors argument of sigplot_bar, return the
-    final colors used in the signature bar chart.
+    Given the variable names / features and the colors argument of barplot,
+    return the final colors used in the bar chart.
     """
-    n_features = len(mutation_types)
+    n_vars = len(var_names)
 
     if colors == "SBS96" or (
-        n_features == 96 and all(mutation_types == SBS_TYPES_96) and colors is None
+        n_vars == 96 and all(var_names == SBS_TYPES_96) and colors is None
     ):
-        if n_features != 96:
+        if n_vars != 96:
             raise ValueError(
                 "The standard SBS colors can only be used "
                 "when the signatures have 96 features."
             )
         colors = COLORS_SBS96
 
     elif colors == "Indel83" or (
-        n_features == 83 and all(mutation_types == INDEL_TYPES_83) and colors is None
+        n_vars == 83 and all(var_names == INDEL_TYPES_83) and colors is None
     ):
-        if n_features != 83:
+        if n_vars != 83:
             raise ValueError(
                 "The standard Indel colors can only be used "
                 "when the signatures have 83 features."
             )
         colors = COLORS_INDEL83
 
     elif type(colors) in [str, tuple]:
-        colors = n_features * [colors]
+        colors = n_vars * [colors]
 
     elif type(colors) is list:
-        if len(colors) != n_features:
-            raise ValueError(
-                f"The list of colors must be of length n_features={n_features}."
-            )
+        if len(colors) != n_vars:
+            raise ValueError(f"The list of colors must be of length n_vars={n_vars}.")
 
     else:
-        colors = n_features * ["gray"]
+        colors = n_vars * ["gray"]
 
     return colors
 
 
-def _signature_plot(
-    signature, colors=None, annotate_mutation_types=False, ax=None, **kwargs
-):
+def _barplot_single(
+    data: pd.DataFrame,
+    colors: ColorType | list[ColorType] | None = None,
+    annotate_vars: bool = False,
+    ax: Axes | None = None,
+    **kwargs,
+) -> Axes:
     """
-    Inputs:
-    -------
-    signature: pd.Signature
-        Signature with mutation types and name.
+    Plot the relative values of a non-negative dataframe
+    with a single row.
 
-    colors: str, tuple or list
+    Inputs
+    ------
+    data: pd.DataFrame
+        A dataframe with only one row, typically a single signature
+        or the feature counts of a single sample.
+        The columns of data are expected to be the names of the features.
+
+    colors:
         Can be set to 'SBS96' or 'Indel83' to use the standard bar colors
-        for these mutation types.
-        Otherwise, when a single string or tuple is provided,
-        all bars will have the same color. Alternatively,
-        a list can be used to specifiy the color of each bar individually.
+        for these features.
+        Otherwise, when a single color is provided, all bars will have
+        the same color. Alternatively, a list can be used to specifiy
+        the color of each bar individually.
+
+    annotate_vars: bool, default=False
+        If True, the x-axis has ticks and annotations.
 
     ax:
-        A single matplotlib Axes in which to draw the plot.
+        Axes object to draw the plot onto. Otherwise, create an Axes internally.
 
     kwargs: dict
         Any keyword arguments to be passed to matplotlibs ax.bar
     """
     if ax is None:
         _, ax = plt.subplots(figsize=(4, 1))
 
-    signature_normalized = signature / signature.sum(axis=0)
-    mutation_types = signature.index
-    colors = _get_colors_signature_plot(mutation_types, colors)
+    data_normalized = data.div(data.sum(axis=1), axis=0)
+    var_names = data.columns
+    colors = _get_colors_barplot(var_names, colors)
 
-    ax.set_title(signature_normalized.columns[0])
+    ax.set_title(data.index[0])
     ax.spines["left"].set_visible(False)
     ax.get_yaxis().set_visible(False)
-    ax.set_xlim((-1, len(mutation_types)))
+    ax.set_xlim((-1, len(var_names)))
 
     ax.bar(
-        mutation_types,
-        signature_normalized.iloc[:, 0],
+        var_names,
+        data_normalized.iloc[0, :],
         linewidth=0,
         color=colors,
         **kwargs,
     )
 
-    if annotate_mutation_types:
-        ax.set_xticks(mutation_types)
+    if annotate_vars:
+        ax.set_xticks(var_names)
         ax.set_xticklabels(
-            mutation_types, family="monospace", fontsize=4, ha="center", rotation=90
+            var_names, family="monospace", fontsize="x-small", ha="center", rotation=90
         )
-
     else:
         ax.set_xticks([])
 
     return ax
 
 
-def signature_plot(
-    signature,
-    catalog=None,
-    colors=None,
-    annotate_mutation_types=False,
-    ax=None,
+def _barplot_matched(
+    data: pd.DataFrame,
+    catalog: pd.DataFrame | None = None,
+    colors: ColorType | list[ColorType] | None = None,
+    annotate_vars: bool = False,
+    ax: Axes | Iterable[Axes] | None = None,
     **kwargs,
-):
+) -> Axes | Iterable[Axes]:
     """
-    Inputs:
-    -------
-    signature: pd.Signature
-        Signature with mutation types and name.
+    Plot the relative values of a non-negative dataframe
+    with a single row.
+    The closest matching row from a 'catalog' can also be plotted.
+
+    Inputs
+    ------
+    data: pd.DataFrame
+        A dataframe with only one row, typically a single mutational
+        signature.
 
     catalog: pd.DataFrame
-        If a catalog is provided, the single best matching catalog signature
-        will also be plotted.
+        If a catalog with matching features is provided, the single best
+        matching row will also be plotted.
 
     colors: str, tuple or list
         Can be set to 'SBS96' or 'Indel83' to use the standard bar colors
-        for these mutation types.
-        Otherwise, when a single string or tuple is provided,
-        all bars will have the same color. Alternatively,
-        a list can be used to specifiy the color of each bar individually.
+        for these features.
+        Otherwise, when a single color is provided, all bars will have
+        the same color. Alternatively, a list can be used to specifiy
+        the color of each bar individually.
+
+    annotate_vars: bool, default=False
+        If True, the x-axis has ticks and annotations.
 
     ax:
-        Axes in which to draw the plot. A single Axes if catalog is None;
+        Axes object(s) to draw the plot onto. A single Axes if catalog is None;
         two Axes if a catalog is given.
 
     kwargs: dict
         Any keyword arguments to be passed to matplotlibs ax.bar
     """
     if catalog is None:
-        if ax is None:
-            _, ax = plt.subplots(figsize=(4, 1))
-
-        signatures = [signature]
-        axes = [ax]
+        assert isinstance(ax, Axes) or ax is None
+        return _barplot_single(
+            data, colors=colors, annotate_vars=annotate_vars, ax=ax, **kwargs
+        )
 
+    if ax is None:
+        _, axes = plt.subplots(1, 2, figsize=(8, 1))
     else:
-        if ax is None:
-            _, ax = plt.subplots(1, 2, figsize=(8, 1))
-
-        matched_signature = match_to_catalog(signature, catalog, metric="cosine")
-        signatures = [signature, matched_signature]
         axes = ax
 
-    for sig, axis in zip(signatures, axes):
-        _signature_plot(
-            sig,
+    matched_data = match_to_catalog(data, catalog, metric="cosine")
+    data_all = [data, matched_data]
+
+    for d, axis in zip(data_all, axes):
+        _barplot_single(
+            d,
             colors=colors,
-            annotate_mutation_types=annotate_mutation_types,
+            annotate_vars=annotate_vars,
             ax=axis,
             **kwargs,
         )
 
-    if catalog is None:
-        return axes[0]
-
     return axes
 
 
-def signatures_plot(
-    signatures,
-    catalog=None,
-    colors=None,
-    annotate_mutation_types=False,
-    axes=None,
+def barplot_pandas(
+    data: pd.DataFrame,
+    catalog: pd.DataFrame | None = None,
+    colors: ColorType | list[ColorType] | None = None,
+    annotate_vars: bool = False,
+    axes: Axes | Iterable[Axes] | None = None,
     **kwargs,
-):
+) -> Axes | Iterable[Axes]:
     """
-    Inputs:
-    -------
-    signatures : pd.DataFrame
-        Named signatures of shape (n_features, n_signatures)
+    Plot the relative values of the rows of a non-negative dataframe.
+    The closest matching rows from a 'catalog' can also be plotted.
+
+    Inputs
+    ------
+    data : pd.DataFrame
+        Annotated dataframe of shape (n_obs, n_vars), typically
+        a collection of mutational signatures.
 
     catalog: pd.DataFrame
-        If a catalog is provided, the best matching catalog signatures
-        will also be plotted.
+        If a catalog with matching features is provided, the best matching
+        rows of the catalog are also plotted.
 
-    axes : list
-        Axes in which to draw the plot. Multiple Axes if more than one signature
-        is provided or a catalog is given. Otherwise a single axis.
-        When a catalog is provided, axes is expected to be of shape (n_signatures, 2).
-    """
-    n_signatures = signatures.shape[1]
-
-    if n_signatures == 1:
-        ax = signature_plot(
-            signatures,
+    colors: str, tuple or list
+        Can be set to 'SBS96' or 'Indel83' to use the standard bar colors
+        for these features.
+        Otherwise, when a single color is provided, all bars will have
+        the same color. Alternatively, a list can be used to specifiy
+        the color of each bar individually.
+
+    annotate_vars: bool, default=False
+        If True, the x-axis has ticks and annotations.
+
+    axes : Axes | list[Axes]
+        Axes object(s) to draw the plot onto. Multiple Axes if 'data' has more than
+        one column or a catalog is given. Otherwise a single Axes.
+        When a catalog is provided, axes is expected to be of shape (n_obs, 2).
+    """
+    n_obs = data.shape[0]
+
+    if n_obs == 1:
+        return _barplot_matched(
+            data,
             catalog=catalog,
             colors=colors,
-            annotate_mutation_types=annotate_mutation_types,
+            annotate_vars=annotate_vars,
             ax=axes,
             **kwargs,
         )
-        return ax
 
     if axes is None:
         if catalog is None:
-            _, axes = plt.subplots(n_signatures, 1, figsize=(4, n_signatures))
+            _, axes = plt.subplots(n_obs, 1, figsize=(4, n_obs))
         else:
-            _, axes = plt.subplots(n_signatures, 2, figsize=(8, n_signatures))
+            _, axes = plt.subplots(n_obs, 2, figsize=(8, n_obs))
 
-    for ax, signature in zip(axes, signatures):
-        signature_plot(
-            signatures[[signature]],
+    assert isinstance(
+        axes, Iterable
+    ), "Adding multiple barplots to custom 'axes' requires 'axes' to be iterable."
+
+    for ax, row in zip(axes, data.T):
+        _barplot_matched(
+            data.loc[[row], :],
             catalog=catalog,
             colors=colors,
-            annotate_mutation_types=annotate_mutation_types,
+            annotate_vars=annotate_vars,
             ax=ax,
             **kwargs,
         )
-    plt.tight_layout()
 
+    plt.tight_layout()
     return axes
 
 
-def _get_sample_order(exposures: pd.DataFrame, normalize=True):
+def barplot(adata: AnnData, **kwargs) -> Axes | Iterable[Axes]:
+    return barplot_pandas(adata.to_df(), **kwargs)
+
+
+def get_obs_order(data: pd.DataFrame, normalize: bool = True) -> np.ndarray:
     """
-    Compute the aesthetically most pleasing order of the samples
-    for a stacked bar chart of the exposures.
+    Compute the aesthetically most pleasing order of the observations
+    of a non-negative data array of shape (n_obs, n_dimensions) for a
+    stacked barchart using hierarchical clustering.
 
-    Parameters
-    ----------
-    exposures : pd.DataFrame of shape (n_signatures, n_samples)
-        The named exposure matrix
+    Inputs
+    ------
+    data : pd.DataFrame of shape (n_obs, n_dimensions)
+        An annotated non-negative data matrix, typically the signature
+        exposures.
 
     normalize : bool, default=True
-        If True, the exposures are normalized before computing the
-        hierarchical clustering.
+        If True, the data is row-normalized before computing the
+        optimal order.
 
     Returns
     -------
-    sample_order : np.ndarray
-        The ordered sample names
+    order : np.ndarray
+        The ordered observations.
     """
     if normalize:
-        # not in-place
-        exposures = exposures / exposures.sum(axis=0)
+        # no in-place
+        data = data.div(data.sum(axis=1), axis=0)
 
-    d = pdist(exposures.T)
+    d = pdist(data)
     linkage = fastcluster.linkage(d)
-    # get the optimal sample order that is consistent
+    # get the optimal order that is consistent
     # with the hierarchical clustering linkage
-    sample_order = hierarchy.leaves_list(hierarchy.optimal_leaf_ordering(linkage, d))
-    sample_order = exposures.columns[sample_order].to_numpy()
-    return sample_order
+    obs_order = hierarchy.leaves_list(hierarchy.optimal_leaf_ordering(linkage, d))
+    obs_order = data.index[obs_order].to_numpy()
+    return obs_order
+
+
+def _reorder_data(
+    data: pd.DataFrame,
+    obs_order: np.ndarray | None = None,
+    normalize: bool = True,
+    reorder_dimensions: bool = True,
+) -> pd.DataFrame:
+    """
+    Reorder non-negative data using hierarchical clustering and optionally
+    reorder the dimensions by their total relative sums.
+
+    Inputs
+    ------
+    data : pd.DataFrame of shape (n_obs, n_dimensions)
+        An annotated non-negative data matrix, typically the signature
+        exposures.
 
+    obs_order : np.ndarray, default=None
+        An optional predefined order of the observations.
 
-def _reorder_exposures(
-    exposures: pd.DataFrame, sample_order=None, reorder_signatures=True
-):
-    """
-    Reorder the samples with hierarchical clustering and
-    reorder the signatures by their total relative exposure.
-
-    Parameters
-    ----------
-    exposures : pd.DataFrame of shape (n_signatures, n_samples)
-        The named exposure matrix
-
-    sample_order : np.ndarray, default=None
-        A predefined order of the samples as a list of sample names.
-        If None, hierarchical clustering is used to compute the
-        aesthetically most pleasing order.
+    normalize : bool, default=True
+        If True, the data is row-normalized before computing the
+        optimal order. Only used if 'data_order' is not given.
 
-    reorder_signatures : bool, default=True
-        If True, the signatures will be reordered such that the
-        total relative exposures of the signatures decrease from the bottom
-        to the top signature in the stacked bar chart.
+    reorder_dimensions : bool, default=True
+        If True, the dimensions/columns will be reordered such that their
+        total relative sums decrease from the left to the right.
 
     Returns
     -------
-    exposures_reordered : pd.DataFrame of shape (n_signatures, n_samples)
-        The reorderd named exposure matrix
+    data_reordered : pd.DataFrame of shape (n_obs, n_dimensions)
+        The reorderd annotated data.
     """
-    if sample_order is None:
-        sample_order = _get_sample_order(exposures)
-
-    exposures_reordered = exposures[sample_order]
-
-    # order the signatures by their total relative exposure
-    if reorder_signatures:
-        exposures_normalized = exposures_reordered / exposures_reordered.sum(axis=0)
-        signature_order = (
-            exposures_normalized.sum(axis=1).sort_values(ascending=False).index
-        )
-        exposures_reordered = exposures_reordered.reindex(signature_order)
-
-    return exposures_reordered
+    if obs_order is None:
+        obs_order = get_obs_order(data, normalize=normalize)
 
+    data_reordered = data.loc[obs_order, :]
 
-def exposures_plot(
-    exposures: pd.DataFrame,
-    sample_order=None,
-    reorder_signatures=True,
-    annotate_samples=True,
-    colors=None,
-    ncol_legend=1,
-    ax=None,
+    # order the columns by their total relative contribution
+    if reorder_dimensions:
+        data_normalized = data.div(data.sum(axis=1), axis=0)
+        dim_ordered = data_normalized.sum(axis=0).sort_values(ascending=False).index
+        data_reordered = data_reordered[dim_ordered]
+
+    return data_reordered
+
+
+def stacked_barplot(
+    data: pd.DataFrame,
+    obs_order: np.ndarray | None = None,
+    reorder_dimensions: bool = True,
+    annotate_obs: bool = True,
+    colors: Iterable[ColorType] | None = None,
+    title: str | None = None,
+    ncol_legend: int = 1,
+    ax: Axes | None = None,
     **kwargs,
-):
+) -> Axes:
     """
-    Visualize the exposures with a stacked bar chart.
+    Visualize non-negative data with a stacked bar chart, typically
+    the signature exposures.
 
-    Parameter
-    ---------
-    exposures : pd.DataFrame of shape (n_signatures, n_samples)
-        The named exposure matrix.
+    Inputs
+    ------
+    data : pd.DataFrame of shape (n_obs, n_dimensions)
+        An annotated non-negative data matrix, typically the signature
+        exposures.
 
-    sample_order : np.ndarray, default=None
-        A predefined order of the samples as a list of sample names.
+    obs_order : np.ndarray, default=None
+        An optional predefined order of the observations.
         If None, hierarchical clustering is used to compute the
         aesthetically most pleasing order.
 
-    reorder_signatures : bool, default=True
-        If True, the signatures will be reordered such that the
-        total relative exposures of the signatures decrease from the bottom
-        to the top signature in the stacked bar chart.
+    reorder_dimensions : bool, default=True
+        If True, the columns of 'data' will be reordered such that their
+        total relative contributions in the stacked bar chart is increasing.
 
-    annotate_samples : bool, default=True
-        If True, the x-axis is annotated with the sample names.
+    annotate_obs : bool, default=True
+        If True, the x-axis is annotated with the observation names.
 
-    colors : list of length n_signatures, default=None
-        Colors to pass to matplotlibs ax.bar, one per signature.
+    colors : iterable of length n_dimensions, default=None
+        Colors to pass to matplotlibs ax.bar, one per dimension.
 
     n_col_legend : int, default=1
         The number of columns of the legend.
 
     ax : matplotlib.axes.Axes, default=None
-        Pre-existing axes for the plot. Otherwise, create an axis internally.
+        Axes object to draw the plot onto. Otherwise, create an Axes internally.
 
     kwargs : dict
         Any keyword arguments to be passed to matplotlibs ax.bar.
 
     Returns
     -------
     ax : matplotlib.axes.Axes
         The matplotlib axes containing the plot.
     """
-    n_signatures, n_samples = exposures.shape
-    # not in-place
-    exposures = exposures / exposures.sum(axis=0)
-    exposures = _reorder_exposures(
-        exposures, sample_order=sample_order, reorder_signatures=reorder_signatures
+    n_obs, n_dimensions = data.shape
+    data = data.div(data.sum(axis=1), axis=0)
+    data = _reorder_data(
+        data, obs_order=obs_order, reorder_dimensions=reorder_dimensions
     )
 
     if ax is None:
-        _, ax = plt.subplots(figsize=(0.3 * n_samples, 4))
+        _, ax = plt.subplots(figsize=(0.3 * n_obs, 4))
 
     if colors is None:
-        colors = list(sns.color_palette("deep")) * (1 + n_signatures // 10)
+        colors = sns.color_palette("deep") * (1 + n_dimensions // 10)
 
-    bottom = np.zeros(n_samples)
+    bottom = np.zeros(n_obs)
 
-    for signature, color in zip(exposures.T, colors):
-        signature_exposures = exposures.T[signature].to_numpy()
+    for dimension, color in zip(data, colors):
+        values = data[dimension].to_numpy()
         ax.bar(
-            np.arange(n_samples),
-            signature_exposures,
+            np.arange(n_obs),
+            values,
             color=color,
             width=1,
-            label=signature,
+            label=dimension,
             linewidth=0,
             bottom=bottom,
             **kwargs,
         )
-        bottom += signature_exposures
-
-    if annotate_samples:
-        ax.set_xticks(np.arange(n_samples))
-        ax.set_xticklabels(exposures.columns, rotation=90, ha="center", fontsize=10)
+        bottom += values
 
+    if annotate_obs:
+        ax.set_xticks(np.arange(n_obs))
+        ax.set_xticklabels(data.index, rotation=90, ha="center", fontsize="x-small")
     else:
         ax.get_xaxis().set_visible(False)
 
-    ax.set_title("Sample exposures")
+    if title:
+        ax.set_title(title)
+
     ax.spines[["left", "bottom"]].set_visible(False)
     ax.get_yaxis().set_visible(False)
     ax.legend(loc="center left", bbox_to_anchor=(0.975, 0.5), ncol=ncol_legend)
 
     return ax
```

### Comparing `salamander_learn-0.3.2/PKG-INFO` & `salamander_learn-0.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: salamander-learn
-Version: 0.3.2
+Version: 0.4.0
 Summary: Salamander is a non-negative matrix factorization framework for signature analysis
 License: MIT
 Author: Benedikt Geiger
 Maintainer: Benedikt Geiger
 Maintainer-email: benedikt_geiger@hms.harvard.edu
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: adjustText (>=0.8,<0.9)
+Requires-Dist: anndata (>=0.10.5,<0.11.0)
 Requires-Dist: fastcluster (>=1.2.6,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
-Requires-Dist: numba (>=0.57,<0.58)
+Requires-Dist: mudata (>=0.2.3,<0.3.0)
+Requires-Dist: numba (>=0.59,<0.60)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: scikit-learn (>=1.3.0,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: seaborn (>=0.13.0,<0.14.0)
 Requires-Dist: umap-learn (>=0.5.4,<0.6.0)
 Description-Content-Type: text/markdown
```


# Comparing `tmp/ministats-0.3.0.tar.gz` & `tmp/ministats-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ministats-0.3.0.tar", last modified: Fri Mar 29 16:00:35 2024, max compression
+gzip compressed data, was "ministats-0.3.1.tar", last modified: Wed May  1 12:37:52 2024, max compression
```

## Comparing `ministats-0.3.0.tar` & `ministats-0.3.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2024-03-29 16:00:35.487994 ministats-0.3.0/
--rw-r--r--   0 ivan       (501) staff       (20)     3644 2023-06-29 19:55:38.000000 ministats-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 ivan       (501) staff       (20)      165 2024-03-28 16:54:20.000000 ministats-0.3.0/HISTORY.md
--rw-r--r--   0 ivan       (501) staff       (20)     1069 2023-06-29 19:16:59.000000 ministats-0.3.0/LICENSE
--rw-r--r--   0 ivan       (501) staff       (20)      239 2024-03-28 14:53:04.000000 ministats-0.3.0/MANIFEST.in
--rw-r--r--   0 ivan       (501) staff       (20)     2650 2024-03-29 16:00:35.488150 ministats-0.3.0/PKG-INFO
--rw-r--r--   0 ivan       (501) staff       (20)     1560 2024-03-29 15:04:12.000000 ministats-0.3.0/README.md
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2024-03-29 16:00:35.475278 ministats-0.3.0/docs/
--rw-r--r--   0 ivan       (501) staff       (20)      610 2023-06-29 19:16:59.000000 ministats-0.3.0/docs/Makefile
--rwxr-xr-x   0 ivan       (501) staff       (20)     4822 2023-06-29 19:16:59.000000 ministats-0.3.0/docs/conf.py
--rw-r--r--   0 ivan       (501) staff       (20)       33 2023-06-29 19:16:59.000000 ministats-0.3.0/docs/contributing.rst
--rw-r--r--   0 ivan       (501) staff       (20)       28 2023-06-29 19:16:59.000000 ministats-0.3.0/docs/history.rst
--rw-r--r--   0 ivan       (501) staff       (20)      301 2023-06-29 19:16:59.000000 ministats-0.3.0/docs/index.rst
--rw-r--r--   0 ivan       (501) staff       (20)     1168 2023-06-29 19:16:59.000000 ministats-0.3.0/docs/installation.rst
--rw-r--r--   0 ivan       (501) staff       (20)      771 2023-06-29 19:16:59.000000 ministats-0.3.0/docs/make.bat
--rw-r--r--   0 ivan       (501) staff       (20)       27 2023-06-29 19:16:59.000000 ministats-0.3.0/docs/readme.rst
--rw-r--r--   0 ivan       (501) staff       (20)       79 2023-06-29 19:16:59.000000 ministats-0.3.0/docs/usage.rst
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2024-03-29 16:00:35.482483 ministats-0.3.0/ministats/
--rw-r--r--   0 ivan       (501) staff       (20)     1488 2024-03-29 16:00:12.000000 ministats-0.3.0/ministats/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)     2919 2024-03-29 15:17:22.000000 ministats-0.3.0/ministats/confidence_intervals.py
--rw-r--r--   0 ivan       (501) staff       (20)     1017 2024-03-29 15:01:45.000000 ministats-0.3.0/ministats/estimators.py
--rw-r--r--   0 ivan       (501) staff       (20)     1228 2024-03-29 15:17:16.000000 ministats-0.3.0/ministats/formulas.py
--rw-r--r--   0 ivan       (501) staff       (20)    10121 2024-03-29 15:00:07.000000 ministats-0.3.0/ministats/hypothesis_tests.py
--rw-r--r--   0 ivan       (501) staff       (20)    35114 2024-03-29 14:57:40.000000 ministats-0.3.0/ministats/plots.py
--rw-r--r--   0 ivan       (501) staff       (20)     2869 2024-03-29 14:58:15.000000 ministats-0.3.0/ministats/probs.py
--rw-r--r--   0 ivan       (501) staff       (20)     1686 2024-03-29 14:58:48.000000 ministats-0.3.0/ministats/sampling.py
--rw-r--r--   0 ivan       (501) staff       (20)     4106 2024-03-29 15:17:12.000000 ministats-0.3.0/ministats/simulations.py
--rw-r--r--   0 ivan       (501) staff       (20)     2118 2024-03-28 14:51:57.000000 ministats-0.3.0/ministats/utils.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2024-03-29 16:00:35.485422 ministats-0.3.0/ministats.egg-info/
--rw-r--r--   0 ivan       (501) staff       (20)     2650 2024-03-29 16:00:35.000000 ministats-0.3.0/ministats.egg-info/PKG-INFO
--rw-r--r--   0 ivan       (501) staff       (20)      721 2024-03-29 16:00:35.000000 ministats-0.3.0/ministats.egg-info/SOURCES.txt
--rw-r--r--   0 ivan       (501) staff       (20)        1 2024-03-29 16:00:35.000000 ministats-0.3.0/ministats.egg-info/dependency_links.txt
--rw-r--r--   0 ivan       (501) staff       (20)        1 2024-03-29 16:00:35.000000 ministats-0.3.0/ministats.egg-info/not-zip-safe
--rw-r--r--   0 ivan       (501) staff       (20)       85 2024-03-29 16:00:35.000000 ministats-0.3.0/ministats.egg-info/requires.txt
--rw-r--r--   0 ivan       (501) staff       (20)       10 2024-03-29 16:00:35.000000 ministats-0.3.0/ministats.egg-info/top_level.txt
--rw-r--r--   0 ivan       (501) staff       (20)      424 2024-03-29 16:00:35.488885 ministats-0.3.0/setup.cfg
--rw-r--r--   0 ivan       (501) staff       (20)     1652 2024-03-29 16:00:12.000000 ministats-0.3.0/setup.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2024-03-29 16:00:35.487425 ministats-0.3.0/tests/
--rw-r--r--   0 ivan       (501) staff       (20)       39 2023-06-29 19:16:59.000000 ministats-0.3.0/tests/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)     1188 2024-03-29 14:15:25.000000 ministats-0.3.0/tests/test_estimtors.py
--rw-r--r--   0 ivan       (501) staff       (20)      526 2024-03-29 14:15:20.000000 ministats-0.3.0/tests/test_ministats.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2024-05-01 12:37:52.685646 ministats-0.3.1/
+-rw-r--r--   0 ivan       (501) staff       (20)     3644 2023-06-29 19:55:38.000000 ministats-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 ivan       (501) staff       (20)      165 2024-03-28 16:54:20.000000 ministats-0.3.1/HISTORY.md
+-rw-r--r--   0 ivan       (501) staff       (20)     1069 2023-06-29 19:16:59.000000 ministats-0.3.1/LICENSE
+-rw-r--r--   0 ivan       (501) staff       (20)      239 2024-03-28 14:53:04.000000 ministats-0.3.1/MANIFEST.in
+-rw-r--r--   0 ivan       (501) staff       (20)     2648 2024-05-01 12:37:52.685849 ministats-0.3.1/PKG-INFO
+-rw-r--r--   0 ivan       (501) staff       (20)     1558 2024-03-29 16:17:49.000000 ministats-0.3.1/README.md
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2024-05-01 12:37:52.673581 ministats-0.3.1/docs/
+-rw-r--r--   0 ivan       (501) staff       (20)      610 2023-06-29 19:16:59.000000 ministats-0.3.1/docs/Makefile
+-rwxr-xr-x   0 ivan       (501) staff       (20)     4822 2023-06-29 19:16:59.000000 ministats-0.3.1/docs/conf.py
+-rw-r--r--   0 ivan       (501) staff       (20)       33 2023-06-29 19:16:59.000000 ministats-0.3.1/docs/contributing.rst
+-rw-r--r--   0 ivan       (501) staff       (20)       28 2023-06-29 19:16:59.000000 ministats-0.3.1/docs/history.rst
+-rw-r--r--   0 ivan       (501) staff       (20)      301 2023-06-29 19:16:59.000000 ministats-0.3.1/docs/index.rst
+-rw-r--r--   0 ivan       (501) staff       (20)     1168 2023-06-29 19:16:59.000000 ministats-0.3.1/docs/installation.rst
+-rw-r--r--   0 ivan       (501) staff       (20)      771 2023-06-29 19:16:59.000000 ministats-0.3.1/docs/make.bat
+-rw-r--r--   0 ivan       (501) staff       (20)       27 2023-06-29 19:16:59.000000 ministats-0.3.1/docs/readme.rst
+-rw-r--r--   0 ivan       (501) staff       (20)       79 2023-06-29 19:16:59.000000 ministats-0.3.1/docs/usage.rst
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2024-05-01 12:37:52.680012 ministats-0.3.1/ministats/
+-rw-r--r--   0 ivan       (501) staff       (20)     1528 2024-05-01 12:36:30.000000 ministats-0.3.1/ministats/__init__.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2919 2024-03-29 15:17:22.000000 ministats-0.3.1/ministats/confidence_intervals.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1017 2024-03-29 15:01:45.000000 ministats-0.3.1/ministats/estimators.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1228 2024-03-29 15:17:16.000000 ministats-0.3.1/ministats/formulas.py
+-rw-r--r--   0 ivan       (501) staff       (20)    10121 2024-03-29 15:00:07.000000 ministats-0.3.1/ministats/hypothesis_tests.py
+-rw-r--r--   0 ivan       (501) staff       (20)    36208 2024-04-28 17:35:06.000000 ministats-0.3.1/ministats/plots.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2869 2024-03-29 14:58:15.000000 ministats-0.3.1/ministats/probs.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1686 2024-03-29 14:58:48.000000 ministats-0.3.1/ministats/sampling.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4106 2024-03-29 15:17:12.000000 ministats-0.3.1/ministats/simulations.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2118 2024-03-28 14:51:57.000000 ministats-0.3.1/ministats/utils.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2024-05-01 12:37:52.682778 ministats-0.3.1/ministats.egg-info/
+-rw-r--r--   0 ivan       (501) staff       (20)     2648 2024-05-01 12:37:52.000000 ministats-0.3.1/ministats.egg-info/PKG-INFO
+-rw-r--r--   0 ivan       (501) staff       (20)      721 2024-05-01 12:37:52.000000 ministats-0.3.1/ministats.egg-info/SOURCES.txt
+-rw-r--r--   0 ivan       (501) staff       (20)        1 2024-05-01 12:37:52.000000 ministats-0.3.1/ministats.egg-info/dependency_links.txt
+-rw-r--r--   0 ivan       (501) staff       (20)        1 2024-05-01 12:37:52.000000 ministats-0.3.1/ministats.egg-info/not-zip-safe
+-rw-r--r--   0 ivan       (501) staff       (20)       85 2024-05-01 12:37:52.000000 ministats-0.3.1/ministats.egg-info/requires.txt
+-rw-r--r--   0 ivan       (501) staff       (20)       10 2024-05-01 12:37:52.000000 ministats-0.3.1/ministats.egg-info/top_level.txt
+-rw-r--r--   0 ivan       (501) staff       (20)      424 2024-05-01 12:37:52.686796 ministats-0.3.1/setup.cfg
+-rw-r--r--   0 ivan       (501) staff       (20)     1652 2024-05-01 12:36:30.000000 ministats-0.3.1/setup.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2024-05-01 12:37:52.684929 ministats-0.3.1/tests/
+-rw-r--r--   0 ivan       (501) staff       (20)       39 2023-06-29 19:16:59.000000 ministats-0.3.1/tests/__init__.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1188 2024-03-29 14:15:25.000000 ministats-0.3.1/tests/test_estimtors.py
+-rw-r--r--   0 ivan       (501) staff       (20)      526 2024-03-29 14:15:20.000000 ministats-0.3.1/tests/test_ministats.py
```

### Comparing `ministats-0.3.0/CONTRIBUTING.md` & `ministats-0.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ministats-0.3.0/LICENSE` & `ministats-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ministats-0.3.0/PKG-INFO` & `ministats-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ministats
-Version: 0.3.0
+Version: 0.3.1
 Summary: Common statistical testing procedures used for STATS 101 topics. The code is intentionally simple to make it easy to forllow for beginners.
 Home-page: https://github.com/minireference/ministats
 Author: Ivan Savov
 Author-email: ivan@minireference.com
 License: MIT license
 Keywords: ministats
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -22,24 +22,24 @@
 License-File: LICENSE
 
 # Mini Stats Helpers
 
 [![image](https://img.shields.io/pypi/v/ministats.svg)](https://pypi.python.org/pypi/ministats)
 [![Documentation Status](https://readthedocs.org/projects/ministats/badge/?version=latest)](https://ministats.readthedocs.io/en/latest/?version=latest)
 
-Common statistical testing procedures used for STATS 101 topics. THhe
-code is intentionally simple, to make it easy to read for beginners.
+Common statistical testing procedures used for STATS 101 topics.
+The code is intentionally simple, to make it easy to read for beginners.
 
 -   Free software: MIT license
 -   Documentation: https://ministats.readthedocs.io
 
 
 ## About
 
-This library contains helper functions for statistical analysis procedures implmemented "from scratch."
+This library contains helper functions for statistical analysis procedures implemented "from scratch."
 Many of these procedures can be performed more quickly by simply calling an appropriate function defined in one of the existing libraries for statistical analysis,
 but we deliberately show the step by step procedures,
 so you'll know what's going on under the hood.
 
 
 
 ## Features
@@ -50,15 +50,15 @@
 
 
 
 ## Roadmap
 
 - [x] import plot helpers from https://github.com/minireference/noBSstatsnotebooks/blob/main/notebooks/plot_helpers.py
 - [x] import stats helpers from https://github.com/minireference/noBSstatsnotebooks/blob/main/notebooks/stats_helpers.py
-- [x] add github actions CI
+- [x] add GitHub actions CI
 - [x] add some tests
 - [ ] Split `plots.py` into:
    - [ ] `plots/discrete.py`
    - [ ] `plots/continuous.py`
    - [ ] `plots/linear_models.py`
    - [ ] `plots/figures.py` (not in main namespace)
    - [ ] `plots/sampling_dist` ? (not in main namespace)
```

### Comparing `ministats-0.3.0/README.md` & `ministats-0.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Mini Stats Helpers
 
 [![image](https://img.shields.io/pypi/v/ministats.svg)](https://pypi.python.org/pypi/ministats)
 [![Documentation Status](https://readthedocs.org/projects/ministats/badge/?version=latest)](https://ministats.readthedocs.io/en/latest/?version=latest)
 
-Common statistical testing procedures used for STATS 101 topics. THhe
-code is intentionally simple, to make it easy to read for beginners.
+Common statistical testing procedures used for STATS 101 topics.
+The code is intentionally simple, to make it easy to read for beginners.
 
 -   Free software: MIT license
 -   Documentation: https://ministats.readthedocs.io
 
 
 ## About
 
-This library contains helper functions for statistical analysis procedures implmemented "from scratch."
+This library contains helper functions for statistical analysis procedures implemented "from scratch."
 Many of these procedures can be performed more quickly by simply calling an appropriate function defined in one of the existing libraries for statistical analysis,
 but we deliberately show the step by step procedures,
 so you'll know what's going on under the hood.
 
 
 
 ## Features
@@ -27,15 +27,15 @@
 
 
 
 ## Roadmap
 
 - [x] import plot helpers from https://github.com/minireference/noBSstatsnotebooks/blob/main/notebooks/plot_helpers.py
 - [x] import stats helpers from https://github.com/minireference/noBSstatsnotebooks/blob/main/notebooks/stats_helpers.py
-- [x] add github actions CI
+- [x] add GitHub actions CI
 - [x] add some tests
 - [ ] Split `plots.py` into:
    - [ ] `plots/discrete.py`
    - [ ] `plots/continuous.py`
    - [ ] `plots/linear_models.py`
    - [ ] `plots/figures.py` (not in main namespace)
    - [ ] `plots/sampling_dist` ? (not in main namespace)
```

### Comparing `ministats-0.3.0/docs/Makefile` & `ministats-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ministats-0.3.0/docs/conf.py` & `ministats-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ministats-0.3.0/docs/installation.rst` & `ministats-0.3.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ministats-0.3.0/docs/make.bat` & `ministats-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ministats-0.3.0/ministats/__init__.py` & `ministats-0.3.1/ministats/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Mini Statistics."""
 
 __author__ = """Ivan Savov"""
 __email__ = 'ivan@minireference.com'
-__version__ = '0.3.0'
+__version__ = '0.3.1'
 
 
 from .confidence_intervals import (
     ci_mean,
     ci_var,
     ci_dmeans,
 )
@@ -63,14 +63,16 @@
     plot_alpha_beta_errors,
     plot_lm_simple,
     plot_residuals,
     plot_residuals2,
     plot_lm_partial,
     plot_lm_ttest,
     plot_lm_anova,
+    plot_lm_scale_loc,
+    calc_lm_vif,
 )
 
 from .sampling import (
     gen_sampling_dist,
     gen_boot_dist
 )
```

### Comparing `ministats-0.3.0/ministats/confidence_intervals.py` & `ministats-0.3.1/ministats/confidence_intervals.py`

 * *Files identical despite different names*

### Comparing `ministats-0.3.0/ministats/estimators.py` & `ministats-0.3.1/ministats/estimators.py`

 * *Files identical despite different names*

### Comparing `ministats-0.3.0/ministats/formulas.py` & `ministats-0.3.1/ministats/formulas.py`

 * *Files identical despite different names*

### Comparing `ministats-0.3.0/ministats/hypothesis_tests.py` & `ministats-0.3.1/ministats/hypothesis_tests.py`

 * *Files identical despite different names*

### Comparing `ministats-0.3.0/ministats/plots.py` & `ministats-0.3.1/ministats/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from scipy.integrate import quad
 import seaborn as sns
 import statsmodels.formula.api as smf
+import statsmodels.api as sm
 
 from scipy.stats import randint    # special handling beta+1=beta
 from scipy.stats import nbinom     # display parameter n as r
 from scipy.stats import hypergeom  # special handling M=a+b, n=a, N=n
 from scipy.stats import expon      # hide loc=0 parameter
 from scipy.stats import gamma      # hide loc=0 parameter
 from scipy.stats import norm
@@ -835,15 +836,15 @@
             else:
                 perc_obs = round(100*(1-alpha_obs))
                 label_obs = f"{perc_obs}% confidence interval for observations"
         else:
             label_obs = None
         ax.fill_between(x_vals, lower_obs, upper_obs, alpha=0.1, color="C0", label=label_obs)
 
-    if lab_mean or lab_obs:
+    if (ci_mean and lab_mean) or (ci_obs and lab_obs):
         ax.legend()
 
 
 def plot_residuals(xdata, ydata, b0, b1, xlims=None, ax=None):
     """
     Plot residuals between the points (x,y) and the line y = b0 + b1*x.
     """
@@ -996,7 +997,41 @@
         ax.plot([i-0.7, i], [beta0, beta0 + beta], color="k", linestyle=linestyle,
                 label=f"$\\beta_{{\\texttt{{{label}}}}}$ = \\texttt{{{slopelab}}} slope")
 
     # Return axes
     ax.legend()
     return ax
 
+
+def plot_lm_scale_loc(lmfit, pred=None):
+    """
+    Plot the scale-location plot for the linear model `lmfit`.
+    """
+    sigmahat = np.sqrt(lmfit.scale)
+    std_resids = lmfit.resid / sigmahat
+    sqrt_abs_std_resids = np.sqrt(np.abs(std_resids))
+    if pred:
+        xs = lmfit.model.data.orig_exog[pred]
+        xlabel = pred
+    else:
+        xs = lmfit.fittedvalues
+        xlabel = "fitted values"
+    ax = sns.regplot(x=xs, y=sqrt_abs_std_resids, lowess=True)
+    ax.set_xlabel(xlabel)
+    ax.set_ylabel(r"$\sqrt{|\text{standardized residuals}|}$")
+    return ax
+
+
+def calc_lm_vif(lmfit, pred):
+    """
+    Calculate the variance inflation factor of the `pred` (str)
+    for the linear model fit `lmfit`.
+    """
+    dmatrix = lmfit.model.exog
+    pred_idx = lmfit.model.exog_names.index(pred)
+    n_cols = dmatrix.shape[1]
+    x_i = dmatrix[:, pred_idx]
+    mask = np.arange(n_cols) != pred_idx
+    X_noti = dmatrix[:, mask]
+    r_squared_i = sm.OLS(x_i, X_noti).fit().rsquared
+    vif = 1. / (1. - r_squared_i)
+    return vif
```

### Comparing `ministats-0.3.0/ministats/probs.py` & `ministats-0.3.1/ministats/probs.py`

 * *Files identical despite different names*

### Comparing `ministats-0.3.0/ministats/sampling.py` & `ministats-0.3.1/ministats/sampling.py`

 * *Files identical despite different names*

### Comparing `ministats-0.3.0/ministats/simulations.py` & `ministats-0.3.1/ministats/simulations.py`

 * *Files identical despite different names*

### Comparing `ministats-0.3.0/ministats/utils.py` & `ministats-0.3.1/ministats/utils.py`

 * *Files identical despite different names*

### Comparing `ministats-0.3.0/ministats.egg-info/PKG-INFO` & `ministats-0.3.1/ministats.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ministats
-Version: 0.3.0
+Version: 0.3.1
 Summary: Common statistical testing procedures used for STATS 101 topics. The code is intentionally simple to make it easy to forllow for beginners.
 Home-page: https://github.com/minireference/ministats
 Author: Ivan Savov
 Author-email: ivan@minireference.com
 License: MIT license
 Keywords: ministats
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -22,24 +22,24 @@
 License-File: LICENSE
 
 # Mini Stats Helpers
 
 [![image](https://img.shields.io/pypi/v/ministats.svg)](https://pypi.python.org/pypi/ministats)
 [![Documentation Status](https://readthedocs.org/projects/ministats/badge/?version=latest)](https://ministats.readthedocs.io/en/latest/?version=latest)
 
-Common statistical testing procedures used for STATS 101 topics. THhe
-code is intentionally simple, to make it easy to read for beginners.
+Common statistical testing procedures used for STATS 101 topics.
+The code is intentionally simple, to make it easy to read for beginners.
 
 -   Free software: MIT license
 -   Documentation: https://ministats.readthedocs.io
 
 
 ## About
 
-This library contains helper functions for statistical analysis procedures implmemented "from scratch."
+This library contains helper functions for statistical analysis procedures implemented "from scratch."
 Many of these procedures can be performed more quickly by simply calling an appropriate function defined in one of the existing libraries for statistical analysis,
 but we deliberately show the step by step procedures,
 so you'll know what's going on under the hood.
 
 
 
 ## Features
@@ -50,15 +50,15 @@
 
 
 
 ## Roadmap
 
 - [x] import plot helpers from https://github.com/minireference/noBSstatsnotebooks/blob/main/notebooks/plot_helpers.py
 - [x] import stats helpers from https://github.com/minireference/noBSstatsnotebooks/blob/main/notebooks/stats_helpers.py
-- [x] add github actions CI
+- [x] add GitHub actions CI
 - [x] add some tests
 - [ ] Split `plots.py` into:
    - [ ] `plots/discrete.py`
    - [ ] `plots/continuous.py`
    - [ ] `plots/linear_models.py`
    - [ ] `plots/figures.py` (not in main namespace)
    - [ ] `plots/sampling_dist` ? (not in main namespace)
```

### Comparing `ministats-0.3.0/ministats.egg-info/SOURCES.txt` & `ministats-0.3.1/ministats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ministats-0.3.0/setup.py` & `ministats-0.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,10 +46,10 @@
     include_package_data=True,
     keywords='ministats',
     name='ministats',
     packages=find_packages(include=['ministats', 'ministats.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/minireference/ministats',
-    version='0.3.0',
+    version='0.3.1',
     zip_safe=False,
 )
```

### Comparing `ministats-0.3.0/tests/test_estimtors.py` & `ministats-0.3.1/tests/test_estimtors.py`

 * *Files identical despite different names*

### Comparing `ministats-0.3.0/tests/test_ministats.py` & `ministats-0.3.1/tests/test_ministats.py`

 * *Files identical despite different names*


# Comparing `tmp/pygformula-1.0.5.tar.gz` & `tmp/pygformula-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygformula-1.0.5.tar", last modified: Wed Apr 24 19:58:37 2024, max compression
+gzip compressed data, was "pygformula-1.1.0.tar", last modified: Wed May  1 03:35:10 2024, max compression
```

## Comparing `pygformula-1.0.5.tar` & `pygformula-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 19:58:37.417611 pygformula-1.0.5/
--rw-rw-rw-   0        0        0     1122 2024-04-18 20:33:45.000000 pygformula-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     1453 2024-04-24 19:58:37.416611 pygformula-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1203 2024-04-24 19:58:04.000000 pygformula-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 19:58:37.376628 pygformula-1.0.5/pygformula/
--rw-rw-rw-   0        0        0       53 2024-04-18 18:44:20.000000 pygformula-1.0.5/pygformula/__init__.py
--rw-rw-rw-   0        0        0    14167 2024-04-18 20:33:45.000000 pygformula-1.0.5/pygformula/comparisons.py
--rw-rw-rw-   0        0        0     9610 2024-04-18 20:32:39.000000 pygformula-1.0.5/pygformula/data.py
-drwxrwxrwx   0        0        0        0 2024-04-24 19:58:37.405610 pygformula-1.0.5/pygformula/parametric_gformula/
--rw-rw-rw-   0        0        0       55 2024-02-09 07:11:15.000000 pygformula-1.0.5/pygformula/parametric_gformula/__init__.py
--rw-rw-rw-   0        0        0    17447 2024-04-18 20:33:45.000000 pygformula-1.0.5/pygformula/parametric_gformula/bootstrap.py
--rw-rw-rw-   0        0        0    21378 2024-04-18 20:33:45.000000 pygformula-1.0.5/pygformula/parametric_gformula/fit.py
--rw-rw-rw-   0        0        0     8385 2024-04-18 20:33:45.000000 pygformula-1.0.5/pygformula/parametric_gformula/histories.py
--rw-rw-rw-   0        0        0    12355 2024-04-18 20:33:45.000000 pygformula-1.0.5/pygformula/parametric_gformula/interventions.py
--rw-rw-rw-   0        0        0    44695 2024-04-18 20:33:45.000000 pygformula-1.0.5/pygformula/parametric_gformula/parametric_gformula.py
--rw-rw-rw-   0        0        0    25088 2024-04-18 20:33:45.000000 pygformula-1.0.5/pygformula/parametric_gformula/simulate.py
--rw-rw-rw-   0        0        0    19939 2024-04-18 20:33:45.000000 pygformula-1.0.5/pygformula/plot.py
-drwxrwxrwx   0        0        0        0 2024-04-24 19:58:37.411610 pygformula-1.0.5/pygformula/utils/
--rw-rw-rw-   0        0        0        0 2024-04-18 20:33:45.000000 pygformula-1.0.5/pygformula/utils/__init__.py
--rw-rw-rw-   0        0        0     7677 2024-04-18 20:33:45.000000 pygformula-1.0.5/pygformula/utils/helper.py
--rw-rw-rw-   0        0        0    39587 2024-04-24 19:56:21.000000 pygformula-1.0.5/pygformula/utils/util.py
-drwxrwxrwx   0        0        0        0 2024-04-24 19:58:37.387610 pygformula-1.0.5/pygformula.egg-info/
--rw-rw-rw-   0        0        0     1453 2024-04-24 19:58:37.000000 pygformula-1.0.5/pygformula.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      644 2024-04-24 19:58:37.000000 pygformula-1.0.5/pygformula.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 19:58:37.000000 pygformula-1.0.5/pygformula.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-24 19:58:37.000000 pygformula-1.0.5/pygformula.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 19:58:37.417611 pygformula-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      421 2024-04-24 19:58:32.000000 pygformula-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 03:35:10.857942 pygformula-1.1.0/
+-rw-rw-rw-   0        0        0     1122 2024-04-18 20:33:45.000000 pygformula-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1451 2024-05-01 03:35:10.856943 pygformula-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1201 2024-05-01 03:32:18.000000 pygformula-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 03:35:10.818853 pygformula-1.1.0/pygformula/
+-rw-rw-rw-   0        0        0       53 2024-04-18 18:44:20.000000 pygformula-1.1.0/pygformula/__init__.py
+-rw-rw-rw-   0        0        0    14167 2024-04-18 20:33:45.000000 pygformula-1.1.0/pygformula/comparisons.py
+-rw-rw-rw-   0        0        0     9610 2024-04-18 20:32:39.000000 pygformula-1.1.0/pygformula/data.py
+-rw-rw-rw-   0        0        0    12355 2024-04-18 20:33:45.000000 pygformula-1.1.0/pygformula/interventions.py
+drwxrwxrwx   0        0        0        0 2024-05-01 03:35:10.844169 pygformula-1.1.0/pygformula/parametric_gformula/
+-rw-rw-rw-   0        0        0       55 2024-02-09 07:11:15.000000 pygformula-1.1.0/pygformula/parametric_gformula/__init__.py
+-rw-rw-rw-   0        0        0    17447 2024-04-18 20:33:45.000000 pygformula-1.1.0/pygformula/parametric_gformula/bootstrap.py
+-rw-rw-rw-   0        0        0    21378 2024-04-18 20:33:45.000000 pygformula-1.1.0/pygformula/parametric_gformula/fit.py
+-rw-rw-rw-   0        0        0     8385 2024-04-18 20:33:45.000000 pygformula-1.1.0/pygformula/parametric_gformula/histories.py
+-rw-rw-rw-   0        0        0    44696 2024-05-01 02:34:23.000000 pygformula-1.1.0/pygformula/parametric_gformula/parametric_gformula.py
+-rw-rw-rw-   0        0        0    25089 2024-05-01 02:34:15.000000 pygformula-1.1.0/pygformula/parametric_gformula/simulate.py
+-rw-rw-rw-   0        0        0    19939 2024-04-18 20:33:45.000000 pygformula-1.1.0/pygformula/plot.py
+drwxrwxrwx   0        0        0        0 2024-05-01 03:35:10.850931 pygformula-1.1.0/pygformula/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-18 20:33:45.000000 pygformula-1.1.0/pygformula/utils/__init__.py
+-rw-rw-rw-   0        0        0     7677 2024-04-18 20:33:45.000000 pygformula-1.1.0/pygformula/utils/helper.py
+-rw-rw-rw-   0        0        0    39587 2024-04-24 19:56:21.000000 pygformula-1.1.0/pygformula/utils/util.py
+drwxrwxrwx   0        0        0        0 2024-05-01 03:35:10.828166 pygformula-1.1.0/pygformula.egg-info/
+-rw-rw-rw-   0        0        0     1451 2024-05-01 03:35:10.000000 pygformula-1.1.0/pygformula.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      624 2024-05-01 03:35:10.000000 pygformula-1.1.0/pygformula.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 03:35:10.000000 pygformula-1.1.0/pygformula.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-01 03:35:10.000000 pygformula-1.1.0/pygformula.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 03:35:10.858942 pygformula-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      421 2024-05-01 03:32:18.000000 pygformula-1.1.0/setup.py
```

### Comparing `pygformula-1.0.5/LICENSE` & `pygformula-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygformula-1.0.5/PKG-INFO` & `pygformula-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygformula
-Version: 1.0.5
+Version: 1.1.0
 Summary: A python implementation of the parametric g-formula
 Maintainer: Jing Li
 Maintainer-email: jing_li@hsph.harvard.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pygformula: a python implementation of the parametric g-formula
@@ -44,8 +44,7 @@
 - statsmodels
 - tqdm
 
 
 ## Documentation
 
 The online documentation is available at [pygformula documentation](https://pygformula.readthedocs.io).
-
```

### Comparing `pygformula-1.0.5/README.md` & `pygformula-1.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -35,8 +35,7 @@
 - statsmodels
 - tqdm
 
 
 ## Documentation
 
 The online documentation is available at [pygformula documentation](https://pygformula.readthedocs.io).
-
```

### Comparing `pygformula-1.0.5/pygformula/comparisons.py` & `pygformula-1.1.0/pygformula/comparisons.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.0.5/pygformula/data.py` & `pygformula-1.1.0/pygformula/data.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.0.5/pygformula/parametric_gformula/bootstrap.py` & `pygformula-1.1.0/pygformula/parametric_gformula/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.0.5/pygformula/parametric_gformula/fit.py` & `pygformula-1.1.0/pygformula/parametric_gformula/fit.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.0.5/pygformula/parametric_gformula/histories.py` & `pygformula-1.1.0/pygformula/parametric_gformula/histories.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.0.5/pygformula/parametric_gformula/interventions.py` & `pygformula-1.1.0/pygformula/interventions.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.0.5/pygformula/parametric_gformula/parametric_gformula.py` & `pygformula-1.1.0/pygformula/parametric_gformula/parametric_gformula.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from joblib import Parallel, delayed
 from tqdm import tqdm
 from lifelines import CoxPHFitter
 from .fit import fit_covariate_model, fit_ymodel, fit_compevent_model, fit_censor_model
 from .histories import update_precoded_history, update_custom_history
 from .simulate import simulate
 from .bootstrap import Bootstrap
-from .interventions import natural
+from ..interventions import natural
 from ..utils.helper import get_cov_hist_info, visit_func, hr_data_helper, hr_comp_data_helper, categorical_func
 from ..utils.util import read_intervention_input, error_catch, keywords_check, save_config, save_results, get_output, get_hr_output
 from ..comparisons import comparison_calculate
 from ..plot import plot_natural_course, plot_interventions
 
 
 class ParametricGformula:
```

### Comparing `pygformula-1.0.5/pygformula/parametric_gformula/simulate.py` & `pygformula-1.1.0/pygformula/parametric_gformula/simulate.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import math
 import types
 from functools import reduce
 import operator
 from scipy.stats import truncnorm
 from .histories import update_precoded_history, update_custom_history
 from ..utils.helper import categorical_func
-from .interventions import intervention_func
+from ..interventions import intervention_func
 
 
 def binorm_sample(prob):
     return np.random.binomial(n=1, p=prob, size=1)[0]
 
 def norm_sample(mean, rmse):
     return np.random.normal(loc=mean, scale=rmse, size=1)[0]
```

### Comparing `pygformula-1.0.5/pygformula/plot.py` & `pygformula-1.1.0/pygformula/plot.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.0.5/pygformula/utils/helper.py` & `pygformula-1.1.0/pygformula/utils/helper.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.0.5/pygformula/utils/util.py` & `pygformula-1.1.0/pygformula/utils/util.py`

 * *Files identical despite different names*

### Comparing `pygformula-1.0.5/pygformula.egg-info/PKG-INFO` & `pygformula-1.1.0/pygformula.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygformula
-Version: 1.0.5
+Version: 1.1.0
 Summary: A python implementation of the parametric g-formula
 Maintainer: Jing Li
 Maintainer-email: jing_li@hsph.harvard.edu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pygformula: a python implementation of the parametric g-formula
@@ -44,8 +44,7 @@
 - statsmodels
 - tqdm
 
 
 ## Documentation
 
 The online documentation is available at [pygformula documentation](https://pygformula.readthedocs.io).
-
```

### Comparing `pygformula-1.0.5/pygformula.egg-info/SOURCES.txt` & `pygformula-1.1.0/pygformula.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 LICENSE
 README.md
 setup.py
 pygformula/__init__.py
 pygformula/comparisons.py
 pygformula/data.py
+pygformula/interventions.py
 pygformula/plot.py
 pygformula.egg-info/PKG-INFO
 pygformula.egg-info/SOURCES.txt
 pygformula.egg-info/dependency_links.txt
 pygformula.egg-info/top_level.txt
 pygformula/parametric_gformula/__init__.py
 pygformula/parametric_gformula/bootstrap.py
 pygformula/parametric_gformula/fit.py
 pygformula/parametric_gformula/histories.py
-pygformula/parametric_gformula/interventions.py
 pygformula/parametric_gformula/parametric_gformula.py
 pygformula/parametric_gformula/simulate.py
 pygformula/utils/__init__.py
 pygformula/utils/helper.py
 pygformula/utils/util.py
```


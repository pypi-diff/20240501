# Comparing `tmp/cvxriskopt-0.1.2.tar.gz` & `tmp/cvxriskopt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxriskopt-0.1.2.tar", last modified: Thu Apr 25 01:58:38 2024, max compression
+gzip compressed data, was "cvxriskopt-0.1.3.tar", last modified: Wed May  1 00:59:23 2024, max compression
```

## Comparing `cvxriskopt-0.1.2.tar` & `cvxriskopt-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 sleiman    (501) staff       (20)        0 2024-04-25 01:58:38.992786 cvxriskopt-0.1.2/
--rw-r--r--   0 sleiman    (501) staff       (20)    35149 2024-04-24 22:44:20.000000 cvxriskopt-0.1.2/LICENSE
--rw-r--r--   0 sleiman    (501) staff       (20)     1525 2024-04-25 01:58:38.992619 cvxriskopt-0.1.2/PKG-INFO
--rw-r--r--   0 sleiman    (501) staff       (20)      718 2024-04-25 00:13:52.000000 cvxriskopt-0.1.2/README.md
-drwxr-xr-x   0 sleiman    (501) staff       (20)        0 2024-04-25 01:58:38.990492 cvxriskopt-0.1.2/cvxRiskOpt/
--rw-r--r--   0 sleiman    (501) staff       (20)        0 2024-04-09 19:49:24.000000 cvxriskopt-0.1.2/cvxRiskOpt/__init__.py
--rw-r--r--   0 sleiman    (501) staff       (20)    17005 2024-04-25 00:40:56.000000 cvxriskopt-0.1.2/cvxRiskOpt/cclp_risk_opt.py
--rw-r--r--   0 sleiman    (501) staff       (20)     7462 2024-04-25 00:41:30.000000 cvxriskopt-0.1.2/cvxRiskOpt/mpc_helpers.py
--rw-r--r--   0 sleiman    (501) staff       (20)    17494 2024-04-25 00:41:30.000000 cvxriskopt-0.1.2/cvxRiskOpt/wass_risk_opt_pb.py
-drwxr-xr-x   0 sleiman    (501) staff       (20)        0 2024-04-25 01:58:38.992283 cvxriskopt-0.1.2/cvxRiskOpt.egg-info/
--rw-r--r--   0 sleiman    (501) staff       (20)     1525 2024-04-25 01:58:38.000000 cvxriskopt-0.1.2/cvxRiskOpt.egg-info/PKG-INFO
--rw-r--r--   0 sleiman    (501) staff       (20)      398 2024-04-25 01:58:38.000000 cvxriskopt-0.1.2/cvxRiskOpt.egg-info/SOURCES.txt
--rw-r--r--   0 sleiman    (501) staff       (20)        1 2024-04-25 01:58:38.000000 cvxriskopt-0.1.2/cvxRiskOpt.egg-info/dependency_links.txt
--rw-r--r--   0 sleiman    (501) staff       (20)      126 2024-04-25 01:58:38.000000 cvxriskopt-0.1.2/cvxRiskOpt.egg-info/requires.txt
--rw-r--r--   0 sleiman    (501) staff       (20)       11 2024-04-25 01:58:38.000000 cvxriskopt-0.1.2/cvxRiskOpt.egg-info/top_level.txt
--rw-r--r--   0 sleiman    (501) staff       (20)       38 2024-04-25 01:58:38.992827 cvxriskopt-0.1.2/setup.cfg
--rw-r--r--   0 sleiman    (501) staff       (20)     1018 2024-04-25 01:55:57.000000 cvxriskopt-0.1.2/setup.py
-drwxr-xr-x   0 sleiman    (501) staff       (20)        0 2024-04-25 01:58:38.991922 cvxriskopt-0.1.2/tests/
--rw-r--r--   0 sleiman    (501) staff       (20)    12028 2024-04-24 23:38:45.000000 cvxriskopt-0.1.2/tests/test_cclp_risk_opt.py
--rw-r--r--   0 sleiman    (501) staff       (20)     2746 2024-04-24 22:52:27.000000 cvxriskopt-0.1.2/tests/test_mpc_helpers_functions.py
--rw-r--r--   0 sleiman    (501) staff       (20)    26992 2024-04-24 22:52:27.000000 cvxriskopt-0.1.2/tests/test_wass_risk_opt_pb.py
+drwxr-xr-x   0 sleiman    (501) staff       (20)        0 2024-05-01 00:59:23.962991 cvxriskopt-0.1.3/
+-rw-r--r--   0 sleiman    (501) staff       (20)    35149 2024-04-24 22:44:20.000000 cvxriskopt-0.1.3/LICENSE
+-rw-r--r--   0 sleiman    (501) staff       (20)     1771 2024-05-01 00:59:23.962829 cvxriskopt-0.1.3/PKG-INFO
+-rw-r--r--   0 sleiman    (501) staff       (20)      964 2024-04-28 17:00:05.000000 cvxriskopt-0.1.3/README.md
+drwxr-xr-x   0 sleiman    (501) staff       (20)        0 2024-05-01 00:59:23.960245 cvxriskopt-0.1.3/cvxRiskOpt/
+-rw-r--r--   0 sleiman    (501) staff       (20)        0 2024-04-09 19:49:24.000000 cvxriskopt-0.1.3/cvxRiskOpt/__init__.py
+-rw-r--r--   0 sleiman    (501) staff       (20)    20512 2024-04-30 20:57:20.000000 cvxriskopt-0.1.3/cvxRiskOpt/cclp_risk_opt.py
+-rw-r--r--   0 sleiman    (501) staff       (20)     9410 2024-04-30 21:57:24.000000 cvxriskopt-0.1.3/cvxRiskOpt/mpc_helpers.py
+-rw-r--r--   0 sleiman    (501) staff       (20)    21710 2024-05-01 00:19:34.000000 cvxriskopt-0.1.3/cvxRiskOpt/wass_risk_opt_pb.py
+drwxr-xr-x   0 sleiman    (501) staff       (20)        0 2024-05-01 00:59:23.962467 cvxriskopt-0.1.3/cvxRiskOpt.egg-info/
+-rw-r--r--   0 sleiman    (501) staff       (20)     1771 2024-05-01 00:59:23.000000 cvxriskopt-0.1.3/cvxRiskOpt.egg-info/PKG-INFO
+-rw-r--r--   0 sleiman    (501) staff       (20)      398 2024-05-01 00:59:23.000000 cvxriskopt-0.1.3/cvxRiskOpt.egg-info/SOURCES.txt
+-rw-r--r--   0 sleiman    (501) staff       (20)        1 2024-05-01 00:59:23.000000 cvxriskopt-0.1.3/cvxRiskOpt.egg-info/dependency_links.txt
+-rw-r--r--   0 sleiman    (501) staff       (20)      126 2024-05-01 00:59:23.000000 cvxriskopt-0.1.3/cvxRiskOpt.egg-info/requires.txt
+-rw-r--r--   0 sleiman    (501) staff       (20)       11 2024-05-01 00:59:23.000000 cvxriskopt-0.1.3/cvxRiskOpt.egg-info/top_level.txt
+-rw-r--r--   0 sleiman    (501) staff       (20)       38 2024-05-01 00:59:23.963030 cvxriskopt-0.1.3/setup.cfg
+-rw-r--r--   0 sleiman    (501) staff       (20)     1018 2024-05-01 00:52:26.000000 cvxriskopt-0.1.3/setup.py
+drwxr-xr-x   0 sleiman    (501) staff       (20)        0 2024-05-01 00:59:23.962059 cvxriskopt-0.1.3/tests/
+-rw-r--r--   0 sleiman    (501) staff       (20)    12028 2024-04-24 23:38:45.000000 cvxriskopt-0.1.3/tests/test_cclp_risk_opt.py
+-rw-r--r--   0 sleiman    (501) staff       (20)     2746 2024-04-24 22:52:27.000000 cvxriskopt-0.1.3/tests/test_mpc_helpers_functions.py
+-rw-r--r--   0 sleiman    (501) staff       (20)    26992 2024-05-01 00:47:28.000000 cvxriskopt-0.1.3/tests/test_wass_risk_opt_pb.py
```

### Comparing `cvxriskopt-0.1.2/LICENSE` & `cvxriskopt-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxriskopt-0.1.2/PKG-INFO` & `cvxriskopt-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxRiskOpt
-Version: 0.1.2
+Version: 0.1.3
 Summary: Risk-Based Optimization tool using CVXPY and CVXPYgen
 Home-page: https://github.com/TSummersLab/cvxRiskOpt
 Author: Sleiman Safaoui, Tyler Summers
 Author-email: snsafaoui@gmail.com, tyler.summers@utdallas.edu
 Maintainer: Sleiman Safaoui
 Maintainer-email: snsafaoui@gmail.com
 License: GPL-3.0
@@ -24,39 +24,38 @@
 
 # CVXPY Risk Optimization
 
 A package for risk-based optimization using CVXPY and CVXPYgen.
 
 ## Installation
 
-- create and activate conda env 
+### Installing from PyPI
+The package can be installed using pip:
 ```
-conda create --name cvxRiskOpt python=3.10 pip -y
-conda activate cvxRiskOpt
-```
-- install dependencies
+pip install cvxRiskOpt
 ```
-pip install cvxpy>=1.4.1
-pip install cvxpygen>=0.3.4
-pip install scipy>=1.11.4
-pip install numpy>=1.26.2
-pip install matplotlib>=3.8.0
+Notes:
+- The installation will also include cvxpy and cvxpygen.
+- Please refer to cvxpy's documentation for [installing additional solvers](https://www.cvxpy.org/install/).
+- Compiling code with Clarabel requires `Rust`, `Eigen`, and `cbindgen`. (e.g. These can be installed with `homebrew` on MacOS) 
+
+### Installing from source
+- Clone/Download the package
+- Create and activate conda env 
 ```
-For development, also install:
-```
-pip install pytest==7.4.0
-pip install polytope==0.2.5
-pip install Sphinx==7.2.6
+conda create --name cvxRiskOpt python=3.10 pip -y
+conda activate cvxRiskOpt
 ```
-- install the package
+- Install dependencies (see `setup.py`)
+- Install the package
 ```
 python3 -m pip install -e .
 ```
 
 ## Tests
-To run tests,
+To run tests, execute the following from the root of the package.
 ```
 pytest
 ```
 
 ## Examples
-There are several examples in `examples` demonstrating the usage of the package's functionality.
+There are several examples in `examples` demonstrating the usage of the package.
```

### Comparing `cvxriskopt-0.1.2/cvxRiskOpt/cclp_risk_opt.py` & `cvxriskopt-0.1.3/cvxRiskOpt/cclp_risk_opt.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+""""""
 """
 cvxRiskOpt: Risk-Based Optimization tool using CVXPY and CVXPYgen
 Copyright (C) 2024  Sleiman Safaoui
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
@@ -16,16 +17,17 @@
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 GitHub:
 @The-SS
 Email:
 snsafaoui@gmail.com
 sleiman.safaoui@utdallas.edu
-"""
-"""
+
+
+
 CVXPY-based Chance Constraints Linear Programs
 
 We implement some results from:
 "On Distributionally Robust Chance-Constrained Linear Programs"
 """
 import cvxpy as cp
 import numpy as np
@@ -228,16 +230,36 @@
 
 def _format_inputs(eps: int | float,
                    a: int | float | list | np.ndarray | cp.Variable | cp.Expression = None,
                    b: int | float | cp.Variable | cp.Expression = None,
                    xi1_hat: int | float | list | np.ndarray | cp.Variable | cp.Expression = None,
                    xi2_hat: int | float = None,
                    gam11: int | float | list | np.ndarray = None,
-                   gam12=None,
+                   gam12: int | float | list | np.ndarray = None,
                    gam22: int | float = None):
+    """
+    Format the inputs to make them compatible with the CCLP functions
+
+    :param eps: The epsilon value in the chance constraint.
+    :type eps: float
+    :param a: The "a" term in the chance constraint.
+    :type a: int | float | list | np.ndarray | cp.Variable | cp.Expression, optional
+    :param b: The "b" term in the chance constraint.
+    :type b: int | float | cp.Variable | cp.Expression, optional
+    :param xi1_hat: The mean of the "xi1" term in the chance constraint.
+    :type xi1_hat: int | float | list | np.ndarray | cp.Variable | cp.Expression, optional
+    :param xi2_hat: The mean of the "xi2" term in the chance constraint.
+    :type xi2_hat: int | float, optional
+    :param gam11: The covariance "gam11" of the "xi1" term in the chance constraint.
+    :type gam11: int | float | list | np.ndarray, optional
+    :param gam12: The cross-covariance "gam12" between the xi1 and xi2 terms in the chance constraint.
+    :type gam12: int | float | list | np.ndarray, optional
+    :param gam22: The variance "gam22" of the "xi2" term in the chance constraint.
+    :type gam22: int | float, optional
+    """
     # check eps
     if not isinstance(eps, (int, float)) or eps <= 0 or eps > 0.5:
         raise ValueError("eps must be a number in (0, 0.5].")
 
     # checks to figure out what terms are included in the sum
     a_xi1_present, xi2_present, b_present = False, False, False
 
@@ -268,26 +290,39 @@
               a_xi1_present: bool, xi2_present: bool, b_present: bool,
               assume_sym=False, assume_psd=False):
     """
     returns the deterministic constraint from reformulating the CCLP.
     Form: kappa_e * sigma_x + psi_hat <= 0
 
     :param kappa_e: tightening term based on special cases
+    :type kappa_e: int | float
     :param a: a term
+    :type a: np.ndarray | cp.Variable | cp.Expression
     :param b: b term
+    :type b: int | float | cp.Variable | cp.Expression
     :param xi1_hat: xi1 term mean
+    :type xi1_hat: np.ndarray | cp.Variable | cp.Expression
     :param xi2_hat: xi2 term mean
+    :type xi2_hat: int | float
     :param gam11: xi1 term covar
+    :type gam11: np.ndarray
     :param gam12: xi2 term var
+    :type gam12: np.ndarray
     :param gam22: xi1 and xi2 cross covar
+    :type gam22: np.ndarray
     :param a_xi1_present: indicates a and xi1 present
+    :type a_xi1_present: bool
     :param xi2_present: indicates xi2 present
+    :type xi2_present: bool
     :param b_present: indicates b present
+    :type b_present: bool
     :param assume_sym: assume covar symmetric (else check)
+    :type assume_sym: bool, optional
     :param assume_psd: assume covar PSD (else check)
+    :type assume_psd: bool, optional
     :return:
     """
 
     # There are 5 cases:
     # 1. No expression (user error?)
     if not a_xi1_present and not xi2_present and not b_present:
         raise ValueError("No expression provided")
@@ -321,100 +356,133 @@
         psi_hat = a_til @ xi_hat + b
 
         gamma = _construct_gamma(gam11, gam12, gam22)
         sigma_x = _cp_sqrt_quad_form(a_til, gamma, assume_sym=assume_sym, assume_psd=assume_psd)
     return kappa_e * sigma_x + psi_hat <= 0
 
 
-def cclp_gauss(eps, a=None, b=None,
-               xi1_hat=None, xi2_hat=None,
-               gam11=None, gam12=None, gam22=None,
+def cclp_gauss(eps: int | float,
+               a: int | float | list | np.ndarray | cp.Variable | cp.Expression = None,
+               b: int | float | cp.Variable | cp.Expression = None,
+               xi1_hat: int | float | list | np.ndarray | cp.Variable | cp.Expression = None,
+               xi2_hat: int | float = None,
+               gam11: int | float | list | np.ndarray = None,
+               gam12: int | float | list | np.ndarray = None,
+               gam22: int | float = None,
                assume_sym=False, assume_psd=False):
     """
-    Reformulates a CC of the type Prob(a^T xi1 + b + xi2 <= 0) >= 1-eps.
+    Reformulates a CC of the type
+    :math:`\\mathbb{P}(a^T \\xi_1 + b + \\xi_2 \\leq 0) \\geq 1-\\epsilon`
+    where the distribution is Gaussian.
 
     This function reformulates a chance constraint (CC) where the distribution is known to be a Gaussian distribution with:
-    xi = [xi1^T xi2]^T
-    Expect(xi) = [xi1_hat^T xi2_hat]^T
-    Cov(xi) = [gam11       gam12
-               gam12^T    gam22]
 
-    :param eps: The epsilon value in the chance constraint.
-    :type eps: float
-    :param a: The coefficient vector a in the chance constraint.
-    :type a: array_like, optional
-    :param b: The constant term b in the chance constraint.
-    :type b: float, optional
-    :param xi1_hat: The expected value of xi1.
-    :type xi1_hat: array_like, optional
-    :param xi2_hat: The expected value of xi2.
-    :type xi2_hat: array_like, optional
-    :param gam11: The covariance matrix of xi1.
-    :type gam11: array_like, optional
-    :param gam12: The cross-covariance matrix between xi1 and xi2.
-    :type gam12: array_like, optional
-    :param gam22: The covariance matrix of xi2.
-    :type gam22: array_like, optional
-    :param assume_sym: Whether to assume the covariance matrix is symmetric.
-    :type assume_sym: bool, optional
-    :param assume_psd: Whether to assume the covariance matrix is positive semi-definite.
-    :type assume_psd: bool, optional
-    :return: The reformulated chance constraint.
-    :rtype: cvxpy.Constraint or cp.Expression
+    .. math::
+        \\begin{align*}
+        \\xi &= [\\xi_1^T \\xi_2]^T \\\\
+        \\text{Expect}(\\xi) &= [\\hat{\\xi_1}^T \\hat{\\xi_2}]^T \\\\
+        \\text{Cov}(\\xi) &= \\begin{bmatrix} \\text{gam11} & \\text{gam12} \\\\ \\text{gam12}^T & \\text{gam22} \\end{bmatrix}
+        \\end{align*}
+
+    Arguments:
+    ----------
+        eps : int | float:
+            The epsilon risk bound in the chance constraint.
+        a : int | float | list | np.ndarray | cp.Variable | cp.Expression, optional:
+            The coefficient vector/scalar "a" in the chance constraint.
+        b : int | float | cp.Variable | cp.Expression, optional:
+            The scalar term "b" in the chance constraint.
+        xi1_hat : int | float | list | np.ndarray | cp.Variable | cp.Expression, optional:
+            The expected value of xi1.
+        xi2_hat : int | float, optional:
+            The expected value of xi2.
+        gam11 : int | float | list | np.ndarray, optional:
+            The covariance matrix of xi1.
+        gam12 : int | float | list | np.ndarray, optional:
+            The cross-covariance matrix between xi1 and xi2.
+        gam22 : int | float, optional:
+            The covariance matrix of xi2.
+        assume_sym : bool, optional:
+            Whether to assume the covariance matrix is symmetric (otherwise, it is checked).
+        assume_psd : bool, optional:
+            Whether to assume the covariance matrix is positive semi-definite (otherwise, it is checked).
+
+    Returns:
+    --------
+        cvxpy.Constraint or cp.Expression:
+            The reformulated deterministic chance constraint.
     """
     # check inputs
     inputs = _format_inputs(eps, a, b,
                             xi1_hat, xi2_hat,
                             gam11, gam12, gam22)
 
     kappa_e = gauss.ppf(1 - eps)
 
     constr = _det_cclp(kappa_e, *inputs, assume_sym, assume_psd)
 
     return constr
 
 
-def cclp_dro_mean_cov(eps, a=None, b=None,
-                      xi1_hat=None, xi2_hat=None,
-                      gam11=None, gam12=None, gam22=None,
+def cclp_dro_mean_cov(eps: int | float,
+                      a: int | float | list | np.ndarray | cp.Variable | cp.Expression = None,
+                      b: int | float | cp.Variable | cp.Expression = None,
+                      xi1_hat: int | float | list | np.ndarray | cp.Variable | cp.Expression = None,
+                      xi2_hat: int | float = None,
+                      gam11: int | float | list | np.ndarray = None,
+                      gam12: int | float | list | np.ndarray = None,
+                      gam22: int | float = None,
                       assume_sym=False, assume_psd=False,
                       centrally_symmetric=False):
     """
-    Reformulates a DRO CC of the type inf_{moment based set} Prob(a^T exp + b <= 0) >= bound.
+    Reformulates a DRO CC of the type
+    :math:`\\inf_{\\mathbb{P} \\in \\mathcal{P}} \\mathbb{P}(a^T \\xi_1 + b + \\xi_2 \\leq 0) \\geq 1-\\epsilon`
+    where :math:`\\mathcal{P}` is a moment-based ambiguity set.
+
+    This function reformulates a distributionally robust optimization (DRO) chance constraint (CC) where the distribution
+    is unknown but belongs to a moment based ambiguity set with known mean and covariance:
+
+    .. math::
+        \\begin{align*}
+        \\xi &= [\\xi_1^T \\xi_2]^T \\\\
+        \\text{Expect}(\\xi) &= [\\hat{\\xi_1}^T \\hat{\\xi_2}]^T \\\\
+        \\text{Cov}(\\xi) &= \\begin{bmatrix} \\text{gam11} & \\text{gam12} \\\\ \\text{gam12}^T & \\text{gam22} \\end{bmatrix}
+        \\end{align*}
+
+    Arguments:
+    ----------
+        eps : int | float:
+            The epsilon risk bound in the chance constraint.
+        a : int | float | list | np.ndarray | cp.Variable | cp.Expression, optional:
+            The coefficient vector/scalar "a" in the chance constraint.
+        b : int | float | cp.Variable | cp.Expression, optional:
+            The scalar term "b" in the chance constraint.
+        xi1_hat : int | float | list | np.ndarray | cp.Variable | cp.Expression, optional:
+            The expected value of xi1.
+        xi2_hat : int | float, optional:
+            The expected value of xi2.
+        gam11 : int | float | list | np.ndarray, optional:
+            The covariance matrix of xi1.
+        gam12 : int | float | list | np.ndarray, optional:
+            The cross-covariance matrix between xi1 and xi2.
+        gam22 : int | float, optional:
+            The covariance matrix of xi2.
+        assume_sym : bool, optional:
+            Whether to assume the covariance matrix is symmetric (otherwise, it is checked).
+        assume_psd : bool, optional:
+            Whether to assume the covariance matrix is positive semi-definite (otherwise, it is checked).
+        centrally_symmetric: bool, optional:
+            Flag if distribution is centrally symmetric
+            (Def 3.1 in "On Distributionally Robust Chance-Constrained Linear Programs").
+
+    Returns:
+    --------
+        cvxpy.Constraint or cp.Expression:
+            The reformulated deterministic chance constraint.
 
-    This function reformulates a distributionally robust optimization (DRO) chance constraint (CC) where the distribution is unknown but belongs to a moment based ambiguity set with known mean and covariance:
-    d = [a^T b]^T
-    Expect(d) = [a_hat^T b_hat]^T
-    Cov(d) = [a_cov             ab_cross_cov
-              ab_cross_cov^T    b_cross     ]
-
-    :param eps: The epsilon value in the chance constraint.
-    :type eps: float
-    :param a: The coefficient vector a in the chance constraint.
-    :type a: array_like, optional
-    :param b: The constant term b in the chance constraint.
-    :type b: float, optional
-    :param xi1_hat: The expected value of xi1.
-    :type xi1_hat: array_like, optional
-    :param xi2_hat: The expected value of xi2.
-    :type xi2_hat: array_like, optional
-    :param gam11: The covariance matrix of xi1.
-    :type gam11: array_like, optional
-    :param gam12: The cross-covariance matrix between xi1 and xi2.
-    :type gam12: array_like, optional
-    :param gam22: The covariance matrix of xi2.
-    :type gam22: array_like, optional
-    :param assume_sym: Whether to assume the covariance matrix is symmetric.
-    :type assume_sym: bool, optional
-    :param assume_psd: Whether to assume the covariance matrix is positive semi-definite.
-    :type assume_psd: bool, optional
-    :param centrally_symmetric: Flag if distribution is centrally symmetric (Def 3.1).
-    :type centrally_symmetric: bool, optional
-    :return: The reformulated chance constraint.
-    :rtype: cvxpy.Constraint or cvxpy.Expression
     """
     # check inputs
     inputs = _format_inputs(eps, a, b,
                             xi1_hat, xi2_hat,
                             gam11, gam12, gam22)
 
     if centrally_symmetric:
```

### Comparing `cvxriskopt-0.1.2/cvxRiskOpt/mpc_helpers.py` & `cvxriskopt-0.1.3/cvxRiskOpt/mpc_helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+""""""
 """
 cvxRiskOpt: Risk-Based Optimization tool using CVXPY and CVXPYgen
 Copyright (C) 2024  Sleiman Safaoui
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
@@ -16,32 +17,45 @@
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 GitHub:
 @The-SS
 Email:
 snsafaoui@gmail.com
 sleiman.safaoui@utdallas.edu
-"""
-"""
+
+
+
 Some helper functions for designing and solving MPC problems
 """
 import numpy as np
 import cvxpy as cp
 
 
 def cp_var_mat_to_list(mat: cp.Variable | cp.Parameter, horizon: int):
     """
-    Converts a 1D or 2D cp.Variable matrix to a list of cp.Variable vectors.
-    E.g.
-    (3, 4) matrix where horizon is 4 turns into [(3,), (3,), (3,), (3,)].
-    (3,) of horizon 1 turns into [(3,)]
-    (4,) where 4 is horizon turns into [(), (), (), ()]
-    :param mat: (m, horizon), (horizon, m), (m,), or (horizon,) cp.Variable
-    :param horizon: horizon (e.g. MPC horizon).
-    :return:
+    Converts a 1D or 2D cp.Variable/Parameter matrix to a list of cp.Variable/Parameter vectors.
+
+    Some functions, such as lin_mpc_expect_xQx, require lists or arrays of variables/parameters over time as inputs.
+    This function splits a variable/parameter into a list of variables/parameters.
+    e.g.
+        - (3, 4) matrix where the horizon is 4 --> turns into [(3,), (3,), (3,), (3,)].
+        - (3,) of horizon 1 --> turns into [(3,)]
+        - (4,) where 4 is horizon --> turns into [(), (), (), ()]
+
+    Arguments:
+    ----------
+        mat: cp.Variable | cp.Parameter:
+            (m, horizon), (horizon, m), (m,), or (horizon,) cp.Variable
+        horizon: int:
+            mat horizon, e.g. MPC horizon (to identify the "horizon" dimension in mat)
+
+    Returns:
+    --------
+        list:
+            List of cp.Variables or cp.Parameters
     """
     # Get the shape of u
     shape = mat.shape
 
     # Check the shape of u and generate the list accordingly
     if horizon == 1:
         # If t = 1, return [u]
@@ -55,33 +69,59 @@
     elif len(shape) == 2 and shape[0] == horizon:
         # If t > 1 and shape = (t, m), return [u[0, :], ..., u[t-1, :]]
         return [mat[i, :] for i in range(horizon)]
     else:
         raise ValueError("Input variable u has an unsupported shape.")
 
 
-def expect_cov_x_t(t, A, B,
+def expect_cov_x_t(t: int, A: int | float | np.ndarray, B: int | float | np.ndarray,
                    x0_mean: cp.Variable | cp.Parameter | cp.Expression,
                    x0_cov: np.ndarray,
                    u: list,
                    w_mean: list, w_cov: list):
     """
-    Computes the expected next state E(x_{t}) and its covariance Cov(x_{t})
-    for a linear system x_{t+1} = Ax_t + Bu_t + w_t.
-    E(x_{t}) = A^{t} x0_mean + sum_{i=0}^{t-1} (A^i B u_{t-1-i} + A^i w_{t-1-i}_mean)
-    Cov(x_{t}) = A^{t} x0_cov A^{t}^T + sum_{i=0}^{t-1} (A^i w_{t-1-i}_cov A^i^T)
-    :param t: current time step for x_t (t >= 1)
-    :param A: dynamics matrix
-    :param B: input matrix
-    :param x0_mean: mean state at t=0
-    :param x0_cov: covariance of state at t=0
-    :param u: list of control decision variables
-    :param w_mean: list of noise mean value
-    :param w_cov: list of noise covariance values
-    :return:
+    Computes the expressions for the expected next state :math:`\\mathbb{E}(x_{t})` and its covariance :math:`\\text{Cov}(x_t)`
+    for a linear system :math:`x_{t+1} = Ax_t + Bu_t + w_t`.
+
+    The expected value and covariance are found by recursively applying the dynamics stating from an initial state :math:`x_0`
+    whose mean :math:`\\overline{x}_0` and covariance :math:`\\Sigma_{x_0}` are known.
+    The mean :math:`\\overline{w}` and covariance :math:`\\Sigma_{w}` of the noise must also be known.
+    The terms are computed as follows:
+
+    .. math ::
+        \\begin{align*}
+        \\mathbb{E}(x_{t}) &= A^{t} \\overline{x}_0 + \\sum_{i=0}^{t-1} (A^i B u_{t-1-i} + A^i \\overline{w}_{t-1-i}) \\\\
+        \\text{Cov}(x_{t}) &= A^{t} \\Sigma_{x_0} {A^{t}}^T + \\sum_{i=0}^{t-1} (A^i \\Sigma_{w_{t-1-i}} {A^i}^T)
+        \\end{align*}
+
+    Arguments:
+    ----------
+        t: int:
+            Current time step for x_t (t >= 1)
+        A: int | float | np.ndarray:
+            Dynamics matrix
+        B: int | float | np.ndarray:
+            Input matrix
+        x0_mean: cp.Variable | cp.Parameter | cp.Expression:
+            Mean state at t=0
+        x0_cov: np.ndarray:
+            Covariance of state at t=0
+        u: list:
+            List of control decision variables
+        w_mean: list:
+            List of noise mean value
+        w_cov: list:
+            List of noise covariance values
+
+    Returns:
+    --------
+        cp.Expression:
+            Expected value expression of the state at time t (xt_mean)
+        cp.Expression:
+            Covariance expression of the state at time t (xt_cov)
     """
     if isinstance(A, (int, float)):
         n = 1
     elif isinstance(A, np.ndarray):
         n = A.shape[0]
     else:
         raise ValueError("A can either be a square matrix or a scalar")
@@ -131,56 +171,65 @@
         AiBu = Ai * Bu if n == 1 else Ai @ Bu
         Aiw_mean = Ai * w_mean[t-1-i] if n == 1 else Ai @ w_mean[t-1-i]
         xt_mean = xt_mean + AiBu + Aiw_mean
 
         AcovA = w_cov[t-1-i] * Ai ** 2 if n == 1 else Ai @ w_cov[t-1-i] @ Ai.T
         xt_cov = xt_cov + AcovA
 
-        # if u[0].shape == ():
-        #     xt_mean = xt_mean + Ai @ B * u[t-1-i]
-        # else:
-        #     xt_mean = xt_mean + Ai @ B @ u[t-1-i]
-        # if w_mean[0].shape == ():
-        #     xt_mean = xt_mean + Ai * w_mean[t-1-i]
-        # else:
-        #     xt_mean = xt_mean + Ai @ w_mean[t-1-i]
-        # if w_cov[0].shape == ():
-        #     xt_cov = xt_cov + w_cov[t-1-i] * Ai @ Ai.T
-        # else:
-        #     xt_cov = xt_cov + Ai @ w_cov[t-1-i] @ Ai.T
-
     return xt_mean, xt_cov
 
 
 def lin_mpc_expect_xQx(t: int, horizon: int,
                        A: int | float | np.ndarray, B: int | float | np.ndarray,
                        u: list | cp.Variable,
                        Q: int | float | np.ndarray,
                        x0_mean: cp.Parameter | cp.Variable | cp.Expression,
                        x0_cov: np.ndarray = None,
                        w_mean: list | np.ndarray = None,
                        w_cov: list | np.ndarray = None):
     """
-    Finds the E(x_t^T Q x_t) term
+    Finds the expression for :math:`\\mathbb{E}(x_t^T Q x_t)`, the weighted quadratic state cost at time :math:`t`.
+
+    Finds the expression for :math:`\\mathbb{E}(x_t^T Q x_t)`
     where
-    x_t is a random variable at timestep t in the MPC horizon
+    :math:`x_t` is a random variable (due to the noise) representing the state at timestep :math:`t` in the MPC horizon
     and
     the dynamics are:
-    x_{t+1} = Ax_t + Bu_t + w_t.
-    :param t: current control time step (starting from 0)
-    :param horizon: MPC horizon length
-    :param A: dynamics matrix
-    :param B: input matrix
-    :param u: list of control decision variables (or cp Variable)
-    :param Q: state cost matrix x^T Q x
-    :param x0_mean: mean state at t=0
-    :param x0_cov: covariance of state at t=0
-    :param w_mean: list of noise mean value (or single noise mean)
-    :param w_cov: list of noise covariance values (or single noise covar)
-    :return:
+    :math:`x_{t+1} = Ax_t + Bu_t + w_t`.
+
+    Arguments:
+    ----------
+        t: int:
+            Control time step (starting from 0)
+        horizon: int:
+            MPC horizon length
+        A: int | float | np.ndarray:
+            Dynamics matrix
+        B: int | float | np.ndarray:
+            Input matrix
+        u: list | cp.Variable
+            List of control decision variables (or cp Variable)
+        Q: int | float | np.ndarray:
+            State cost matrix
+        x0_mean: cp.Parameter | cp.Variable | cp.Expression:
+            Mean state at :math:`t=0`
+        x0_cov: np.ndarray, optional:
+            Covariance of state at :math:`t=0`. If not passed, assumed to be zero.
+        w_mean: list | np.ndarray, optional:
+            List of noise mean value (or single noise mean). If not passed, assumed to be zero.
+        w_cov: list | np.ndarray, optional:
+            List of noise covariance values (or single noise covar). If not passed, assumed to be zero.
+
+    Returns:
+    --------
+        cp.Expression:
+            Expression for :math:`\\mathbb{E}(x_t^T Q x_t)`
+        dict:
+            dictionary containing the expressions for the mean and covariance of the state at time :math:`t`
+            ("x_mean", "x_cov")
     """
     # handle optional arguments
     n = x0_mean.shape[0] if x0_mean.ndim > 0 else 1
     if x0_cov is None:
         x0_cov = np.zeros((n, n))
     if w_mean is None:
         w_mean = np.zeros(n)
```

### Comparing `cvxriskopt-0.1.2/cvxRiskOpt/wass_risk_opt_pb.py` & `cvxriskopt-0.1.3/cvxRiskOpt/wass_risk_opt_pb.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+""""""
 """
 cvxRiskOpt: Risk-Based Optimization tool using CVXPY and CVXPYgen
 Copyright (C) 2024  Sleiman Safaoui
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
@@ -16,69 +17,77 @@
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 GitHub:
 @The-SS
 Email:
 snsafaoui@gmail.com
 sleiman.safaoui@utdallas.edu
-"""
-"""
+
+
+
 CVXPY-based data-driven optimization problems that compute risk metrics.
 
 We implement some results from:
 "Data-driven distributionally robust optimization using the Wasserstein metric: 
     Performance guarantees and tractable reformulations"
 """
 import cvxpy as cp
 import numpy as np
 from numbers import Number
 from cvxpy.problems.problem import Problem as CVXPYProb
 from cvxpy.utilities.deterministic import unique_list
-from typing import Dict, List, Optional, Union
+from typing import Union
 
 
 class WassWCEMaxAffine(CVXPYProb):
     """
-    Wasserstein Worst Case Expectation with Max of Affine terms.
+    Wasserstein Worst Case Expectation Problem with Max of Affine Terms.
 
     This class implements a generic solution for Cor 5.1 (i), eq (15a) with affine loss functions:
-    l = max_k {a_k @ xi + b_k}
+
+    .. math::
+
+        \\ell = \\max_k \\{ \\langle a_k,  \\xi \\rangle + b_k \\}
+
     where
-    xi (m x 1): the random variable for which we have samples
-    a_k (m x 1): a vector that is either a constant vector or a scalar times a decision variable (cvxpy affine expression)
-    b_k (1 x 1): a scalar or a 1-dimensional cvxpy affine expression
+        - xi (m x 1): the random variable for which we have samples
+        - a_k (m x 1): a vector that is either a constant vector or a scalar times a decision variable (cvxpy affine expression)
+        - b_k (1 x 1): a scalar or a 1-dimensional cvxpy affine expression
+        - :math:`\\langle \\cdot, \\cdot \\rangle` is the inner product
 
     .. note::
         Currently, this is only implemented for the 1-, 2-, and inf-norm cases.
 
-    :param num_samples: The number of samples.
-    :type num_samples: int
-    :param a_k_list: A list of vectors that are either constant vectors or scalars times a decision variable.
-    :type a_k_list: list of array_like or cvxpy.AffineExpression
-    :param b_k_list: A list of scalars or 1-dimensional cvxpy affine expressions.
-    :type b_k_list: list of float or cvxpy.AffineExpression, optional
-    :param support_C: The support matrix C.
-    :type support_C: array_like, optional
-    :param support_d: The support vector d.
-    :type support_d: array_like, optional
-    :param used_norm: The norm to be used. Default is 2.
-    :type used_norm: int, optional
-    :param vp_suffix: The suffix for the variable prefix.
-    :type vp_suffix: str, optional
+    Arguments:
+    ----------
+        num_samples: int:
+            The number of samples.
+        a_k_list: Number | array_like
+            A list of vectors that are either constant vectors or scalars times a decision variable.
+        b_k_list: array_like
+            A list of scalars or 1-dimensional cvxpy affine expressions.
+        support_C: np.ndarray, optional
+            The support matrix C. If None passed, the support is considered to be the real space.
+        support_d: np.ndarray, optional
+            The support vector d. If None passed, the support is considered to be the real space.
+        used_norm: int | np.inf, optional
+            The norm to be used. Either 1, 2, or infinity (np.inf). Default is 2.
+        vp_suffix: str, optional
+            The suffix for the variable/parameter names.
     """
     instance_counter = 0
 
-    def __init__(self, num_samples,
-                 a_k_list, b_k_list=None,
+    def __init__(self, num_samples: int,
+                 a_k_list: list, b_k_list: list = None,
                  support_C=None, support_d=None, used_norm=2,
-                 vp_suffix=None):
+                 vp_suffix: str = None) -> None:
         # choose the cp variable and parameter suffix
         WassWCEMaxAffine.instance_counter += 1
         if vp_suffix is None:
-            vp_suffix = "_WWCEMA" + str(WassWCEMaxAffine.instance_counter)
+            vp_suffix = "_wwcema" + str(WassWCEMaxAffine.instance_counter)
 
         # number of samples
         self._num_samples = num_samples
 
         # # loss function terms
         # if a_k_list is None or a_k_list == []:
         #     raise ValueError('Problem statement error: a_k_list must be non-empty')
@@ -191,26 +200,75 @@
             if self._use_gamma:
                 constraints += [self._gamma[i] >= 0]
         return constraints
 
     # TODO: consider implementing some operators.
 
 
+def update_wass_wce_params(prob, eps, samples) -> None:
+    """
+    Update the parameters associated with the WassWCEMaxAffine problem.
+
+    Arguments:
+    ----------
+        prob: WassWCEMaxAffine:
+            WassWCEMaxAffine problem
+        eps: int:
+            Wasserstein ball radius
+        samples: np.ndarray:
+            Data samples
+    """
+    for par in prob.param_dict.keys():
+        if 'eps' in par:
+            prob.param_dict[par].value = eps
+        if 'samples' in par:
+            prob.param_dict[par].value = samples
+    return
+
+
 class WassDRExpectation(WassWCEMaxAffine):
     """
-    Provides a high-level implementation of the DR Expectation function.
-    sup_{P in \mathcal{P}} E^P[a * xi + b]
-    where a, b may contain decision variables
+    Provides a high-level implementation of the DR Expectation with a Wasserstein-based ambiguity set.
+
+    Implements
+
+    .. math::
+
+        \\sup_{\\mathbb{P} \\in \\mathcal{P}} \\quad \\mathbb{E}^\\mathbb{P} \\left[ \\langle a, \\xi \\rangle + b \\right]
+
+    where :math:`a, b` may contain decision variables and :math:`\\langle \\cdot, \\cdot \\rangle` is the inner product.
+
+
+    Arguments:
+    ----------
+        num_samples: int:
+            The number of samples.
+        a: int | float | cp.Variable | cp.Parameter | cp.Expression:
+            The "a" term in :math:`\\langle a, xi \\rangle + b`.
+        b: int | float | cp.Variable | cp.Parameter | cp.Expression, optional"
+            The "b" term in :math:`\\langle a, xi \\rangle + b`. If not assigned, 0 is used.
+        support_C: np.ndarray, optional
+            The support matrix C. If None passed, the support is considered to be the real space.
+        support_d: np.ndarray, optional
+            The support vector d. If None passed, the support is considered to be the real space.
+        used_norm: int | np.inf, optional
+            The norm to be used. Either 1, 2, or infinity (np.inf). Default is 2.
+        vp_suffix: str, optional
+            The suffix for the variable/parameter names.
     """
     instance_counter = 0
 
-    def __init__(self, num_samples, a, b=0, support_C=None, support_d=None, used_norm=2, vp_suffix=None):
+    def __init__(self,
+                 num_samples: int,
+                 a: int | float | cp.Variable | cp.Parameter | cp.Expression,
+                 b: int | float | cp.Variable | cp.Parameter | cp.Expression = 0,
+                 support_C=None, support_d=None, used_norm=2, vp_suffix=None):
         WassDRExpectation.instance_counter += 1
         if vp_suffix is None:
-            vp_suffix = "_WDRE" + str(WassDRExpectation.instance_counter)
+            vp_suffix = "_wdre" + str(WassDRExpectation.instance_counter)
         if b == 0:
             b = []
         a = [a]
         super().__init__(num_samples, a, b, support_C, support_d, used_norm, vp_suffix=vp_suffix)
 
     def _problems_match(self, other) -> bool:
         if self._used_norm != other._used_norm:
@@ -300,37 +358,84 @@
 
     # TODO: consider implementing the following
     #   __neg__, __rsub__, __radd__
 
 
 class WassDRCVaR(WassWCEMaxAffine):
     """
-    Provides a high-level implementation of the DR-CVaR function.
-    sup_{P in \mathcal{P}} CVaR^P[a * xi + b]
-    where a, b may contain decision variables
+    Provides a high-level implementation of the DR-CVaR with a Wasserstein-based ambiguity set.
+
+    Implements
+
+    .. math ::
+
+        \\sup_{\\mathbb{P} \\in \\mathcal{P}} \\quad  \\text{CVaR}_{\\alpha}^\\mathbb{P}\\left[ \\langle a, \\xi \\rangle + b \\right]
+
+    where :math:`a, b` may contain decision variables and :math:`\\langle \\cdot, \\cdot \\rangle` is the inner product.
+    :math:`\\alpha` is the CVaR level (average in alpha * 100% of the worst/highest cases)
+
+    Alternatively, this can also implement the CVaR reformulated form as a max of two affine terms:
+
+     .. math ::
+
+        \\sup_{\\mathbb{P} \\in \\mathcal{P}} \\quad  \\mathbb{E}^{\\mathbb{P}} \\max_{k \\in \\{1, 2\\}} \\left[ \\langle a_k, \\xi \\rangle + b_k \\right].
+
+
+    .. Note ::
+
+        Either "a" and "b" must be passed or "a_k_list" and "b_k_list", but not both nor neither.
+
+
+    Arguments:
+    ----------
+        num_samples: int:
+            The number of samples.
+        xi_length: int:
+            Size of a sample. If :math:`\\xi` is m x 1 --> xi_length = m
+        a: int | float | cp.Variable | cp.Parameter | cp.Expression, optional:
+            The "a" term in :math:`\\langle a, xi \\rangle + b`.
+            If this is passed, the "b" term is expected.
+            This should not be passed if "a_k_list" and "b_k_list" are passed.
+        b: int | float | cp.Variable | cp.Parameter | cp.Expression, optional, optional:
+            The "b" term in :math:`\\langle a, xi \\rangle + b`. If not assigned, 0 is used.
+            This should not be passed if "a_k_list" and "b_k_list" are passed.
+        a_k_list: Number | array_like, optional:
+            A list of vectors that are either constant vectors or scalars times a decision variable.
+            If this is passed, the "b_k_list" term is expected.
+            This should not be passed if "a" and "b" are passed.
+        b_k_list: array_like, optional:
+            A list of scalars or 1-dimensional cvxpy affine expressions.
+            This should not be passed if "a" and "b" are passed.
+        alpha: float, optional:
+            CVaR level (average in alpha * 100% of the worst/highest cases)
+        support_C: np.ndarray, optional
+            The support matrix C. If None passed, the support is considered to be the real space.
+        support_d: np.ndarray, optional
+            The support vector d. If None passed, the support is considered to be the real space.
+        used_norm: int | np.inf, optional
+            The norm to be used. Either 1, 2, or infinity (np.inf). Default is 2.
+        vp_suffix: str, optional
+            The suffix for the variable/parameter names.
+
     """
     instance_counter = 0
 
-    def __init__(self, num_samples, xi_length, a=None, b=0, a_k_list=None, b_k_list=None, alpha=0.1, support_C=None,
-                 support_d=None, used_norm=2, vp_suffix=None):
-        """
-        :param num_samples:
-        :param a: a term in a * xi + b
-        :param b: b term in a * xi + b
-        :param a_k_list: a_k_list used in WassWCEMaxAffine
-        :param b_k_list: b_k_list used in WassWCEMaxAffine
-        :param alpha: CVaR level (average in alpha * 100% of the worst/highest cases)
-        :param xi_length: size of a sample. If xi is m x 1 --> xi_length = m
-        :param support_C: C term in support of random variable {xi | C*xi <= d}
-        :param support_d: d term in support of random variable {xi | C*xi <= d}
-        :param used_norm: norm being used
-        """
+    def __init__(self,
+                 num_samples: int, xi_length: int,
+                 a: int | float | cp.Variable | cp.Parameter | cp.Expression = None,
+                 b: int | float | cp.Variable | cp.Parameter | cp.Expression = 0,
+                 a_k_list=None,
+                 b_k_list=None,
+                 alpha=0.1,
+                 support_C=None, support_d=None,
+                 used_norm=2, vp_suffix=None):
+
         WassDRCVaR.instance_counter += 1
         if vp_suffix is None:
-            vp_suffix = "_WDRCVAR" + str(WassDRCVaR.instance_counter)
+            vp_suffix = "_wdrcvar" + str(WassDRCVaR.instance_counter)
 
         self._alpha = alpha
 
         if a is None and (a_k_list is None or b_k_list is None):
             raise ValueError(
                 'Option 1: provide a (optionally b). Option 2: provided a_k_list and b_k_list. Both failed.')
         if a is None:
```

### Comparing `cvxriskopt-0.1.2/cvxRiskOpt.egg-info/PKG-INFO` & `cvxriskopt-0.1.3/cvxRiskOpt.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxRiskOpt
-Version: 0.1.2
+Version: 0.1.3
 Summary: Risk-Based Optimization tool using CVXPY and CVXPYgen
 Home-page: https://github.com/TSummersLab/cvxRiskOpt
 Author: Sleiman Safaoui, Tyler Summers
 Author-email: snsafaoui@gmail.com, tyler.summers@utdallas.edu
 Maintainer: Sleiman Safaoui
 Maintainer-email: snsafaoui@gmail.com
 License: GPL-3.0
@@ -24,39 +24,38 @@
 
 # CVXPY Risk Optimization
 
 A package for risk-based optimization using CVXPY and CVXPYgen.
 
 ## Installation
 
-- create and activate conda env 
+### Installing from PyPI
+The package can be installed using pip:
 ```
-conda create --name cvxRiskOpt python=3.10 pip -y
-conda activate cvxRiskOpt
-```
-- install dependencies
+pip install cvxRiskOpt
 ```
-pip install cvxpy>=1.4.1
-pip install cvxpygen>=0.3.4
-pip install scipy>=1.11.4
-pip install numpy>=1.26.2
-pip install matplotlib>=3.8.0
+Notes:
+- The installation will also include cvxpy and cvxpygen.
+- Please refer to cvxpy's documentation for [installing additional solvers](https://www.cvxpy.org/install/).
+- Compiling code with Clarabel requires `Rust`, `Eigen`, and `cbindgen`. (e.g. These can be installed with `homebrew` on MacOS) 
+
+### Installing from source
+- Clone/Download the package
+- Create and activate conda env 
 ```
-For development, also install:
-```
-pip install pytest==7.4.0
-pip install polytope==0.2.5
-pip install Sphinx==7.2.6
+conda create --name cvxRiskOpt python=3.10 pip -y
+conda activate cvxRiskOpt
 ```
-- install the package
+- Install dependencies (see `setup.py`)
+- Install the package
 ```
 python3 -m pip install -e .
 ```
 
 ## Tests
-To run tests,
+To run tests, execute the following from the root of the package.
 ```
 pytest
 ```
 
 ## Examples
-There are several examples in `examples` demonstrating the usage of the package's functionality.
+There are several examples in `examples` demonstrating the usage of the package.
```

### Comparing `cvxriskopt-0.1.2/setup.py` & `cvxriskopt-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup
 
 setup(
     name="cvxRiskOpt",
-    version="0.1.2",
+    version="0.1.3",
     description="Risk-Based Optimization tool using CVXPY and CVXPYgen",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Sleiman Safaoui, Tyler Summers",
     author_email="snsafaoui@gmail.com, tyler.summers@utdallas.edu",
     maintainer="Sleiman Safaoui",
     maintainer_email="snsafaoui@gmail.com",
```

### Comparing `cvxriskopt-0.1.2/tests/test_cclp_risk_opt.py` & `cvxriskopt-0.1.3/tests/test_cclp_risk_opt.py`

 * *Files identical despite different names*

### Comparing `cvxriskopt-0.1.2/tests/test_mpc_helpers_functions.py` & `cvxriskopt-0.1.3/tests/test_mpc_helpers_functions.py`

 * *Files identical despite different names*

### Comparing `cvxriskopt-0.1.2/tests/test_wass_risk_opt_pb.py` & `cvxriskopt-0.1.3/tests/test_wass_risk_opt_pb.py`

 * *Files identical despite different names*


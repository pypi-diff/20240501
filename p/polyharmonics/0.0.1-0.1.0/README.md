# Comparing `tmp/polyharmonics-0.0.1.tar.gz` & `tmp/polyharmonics-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyharmonics-0.0.1.tar", max compression
+gzip compressed data, was "polyharmonics-0.1.0.tar", max compression
```

## Comparing `polyharmonics-0.0.1.tar` & `polyharmonics-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rwxr-xr-x   0        0        0    32471 2024-04-10 16:50:33.469033 polyharmonics-0.0.1/LICENSE
--rwxr-xr-x   0        0        0     6305 2024-04-13 10:48:02.826181 polyharmonics-0.0.1/README.md
--rwxr-xr-x   0        0        0      403 2024-04-15 11:58:59.989064 polyharmonics-0.0.1/polyharmonics/__init__.py
--rwxr-xr-x   0        0        0     2902 2024-04-15 12:10:22.993856 polyharmonics-0.0.1/polyharmonics/__main__.py
--rwxr-xr-x   0        0        0     5116 2024-04-15 12:09:05.898982 polyharmonics-0.0.1/polyharmonics/legendre_polynomials.py
--rwxr-xr-x   0        0        0     3438 2024-04-12 19:48:02.557955 polyharmonics-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     7788 1970-01-01 00:00:00.000000 polyharmonics-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1466 2024-04-16 13:33:46.000000 polyharmonics-0.1.0/LICENSE
+-rwxr-xr-x   0        0        0     6272 2024-05-01 17:53:48.000000 polyharmonics-0.1.0/README.md
+-rwxr-xr-x   0        0        0      466 2024-05-01 18:06:30.000000 polyharmonics-0.1.0/polyharmonics/__init__.py
+-rwxr-xr-x   0        0        0     7681 2024-05-01 18:09:26.000000 polyharmonics-0.1.0/polyharmonics/__main__.py
+-rwxr-xr-x   0        0        0     6679 2024-05-01 18:08:21.000000 polyharmonics-0.1.0/polyharmonics/associated_legendre_functions.py
+-rwxr-xr-x   0        0        0     5068 2024-05-01 18:08:29.000000 polyharmonics-0.1.0/polyharmonics/legendre_polynomials.py
+-rwxr-xr-x   0        0        0     3438 2024-04-27 09:22:00.000000 polyharmonics-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7757 1970-01-01 00:00:00.000000 polyharmonics-0.1.0/PKG-INFO
```

### Comparing `polyharmonics-0.0.1/README.md` & `polyharmonics-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,28 +21,33 @@
 
 Conda package manager is recommended. Create a conda environment.
 
 ```bash
 conda create -n polyharmonics python==3.10
 ```
 
-Activate conda environment and install poetry
+Activate conda environment
 
 ```bash
 conda activate polyharmonics
-pip install poetry
 ```
 
-Install with `make install`. Then you can run the client using the following command:
+Install the package
+
+```bash
+pip install polyharmonics
+```
+
+Then you can run the client using the following command:
 
 ```bash
 polyharmonics --help
 ```
 
-or with `Poetry`:
+Or with `Poetry`:
 
 ```bash
 poetry run polyharmonics --help
 ```
 
 ### Makefile usage
 
@@ -226,15 +231,15 @@
 
 GitHub creates the `bug`, `enhancement`, and `documentation` labels for you. Dependabot creates the `dependencies` label. Create the remaining labels on the Issues tab of your GitHub repository, when you need them.
 
 ## 🛡 License
 
 [![License](https://img.shields.io/github/license/ComicIvans/polyharmonics)](https://github.com/ComicIvans/polyharmonics/blob/main/LICENSE)
 
-This project is licensed under the terms of the `GNU GPL v3.0` license. See [LICENSE](https://github.com/ComicIvans/polyharmonics/blob/main/LICENSE) for more details.
+This project uses the `BSD-3-Clause` license. See [LICENSE](https://github.com/ComicIvans/polyharmonics/blob/main/LICENSE) for more details.
 
 ## 📃 Citation
 
 ```bibtex
 @misc{polyharmonics,
   author = {Iván Salido Cobo},
   title = {Ortogonal Polynomials in the unit sphere.},
```

### Comparing `polyharmonics-0.0.1/polyharmonics/legendre_polynomials.py` & `polyharmonics-0.1.0/polyharmonics/legendre_polynomials.py`

 * *Files 16% similar despite different names*

```diff
@@ -52,29 +52,27 @@
                 multinomial=False,
                 power_exp=False,
                 power_base=False,
                 log=False,
             )
 
 
-def legendre_rec(
-    n: int, store: bool = True, prevPol: Expr = None, callback: bool = False
-):
+def legendre_rec(n: int, store: bool = True, callback: bool = False):
     if n == 0:
         return x**0
     elif n == 1:
         if callback:
             return x**1, x**0
         else:
             return x**1
     else:
         if store:
             if len(LEGENDRE_REC_STORE) <= n:
                 if len(LEGENDRE_REC_STORE) < n:
-                    legendre_rec(n - 1, store=True)
+                    legendre_rec(n - 1, store=store)
                 LEGENDRE_REC_STORE.append(
                     expand(
                         (
                             (2 * n - 1) * x * LEGENDRE_REC_STORE[n - 1]
                             - (n - 1) * LEGENDRE_REC_STORE[n - 2]
                         )
                         / n,
@@ -84,33 +82,31 @@
                         power_exp=False,
                         power_base=False,
                         log=False,
                     ),
                 )
             return LEGENDRE_REC_STORE[n]
         else:
-            currPol, prevPol = legendre_rec(
-                n - 1, store=False, prevPol=None, callback=True
-            )
+            curr_pol, prev_pol = legendre_rec(n - 1, store=store, callback=True)
             if callback:
                 return (
                     expand(
-                        ((2 * n - 1) * x * currPol - (n - 1) * prevPol) / n,
+                        ((2 * n - 1) * x * curr_pol - (n - 1) * prev_pol) / n,
                         deep=True,
                         mul=True,
                         multinomial=False,
                         power_exp=False,
                         power_base=False,
                         log=False,
                     ),
-                    currPol,
+                    curr_pol,
                 )
             else:
                 return expand(
-                    ((2 * n - 1) * x * currPol - (n - 1) * prevPol) / n,
+                    ((2 * n - 1) * x * curr_pol - (n - 1) * prev_pol) / n,
                     deep=True,
                     mul=True,
                     multinomial=False,
                     power_exp=False,
                     power_base=False,
                     log=False,
                 )
@@ -130,19 +126,19 @@
     Examples:
         .. code:: python
 
             >>> legendre(1)
             x
             >>> legendre([0, 1])
             [1, x]
-    """
+    """  # noqa: E501
     if isinstance(n, int):
         if n < 0:
             raise ValueError("Degree n must be greater than or equal to 0")
         return legendre_rec(n, store=False)
     elif isinstance(n, list):
         if any(i < 0 for i in n):
             raise ValueError("All degrees n must be greater than or equal to 0")
-        store = len(n) > 1
+        store: bool = len(n) > 1
         return [legendre_rec(i, store=store) for i in n]
     else:
         raise TypeError("n must be an integer or a list of integers")
```

### Comparing `polyharmonics-0.0.1/pyproject.toml` & `polyharmonics-0.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polyharmonics"
-version = "0.0.1"
+version = "0.1.0"
 description = "Ortogonal polynomials in the unit sphere"
 readme = "README.md"
 authors = [
   "Iván Salido Cobo <isalidocobo@gmail.com>",
 ]
-license = "GNU GPL v3.0"
+license = "BSD-3-Clause"
 repository = "https://github.com/ComicIvans/polyharmonics"
 homepage = "https://github.com/ComicIvans/polyharmonics"
 
 # Keywords description https://python-poetry.org/docs/pyproject/#keywords
 keywords = [
   "python",
   "polynomials",
@@ -57,15 +57,15 @@
 numpy = "^1.26.4"
 
 [tool.poetry.dev-dependencies]
 pytest = "^8.1.1"
 pytest-html = "^4.1.1"
 pytest-cov = "^5.0.0"
 bandit = "^1.7.1"
-ruff = "^0.3.5"
+ruff = "^0.4.1"
 pre-commit = "^3.5.0"
 coverage = "^7.4.4"
 coverage-badge = "^1.1.0"
 
 
 
 [tool.ruff]
```

### Comparing `polyharmonics-0.0.1/PKG-INFO` & `polyharmonics-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: polyharmonics
-Version: 0.0.1
+Version: 0.1.0
 Summary: Ortogonal polynomials in the unit sphere
 Home-page: https://github.com/ComicIvans/polyharmonics
-License: GNU GPL v3.0
+License: BSD-3-Clause
 Keywords: python,polynomials,unit sphere,orthogonal polynomials,mathematics,math,legendre polynomials,associated legendre functions,spherical harmonics
 Author: Iván Salido Cobo
 Author-email: isalidocobo@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Mathematics
@@ -53,28 +53,33 @@
 
 Conda package manager is recommended. Create a conda environment.
 
 ```bash
 conda create -n polyharmonics python==3.10
 ```
 
-Activate conda environment and install poetry
+Activate conda environment
 
 ```bash
 conda activate polyharmonics
-pip install poetry
 ```
 
-Install with `make install`. Then you can run the client using the following command:
+Install the package
+
+```bash
+pip install polyharmonics
+```
+
+Then you can run the client using the following command:
 
 ```bash
 polyharmonics --help
 ```
 
-or with `Poetry`:
+Or with `Poetry`:
 
 ```bash
 poetry run polyharmonics --help
 ```
 
 ### Makefile usage
 
@@ -258,15 +263,15 @@
 
 GitHub creates the `bug`, `enhancement`, and `documentation` labels for you. Dependabot creates the `dependencies` label. Create the remaining labels on the Issues tab of your GitHub repository, when you need them.
 
 ## 🛡 License
 
 [![License](https://img.shields.io/github/license/ComicIvans/polyharmonics)](https://github.com/ComicIvans/polyharmonics/blob/main/LICENSE)
 
-This project is licensed under the terms of the `GNU GPL v3.0` license. See [LICENSE](https://github.com/ComicIvans/polyharmonics/blob/main/LICENSE) for more details.
+This project uses the `BSD-3-Clause` license. See [LICENSE](https://github.com/ComicIvans/polyharmonics/blob/main/LICENSE) for more details.
 
 ## 📃 Citation
 
 ```bibtex
 @misc{polyharmonics,
   author = {Iván Salido Cobo},
   title = {Ortogonal Polynomials in the unit sphere.},
```


# Comparing `tmp/pycaleva-0.7.0.tar.gz` & `tmp/pycaleva-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycaleva-0.7.0.tar", last modified: Wed Dec  7 08:50:18 2022, max compression
+gzip compressed data, was "pycaleva-0.8.0.tar", last modified: Wed May  1 19:26:30 2024, max compression
```

## Comparing `pycaleva-0.7.0.tar` & `pycaleva-0.8.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-12-07 08:50:18.258319 pycaleva-0.7.0/
--rw-rw-rw-   0        0        0     1549 2022-02-27 11:25:09.000000 pycaleva-0.7.0/LICENSE
--rw-rw-rw-   0        0        0     7148 2022-12-07 08:50:18.259319 pycaleva-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     6355 2022-05-21 12:02:13.000000 pycaleva-0.7.0/README.md
--rw-rw-rw-   0        0        0       86 2022-12-07 08:50:18.263321 pycaleva-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1363 2022-12-07 08:16:30.000000 pycaleva-0.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-07 08:50:18.226312 pycaleva-0.7.0/src/
-drwxrwxrwx   0        0        0        0 2022-12-07 08:50:18.246317 pycaleva-0.7.0/src/pycaleva/
--rw-rw-rw-   0        0        0       81 2022-05-21 12:54:54.000000 pycaleva-0.7.0/src/pycaleva/__init__.py
--rw-rw-rw-   0        0        0    36822 2022-12-07 08:20:25.000000 pycaleva-0.7.0/src/pycaleva/_basecalib.py
--rw-rw-rw-   0        0        0     6226 2022-03-01 20:46:48.000000 pycaleva-0.7.0/src/pycaleva/_report.py
--rw-rw-rw-   0        0        0      567 2022-03-08 19:33:00.000000 pycaleva-0.7.0/src/pycaleva/_result_types.py
--rw-rw-rw-   0        0        0    21068 2022-05-21 12:54:03.000000 pycaleva-0.7.0/src/pycaleva/calbelt.py
--rw-rw-rw-   0        0        0      948 2022-12-07 08:20:31.000000 pycaleva-0.7.0/src/pycaleva/calibeval.py
--rw-rw-rw-   0        0        0     1794 2022-12-07 08:18:23.000000 pycaleva-0.7.0/src/pycaleva/metrics.py
-drwxrwxrwx   0        0        0        0 2022-12-07 08:50:18.257321 pycaleva-0.7.0/src/pycaleva.egg-info/
--rw-rw-rw-   0        0        0     7148 2022-12-07 08:50:17.000000 pycaleva-0.7.0/src/pycaleva.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2022-12-07 08:50:18.000000 pycaleva-0.7.0/src/pycaleva.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-07 08:50:17.000000 pycaleva-0.7.0/src/pycaleva.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      131 2022-12-07 08:50:17.000000 pycaleva-0.7.0/src/pycaleva.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-12-07 08:50:17.000000 pycaleva-0.7.0/src/pycaleva.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-01 19:26:30.187409 pycaleva-0.8.0/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1520 2024-05-01 18:08:29.000000 pycaleva-0.8.0/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)     7394 2024-05-01 19:26:30.187409 pycaleva-0.8.0/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     6571 2024-05-01 18:30:48.000000 pycaleva-0.8.0/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)       79 2024-05-01 19:26:30.191409 pycaleva-0.8.0/setup.cfg
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1321 2024-05-01 18:46:24.000000 pycaleva-0.8.0/setup.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-01 19:26:30.187409 pycaleva-0.8.0/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-01 19:26:30.187409 pycaleva-0.8.0/src/pycaleva/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       80 2024-05-01 18:08:29.000000 pycaleva-0.8.0/src/pycaleva/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    36030 2024-05-01 19:21:29.000000 pycaleva-0.8.0/src/pycaleva/_basecalib.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     6056 2024-05-01 18:48:50.000000 pycaleva-0.8.0/src/pycaleva/_report.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      556 2024-05-01 18:08:29.000000 pycaleva-0.8.0/src/pycaleva/_result_types.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    20495 2024-05-01 18:08:29.000000 pycaleva-0.8.0/src/pycaleva/calbelt.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      925 2024-05-01 18:08:29.000000 pycaleva-0.8.0/src/pycaleva/calibeval.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1751 2024-05-01 18:08:29.000000 pycaleva-0.8.0/src/pycaleva/metrics.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2024-05-01 19:26:30.187409 pycaleva-0.8.0/src/pycaleva.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     7394 2024-05-01 19:26:30.000000 pycaleva-0.8.0/src/pycaleva.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      395 2024-05-01 19:26:30.000000 pycaleva-0.8.0/src/pycaleva.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2024-05-01 19:26:30.000000 pycaleva-0.8.0/src/pycaleva.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      124 2024-05-01 19:26:30.000000 pycaleva-0.8.0/src/pycaleva.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        9 2024-05-01 19:26:30.000000 pycaleva-0.8.0/src/pycaleva.egg-info/top_level.txt
```

### Comparing `pycaleva-0.7.0/LICENSE` & `pycaleva-0.8.0/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-BSD 3-Clause License
-
-Copyright (c) 2022, Martin Weigl
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2022, Martin Weigl
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `pycaleva-0.7.0/PKG-INFO` & `pycaleva-0.8.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,174 +1,148 @@
-Metadata-Version: 2.1
-Name: pycaleva
-Version: 0.7.0
-Summary: A framework for calibration evaluation of binary classification models
-Home-page: https://github.com/MartinWeigl/pycaleva
-Author: Martin Weigl
-Author-email: martinweigl48@gmail.com
-Project-URL: Source, https://github.com/MartinWeigl/pycaleva
-Project-URL: Documentation, https://martinweigl.github.io/pycaleva/
-Keywords: calibration,classification,model,machine_learning,statistics
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![](https://martinweigl.github.io/pycaleva/assets/logo.svg)](https://martinweigl.github.io/pycaleva/)
-
-[Documentation]: https://martinweigl.github.io/pycaleva/
-
-### A framework for calibration evaluation of binary classification models. 
-- - -
-
-When performing classification tasks you sometimes want to obtain the probability of a class label instead of the class label itself. For example, it might be interesting to determine the risk of cancer for a patient. It is desireable to have a calibrated model which delivers predicted probabilities very close to the actual class membership probabilities. For this reason, this framework was developed allowing users to **measure the calibration of binary classification models**.
-
-- Evaluate the calibration of binary classification models with probabilistic output (LogisticRegression, SVM, NeuronalNets ...).  
-- Apply your model to testdata and use true class labels and predicted probabilities as input for the framework.  
-- Various statistical tests, metrics and plots are available.  
-- Supports creating a calibration report in pdf-format for your model.
-
-\
-<img src="https://martinweigl.github.io/pycaleva/assets/design.png" width="600" alt="Image Design">
-\
-\
-See the [documentation] for detailed information about classes and methods.
-
-
-
-Installation
-------------
-
-
-    $ pip install pycaleva
-
-or build on your own
-
-    $ git clone https://github.com/MartinWeigl/pycaleva.git
-    $ cd pycaleva
-    $ python setup.py install
-
-
-Requirements
-------------
-- numpy>=1.17
-- scipy>=1.3
-- matplotlib>=3.1
-- tqdm>=4.40
-- pandas>=1.3.0
-- statsmodels>=0.13.1
-- fpdf2>=2.5.0
-- ipython>=7.30.1
-
-
-Usage
------
-
-- Import and initialize  
-    ```python
-    from pycaleva import CalibrationEvaluator
-    ce = CalibrationEvaluator(y_test, pred_prob, outsample=True, n_groups='auto')
-    ```
-- Apply statistical tests
-    ```python
-    ce.hosmerlemeshow()     # Hosmer Lemeshow Test
-    ce.pigeonheyse()        # Pigeon Heyse Test
-    ce.z_test()             # Spiegelhalter z-Test
-    ce.calbelt(plot=False)  # Calibrationi Belt (Test only)
-    ```
-- Show calibration plot
-    ```python
-    ce.calibration_plot()
-    ```
-- Show calibration belt
-    ```python
-    ce.calbelt(plot=True)
-    ```
-- Get various metrics
-    ```python
-    ce.metrics()
-    ```
-- Create pdf calibration report
-    ```python
-    ce.calibration_report('report.pdf', 'my_model')
-    ```
-
-See  the [documentation] of single methods for detailed usage examples.
-
-Example Results
----------------
-| Well calibrated model | Poorly calibrated model |
-| :---: | :---: |
-| <img src="https://martinweigl.github.io/pycaleva/assets/calplot_well.png" width="65%" alt="Image Calibration plot well calibrated">  |  <img src="https://martinweigl.github.io/pycaleva/assets/calplot_poorly.png" width="65%" alt="Image Calibration plot poorly calibrated"> |
-| <img src="https://martinweigl.github.io/pycaleva/assets/calbelt_well.png" width="65%" alt="Image Calibration belt well calibrated">  |  <img src="https://martinweigl.github.io/pycaleva/assets/calbelt_poorly.png" width="65%" alt="Image Calibration belt well calibrated"> |
-| <pre lang="python">hltest_result(statistic=4.982635477424991, pvalue=0.8358193332183672, dof=9)</pre> | <pre lang="python">hltest_result(statistic=26.32792475118742, pvalue=0.0018051545107069522, dof=9)</pre> |
-| <pre lang="python">ztest_result(statistic=-0.21590257919669287, pvalue=0.829063686607032)</pre> | <pre lang="python">ztest_result(statistic=-3.196125145498827, pvalue=0.0013928668407116645)</pre> |
-
-
-Features
---------
-* Statistical tests for binary model calibration
-    * Hosmer Lemeshow Test
-    * Pigeon Heyse Test
-    * Spiegelhalter z-test
-    * Calibration belt
-* Graphical represantions showing calibration of binary models
-    * Calibration plot
-    * Calibration belt
-* Various Metrics
-    * Brier Score
-    * Adaptive Calibration Error
-    * Maximum Calibration Error
-    * Area within LOWESS Curve
-    * (AUROC)
-
-The above features are explained in more detail in PyCalEva's [documentation]
-
-
-References
-----------
-- **Statistical tests and metrics**:  
-
-    [1] Hosmer Jr, David W., Stanley Lemeshow, and Rodney X. Sturdivant.
-        Applied logistic regression. Vol. 398. John Wiley & Sons, 2013.
-
-    [2] Pigeon, Joseph G., and Joseph F. Heyse.
-        An improved goodness of fit statistic for probability prediction models.
-        Biometrical Journal: Journal of Mathematical Methods in Biosciences 41.1 (1999): 71-82.
-
-    [3] Spiegelhalter, D. J. (1986). Probabilistic prediction in patient management and clinical trials.
-        Statistics in medicine, 5(5), 421-433.
-
-    [4] Huang, Y., Li, W., Macheret, F., Gabriel, R. A., & Ohno-Machado, L. (2020).
-        A tutorial on calibration measurements and calibration models for clinical prediction models.
-        Journal of the American Medical Informatics Association, 27(4), 621-633.
-
-    
-- **Calibration plot**:  
-
-    [5] Jr, F. E. H. (2021). rms: Regression modeling strategies (R package version
-        6.2-0) [Computer software]. The Comprehensive R Archive Network.
-        Available from https://CRAN.R-project.org/package=rms
-
-- **Calibration belt**:  
-
-    [6] Nattino, G., Finazzi, S., & Bertolini, G. (2014). A new calibration test 
-        and a reappraisal of the calibration belt for the assessment of prediction models 
-        based on dichotomous outcomes. Statistics in medicine, 33(14), 2390-2407.
-
-    [7] Bulgarelli, L. (2021). calibrattion-belt: Assessment of calibration in binomial prediction models [Computer software].
-        Available from https://github.com/fabiankueppers/calibration-framework
-
-    [8] Nattino, G., Finazzi, S., Bertolini, G., Rossi, C., & Carrara, G. (2017).
-        givitiR: The giviti calibration test and belt (R package version 1.3) [Computer
-        software]. The Comprehensive R Archive Network.
-        Available from https://CRAN.R-project.org/package=givitiR
-
-- **Others**:  
-
-    [9] Sturges, H. A. (1926). The choice of a class interval. 
-        Journal of the american statistical association, 21(153), 65-66.
-
-For most of the implemented methods in this software you can find references in the [documentation] as well.
+[![](https://martinweigl.github.io/pycaleva/assets/logo.svg)](https://martinweigl.github.io/pycaleva/)
+
+[Documentation]: https://martinweigl.github.io/pycaleva/
+
+### A framework for calibration evaluation of binary classification models.
+
+---
+
+When performing classification tasks you sometimes want to obtain the probability of a class label instead of the class label itself. For example, it might be interesting to determine the risk of cancer for a patient. It is desireable to have a calibrated model which delivers predicted probabilities very close to the actual class membership probabilities. For this reason, this framework was developed allowing users to **measure the calibration of binary classification models**.
+
+- Evaluate the calibration of binary classification models with probabilistic output (LogisticRegression, SVM, NeuronalNets ...).
+- Apply your model to testdata and use true class labels and predicted probabilities as input for the framework.
+- Various statistical tests, metrics and plots are available.
+- Supports creating a calibration report in pdf-format for your model.
+
+\
+<img src="https://martinweigl.github.io/pycaleva/assets/design.png" width="600" alt="Image Design">
+\
+\
+See the [documentation] for detailed information about classes and methods.
+
+## Installation
+
+    $ pip install pycaleva
+
+or build on your own
+
+    $ git clone https://github.com/MartinWeigl/pycaleva.git
+    $ cd pycaleva
+    $ python setup.py install
+
+## Requirements
+
+- numpy>=1.26
+- scipy>=1.13
+- scikit-learn>=1.4
+- matplotlib>=3.8
+- tqdm>=4.66
+- pandas>=2.2
+- statsmodels>=0.14
+- fpdf2>=2.7
+- ipython>=8.24
+
+## Usage
+
+- Import and initialize
+  ```python
+  from pycaleva import CalibrationEvaluator
+  ce = CalibrationEvaluator(y_test, pred_prob, outsample=True, n_groups='auto')
+  ```
+- Apply statistical tests
+  ```python
+  ce.hosmerlemeshow()     # Hosmer Lemeshow Test
+  ce.pigeonheyse()        # Pigeon Heyse Test
+  ce.z_test()             # Spiegelhalter z-Test
+  ce.calbelt(plot=False)  # Calibrationi Belt (Test only)
+  ```
+- Show calibration plot
+  ```python
+  ce.calibration_plot()
+  ```
+- Show calibration belt
+  ```python
+  ce.calbelt(plot=True)
+  ```
+- Get various metrics
+  ```python
+  ce.metrics()
+  ```
+- Create pdf calibration report
+  ```python
+  ce.calibration_report('report.pdf', 'my_model')
+  ```
+
+See the [documentation] of single methods for detailed usage examples.
+
+## Example Results
+
+|                                                        Well calibrated model                                                        |                                                         Poorly calibrated model                                                         |
+| :---------------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------------: |
+| <img src="https://martinweigl.github.io/pycaleva/assets/calplot_well.png" width="65%" alt="Image Calibration plot well calibrated"> | <img src="https://martinweigl.github.io/pycaleva/assets/calplot_poorly.png" width="65%" alt="Image Calibration plot poorly calibrated"> |
+| <img src="https://martinweigl.github.io/pycaleva/assets/calbelt_well.png" width="65%" alt="Image Calibration belt well calibrated"> |  <img src="https://martinweigl.github.io/pycaleva/assets/calbelt_poorly.png" width="65%" alt="Image Calibration belt well calibrated">  |
+|                <pre lang="python">hltest_result(statistic=4.982635477424991, pvalue=0.8358193332183672, dof=9)</pre>                |                <pre lang="python">hltest_result(statistic=26.32792475118742, pvalue=0.0018051545107069522, dof=9)</pre>                 |
+|                   <pre lang="python">ztest_result(statistic=-0.21590257919669287, pvalue=0.829063686607032)</pre>                   |                    <pre lang="python">ztest_result(statistic=-3.196125145498827, pvalue=0.0013928668407116645)</pre>                    |
+
+## Features
+
+- Statistical tests for binary model calibration
+  - Hosmer Lemeshow Test
+  - Pigeon Heyse Test
+  - Spiegelhalter z-test
+  - Calibration belt
+- Graphical represantions showing calibration of binary models
+  - Calibration plot
+  - Calibration belt
+- Various Metrics
+  - Brier Score
+  - Adaptive Calibration Error
+  - Maximum Calibration Error
+  - Area within LOWESS Curve
+  - (AUROC)
+
+The above features are explained in more detail in PyCalEva's [documentation]
+
+## References
+
+- **Statistical tests and metrics**:
+
+  [1] Hosmer Jr, David W., Stanley Lemeshow, and Rodney X. Sturdivant.
+  Applied logistic regression. Vol. 398. John Wiley & Sons, 2013.
+
+  [2] Pigeon, Joseph G., and Joseph F. Heyse.
+  An improved goodness of fit statistic for probability prediction models.
+  Biometrical Journal: Journal of Mathematical Methods in Biosciences 41.1 (1999): 71-82.
+
+  [3] Spiegelhalter, D. J. (1986). Probabilistic prediction in patient management and clinical trials.
+  Statistics in medicine, 5(5), 421-433.
+
+  [4] Huang, Y., Li, W., Macheret, F., Gabriel, R. A., & Ohno-Machado, L. (2020).
+  A tutorial on calibration measurements and calibration models for clinical prediction models.
+  Journal of the American Medical Informatics Association, 27(4), 621-633.
+
+- **Calibration plot**:
+
+  [5] Jr, F. E. H. (2021). rms: Regression modeling strategies (R package version
+  6.2-0) [Computer software]. The Comprehensive R Archive Network.
+  Available from https://CRAN.R-project.org/package=rms
+
+- **Calibration belt**:
+
+  [6] Nattino, G., Finazzi, S., & Bertolini, G. (2014). A new calibration test
+  and a reappraisal of the calibration belt for the assessment of prediction models
+  based on dichotomous outcomes. Statistics in medicine, 33(14), 2390-2407.
+
+  [7] Bulgarelli, L. (2021). calibrattion-belt: Assessment of calibration in binomial prediction models [Computer software].
+  Available from https://github.com/fabiankueppers/calibration-framework
+
+  [8] Nattino, G., Finazzi, S., Bertolini, G., Rossi, C., & Carrara, G. (2017).
+  givitiR: The giviti calibration test and belt (R package version 1.3) [Computer
+  software]. The Comprehensive R Archive Network.
+  Available from https://CRAN.R-project.org/package=givitiR
+
+- **Others**:
+
+  [9] Sturges, H. A. (1926). The choice of a class interval.
+  Journal of the american statistical association, 21(153), 65-66.
+
+For most of the implemented methods in this software you can find references in the [documentation] as well.
```

### Comparing `pycaleva-0.7.0/src/pycaleva/_basecalib.py` & `pycaleva-0.8.0/src/pycaleva/_basecalib.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,888 +1,888 @@
-"""
-A framework for calibration assessment of binary classification models 
-written in Python.
-
-References
-----------
-[1] Hosmer Jr, David W., Stanley Lemeshow, and Rodney X. Sturdivant.
-        Applied logistic regression. Vol. 398. John Wiley & Sons, 2013.
-
-[2] Pigeon, Joseph G., and Joseph F. Heyse.
-    An improved goodness of fit statistic for probability prediction models.
-    Biometrical Journal: Journal of Mathematical Methods in Biosciences 41.1 (1999): 71-82.
-
-[3] Spiegelhalter, D. J. (1986). Probabilistic prediction in patient management and clinical trials.
-    Statistics in medicine, 5(5), 421-433.
-
-[4] Huang, Y., Li, W., Macheret, F., Gabriel, R. A., & Ohno-Machado, L. (2020).
-    A tutorial on calibration measurements and calibration models for clinical prediction models.
-    Journal of the American Medical Informatics Association, 27(4), 621-633.
-
-[5] Jr, F. E. H. (2021). rms: Regression modeling strategies (R package version
-    6.2-0) [Computer software]. The Comprehensive R Archive Network.
-    Available from https://CRAN.R-project.org/package=rms
-
-[6] Nattino, G., Finazzi, S., & Bertolini, G. (2014). A new calibration test 
-    and a reappraisal of the calibration belt for the assessment of prediction models 
-    based on dichotomous outcomes. Statistics in medicine, 33(14), 2390-2407.
-
-[7] Bulgarelli, L. (2021). calibrattion-belt: Assessment of calibration in binomial prediction models [Computer software].
-    Available from https://github.com/fabiankueppers/calibration-framework
-
-[8] Nattino, G., Finazzi, S., Bertolini, G., Rossi, C., & Carrara, G. (2017).
-    givitiR: The giviti calibration test and belt (R package version 1.3) [Computer
-    software]. The Comprehensive R Archive Network.
-    Available from https://CRAN.R-project.org/package=givitiR
-
-[9] [Sturges, H. A. (1926). The choice of a class interval. 
-    Journal of the american statistical association, 21(153), 65-66.]
-
-[10] "Hosmer-Lemeshow test", https://en.wikipedia.org/wiki/Hosmer-Lemeshow_test
-
-[11] Pigeon, Joseph G., and Joseph F. Heyse. "A cautionary note about assessing 
-     the fit of logistic regression models." (1999): 847-853.
-"""
-
-from enum import Flag
-from math import log2, ceil, sqrt
-from typing import Union
-import warnings
-import numpy as np
-import pandas as pd
-import matplotlib.pyplot as plt
-from scipy.stats import chi2, norm
-from scipy import integrate
-from sklearn.metrics import roc_auc_score
-from statsmodels.nonparametric.smoothers_lowess import lowess
-from IPython.display import display
-
-from .calbelt import CalibrationBelt
-from .metrics import brier
-from ._result_types import *
-
-
-# SETS THE LIMIT FOR THE FREQUENCY IN CONTINGENCY TABLES
-CHI_SQUARE_VIOLATION_LIMIT = 1
-
-# SETS THE LIMIT FOR HIGHLIGHTING HIGH DEVIATION OF OBSERVED AND EXPECTED COUNTS IN CT
-HIGHLIGHT_DEVIATION_LIMIT = 0.1
-
-# SETS THE OUTPUT PRECISION OF FLOATS IN DATAFRAME
-pd.options.display.precision = 3
-
-
-class DEVEL(Flag):
-    INTERNAL = False
-    EXTERNAL = True
-
-
-# _BaseCalibrationEvaluator  <--(inherits from)-- CalibrationEvaluator
-class _BaseCalibrationEvaluator:
-
-    # CONSTRUCTOR
-    def __init__(self, y_true:np.ndarray, y_pred:np.ndarray, outsample:bool, n_groups:Union[int,str]=10) -> None:
-        """This is the main class for the PyCalEva framework bundeling statistical tests, 
-            metrics and plot for calibration measurement of binary classification models.
-
-        Parameters
-        ----------
-        y_true : array_like
-                Expected class labels given in test set. (Ground truth y)
-        y_pred : array_like
-                Observed probabilities predicted by a classification model.
-        outsample : bool
-                Set to 'False' for internal evaluation or set to 'True'
-                for external evaluation.
-        n_groups: int or str (optional, default=10)
-                Number of groups to use for grouping probabilities.
-                Set to 'auto' to use sturges function for estimation of optimal group size [9].
-
-        Raises
-        ------
-            ValueError: If the given data (y_true,y_pred) or the given number of groups is invalid
-
-        Examples
-        --------
-        >>> from pycaleva import CalibrationEvaluator
-        >>> ce = CalibrationEvaluator(y_test, pred_prob, outsample=True, n_groups='auto')
-
-        References
-        ----------
-        ..  [9] Sturges, H. A. (1926). The choice of a class interval. 
-            Journal of the american statistical association, 21(153), 65-66.
-
-        """
-        
-        # Check parameters
-        self.__check_parameters(np.array(y_true), np.array(y_pred), outsample)
-
-        self.__y = np.array(y_true) # True class labels
-        self.__p = np.array(y_pred) # Predicted class probabilities
-
-        self.__n = len(y_true)      # Sample size
-        self.__ngroups = None       # Group size
-
-        # Set if external testset or internal trainingsset is used 
-        if outsample:
-            self.__devel = DEVEL.EXTERNAL
-        else:
-            self.__devel = DEVEL.INTERNAL
-        
-        # Define calibration metrics
-        self.__auroc = roc_auc_score(self.__y, self.__p)    # Area under the receiver operating curve
-        self.__brier = brier(self.__y, self.__p,)           # Brier score
-        self.__ace = None                                   # Adative calibration error
-        self.__mce = None                                   # Maximum calibration error
-        self.__awlc = None                                  # Area within lowess curve
-
-        # Group data according to predicted probabilities --> will also set contengency table for groups
-        self.__data = None
-        self.__ct = None
-        self.group_data(n_groups) # --> This method will update all groupbased metrics as well
-
-    # PROPERTIES
-    #---------------------------------------------------------------------------------------------
-    @property
-    def contingency_table(self):
-        """Get the contingency table for grouped observed and expected class membership probabilities.
-        
-        Returns
-        -------
-            contingency_table :  DataFrame
-        """
-        return self.__ct
-
-    @property
-    def auroc(self):
-        """Get the area under the receiver operating characteristic
-
-        Returns
-        -------
-            auroc :  float
-        """
-        return self.__auroc
-
-    @property
-    def brier(self):
-        """Get the brier score for the current y_true and y_pred of class instance.
-
-        Returns
-        -------
-            brier_score :  float
-        """
-        return self.__brier
-
-    @property
-    def ace(self):
-        """Get the adaptive calibration error based on grouped data.
-
-        Returns
-        -------
-            adaptive calibration error : float
-        """
-        return self.__ace
-
-    @property
-    def mce(self):
-        """Get the maximum calibration error based on grouped data.
-
-        Returns
-        -------
-            maximum calibration error : float
-        """
-        return self.__mce
-
-    @property
-    def awlc(self):
-        """Get the area between the nonparametric curve estimated by lowess and
-            the theoritcally perfect calibration given by the calibration plot bisector.
-        
-        Returns
-        -------
-            Area within lowess curve : float
-        """
-        return self.__awlc
-
-    @property
-    def outsample(self):
-        """Get information if outsample is set. External validation if set to 'True'.
-        
-        Returns
-        -------
-            Outsample status : bool
-        """
-        return self.__devel
-
-
-    # PRIVATE METHODS
-    # --------------------------------------------------------------------------------------------
-    
-    # Check if parameters are valid
-    def __check_parameters(self, y, p, outsample) -> bool:
-        if (len(y) != len(p)):
-            raise ValueError("Observations y_true and Predictions y_pred differ in size!")
-        if not ( ((y==0) | (y==1)).all() ):
-            raise ValueError("Invalid class labels! y_train must be dichotomous containing only values 0 or 1")
-        if ( (p < 0.0 ).any() or (p > 1.0).any() ):
-            raise ValueError("Predicted probabilities y_pred must be in range [0.0 1.0]!")
-        if (abs( p.sum() - y.sum() ) < 1e-04 ) and outsample == True:
-            warnings.warn(Warning("Please set parameter outsample to 'false' if the evaluated model was fit on this dataset!"), "UserWarning")
-        if ( y.sum() <= 1 ) or ( y.sum() >= (len(y) - 1) ):
-            raise ValueError("The number of events/non events in observations can not be less than 1.")
-
-        return True
-
-
-    def __calc_ace(self):
-        return np.abs((self.__ct.mean_predicted - self.__ct.mean_observed)).sum() / self.__ngroups
-
-    def __calc_mce(self):
-        return np.abs((self.__ct.mean_predicted - self.__ct.mean_observed)).max()
-
-    def __init_contingency_table(self) -> pd.DataFrame:
-        """Initialize the contingency table using data
-
-        Returns:
-            contingency_table : DataFrame:
-        """
-        data = self.__data
-        total = data['class'].groupby(data.dcl).count()         # Total observations per group
-        mean_predicted = data['prob'].groupby(data.dcl).mean()  # Mean predicted probability per group
-        mean_observed = data['class'].groupby(data.dcl).mean()  # Mean observed probability per group
-        observed = data['class'].groupby(data.dcl).sum()        # Number of observed class 1 events
-        predicted = data['prob'].groupby(data.dcl).sum()        # Number of predicted class 1 events
-
-        c_table = pd.DataFrame({"total":total, "mean_predicted":mean_predicted, "mean_observed":mean_observed, \
-                                "observed_0":total-observed, "predicted_0":total-predicted, 
-                                "observed_1":observed, "predicted_1":predicted})
-        c_table.index.rename('Interval', inplace=True) #Rename index column
-        return c_table
-
-
-    def __highlight_high_diff(self,row:pd.Series):
-        """Highlight contingency table cells with high difference in observed and expected values
-        """
-        props = [f'color: black']*len(row)
-
-        if ( abs(row.predicted_1 - row.observed_1) > (HIGHLIGHT_DEVIATION_LIMIT * row.total) ):
-            props[-1] = f'color: red'
-
-        return props
-
-
-    def __warn_expected_low(self):
-        """Print warning message if expected frequencies are low.
-        """
-        if (self.__ct.predicted_1 < CHI_SQUARE_VIOLATION_LIMIT).any():
-           print(f'Warning! Some expected frequencies are smaller then {CHI_SQUARE_VIOLATION_LIMIT}. ' +
-                    'Possible violoation of chi²-distribution.')
-
-
-    def __show_contingency_table(self, phi=None):
-        """Display the contingency table using IPython.
-        """
-        ct_out = self.__ct.drop(['observed_0', 'predicted_0'], axis=1).copy()
-
-        # Add phi correction factor if values are given
-        if not phi is None:
-            ct_out.insert(3, "phi", phi)
-
-        ct_out.reset_index(inplace=True)
-        display(ct_out.style.apply(self.__highlight_high_diff, axis = 1))
-
-
-    def __update_groupbased_metrics(self):
-        """Update all metrics of class instance that are based on grouping
-        """
-        self.__ace = self.__calc_ace()                      # Update Adative Calibration Error
-        self.__mce = self.__calc_mce()                      # Update Maximum Calibration Error
-
-        self.__nonparametric_fit()                          # Calculate nonparametric fit and update Area Within Lowess Curve
-
-
-    def __nonparametric_fit(self, update_awlc=True):
-        # Nonparametric curve based on y and p using lowess
-        x_nonparametric = np.arange(0,1,0.005)
-        y_nonparametric = lowess(self.__y, self.__p, it=0, xvals=x_nonparametric)
-
-        if update_awlc:
-            diff = np.abs(x_nonparametric - y_nonparametric)
-            self.__awlc = integrate.trapezoid(diff, x_nonparametric) # Area within loss curve
-            
-        return (x_nonparametric, y_nonparametric)
-
-
-    def __metrics_to_string(self):
-        """Returns all metrics as formatted table.
-
-        Returns
-        -------
-            all_metrics: str
-        """
-        metrics = {"AUROC":self.__auroc, "Brier":self.__brier, "ACE":self.__ace, "MCE":self.__mce, "AWLC":self.__awlc }
-
-        lines = ['{:<10s}{:>8d}'.format("n",self.__n)]
-        for k, v in metrics.items():
-            lines.append('{:<10s}{:>8.3f}'.format(k,v))
-        
-        textstr = '\n'.join(lines)
-        return textstr
-
-
-    # PUBLIC METHODS
-    # --------------------------------------------------------------------------------------------
-    
-    # UTILITY: Return all metrics
-    def metrics(self):
-        """Get all available calibration metrics as combined result tuple.
-
-        Returns
-        -------
-        auroc   : float
-                    Area under the receiver operating characteristic.
-        brier   : float
-                    The scaled brier score.
-        ace     : int
-                    Adaptive calibration error.
-        mce     : float
-                    Maximum calibration error.
-        awlc    : float
-                    Area within the lowess curve
-        
-        Examples
-        --------
-        >>> from pycaleva import CalibrationEvaluator
-        >>> ce = CalibrationEvaluator(y_test, pred_prob, outsample=True, n_groups='auto')
-        >>> ce.metrics()
-        metrics_result(auroc=0.9739811912225705, brier=0.2677083794415594, ace=0.0361775962446639, mce=0.1837227304691177, awlc=0.041443052220213474)
-        """
-        return metrics_result(self.__auroc, self.__brier, self.__ace, self.__mce, self.__awlc)
-
-
-    # UTILITY: Group data
-    def group_data(self, n_groups:Union[int,str]) -> None:
-        r"""Group class labels and predicted probabilities into equal sized groupes of size n.
-
-        Parameters
-        ----------
-        n_groups: int or str
-                Number of groups to use for grouping probabilities.
-                Set to 'auto' to use sturges function for estimation of optimal group size [9].
-
-        Notes
-        -----
-        Sturges function for estimation of optimal group size:
-        
-        .. math::
-            k=\left\lceil\log _{2} n\right\rceil+1
-
-        Hosmer and Lemeshow recommend setting number of groups to 10 and with equally sized groups [1].
-            
-        Raises
-        ------
-            ValueError: If the given number of groups is invalid.
-        
-        References
-        ----------
-        ..  [1] Hosmer Jr, David W., Stanley Lemeshow, and Rodney X. Sturdivant.
-                Applied logistic regression. Vol. 398. John Wiley & Sons, 2013.
-        ..  [9] Sturges, H. A. (1926). The choice of a class interval. 
-                Journal of the american statistical association, 21(153), 65-66.
-
-        """
-
-        # Check group size parameter and set accordingly
-        if isinstance(n_groups, int) and 2 <= n_groups < self.__n:
-            self.__ngroups = n_groups   # Group size
-        elif isinstance(n_groups, str) and n_groups == 'auto':
-            self.__ngroups = ceil(log2(self.__n)) + 1
-        else:
-            raise ValueError(f"'{n_groups}' is an invalid value of parameter n_groups!")
-
-        df = pd.DataFrame(data={'class':self.__y, 'prob':self.__p})
-        
-        # Sort Values according to their probability
-        df = df.sort_values('prob')
-        df.reset_index(inplace=True)
-        
-        # Group data using deciles of risks
-        try:
-            df['dcl'] = pd.qcut(df['prob'], self.__ngroups)
-        except ValueError:
-            # Most likely low variance in probabilities results in non unique bin edges
-            try:
-                # FIX -> Put some probabilities into the same group
-                df['dcl'] = pd.qcut(df['prob'].rank(method='first'), self.__ngroups)
-
-                # Get propper interval labels after applied fix
-                new_categories = {}
-                df['rank'] = df['prob'].rank(method='first')
-                #for bin in set(df.dcl):
-                    #if bin.right > len(df.prob)-1:
-                        #new_categories[bin] = pd.Interval(left=round(df.prob[int(bin.left)],3), right=round(df.prob.iloc[-1],3))
-                    #else:
-                        #new_categories[bin] = pd.Interval(left=round(df.prob[int(bin.left)],3), right=round(df.prob[int(bin.right)],3))
-                    
-                #df['dcl'] = df['dcl'].cat.rename_categories(new_categories)
-            except ValueError:
-                raise Exception("Could not create groups. Maybe try with a lower number of groups or set n_groups to 'auto'.")
-        except BaseException as err:
-            print(f"Unexpected {err=}, {type(err)=}")
-            raise
-
-        self.__data = df
-        self.__ct = self.__init_contingency_table()
-
-        self.__update_groupbased_metrics()
-
-
-    # UTILITY: Merge Groups
-    def merge_groups(self, min_count:int=CHI_SQUARE_VIOLATION_LIMIT) -> None:
-        """Merge groups in contingency table to have count of expected and observed class events >= min_count.
-
-        Parameters
-        ----------
-        min_count : int (optional, default=1)
-
-        Notes
-        -----
-        Hosmer and Lemeshow mention the possibility to merge groups at low samplesize to have higher expected and observed class event counts [1].
-        This should guarantee that the requirements for chi-square goodness-of-fit tests are fullfilled.
-        Be aware that the power of tests will be lower after merge!
-
-        References
-        ----------
-        ..  [1] Hosmer Jr, David W., Stanley Lemeshow, and Rodney X. Sturdivant.
-                Applied logistic regression. Vol. 398. John Wiley & Sons, 2013.
-        """
-
-        i = 0
-        merged_rows = self.__ct.iloc[0:i].sum(axis=0, numeric_only=True)
-
-        # Merge groups as long expected and observed count is below min_count
-        while (i < self.__ngroups and (merged_rows["observed_1"] < min_count or merged_rows["predicted_1"] < min_count) ):
-            merged_rows = self.__ct.iloc[0:i].sum(axis=0, numeric_only=True)
-            i += 1
-
-        # Reset index of contingency table and add merged row
-        idx = pd.Interval(self.__ct.index[0].left, self.__ct.index[i-1].right)
-        self.__ct.loc[idx] = merged_rows
-
-        self.__ct = self.__ct[i:]
-        self.__ct.sort_index(axis=0, inplace=True)
-
-        # Update number of groups
-        self.__ngroups = len(self.__ct)
-
-        # Update bins in data
-        self.__data['dcl'] = pd.cut(self.__data['prob'], self.__ct.index)
-
-        # Update metrics
-        self.__update_groupbased_metrics()
-
-
-    # STATISTICAL TEST: Hosmer Lemeshow Test
-    def hosmerlemeshow(self, verbose = True) -> hltest_result:
-        r""" Perform the Hosmer-Lemeshow goodness of fit test on the data of class instance.
-            The Hosmer-Lemeshow test checks the null hypothesis that the number of 
-            given observed events match the number of expected events using given 
-            probabilistic class predictions and dividing those into deciles of risks.
-            
-            Parameters
-            ----------
-            verbose : bool (optional, default=True)
-                Whether or not to show test results and contingency table the teststatistic
-                relies on.
-            
-            Returns
-            -------
-            C       : float
-                        The Hosmer-Lemeshow test statistic.
-            p-value : float
-                        The p-value of the test.
-            dof     : int
-                        Degrees of freedom
-            
-            See Also
-            --------
-            CalibrationEvaluator.pigeonheyse
-            CalibrationEvaluator.z_test
-            scipy.stats.chisquare
-
-            Notes
-            -----
-            A low value for C and high p-value (>0.05) indicate a well calibrated model.
-            The power of this test is highly dependent on the sample size. Also the 
-            teststatistic lacks fit to chi-squared distribution in some situations [3]. 
-            In order to decide on model fit it is recommended to check it's discrematory
-            power as well using metrics like AUROC, precision, recall. Furthermore a
-            calibration plot (or reliability plot) can help to identify regions of the
-            model underestimate or overestimate the true class membership probabilities.
-            
-            Hosmer and Lemeshow estimated the degrees of freedom for the teststatistic
-            performing extensive simulations. According to their results the degrees of 
-            freedom are k-2 where k is the number of subroups the data is divided into. 
-            In the case of external evaluation the degrees of freedom is the same as k [1]. 
-            
-            Teststatistc:
-
-                .. math:: 
-                    E_{k 1}=\sum_{i=1}^{n_{k}} \hat{p}_{i 1}
-
-                .. math:: 
-                    O_{k 1}=\sum_{i=1}^{n_{k}} y_{i 1}
-
-                .. math:: 
-                    \hat{C}=\sum_{k=1}^{G} \frac{\left(O_{k 1}-E_{k 1}\right)^{2}}{E_{k 1}} + \frac{\left(O_{k 0}-E_{k 0}\right)^{2}}{E_{k 0}}
-
-            References
-            ----------
-            ..  [1] Hosmer Jr, David W., Stanley Lemeshow, and Rodney X. Sturdivant. 
-                Applied logistic regression. Vol. 398. John Wiley & Sons, 2013.
-            ..  [10] "Hosmer-Lemeshow test", https://en.wikipedia.org/wiki/Hosmer-Lemeshow_test
-            ..  [11] Pigeon, Joseph G., and Joseph F. Heyse. "A cautionary note about assessing 
-                the fit of logistic regression models." (1999): 847-853.
-
-            Examples
-            --------
-            >>> from pycaleva import CalibrationEvaluator
-            >>> ce = CalibrationEvaluator(y_test, pred_prob, outsample=True, n_groups='auto')
-            >>> ce.hosmerlemeshow()
-            hltest_result(statistic=4.982635477424991, pvalue=0.8358193332183672, dof=9)
-        """
-
-        # Calculate Hosmer Lemeshow Teststatistic based on contengency table
-        C_ = ( (self.__ct.observed_1 - self.__ct.predicted_1)**2 / \
-                (self.__ct.total*self.__ct.mean_predicted*(1-self.__ct.mean_predicted)) ).sum()
-        
-        # DoF Internal = Number Subgroups - Parameters of Logistic Regression [1]
-        # DoF External = Number Subgroups [1]
-        if self.__devel == DEVEL.INTERNAL:
-            dof = self.__ngroups-2
-        else:
-            dof = self.__ngroups
-        
-        # Calculate pvalue
-        pval = 1 - chi2.cdf(C_, dof)
-        
-        # Show the contingency table
-        if verbose:
-            self.__show_contingency_table()
-        
-            # Warn user if expected frequencies are < 5
-            self.__warn_expected_low()
-
-            if (pval < 0.001):
-                print(f'C({dof}): {C_:.2f} p-value: < 0.001')
-            else:
-                print(f'C({dof}): {C_:.2f} p-value: {pval:.3f}')
-        
-        return hltest_result(C_, pval, dof)
-
-
-    # STATISTICAL TEST: Pigeon Heyse Test
-    def pigeonheyse(self, verbose = True) -> phtest_result:
-        r"""Perform the Pigeon-Heyse goodness of fit test.
-        The Pigeon-Heyse test checks the null hypothesis that number of given observed 
-        events match the number of expected events over divided subgroups.
-        Unlike the Hosmer-Lemeshow test this test allows the use of different
-        grouping strategies and is more robust against variance within subgroups.
-        
-        Parameters
-        ----------
-        verbose : bool (optional, default=True)
-                Whether or not to show test results and contingency table the teststatistic
-                relies on.
-
-        Returns
-        -------
-        J : float
-            The Pigeon-Heyse test statistic J².
-        p : float
-            The p-value of the test.
-        dof : int
-                Degrees of freedom
-        
-        See Also
-        --------
-        CalibrationEvaluator.hosmerlemeshow
-        CalibrationEvaluator.z_test
-        scipy.stats.chisquare
-
-        Notes
-        -----
-        This is an implemenation of the test proposed by Pigeon and Heyse [2].
-        A low value for J² and high p-value (>0.05) indicate a well calibrated model.
-        Other then the Hosmer-Lemeshow test an adjustment factor is added to
-        the calculation of the teststatistic, making the use of different 
-        grouping strategies possible as well.
-        
-        The power of this test is highly dependent on the sample size.
-        In order to decide on model fit it is recommended to check it's discrematory
-        power as well using metrics like AUROC, precision, recall. Furthermore a
-        calibration plot (or reliability plot) can help to identify regions of the
-        model underestimate or overestimate the true class membership probabilities.
-        
-        Teststatistc:
-
-            .. math:: 
-                \phi_{k}=\frac{\sum_{i=1}^{n_{k}} \hat{p}_{i 1}\left(1-\hat{p}_{i 1}\right)}{n_{k} \bar{p}_{k 1}\left(1-\bar{p}_{k 1}\right)}
-
-            .. math:: 
-                {J}^{2}=\sum_{k=1}^{G} \frac{\left(O_{k 1}-E_{k 1}\right)^{2}}{\phi_{k} E_{k 1}} + \frac{\left(O_{k 0}-E_{k 0}\right)^{2}}{\phi_{k} E_{k 0}}
-
-        References
-        ----------
-        ..  [1] Hosmer Jr, David W., Stanley Lemeshow, and Rodney X. Sturdivant. 
-            Applied logistic regression. Vol. 398. John Wiley & Sons, 2013.
-        ..  [2] Pigeon, Joseph G., and Joseph F. Heyse. "An improved goodness of 
-            fit statistic for probability prediction models."
-            Biometrical Journal: Journal of Mathematical Methods in Biosciences 
-            41.1 (1999): 71-82.
-        ..  [11] Pigeon, Joseph G., and Joseph F. Heyse. "A cautionary note about assessing 
-            the fit of logistic regression models." (1999): 847-853.
-        
-        Examples
-        --------
-        >>> from pycaleva import CalibrationEvaluator
-        >>> ce = CalibrationEvaluator(y_test, pred_prob, outsample=True, n_groups='auto')
-        >>> ce.pigeonheyse()
-        phtest_result(statistic=5.269600396341568, pvalue=0.8102017228852412, dof=9)
-        """
-        
-        # Factor phi to adjust X² statistic
-        phi = ( self.__data['prob'].groupby(self.__data.dcl).apply(lambda x: (x *(1-x)).sum()) ) /  \
-            ( self.__ct.total * self.__ct.mean_predicted * (1 - self.__ct.mean_predicted) )
-
-        # Teststatistic
-        J_square = ( (self.__ct.observed_1 - self.__ct.predicted_1)**2 / \
-            (phi*self.__ct.total*self.__ct.mean_predicted*(1-self.__ct.mean_predicted)) ).sum()
-        
-
-        # DoF Internal = Number Subgroups - 1 [2]
-        # DoF External = Number Subgroups [1] 
-        if self.__devel == DEVEL.INTERNAL:
-            dof = self.__ngroups - 1
-        else:
-            dof = self.__ngroups
-
-
-        pval = 1 - chi2.cdf(J_square, dof)  # Calculate pvalue
-        
-        if verbose:
-            # Show the contingency table
-            self.__show_contingency_table(phi)
-
-            # Warn user if expected frequencies are < 5
-            self.__warn_expected_low()
-
-            if (pval < 0.001):
-                print(f'J²({dof}): {J_square:.2f} p-value: < 0.001')
-            else:
-                print(f'J²({dof}): {J_square:.2f} p-value: {pval:.3f}')
-
-        return phtest_result(J_square, pval, dof)
-
-
-    # STATISTICAL TEST: Spiegelhalter z-test
-    def z_test(self) -> ztest_result:
-        r"""Perform the Spieglhalter's z-test for calibration.
-        
-        Returns
-        -------
-        statistic : float
-            The Spiegelhalter z-test statistic.
-        p : float
-            The p-value of the test.
-        
-
-        See Also
-        --------
-        CalibrationEvaluator.hosmerlemeshow
-        CalibrationEvaluator.pigeonheyse
-
-
-        Notes
-        -----
-        This calibration test is performed in the manner of a z-test. 
-        The nullypothesis is that the estimated probabilities are equal to the true class probabilities.
-        The test statistic under the nullypothesis can be approximated by a normal distribution. 
-        A low value for Z and high p-value (>0.05) indicate a well calibrated model.
-        Other than Hosmer Lemeshow Test or Pigeon Heyse Test, this test is not based on grouping strategies.
-
-        Teststatistc:
-
-            .. math::
-                Z=\frac{\sum_{i=1}^{n}\left(y_{i}-\hat{p}_{i}\right)\left(1-2 \hat{p}_{i}\right)}{\sqrt{\sum_{i=1}^{n}\left(1-2 \hat{p}_{i}\right)^{2} \hat{p}_{i}\left(1-\hat{p}_{i}\right)}}
-            
-        
-        References
-        ----------
-        ..  [1] Spiegelhalter, D. J. (1986). Probabilistic prediction in patient management and clinical trials. 
-            Statistics in medicine, 5(5), 421-433.
-        ..  [2] Huang, Y., Li, W., Macheret, F., Gabriel, R. A., & Ohno-Machado, L. (2020). 
-            A tutorial on calibration measurements and calibration models for clinical prediction models. 
-            Journal of the American Medical Informatics Association, 27(4), 621-633.
-        
-
-        Examples
-        --------
-        >>> from pycaleva import CalibrationEvaluator
-        >>> ce = CalibrationEvaluator(y_test, pred_prob, outsample=True, n_groups='auto')
-        >>> ce.z_test()
-        ztest_result(statistic=-0.21590257919669287, pvalue=0.829063686607032)
-
-        """
-
-        num = ( (self.__y - self.__p) * ( 1 - 2 * self.__p )  ).sum()
-        denom = sqrt( ((1 - 2 * self.__p)**2 * self.__p * ( 1 - self.__p)).sum() )
-
-        z = num / denom
-        pval = 2 * norm.cdf(-abs(z))
-
-        return ztest_result(z, pval)
-
-
-    # STATISTICAL TEST / PLOT : Calibration Belt
-    def calbelt(self, plot:bool=False, subset = None, confLevels=[0.8, 0.95], alpha=0.95) -> calbelt_result:
-        """Calculate the calibration belt and draw plot if desired.
-        
-        Parameters
-        ----------
-        plot: boolean, optional
-            Decide if plot for calibration belt should be shown.
-            Much faster calculation if set to 'false'!
-        subset: array_like
-            An optional boolean vector specifying the subset of observations to be considered.
-            Defaults to None.
-        confLevels: list
-            A numeric vector containing the confidence levels of the calibration belt.
-            Defaults to [0.8,0.95].
-        alpha: float
-            The level of significance to use.
-
-        Returns
-        -------
-        T : float
-            The Calibration plot test statistic T.
-        p : float
-            The p-value of the test.
-        fig : matplotlib.figure
-            The calibration belt plot. Only returned if plot='True'
-        
-        See Also
-        --------
-        pycaleva.calbelt.CalibrationBelt
-        CalibrationEvaluator.calplot
-        
-
-        Notes
-        -----
-        This is an implemenation of the test proposed by Nattino et al. [6]. 
-        The implementation was built upon the python port of the R-Package givitiR [8] and the python implementation calibration-belt [7].
-        The calibration belt estimates the true underlying calibration curve given predicted probabilities and true class labels.
-        Instead of directly drawing the calibration curve a belt is drawn using confidence levels.
-        A low value for the teststatistic and a high p-value (>0.05) indicate a well calibrated model.
-        Other than Hosmer Lemeshow Test or Pigeon Heyse Test, this test is not based on grouping strategies.
-
-        References
-        ----------
-        ..  [6] Nattino, G., Finazzi, S., & Bertolini, G. (2014). A new calibration test 
-            and a reappraisal of the calibration belt for the assessment of prediction models 
-            based on dichotomous outcomes. Statistics in medicine, 33(14), 2390-2407.
-
-        ..  [7] Bulgarelli, L. (2021). calibrattion-belt: Assessment of calibration in binomial prediction models [Computer software].
-            Available from https://github.com/fabiankueppers/calibration-framework
-
-        ..  [8] Nattino, G., Finazzi, S., Bertolini, G., Rossi, C., & Carrara, G. (2017).
-            givitiR: The giviti calibration test and belt (R package version 1.3) [Computer
-            software]. The Comprehensive R Archive Network.
-            Available from https://CRAN.R-project.org/package=givitiR
-        
-
-        Examples
-        --------
-        >>> from pycaleva import CalibrationEvaluator
-        >>> ce = CalibrationEvaluator(y_test, pred_prob, outsample=True, n_groups='auto')
-        >>> ce.calbelt(plot=False)
-        calbelt_result(statistic=1.6111330037643796, pvalue=0.4468347221346196, fig=None)
-
-        """
-        
-        cb = CalibrationBelt(self.__y, self.__p, self.__devel, subset=subset, confLevels=confLevels, alpha=alpha)
-        
-        if plot:
-            return cb.plot()
-        else:
-            return cb.stats()
-
-
-    def calibration_plot(self):
-        """Generate the calibration plot for the given predicted probabilities and true class labels of current class instance.
-
-        Returns
-        -------
-            plot : matplotlib.figure
-
-        Notes
-        -----
-        This calibration plot is showing the predicted class probability against the actual probability according to the true class labels 
-        as a red triangle for each of the groups. An additional calibration curve is draw, estimated using the LOWESS algorithm. 
-        A model is well calibrated, if the red triangles and the calibration curve are both close to the plots bisector.
-        In the left corner of the plot all available metrics are listed as well. This implementation was made following the example of the R package
-        rms [5].
-
-        See Also
-        --------
-        CalibrationEvaluator.calbelt
-
-        References
-        ----------
-        ..  [5] Jr, F. E. H. (2021). rms: Regression modeling strategies (R package version
-            6.2-0) [Computer software]. The Comprehensive R Archive Network.
-            Available from https://CRAN.R-project.org/package=rms
-
-        Examples
-        --------
-        >>> from pycaleva import CalibrationEvaluator
-        >>> ce = CalibrationEvaluator(y_test, pred_prob, outsample=True, n_groups='auto')
-        >>> ce.calibration_plot()
-
-        """
-        fig, ax1 = plt.subplots(figsize=(10,6))
-        ax1.set_ylim(0.0, 1.05)
-
-        # Draw a calibration plot using matplotlib only
-        y_grouped = self.__ct["mean_observed"]
-        p_grouped = self.__ct["mean_predicted"]
-
-        # Get nonparametric curve based on y and p using lowess
-        x_nonparametric,y_nonparametric = self.__nonparametric_fit(update_awlc=False)
-
-        # Add calibration line for model
-        plt.scatter(p_grouped,y_grouped, marker="^", facecolors='none', edgecolors='r', label=f'Grouped observations g={self.__ngroups}')
-
-        # Add histogram on second axis
-        h, e = np.histogram(self.__p, bins=50)
-        h = h.astype('float')
-        h /= h.max()                # Get relative frequencies
-        ax2 = ax1.twinx()
-        ax2.set_ylim(-0.1,5)        # Scale down histogram
-        ax2.axis('off')             # Hide labels and ticks
-        ax2.stem(e[:-1],h, linefmt="grey", markerfmt=" ", basefmt=" ")
-
-        # Add line for nonparametric fit using lowess
-        ax1.plot(x_nonparametric, y_nonparametric, label="Nonparametric")
-
-        # Add line for perfect calibration
-        ax1.plot([0, 1], [0, 1], "k:", label="Perfectly calibrated")
-
-        ax1.set_xlabel('Predicted Probability')
-        ax1.set_ylabel('Actual Probability')
-        
-        props = dict(boxstyle='round', facecolor='white', alpha=0.4)
-        ax1.text(0.00, 0.75, self.__metrics_to_string(), fontsize=10, family='monospace', bbox=props)
-
-        ax1.legend(loc='best', bbox_to_anchor=(0.5, 0., 0.5, 0.5))
-
-        return fig
+"""
+A framework for calibration assessment of binary classification models 
+written in Python.
+
+References
+----------
+[1] Hosmer Jr, David W., Stanley Lemeshow, and Rodney X. Sturdivant.
+        Applied logistic regression. Vol. 398. John Wiley & Sons, 2013.
+
+[2] Pigeon, Joseph G., and Joseph F. Heyse.
+    An improved goodness of fit statistic for probability prediction models.
+    Biometrical Journal: Journal of Mathematical Methods in Biosciences 41.1 (1999): 71-82.
+
+[3] Spiegelhalter, D. J. (1986). Probabilistic prediction in patient management and clinical trials.
+    Statistics in medicine, 5(5), 421-433.
+
+[4] Huang, Y., Li, W., Macheret, F., Gabriel, R. A., & Ohno-Machado, L. (2020).
+    A tutorial on calibration measurements and calibration models for clinical prediction models.
+    Journal of the American Medical Informatics Association, 27(4), 621-633.
+
+[5] Jr, F. E. H. (2021). rms: Regression modeling strategies (R package version
+    6.2-0) [Computer software]. The Comprehensive R Archive Network.
+    Available from https://CRAN.R-project.org/package=rms
+
+[6] Nattino, G., Finazzi, S., & Bertolini, G. (2014). A new calibration test 
+    and a reappraisal of the calibration belt for the assessment of prediction models 
+    based on dichotomous outcomes. Statistics in medicine, 33(14), 2390-2407.
+
+[7] Bulgarelli, L. (2021). calibrattion-belt: Assessment of calibration in binomial prediction models [Computer software].
+    Available from https://github.com/fabiankueppers/calibration-framework
+
+[8] Nattino, G., Finazzi, S., Bertolini, G., Rossi, C., & Carrara, G. (2017).
+    givitiR: The giviti calibration test and belt (R package version 1.3) [Computer
+    software]. The Comprehensive R Archive Network.
+    Available from https://CRAN.R-project.org/package=givitiR
+
+[9] [Sturges, H. A. (1926). The choice of a class interval. 
+    Journal of the american statistical association, 21(153), 65-66.]
+
+[10] "Hosmer-Lemeshow test", https://en.wikipedia.org/wiki/Hosmer-Lemeshow_test
+
+[11] Pigeon, Joseph G., and Joseph F. Heyse. "A cautionary note about assessing 
+     the fit of logistic regression models." (1999): 847-853.
+"""
+
+from enum import Flag
+from math import log2, ceil, sqrt
+from typing import Union
+import warnings
+import numpy as np
+import pandas as pd
+import matplotlib.pyplot as plt
+from scipy.stats import chi2, norm
+from scipy import integrate
+from sklearn.metrics import roc_auc_score
+from statsmodels.nonparametric.smoothers_lowess import lowess
+from IPython.display import display
+
+from .calbelt import CalibrationBelt
+from .metrics import brier
+from ._result_types import *
+
+
+# SETS THE LIMIT FOR THE FREQUENCY IN CONTINGENCY TABLES
+CHI_SQUARE_VIOLATION_LIMIT = 1
+
+# SETS THE LIMIT FOR HIGHLIGHTING HIGH DEVIATION OF OBSERVED AND EXPECTED COUNTS IN CT
+HIGHLIGHT_DEVIATION_LIMIT = 0.1
+
+# SETS THE OUTPUT PRECISION OF FLOATS IN DATAFRAME
+pd.options.display.precision = 3
+
+
+class DEVEL(Flag):
+    INTERNAL = False
+    EXTERNAL = True
+
+
+# _BaseCalibrationEvaluator  <--(inherits from)-- CalibrationEvaluator
+class _BaseCalibrationEvaluator:
+
+    # CONSTRUCTOR
+    def __init__(self, y_true:np.ndarray, y_pred:np.ndarray, outsample:bool, n_groups:Union[int,str]=10) -> None:
+        """This is the main class for the PyCalEva framework bundeling statistical tests, 
+            metrics and plot for calibration measurement of binary classification models.
+
+        Parameters
+        ----------
+        y_true : array_like
+                Expected class labels given in test set. (Ground truth y)
+        y_pred : array_like
+                Observed probabilities predicted by a classification model.
+        outsample : bool
+                Set to 'False' for internal evaluation or set to 'True'
+                for external evaluation.
+        n_groups: int or str (optional, default=10)
+                Number of groups to use for grouping probabilities.
+                Set to 'auto' to use sturges function for estimation of optimal group size [9].
+
+        Raises
+        ------
+            ValueError: If the given data (y_true,y_pred) or the given number of groups is invalid
+
+        Examples
+        --------
+        >>> from pycaleva import CalibrationEvaluator
+        >>> ce = CalibrationEvaluator(y_test, pred_prob, outsample=True, n_groups='auto')
+
+        References
+        ----------
+        ..  [9] Sturges, H. A. (1926). The choice of a class interval. 
+            Journal of the american statistical association, 21(153), 65-66.
+
+        """
+        
+        # Check parameters
+        self.__check_parameters(np.array(y_true), np.array(y_pred), outsample)
+
+        self.__y = np.array(y_true) # True class labels
+        self.__p = np.array(y_pred) # Predicted class probabilities
+
+        self.__n = len(y_true)      # Sample size
+        self.__ngroups = None       # Group size
+
+        # Set if external testset or internal trainingsset is used 
+        if outsample:
+            self.__devel = DEVEL.EXTERNAL
+        else:
+            self.__devel = DEVEL.INTERNAL
+        
+        # Define calibration metrics
+        self.__auroc = roc_auc_score(self.__y, self.__p)    # Area under the receiver operating curve
+        self.__brier = brier(self.__y, self.__p,)           # Brier score
+        self.__ace = None                                   # Adative calibration error
+        self.__mce = None                                   # Maximum calibration error
+        self.__awlc = None                                  # Area within lowess curve
+
+        # Group data according to predicted probabilities --> will also set contengency table for groups
+        self.__data = None
+        self.__ct = None
+        self.group_data(n_groups) # --> This method will update all groupbased metrics as well
+
+    # PROPERTIES
+    #---------------------------------------------------------------------------------------------
+    @property
+    def contingency_table(self):
+        """Get the contingency table for grouped observed and expected class membership probabilities.
+        
+        Returns
+        -------
+            contingency_table :  DataFrame
+        """
+        return self.__ct
+
+    @property
+    def auroc(self):
+        """Get the area under the receiver operating characteristic
+
+        Returns
+        -------
+            auroc :  float
+        """
+        return self.__auroc
+
+    @property
+    def brier(self):
+        """Get the brier score for the current y_true and y_pred of class instance.
+
+        Returns
+        -------
+            brier_score :  float
+        """
+        return self.__brier
+
+    @property
+    def ace(self):
+        """Get the adaptive calibration error based on grouped data.
+
+        Returns
+        -------
+            adaptive calibration error : float
+        """
+        return self.__ace
+
+    @property
+    def mce(self):
+        """Get the maximum calibration error based on grouped data.
+
+        Returns
+        -------
+            maximum calibration error : float
+        """
+        return self.__mce
+
+    @property
+    def awlc(self):
+        """Get the area between the nonparametric curve estimated by lowess and
+            the theoritcally perfect calibration given by the calibration plot bisector.
+        
+        Returns
+        -------
+            Area within lowess curve : float
+        """
+        return self.__awlc
+
+    @property
+    def outsample(self):
+        """Get information if outsample is set. External validation if set to 'True'.
+        
+        Returns
+        -------
+            Outsample status : bool
+        """
+        return self.__devel
+
+
+    # PRIVATE METHODS
+    # --------------------------------------------------------------------------------------------
+    
+    # Check if parameters are valid
+    def __check_parameters(self, y, p, outsample) -> bool:
+        if (len(y) != len(p)):
+            raise ValueError("Observations y_true and Predictions y_pred differ in size!")
+        if not ( ((y==0) | (y==1)).all() ):
+            raise ValueError("Invalid class labels! y_train must be dichotomous containing only values 0 or 1")
+        if ( (p < 0.0 ).any() or (p > 1.0).any() ):
+            raise ValueError("Predicted probabilities y_pred must be in range [0.0 1.0]!")
+        if (abs( p.sum() - y.sum() ) < 1e-04 ) and outsample == True:
+            warnings.warn(Warning("Please set parameter outsample to 'false' if the evaluated model was fit on this dataset!"), "UserWarning")
+        if ( y.sum() <= 1 ) or ( y.sum() >= (len(y) - 1) ):
+            raise ValueError("The number of events/non events in observations can not be less than 1.")
+
+        return True
+
+
+    def __calc_ace(self):
+        return np.abs((self.__ct.mean_predicted - self.__ct.mean_observed)).sum() / self.__ngroups
+
+    def __calc_mce(self):
+        return np.abs((self.__ct.mean_predicted - self.__ct.mean_observed)).max()
+
+    def __init_contingency_table(self) -> pd.DataFrame:
+        """Initialize the contingency table using data
+
+        Returns:
+            contingency_table : DataFrame:
+        """
+        data = self.__data
+        total = data['class'].groupby(data.dcl, observed=False).count()         # Total observations per group
+        mean_predicted = data['prob'].groupby(data.dcl, observed=False).mean()  # Mean predicted probability per group
+        mean_observed = data['class'].groupby(data.dcl, observed=False).mean()  # Mean observed probability per group
+        observed = data['class'].groupby(data.dcl, observed=False).sum()        # Number of observed class 1 events
+        predicted = data['prob'].groupby(data.dcl, observed=False).sum()        # Number of predicted class 1 events
+
+        c_table = pd.DataFrame({"total":total, "mean_predicted":mean_predicted, "mean_observed":mean_observed, \
+                                "observed_0":total-observed, "predicted_0":total-predicted, 
+                                "observed_1":observed, "predicted_1":predicted})
+        c_table.index.rename('Interval', inplace=True) #Rename index column
+        return c_table
+
+
+    def __highlight_high_diff(self,row:pd.Series):
+        """Highlight contingency table cells with high difference in observed and expected values
+        """
+        props = [f'color: black']*len(row)
+
+        if ( abs(row.predicted_1 - row.observed_1) > (HIGHLIGHT_DEVIATION_LIMIT * row.total) ):
+            props[-1] = f'color: red'
+
+        return props
+
+
+    def __warn_expected_low(self):
+        """Print warning message if expected frequencies are low.
+        """
+        if (self.__ct.predicted_1 < CHI_SQUARE_VIOLATION_LIMIT).any():
+           print(f'Warning! Some expected frequencies are smaller then {CHI_SQUARE_VIOLATION_LIMIT}. ' +
+                    'Possible violoation of chi²-distribution.')
+
+
+    def __show_contingency_table(self, phi=None):
+        """Display the contingency table using IPython.
+        """
+        ct_out = self.__ct.drop(['observed_0', 'predicted_0'], axis=1).copy()
+
+        # Add phi correction factor if values are given
+        if not phi is None:
+            ct_out.insert(3, "phi", phi)
+
+        ct_out.reset_index(inplace=True)
+        display(ct_out.style.apply(self.__highlight_high_diff, axis = 1))
+
+
+    def __update_groupbased_metrics(self):
+        """Update all metrics of class instance that are based on grouping
+        """
+        self.__ace = self.__calc_ace()                      # Update Adative Calibration Error
+        self.__mce = self.__calc_mce()                      # Update Maximum Calibration Error
+
+        self.__nonparametric_fit()                          # Calculate nonparametric fit and update Area Within Lowess Curve
+
+
+    def __nonparametric_fit(self, update_awlc=True):
+        # Nonparametric curve based on y and p using lowess
+        x_nonparametric = np.arange(0,1,0.005)
+        y_nonparametric = lowess(self.__y, self.__p, it=0, xvals=x_nonparametric)
+
+        if update_awlc:
+            diff = np.abs(x_nonparametric - y_nonparametric)
+            self.__awlc = integrate.trapezoid(diff, x_nonparametric) # Area within loss curve
+            
+        return (x_nonparametric, y_nonparametric)
+
+
+    def __metrics_to_string(self):
+        """Returns all metrics as formatted table.
+
+        Returns
+        -------
+            all_metrics: str
+        """
+        metrics = {"AUROC":self.__auroc, "Brier":self.__brier, "ACE":self.__ace, "MCE":self.__mce, "AWLC":self.__awlc }
+
+        lines = ['{:<10s}{:>8d}'.format("n",self.__n)]
+        for k, v in metrics.items():
+            lines.append('{:<10s}{:>8.3f}'.format(k,v))
+        
+        textstr = '\n'.join(lines)
+        return textstr
+
+
+    # PUBLIC METHODS
+    # --------------------------------------------------------------------------------------------
+    
+    # UTILITY: Return all metrics
+    def metrics(self):
+        """Get all available calibration metrics as combined result tuple.
+
+        Returns
+        -------
+        auroc   : float
+                    Area under the receiver operating characteristic.
+        brier   : float
+                    The scaled brier score.
+        ace     : int
+                    Adaptive calibration error.
+        mce     : float
+                    Maximum calibration error.
+        awlc    : float
+                    Area within the lowess curve
+        
+        Examples
+        --------
+        >>> from pycaleva import CalibrationEvaluator
+        >>> ce = CalibrationEvaluator(y_test, pred_prob, outsample=True, n_groups='auto')
+        >>> ce.metrics()
+        metrics_result(auroc=0.9739811912225705, brier=0.2677083794415594, ace=0.0361775962446639, mce=0.1837227304691177, awlc=0.041443052220213474)
+        """
+        return metrics_result(self.__auroc, self.__brier, self.__ace, self.__mce, self.__awlc)
+
+
+    # UTILITY: Group data
+    def group_data(self, n_groups:Union[int,str]) -> None:
+        r"""Group class labels and predicted probabilities into equal sized groupes of size n.
+
+        Parameters
+        ----------
+        n_groups: int or str
+                Number of groups to use for grouping probabilities.
+                Set to 'auto' to use sturges function for estimation of optimal group size [9].
+
+        Notes
+        -----
+        Sturges function for estimation of optimal group size:
+        
+        .. math::
+            k=\left\lceil\log _{2} n\right\rceil+1
+
+        Hosmer and Lemeshow recommend setting number of groups to 10 and with equally sized groups [1].
+            
+        Raises
+        ------
+            ValueError: If the given number of groups is invalid.
+        
+        References
+        ----------
+        ..  [1] Hosmer Jr, David W., Stanley Lemeshow, and Rodney X. Sturdivant.
+                Applied logistic regression. Vol. 398. John Wiley & Sons, 2013.
+        ..  [9] Sturges, H. A. (1926). The choice of a class interval. 
+                Journal of the american statistical association, 21(153), 65-66.
+
+        """
+
+        # Check group size parameter and set accordingly
+        if isinstance(n_groups, int) and 2 <= n_groups < self.__n:
+            self.__ngroups = n_groups   # Group size
+        elif isinstance(n_groups, str) and n_groups == 'auto':
+            self.__ngroups = ceil(log2(self.__n)) + 1
+        else:
+            raise ValueError(f"'{n_groups}' is an invalid value of parameter n_groups!")
+
+        df = pd.DataFrame(data={'class':self.__y, 'prob':self.__p})
+        
+        # Sort Values according to their probability
+        df = df.sort_values('prob')
+        df.reset_index(inplace=True)
+        
+        # Group data using deciles of risks
+        try:
+            df['dcl'] = pd.qcut(df['prob'], self.__ngroups)
+        except ValueError:
+            # Most likely low variance in probabilities results in non unique bin edges
+            try:
+                # FIX -> Put some probabilities into the same group
+                df['dcl'] = pd.qcut(df['prob'].rank(method='first'), self.__ngroups)
+
+                # Get propper interval labels after applied fix
+                new_categories = {}
+                df['rank'] = df['prob'].rank(method='first')
+                #for bin in set(df.dcl):
+                    #if bin.right > len(df.prob)-1:
+                        #new_categories[bin] = pd.Interval(left=round(df.prob[int(bin.left)],3), right=round(df.prob.iloc[-1],3))
+                    #else:
+                        #new_categories[bin] = pd.Interval(left=round(df.prob[int(bin.left)],3), right=round(df.prob[int(bin.right)],3))
+                    
+                #df['dcl'] = df['dcl'].cat.rename_categories(new_categories)
+            except ValueError:
+                raise Exception("Could not create groups. Maybe try with a lower number of groups or set n_groups to 'auto'.")
+        except BaseException as err:
+            print(f"Unexpected {err=}, {type(err)=}")
+            raise
+
+        self.__data = df
+        self.__ct = self.__init_contingency_table()
+
+        self.__update_groupbased_metrics()
+
+
+    # UTILITY: Merge Groups
+    def merge_groups(self, min_count:int=CHI_SQUARE_VIOLATION_LIMIT) -> None:
+        """Merge groups in contingency table to have count of expected and observed class events >= min_count.
+
+        Parameters
+        ----------
+        min_count : int (optional, default=1)
+
+        Notes
+        -----
+        Hosmer and Lemeshow mention the possibility to merge groups at low samplesize to have higher expected and observed class event counts [1].
+        This should guarantee that the requirements for chi-square goodness-of-fit tests are fullfilled.
+        Be aware that the power of tests will be lower after merge!
+
+        References
+        ----------
+        ..  [1] Hosmer Jr, David W., Stanley Lemeshow, and Rodney X. Sturdivant.
+                Applied logistic regression. Vol. 398. John Wiley & Sons, 2013.
+        """
+
+        i = 0
+        merged_rows = self.__ct.iloc[0:i].sum(axis=0, numeric_only=True)
+
+        # Merge groups as long expected and observed count is below min_count
+        while (i < self.__ngroups and (merged_rows["observed_1"] < min_count or merged_rows["predicted_1"] < min_count) ):
+            merged_rows = self.__ct.iloc[0:i].sum(axis=0, numeric_only=True)
+            i += 1
+
+        # Reset index of contingency table and add merged row
+        idx = pd.Interval(self.__ct.index[0].left, self.__ct.index[i-1].right)
+        self.__ct.loc[idx] = merged_rows
+
+        self.__ct = self.__ct[i:]
+        self.__ct.sort_index(axis=0, inplace=True)
+
+        # Update number of groups
+        self.__ngroups = len(self.__ct)
+
+        # Update bins in data
+        self.__data['dcl'] = pd.cut(self.__data['prob'], self.__ct.index)
+
+        # Update metrics
+        self.__update_groupbased_metrics()
+
+
+    # STATISTICAL TEST: Hosmer Lemeshow Test
+    def hosmerlemeshow(self, verbose = True) -> hltest_result:
+        r""" Perform the Hosmer-Lemeshow goodness of fit test on the data of class instance.
+            The Hosmer-Lemeshow test checks the null hypothesis that the number of 
+            given observed events match the number of expected events using given 
+            probabilistic class predictions and dividing those into deciles of risks.
+            
+            Parameters
+            ----------
+            verbose : bool (optional, default=True)
+                Whether or not to show test results and contingency table the teststatistic
+                relies on.
+            
+            Returns
+            -------
+            C       : float
+                        The Hosmer-Lemeshow test statistic.
+            p-value : float
+                        The p-value of the test.
+            dof     : int
+                        Degrees of freedom
+            
+            See Also
+            --------
+            CalibrationEvaluator.pigeonheyse
+            CalibrationEvaluator.z_test
+            scipy.stats.chisquare
+
+            Notes
+            -----
+            A low value for C and high p-value (>0.05) indicate a well calibrated model.
+            The power of this test is highly dependent on the sample size. Also the 
+            teststatistic lacks fit to chi-squared distribution in some situations [3]. 
+            In order to decide on model fit it is recommended to check it's discrematory
+            power as well using metrics like AUROC, precision, recall. Furthermore a
+            calibration plot (or reliability plot) can help to identify regions of the
+            model underestimate or overestimate the true class membership probabilities.
+            
+            Hosmer and Lemeshow estimated the degrees of freedom for the teststatistic
+            performing extensive simulations. According to their results the degrees of 
+            freedom are k-2 where k is the number of subroups the data is divided into. 
+            In the case of external evaluation the degrees of freedom is the same as k [1]. 
+            
+            Teststatistc:
+
+                .. math:: 
+                    E_{k 1}=\sum_{i=1}^{n_{k}} \hat{p}_{i 1}
+
+                .. math:: 
+                    O_{k 1}=\sum_{i=1}^{n_{k}} y_{i 1}
+
+                .. math:: 
+                    \hat{C}=\sum_{k=1}^{G} \frac{\left(O_{k 1}-E_{k 1}\right)^{2}}{E_{k 1}} + \frac{\left(O_{k 0}-E_{k 0}\right)^{2}}{E_{k 0}}
+
+            References
+            ----------
+            ..  [1] Hosmer Jr, David W., Stanley Lemeshow, and Rodney X. Sturdivant. 
+                Applied logistic regression. Vol. 398. John Wiley & Sons, 2013.
+            ..  [10] "Hosmer-Lemeshow test", https://en.wikipedia.org/wiki/Hosmer-Lemeshow_test
+            ..  [11] Pigeon, Joseph G., and Joseph F. Heyse. "A cautionary note about assessing 
+                the fit of logistic regression models." (1999): 847-853.
+
+            Examples
+            --------
+            >>> from pycaleva import CalibrationEvaluator
+            >>> ce = CalibrationEvaluator(y_test, pred_prob, outsample=True, n_groups='auto')
+            >>> ce.hosmerlemeshow()
+            hltest_result(statistic=4.982635477424991, pvalue=0.8358193332183672, dof=9)
+        """
+
+        # Calculate Hosmer Lemeshow Teststatistic based on contengency table
+        C_ = ( (self.__ct.observed_1 - self.__ct.predicted_1)**2 / \
+                (self.__ct.total*self.__ct.mean_predicted*(1-self.__ct.mean_predicted)) ).sum()
+        
+        # DoF Internal = Number Subgroups - Parameters of Logistic Regression [1]
+        # DoF External = Number Subgroups [1]
+        if self.__devel == DEVEL.INTERNAL:
+            dof = self.__ngroups-2
+        else:
+            dof = self.__ngroups
+        
+        # Calculate pvalue
+        pval = 1 - chi2.cdf(C_, dof)
+        
+        # Show the contingency table
+        if verbose:
+            self.__show_contingency_table()
+        
+            # Warn user if expected frequencies are < 5
+            self.__warn_expected_low()
+
+            if (pval < 0.001):
+                print(f'C({dof}): {C_:.2f} p-value: < 0.001')
+            else:
+                print(f'C({dof}): {C_:.2f} p-value: {pval:.3f}')
+        
+        return hltest_result(C_, pval, dof)
+
+
+    # STATISTICAL TEST: Pigeon Heyse Test
+    def pigeonheyse(self, verbose = True) -> phtest_result:
+        r"""Perform the Pigeon-Heyse goodness of fit test.
+        The Pigeon-Heyse test checks the null hypothesis that number of given observed 
+        events match the number of expected events over divided subgroups.
+        Unlike the Hosmer-Lemeshow test this test allows the use of different
+        grouping strategies and is more robust against variance within subgroups.
+        
+        Parameters
+        ----------
+        verbose : bool (optional, default=True)
+                Whether or not to show test results and contingency table the teststatistic
+                relies on.
+
+        Returns
+        -------
+        J : float
+            The Pigeon-Heyse test statistic J².
+        p : float
+            The p-value of the test.
+        dof : int
+                Degrees of freedom
+        
+        See Also
+        --------
+        CalibrationEvaluator.hosmerlemeshow
+        CalibrationEvaluator.z_test
+        scipy.stats.chisquare
+
+        Notes
+        -----
+        This is an implemenation of the test proposed by Pigeon and Heyse [2].
+        A low value for J² and high p-value (>0.05) indicate a well calibrated model.
+        Other then the Hosmer-Lemeshow test an adjustment factor is added to
+        the calculation of the teststatistic, making the use of different 
+        grouping strategies possible as well.
+        
+        The power of this test is highly dependent on the sample size.
+        In order to decide on model fit it is recommended to check it's discrematory
+        power as well using metrics like AUROC, precision, recall. Furthermore a
+        calibration plot (or reliability plot) can help to identify regions of the
+        model underestimate or overestimate the true class membership probabilities.
+        
+        Teststatistc:
+
+            .. math:: 
+                \phi_{k}=\frac{\sum_{i=1}^{n_{k}} \hat{p}_{i 1}\left(1-\hat{p}_{i 1}\right)}{n_{k} \bar{p}_{k 1}\left(1-\bar{p}_{k 1}\right)}
+
+            .. math:: 
+                {J}^{2}=\sum_{k=1}^{G} \frac{\left(O_{k 1}-E_{k 1}\right)^{2}}{\phi_{k} E_{k 1}} + \frac{\left(O_{k 0}-E_{k 0}\right)^{2}}{\phi_{k} E_{k 0}}
+
+        References
+        ----------
+        ..  [1] Hosmer Jr, David W., Stanley Lemeshow, and Rodney X. Sturdivant. 
+            Applied logistic regression. Vol. 398. John Wiley & Sons, 2013.
+        ..  [2] Pigeon, Joseph G., and Joseph F. Heyse. "An improved goodness of 
+            fit statistic for probability prediction models."
+            Biometrical Journal: Journal of Mathematical Methods in Biosciences 
+            41.1 (1999): 71-82.
+        ..  [11] Pigeon, Joseph G., and Joseph F. Heyse. "A cautionary note about assessing 
+            the fit of logistic regression models." (1999): 847-853.
+        
+        Examples
+        --------
+        >>> from pycaleva import CalibrationEvaluator
+        >>> ce = CalibrationEvaluator(y_test, pred_prob, outsample=True, n_groups='auto')
+        >>> ce.pigeonheyse()
+        phtest_result(statistic=5.269600396341568, pvalue=0.8102017228852412, dof=9)
+        """
+        
+        # Factor phi to adjust X² statistic
+        phi = ( self.__data['prob'].groupby(self.__data.dcl, observed=False).apply(lambda x: (x *(1-x)).sum()) ) /  \
+            ( self.__ct.total * self.__ct.mean_predicted * (1 - self.__ct.mean_predicted) )
+
+        # Teststatistic
+        J_square = ( (self.__ct.observed_1 - self.__ct.predicted_1)**2 / \
+            (phi*self.__ct.total*self.__ct.mean_predicted*(1-self.__ct.mean_predicted)) ).sum()
+        
+
+        # DoF Internal = Number Subgroups - 1 [2]
+        # DoF External = Number Subgroups [1] 
+        if self.__devel == DEVEL.INTERNAL:
+            dof = self.__ngroups - 1
+        else:
+            dof = self.__ngroups
+
+
+        pval = 1 - chi2.cdf(J_square, dof)  # Calculate pvalue
+        
+        if verbose:
+            # Show the contingency table
+            self.__show_contingency_table(phi)
+
+            # Warn user if expected frequencies are < 5
+            self.__warn_expected_low()
+
+            if (pval < 0.001):
+                print(f'J²({dof}): {J_square:.2f} p-value: < 0.001')
+            else:
+                print(f'J²({dof}): {J_square:.2f} p-value: {pval:.3f}')
+
+        return phtest_result(J_square, pval, dof)
+
+
+    # STATISTICAL TEST: Spiegelhalter z-test
+    def z_test(self) -> ztest_result:
+        r"""Perform the Spieglhalter's z-test for calibration.
+        
+        Returns
+        -------
+        statistic : float
+            The Spiegelhalter z-test statistic.
+        p : float
+            The p-value of the test.
+        
+
+        See Also
+        --------
+        CalibrationEvaluator.hosmerlemeshow
+        CalibrationEvaluator.pigeonheyse
+
+
+        Notes
+        -----
+        This calibration test is performed in the manner of a z-test. 
+        The nullypothesis is that the estimated probabilities are equal to the true class probabilities.
+        The test statistic under the nullypothesis can be approximated by a normal distribution. 
+        A low value for Z and high p-value (>0.05) indicate a well calibrated model.
+        Other than Hosmer Lemeshow Test or Pigeon Heyse Test, this test is not based on grouping strategies.
+
+        Teststatistc:
+
+            .. math::
+                Z=\frac{\sum_{i=1}^{n}\left(y_{i}-\hat{p}_{i}\right)\left(1-2 \hat{p}_{i}\right)}{\sqrt{\sum_{i=1}^{n}\left(1-2 \hat{p}_{i}\right)^{2} \hat{p}_{i}\left(1-\hat{p}_{i}\right)}}
+            
+        
+        References
+        ----------
+        ..  [1] Spiegelhalter, D. J. (1986). Probabilistic prediction in patient management and clinical trials. 
+            Statistics in medicine, 5(5), 421-433.
+        ..  [2] Huang, Y., Li, W., Macheret, F., Gabriel, R. A., & Ohno-Machado, L. (2020). 
+            A tutorial on calibration measurements and calibration models for clinical prediction models. 
+            Journal of the American Medical Informatics Association, 27(4), 621-633.
+        
+
+        Examples
+        --------
+        >>> from pycaleva import CalibrationEvaluator
+        >>> ce = CalibrationEvaluator(y_test, pred_prob, outsample=True, n_groups='auto')
+        >>> ce.z_test()
+        ztest_result(statistic=-0.21590257919669287, pvalue=0.829063686607032)
+
+        """
+
+        num = ( (self.__y - self.__p) * ( 1 - 2 * self.__p )  ).sum()
+        denom = sqrt( ((1 - 2 * self.__p)**2 * self.__p * ( 1 - self.__p)).sum() )
+
+        z = num / denom
+        pval = 2 * norm.cdf(-abs(z))
+
+        return ztest_result(z, pval)
+
+
+    # STATISTICAL TEST / PLOT : Calibration Belt
+    def calbelt(self, plot:bool=False, subset = None, confLevels=[0.8, 0.95], alpha=0.95) -> calbelt_result:
+        """Calculate the calibration belt and draw plot if desired.
+        
+        Parameters
+        ----------
+        plot: boolean, optional
+            Decide if plot for calibration belt should be shown.
+            Much faster calculation if set to 'false'!
+        subset: array_like
+            An optional boolean vector specifying the subset of observations to be considered.
+            Defaults to None.
+        confLevels: list
+            A numeric vector containing the confidence levels of the calibration belt.
+            Defaults to [0.8,0.95].
+        alpha: float
+            The level of significance to use.
+
+        Returns
+        -------
+        T : float
+            The Calibration plot test statistic T.
+        p : float
+            The p-value of the test.
+        fig : matplotlib.figure
+            The calibration belt plot. Only returned if plot='True'
+        
+        See Also
+        --------
+        pycaleva.calbelt.CalibrationBelt
+        CalibrationEvaluator.calplot
+        
+
+        Notes
+        -----
+        This is an implemenation of the test proposed by Nattino et al. [6]. 
+        The implementation was built upon the python port of the R-Package givitiR [8] and the python implementation calibration-belt [7].
+        The calibration belt estimates the true underlying calibration curve given predicted probabilities and true class labels.
+        Instead of directly drawing the calibration curve a belt is drawn using confidence levels.
+        A low value for the teststatistic and a high p-value (>0.05) indicate a well calibrated model.
+        Other than Hosmer Lemeshow Test or Pigeon Heyse Test, this test is not based on grouping strategies.
+
+        References
+        ----------
+        ..  [6] Nattino, G., Finazzi, S., & Bertolini, G. (2014). A new calibration test 
+            and a reappraisal of the calibration belt for the assessment of prediction models 
+            based on dichotomous outcomes. Statistics in medicine, 33(14), 2390-2407.
+
+        ..  [7] Bulgarelli, L. (2021). calibrattion-belt: Assessment of calibration in binomial prediction models [Computer software].
+            Available from https://github.com/fabiankueppers/calibration-framework
+
+        ..  [8] Nattino, G., Finazzi, S., Bertolini, G., Rossi, C., & Carrara, G. (2017).
+            givitiR: The giviti calibration test and belt (R package version 1.3) [Computer
+            software]. The Comprehensive R Archive Network.
+            Available from https://CRAN.R-project.org/package=givitiR
+        
+
+        Examples
+        --------
+        >>> from pycaleva import CalibrationEvaluator
+        >>> ce = CalibrationEvaluator(y_test, pred_prob, outsample=True, n_groups='auto')
+        >>> ce.calbelt(plot=False)
+        calbelt_result(statistic=1.6111330037643796, pvalue=0.4468347221346196, fig=None)
+
+        """
+        
+        cb = CalibrationBelt(self.__y, self.__p, self.__devel, subset=subset, confLevels=confLevels, alpha=alpha)
+        
+        if plot:
+            return cb.plot()
+        else:
+            return cb.stats()
+
+
+    def calibration_plot(self):
+        """Generate the calibration plot for the given predicted probabilities and true class labels of current class instance.
+
+        Returns
+        -------
+            plot : matplotlib.figure
+
+        Notes
+        -----
+        This calibration plot is showing the predicted class probability against the actual probability according to the true class labels 
+        as a red triangle for each of the groups. An additional calibration curve is draw, estimated using the LOWESS algorithm. 
+        A model is well calibrated, if the red triangles and the calibration curve are both close to the plots bisector.
+        In the left corner of the plot all available metrics are listed as well. This implementation was made following the example of the R package
+        rms [5].
+
+        See Also
+        --------
+        CalibrationEvaluator.calbelt
+
+        References
+        ----------
+        ..  [5] Jr, F. E. H. (2021). rms: Regression modeling strategies (R package version
+            6.2-0) [Computer software]. The Comprehensive R Archive Network.
+            Available from https://CRAN.R-project.org/package=rms
+
+        Examples
+        --------
+        >>> from pycaleva import CalibrationEvaluator
+        >>> ce = CalibrationEvaluator(y_test, pred_prob, outsample=True, n_groups='auto')
+        >>> ce.calibration_plot()
+
+        """
+        fig, ax1 = plt.subplots(figsize=(10,6))
+        ax1.set_ylim(0.0, 1.05)
+
+        # Draw a calibration plot using matplotlib only
+        y_grouped = self.__ct["mean_observed"]
+        p_grouped = self.__ct["mean_predicted"]
+
+        # Get nonparametric curve based on y and p using lowess
+        x_nonparametric,y_nonparametric = self.__nonparametric_fit(update_awlc=False)
+
+        # Add calibration line for model
+        plt.scatter(p_grouped,y_grouped, marker="^", facecolors='none', edgecolors='r', label=f'Grouped observations g={self.__ngroups}')
+
+        # Add histogram on second axis
+        h, e = np.histogram(self.__p, bins=50)
+        h = h.astype('float')
+        h /= h.max()                # Get relative frequencies
+        ax2 = ax1.twinx()
+        ax2.set_ylim(-0.1,5)        # Scale down histogram
+        ax2.axis('off')             # Hide labels and ticks
+        ax2.stem(e[:-1],h, linefmt="grey", markerfmt=" ", basefmt=" ")
+
+        # Add line for nonparametric fit using lowess
+        ax1.plot(x_nonparametric, y_nonparametric, label="Nonparametric")
+
+        # Add line for perfect calibration
+        ax1.plot([0, 1], [0, 1], "k:", label="Perfectly calibrated")
+
+        ax1.set_xlabel('Predicted Probability')
+        ax1.set_ylabel('Actual Probability')
+        
+        props = dict(boxstyle='round', facecolor='white', alpha=0.4)
+        ax1.text(0.00, 0.75, self.__metrics_to_string(), fontsize=10, family='monospace', bbox=props)
+
+        ax1.legend(loc='best', bbox_to_anchor=(0.5, 0., 0.5, 0.5))
+
+        return fig
```

### Comparing `pycaleva-0.7.0/src/pycaleva/_report.py` & `pycaleva-0.8.0/src/pycaleva/_report.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,173 +1,173 @@
-"""
-This file holds the logic for saving calibration measurement results to reports in pdf format.
-
-
-References
-----------
-The report export functionality is using the fpdf2 package.
-https://pyfpdf.github.io/fpdf2/index.html
-
-"""
-
-from fpdf import FPDF
-from datetime import datetime
-from ._basecalib import _BaseCalibrationEvaluator
-from ._basecalib import DEVEL
-import shutil
-import os
-import tempfile
-import matplotlib.pyplot as plt
-
-
-class _Report(FPDF):
-    def __init__(self):
-        super().__init__()
-        self.__page_width = None
-
-        # Create a CalibrationEvaluator Instance to get calibration result data from
-        self.__ca = None
-
-        # Use temp directory of os to temporarily save plots to
-        self.__plot_dir = tempfile.mkdtemp() 
-        
-
-    def __header(self, model_name:str) -> None:
-        
-        # Write title
-        self.set_font('Times','B',12.0) 
-        now = datetime.now().strftime("%d/%m/%Y %H:%M:%S")
-        self.cell(self.__page_width, 0.0, f'Calibration report - {now}', align='C')
-        self.ln(8)
-
-        # Write model name
-        self.set_font('Courier', '', 10)
-        self.cell(self.__page_width/2, 0.0, f"Model: {model_name}", 0, 0, "L")
-        self.ln(8)
-
-        # Write type of evaluation
-        if self.__ca.outsample == DEVEL.INTERNAL:
-            self.cell(self.__page_width/2, 0.0, "Evaluation: Internal", 0, 0, "L")
-        else:
-            self.cell(self.__page_width/2, 0.0, "Evaluation: External", 0, 0, "L")
-        
-
-    def __contingency_table(self) -> None:
-        line_height = self.font_size * 2
-
-        df = self.__ca.contingency_table.reset_index(level=0)
-
-        col_width = self.epw / len(df.columns)  # distribute content evenly
-
-        # Write table header
-        self.set_font('Courier', 'B', 8)
-        for datum in df.columns:
-            self.multi_cell(col_width, line_height, datum, border=1, ln=3, max_line_height=self.font_size)
-        self.ln(line_height)
-
-        # Write table content
-        self.set_font('Courier', '', 8)
-        for index,row in df.iterrows():
-            for datum in row:
-                if (isinstance(datum,float)):
-                    self.multi_cell(col_width, line_height, str(round(datum,3)), border=1, ln=3, max_line_height=self.font_size)
-                else:
-                    self.multi_cell(col_width, line_height, str(datum), border=1, ln=3, max_line_height=self.font_size)
-            self.ln(line_height)
-        self.ln(8)
-
-    def __stattests(self) -> None:
-        hl = self.__ca.hosmerlemeshow(verbose=False);
-        if (hl.pvalue < 0.001):
-            self.cell(self.__page_width, 0.0, f'Hosmer Lemeshow Test: C({hl.dof})={round(hl.statistic,4)} p-value: < 0.001', align='L')
-        else:
-            self.cell(self.__page_width, 0.0, f'Hosmer Lemeshow Test: C({hl.dof})={round(hl.statistic,4)} p-value: {round(hl.pvalue,4)}', align='L')
-        self.ln(8)
-
-        ph = self.__ca.pigeonheyse(verbose=False);
-        if (ph.pvalue < 0.001):
-            self.cell(self.__page_width, 0.0, f'Pigeon Heyse Test: J²({ph.dof})={round(ph.statistic,4)} p-value: < 0.001', align='L')
-        else:
-            self.cell(self.__page_width, 0.0, f'Pigeon Heyse Test: J²({ph.dof})={round(ph.statistic,4)} p-value: {round(ph.pvalue,4)}', align='L')
-        self.ln(8)
-
-        zt = self.__ca.z_test()
-        if (zt.pvalue < 0.001):
-            self.cell(self.__page_width, 0.0, f'Spieglhalter z-test: Z={round(zt.statistic,4)} p-value: < 0.001', align='L')
-        else:
-            self.cell(self.__page_width, 0.0, f'Spieglhalter z-test: Z={round(zt.statistic,4)} p-value: {round(zt.pvalue,4)}', align='L')
-
-
-        self.ln(8)
-
-
-    def __create_plots(self):
-        # Delete folder if exists and create it again
-        try:
-            shutil.rmtree(self.__plot_dir)
-            os.mkdir(self.__plot_dir)
-
-            fig = self.__ca.calibration_plot()
-            fig.savefig(f"{self.__plot_dir}/calplot.png", dpi=300)
-            plt.close(fig)
-
-            # TODO: Make parameter devel dynamic
-            fig = self.__ca.calbelt(plot=True).fig
-            fig.savefig(f"{self.__plot_dir}/calbelt.png", dpi=300)
-            plt.close(fig)
-
-        except FileNotFoundError:
-            os.mkdir(self.__plot_dir)
-
-    def __plots(self):
-        self.__create_plots()
-
-        self.set_font('Courier', 'U', 8)
-        self.cell(self.__page_width, 0.0, 'Calibration Plot', align='L')
-        self.ln(8)
-        self.image(f'{self.__plot_dir}/calplot.png', h=self.eph/2.2, w=self.epw)
-
-
-        # Add new page
-        self.add_page()
-
-        self.set_font('Courier', 'U', 8)
-        self.cell(self.__page_width, 0.0, 'Calibration Belt', align='L')
-        self.ln(8)
-        self.image(f'{self.__plot_dir}/calbelt.png', h=self.eph/2, w=self.epw)
-        
-        # Clear temporary saved plots
-        shutil.rmtree(self.__plot_dir)
-        os.mkdir(self.__plot_dir)
-
-
-    def footer(self):
-        # Position cursor at 1.5 cm from bottom:
-        self.set_y(-15)
-        # Setting font: helvetica italic 8
-        self.set_font("helvetica", "I", 8)
-        # Printing page number:
-        self.cell(0, 10, f"Page {self.page_no()}/{{nb}}", 0, 0, "C")
-
-    def create(self, filepath:str, model_name:str, ca:_BaseCalibrationEvaluator):
-        
-        self.__ca = ca
-
-        # Add new page
-        self.add_page()
-
-        self.__page_width = self.w - 2 * self.l_margin
-
-        self.__header(model_name)   # Write header
-        self.ln(8)
-
-        self.__contingency_table()  # Write contingency table
-        self.__stattests()          # Write statistic test results
-        self.__plots()              # Write plots
-
-        try:
-            self.output(filepath, 'F')
-            print(f"Calibration report for model '{model_name}' saved to {filepath}")
-        except PermissionError:
-            raise Exception(f"Could not write report to {filepath} due to permission error. Close the file first!")
-        except FileNotFoundError:
+"""
+This file holds the logic for saving calibration measurement results to reports in pdf format.
+
+
+References
+----------
+The report export functionality is using the fpdf2 package.
+https://pyfpdf.github.io/fpdf2/index.html
+
+"""
+
+from fpdf import FPDF
+from datetime import datetime
+from ._basecalib import _BaseCalibrationEvaluator
+from ._basecalib import DEVEL
+import shutil
+import os
+import tempfile
+import matplotlib.pyplot as plt
+
+
+class _Report(FPDF):
+    def __init__(self):
+        super().__init__()
+        self.__page_width = None
+
+        # Create a CalibrationEvaluator Instance to get calibration result data from
+        self.__ca = None
+
+        # Use temp directory of os to temporarily save plots to
+        self.__plot_dir = tempfile.mkdtemp() 
+        
+
+    def __header(self, model_name:str) -> None:
+        
+        # Write title
+        self.set_font('Times','B',12.0) 
+        now = datetime.now().strftime("%d/%m/%Y %H:%M:%S")
+        self.cell(self.__page_width, 0.0, f'Calibration report - {now}', align='C')
+        self.ln(8)
+
+        # Write model name
+        self.set_font('Courier', '', 10)
+        self.cell(self.__page_width/2, 0.0, f"Model: {model_name}", 0, 0, "L")
+        self.ln(8)
+
+        # Write type of evaluation
+        if self.__ca.outsample == DEVEL.INTERNAL:
+            self.cell(self.__page_width/2, 0.0, "Evaluation: Internal", 0, 0, "L")
+        else:
+            self.cell(self.__page_width/2, 0.0, "Evaluation: External", 0, 0, "L")
+        
+
+    def __contingency_table(self) -> None:
+        line_height = self.font_size * 2
+
+        df = self.__ca.contingency_table.reset_index(level=0)
+
+        col_width = self.epw / len(df.columns)  # distribute content evenly
+
+        # Write table header
+        self.set_font('Courier', 'B', 8)
+        for datum in df.columns:
+            self.multi_cell(col_width, line_height, datum, border=1, ln=3, max_line_height=self.font_size)
+        self.ln(line_height)
+
+        # Write table content
+        self.set_font('Courier', '', 8)
+        for index,row in df.iterrows():
+            for datum in row:
+                if (isinstance(datum,float)):
+                    self.multi_cell(col_width, line_height, str(round(datum,3)), border=1, ln=3, max_line_height=self.font_size)
+                else:
+                    self.multi_cell(col_width, line_height, str(datum), border=1, ln=3, max_line_height=self.font_size)
+            self.ln(line_height)
+        self.ln(8)
+
+    def __stattests(self) -> None:
+        hl = self.__ca.hosmerlemeshow(verbose=False);
+        if (hl.pvalue < 0.001):
+            self.cell(self.__page_width, 0.0, f'Hosmer Lemeshow Test: C({hl.dof})={round(hl.statistic,4)} p-value: < 0.001', align='L')
+        else:
+            self.cell(self.__page_width, 0.0, f'Hosmer Lemeshow Test: C({hl.dof})={round(hl.statistic,4)} p-value: {round(hl.pvalue,4)}', align='L')
+        self.ln(8)
+
+        ph = self.__ca.pigeonheyse(verbose=False);
+        if (ph.pvalue < 0.001):
+            self.cell(self.__page_width, 0.0, f'Pigeon Heyse Test: J²({ph.dof})={round(ph.statistic,4)} p-value: < 0.001', align='L')
+        else:
+            self.cell(self.__page_width, 0.0, f'Pigeon Heyse Test: J²({ph.dof})={round(ph.statistic,4)} p-value: {round(ph.pvalue,4)}', align='L')
+        self.ln(8)
+
+        zt = self.__ca.z_test()
+        if (zt.pvalue < 0.001):
+            self.cell(self.__page_width, 0.0, f'Spiegelhalter z-test: Z={round(zt.statistic,4)} p-value: < 0.001', align='L')
+        else:
+            self.cell(self.__page_width, 0.0, f'Spiegelhalter z-test: Z={round(zt.statistic,4)} p-value: {round(zt.pvalue,4)}', align='L')
+
+
+        self.ln(8)
+
+
+    def __create_plots(self):
+        # Delete folder if exists and create it again
+        try:
+            shutil.rmtree(self.__plot_dir)
+            os.mkdir(self.__plot_dir)
+
+            fig = self.__ca.calibration_plot()
+            fig.savefig(f"{self.__plot_dir}/calplot.png", dpi=300)
+            plt.close(fig)
+
+            # TODO: Make parameter devel dynamic
+            fig = self.__ca.calbelt(plot=True).fig
+            fig.savefig(f"{self.__plot_dir}/calbelt.png", dpi=300)
+            plt.close(fig)
+
+        except FileNotFoundError:
+            os.mkdir(self.__plot_dir)
+
+    def __plots(self):
+        self.__create_plots()
+
+        self.set_font('Courier', 'U', 8)
+        self.cell(self.__page_width, 0.0, 'Calibration Plot', align='L')
+        self.ln(8)
+        self.image(f'{self.__plot_dir}/calplot.png', h=self.eph/2.2, w=self.epw)
+
+
+        # Add new page
+        self.add_page()
+
+        self.set_font('Courier', 'U', 8)
+        self.cell(self.__page_width, 0.0, 'Calibration Belt', align='L')
+        self.ln(8)
+        self.image(f'{self.__plot_dir}/calbelt.png', h=self.eph/2, w=self.epw)
+        
+        # Clear temporary saved plots
+        shutil.rmtree(self.__plot_dir)
+        os.mkdir(self.__plot_dir)
+
+
+    def footer(self):
+        # Position cursor at 1.5 cm from bottom:
+        self.set_y(-15)
+        # Setting font: helvetica italic 8
+        self.set_font("helvetica", "I", 8)
+        # Printing page number:
+        self.cell(0, 10, f"Page {self.page_no()}/{{nb}}", 0, 0, "C")
+
+    def create(self, filepath:str, model_name:str, ca:_BaseCalibrationEvaluator):
+        
+        self.__ca = ca
+
+        # Add new page
+        self.add_page()
+
+        self.__page_width = self.w - 2 * self.l_margin
+
+        self.__header(model_name)   # Write header
+        self.ln(8)
+
+        self.__contingency_table()  # Write contingency table
+        self.__stattests()          # Write statistic test results
+        self.__plots()              # Write plots
+
+        try:
+            self.output(filepath, 'F')
+            print(f"Calibration report for model '{model_name}' saved to {filepath}")
+        except PermissionError:
+            raise Exception(f"Could not write report to {filepath} due to permission error. Close the file first!")
+        except FileNotFoundError:
             raise Exception(f"Invalid Path for '{filepath}'!")
```

### Comparing `pycaleva-0.7.0/src/pycaleva/_result_types.py` & `pycaleva-0.8.0/src/pycaleva/_result_types.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from collections import namedtuple
-
-# DEFINE RESULT TYPES AS namedtuple
-
-__all__ = ['hltest_result', 'phtest_result', 'ztest_result', 'calbelt_result', 'metrics_result']
-
-metrics_result = namedtuple('metrics_result', ['auroc', 'brier', 'ace', 'mce', 'awlc'])
-hltest_result = namedtuple('hltest_result', ['statistic', 'pvalue', 'dof'])
-phtest_result = namedtuple('phtest_result', ['statistic', 'pvalue', 'dof'])
-ztest_result = namedtuple('ztest_result', ['statistic', 'pvalue'])
-calbelt_result = namedtuple('calbelt_result', ['statistic', 'pvalue', 'fig'])
+from collections import namedtuple
+
+# DEFINE RESULT TYPES AS namedtuple
+
+__all__ = ['hltest_result', 'phtest_result', 'ztest_result', 'calbelt_result', 'metrics_result']
+
+metrics_result = namedtuple('metrics_result', ['auroc', 'brier', 'ace', 'mce', 'awlc'])
+hltest_result = namedtuple('hltest_result', ['statistic', 'pvalue', 'dof'])
+phtest_result = namedtuple('phtest_result', ['statistic', 'pvalue', 'dof'])
+ztest_result = namedtuple('ztest_result', ['statistic', 'pvalue'])
+calbelt_result = namedtuple('calbelt_result', ['statistic', 'pvalue', 'fig'])
```

### Comparing `pycaleva-0.7.0/src/pycaleva/calbelt.py` & `pycaleva-0.8.0/src/pycaleva/calbelt.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,574 +1,574 @@
-from math import sqrt, exp, pi, asin, atan, acos
-import warnings
-
-from tqdm import tqdm
-import numpy as np
-import matplotlib.pyplot as plt
-from matplotlib.patches import Patch
-
-from scipy.stats import chi2
-from scipy.special import logit, xlogy, expit
-from scipy.integrate import quad as integrate
-from scipy.optimize import brentq, minimize, NonlinearConstraint
-
-import statsmodels.api as sm
-import statsmodels.formula.api as smf
-
-from ._result_types import *
-
-
-# DEFINE Cumulative density functions for m degrees 1 to 4
-#----------------------------------------------------------
-
-# Some scary math :(
-def cdf_m(T:float, m:int, outsample:bool, alpha:float):
-    """Defines the cumulative density functions for calibration belt of m degrees 1 to 4.
-        Available for external or internal evaluation of models.
-
-    Parameters
-    ----------
-    T: float
-        The calibration belt teststatistic.
-    m: int
-        Degress of polynomial fit.
-    outsample : bool
-        Set to True for 'external' or False for 'internal' evaluation.
-    alpha : float
-        The level of significance to use.
-
-
-    Returns:
-    -------
-        cdf : float
-            The cdf value for calibration belt according to parameters. 
-    """
-    pDegInc = 1 - alpha
-    k = chi2.ppf(1-pDegInc, 1)
-
-    # EXTERNAL EVALUATION
-    if (outsample):
-        if (T <= (m-1) * k ):
-            return 0
-        else:
-            if m == 1:
-                # EXTERNAL m=1
-                return chi2.cdf(T, 2)
-
-            elif m == 2:
-                # EXTERNAL m=2
-                return (
-                    ((chi2.cdf(T, df = 1) - 1 + pDegInc + 
-                     (-1) * sqrt(2)/sqrt(pi) * exp(-T/2) * (sqrt(T) - 
-                    sqrt(k)))/pDegInc)
-                )
-
-            elif m == 3:
-                # EXTERNAL m=3
-                integrand1 = ( lambda y: (chi2.cdf(T - y, df = 1) - 1 + pDegInc) * chi2.pdf(y, df = 1) )
-                integrand2 = ( lambda y: (sqrt(T - y) - sqrt(k)) * 1/sqrt(y) )
-
-                integral1 = integrate(integrand1, a = k, b = T - k)[0]
-                integral2 = integrate(integrand2, a = k, b = T - k)[0]
-
-                num = (integral1 - exp(-T/2)/(2 * pi) * 2 * integral2)
-                den = pDegInc**2
-                return (num/den)
-
-            elif m == 4:
-                # EXTERNAL m=4
-                integrand = ( lambda r: ( (r**2 * (exp(-(r**2)/2) - exp(-T/2)) * 
-                    (-pi * sqrt(k)/(2 * r) + 2 * sqrt(k)/r * 
-                    asin((r**2/k - 1)**(-1/2)) - 2 * atan((1 - 
-                    2 * k/r**2)**(-1/2)) + 2 * sqrt(k)/r * atan((r**2/k - 
-                    2)**(-1/2)) + 2 * atan(r/sqrt(k) * sqrt(r**2/k - 
-                    2)) - 2 * sqrt(k)/r * atan(sqrt(r**2/k - 
-                    2)))) )
-                )
-                
-                integral = integrate(integrand, a = sqrt(3 * k), b = sqrt(T))[0]
-
-                return ((2/(pi * pDegInc**2))**(3/2) * integral)
-
-            else:
-                # EXTERNEAL m>4 is not defined!
-                return NotImplemented
-
-    # INTERNAL EVALUATION
-    else:
-        if (T <= (m-2) * k):
-            return 0
-        else:
-            if m == 1:
-                # INTERNAL m=1 --> Not defined as polynial fit starts with degree 2 for internal evaluation
-                return NotImplemented
-
-            elif m == 2:
-                # INTERNAL m=2
-                return chi2.cdf(T, 1)
-
-            elif m == 3:
-                # INTERNAL m=3
-                integrand = ( lambda r: (r * exp(-(r**2)/2) * acos(sqrt(k)/r)) )
-                
-                integral = integrate(integrand, a = sqrt(k), b = sqrt(T))[0]
-                return (2/(pi * pDegInc) * integral)
-
-            elif m == 4:
-                # INTERNAL m=4
-                integrand = (lambda r: (r**2 * exp(-(r**2)/2) * (atan(sqrt(r**2/k * 
-                                (r**2/k - 2))) - sqrt(k)/r * atan(sqrt(r**2/k - 
-                                2)) - sqrt(k)/r * acos((r**2/k - 1)**(-1/2))))
-                            )
-                
-                integral = integrate(integrand, a = sqrt(2 * k), b = sqrt(T))[0]
-                return ((2/pi)**(3/2) * (pDegInc)**(-2) * integral)
-            else:
-                # INTERNAL m>4 is not defined!
-                return NotImplemented
-
-
-
-# MAIN Class for CalibrationBelt Test and Plotting
-#-----------------------------------------------------------------
-
-class CalibrationBelt():
-
-    def __init__(self, y_true:np.ndarray, y_pred:np.ndarray, outsample:bool, subset = None, confLevels=[0.8, 0.95], alpha=0.95):
-        """Calculate the calibration belt and draw plot if desired.
-        
-        Parameters
-        ----------
-        y_true : array_like
-            Expected class labels given in test set. (Ground truth y)
-        y_pred : array_like
-            Observed probabilities predicted by a classification model.
-        outsample : bool
-            Set to 'False' for internal evaluation or set to 'True'
-            for external evaluation.
-        subset: array_like
-            An optional boolean vector specifying the subset of observations to be considered.
-            Defaults to None.
-        confLevels: list
-            A numeric vector containing the confidence levels of the calibration belt.
-            Defaults to [0.8,0.95].
-        alpha: float
-            The level of significance to use.
-
-        Returns
-        -------
-        T : float
-            The Calibration plot test statistic T.
-        p : float
-            The p-value of the test.
-        fig : matplotlib.figure
-            The calibration belt plot. Only returned if plot='True'
-        
-        See Also
-        --------
-        CalibrationEvaluator.calplot
-        
-
-        Notes
-        -----
-        This is an implemenation of the test proposed by Nattino et al. [6]. 
-        The implementation was built upon the python port of the R-Package givitiR [8] and the python implementation calibration-belt [7].
-        The calibration belt estimates the true underlying calibration curve given predicted probabilities and true class labels.
-        Instead of directly drawing the calibration curve a belt is drawn using confidence levels.
-        A low value for the teststatistic and a high p-value (>0.05) indicate a well calibrated model.
-        Other than Hosmer Lemeshow Test or Pigeon Heyse Test, this test is not based on grouping strategies.
-
-        References
-        ----------
-        ..  [6] Nattino, G., Finazzi, S., & Bertolini, G. (2014). A new calibration test 
-            and a reappraisal of the calibration belt for the assessment of prediction models 
-            based on dichotomous outcomes. Statistics in medicine, 33(14), 2390-2407.
-
-        ..  [7] Bulgarelli, L. (2021). calibrattion-belt: Assessment of calibration in binomial prediction models [Computer software].
-            Available from https://github.com/fabiankueppers/calibration-framework
-
-        ..  [8] Nattino, G., Finazzi, S., Bertolini, G., Rossi, C., & Carrara, G. (2017).
-            givitiR: The giviti calibration test and belt (R package version 1.3) [Computer
-            software]. The Comprehensive R Archive Network.
-            Available from https://CRAN.R-project.org/package=givitiR
-        
-
-        Examples
-        --------
-        >>> from pycaleva import CalibrationBelt
-        >>> cb = CalibrationBelt(y_test, pred_prob, outsample=True)
-        >>> cb.stats()
-        >>> cb.plot()
-        """
-        
-        # Check parameters
-        self.__check_parameters(y_true,y_pred,outsample,alpha)
-
-        if not subset is None:
-            # Pick a random subset from data
-            idx = np.random.choice(np.arange(len(y_true)), subset, replace=False)
-            self.__y = y_true[idx]
-            self.__p = y_pred[idx]
-        else:
-            self.__y = y_true
-            self.__p = y_pred
-
-        self.__clip_probs()
-        self.__n = len(self.__y)
-
-        # Warn user at internal evaluation
-        if not outsample:
-            warnings.warn("Evaluation only valid for Logistic Regression Models");
-
-        self.__outsample = outsample
-
-        self.__confLevels = sorted(confLevels, reverse=True)
-        self.__logit_e = logit(self.__p)   # Get logit form of predicted probabilities
-
-        # Find polynomial fit using forward selection procedure
-        self.__maxDeg = 4
-        self.__model, self.__m =  self.__forward_select(alpha, self.__maxDeg)
-
-        # Get teststatistic and p-value
-        self.__T, self.__pval = self.__test(alpha)
-
-        self.__boundaries = {}
-
-
-    def __check_parameters(self, y, p, outsample, alpha) -> bool:
-        if (len(y) != len(p)):
-            raise ValueError("Observations y_true and Predictions y_pred differ in size!")
-        if not ( ((y==0) | (y==1)).all() ):
-            raise ValueError("Invalid class labels! y_train must be dichotomous containing only values 0 or 1")
-        if ( (p < 0.0 ).any() or (p > 1.0).any() ):
-            raise ValueError("Predicted probabilities y_pred must be in range [0.0 1.0]!")
-        if (alpha < 0.0 or alpha > 1.0):
-            raise ValueError("Alpha must be in range 0.0 - 1.0")
-        if (abs( p.sum() - y.sum() ) < 1e-04 ) and outsample == True:
-            warnings.warn("Please set parameter outsample to 'false' if the evaluated model was fit on this dataset!", "UserWarning")
-        if ( y.sum() <= 1 ) or ( y.sum() >= (len(y) - 1) ):
-            raise ValueError("The number of events/non events in observations can not be less than 1.")
-
-        return True
-
-    # Avoid probabilities to be exactly zero or one
-    def __clip_probs(self):
-        self.__p = np.clip(self.__p, 1e-10, 1-(1e-10))
-    
-
-    # Find polynomial fit using forward selection process
-    def __forward_select(self, alpha, maxDeg):
-        family = sm.families.Binomial()
-        m = 0
-
-        if (self.__outsample):
-            m_start = 1
-            fit_formula = f"o ~ {m_start} + "
-        else:
-            m_start = 2
-            fit_formula = f"o ~ I(ge ** {m_start-1}) + "
-        
-        data = {"o": self.__y, "ge": self.__logit_e}
-        inv_chi2 = chi2.ppf(alpha, 1)
-
-        n = m_start
-        while n <= maxDeg:
-            # Add new term
-            fit_formula += f"I(ge ** {n})"
-
-            fit_new = smf.glm(formula=fit_formula, data=data,family=family).fit()
-
-            if n > m_start:
-                # Log-likelihood ratio test
-                Dm = (2 * (fit.llf - fit_new.llf))
-
-                # Use previous order for m if model does not improve
-                if Dm < inv_chi2:
-                    m = n-1
-                    break
-
-            m = n
-            fit = fit_new
-            n += 1
-
-            fit_formula += " + "
-        return(fit, m)
-
-
-    def __test(self, alpha):
-        # Log-Likelihood of perfectly calibrated model (y_i = p_i)
-        llf_perfect = np.sum(xlogy(self.__y, self.__p) + xlogy(1 - self.__y, 1 - self.__p))
-        T = 2 * (self.__model.llf - llf_perfect)
-
-        pval = 1 - cdf_m(T, self.__m, self.__outsample, alpha)
-
-        return T, pval
-
-
-    def _root_fun(self, x, *args):
-        m, q, confidence = args
-        return cdf_m(x, m, self.__outsample, q) - confidence
-
-
-    def _fun(self, alpha, *args):
-        geM, sign = args
-        return sign * (alpha @ geM)
-
-
-    def _jac(self, alpha, *args):
-        geM, sign = args
-        return sign * geM
-
-
-    def __calculate_boundaries(self, confidence, size=50, q=.95, **kwargs):
-        # Cache boundaries for each confidence interval to save the parameters used in their calculation.
-        if confidence in self.__boundaries:
-            params = self.__boundaries[confidence]["params"]
-
-            # If a request for the same interval is requested
-            # it is only calculted one of the parameters change.
-            # The parameters that modify the belt are (size, q, m).
-            # In the case `size` changes, we compute the boundaries
-            # only if the new `size` is greater than the previously used.
-            
-            if (size <= params["size"] and
-                    q == params["q"] and
-                    self.__m == params["m"]):
-                return self.boundaries[confidence]["boundaries"]
-
-        # New parameters
-        params = {"size": size, "q": q, "m": self.__m}
-
-        # Find ky
-        if self.__outsample:
-            ky = (self.__m - 1) * chi2.ppf(q, 1)
-        else:
-            ky = (self.__m - 2) * chi2.ppf(q, 1)
-
-            try:
-                cdf_m(ky, self.__m, self.__outsample, q)
-            except:
-                ky += 1e-04
-
-
-        args = self.__m, q, confidence
-
-
-        k = brentq(self._root_fun, ky, 40, args=args)
-
-        # Calculate logit(E) matrix
-        M = np.linspace([0], [self.__m], num = self.__m + 1, axis=1)
-        Ge = logit(self.__p)[np.newaxis]
-        GeM = Ge.T ** M
-
-        # Upper boundary (Eq27)
-        boundary = self.__model.llf - k / 2
-
-        # Create subset based on size
-        logit_sub = np.linspace(np.min(Ge), np.max(Ge), num=size//2)
-        e_sub = np.linspace(np.min(self.__p), np.max(self.__p), num=size//2)
-        Ge_sub = np.sort(np.append(logit_sub, logit(e_sub)))
-        GeM_sub = Ge_sub[np.newaxis].T ** M
-
-        # Constraint function (Eq27)
-        def fun_lalpha(alpha):
-            # Calculate probability
-            alphaE = expit(GeM @ alpha)
-
-            # Clip probability to epsilon so
-            # we can compute log-likelihood
-            eps = 1e-5
-            alphaE = np.clip(alphaE, eps, 1-eps)
-
-            # Compute Log-likelihood
-            lalpha = xlogy(self.__y, alphaE) + xlogy(1-self.__y, 1 - alphaE)
-            return np.nansum(lalpha)
-
-        def jac_lalpha(alpha):
-            # Calculate probability
-            alphaE = expit(GeM @ alpha)
-            return (self.__y - alphaE) @ GeM
-
-
-        constraints = NonlinearConstraint(
-                fun_lalpha,
-                boundary, 0,
-                jac_lalpha,
-                keep_feasible=True
-            )
-
-        def _minimize(args):
-            return minimize(
-                fun=self._fun, x0=self.__model.params, args=args,
-                method='trust-constr', jac=self._jac,
-                hess=lambda alpha, *args: np.zeros((self.__m+1,)),
-                constraints=constraints, tol=1e-4
-            ).x
-
-        
-        lower, upper = [], []
-        for geM in tqdm(GeM_sub):
-            
-            # Minimize alpha to find lower bound
-            args = (geM, 1)
-            min_alpha = _minimize(args)
-
-            # Maximize alpha to find upper bound
-            args = (geM, -1)
-            max_alpha = _minimize(args)
-
-            # Calculate bounds
-            lower.append(expit(min_alpha @ geM))
-            upper.append(expit(max_alpha @ geM))
-
-
-        # Save parameters
-        boundaries = np.array([expit(Ge_sub), lower, upper]).T
-        self.__boundaries[confidence] = {
-            "params": params,
-            "boundaries": boundaries
-        }
-        
-        return boundaries
-
-
-    def __get_plot_text(self):
-        infos = {"Degree Fit":self.__m, "n":self.__n, "T":self.__T}
-
-        lines = ['{:<10s}{:>8d}'.format("n",self.__n)]
-        lines = []
-        for k, v in infos.items():
-            if (isinstance(v,int)):
-                lines.append('{:<10s}{:>8d}'.format(k,v))
-            else:
-                lines.append('{:<10s}{:>8.3f}'.format(k,v))
-        
-        # Set text for p-value
-        if self.__pval < .001:
-            lines.append('{:<10s}{:>8s}'.format("p-value","< 0.001"))
-        else:
-            lines.append('{:<10s}{:>8.3f}'.format("p-value",self.__pval))
-
-        textstr = '\n'.join(lines)
-        return textstr
-
-
-    # Return teststatistic and p-value
-    def stats(self):
-        """Get the calibration belt test result, withour drawing the plot.
-
-        Returns
-        -------
-            T : float
-                The Calibration plot test statistic T.
-            p : float
-                The p-value of the test.
-
-        Notes
-        -----
-        A low value for the teststatistic and a high p-value (>0.05) indicate a well calibrated model.
-
-        Examples
-        --------
-        >>> from pycaleva.calbelt import CalibrationBelt
-        >>> cb = CalibrationBelt(y_test, pred_prob, outsample=True)
-        >>> cb.stats()
-        calbelt_result(statistic=1.6111330037643796, pvalue=0.4468347221346196, fig=None)
-        """
-
-        return calbelt_result(self.__T, self.__pval, None)
-
-
-
-    def plot(self, alpha=.95, **kwargs):
-        """Draw the calibration belt plot.
-        
-        Parameters
-        ----------
-        alpha: float, optional
-            Sets the significance level.
-        confLevels: list, optional
-            Set the confidence intervalls for the calibration belt.
-            Defaults to [0.8,0.95].
-
-        Returns
-        -------
-        T : float
-            The Calibration plot test statistic T.
-        p : float
-            The p-value of the test.
-        fig : matplotlib.figure
-            The calibration belt plot. Only returned if plot='True'
-        
-        See Also
-        --------
-        CalibrationEvaluator.calbelt
-        
-
-        Notes
-        -----
-        This is an implemenation of the test proposed by Nattino et al. [6]. 
-        The implementation was built upon the python port of the R-Package givitiR [8] and the python implementation calibration-belt [7].
-        The calibration belt estimates the true underlying calibration curve given predicted probabilities and true class labels.
-        Instead of directly drawing the calibration curve a belt is drawn using confidence levels.
-        A low value for the teststatistic and a high p-value (>0.05) indicate a well calibrated model.
-        Other than Hosmer Lemeshow Test or Pigeon Heyse Test, this test is not based on grouping strategies.
-
-        References
-        ----------
-        ..  [6] Nattino, G., Finazzi, S., & Bertolini, G. (2014). A new calibration test 
-            and a reappraisal of the calibration belt for the assessment of prediction models 
-            based on dichotomous outcomes. Statistics in medicine, 33(14), 2390-2407.
-
-        ..  [7] Bulgarelli, L. (2021). calibrattion-belt: Assessment of calibration in binomial prediction models [Computer software].
-            Available from https://github.com/lbulgarelli/calibration
-
-        ..  [8] Nattino, G., Finazzi, S., Bertolini, G., Rossi, C., & Carrara, G. (2017).
-            givitiR: The giviti calibration test and belt (R package version 1.3) [Computer
-            software]. The Comprehensive R Archive Network.
-            Available from https://CRAN.R-project.org/package=givitiR
-        
-
-        Examples
-        --------
-        >>> from pycaleva.calbelt import CalibrationBelt
-        >>> cb = CalibrationBelt(y_test, pred_prob, outsample=True)
-        >>> cb.plot()
-        calbelt_result(statistic=1.6111330037643796, pvalue=0.4468347221346196, fig=matplotlib.figure)
-
-        """
-
-        for confidence in self.__confLevels:
-            self.__calculate_boundaries(confidence, q=alpha, **kwargs)
-
-        # Plot stats
-        fig, ax = plt.subplots(1, figsize=(10,6))
-
-        # Info Textbox upper left
-        props = dict(boxstyle='round', facecolor='white', alpha=0.4)
-        ax.text(0.00, 0.85, self.__get_plot_text(), fontsize=10, family='monospace', bbox=props)
-
-        # Set primary color belt
-        facecol = 'cornflowerblue' 
-
-        # Set alpha of colour for each confidence level
-        col_alphas = np.linspace(start=0.9, stop=0.4, num=len(self.__confLevels) )
-        
-        legend_elements = []
-
-        # Update boundary and legend for each confidence level
-        for i,confLevel in enumerate(self.__confLevels):
-            legend_elements.append( Patch(facecolor=facecol, alpha=col_alphas[i], label=f'{int(confLevel*100)}%') )
-            bound = self.__boundaries[confLevel]["boundaries"].T
-            ax.fill_between(bound[0], bound[1], bound[2], color='white', alpha=1)
-            ax.fill_between(bound[0], bound[1], bound[2], color=facecol, alpha=col_alphas[i])
-
-        # Set legend
-        ax.legend(title='Confidence level', handles=legend_elements, loc='lower right')
-
-        ax.set_xlabel('Predicted Probability')
-        ax.set_ylabel('Actual Probability')
-
-        # Plot perfect calibration using doted line
-        ax.plot([0, 1], [0, 1], "k:")
-
+from math import sqrt, exp, pi, asin, atan, acos
+import warnings
+
+from tqdm import tqdm
+import numpy as np
+import matplotlib.pyplot as plt
+from matplotlib.patches import Patch
+
+from scipy.stats import chi2
+from scipy.special import logit, xlogy, expit
+from scipy.integrate import quad as integrate
+from scipy.optimize import brentq, minimize, NonlinearConstraint
+
+import statsmodels.api as sm
+import statsmodels.formula.api as smf
+
+from ._result_types import *
+
+
+# DEFINE Cumulative density functions for m degrees 1 to 4
+#----------------------------------------------------------
+
+# Some scary math :(
+def cdf_m(T:float, m:int, outsample:bool, alpha:float):
+    """Defines the cumulative density functions for calibration belt of m degrees 1 to 4.
+        Available for external or internal evaluation of models.
+
+    Parameters
+    ----------
+    T: float
+        The calibration belt teststatistic.
+    m: int
+        Degress of polynomial fit.
+    outsample : bool
+        Set to True for 'external' or False for 'internal' evaluation.
+    alpha : float
+        The level of significance to use.
+
+
+    Returns:
+    -------
+        cdf : float
+            The cdf value for calibration belt according to parameters. 
+    """
+    pDegInc = 1 - alpha
+    k = chi2.ppf(1-pDegInc, 1)
+
+    # EXTERNAL EVALUATION
+    if (outsample):
+        if (T <= (m-1) * k ):
+            return 0
+        else:
+            if m == 1:
+                # EXTERNAL m=1
+                return chi2.cdf(T, 2)
+
+            elif m == 2:
+                # EXTERNAL m=2
+                return (
+                    ((chi2.cdf(T, df = 1) - 1 + pDegInc + 
+                     (-1) * sqrt(2)/sqrt(pi) * exp(-T/2) * (sqrt(T) - 
+                    sqrt(k)))/pDegInc)
+                )
+
+            elif m == 3:
+                # EXTERNAL m=3
+                integrand1 = ( lambda y: (chi2.cdf(T - y, df = 1) - 1 + pDegInc) * chi2.pdf(y, df = 1) )
+                integrand2 = ( lambda y: (sqrt(T - y) - sqrt(k)) * 1/sqrt(y) )
+
+                integral1 = integrate(integrand1, a = k, b = T - k)[0]
+                integral2 = integrate(integrand2, a = k, b = T - k)[0]
+
+                num = (integral1 - exp(-T/2)/(2 * pi) * 2 * integral2)
+                den = pDegInc**2
+                return (num/den)
+
+            elif m == 4:
+                # EXTERNAL m=4
+                integrand = ( lambda r: ( (r**2 * (exp(-(r**2)/2) - exp(-T/2)) * 
+                    (-pi * sqrt(k)/(2 * r) + 2 * sqrt(k)/r * 
+                    asin((r**2/k - 1)**(-1/2)) - 2 * atan((1 - 
+                    2 * k/r**2)**(-1/2)) + 2 * sqrt(k)/r * atan((r**2/k - 
+                    2)**(-1/2)) + 2 * atan(r/sqrt(k) * sqrt(r**2/k - 
+                    2)) - 2 * sqrt(k)/r * atan(sqrt(r**2/k - 
+                    2)))) )
+                )
+                
+                integral = integrate(integrand, a = sqrt(3 * k), b = sqrt(T))[0]
+
+                return ((2/(pi * pDegInc**2))**(3/2) * integral)
+
+            else:
+                # EXTERNEAL m>4 is not defined!
+                return NotImplemented
+
+    # INTERNAL EVALUATION
+    else:
+        if (T <= (m-2) * k):
+            return 0
+        else:
+            if m == 1:
+                # INTERNAL m=1 --> Not defined as polynial fit starts with degree 2 for internal evaluation
+                return NotImplemented
+
+            elif m == 2:
+                # INTERNAL m=2
+                return chi2.cdf(T, 1)
+
+            elif m == 3:
+                # INTERNAL m=3
+                integrand = ( lambda r: (r * exp(-(r**2)/2) * acos(sqrt(k)/r)) )
+                
+                integral = integrate(integrand, a = sqrt(k), b = sqrt(T))[0]
+                return (2/(pi * pDegInc) * integral)
+
+            elif m == 4:
+                # INTERNAL m=4
+                integrand = (lambda r: (r**2 * exp(-(r**2)/2) * (atan(sqrt(r**2/k * 
+                                (r**2/k - 2))) - sqrt(k)/r * atan(sqrt(r**2/k - 
+                                2)) - sqrt(k)/r * acos((r**2/k - 1)**(-1/2))))
+                            )
+                
+                integral = integrate(integrand, a = sqrt(2 * k), b = sqrt(T))[0]
+                return ((2/pi)**(3/2) * (pDegInc)**(-2) * integral)
+            else:
+                # INTERNAL m>4 is not defined!
+                return NotImplemented
+
+
+
+# MAIN Class for CalibrationBelt Test and Plotting
+#-----------------------------------------------------------------
+
+class CalibrationBelt():
+
+    def __init__(self, y_true:np.ndarray, y_pred:np.ndarray, outsample:bool, subset = None, confLevels=[0.8, 0.95], alpha=0.95):
+        """Calculate the calibration belt and draw plot if desired.
+        
+        Parameters
+        ----------
+        y_true : array_like
+            Expected class labels given in test set. (Ground truth y)
+        y_pred : array_like
+            Observed probabilities predicted by a classification model.
+        outsample : bool
+            Set to 'False' for internal evaluation or set to 'True'
+            for external evaluation.
+        subset: array_like
+            An optional boolean vector specifying the subset of observations to be considered.
+            Defaults to None.
+        confLevels: list
+            A numeric vector containing the confidence levels of the calibration belt.
+            Defaults to [0.8,0.95].
+        alpha: float
+            The level of significance to use.
+
+        Returns
+        -------
+        T : float
+            The Calibration plot test statistic T.
+        p : float
+            The p-value of the test.
+        fig : matplotlib.figure
+            The calibration belt plot. Only returned if plot='True'
+        
+        See Also
+        --------
+        CalibrationEvaluator.calplot
+        
+
+        Notes
+        -----
+        This is an implemenation of the test proposed by Nattino et al. [6]. 
+        The implementation was built upon the python port of the R-Package givitiR [8] and the python implementation calibration-belt [7].
+        The calibration belt estimates the true underlying calibration curve given predicted probabilities and true class labels.
+        Instead of directly drawing the calibration curve a belt is drawn using confidence levels.
+        A low value for the teststatistic and a high p-value (>0.05) indicate a well calibrated model.
+        Other than Hosmer Lemeshow Test or Pigeon Heyse Test, this test is not based on grouping strategies.
+
+        References
+        ----------
+        ..  [6] Nattino, G., Finazzi, S., & Bertolini, G. (2014). A new calibration test 
+            and a reappraisal of the calibration belt for the assessment of prediction models 
+            based on dichotomous outcomes. Statistics in medicine, 33(14), 2390-2407.
+
+        ..  [7] Bulgarelli, L. (2021). calibrattion-belt: Assessment of calibration in binomial prediction models [Computer software].
+            Available from https://github.com/fabiankueppers/calibration-framework
+
+        ..  [8] Nattino, G., Finazzi, S., Bertolini, G., Rossi, C., & Carrara, G. (2017).
+            givitiR: The giviti calibration test and belt (R package version 1.3) [Computer
+            software]. The Comprehensive R Archive Network.
+            Available from https://CRAN.R-project.org/package=givitiR
+        
+
+        Examples
+        --------
+        >>> from pycaleva import CalibrationBelt
+        >>> cb = CalibrationBelt(y_test, pred_prob, outsample=True)
+        >>> cb.stats()
+        >>> cb.plot()
+        """
+        
+        # Check parameters
+        self.__check_parameters(y_true,y_pred,outsample,alpha)
+
+        if not subset is None:
+            # Pick a random subset from data
+            idx = np.random.choice(np.arange(len(y_true)), subset, replace=False)
+            self.__y = y_true[idx]
+            self.__p = y_pred[idx]
+        else:
+            self.__y = y_true
+            self.__p = y_pred
+
+        self.__clip_probs()
+        self.__n = len(self.__y)
+
+        # Warn user at internal evaluation
+        if not outsample:
+            warnings.warn("Evaluation only valid for Logistic Regression Models");
+
+        self.__outsample = outsample
+
+        self.__confLevels = sorted(confLevels, reverse=True)
+        self.__logit_e = logit(self.__p)   # Get logit form of predicted probabilities
+
+        # Find polynomial fit using forward selection procedure
+        self.__maxDeg = 4
+        self.__model, self.__m =  self.__forward_select(alpha, self.__maxDeg)
+
+        # Get teststatistic and p-value
+        self.__T, self.__pval = self.__test(alpha)
+
+        self.__boundaries = {}
+
+
+    def __check_parameters(self, y, p, outsample, alpha) -> bool:
+        if (len(y) != len(p)):
+            raise ValueError("Observations y_true and Predictions y_pred differ in size!")
+        if not ( ((y==0) | (y==1)).all() ):
+            raise ValueError("Invalid class labels! y_train must be dichotomous containing only values 0 or 1")
+        if ( (p < 0.0 ).any() or (p > 1.0).any() ):
+            raise ValueError("Predicted probabilities y_pred must be in range [0.0 1.0]!")
+        if (alpha < 0.0 or alpha > 1.0):
+            raise ValueError("Alpha must be in range 0.0 - 1.0")
+        if (abs( p.sum() - y.sum() ) < 1e-04 ) and outsample == True:
+            warnings.warn("Please set parameter outsample to 'false' if the evaluated model was fit on this dataset!", "UserWarning")
+        if ( y.sum() <= 1 ) or ( y.sum() >= (len(y) - 1) ):
+            raise ValueError("The number of events/non events in observations can not be less than 1.")
+
+        return True
+
+    # Avoid probabilities to be exactly zero or one
+    def __clip_probs(self):
+        self.__p = np.clip(self.__p, 1e-10, 1-(1e-10))
+    
+
+    # Find polynomial fit using forward selection process
+    def __forward_select(self, alpha, maxDeg):
+        family = sm.families.Binomial()
+        m = 0
+
+        if (self.__outsample):
+            m_start = 1
+            fit_formula = f"o ~ {m_start} + "
+        else:
+            m_start = 2
+            fit_formula = f"o ~ I(ge ** {m_start-1}) + "
+        
+        data = {"o": self.__y, "ge": self.__logit_e}
+        inv_chi2 = chi2.ppf(alpha, 1)
+
+        n = m_start
+        while n <= maxDeg:
+            # Add new term
+            fit_formula += f"I(ge ** {n})"
+
+            fit_new = smf.glm(formula=fit_formula, data=data,family=family).fit()
+
+            if n > m_start:
+                # Log-likelihood ratio test
+                Dm = (2 * (fit.llf - fit_new.llf))
+
+                # Use previous order for m if model does not improve
+                if Dm < inv_chi2:
+                    m = n-1
+                    break
+
+            m = n
+            fit = fit_new
+            n += 1
+
+            fit_formula += " + "
+        return(fit, m)
+
+
+    def __test(self, alpha):
+        # Log-Likelihood of perfectly calibrated model (y_i = p_i)
+        llf_perfect = np.sum(xlogy(self.__y, self.__p) + xlogy(1 - self.__y, 1 - self.__p))
+        T = 2 * (self.__model.llf - llf_perfect)
+
+        pval = 1 - cdf_m(T, self.__m, self.__outsample, alpha)
+
+        return T, pval
+
+
+    def _root_fun(self, x, *args):
+        m, q, confidence = args
+        return cdf_m(x, m, self.__outsample, q) - confidence
+
+
+    def _fun(self, alpha, *args):
+        geM, sign = args
+        return sign * (alpha @ geM)
+
+
+    def _jac(self, alpha, *args):
+        geM, sign = args
+        return sign * geM
+
+
+    def __calculate_boundaries(self, confidence, size=50, q=.95, **kwargs):
+        # Cache boundaries for each confidence interval to save the parameters used in their calculation.
+        if confidence in self.__boundaries:
+            params = self.__boundaries[confidence]["params"]
+
+            # If a request for the same interval is requested
+            # it is only calculted one of the parameters change.
+            # The parameters that modify the belt are (size, q, m).
+            # In the case `size` changes, we compute the boundaries
+            # only if the new `size` is greater than the previously used.
+            
+            if (size <= params["size"] and
+                    q == params["q"] and
+                    self.__m == params["m"]):
+                return self.boundaries[confidence]["boundaries"]
+
+        # New parameters
+        params = {"size": size, "q": q, "m": self.__m}
+
+        # Find ky
+        if self.__outsample:
+            ky = (self.__m - 1) * chi2.ppf(q, 1)
+        else:
+            ky = (self.__m - 2) * chi2.ppf(q, 1)
+
+            try:
+                cdf_m(ky, self.__m, self.__outsample, q)
+            except:
+                ky += 1e-04
+
+
+        args = self.__m, q, confidence
+
+
+        k = brentq(self._root_fun, ky, 40, args=args)
+
+        # Calculate logit(E) matrix
+        M = np.linspace([0], [self.__m], num = self.__m + 1, axis=1)
+        Ge = logit(self.__p)[np.newaxis]
+        GeM = Ge.T ** M
+
+        # Upper boundary (Eq27)
+        boundary = self.__model.llf - k / 2
+
+        # Create subset based on size
+        logit_sub = np.linspace(np.min(Ge), np.max(Ge), num=size//2)
+        e_sub = np.linspace(np.min(self.__p), np.max(self.__p), num=size//2)
+        Ge_sub = np.sort(np.append(logit_sub, logit(e_sub)))
+        GeM_sub = Ge_sub[np.newaxis].T ** M
+
+        # Constraint function (Eq27)
+        def fun_lalpha(alpha):
+            # Calculate probability
+            alphaE = expit(GeM @ alpha)
+
+            # Clip probability to epsilon so
+            # we can compute log-likelihood
+            eps = 1e-5
+            alphaE = np.clip(alphaE, eps, 1-eps)
+
+            # Compute Log-likelihood
+            lalpha = xlogy(self.__y, alphaE) + xlogy(1-self.__y, 1 - alphaE)
+            return np.nansum(lalpha)
+
+        def jac_lalpha(alpha):
+            # Calculate probability
+            alphaE = expit(GeM @ alpha)
+            return (self.__y - alphaE) @ GeM
+
+
+        constraints = NonlinearConstraint(
+                fun_lalpha,
+                boundary, 0,
+                jac_lalpha,
+                keep_feasible=True
+            )
+
+        def _minimize(args):
+            return minimize(
+                fun=self._fun, x0=self.__model.params, args=args,
+                method='trust-constr', jac=self._jac,
+                hess=lambda alpha, *args: np.zeros((self.__m+1,)),
+                constraints=constraints, tol=1e-4
+            ).x
+
+        
+        lower, upper = [], []
+        for geM in tqdm(GeM_sub):
+            
+            # Minimize alpha to find lower bound
+            args = (geM, 1)
+            min_alpha = _minimize(args)
+
+            # Maximize alpha to find upper bound
+            args = (geM, -1)
+            max_alpha = _minimize(args)
+
+            # Calculate bounds
+            lower.append(expit(min_alpha @ geM))
+            upper.append(expit(max_alpha @ geM))
+
+
+        # Save parameters
+        boundaries = np.array([expit(Ge_sub), lower, upper]).T
+        self.__boundaries[confidence] = {
+            "params": params,
+            "boundaries": boundaries
+        }
+        
+        return boundaries
+
+
+    def __get_plot_text(self):
+        infos = {"Degree Fit":self.__m, "n":self.__n, "T":self.__T}
+
+        lines = ['{:<10s}{:>8d}'.format("n",self.__n)]
+        lines = []
+        for k, v in infos.items():
+            if (isinstance(v,int)):
+                lines.append('{:<10s}{:>8d}'.format(k,v))
+            else:
+                lines.append('{:<10s}{:>8.3f}'.format(k,v))
+        
+        # Set text for p-value
+        if self.__pval < .001:
+            lines.append('{:<10s}{:>8s}'.format("p-value","< 0.001"))
+        else:
+            lines.append('{:<10s}{:>8.3f}'.format("p-value",self.__pval))
+
+        textstr = '\n'.join(lines)
+        return textstr
+
+
+    # Return teststatistic and p-value
+    def stats(self):
+        """Get the calibration belt test result, withour drawing the plot.
+
+        Returns
+        -------
+            T : float
+                The Calibration plot test statistic T.
+            p : float
+                The p-value of the test.
+
+        Notes
+        -----
+        A low value for the teststatistic and a high p-value (>0.05) indicate a well calibrated model.
+
+        Examples
+        --------
+        >>> from pycaleva.calbelt import CalibrationBelt
+        >>> cb = CalibrationBelt(y_test, pred_prob, outsample=True)
+        >>> cb.stats()
+        calbelt_result(statistic=1.6111330037643796, pvalue=0.4468347221346196, fig=None)
+        """
+
+        return calbelt_result(self.__T, self.__pval, None)
+
+
+
+    def plot(self, alpha=.95, **kwargs):
+        """Draw the calibration belt plot.
+        
+        Parameters
+        ----------
+        alpha: float, optional
+            Sets the significance level.
+        confLevels: list, optional
+            Set the confidence intervalls for the calibration belt.
+            Defaults to [0.8,0.95].
+
+        Returns
+        -------
+        T : float
+            The Calibration plot test statistic T.
+        p : float
+            The p-value of the test.
+        fig : matplotlib.figure
+            The calibration belt plot. Only returned if plot='True'
+        
+        See Also
+        --------
+        CalibrationEvaluator.calbelt
+        
+
+        Notes
+        -----
+        This is an implemenation of the test proposed by Nattino et al. [6]. 
+        The implementation was built upon the python port of the R-Package givitiR [8] and the python implementation calibration-belt [7].
+        The calibration belt estimates the true underlying calibration curve given predicted probabilities and true class labels.
+        Instead of directly drawing the calibration curve a belt is drawn using confidence levels.
+        A low value for the teststatistic and a high p-value (>0.05) indicate a well calibrated model.
+        Other than Hosmer Lemeshow Test or Pigeon Heyse Test, this test is not based on grouping strategies.
+
+        References
+        ----------
+        ..  [6] Nattino, G., Finazzi, S., & Bertolini, G. (2014). A new calibration test 
+            and a reappraisal of the calibration belt for the assessment of prediction models 
+            based on dichotomous outcomes. Statistics in medicine, 33(14), 2390-2407.
+
+        ..  [7] Bulgarelli, L. (2021). calibrattion-belt: Assessment of calibration in binomial prediction models [Computer software].
+            Available from https://github.com/lbulgarelli/calibration
+
+        ..  [8] Nattino, G., Finazzi, S., Bertolini, G., Rossi, C., & Carrara, G. (2017).
+            givitiR: The giviti calibration test and belt (R package version 1.3) [Computer
+            software]. The Comprehensive R Archive Network.
+            Available from https://CRAN.R-project.org/package=givitiR
+        
+
+        Examples
+        --------
+        >>> from pycaleva.calbelt import CalibrationBelt
+        >>> cb = CalibrationBelt(y_test, pred_prob, outsample=True)
+        >>> cb.plot()
+        calbelt_result(statistic=1.6111330037643796, pvalue=0.4468347221346196, fig=matplotlib.figure)
+
+        """
+
+        for confidence in self.__confLevels:
+            self.__calculate_boundaries(confidence, q=alpha, **kwargs)
+
+        # Plot stats
+        fig, ax = plt.subplots(1, figsize=(10,6))
+
+        # Info Textbox upper left
+        props = dict(boxstyle='round', facecolor='white', alpha=0.4)
+        ax.text(0.00, 0.85, self.__get_plot_text(), fontsize=10, family='monospace', bbox=props)
+
+        # Set primary color belt
+        facecol = 'cornflowerblue' 
+
+        # Set alpha of colour for each confidence level
+        col_alphas = np.linspace(start=0.9, stop=0.4, num=len(self.__confLevels) )
+        
+        legend_elements = []
+
+        # Update boundary and legend for each confidence level
+        for i,confLevel in enumerate(self.__confLevels):
+            legend_elements.append( Patch(facecolor=facecol, alpha=col_alphas[i], label=f'{int(confLevel*100)}%') )
+            bound = self.__boundaries[confLevel]["boundaries"].T
+            ax.fill_between(bound[0], bound[1], bound[2], color='white', alpha=1)
+            ax.fill_between(bound[0], bound[1], bound[2], color=facecol, alpha=col_alphas[i])
+
+        # Set legend
+        ax.legend(title='Confidence level', handles=legend_elements, loc='lower right')
+
+        ax.set_xlabel('Predicted Probability')
+        ax.set_ylabel('Actual Probability')
+
+        # Plot perfect calibration using doted line
+        ax.plot([0, 1], [0, 1], "k:")
+
         return calbelt_result(self.__T, self.__pval, fig)
```

### Comparing `pycaleva-0.7.0/src/pycaleva/calibeval.py` & `pycaleva-0.8.0/src/pycaleva/calibeval.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-
-""" This module holds the class *CalibrationEvaluator* that bundles all functionalities of the PyCalEva Framework."""
-
-from ._basecalib import _BaseCalibrationEvaluator
-from ._report import _Report
-
-__all__ = ['CalibrationEvaluator']
-
-
-# This class extends the _BaseCalibrationEvaluator adding a pdf-Report functionality
-class CalibrationEvaluator(_BaseCalibrationEvaluator):
-    # Docstring inherited from _BaseCalibrationEvaluator !!
-
-    def calibration_report(self, filepath:str, model_name:str) -> None:
-        """Create a pdf-report including statistical tests and plots regarding the calibration of a binary classification model.
-
-        Parameters
-        ----------
-            filepath: str
-                    The filepath for the output file. Must end with '.pdf'
-            model_name: str
-                    The name for the evaluated model.
-        """
+
+""" This module holds the class *CalibrationEvaluator* that bundles all functionalities of the PyCalEva Framework."""
+
+from ._basecalib import _BaseCalibrationEvaluator
+from ._report import _Report
+
+__all__ = ['CalibrationEvaluator']
+
+
+# This class extends the _BaseCalibrationEvaluator adding a pdf-Report functionality
+class CalibrationEvaluator(_BaseCalibrationEvaluator):
+    # Docstring inherited from _BaseCalibrationEvaluator !!
+
+    def calibration_report(self, filepath:str, model_name:str) -> None:
+        """Create a pdf-report including statistical tests and plots regarding the calibration of a binary classification model.
+
+        Parameters
+        ----------
+            filepath: str
+                    The filepath for the output file. Must end with '.pdf'
+            model_name: str
+                    The name for the evaluated model.
+        """
         _Report().create(filepath, model_name, self)
```

### Comparing `pycaleva-0.7.0/src/pycaleva/metrics.py` & `pycaleva-0.8.0/src/pycaleva/metrics.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-"""
-This module holds some metrics in context of calibration measurement of binary probabilistic classfication.
-"""
-
-import numpy as np
-
-
-def brier(y,p,scale=False):
-    r"""Calculate the brier score for given binary class labels and the according class probabilities.
-    
-        Parameters
-        ----------
-        y : array_like
-                Expected class labels given in test set. (Ground truth y)
-        p : array_like
-                Observed probabilities predicted by a classification model.
-                
-        Returns
-        -------
-        b : float
-            The Brier score for given data.
-        
-        Notes
-        -----
-        This score can be used for validation of classification models representing both, the discrimination and calibration
-        of the model. A low score is indicating good discrimination and calibration in context of given test data.
-        
-        Formula:
-
-        .. math::
-            B=\frac{1}{N} \sum_{i=1}^{N}\left(y_{i}-\hat{p}_{i}\right)^{2}
-
-        References
-        ----------
-        ..  [1] Huang, Y., Li, W., Macheret, F., Gabriel, R. A., & Ohno-Machado, L. (2020). 
-            A tutorial on calibration measurements and calibration models for clinical prediction models. 
-            Journal of the American Medical Informatics Association, 27(4), 621-633.
-            [2] Steyerberg, E. W., Vickers, A. J., Cook, N. R., Gerds, T., Gonen, M., Obuchowski, N., ... & Kattan, M. W. (2010). 
-            Assessing the performance of prediction models: a framework for some traditional and novel measures. 
-            Epidemiology (Cambridge, Mass.), 21(1), 128.
-        """
-    
-    brier_score = (np.square(y-p)).sum() / len(y)
+"""
+This module holds some metrics in context of calibration measurement of binary probabilistic classfication.
+"""
+
+import numpy as np
+
+
+def brier(y,p,scale=False):
+    r"""Calculate the brier score for given binary class labels and the according class probabilities.
+    
+        Parameters
+        ----------
+        y : array_like
+                Expected class labels given in test set. (Ground truth y)
+        p : array_like
+                Observed probabilities predicted by a classification model.
+                
+        Returns
+        -------
+        b : float
+            The Brier score for given data.
+        
+        Notes
+        -----
+        This score can be used for validation of classification models representing both, the discrimination and calibration
+        of the model. A low score is indicating good discrimination and calibration in context of given test data.
+        
+        Formula:
+
+        .. math::
+            B=\frac{1}{N} \sum_{i=1}^{N}\left(y_{i}-\hat{p}_{i}\right)^{2}
+
+        References
+        ----------
+        ..  [1] Huang, Y., Li, W., Macheret, F., Gabriel, R. A., & Ohno-Machado, L. (2020). 
+            A tutorial on calibration measurements and calibration models for clinical prediction models. 
+            Journal of the American Medical Informatics Association, 27(4), 621-633.
+            [2] Steyerberg, E. W., Vickers, A. J., Cook, N. R., Gerds, T., Gonen, M., Obuchowski, N., ... & Kattan, M. W. (2010). 
+            Assessing the performance of prediction models: a framework for some traditional and novel measures. 
+            Epidemiology (Cambridge, Mass.), 21(1), 128.
+        """
+    
+    brier_score = (np.square(y-p)).sum() / len(y)
     return (np.square(y-p)).sum() / len(y)
```

### Comparing `pycaleva-0.7.0/src/pycaleva.egg-info/PKG-INFO` & `pycaleva-0.8.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,174 +1,170 @@
-Metadata-Version: 2.1
-Name: pycaleva
-Version: 0.7.0
-Summary: A framework for calibration evaluation of binary classification models
-Home-page: https://github.com/MartinWeigl/pycaleva
-Author: Martin Weigl
-Author-email: martinweigl48@gmail.com
-Project-URL: Source, https://github.com/MartinWeigl/pycaleva
-Project-URL: Documentation, https://martinweigl.github.io/pycaleva/
-Keywords: calibration,classification,model,machine_learning,statistics
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![](https://martinweigl.github.io/pycaleva/assets/logo.svg)](https://martinweigl.github.io/pycaleva/)
-
-[Documentation]: https://martinweigl.github.io/pycaleva/
-
-### A framework for calibration evaluation of binary classification models. 
-- - -
-
-When performing classification tasks you sometimes want to obtain the probability of a class label instead of the class label itself. For example, it might be interesting to determine the risk of cancer for a patient. It is desireable to have a calibrated model which delivers predicted probabilities very close to the actual class membership probabilities. For this reason, this framework was developed allowing users to **measure the calibration of binary classification models**.
-
-- Evaluate the calibration of binary classification models with probabilistic output (LogisticRegression, SVM, NeuronalNets ...).  
-- Apply your model to testdata and use true class labels and predicted probabilities as input for the framework.  
-- Various statistical tests, metrics and plots are available.  
-- Supports creating a calibration report in pdf-format for your model.
-
-\
-<img src="https://martinweigl.github.io/pycaleva/assets/design.png" width="600" alt="Image Design">
-\
-\
-See the [documentation] for detailed information about classes and methods.
-
-
-
-Installation
-------------
-
-
-    $ pip install pycaleva
-
-or build on your own
-
-    $ git clone https://github.com/MartinWeigl/pycaleva.git
-    $ cd pycaleva
-    $ python setup.py install
-
-
-Requirements
-------------
-- numpy>=1.17
-- scipy>=1.3
-- matplotlib>=3.1
-- tqdm>=4.40
-- pandas>=1.3.0
-- statsmodels>=0.13.1
-- fpdf2>=2.5.0
-- ipython>=7.30.1
-
-
-Usage
------
-
-- Import and initialize  
-    ```python
-    from pycaleva import CalibrationEvaluator
-    ce = CalibrationEvaluator(y_test, pred_prob, outsample=True, n_groups='auto')
-    ```
-- Apply statistical tests
-    ```python
-    ce.hosmerlemeshow()     # Hosmer Lemeshow Test
-    ce.pigeonheyse()        # Pigeon Heyse Test
-    ce.z_test()             # Spiegelhalter z-Test
-    ce.calbelt(plot=False)  # Calibrationi Belt (Test only)
-    ```
-- Show calibration plot
-    ```python
-    ce.calibration_plot()
-    ```
-- Show calibration belt
-    ```python
-    ce.calbelt(plot=True)
-    ```
-- Get various metrics
-    ```python
-    ce.metrics()
-    ```
-- Create pdf calibration report
-    ```python
-    ce.calibration_report('report.pdf', 'my_model')
-    ```
-
-See  the [documentation] of single methods for detailed usage examples.
-
-Example Results
----------------
-| Well calibrated model | Poorly calibrated model |
-| :---: | :---: |
-| <img src="https://martinweigl.github.io/pycaleva/assets/calplot_well.png" width="65%" alt="Image Calibration plot well calibrated">  |  <img src="https://martinweigl.github.io/pycaleva/assets/calplot_poorly.png" width="65%" alt="Image Calibration plot poorly calibrated"> |
-| <img src="https://martinweigl.github.io/pycaleva/assets/calbelt_well.png" width="65%" alt="Image Calibration belt well calibrated">  |  <img src="https://martinweigl.github.io/pycaleva/assets/calbelt_poorly.png" width="65%" alt="Image Calibration belt well calibrated"> |
-| <pre lang="python">hltest_result(statistic=4.982635477424991, pvalue=0.8358193332183672, dof=9)</pre> | <pre lang="python">hltest_result(statistic=26.32792475118742, pvalue=0.0018051545107069522, dof=9)</pre> |
-| <pre lang="python">ztest_result(statistic=-0.21590257919669287, pvalue=0.829063686607032)</pre> | <pre lang="python">ztest_result(statistic=-3.196125145498827, pvalue=0.0013928668407116645)</pre> |
-
-
-Features
---------
-* Statistical tests for binary model calibration
-    * Hosmer Lemeshow Test
-    * Pigeon Heyse Test
-    * Spiegelhalter z-test
-    * Calibration belt
-* Graphical represantions showing calibration of binary models
-    * Calibration plot
-    * Calibration belt
-* Various Metrics
-    * Brier Score
-    * Adaptive Calibration Error
-    * Maximum Calibration Error
-    * Area within LOWESS Curve
-    * (AUROC)
-
-The above features are explained in more detail in PyCalEva's [documentation]
-
-
-References
-----------
-- **Statistical tests and metrics**:  
-
-    [1] Hosmer Jr, David W., Stanley Lemeshow, and Rodney X. Sturdivant.
-        Applied logistic regression. Vol. 398. John Wiley & Sons, 2013.
-
-    [2] Pigeon, Joseph G., and Joseph F. Heyse.
-        An improved goodness of fit statistic for probability prediction models.
-        Biometrical Journal: Journal of Mathematical Methods in Biosciences 41.1 (1999): 71-82.
-
-    [3] Spiegelhalter, D. J. (1986). Probabilistic prediction in patient management and clinical trials.
-        Statistics in medicine, 5(5), 421-433.
-
-    [4] Huang, Y., Li, W., Macheret, F., Gabriel, R. A., & Ohno-Machado, L. (2020).
-        A tutorial on calibration measurements and calibration models for clinical prediction models.
-        Journal of the American Medical Informatics Association, 27(4), 621-633.
-
-    
-- **Calibration plot**:  
-
-    [5] Jr, F. E. H. (2021). rms: Regression modeling strategies (R package version
-        6.2-0) [Computer software]. The Comprehensive R Archive Network.
-        Available from https://CRAN.R-project.org/package=rms
-
-- **Calibration belt**:  
-
-    [6] Nattino, G., Finazzi, S., & Bertolini, G. (2014). A new calibration test 
-        and a reappraisal of the calibration belt for the assessment of prediction models 
-        based on dichotomous outcomes. Statistics in medicine, 33(14), 2390-2407.
-
-    [7] Bulgarelli, L. (2021). calibrattion-belt: Assessment of calibration in binomial prediction models [Computer software].
-        Available from https://github.com/fabiankueppers/calibration-framework
-
-    [8] Nattino, G., Finazzi, S., Bertolini, G., Rossi, C., & Carrara, G. (2017).
-        givitiR: The giviti calibration test and belt (R package version 1.3) [Computer
-        software]. The Comprehensive R Archive Network.
-        Available from https://CRAN.R-project.org/package=givitiR
-
-- **Others**:  
-
-    [9] Sturges, H. A. (1926). The choice of a class interval. 
-        Journal of the american statistical association, 21(153), 65-66.
-
-For most of the implemented methods in this software you can find references in the [documentation] as well.
+Metadata-Version: 2.1
+Name: pycaleva
+Version: 0.8.0
+Summary: A framework for calibration evaluation of binary classification models
+Home-page: https://github.com/MartinWeigl/pycaleva
+Author: Martin Weigl
+Author-email: martinweigl48@gmail.com
+License: UNKNOWN
+Project-URL: Source, https://github.com/MartinWeigl/pycaleva
+Project-URL: Documentation, https://martinweigl.github.io/pycaleva/
+Keywords: calibration,classification,model,machine_learning,statistics
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![](https://martinweigl.github.io/pycaleva/assets/logo.svg)](https://martinweigl.github.io/pycaleva/)
+
+[Documentation]: https://martinweigl.github.io/pycaleva/
+
+### A framework for calibration evaluation of binary classification models.
+
+---
+
+When performing classification tasks you sometimes want to obtain the probability of a class label instead of the class label itself. For example, it might be interesting to determine the risk of cancer for a patient. It is desireable to have a calibrated model which delivers predicted probabilities very close to the actual class membership probabilities. For this reason, this framework was developed allowing users to **measure the calibration of binary classification models**.
+
+- Evaluate the calibration of binary classification models with probabilistic output (LogisticRegression, SVM, NeuronalNets ...).
+- Apply your model to testdata and use true class labels and predicted probabilities as input for the framework.
+- Various statistical tests, metrics and plots are available.
+- Supports creating a calibration report in pdf-format for your model.
+
+\
+<img src="https://martinweigl.github.io/pycaleva/assets/design.png" width="600" alt="Image Design">
+\
+\
+See the [documentation] for detailed information about classes and methods.
+
+## Installation
+
+    $ pip install pycaleva
+
+or build on your own
+
+    $ git clone https://github.com/MartinWeigl/pycaleva.git
+    $ cd pycaleva
+    $ python setup.py install
+
+## Requirements
+
+- numpy>=1.26
+- scipy>=1.13
+- scikit-learn>=1.4
+- matplotlib>=3.8
+- tqdm>=4.66
+- pandas>=2.2
+- statsmodels>=0.14
+- fpdf2>=2.7
+- ipython>=8.24
+
+## Usage
+
+- Import and initialize
+  ```python
+  from pycaleva import CalibrationEvaluator
+  ce = CalibrationEvaluator(y_test, pred_prob, outsample=True, n_groups='auto')
+  ```
+- Apply statistical tests
+  ```python
+  ce.hosmerlemeshow()     # Hosmer Lemeshow Test
+  ce.pigeonheyse()        # Pigeon Heyse Test
+  ce.z_test()             # Spiegelhalter z-Test
+  ce.calbelt(plot=False)  # Calibrationi Belt (Test only)
+  ```
+- Show calibration plot
+  ```python
+  ce.calibration_plot()
+  ```
+- Show calibration belt
+  ```python
+  ce.calbelt(plot=True)
+  ```
+- Get various metrics
+  ```python
+  ce.metrics()
+  ```
+- Create pdf calibration report
+  ```python
+  ce.calibration_report('report.pdf', 'my_model')
+  ```
+
+See the [documentation] of single methods for detailed usage examples.
+
+## Example Results
+
+|                                                        Well calibrated model                                                        |                                                         Poorly calibrated model                                                         |
+| :---------------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------------: |
+| <img src="https://martinweigl.github.io/pycaleva/assets/calplot_well.png" width="65%" alt="Image Calibration plot well calibrated"> | <img src="https://martinweigl.github.io/pycaleva/assets/calplot_poorly.png" width="65%" alt="Image Calibration plot poorly calibrated"> |
+| <img src="https://martinweigl.github.io/pycaleva/assets/calbelt_well.png" width="65%" alt="Image Calibration belt well calibrated"> |  <img src="https://martinweigl.github.io/pycaleva/assets/calbelt_poorly.png" width="65%" alt="Image Calibration belt well calibrated">  |
+|                <pre lang="python">hltest_result(statistic=4.982635477424991, pvalue=0.8358193332183672, dof=9)</pre>                |                <pre lang="python">hltest_result(statistic=26.32792475118742, pvalue=0.0018051545107069522, dof=9)</pre>                 |
+|                   <pre lang="python">ztest_result(statistic=-0.21590257919669287, pvalue=0.829063686607032)</pre>                   |                    <pre lang="python">ztest_result(statistic=-3.196125145498827, pvalue=0.0013928668407116645)</pre>                    |
+
+## Features
+
+- Statistical tests for binary model calibration
+  - Hosmer Lemeshow Test
+  - Pigeon Heyse Test
+  - Spiegelhalter z-test
+  - Calibration belt
+- Graphical represantions showing calibration of binary models
+  - Calibration plot
+  - Calibration belt
+- Various Metrics
+  - Brier Score
+  - Adaptive Calibration Error
+  - Maximum Calibration Error
+  - Area within LOWESS Curve
+  - (AUROC)
+
+The above features are explained in more detail in PyCalEva's [documentation]
+
+## References
+
+- **Statistical tests and metrics**:
+
+  [1] Hosmer Jr, David W., Stanley Lemeshow, and Rodney X. Sturdivant.
+  Applied logistic regression. Vol. 398. John Wiley & Sons, 2013.
+
+  [2] Pigeon, Joseph G., and Joseph F. Heyse.
+  An improved goodness of fit statistic for probability prediction models.
+  Biometrical Journal: Journal of Mathematical Methods in Biosciences 41.1 (1999): 71-82.
+
+  [3] Spiegelhalter, D. J. (1986). Probabilistic prediction in patient management and clinical trials.
+  Statistics in medicine, 5(5), 421-433.
+
+  [4] Huang, Y., Li, W., Macheret, F., Gabriel, R. A., & Ohno-Machado, L. (2020).
+  A tutorial on calibration measurements and calibration models for clinical prediction models.
+  Journal of the American Medical Informatics Association, 27(4), 621-633.
+
+- **Calibration plot**:
+
+  [5] Jr, F. E. H. (2021). rms: Regression modeling strategies (R package version
+  6.2-0) [Computer software]. The Comprehensive R Archive Network.
+  Available from https://CRAN.R-project.org/package=rms
+
+- **Calibration belt**:
+
+  [6] Nattino, G., Finazzi, S., & Bertolini, G. (2014). A new calibration test
+  and a reappraisal of the calibration belt for the assessment of prediction models
+  based on dichotomous outcomes. Statistics in medicine, 33(14), 2390-2407.
+
+  [7] Bulgarelli, L. (2021). calibrattion-belt: Assessment of calibration in binomial prediction models [Computer software].
+  Available from https://github.com/fabiankueppers/calibration-framework
+
+  [8] Nattino, G., Finazzi, S., Bertolini, G., Rossi, C., & Carrara, G. (2017).
+  givitiR: The giviti calibration test and belt (R package version 1.3) [Computer
+  software]. The Comprehensive R Archive Network.
+  Available from https://CRAN.R-project.org/package=givitiR
+
+- **Others**:
+
+  [9] Sturges, H. A. (1926). The choice of a class interval.
+  Journal of the american statistical association, 21(153), 65-66.
+
+For most of the implemented methods in this software you can find references in the [documentation] as well.
+
+
```


# Comparing `tmp/scientistmetrics-0.0.3.tar.gz` & `tmp/scientistmetrics-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scientistmetrics-0.0.3.tar", last modified: Sun Sep 17 16:18:23 2023, max compression
+gzip compressed data, was "scientistmetrics-0.0.4.tar", last modified: Wed May  1 17:25:25 2024, max compression
```

## Comparing `scientistmetrics-0.0.3.tar` & `scientistmetrics-0.0.4.tar`

### file list

```diff
@@ -1,40 +1,105 @@
-drwxrwxrwx   0        0        0        0 2023-09-17 16:18:23.904148 scientistmetrics-0.0.3/
--rw-rw-rw-   0        0        0       44 2023-08-24 21:26:38.000000 scientistmetrics-0.0.3/.gitignore
--rw-rw-rw-   0        0        0     1094 2023-07-08 15:34:40.000000 scientistmetrics-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1684 2023-09-17 16:18:23.904148 scientistmetrics-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1111 2023-07-08 15:54:04.000000 scientistmetrics-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-09-17 16:18:23.869386 scientistmetrics-0.0.3/data/
--rw-rw-rw-   0        0        0   333442 2023-08-08 23:12:54.000000 scientistmetrics-0.0.3/data/Life Expectancy Data.csv
--rw-rw-rw-   0        0        0    23873 2023-08-08 18:36:34.000000 scientistmetrics-0.0.3/data/diabetes.csv
--rw-rw-rw-   0        0        0    55628 2023-08-08 22:58:43.000000 scientistmetrics-0.0.3/data/insurance.csv
--rw-rw-rw-   0        0        0  2616832 2023-06-25 15:56:46.000000 scientistmetrics-0.0.3/data/mushroom.xls
-drwxrwxrwx   0        0        0        0 2023-09-17 16:18:23.883430 scientistmetrics-0.0.3/notebooks/
--rw-rw-rw-   0        0        0    17340 2023-08-25 06:22:35.000000 scientistmetrics-0.0.3/notebooks/model.ipynb
--rw-rw-rw-   0        0        0   683169 2023-07-08 16:03:25.000000 scientistmetrics-0.0.3/notebooks/scientistmetrics.ipynb
--rw-rw-rw-   0        0        0   429540 2023-09-17 16:13:06.000000 scientistmetrics-0.0.3/performance.ipynb
-drwxrwxrwx   0        0        0        0 2023-09-17 16:18:23.888434 scientistmetrics-0.0.3/scientistmetrics/
--rw-rw-rw-   0        0        0     1258 2023-09-17 16:14:17.000000 scientistmetrics-0.0.3/scientistmetrics/__init__.py
--rw-rw-rw-   0        0        0     6547 2023-07-08 15:49:11.000000 scientistmetrics-0.0.3/scientistmetrics/association.py
--rw-rw-rw-   0        0        0    79812 2023-09-17 16:11:46.000000 scientistmetrics-0.0.3/scientistmetrics/performance.py
--rw-rw-rw-   0        0        0    11220 2023-08-24 21:04:05.000000 scientistmetrics-0.0.3/scientistmetrics/powerset.py
-drwxrwxrwx   0        0        0        0 2023-09-17 16:18:23.890433 scientistmetrics-0.0.3/scientistmetrics.egg-info/
--rw-rw-rw-   0        0        0     1684 2023-09-17 16:18:23.000000 scientistmetrics-0.0.3/scientistmetrics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      875 2023-09-17 16:18:23.000000 scientistmetrics-0.0.3/scientistmetrics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-17 16:18:23.000000 scientistmetrics-0.0.3/scientistmetrics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-09-17 16:18:23.000000 scientistmetrics-0.0.3/scientistmetrics.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-09-17 16:18:23.900144 scientistmetrics-0.0.3/scientistmetricsdoc/
--rw-rw-rw-   0        0        0        0 2023-08-24 21:28:36.000000 scientistmetrics-0.0.3/scientistmetricsdoc/chapter1.Rmd
--rw-rw-rw-   0        0        0     2717 2023-08-24 22:25:55.000000 scientistmetrics-0.0.3/scientistmetricsdoc/chapter2.Rmd
-drwxrwxrwx   0        0        0        0 2023-09-17 16:18:23.902151 scientistmetrics-0.0.3/scientistmetricsdoc/donnee/
--rw-rw-rw-   0        0        0    23873 2023-08-08 18:36:34.000000 scientistmetrics-0.0.3/scientistmetricsdoc/donnee/diabetes.csv
--rw-rw-rw-   0        0        0    55628 2023-08-08 22:58:43.000000 scientistmetrics-0.0.3/scientistmetricsdoc/donnee/insurance.csv
--rw-rw-rw-   0        0        0     5639 2023-08-24 21:31:20.000000 scientistmetrics-0.0.3/scientistmetricsdoc/main.Rmd
--rw-rw-rw-   0        0        0    75639 2023-08-24 22:26:16.000000 scientistmetrics-0.0.3/scientistmetricsdoc/main.log
--rw-rw-rw-   0        0        0       29 2023-08-24 22:26:16.000000 scientistmetrics-0.0.3/scientistmetricsdoc/main.maf
--rw-rw-rw-   0        0        0        0 2023-08-24 22:26:13.000000 scientistmetrics-0.0.3/scientistmetricsdoc/main.mtc
--rw-rw-rw-   0        0        0        0 2023-08-24 22:26:13.000000 scientistmetrics-0.0.3/scientistmetricsdoc/main.mtc0
--rw-rw-rw-   0        0        0      501 2023-08-24 22:26:15.000000 scientistmetrics-0.0.3/scientistmetricsdoc/main.mtc1
--rw-rw-rw-   0        0        0    57915 2023-08-24 22:26:16.000000 scientistmetrics-0.0.3/scientistmetricsdoc/main.pdf
--rw-rw-rw-   0        0        0      216 2023-08-24 21:26:37.000000 scientistmetrics-0.0.3/scientistmetricsdoc/scientistmetricsdoc.Rproj
--rw-rw-rw-   0        0        0       42 2023-09-17 16:18:23.904148 scientistmetrics-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      835 2023-09-17 16:17:45.000000 scientistmetrics-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 17:25:25.267658 scientistmetrics-0.0.4/
+-rw-rw-rw-   0        0        0       44 2023-08-24 21:26:38.000000 scientistmetrics-0.0.4/.gitignore
+-rw-rw-rw-   0        0        0     1094 2023-07-08 15:34:40.000000 scientistmetrics-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2752 2024-05-01 17:25:25.265626 scientistmetrics-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2023 2024-05-01 17:23:23.000000 scientistmetrics-0.0.4/README.md
+-rw-rw-rw-   0        0        0   174199 2024-05-01 16:50:19.000000 scientistmetrics-0.0.4/association.ipynb
+drwxrwxrwx   0        0        0        0 2024-05-01 17:25:25.117666 scientistmetrics-0.0.4/data/
+-rw-rw-rw-   0        0        0   333442 2023-08-08 23:12:54.000000 scientistmetrics-0.0.4/data/Life Expectancy Data.csv
+-rw-rw-rw-   0        0        0    23873 2023-08-08 18:36:34.000000 scientistmetrics-0.0.4/data/diabetes.csv
+-rw-rw-rw-   0        0        0    55628 2023-08-08 22:58:43.000000 scientistmetrics-0.0.4/data/insurance.csv
+-rw-rw-rw-   0        0        0  2616832 2023-06-25 15:56:46.000000 scientistmetrics-0.0.4/data/mushroom.xls
+-rw-rw-rw-   0        0        0      958 2024-04-30 19:14:39.000000 scientistmetrics-0.0.4/data/vehicules_1.txt
+-rw-rw-rw-   0        0        0      263 2024-04-30 19:14:39.000000 scientistmetrics-0.0.4/data/vehicules_2.txt
+-rw-rw-rw-   0        0        0   259020 2024-05-01 16:11:11.000000 scientistmetrics-0.0.4/lm_metrics.ipynb
+-rw-rw-rw-   0        0        0    64512 2024-05-01 16:12:43.000000 scientistmetrics-0.0.4/logit_metrics.ipynb
+-rw-rw-rw-   0        0        0   429852 2024-03-24 20:02:52.000000 scientistmetrics-0.0.4/performance.ipynb
+-rw-rw-rw-   0        0        0    17099 2024-05-01 16:50:10.000000 scientistmetrics-0.0.4/powerset_model.ipynb
+drwxrwxrwx   0        0        0        0 2024-05-01 17:25:25.232562 scientistmetrics-0.0.4/scientistmetrics/
+-rw-rw-rw-   0        0        0     2497 2024-05-01 09:27:02.000000 scientistmetrics-0.0.4/scientistmetrics/__init__.py
+-rw-rw-rw-   0        0        0     1471 2024-05-01 15:27:15.000000 scientistmetrics-0.0.4/scientistmetrics/accuracy_score.py
+-rw-rw-rw-   0        0        0     3327 2024-05-01 16:28:39.000000 scientistmetrics-0.0.4/scientistmetrics/association.py
+-rw-rw-rw-   0        0        0     1287 2024-05-01 15:26:31.000000 scientistmetrics-0.0.4/scientistmetrics/average_precision_score.py
+-rw-rw-rw-   0        0        0     1491 2024-05-01 15:30:35.000000 scientistmetrics-0.0.4/scientistmetrics/balanced_accuracy_score.py
+-rw-rw-rw-   0        0        0     1186 2024-05-01 15:43:43.000000 scientistmetrics-0.0.4/scientistmetrics/brier_score_loss.py
+-rw-rw-rw-   0        0        0     2924 2024-05-01 15:31:57.000000 scientistmetrics-0.0.4/scientistmetrics/check_autocorrelation.py
+-rw-rw-rw-   0        0        0     2711 2024-05-01 15:31:44.000000 scientistmetrics-0.0.4/scientistmetrics/check_heteroscedasticity.py
+-rw-rw-rw-   0        0        0     2099 2024-05-01 15:32:06.000000 scientistmetrics-0.0.4/scientistmetrics/check_kmo.py
+-rw-rw-rw-   0        0        0     2829 2024-05-01 15:32:18.000000 scientistmetrics-0.0.4/scientistmetrics/check_model.py
+-rw-rw-rw-   0        0        0     2682 2024-05-01 15:33:39.000000 scientistmetrics-0.0.4/scientistmetrics/check_normality.py
+-rw-rw-rw-   0        0        0     2528 2024-05-01 15:34:11.000000 scientistmetrics-0.0.4/scientistmetrics/check_overdispersion.py
+-rw-rw-rw-   0        0        0     2575 2024-05-01 15:34:43.000000 scientistmetrics-0.0.4/scientistmetrics/check_spericity_bartlett.py
+-rw-rw-rw-   0        0        0     1362 2024-05-01 15:34:36.000000 scientistmetrics-0.0.4/scientistmetrics/check_symetric.py
+-rw-rw-rw-   0        0        0      692 2024-05-01 15:34:50.000000 scientistmetrics-0.0.4/scientistmetrics/coefficients.py
+-rw-rw-rw-   0        0        0     3219 2024-05-01 15:36:19.000000 scientistmetrics-0.0.4/scientistmetrics/compare_performance.py
+-rw-rw-rw-   0        0        0      462 2024-05-01 15:05:51.000000 scientistmetrics-0.0.4/scientistmetrics/diff.py
+-rw-rw-rw-   0        0        0      619 2024-05-01 15:06:06.000000 scientistmetrics-0.0.4/scientistmetrics/efron_rsquare.py
+-rw-rw-rw-   0        0        0      965 2024-05-01 15:06:19.000000 scientistmetrics-0.0.4/scientistmetrics/error_rate.py
+-rw-rw-rw-   0        0        0     1065 2024-05-01 15:38:10.000000 scientistmetrics-0.0.4/scientistmetrics/explained_variance_score.py
+-rw-rw-rw-   0        0        0      372 2024-05-01 15:06:38.000000 scientistmetrics-0.0.4/scientistmetrics/extractAIC.py
+-rw-rw-rw-   0        0        0      643 2024-05-01 15:06:49.000000 scientistmetrics-0.0.4/scientistmetrics/extractAICC.py
+-rw-rw-rw-   0        0        0      376 2024-05-01 15:06:58.000000 scientistmetrics-0.0.4/scientistmetrics/extractBIC.py
+-rw-rw-rw-   0        0        0     1403 2024-05-01 15:39:59.000000 scientistmetrics-0.0.4/scientistmetrics/f1_score.py
+-rw-rw-rw-   0        0        0     1862 2024-05-01 15:41:12.000000 scientistmetrics-0.0.4/scientistmetrics/ggroc.py
+-rw-rw-rw-   0        0        0     2864 2024-05-01 15:44:52.000000 scientistmetrics-0.0.4/scientistmetrics/hosmerlemeshowtest.py
+-rw-rw-rw-   0        0        0      891 2024-05-01 15:08:37.000000 scientistmetrics-0.0.4/scientistmetrics/lag.py
+-rw-rw-rw-   0        0        0     4182 2024-05-01 15:08:53.000000 scientistmetrics-0.0.4/scientistmetrics/likelihoodratiotest.py
+-rw-rw-rw-   0        0        0      422 2024-05-01 15:09:10.000000 scientistmetrics-0.0.4/scientistmetrics/logLik.py
+-rw-rw-rw-   0        0        0     1458 2024-05-01 15:47:27.000000 scientistmetrics-0.0.4/scientistmetrics/log_loss.py
+-rw-rw-rw-   0        0        0     1190 2024-05-01 15:48:35.000000 scientistmetrics-0.0.4/scientistmetrics/mae.py
+-rw-rw-rw-   0        0        0     2035 2024-05-01 15:50:48.000000 scientistmetrics-0.0.4/scientistmetrics/mannwhitneytest.py
+-rw-rw-rw-   0        0        0     1235 2024-05-01 15:51:35.000000 scientistmetrics-0.0.4/scientistmetrics/mape.py
+-rw-rw-rw-   0        0        0     1168 2024-05-01 15:52:14.000000 scientistmetrics-0.0.4/scientistmetrics/max_error.py
+-rw-rw-rw-   0        0        0     1211 2024-05-01 15:53:55.000000 scientistmetrics-0.0.4/scientistmetrics/mdae.py
+-rw-rw-rw-   0        0        0     1481 2024-05-01 15:55:14.000000 scientistmetrics-0.0.4/scientistmetrics/mdape.py
+-rw-rw-rw-   0        0        0     3204 2024-05-01 15:55:35.000000 scientistmetrics-0.0.4/scientistmetrics/model_performance.py
+-rw-rw-rw-   0        0        0     1536 2024-05-01 15:56:38.000000 scientistmetrics-0.0.4/scientistmetrics/mse.py
+-rw-rw-rw-   0        0        0     1512 2024-05-01 15:57:48.000000 scientistmetrics-0.0.4/scientistmetrics/multiclass_roc.py
+-rw-rw-rw-   0        0        0     3355 2024-04-28 15:50:39.000000 scientistmetrics-0.0.4/scientistmetrics/performance.py
+-rw-rw-rw-   0        0        0    11883 2024-05-01 16:12:07.000000 scientistmetrics-0.0.4/scientistmetrics/powerset.py
+-rw-rw-rw-   0        0        0     1423 2024-05-01 16:01:28.000000 scientistmetrics-0.0.4/scientistmetrics/precision_score.py
+-rw-rw-rw-   0        0        0     1289 2024-05-01 15:17:29.000000 scientistmetrics-0.0.4/scientistmetrics/r2.py
+-rw-rw-rw-   0        0        0     1377 2024-05-01 16:03:09.000000 scientistmetrics-0.0.4/scientistmetrics/r2_count.py
+-rw-rw-rw-   0        0        0     1564 2024-05-01 16:02:26.000000 scientistmetrics-0.0.4/scientistmetrics/r2_count_adj.py
+-rw-rw-rw-   0        0        0      439 2024-05-01 16:03:26.000000 scientistmetrics-0.0.4/scientistmetrics/r2_coxsnell.py
+-rw-rw-rw-   0        0        0     1036 2024-05-01 16:04:09.000000 scientistmetrics-0.0.4/scientistmetrics/r2_efron.py
+-rw-rw-rw-   0        0        0     1090 2024-05-01 15:13:46.000000 scientistmetrics-0.0.4/scientistmetrics/r2_kullback.py
+-rw-rw-rw-   0        0        0     1140 2024-05-01 15:14:02.000000 scientistmetrics-0.0.4/scientistmetrics/r2_mcfadden.py
+-rw-rw-rw-   0        0        0      622 2024-05-01 16:05:04.000000 scientistmetrics-0.0.4/scientistmetrics/r2_mckelvey.py
+-rw-rw-rw-   0        0        0      572 2024-05-01 15:14:49.000000 scientistmetrics-0.0.4/scientistmetrics/r2_nagelkerke.py
+-rw-rw-rw-   0        0        0     1497 2024-05-01 16:05:39.000000 scientistmetrics-0.0.4/scientistmetrics/r2_score.py
+-rw-rw-rw-   0        0        0      846 2024-05-01 16:05:52.000000 scientistmetrics-0.0.4/scientistmetrics/r2_somers.py
+-rw-rw-rw-   0        0        0     1076 2024-05-01 15:15:48.000000 scientistmetrics-0.0.4/scientistmetrics/r2_tjur.py
+-rw-rw-rw-   0        0        0      786 2024-05-01 16:06:07.000000 scientistmetrics-0.0.4/scientistmetrics/r2_xu.py
+-rw-rw-rw-   0        0        0     1420 2024-05-01 16:07:46.000000 scientistmetrics-0.0.4/scientistmetrics/recall_score.py
+-rw-rw-rw-   0        0        0     2188 2024-05-01 15:19:34.000000 scientistmetrics-0.0.4/scientistmetrics/residuals.py
+-rw-rw-rw-   0        0        0     1929 2024-05-01 16:09:02.000000 scientistmetrics-0.0.4/scientistmetrics/rmse.py
+-rw-rw-rw-   0        0        0     1303 2024-05-01 16:10:17.000000 scientistmetrics-0.0.4/scientistmetrics/roc_auc_score.py
+-rw-rw-rw-   0        0        0     2055 2024-05-01 15:20:45.000000 scientistmetrics-0.0.4/scientistmetrics/rstandard.py
+-rw-rw-rw-   0        0        0     1395 2024-05-01 16:10:37.000000 scientistmetrics-0.0.4/scientistmetrics/rstudent.py
+drwxrwxrwx   0        0        0        0 2024-05-01 17:25:25.264336 scientistmetrics-0.0.4/scientistmetrics.egg-info/
+-rw-rw-rw-   0        0        0     2752 2024-05-01 17:25:24.000000 scientistmetrics-0.0.4/scientistmetrics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2935 2024-05-01 17:25:24.000000 scientistmetrics-0.0.4/scientistmetrics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 17:25:24.000000 scientistmetrics-0.0.4/scientistmetrics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2024-05-01 17:25:24.000000 scientistmetrics-0.0.4/scientistmetrics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-01 17:25:24.000000 scientistmetrics-0.0.4/scientistmetrics.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 17:25:25.259405 scientistmetrics-0.0.4/scientistmetricsdoc/
+-rw-rw-rw-   0        0        0        0 2023-08-24 21:28:36.000000 scientistmetrics-0.0.4/scientistmetricsdoc/chapter1.Rmd
+-rw-rw-rw-   0        0        0     2717 2023-08-24 22:25:55.000000 scientistmetrics-0.0.4/scientistmetricsdoc/chapter2.Rmd
+-rw-rw-rw-   0        0        0     7696 2023-09-17 18:16:41.000000 scientistmetrics-0.0.4/scientistmetricsdoc/chapter3.Rmd
+-rw-rw-rw-   0        0        0    21306 2024-04-28 14:54:52.000000 scientistmetrics-0.0.4/scientistmetricsdoc/chapter4.Rmd
+drwxrwxrwx   0        0        0        0 2024-05-01 17:25:25.261141 scientistmetrics-0.0.4/scientistmetricsdoc/donnee/
+-rw-rw-rw-   0        0        0    23873 2023-08-08 18:36:34.000000 scientistmetrics-0.0.4/scientistmetricsdoc/donnee/diabetes.csv
+-rw-rw-rw-   0        0        0    55628 2023-08-08 22:58:43.000000 scientistmetrics-0.0.4/scientistmetricsdoc/donnee/insurance.csv
+drwxrwxrwx   0        0        0        0 2024-05-01 17:25:25.263331 scientistmetrics-0.0.4/scientistmetricsdoc/images/
+-rw-rw-rw-   0        0        0    23108 2023-09-19 16:50:50.000000 scientistmetrics-0.0.4/scientistmetricsdoc/images/cm-matrix.png
+-rw-rw-rw-   0        0        0     5697 2023-09-19 13:31:01.000000 scientistmetrics-0.0.4/scientistmetricsdoc/main.Rmd
+-rw-rw-rw-   0        0        0    83535 2024-04-28 14:55:18.000000 scientistmetrics-0.0.4/scientistmetricsdoc/main.log
+-rw-rw-rw-   0        0        0       29 2024-04-28 14:55:17.000000 scientistmetrics-0.0.4/scientistmetricsdoc/main.maf
+-rw-rw-rw-   0        0        0        0 2024-04-28 14:55:17.000000 scientistmetrics-0.0.4/scientistmetricsdoc/main.mtc
+-rw-rw-rw-   0        0        0        0 2024-04-28 14:55:16.000000 scientistmetrics-0.0.4/scientistmetricsdoc/main.mtc0
+-rw-rw-rw-   0        0        0     5686 2024-04-28 14:55:17.000000 scientistmetrics-0.0.4/scientistmetricsdoc/main.mtc1
+-rw-rw-rw-   0        0        0   151930 2024-04-28 14:55:18.000000 scientistmetrics-0.0.4/scientistmetricsdoc/main.pdf
+-rw-rw-rw-   0        0        0      216 2024-04-28 14:09:59.000000 scientistmetrics-0.0.4/scientistmetricsdoc/scientistmetricsdoc.Rproj
+-rw-rw-rw-   0        0        0       42 2024-05-01 17:25:25.267658 scientistmetrics-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1085 2024-05-01 17:24:38.000000 scientistmetrics-0.0.4/setup.py
```

### Comparing `scientistmetrics-0.0.3/LICENSE` & `scientistmetrics-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scientistmetrics-0.0.3/PKG-INFO` & `scientistmetrics-0.0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,91 @@
 Metadata-Version: 2.1
 Name: scientistmetrics
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python package for metrics and scoring : quantifying the quality of predictions
 Home-page: https://github.com/enfantbenidedieu/scientistmetrics
 Author: Duverier DJIFACK ZEBAZE
 Author-email: duverierdjifack@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: pandas>=2.2.2
+Requires-Dist: scikit-learn>=1.2.2
+Requires-Dist: plotnine>=0.10.1
+Requires-Dist: statsmodels>=0.14.0
+Requires-Dist: scipy>=1.10.1
 
-# scientistmetrics
+# scientistmetrics : python library for model metrics
 
 ## About scientistmetrics
 
-**scientistmetrics** is a `Python` package for calculating correlation amongst categorical variables.
+scientistmetrics is a Python package for metrics and scoring : quantifying the quality of predictions
 
 ## Why scientistmetrics?
 
-The function provides the option for computing one of six measures of association between two nominal variables from the data given in a 2d contingency table: 
-* Pearson's chi-squared test : https://en.wikipedia.org/wiki/Pearson%27s_chi-squared_test
-* Phi coefficient : https://en.wikipedia.org/wiki/Phi_coefficient
-* G-test: https://en.wikipedia.org/wiki/G-test
-* Cramer's V : https://en.wikipedia.org/wiki/Cramer's_V
-* Tschuprow's T : https://en.wikipedia.org/wiki/Tschuprow's_T
-* Pearson contingency coefficient : https://www.statisticshowto.com/contingency-coefficient/
+### Measure of association with categoricals variables
+
+scientistmetrics provides the option for computing one of six measures of association between two nominal variables from the data given in a 2d contingency table:
+
+* Chi - squard test : [https://en.wikipedia.org/wiki/Chi-squared_test](https://en.wikipedia.org/wiki/Chi-squared_test)
+* Cramer's V : [https://en.wikipedia.org/wiki/Cram%C3%A9r%27s_V](https://en.wikipedia.org/wiki/Cram%C3%A9r%27s_V)
+* Tschuprow's T : [https://en.wikipedia.org/wiki/Tschuprow%27s_T](https://en.wikipedia.org/wiki/Tschuprow%27s_T)
+* G-test : [https://en.wikipedia.org/wiki/G-test](https://en.wikipedia.org/wiki/G-test)
+* Phi coefficient : [https://en.wikipedia.org/wiki/Phi_coefficient](https://en.wikipedia.org/wiki/Phi_coefficient)
+* Pearson contingence coefficient : [https://www.statisticshowto.com/contingency-coefficient/](https://www.statisticshowto.com/contingency-coefficient/)
+
+### Classification metrics
+
+scientistmetrics provides metrics for classification problem :
+
+* accuracy score
+* f1 score
+* precision
+* recall
+* etc...
+
+### Regression metrics
+
+scientistmetrics provides metrics for regression problem :
+
+* Rsquared
+* Adjusted Rsquared
+* Mean squared error
+* etc...
+
+### Powerset model
+
+scientistmetrics provides a function that gives a set of all subsets model.
 
 Notebook is availabled.
 
 ## Installation
 
 ### Dependencies
 
 scientistmetrics requires :
 
 ```
-Python >=3.10
-Numpy >=1.23.5
-Pandas >=1.5.3
-Plotnine >=0.10.1
-Scipy >=1.10.1
+python >=3.10
+numpy >=1.26.4
+pandas >=2.2.2
+scikit-learn >=1.2.2
+plotnine >=0.10.1
+statsmodels >=0.14.0
+scipy >=1.10.1
 ```
 
 ## User installation
 
 You can install scientistmetrics using `pip` :
 
 ```
 pip install scientistmetrics
 ```
 
-## Author
-
-Duvérier DJIFACK ZEBAZE
+## Author(s)
 
+Duvérier DJIFACK ZEBAZE [duverierdjifack@gmail.com](mailto:duverierdjifack@gmail.com)
```

### Comparing `scientistmetrics-0.0.3/README.md` & `scientistmetrics-0.0.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,71 @@
-# scientistmetrics
+# scientistmetrics : python library for model metrics
 
 ## About scientistmetrics
 
-**scientistmetrics** is a `Python` package for calculating correlation amongst categorical variables.
+scientistmetrics is a Python package for metrics and scoring : quantifying the quality of predictions
 
 ## Why scientistmetrics?
 
-The function provides the option for computing one of six measures of association between two nominal variables from the data given in a 2d contingency table: 
-* Pearson's chi-squared test : https://en.wikipedia.org/wiki/Pearson%27s_chi-squared_test
-* Phi coefficient : https://en.wikipedia.org/wiki/Phi_coefficient
-* G-test: https://en.wikipedia.org/wiki/G-test
-* Cramer's V : https://en.wikipedia.org/wiki/Cramer's_V
-* Tschuprow's T : https://en.wikipedia.org/wiki/Tschuprow's_T
-* Pearson contingency coefficient : https://www.statisticshowto.com/contingency-coefficient/
+### Measure of association with categoricals variables
+
+scientistmetrics provides the option for computing one of six measures of association between two nominal variables from the data given in a 2d contingency table:
+
+* Chi - squard test : [https://en.wikipedia.org/wiki/Chi-squared_test](https://en.wikipedia.org/wiki/Chi-squared_test)
+* Cramer's V : [https://en.wikipedia.org/wiki/Cram%C3%A9r%27s_V](https://en.wikipedia.org/wiki/Cram%C3%A9r%27s_V)
+* Tschuprow's T : [https://en.wikipedia.org/wiki/Tschuprow%27s_T](https://en.wikipedia.org/wiki/Tschuprow%27s_T)
+* G-test : [https://en.wikipedia.org/wiki/G-test](https://en.wikipedia.org/wiki/G-test)
+* Phi coefficient : [https://en.wikipedia.org/wiki/Phi_coefficient](https://en.wikipedia.org/wiki/Phi_coefficient)
+* Pearson contingence coefficient : [https://www.statisticshowto.com/contingency-coefficient/](https://www.statisticshowto.com/contingency-coefficient/)
+
+### Classification metrics
+
+scientistmetrics provides metrics for classification problem :
+
+* accuracy score
+* f1 score
+* precision
+* recall
+* etc...
+
+### Regression metrics
+
+scientistmetrics provides metrics for regression problem :
+
+* Rsquared
+* Adjusted Rsquared
+* Mean squared error
+* etc...
+
+### Powerset model
+
+scientistmetrics provides a function that gives a set of all subsets model.
 
 Notebook is availabled.
 
 ## Installation
 
 ### Dependencies
 
 scientistmetrics requires :
 
 ```
-Python >=3.10
-Numpy >=1.23.5
-Pandas >=1.5.3
-Plotnine >=0.10.1
-Scipy >=1.10.1
+python >=3.10
+numpy >=1.26.4
+pandas >=2.2.2
+scikit-learn >=1.2.2
+plotnine >=0.10.1
+statsmodels >=0.14.0
+scipy >=1.10.1
 ```
 
 ## User installation
 
 You can install scientistmetrics using `pip` :
 
 ```
 pip install scientistmetrics
 ```
 
-## Author
+## Author(s)
 
-Duvérier DJIFACK ZEBAZE
+Duvérier DJIFACK ZEBAZE [duverierdjifack@gmail.com](mailto:duverierdjifack@gmail.com)
```

### Comparing `scientistmetrics-0.0.3/data/Life Expectancy Data.csv` & `scientistmetrics-0.0.4/data/Life Expectancy Data.csv`

 * *Files identical despite different names*

### Comparing `scientistmetrics-0.0.3/data/diabetes.csv` & `scientistmetrics-0.0.4/data/diabetes.csv`

 * *Files identical despite different names*

### Comparing `scientistmetrics-0.0.3/data/insurance.csv` & `scientistmetrics-0.0.4/data/insurance.csv`

 * *Files identical despite different names*

### Comparing `scientistmetrics-0.0.3/data/mushroom.xls` & `scientistmetrics-0.0.4/data/mushroom.xls`

 * *Files identical despite different names*

### Comparing `scientistmetrics-0.0.3/notebooks/model.ipynb` & `scientistmetrics-0.0.4/powerset_model.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.985563100240096%*

 * *Differences: {"'cells'": "{1: {'source': ['# warnings message\\n', 'import warnings\\n', "*

 * *            '"warnings.simplefilter(action=\'ignore\', category=FutureWarning)\\n", '*

 * *            '\'warnings.filterwarnings("ignore")\']}, 2: {\'execution_count\': 2, \'outputs\': {0: '*

 * *            "{'execution_count': 2}}, 'source': {insert: [(3, 'insurance = "*

 * *            'pd.read_csv("./data/insurance.csv",sep=",")\\n\')], delete: [4, 2]}}, 3: '*

 * *            "{'execution_count': 3}, 4: {'execution_count': 4}, 6: {'execution_cou […]*

```diff
@@ -17,33 +17,23 @@
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Set repository\n",
-                "import os\n",
-                "os.chdir(\"D:/Bureau/PythonProject/packages/scientistmetrics/data/\")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 2,
-            "metadata": {},
-            "outputs": [],
-            "source": [
                 "# warnings message\n",
                 "import warnings\n",
+                "warnings.simplefilter(action='ignore', category=FutureWarning)\n",
                 "warnings.filterwarnings(\"ignore\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -132,31 +122,30 @@
                             "0   19  female  27.900         0    yes  southwest  16884.92400\n",
                             "1   18    male  33.770         1     no  southeast   1725.55230\n",
                             "2   28    male  33.000         3     no  southeast   4449.46200\n",
                             "3   33    male  22.705         0     no  northwest  21984.47061\n",
                             "4   32    male  28.880         0     no  northwest   3866.85520"
                         ]
                     },
-                    "execution_count": 3,
+                    "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# Load dataset\n",
                 "import pandas as pd\n",
-                "import numpy as np \n",
                 "\n",
-                "insurance = pd.read_csv(\"insurance.csv\",sep=\",\")\n",
+                "insurance = pd.read_csv(\"./data/insurance.csv\",sep=\",\")\n",
                 "insurance.head()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "<class 'pandas.core.frame.DataFrame'>\n",
@@ -178,15 +167,15 @@
             ],
             "source": [
                 "insurance.info()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Powerset\n",
                 "from scientistmetrics import powersetmodel"
             ]
         },
@@ -195,19 +184,19 @@
             "metadata": {},
             "source": [
                 "## [Insurance dataset](https://www.kaggle.com/datasets/mirichoi0218/insurance)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [],
             "source": [
-                "powersetmodel( )"
+                "#powersetmodel( )"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {},
             "outputs": [],
@@ -222,67 +211,67 @@
             "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "                             predictor  count           aic           bic  \\\n",
-                        "0                                  age      1  20165.691448  20175.374679   \n",
-                        "1                                  sex      1  20254.342034  20264.025265   \n",
-                        "2                                  bmi      1  20218.207703  20227.890934   \n",
-                        "3                             children      1  20253.687895  20263.371126   \n",
-                        "4                               smoker      1  19361.465798  19371.149028   \n",
+                        "                             predictor  count           aic          aicc  \\\n",
+                        "0                                  age      1  20146.184782  20146.197643   \n",
+                        "1                                  sex      1  20238.440934  20238.453796   \n",
+                        "2                                  bmi      1  20207.571639  20207.584501   \n",
+                        "3                             children      1  20236.034544  20236.047406   \n",
+                        "4                               smoker      1  19315.215249  19315.228111   \n",
                         "..                                 ...    ...           ...           ...   \n",
-                        "58           sex+smoker+age+region+bmi      5  18956.398599  18995.131523   \n",
-                        "59      sex+children+smoker+age+region      5  19060.708924  19099.441848   \n",
-                        "60      children+smoker+age+region+bmi      5  18948.093466  18986.826390   \n",
-                        "61      sex+children+smoker+region+bmi      5  19245.006750  19283.739674   \n",
-                        "62  sex+children+smoker+age+region+bmi      6  18950.001771  18993.576310   \n",
+                        "58           bmi+region+smoker+age+sex      5  18939.761117  18939.916457   \n",
+                        "59      region+smoker+children+age+sex      5  19026.745683  19026.901023   \n",
+                        "60      bmi+region+smoker+children+age      5  18930.239296  18930.394636   \n",
+                        "61      bmi+region+smoker+children+sex      5  19203.364541  19203.519880   \n",
+                        "62  bmi+region+smoker+children+age+sex      6  18930.305506  18930.499891   \n",
                         "\n",
-                        "    rsquared  adj. rsquared  expl. var. score     max error  mean abs. error  \\\n",
-                        "0   0.092951       0.091980          0.080826  47441.580644      9168.424250   \n",
-                        "1   0.002843       0.001775          0.004197  45877.276541      9306.430742   \n",
-                        "2   0.040605       0.039578          0.036301  42192.255083      9429.268187   \n",
-                        "3   0.003540       0.002473          0.007042  45260.452040      9340.598349   \n",
-                        "4   0.615870       0.615459          0.628326  28111.608817      5656.730452   \n",
-                        "..       ...            ...               ...           ...              ...   \n",
-                        "58  0.753984       0.752128          0.735545  25352.699836      4309.384386   \n",
-                        "59  0.724981       0.722907          0.723397  28979.084771      3998.380328   \n",
-                        "60  0.756157       0.754318          0.737695  25404.540528      4318.042515   \n",
-                        "61  0.665131       0.662606          0.657970  28816.103678      5401.899702   \n",
-                        "62  0.756181       0.754077          0.737722  25328.174109      4321.661861   \n",
+                        "             bic  rsquared  adj. rsquared  expl. var. score     max error  \\\n",
+                        "0   20155.868013  0.096975       0.096008          0.075113  48034.926674   \n",
+                        "1   20248.124165  0.003434       0.002367          0.003001  48737.463817   \n",
+                        "2   20217.254870  0.035765       0.034733          0.047078  49574.260434   \n",
+                        "3   20245.717775  0.005993       0.004929          0.001336  50259.979313   \n",
+                        "4   19324.898480  0.628346       0.627948          0.600764  30279.845834   \n",
+                        "..           ...       ...            ...               ...           ...   \n",
+                        "58  18978.494041  0.754323       0.752470          0.733238  29957.831151   \n",
+                        "59  19065.478607  0.730398       0.728364          0.708360  29562.578097   \n",
+                        "60  18968.972220  0.756810       0.754976          0.735663  30315.837344   \n",
+                        "61  19242.097464  0.674408       0.671952          0.636199  32269.076471   \n",
+                        "62  18973.880045  0.757312       0.755217          0.733661  30543.928969   \n",
                         "\n",
-                        "    mean sq. error  median abs. error  r2 score  mean abs. percentage error  \\\n",
-                        "0     1.355551e+08        6605.181153  0.080813                    1.176197   \n",
-                        "1     1.469159e+08        7974.827889  0.003777                    1.583882   \n",
-                        "2     1.421947e+08        7745.732362  0.035791                    1.551790   \n",
-                        "3     1.465385e+08        8525.185106  0.006336                    1.554674   \n",
-                        "4     5.481998e+07        4508.504443  0.628271                    0.880813   \n",
-                        "..             ...                ...       ...                         ...   \n",
-                        "58    3.910992e+07        2636.387630  0.734799                    0.462572   \n",
-                        "59    4.086615e+07        1697.414453  0.722890                    0.312082   \n",
-                        "60    3.876490e+07        2713.458369  0.737139                    0.459219   \n",
-                        "61    5.044275e+07        4314.958856  0.657952                    0.804127   \n",
-                        "62    3.875988e+07        2723.954000  0.737173                    0.459775   \n",
+                        "            mae      mape           mse          rmse         mdae        r2  \\\n",
+                        "0   9191.933457  1.101783  1.421230e+08  11921.535549  6457.531701  0.070903   \n",
+                        "1   9280.790422  1.507500  1.526449e+08  12354.953478  7554.988847  0.002118   \n",
+                        "2   9185.404738  1.489000  1.459849e+08  12082.422679  7252.819945  0.045656   \n",
+                        "3   9319.556254  1.468374  1.528720e+08  12364.139862  8085.666225  0.000634   \n",
+                        "4   5912.169213  0.865078  6.111678e+07   7817.721913  4570.928400  0.600463   \n",
+                        "..          ...       ...           ...           ...          ...       ...   \n",
+                        "58  4342.902276  0.445015  4.090282e+07   6395.531494  2463.127876  0.732607   \n",
+                        "59  4285.518203  0.326734  4.465032e+07   6682.089517  1762.900790  0.708109   \n",
+                        "60  4273.346363  0.421702  4.052223e+07   6365.707636  2371.524976  0.735095   \n",
+                        "61  5623.417444  0.820317  5.566241e+07   7460.724777  4349.769423  0.636119   \n",
+                        "62  4302.712108  0.424122  4.082445e+07   6389.400994  2328.982072  0.733119   \n",
                         "\n",
                         "    likelihood test ratio  \n",
-                        "0             1229.689677  \n",
-                        "1             1318.340264  \n",
-                        "2             1282.205932  \n",
-                        "3             1317.686125  \n",
-                        "4              425.464027  \n",
+                        "0             1229.879276  \n",
+                        "1             1322.135428  \n",
+                        "2             1291.266133  \n",
+                        "3             1319.729038  \n",
+                        "4              398.909743  \n",
                         "..                    ...  \n",
-                        "58               8.396828  \n",
-                        "59             112.707153  \n",
-                        "60               0.091696  \n",
-                        "61             297.004980  \n",
+                        "58              11.455611  \n",
+                        "59              98.440177  \n",
+                        "60               1.933790  \n",
+                        "61             275.059035  \n",
                         "62               0.000000  \n",
                         "\n",
-                        "[63 rows x 14 columns]\n"
+                        "[63 rows x 16 columns]\n"
                     ]
                 }
             ],
             "source": [
                 "ols_metrics = ols_res[1]\n",
                 "print(ols_metrics)"
             ]
@@ -327,15 +316,15 @@
                         "dtypes: float64(2), int64(7)\n",
                         "memory usage: 54.1 KB\n"
                     ]
                 }
             ],
             "source": [
                 "# Load datasets\n",
-                "diabetes = pd.read_csv(\"diabetes.csv\",sep=\",\")\n",
+                "diabetes = pd.read_csv(\"./data/diabetes.csv\",sep=\",\")\n",
                 "diabetes.info()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {},
@@ -350,52 +339,52 @@
             "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "                                     predictor  count         aic         bic  \\\n",
-                        "0                          Pregnancies+Glucose      2  790.949984  804.881354   \n",
-                        "1                    BloodPressure+Pregnancies      2  961.255314  975.186683   \n",
-                        "2                    SkinThickness+Pregnancies      2  955.362685  969.294054   \n",
-                        "3                          Pregnancies+Insulin      2  945.340140  959.271509   \n",
-                        "4                              BMI+Pregnancies      2  887.143848  901.075217   \n",
+                        "                                     predictor  count         aic        aicc  \\\n",
+                        "0                          Glucose+Pregnancies      2  790.949984  790.981398   \n",
+                        "1                    BloodPressure+Pregnancies      2  961.255314  961.286728   \n",
+                        "2                    SkinThickness+Pregnancies      2  955.362685  955.394099   \n",
+                        "3                          Pregnancies+Insulin      2  945.340140  945.371554   \n",
+                        "4                              BMI+Pregnancies      2  887.143848  887.175261   \n",
                         "..                                         ...    ...         ...         ...   \n",
-                        "79  SkinThickness+DiabetesPedigreeFunction+Age      3  932.701545  951.276704   \n",
-                        "80        BMI+DiabetesPedigreeFunction+Insulin      3  912.372026  930.947185   \n",
-                        "81                             BMI+Age+Insulin      3  877.795909  896.371068   \n",
-                        "82        Age+DiabetesPedigreeFunction+Insulin      3  926.850265  945.425424   \n",
-                        "83            BMI+DiabetesPedigreeFunction+Age      3  870.006943  888.582102   \n",
+                        "79  SkinThickness+Age+DiabetesPedigreeFunction      3  932.701545  932.753970   \n",
+                        "80        BMI+DiabetesPedigreeFunction+Insulin      3  912.372026  912.424450   \n",
+                        "81                             BMI+Age+Insulin      3  877.795909  877.848334   \n",
+                        "82        DiabetesPedigreeFunction+Age+Insulin      3  926.850265  926.902690   \n",
+                        "83            BMI+Age+DiabetesPedigreeFunction      3  870.006943  870.059367   \n",
                         "\n",
-                        "    r2 mcfadden  r2 cox - snell  r2 nagelkerke  null deviance  resid deviance  \\\n",
-                        "0      0.209902        0.237786       0.327657      993.48391      784.949984   \n",
-                        "1      0.038479        0.048558       0.066911      993.48391      955.255314   \n",
-                        "2      0.044411        0.055830       0.076931      993.48391      949.362685   \n",
-                        "3      0.054499        0.068072       0.093799      993.48391      939.340140   \n",
-                        "4      0.113077        0.136081       0.187512      993.48391      881.143848   \n",
-                        "..          ...             ...            ...            ...             ...   \n",
-                        "79     0.069233        0.085667       0.118044      993.48391      924.701545   \n",
-                        "80     0.089696        0.109552       0.150957      993.48391      904.372026   \n",
-                        "81     0.124499        0.148752       0.204973      993.48391      869.795909   \n",
-                        "82     0.075123        0.092607       0.127607      993.48391      918.850265   \n",
-                        "83     0.132339        0.157342       0.216809      993.48391      862.006943   \n",
+                        "           bic  r2 mcfadden  r2 cox - snell  r2 nagelkerke  null deviance  \\\n",
+                        "0   804.881354     0.209902        0.237786       0.327657      993.48391   \n",
+                        "1   975.186683     0.038479        0.048558       0.066911      993.48391   \n",
+                        "2   969.294054     0.044411        0.055830       0.076931      993.48391   \n",
+                        "3   959.271509     0.054499        0.068072       0.093799      993.48391   \n",
+                        "4   901.075217     0.113077        0.136081       0.187512      993.48391   \n",
+                        "..         ...          ...             ...            ...            ...   \n",
+                        "79  951.276704     0.069233        0.085667       0.118044      993.48391   \n",
+                        "80  930.947185     0.089696        0.109552       0.150957      993.48391   \n",
+                        "81  896.371068     0.124499        0.148752       0.204973      993.48391   \n",
+                        "82  945.425424     0.075123        0.092607       0.127607      993.48391   \n",
+                        "83  888.582102     0.132339        0.157342       0.216809      993.48391   \n",
                         "\n",
-                        "    diff deviance  ...  recall score  f1 score       auc  sensibility  \\\n",
-                        "0      208.533926  ...      0.503731  0.580645  0.689866     0.503731   \n",
-                        "1       38.228596  ...      0.182836  0.277620  0.555418     0.182836   \n",
-                        "2       44.121225  ...      0.208955  0.312849  0.570478     0.208955   \n",
-                        "3       54.143770  ...      0.235075  0.331579  0.568537     0.235075   \n",
-                        "4      112.340063  ...      0.332090  0.425837  0.605045     0.332090   \n",
-                        "..            ...  ...           ...       ...       ...          ...   \n",
-                        "79      68.782365  ...      0.253731  0.342569  0.565866     0.253731   \n",
-                        "80      89.111884  ...      0.283582  0.380952  0.586791     0.283582   \n",
-                        "81     123.688001  ...      0.358209  0.445476  0.612104     0.358209   \n",
-                        "82      74.633645  ...      0.235075  0.324742  0.560537     0.235075   \n",
-                        "83     131.476967  ...      0.380597  0.463636  0.620299     0.380597   \n",
+                        "    resid deviance  ...  recall score  f1 score       auc  sensibility  \\\n",
+                        "0       784.949984  ...      0.503731  0.580645  0.805440     0.503731   \n",
+                        "1       955.255314  ...      0.182836  0.277620  0.628586     0.182836   \n",
+                        "2       949.362685  ...      0.208955  0.312849  0.641407     0.208955   \n",
+                        "3       939.340140  ...      0.235075  0.331579  0.650235     0.235075   \n",
+                        "4       881.143848  ...      0.332090  0.425837  0.721358     0.332090   \n",
+                        "..             ...  ...           ...       ...       ...          ...   \n",
+                        "79      924.701545  ...      0.253731  0.342569  0.698474     0.253731   \n",
+                        "80      904.372026  ...      0.283582  0.380952  0.713731     0.283582   \n",
+                        "81      869.795909  ...      0.358209  0.445476  0.740590     0.358209   \n",
+                        "82      918.850265  ...      0.235075  0.324742  0.704776     0.235075   \n",
+                        "83      862.006943  ...      0.380597  0.463636  0.751433     0.380597   \n",
                         "\n",
                         "    precision  specificity  False Pos. rate  younden index  likelihood ratio  \\\n",
                         "0    0.685279        0.876            0.124       0.379731          4.062350   \n",
                         "1    0.576471        0.928            0.072       0.110836          2.539386   \n",
                         "2    0.622222        0.932            0.068       0.140955          3.072871   \n",
                         "3    0.562500        0.902            0.098       0.137075          2.398721   \n",
                         "4    0.593333        0.878            0.122       0.210090          2.722046   \n",
@@ -415,15 +404,15 @@
                         "..                    ...  \n",
                         "79              62.694603  \n",
                         "80              42.365083  \n",
                         "81               7.788966  \n",
                         "82              56.843322  \n",
                         "83               0.000000  \n",
                         "\n",
-                        "[84 rows x 22 columns]\n"
+                        "[84 rows x 23 columns]\n"
                     ]
                 }
             ],
             "source": [
                 "glm_metrics = glm_res[1]\n",
                 "print(glm_metrics)"
             ]
```

### Comparing `scientistmetrics-0.0.3/performance.ipynb` & `scientistmetrics-0.0.4/performance.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987781660126747%*

 * *Differences: {"'cells'": "{4: {'outputs': {0: {'text': {insert: [(1, 'Int64Index: 51 entries, 0 to 50\\n'), "*

 * *            "(15, 'memory usage: 2.3+ KB\\n')], delete: [15, 1]}}}}, 6: {'outputs': {0: {'data': "*

 * *            "{'text/html': {insert: [(8, '         <td>Date:</td>        <td>2024-03-24 "*

 * *            "20:59</td>        <td>BIC:</td>         <td>713.9834</td>\\n')], delete: [8]}, "*

 * *            "'text/latex': {insert: [(8, 'Date:               & 2024-03-24 20:59 & "*

 * *            "BIC:                & 713.9834  \\ […]*

```diff
@@ -202,29 +202,29 @@
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "<class 'pandas.core.frame.DataFrame'>\n",
-                        "RangeIndex: 51 entries, 0 to 50\n",
+                        "Int64Index: 51 entries, 0 to 50\n",
                         "Data columns (total 9 columns):\n",
                         " #   Column    Non-Null Count  Dtype  \n",
                         "---  ------    --------------  -----  \n",
                         " 0   sid       51 non-null     float32\n",
                         " 1   state     51 non-null     object \n",
                         " 2   crime     51 non-null     int16  \n",
                         " 3   murder    51 non-null     float32\n",
                         " 4   pctmetro  51 non-null     float32\n",
                         " 5   pctwhite  51 non-null     float32\n",
                         " 6   pcths     51 non-null     float32\n",
                         " 7   poverty   51 non-null     float32\n",
                         " 8   single    51 non-null     float32\n",
                         "dtypes: float32(7), int16(1), object(1)\n",
-                        "memory usage: 2.0+ KB\n"
+                        "memory usage: 2.3+ KB\n"
                     ]
                 }
             ],
             "source": [
                 "# Informations\n",
                 "crime.info()"
             ]
@@ -321,15 +321,15 @@
                             "<tr>\n",
                             "        <td>Model:</td>               <td>OLS</td>         <td>Adj. R-squared:</td>     <td>0.695</td> \n",
                             "</tr>\n",
                             "<tr>\n",
                             "  <td>Dependent Variable:</td>       <td>crime</td>             <td>AIC:</td>         <td>708.1879</td>\n",
                             "</tr>\n",
                             "<tr>\n",
-                            "         <td>Date:</td>        <td>2023-09-17 18:11</td>        <td>BIC:</td>         <td>713.9834</td>\n",
+                            "         <td>Date:</td>        <td>2024-03-24 20:59</td>        <td>BIC:</td>         <td>713.9834</td>\n",
                             "</tr>\n",
                             "<tr>\n",
                             "   <td>No. Observations:</td>         <td>51</td>          <td>Log-Likelihood:</td>    <td>-351.09</td>\n",
                             "</tr>\n",
                             "<tr>\n",
                             "       <td>Df Model:</td>              <td>2</td>           <td>F-statistic:</td>       <td>57.96</td> \n",
                             "</tr>\n",
@@ -376,15 +376,15 @@
                             "\\caption{Results: Ordinary least squares}\n",
                             "\\label{}\n",
                             "\\begin{center}\n",
                             "\\begin{tabular}{llll}\n",
                             "\\hline\n",
                             "Model:              & OLS              & Adj. R-squared:     & 0.695     \\\\\n",
                             "Dependent Variable: & crime            & AIC:                & 708.1879  \\\\\n",
-                            "Date:               & 2023-09-17 18:11 & BIC:                & 713.9834  \\\\\n",
+                            "Date:               & 2024-03-24 20:59 & BIC:                & 713.9834  \\\\\n",
                             "No. Observations:   & 51               & Log-Likelihood:     & -351.09   \\\\\n",
                             "Df Model:           & 2                & F-statistic:        & 57.96     \\\\\n",
                             "Df Residuals:       & 48               & Prob (F-statistic): & 1.58e-13  \\\\\n",
                             "R-squared:          & 0.707            & Scale:              & 59346.    \\\\\n",
                             "\\hline\n",
                             "\\end{tabular}\n",
                             "\\end{center}\n",
@@ -419,15 +419,15 @@
                         "text/plain": [
                             "<class 'statsmodels.iolib.summary2.Summary'>\n",
                             "\"\"\"\n",
                             "                 Results: Ordinary least squares\n",
                             "=================================================================\n",
                             "Model:              OLS              Adj. R-squared:     0.695   \n",
                             "Dependent Variable: crime            AIC:                708.1879\n",
-                            "Date:               2023-09-17 18:11 BIC:                713.9834\n",
+                            "Date:               2024-03-24 20:59 BIC:                713.9834\n",
                             "No. Observations:   51               Log-Likelihood:     -351.09 \n",
                             "Df Model:           2                F-statistic:        57.96   \n",
                             "Df Residuals:       48               Prob (F-statistic): 1.58e-13\n",
                             "R-squared:          0.707            Scale:              59346.  \n",
                             "-----------------------------------------------------------------\n",
                             "            Coef.    Std.Err.    t    P>|t|    [0.025     0.975] \n",
                             "-----------------------------------------------------------------\n",
@@ -672,15 +672,15 @@
                             "<tr>\n",
                             "        <td>Model:</td>              <td>Logit</td>           <td>Method:</td>          <td>MLE</td>   \n",
                             "</tr>\n",
                             "<tr>\n",
                             "  <td>Dependent Variable:</td>       <td>admit</td>      <td>Pseudo R-squared:</td>    <td>0.083</td>  \n",
                             "</tr>\n",
                             "<tr>\n",
-                            "         <td>Date:</td>        <td>2023-09-17 18:11</td>       <td>AIC:</td>         <td>470.5175</td> \n",
+                            "         <td>Date:</td>        <td>2024-03-24 21:00</td>       <td>AIC:</td>         <td>470.5175</td> \n",
                             "</tr>\n",
                             "<tr>\n",
                             "   <td>No. Observations:</td>         <td>400</td>             <td>BIC:</td>         <td>494.4663</td> \n",
                             "</tr>\n",
                             "<tr>\n",
                             "       <td>Df Model:</td>              <td>5</td>         <td>Log-Likelihood:</td>    <td>-229.26</td> \n",
                             "</tr>\n",
@@ -723,15 +723,15 @@
                             "\\caption{Results: Logit}\n",
                             "\\label{}\n",
                             "\\begin{center}\n",
                             "\\begin{tabular}{llll}\n",
                             "\\hline\n",
                             "Model:              & Logit            & Method:           & MLE         \\\\\n",
                             "Dependent Variable: & admit            & Pseudo R-squared: & 0.083       \\\\\n",
-                            "Date:               & 2023-09-17 18:11 & AIC:              & 470.5175    \\\\\n",
+                            "Date:               & 2024-03-24 21:00 & AIC:              & 470.5175    \\\\\n",
                             "No. Observations:   & 400              & BIC:              & 494.4663    \\\\\n",
                             "Df Model:           & 5                & Log-Likelihood:   & -229.26     \\\\\n",
                             "Df Residuals:       & 394              & LL-Null:          & -249.99     \\\\\n",
                             "Converged:          & 1.0000           & LLR p-value:      & 7.5782e-08  \\\\\n",
                             "No. Iterations:     & 6.0000           & Scale:            & 1.0000      \\\\\n",
                             "\\hline\n",
                             "\\end{tabular}\n",
@@ -757,15 +757,15 @@
                         "text/plain": [
                             "<class 'statsmodels.iolib.summary2.Summary'>\n",
                             "\"\"\"\n",
                             "                         Results: Logit\n",
                             "=================================================================\n",
                             "Model:              Logit            Method:           MLE       \n",
                             "Dependent Variable: admit            Pseudo R-squared: 0.083     \n",
-                            "Date:               2023-09-17 18:11 AIC:              470.5175  \n",
+                            "Date:               2024-03-24 21:00 AIC:              470.5175  \n",
                             "No. Observations:   400              BIC:              494.4663  \n",
                             "Df Model:           5                Log-Likelihood:   -229.26   \n",
                             "Df Residuals:       394              LL-Null:          -249.99   \n",
                             "Converged:          1.0000           LLR p-value:      7.5782e-08\n",
                             "No. Iterations:     6.0000           Scale:            1.0000    \n",
                             "------------------------------------------------------------------\n",
                             "               Coef.   Std.Err.     z     P>|z|    [0.025   0.975]\n",
@@ -958,15 +958,15 @@
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "<class 'pandas.core.frame.DataFrame'>\n",
-                        "RangeIndex: 200 entries, 0 to 199\n",
+                        "Int64Index: 200 entries, 0 to 199\n",
                         "Data columns (total 13 columns):\n",
                         " #   Column   Non-Null Count  Dtype   \n",
                         "---  ------   --------------  -----   \n",
                         " 0   id       200 non-null    float32 \n",
                         " 1   female   200 non-null    category\n",
                         " 2   ses      200 non-null    category\n",
                         " 3   schtyp   200 non-null    category\n",
@@ -976,15 +976,15 @@
                         " 7   math     200 non-null    float32 \n",
                         " 8   science  200 non-null    float32 \n",
                         " 9   socst    200 non-null    float32 \n",
                         " 10  honors   200 non-null    category\n",
                         " 11  awards   200 non-null    float32 \n",
                         " 12  cid      200 non-null    int16   \n",
                         "dtypes: category(5), float32(7), int16(1)\n",
-                        "memory usage: 7.6 KB\n"
+                        "memory usage: 9.0 KB\n"
                     ]
                 }
             ],
             "source": [
                 "hsbdemo.info()"
             ]
         },
@@ -1127,15 +1127,15 @@
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "<class 'pandas.core.frame.DataFrame'>\n",
-                        "RangeIndex: 200 entries, 0 to 199\n",
+                        "Int64Index: 200 entries, 0 to 199\n",
                         "Data columns (total 13 columns):\n",
                         " #   Column   Non-Null Count  Dtype   \n",
                         "---  ------   --------------  -----   \n",
                         " 0   id       200 non-null    float32 \n",
                         " 1   female   200 non-null    category\n",
                         " 2   ses      200 non-null    category\n",
                         " 3   schtyp   200 non-null    category\n",
@@ -1145,15 +1145,15 @@
                         " 7   math     200 non-null    float32 \n",
                         " 8   science  200 non-null    float32 \n",
                         " 9   socst    200 non-null    float32 \n",
                         " 10  honors   200 non-null    category\n",
                         " 11  awards   200 non-null    float32 \n",
                         " 12  cid      200 non-null    int16   \n",
                         "dtypes: category(4), float32(7), int16(1), int32(1)\n",
-                        "memory usage: 8.0 KB\n"
+                        "memory usage: 9.5 KB\n"
                     ]
                 }
             ],
             "source": [
                 "hsbdemo.info()"
             ]
         },
@@ -1169,15 +1169,15 @@
                             "<tr>\n",
                             "        <td>Model:</td>             <td>MNLogit</td>          <td>Method:</td>          <td>MLE</td>   \n",
                             "</tr>\n",
                             "<tr>\n",
                             "  <td>Dependent Variable:</td>       <td>prog</td>       <td>Pseudo R-squared:</td>    <td>0.118</td>  \n",
                             "</tr>\n",
                             "<tr>\n",
-                            "         <td>Date:</td>        <td>2023-09-17 18:11</td>       <td>AIC:</td>         <td>375.9635</td> \n",
+                            "         <td>Date:</td>        <td>2024-03-24 21:00</td>       <td>AIC:</td>         <td>375.9635</td> \n",
                             "</tr>\n",
                             "<tr>\n",
                             "   <td>No. Observations:</td>         <td>200</td>             <td>BIC:</td>         <td>402.3500</td> \n",
                             "</tr>\n",
                             "<tr>\n",
                             "       <td>Df Model:</td>              <td>6</td>         <td>Log-Likelihood:</td>    <td>-179.98</td> \n",
                             "</tr>\n",
@@ -1231,15 +1231,15 @@
                             "\\caption{Results: MNLogit}\n",
                             "\\label{}\n",
                             "\\begin{center}\n",
                             "\\begin{tabular}{llll}\n",
                             "\\hline\n",
                             "Model:              & MNLogit          & Method:           & MLE         \\\\\n",
                             "Dependent Variable: & prog             & Pseudo R-squared: & 0.118       \\\\\n",
-                            "Date:               & 2023-09-17 18:11 & AIC:              & 375.9635    \\\\\n",
+                            "Date:               & 2024-03-24 21:00 & AIC:              & 375.9635    \\\\\n",
                             "No. Observations:   & 200              & BIC:              & 402.3500    \\\\\n",
                             "Df Model:           & 6                & Log-Likelihood:   & -179.98     \\\\\n",
                             "Df Residuals:       & 192              & LL-Null:          & -204.10     \\\\\n",
                             "Converged:          & 1.0000           & LLR p-value:      & 1.0630e-08  \\\\\n",
                             "No. Iterations:     & 6.0000           & Scale:            & 1.0000      \\\\\n",
                             "\\hline\n",
                             "\\end{tabular}\n",
@@ -1276,15 +1276,15 @@
                         "text/plain": [
                             "<class 'statsmodels.iolib.summary2.Summary'>\n",
                             "\"\"\"\n",
                             "                        Results: MNLogit\n",
                             "=================================================================\n",
                             "Model:              MNLogit          Method:           MLE       \n",
                             "Dependent Variable: prog             Pseudo R-squared: 0.118     \n",
-                            "Date:               2023-09-17 18:11 AIC:              375.9635  \n",
+                            "Date:               2024-03-24 21:00 AIC:              375.9635  \n",
                             "No. Observations:   200              BIC:              402.3500  \n",
                             "Df Model:           6                Log-Likelihood:   -179.98   \n",
                             "Df Residuals:       192              LL-Null:          -204.10   \n",
                             "Converged:          1.0000           LLR p-value:      1.0630e-08\n",
                             "No. Iterations:     6.0000           Scale:            1.0000    \n",
                             "-----------------------------------------------------------------\n",
                             "     prog = 0      Coef.  Std.Err.    t    P>|t|   [0.025  0.975]\n",
@@ -1420,24 +1420,24 @@
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "<class 'pandas.core.frame.DataFrame'>\n",
-                        "RangeIndex: 400 entries, 0 to 399\n",
+                        "Int64Index: 400 entries, 0 to 399\n",
                         "Data columns (total 4 columns):\n",
                         " #   Column  Non-Null Count  Dtype   \n",
                         "---  ------  --------------  -----   \n",
                         " 0   apply   400 non-null    category\n",
                         " 1   pared   400 non-null    int8    \n",
                         " 2   public  400 non-null    int8    \n",
                         " 3   gpa     400 non-null    float32 \n",
                         "dtypes: category(1), float32(1), int8(2)\n",
-                        "memory usage: 3.0 KB\n"
+                        "memory usage: 6.0 KB\n"
                     ]
                 }
             ],
             "source": [
                 "olg.info()"
             ]
         },
@@ -1526,18 +1526,18 @@
                             "<tr>\n",
                             "  <th>Model:</th>               <td>OrderedModel</td>    <th>  AIC:               </th> <td>   727.0</td>\n",
                             "</tr>\n",
                             "<tr>\n",
                             "  <th>Method:</th>           <td>Maximum Likelihood</td> <th>  BIC:               </th> <td>   747.0</td>\n",
                             "</tr>\n",
                             "<tr>\n",
-                            "  <th>Date:</th>              <td>Sun, 17 Sep 2023</td>  <th>                     </th>     <td> </td>   \n",
+                            "  <th>Date:</th>              <td>Sun, 24 Mar 2024</td>  <th>                     </th>     <td> </td>   \n",
                             "</tr>\n",
                             "<tr>\n",
-                            "  <th>Time:</th>                  <td>18:11:58</td>      <th>                     </th>     <td> </td>   \n",
+                            "  <th>Time:</th>                  <td>21:00:03</td>      <th>                     </th>     <td> </td>   \n",
                             "</tr>\n",
                             "<tr>\n",
                             "  <th>No. Observations:</th>       <td>   400</td>       <th>                     </th>     <td> </td>   \n",
                             "</tr>\n",
                             "<tr>\n",
                             "  <th>Df Residuals:</th>           <td>   395</td>       <th>                     </th>     <td> </td>   \n",
                             "</tr>\n",
@@ -1569,16 +1569,16 @@
                         "text/latex": [
                             "\\begin{center}\n",
                             "\\begin{tabular}{lclc}\n",
                             "\\toprule\n",
                             "\\textbf{Dep. Variable:}              &       apply        & \\textbf{  Log-Likelihood:    } &   -358.51   \\\\\n",
                             "\\textbf{Model:}                      &    OrderedModel    & \\textbf{  AIC:               } &     727.0   \\\\\n",
                             "\\textbf{Method:}                     & Maximum Likelihood & \\textbf{  BIC:               } &     747.0   \\\\\n",
-                            "\\textbf{Date:}                       &  Sun, 17 Sep 2023  & \\textbf{                     } &             \\\\\n",
-                            "\\textbf{Time:}                       &      18:11:58      & \\textbf{                     } &             \\\\\n",
+                            "\\textbf{Date:}                       &  Sun, 24 Mar 2024  & \\textbf{                     } &             \\\\\n",
+                            "\\textbf{Time:}                       &      21:00:03      & \\textbf{                     } &             \\\\\n",
                             "\\textbf{No. Observations:}           &          400       & \\textbf{                     } &             \\\\\n",
                             "\\textbf{Df Residuals:}               &          395       & \\textbf{                     } &             \\\\\n",
                             "\\textbf{Df Model:}                   &            3       & \\textbf{                     } &             \\\\\n",
                             "\\bottomrule\n",
                             "\\end{tabular}\n",
                             "\\begin{tabular}{lcccccc}\n",
                             "                                     & \\textbf{coef} & \\textbf{std err} & \\textbf{z} & \\textbf{P$> |$z$|$} & \\textbf{[0.025} & \\textbf{0.975]}  \\\\\n",
@@ -1597,16 +1597,16 @@
                             "<class 'statsmodels.iolib.summary.Summary'>\n",
                             "\"\"\"\n",
                             "                             OrderedModel Results                             \n",
                             "==============================================================================\n",
                             "Dep. Variable:                  apply   Log-Likelihood:                -358.51\n",
                             "Model:                   OrderedModel   AIC:                             727.0\n",
                             "Method:            Maximum Likelihood   BIC:                             747.0\n",
-                            "Date:                Sun, 17 Sep 2023                                         \n",
-                            "Time:                        18:11:58                                         \n",
+                            "Date:                Sun, 24 Mar 2024                                         \n",
+                            "Time:                        21:00:03                                         \n",
                             "No. Observations:                 400                                         \n",
                             "Df Residuals:                     395                                         \n",
                             "Df Model:                           3                                         \n",
                             "===============================================================================================\n",
                             "                                  coef    std err          z      P>|z|      [0.025      0.975]\n",
                             "-----------------------------------------------------------------------------------------------\n",
                             "pared                           1.0476      0.266      3.942      0.000       0.527       1.569\n",
@@ -1986,18 +1986,18 @@
                             "<tr>\n",
                             "  <th>Model:</th>                <td>Poisson</td>     <th>  Df Residuals:      </th>  <td>   196</td>  \n",
                             "</tr>\n",
                             "<tr>\n",
                             "  <th>Method:</th>                 <td>MLE</td>       <th>  Df Model:          </th>  <td>     3</td>  \n",
                             "</tr>\n",
                             "<tr>\n",
-                            "  <th>Date:</th>            <td>Sun, 17 Sep 2023</td> <th>  Pseudo R-squ.:     </th>  <td>0.2118</td>  \n",
+                            "  <th>Date:</th>            <td>Sun, 24 Mar 2024</td> <th>  Pseudo R-squ.:     </th>  <td>0.2118</td>  \n",
                             "</tr>\n",
                             "<tr>\n",
-                            "  <th>Time:</th>                <td>18:11:59</td>     <th>  Log-Likelihood:    </th> <td> -182.75</td> \n",
+                            "  <th>Time:</th>                <td>21:00:05</td>     <th>  Log-Likelihood:    </th> <td> -182.75</td> \n",
                             "</tr>\n",
                             "<tr>\n",
                             "  <th>converged:</th>             <td>True</td>       <th>  LL-Null:           </th> <td> -231.86</td> \n",
                             "</tr>\n",
                             "<tr>\n",
                             "  <th>Covariance Type:</th>     <td>nonrobust</td>    <th>  LLR p-value:       </th> <td>3.747e-21</td>\n",
                             "</tr>\n",
@@ -2023,16 +2023,16 @@
                         "text/latex": [
                             "\\begin{center}\n",
                             "\\begin{tabular}{lclc}\n",
                             "\\toprule\n",
                             "\\textbf{Dep. Variable:}     &   num\\_awards    & \\textbf{  No. Observations:  } &      200    \\\\\n",
                             "\\textbf{Model:}             &     Poisson      & \\textbf{  Df Residuals:      } &      196    \\\\\n",
                             "\\textbf{Method:}            &       MLE        & \\textbf{  Df Model:          } &        3    \\\\\n",
-                            "\\textbf{Date:}              & Sun, 17 Sep 2023 & \\textbf{  Pseudo R-squ.:     } &   0.2118    \\\\\n",
-                            "\\textbf{Time:}              &     18:11:59     & \\textbf{  Log-Likelihood:    } &   -182.75   \\\\\n",
+                            "\\textbf{Date:}              & Sun, 24 Mar 2024 & \\textbf{  Pseudo R-squ.:     } &   0.2118    \\\\\n",
+                            "\\textbf{Time:}              &     21:00:05     & \\textbf{  Log-Likelihood:    } &   -182.75   \\\\\n",
                             "\\textbf{converged:}         &       True       & \\textbf{  LL-Null:           } &   -231.86   \\\\\n",
                             "\\textbf{Covariance Type:}   &    nonrobust     & \\textbf{  LLR p-value:       } & 3.747e-21   \\\\\n",
                             "\\bottomrule\n",
                             "\\end{tabular}\n",
                             "\\begin{tabular}{lcccccc}\n",
                             "                            & \\textbf{coef} & \\textbf{std err} & \\textbf{z} & \\textbf{P$> |$z$|$} & \\textbf{[0.025} & \\textbf{0.975]}  \\\\\n",
                             "\\midrule\n",
@@ -2049,16 +2049,16 @@
                             "<class 'statsmodels.iolib.summary.Summary'>\n",
                             "\"\"\"\n",
                             "                          Poisson Regression Results                          \n",
                             "==============================================================================\n",
                             "Dep. Variable:             num_awards   No. Observations:                  200\n",
                             "Model:                        Poisson   Df Residuals:                      196\n",
                             "Method:                           MLE   Df Model:                            3\n",
-                            "Date:                Sun, 17 Sep 2023   Pseudo R-squ.:                  0.2118\n",
-                            "Time:                        18:11:59   Log-Likelihood:                -182.75\n",
+                            "Date:                Sun, 24 Mar 2024   Pseudo R-squ.:                  0.2118\n",
+                            "Time:                        21:00:05   Log-Likelihood:                -182.75\n",
                             "converged:                       True   LL-Null:                       -231.86\n",
                             "Covariance Type:            nonrobust   LLR p-value:                 3.747e-21\n",
                             "======================================================================================\n",
                             "                         coef    std err          z      P>|z|      [0.025      0.975]\n",
                             "--------------------------------------------------------------------------------------\n",
                             "Intercept             -5.2471      0.658     -7.969      0.000      -6.538      -3.957\n",
                             "prog[T.Academic]       1.0839      0.358      3.025      0.002       0.382       1.786\n",
@@ -2220,15 +2220,15 @@
             "cell_type": "code",
             "execution_count": 35,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "LikelihoodRatioTestResult(statistic=48.2298960501376, pvalue=1.0630010486697938e-08)"
+                            "LikelihoodRatioTestResult(statistic=48.22989605013754, pvalue=1.0630010486698236e-08)"
                         ]
                     },
                     "execution_count": 35,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -2287,15 +2287,15 @@
             "cell_type": "code",
             "execution_count": 38,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "HosmerLemeshowResult(statistic=11.085471996692485, df_denom=8, pvalue=0.19690311592785836)"
+                            "HosmerLemeshowResult(statistic=11.08547199669248, df_denom=8, pvalue=0.1969031159278586)"
                         ]
                     },
                     "execution_count": 38,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -2354,15 +2354,15 @@
                         "needs_background": "light"
                     },
                     "output_type": "display_data"
                 },
                 {
                     "data": {
                         "text/plain": [
-                            "<ggplot: (127913659996)>"
+                            "<ggplot: (151421289740)>"
                         ]
                     },
                     "execution_count": 40,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -2622,15 +2622,15 @@
                             " 'BIC': 494.4662797585469,\n",
                             " 'accuracy': 0.71,\n",
                             " 'r2 mcfadden': 0.08292194470084713,\n",
                             " 'r2 mcfadden adj.': 0.066921193229454,\n",
                             " 'r2 coxsnell': 0.09845702133885237,\n",
                             " 'r2 naglekerke': 0.13799580151192056,\n",
                             " 'r2 efron': 0.1014324863895315,\n",
-                            " 'r2 mckelvey': 0.0066827308985470645,\n",
+                            " 'r2 mckelvey': 0.006682730898547062,\n",
                             " 'r2 count': 0.71,\n",
                             " 'r2 count adj.': 0.08661417322834646,\n",
                             " 'r2 tjur': 0.10178650650542126}"
                         ]
                     },
                     "execution_count": 52,
                     "metadata": {},
@@ -2645,22 +2645,22 @@
             "cell_type": "code",
             "execution_count": 53,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "{'AIC': 375.9634524301854,\n",
-                            " 'AICC': 368.16858063531356,\n",
-                            " 'BIC': 402.34999136256965,\n",
+                            "{'AIC': 375.96345243018544,\n",
+                            " 'AICC': 368.1685806353137,\n",
+                            " 'BIC': 402.3499913625697,\n",
                             " 'accuracy': 0.61,\n",
-                            " 'r2 mcfadden': 0.11815453688722355,\n",
-                            " 'r2 mcfadden adj.': 0.09365634249667465,\n",
-                            " 'r2 coxsnell': 0.21427583263584715,\n",
-                            " 'r2 naglekerke': 0.24626662225304194}"
+                            " 'r2 mcfadden': 0.11815453688722333,\n",
+                            " 'r2 mcfadden adj.': 0.09365634249667454,\n",
+                            " 'r2 coxsnell': 0.21427583263584693,\n",
+                            " 'r2 naglekerke': 0.2462666222530417}"
                         ]
                     },
                     "execution_count": 53,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -3402,15 +3402,15 @@
             "cell_type": "code",
             "execution_count": 69,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "KMOTestResults(value=0.5925472020281817, per_variable=[0.32313631347117067, 0.7633859857484487, 0.6648330185773383, 0.7047119273096056, 0.7429435784725651, 0.6493663908585433, 0.5698283001266957, 0.7235123067251679, 0.6759970081430624, 0.628941773717484, 0.49041648508729574])"
+                            "KMOTestResults(value=0.5925472020281817, per_variable=[0.32313631347117067, 0.7633859857484487, 0.6648330185773383, 0.7047119273096056, 0.742943578472565, 0.6493663908585433, 0.569828300126696, 0.7235123067251679, 0.6759970081430625, 0.628941773717484, 0.4904164850872956])"
                         ]
                     },
                     "execution_count": 69,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -3422,15 +3422,15 @@
             "cell_type": "code",
             "execution_count": 70,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "BartlettSphericityTestResult(statistic=408.01163479701523, df_denom=55.0, pvalue=2.226926752118683e-55)"
+                            "BartlettSphericityTestResult(statistic=408.0116347970153, df_denom=55.0, pvalue=2.226926752118619e-55)"
                         ]
                     },
                     "execution_count": 70,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -3631,15 +3631,15 @@
             "cell_type": "code",
             "execution_count": 77,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "<statsmodels.stats.outliers_influence.GLMInfluence at 0x1dc84022410>"
+                            "<statsmodels.stats.outliers_influence.GLMInfluence at 0x23418b7fd60>"
                         ]
                     },
                     "execution_count": 77,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -3781,15 +3781,15 @@
                             " 'BIC': 494.4662797585469,\n",
                             " 'accuracy': 0.71,\n",
                             " 'r2 mcfadden': 0.08292194470084713,\n",
                             " 'r2 mcfadden adj.': 0.066921193229454,\n",
                             " 'r2 coxsnell': 0.09845702133885237,\n",
                             " 'r2 naglekerke': 0.13799580151192056,\n",
                             " 'r2 efron': 0.1014324863895315,\n",
-                            " 'r2 mckelvey': 0.0066827308985470645,\n",
+                            " 'r2 mckelvey': 0.006682730898547062,\n",
                             " 'r2 count': 0.71,\n",
                             " 'r2 count adj.': 0.08661417322834646,\n",
                             " 'r2 tjur': 0.10178650650542126}"
                         ]
                     },
                     "execution_count": 82,
                     "metadata": {},
@@ -3804,22 +3804,22 @@
             "cell_type": "code",
             "execution_count": 83,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
-                            "{'AIC': 375.9634524301854,\n",
-                            " 'AICC': 368.16858063531356,\n",
-                            " 'BIC': 402.34999136256965,\n",
+                            "{'AIC': 375.96345243018544,\n",
+                            " 'AICC': 368.1685806353137,\n",
+                            " 'BIC': 402.3499913625697,\n",
                             " 'accuracy': 0.61,\n",
-                            " 'r2 mcfadden': 0.11815453688722355,\n",
-                            " 'r2 mcfadden adj.': 0.09365634249667465,\n",
-                            " 'r2 coxsnell': 0.21427583263584715,\n",
-                            " 'r2 naglekerke': 0.24626662225304194}"
+                            " 'r2 mcfadden': 0.11815453688722333,\n",
+                            " 'r2 mcfadden adj.': 0.09365634249667454,\n",
+                            " 'r2 coxsnell': 0.21427583263584693,\n",
+                            " 'r2 naglekerke': 0.2462666222530417}"
                         ]
                     },
                     "execution_count": 83,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -4018,14 +4018,34 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "compare_performance(model=[ols,glm,mlogit,ologit,poisson])"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 87,
+            "metadata": {},
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "0.08292194470084713"
+                        ]
+                    },
+                    "execution_count": 87,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
+            "source": [
+                "r2_mcfadden(glm)"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
```

### Comparing `scientistmetrics-0.0.3/scientistmetrics/powerset.py` & `scientistmetrics-0.0.4/scientistmetrics/powerset.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,72 +1,94 @@
 # -*- coding: utf-8 -*-
 
-import numpy as np
 import pandas as pd
 from sklearn.model_selection import train_test_split
 from more_itertools import powerset
 import statsmodels.formula.api as smf
-import statsmodels.api as sm
-from sklearn.metrics import (
-    # Regression metrics
-    explained_variance_score,
-    max_error,
-    mean_absolute_error,
-    mean_squared_error,
-    mean_squared_log_error,
-    median_absolute_error,
-    r2_score,
-    mean_absolute_percentage_error,
-    # Classification metrics
-    confusion_matrix,
-    accuracy_score,
-    recall_score,
-    f1_score,
-    roc_auc_score,
-)
+from sklearn.metrics import confusion_matrix
+
+from .extractAIC import extractAIC
+from .extractAICC import extractAICC
+from .extractBIC import extractBIC
+
+from .explained_variance_score import explained_variance_score
+from .max_error import max_error
+from .mae import mae
+from .mse import mse
+from .rmse import rmse
+from .mdae import mdae
+from .r2_score import r2_score
+from .mape import mape
+from .accuracy_score import accuracy_score
+from .recall_score import recall_score
+from .f1_score import f1_score
+from .roc_auc_score import roc_auc_score
+from .error_rate import error_rate
+
+from .r2_coxsnell import r2_coxsnell
+from .r2_nagelkerke import r2_nagelkerke
 
 # https://jbhender.github.io/Stats506/F18/GP/Group5.html
 
 def powersetmodel(DTrain=pd.DataFrame,
                   DTest=None,
                   split_data = True,
                   model_type ="linear",
-                  target=str,
+                  target=None,
                   test_size=0.3,
                   random_state=None,
                   shuffle=True,
                   stratity=None,
                   num_from=None,
                   num_to=None):
     """
-    This function return all subsets models giving a set of variables.
+    Powerset Model
+    ---------------
+
+    This function return all subsets models giving a set of variables
 
     Parameters
     ----------
     DTrain : DataFrame
             Training sample
+
     DTest : DataFrame, default = None
             Test sample
+
     split_data : bool, default= True. If Data should be split in train set and test set. Used if DTest is not None. 
+
     model_type : {"linear","logistic"}, default = "linear".
+
     target : target name,
+
     test_size : float or int, default=None
                  If float, should be between 0.0 and 1.0 and represent the proportion of the dataset to include in 
                  the test split. If int, represents the absolute number of test samples. If None, the value is set 
                  to the complement of the train size. If train_size is also None, it will be set to 0.25.
                  See : "https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html"
+
     random_state : int, RandomState instance or None, default=None
                    Controls the shuffling applied to the data before applying the split. 
                    Pass an int for reproducible output across multiple function calls. 
                    See "https://scikit-learn.org/stable/glossary.html#term-random_state"
+
     shuffle : bool, default=True
                Whether or not to shuffle the data before splitting. If shuffle=False then stratify must be None.
+
     stratify : array-like, default=None.
                If not None, data is split in a stratified fashion, using this as the class labels. 
                Read more in the "https://scikit-learn.org/stable/modules/cross_validation.html#stratification"
+    
+    Return
+    ------
+    a tuple of two elements
+    
+    Author(s)
+    --------
+    Duvérier DJIFACK ZEBAZE duverierdjifack@gmail.com
     """
 
     # Set testing samples
     if not isinstance(DTrain,pd.DataFrame):
         raise TypeError(f"{type(DTrain)} is not supported. Please convert to a DataFrame with "
                         "pd.DataFrame. For more information see: "
                         "https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html")
@@ -77,65 +99,74 @@
                             "pd.DataFrame. For more information see: "
                             "https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html")
     else:
         if split_data:
             DTrain, DTest = train_test_split(DTrain,test_size=test_size,random_state=random_state,shuffle=shuffle,stratify=stratity)
         else:
             DTest = DTrain
+
+    if target is None:
+        raise ValueError("'target' must be assigned")
+    
+    # 
+    if model_type not in ["linear","logistic"]:
+        raise ValueError("'model_type' should be one of 'linear', 'logistic'")
         
     # Create formula : https://stackoverflow.com/questions/35518477/statsmodels-short-way-of-writing-formula
     def create_formula(y=str,x=list[str]):
         return y + ' ~ ' + ' + '.join(x)
     
     def predictor(x):
         return '+'.join(x)
 
     # List of features
-    features = list(DTrain.drop(columns=target).columns)
+    features = DTrain.drop(columns=target).columns.tolist()
     # Powerset features and Remove first element
     list_features = list(map(set, powerset(features)))[1:]
 
     # Reduce list_features using num_from and num_to
     if num_from is None:
         num_from = 1
     if num_to is None:
         num_to = len(list_features[-1])
     
     if num_from >= num_to:
-        raise ValueError("Error : 'num_from' must be small than 'num_to'.")
+        raise ValueError("'num_from' must be small than 'num_to'.")
 
     list_features = [num for num in list_features if len(num) in range(num_from,num_to+1,1)]
 
     ################################################################################
     # General metrics - AIC, BIC
     ################################################################################
     def general_metrics(x,model):
         gen_res = {"predictor" : predictor(x),
                    "count":len(x),
-                   "aic":model.aic,
-                   "bic":model.bic}
+                   "aic": extractAIC(model),
+                   "aicc" : extractAICC(model),
+                   "bic":extractBIC(model)}
         return pd.DataFrame(gen_res,index=["metrics"])
     
     def likelihood_ratio_test(full_model, ho_model):
         return 2*(full_model.llf - ho_model.llf)
 
     #################################################################################
     #  Linear regression 
     #################################################################################
     # linear regression metrics
     def ols_metrics(model,ytrue,ypred):
         res = {"rsquared":model.rsquared,
                "adj. rsquared" : model.rsquared_adj,
-               "expl. var. score" : explained_variance_score(ytrue,ypred),
-               "max error" : max_error(ytrue,ypred),
-               "mean abs. error" : mean_absolute_error(ytrue,ypred),
-               "mean sq. error" : mean_squared_error(ytrue,ypred),
-               "median abs. error" : median_absolute_error(ytrue,ypred),
-               "r2 score" : r2_score(ytrue,ypred),
-               "mean abs. percentage error" : mean_absolute_percentage_error(ytrue,ypred)}
+               "expl. var. score" : explained_variance_score(y_true=ytrue,y_pred=ypred),
+               "max error" : max_error(y_true=ytrue,y_pred=ypred),
+               "mae" : mae(y_true=ytrue,y_pred=ypred),
+               "mape" : mape(y_true=ytrue,y_pred=ypred),
+               "mse" : mse(y_true=ytrue,y_pred=ypred),
+               "rmse" : rmse(y_true=ytrue,y_pred=ypred),
+               "mdae" : mdae(y_true=ytrue,y_pred=ypred),
+               "r2" : r2_score(y_true=ytrue,y_pred=ypred)}
         return pd.DataFrame(res,index=["metrics"])
     
     # Estimation of ols model
     def ols_estimated(y,x,df1,df2):
         # Create formula
         formula = create_formula(y=y,x=x)
         # Train the model
@@ -175,41 +206,38 @@
         return pd.DataFrame(res,index=["metrics"])
     
     # Hosmer-Lemeshow Test
     def hosmer_lemeshow_test(ytrue,yprob):
         y_prob = pd.DataFrame(yprob)
         y_prob1 = pd.concat([y_prob, ytrue], axis =1)
         y_prob1.columns = ["prob","test"]
-        y_prob1["decile"] = pd.qcut(y_prob1.prob, 10)
+        y_prob1["decile"] = pd.qcut(y_prob1["prob"], 10)
         obsevents_pos = y_prob1['test'].groupby(y_prob1.decile).sum()
         obsevents_neg = y_prob1["prob"].groupby(y_prob1.decile).count() - obsevents_pos
         expevents_pos = y_prob1["prob"].groupby(y_prob1.decile).sum()
         expevents_neg = y_prob1["prob"].groupby(y_prob1.decile).count() - expevents_pos
         hl = ((obsevents_neg - expevents_neg)**2/expevents_neg).sum()+((obsevents_pos - expevents_pos)**2/expevents_pos).sum()
         return hl
 
     # logistic metric
-    def glm_metrics(model,null_deviance,ytrue,ypred):
-        # Null likelihood - Model likelihood
-        L0, Ln = np.exp(model.llnull), np.exp(model.llf)
-        # R2 Cox and Snell
-        r2coxsnell = 1.0 - (L0/Ln)**(2/model.nobs)
+    def glm_metrics(model,null_deviance,ytrue,yprob):
+        ypred = list(map(round, yprob))
         # Resid deviance
         resid_deviance = -2*model.llf
         res = {"r2 mcfadden":model.prsquared,
-               "r2 cox - snell" : r2coxsnell,
-               "r2 nagelkerke" : r2coxsnell/(1-L0**(2.0/model.nobs)),
+               "r2 cox - snell" : r2_coxsnell(model),
+               "r2 nagelkerke" : r2_nagelkerke(model),
                "null deviance": null_deviance,
                "resid deviance" : resid_deviance ,
                "diff deviance" : null_deviance - resid_deviance,
-               "accuracy score " : accuracy_score(ytrue,ypred),
-               "error rate" : 1.0 - accuracy_score(ytrue,ypred),
-               "recall score" : recall_score(ytrue,ypred),
-               "f1 score" : f1_score(ytrue,ypred),
-               "auc" : roc_auc_score(ytrue,ypred)}
+               "accuracy score " : accuracy_score(y_true=ytrue,y_pred=ypred),
+               "error rate" : error_rate(y_true=ytrue,y_pred=ypred),
+               "recall score" : recall_score(y_true=ytrue,y_pred=ypred),
+               "f1 score" : f1_score(y_true=ytrue,y_pred=ypred),
+               "auc" : roc_auc_score(y_true=ytrue,y_score=yprob)}
         return pd.DataFrame(res,index=["metrics"])
     
     def glm_estimated(y,x,df1,df2):
         # Create formula
         formula = create_formula(y=y,x=x)
         # Null model
         null_model = smf.logit(formula=f"{y}~1",data=df1).fit(disp=False)
@@ -222,15 +250,15 @@
         # Predict under Test dataset
         ypred = list(map(round, yprob))
         # Confusion matrix
         cm = confusion_matrix(df2[y],ypred)
         split_cm = split_confusion_matrix(cm)
         # Metrics under test sampling
         gen_metrics = general_metrics(x,model)
-        logit_metrics = glm_metrics(model,null_deviance,df2[y],ypred)
+        logit_metrics = glm_metrics(model,null_deviance,df2[y],yprob)
         return gen_metrics.join(logit_metrics).join(split_cm)
     
     # Store ols model
     def glm_model(y,x,df1):
         # Create formula
         formula = create_formula(y=y,x=x)
         # Train the model
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scientistmetrics-0.0.3/scientistmetrics.egg-info/PKG-INFO` & `scientistmetrics-0.0.4/scientistmetrics.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,91 @@
 Metadata-Version: 2.1
 Name: scientistmetrics
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python package for metrics and scoring : quantifying the quality of predictions
 Home-page: https://github.com/enfantbenidedieu/scientistmetrics
 Author: Duverier DJIFACK ZEBAZE
 Author-email: duverierdjifack@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: pandas>=2.2.2
+Requires-Dist: scikit-learn>=1.2.2
+Requires-Dist: plotnine>=0.10.1
+Requires-Dist: statsmodels>=0.14.0
+Requires-Dist: scipy>=1.10.1
 
-# scientistmetrics
+# scientistmetrics : python library for model metrics
 
 ## About scientistmetrics
 
-**scientistmetrics** is a `Python` package for calculating correlation amongst categorical variables.
+scientistmetrics is a Python package for metrics and scoring : quantifying the quality of predictions
 
 ## Why scientistmetrics?
 
-The function provides the option for computing one of six measures of association between two nominal variables from the data given in a 2d contingency table: 
-* Pearson's chi-squared test : https://en.wikipedia.org/wiki/Pearson%27s_chi-squared_test
-* Phi coefficient : https://en.wikipedia.org/wiki/Phi_coefficient
-* G-test: https://en.wikipedia.org/wiki/G-test
-* Cramer's V : https://en.wikipedia.org/wiki/Cramer's_V
-* Tschuprow's T : https://en.wikipedia.org/wiki/Tschuprow's_T
-* Pearson contingency coefficient : https://www.statisticshowto.com/contingency-coefficient/
+### Measure of association with categoricals variables
+
+scientistmetrics provides the option for computing one of six measures of association between two nominal variables from the data given in a 2d contingency table:
+
+* Chi - squard test : [https://en.wikipedia.org/wiki/Chi-squared_test](https://en.wikipedia.org/wiki/Chi-squared_test)
+* Cramer's V : [https://en.wikipedia.org/wiki/Cram%C3%A9r%27s_V](https://en.wikipedia.org/wiki/Cram%C3%A9r%27s_V)
+* Tschuprow's T : [https://en.wikipedia.org/wiki/Tschuprow%27s_T](https://en.wikipedia.org/wiki/Tschuprow%27s_T)
+* G-test : [https://en.wikipedia.org/wiki/G-test](https://en.wikipedia.org/wiki/G-test)
+* Phi coefficient : [https://en.wikipedia.org/wiki/Phi_coefficient](https://en.wikipedia.org/wiki/Phi_coefficient)
+* Pearson contingence coefficient : [https://www.statisticshowto.com/contingency-coefficient/](https://www.statisticshowto.com/contingency-coefficient/)
+
+### Classification metrics
+
+scientistmetrics provides metrics for classification problem :
+
+* accuracy score
+* f1 score
+* precision
+* recall
+* etc...
+
+### Regression metrics
+
+scientistmetrics provides metrics for regression problem :
+
+* Rsquared
+* Adjusted Rsquared
+* Mean squared error
+* etc...
+
+### Powerset model
+
+scientistmetrics provides a function that gives a set of all subsets model.
 
 Notebook is availabled.
 
 ## Installation
 
 ### Dependencies
 
 scientistmetrics requires :
 
 ```
-Python >=3.10
-Numpy >=1.23.5
-Pandas >=1.5.3
-Plotnine >=0.10.1
-Scipy >=1.10.1
+python >=3.10
+numpy >=1.26.4
+pandas >=2.2.2
+scikit-learn >=1.2.2
+plotnine >=0.10.1
+statsmodels >=0.14.0
+scipy >=1.10.1
 ```
 
 ## User installation
 
 You can install scientistmetrics using `pip` :
 
 ```
 pip install scientistmetrics
 ```
 
-## Author
-
-Duvérier DJIFACK ZEBAZE
+## Author(s)
 
+Duvérier DJIFACK ZEBAZE [duverierdjifack@gmail.com](mailto:duverierdjifack@gmail.com)
```

### Comparing `scientistmetrics-0.0.3/scientistmetricsdoc/chapter2.Rmd` & `scientistmetrics-0.0.4/scientistmetricsdoc/chapter2.Rmd`

 * *Files identical despite different names*

### Comparing `scientistmetrics-0.0.3/scientistmetricsdoc/donnee/diabetes.csv` & `scientistmetrics-0.0.4/scientistmetricsdoc/donnee/diabetes.csv`

 * *Files identical despite different names*

### Comparing `scientistmetrics-0.0.3/scientistmetricsdoc/donnee/insurance.csv` & `scientistmetrics-0.0.4/scientistmetricsdoc/donnee/insurance.csv`

 * *Files identical despite different names*

### Comparing `scientistmetrics-0.0.3/scientistmetricsdoc/main.Rmd` & `scientistmetrics-0.0.4/scientistmetricsdoc/main.Rmd`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ---
-title: "**scientistmetrics**"
-subtitle: "version $0.0.2$"
+title: "**Logistic Regression Goodness-Of-Fit using Statsmodels and Scientistmetrics**"
+subtitle: "version $0.0.3$"
 author: "Duvérier DJIFACK ZEBAZE"
 #date: "`r format(Sys.Date(), '%d %B %Y')`"
 geometry: "left=2.5cm,right=2.5cm,top=2.5cm,bottom=2.5cm, twoside=true"
 documentclass: report
 fontsize: 11pt
 line-height: 1.5
 urlcolor: blue
@@ -182,14 +182,14 @@
 ```
 
 
 
 ```{python child = "chapter1.Rmd",eval=FALSE,echo=FALSE}
 ```
 
-```{python child = "chapter2.Rmd"}
+```{python child = "chapter4.Rmd"}
 ```
```

### Comparing `scientistmetrics-0.0.3/scientistmetricsdoc/main.log` & `scientistmetrics-0.0.4/scientistmetricsdoc/main.log`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-This is XeTeX, Version 3.141592653-2.6-0.999995 (TeX Live 2023) (preloaded format=xelatex 2023.8.12)  25 AUG 2023 00:26
+This is XeTeX, Version 3.141592653-2.6-0.999995 (TeX Live 2023) (preloaded format=xelatex 2024.2.4)  28 APR 2024 16:55
 entering extended mode
  restricted \write18 enabled.
  %&-line parsing enabled.
 **main.tex
 (./main.tex
-LaTeX2e <2023-06-01> patch level 1
-L3 programming layer <2023-08-11>
+LaTeX2e <2023-11-01> patch level 1
+L3 programming layer <2024-01-22>
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/base/report.cls
 Document Class: report 2023/05/17 v1.4n Standard LaTeX document class
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/base/size11.clo
 File: size11.clo 2023/05/17 v1.4n Standard LaTeX file (size option)
 )
-\c@part=\count181
-\c@chapter=\count182
-\c@section=\count183
-\c@subsection=\count184
-\c@subsubsection=\count185
-\c@paragraph=\count186
-\c@subparagraph=\count187
-\c@figure=\count188
-\c@table=\count189
+\c@part=\count183
+\c@chapter=\count184
+\c@section=\count185
+\c@subsection=\count186
+\c@subsubsection=\count187
+\c@paragraph=\count188
+\c@subparagraph=\count189
+\c@figure=\count190
+\c@table=\count191
 \abovecaptionskip=\skip48
 \belowcaptionskip=\skip49
 \bibindent=\dimen140
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/amsmath/amsmath.sty
 Package: amsmath 2023/05/13 v2.17o AMS math features
 \@mathmargin=\skip50
 For additional information on amsmath, use the `?' option.
@@ -35,48 +35,48 @@
 \ex@=\dimen141
 )) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/amsmath/amsbsy.sty
 Package: amsbsy 1999/11/29 v1.2d Bold Symbols
 \pmbraise@=\dimen142
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/amsmath/amsopn.sty
 Package: amsopn 2022/04/08 v2.04 operator names
 )
-\inf@bad=\count190
+\inf@bad=\count192
 LaTeX Info: Redefining \frac on input line 234.
-\uproot@=\count191
-\leftroot@=\count192
+\uproot@=\count193
+\leftroot@=\count194
 LaTeX Info: Redefining \overline on input line 399.
 LaTeX Info: Redefining \colon on input line 410.
-\classnum@=\count193
-\DOTSCASE@=\count194
+\classnum@=\count195
+\DOTSCASE@=\count196
 LaTeX Info: Redefining \ldots on input line 496.
 LaTeX Info: Redefining \dots on input line 499.
 LaTeX Info: Redefining \cdots on input line 620.
 \Mathstrutbox@=\box51
 \strutbox@=\box52
 LaTeX Info: Redefining \big on input line 722.
 LaTeX Info: Redefining \Big on input line 723.
 LaTeX Info: Redefining \bigg on input line 724.
 LaTeX Info: Redefining \Bigg on input line 725.
 \big@size=\dimen143
 LaTeX Font Info:    Redeclaring font encoding OML on input line 743.
 LaTeX Font Info:    Redeclaring font encoding OMS on input line 744.
-\macc@depth=\count195
+\macc@depth=\count197
 LaTeX Info: Redefining \bmod on input line 905.
 LaTeX Info: Redefining \pmod on input line 910.
 LaTeX Info: Redefining \smash on input line 940.
 LaTeX Info: Redefining \relbar on input line 970.
 LaTeX Info: Redefining \Relbar on input line 971.
-\c@MaxMatrixCols=\count196
+\c@MaxMatrixCols=\count198
 \dotsspace@=\muskip16
-\c@parentequation=\count197
-\dspbrk@lvl=\count198
+\c@parentequation=\count199
+\dspbrk@lvl=\count266
 \tag@help=\toks18
-\row@=\count199
-\column@=\count266
-\maxfields@=\count267
+\row@=\count267
+\column@=\count268
+\maxfields@=\count269
 \andhelp@=\toks19
 \eqnshift@=\dimen144
 \alignsep@=\dimen145
 \tagshift@=\dimen146
 \tagwidth@=\dimen147
 \totwidth@=\dimen148
 \lineht@=\dimen149
@@ -91,15 +91,64 @@
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/amsfonts/amsfonts.sty
 Package: amsfonts 2013/01/14 v3.01 Basic AMSFonts support
 \symAMSa=\mathgroup4
 \symAMSb=\mathgroup5
 LaTeX Font Info:    Redeclaring math symbol \hbar on input line 98.
 LaTeX Font Info:    Overwriting math alphabet `\mathfrak' in version `bold'
 (Font)                  U/euf/m/n --> U/euf/b/n on input line 106.
-)) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/lm/lmodern.sty
+)) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/iftex/iftex.sty
+Package: iftex 2022/02/03 v1.0f TeX engine tests
+) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/unicode-math/unicode-math.sty (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/l3kernel/expl3.sty
+Package: expl3 2024-01-22 L3 programming layer (loader) 
+(c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/l3backend/l3backend-xetex.def
+File: l3backend-xetex.def 2024-01-04 L3 backend support: XeTeX
+\g__graphics_track_int=\count270
+\l__pdf_internal_box=\box53
+\g__pdf_backend_object_int=\count271
+\g__pdf_backend_annotation_int=\count272
+\g__pdf_backend_link_int=\count273
+))
+Package: unicode-math 2023/08/13 v0.8r Unicode maths in XeLaTeX and LuaLaTeX
+(c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/unicode-math/unicode-math-xetex.sty
+Package: unicode-math-xetex 2023/08/13 v0.8r Unicode maths in XeLaTeX and LuaLaTeX
+(c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/l3packages/xparse/xparse.sty
+Package: xparse 2023-10-10 L3 Experimental document command parser
+) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/l3packages/l3keys2e/l3keys2e.sty
+Package: l3keys2e 2023-10-10 LaTeX2e option processing using LaTeX3 keys
+) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/fontspec/fontspec.sty
+Package: fontspec 2022/01/15 v2.8a Font selection for XeLaTeX and LuaLaTeX
+(c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/fontspec/fontspec-xetex.sty
+Package: fontspec-xetex 2022/01/15 v2.8a Font selection for XeLaTeX and LuaLaTeX
+\l__fontspec_script_int=\count274
+\l__fontspec_language_int=\count275
+\l__fontspec_strnum_int=\count276
+\l__fontspec_tmp_int=\count277
+\l__fontspec_tmpa_int=\count278
+\l__fontspec_tmpb_int=\count279
+\l__fontspec_tmpc_int=\count280
+\l__fontspec_em_int=\count281
+\l__fontspec_emdef_int=\count282
+\l__fontspec_strong_int=\count283
+\l__fontspec_strongdef_int=\count284
+\l__fontspec_tmpa_dim=\dimen150
+\l__fontspec_tmpb_dim=\dimen151
+\l__fontspec_tmpc_dim=\dimen152
+(c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/base/fontenc.sty
+Package: fontenc 2021/04/29 v2.0v Standard LaTeX package
+) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/fontspec/fontspec.cfg))) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/base/fix-cm.sty
+Package: fix-cm 2020/11/24 v1.1t fixes to LaTeX
+(c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/base/ts1enc.def
+File: ts1enc.def 2001/06/05 v3.0e (jk/car/fm) Standard LaTeX file
+LaTeX Font Info:    Redeclaring font encoding TS1 on input line 47.
+))
+\g__um_fam_int=\count285
+\g__um_fonts_used_int=\count286
+\l__um_primecount_int=\count287
+\g__um_primekern_muskip=\muskip17
+(c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/unicode-math/unicode-math-table.tex))) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/lm/lmodern.sty
 Package: lmodern 2015/05/01 v1.6.1 Latin Modern Fonts
 LaTeX Font Info:    Overwriting symbol font `operators' in version `normal'
 (Font)                  OT1/cmr/m/n --> OT1/lmr/m/n on input line 22.
 LaTeX Font Info:    Overwriting symbol font `letters' in version `normal'
 (Font)                  OML/cmm/m/it --> OML/lmm/m/it on input line 23.
 LaTeX Font Info:    Overwriting symbol font `symbols' in version `normal'
 (Font)                  OMS/cmsy/m/n --> OMS/lmsy/m/n on input line 24.
@@ -125,64 +174,15 @@
 (Font)                  OT1/cmr/bx/n --> OT1/lmr/bx/n on input line 35.
 LaTeX Font Info:    Overwriting math alphabet `\mathsf' in version `bold'
 (Font)                  OT1/cmss/bx/n --> OT1/lmss/bx/n on input line 36.
 LaTeX Font Info:    Overwriting math alphabet `\mathit' in version `bold'
 (Font)                  OT1/cmr/bx/it --> OT1/lmr/bx/it on input line 37.
 LaTeX Font Info:    Overwriting math alphabet `\mathtt' in version `bold'
 (Font)                  OT1/cmtt/m/n --> OT1/lmtt/m/n on input line 38.
-) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/iftex/iftex.sty
-Package: iftex 2022/02/03 v1.0f TeX engine tests
-) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/unicode-math/unicode-math.sty (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/l3kernel/expl3.sty
-Package: expl3 2023-08-11 L3 programming layer (loader) 
-(c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/l3backend/l3backend-xetex.def
-File: l3backend-xetex.def 2023-04-19 L3 backend support: XeTeX
-\g__graphics_track_int=\count268
-\l__pdf_internal_box=\box53
-\g__pdf_backend_object_int=\count269
-\g__pdf_backend_annotation_int=\count270
-\g__pdf_backend_link_int=\count271
-))
-Package: unicode-math 2023/08/13 v0.8r Unicode maths in XeLaTeX and LuaLaTeX
-(c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/unicode-math/unicode-math-xetex.sty
-Package: unicode-math-xetex 2023/08/13 v0.8r Unicode maths in XeLaTeX and LuaLaTeX
-(c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/l3packages/xparse/xparse.sty
-Package: xparse 2023-02-02 L3 Experimental document command parser
-) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/l3packages/l3keys2e/l3keys2e.sty
-Package: l3keys2e 2023-02-02 LaTeX2e option processing using LaTeX3 keys
-) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/fontspec/fontspec.sty
-Package: fontspec 2022/01/15 v2.8a Font selection for XeLaTeX and LuaLaTeX
-(c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/fontspec/fontspec-xetex.sty
-Package: fontspec-xetex 2022/01/15 v2.8a Font selection for XeLaTeX and LuaLaTeX
-\l__fontspec_script_int=\count272
-\l__fontspec_language_int=\count273
-\l__fontspec_strnum_int=\count274
-\l__fontspec_tmp_int=\count275
-\l__fontspec_tmpa_int=\count276
-\l__fontspec_tmpb_int=\count277
-\l__fontspec_tmpc_int=\count278
-\l__fontspec_em_int=\count279
-\l__fontspec_emdef_int=\count280
-\l__fontspec_strong_int=\count281
-\l__fontspec_strongdef_int=\count282
-\l__fontspec_tmpa_dim=\dimen150
-\l__fontspec_tmpb_dim=\dimen151
-\l__fontspec_tmpc_dim=\dimen152
-(c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/base/fontenc.sty
-Package: fontenc 2021/04/29 v2.0v Standard LaTeX package
-) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/fontspec/fontspec.cfg))) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/base/fix-cm.sty
-Package: fix-cm 2020/11/24 v1.1t fixes to LaTeX
-(c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/base/ts1enc.def
-File: ts1enc.def 2001/06/05 v3.0e (jk/car/fm) Standard LaTeX file
-LaTeX Font Info:    Redeclaring font encoding TS1 on input line 47.
-))
-\g__um_fam_int=\count283
-\g__um_fonts_used_int=\count284
-\l__um_primecount_int=\count285
-\g__um_primekern_muskip=\muskip17
-(c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/unicode-math/unicode-math-table.tex)))
+)
 
 Package fontspec Info: Bookman Old Style scale = 0.9147002546305197.
 
 
 Package fontspec Info: Bookman Old Style scale = 0.9147002546305197.
 
 
@@ -213,15 +213,15 @@
 (fontspec)             - 'italic small caps'  (m/scit) with NFSS spec.: 
 (fontspec)             - 'bold italic' (b/it) with NFSS spec.:
 (fontspec)             <->s*[1]"Bookman Old
 (fontspec)             Style/BI/OT:language=dflt;mapping=tex-text;"
 (fontspec)             - 'bold italic small caps'  (b/scit) with NFSS spec.: 
 
 LaTeX Font Info:    Font shape `TU/BookmanOldStyle(0)/m/n' will be
-(Font)              scaled to size 10.95pt on input line 21.
+(Font)              scaled to size 10.95pt on input line 24.
 
 Package fontspec Info: Bookman Old Style scale = 0.9999970426188203.
 
 
 Package fontspec Info: Bookman Old Style scale = 0.9999970426188203.
 
 
@@ -255,73 +255,73 @@
 (fontspec)             - 'italic small caps'  (m/scit) with NFSS spec.: 
 (fontspec)             - 'bold italic' (b/it) with NFSS spec.:
 (fontspec)             <->s*[0.9207995207232722]"Bookman Old
 (fontspec)             Style/BI/OT:language=dflt;"
 (fontspec)             - 'bold italic small caps'  (b/scit) with NFSS spec.: 
 
 LaTeX Font Info:    Overwriting math alphabet `\mathrm' in version `normal'
-(Font)                  OT1/lmr/m/n --> TU/BookmanOldStyle(1)/m/n on input line 21.
+(Font)                  OT1/lmr/m/n --> TU/BookmanOldStyle(1)/m/n on input line 24.
 LaTeX Font Info:    Overwriting math alphabet `\mathit' in version `normal'
-(Font)                  OT1/lmr/m/it --> TU/BookmanOldStyle(1)/m/it on input line 21.
+(Font)                  OT1/lmr/m/it --> TU/BookmanOldStyle(1)/m/it on input line 24.
 LaTeX Font Info:    Overwriting math alphabet `\mathbf' in version `normal'
-(Font)                  OT1/lmr/bx/n --> TU/BookmanOldStyle(1)/b/n on input line 21.
+(Font)                  OT1/lmr/bx/n --> TU/BookmanOldStyle(1)/b/n on input line 24.
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/upquote/upquote.sty
 Package: upquote 2012/04/19 v1.3 upright-quote and grave-accent glyphs in verbatim
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/base/textcomp.sty
 Package: textcomp 2020/02/02 v2.0n Standard LaTeX package
 )) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/xcolor/xcolor.sty
-Package: xcolor 2022/06/12 v2.14 LaTeX color extensions (UK)
+Package: xcolor 2023/11/15 v3.01 LaTeX color extensions (UK)
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/graphics-cfg/color.cfg
 File: color.cfg 2016/01/02 v1.6 sample color configuration
 )
-Package xcolor Info: Driver file: xetex.def on input line 227.
+Package xcolor Info: Driver file: xetex.def on input line 274.
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/graphics-def/xetex.def
 File: xetex.def 2022/09/22 v5.0n Graphics/color driver for xetex
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/graphics/mathcolor.ltx)
-Package xcolor Info: Model `cmy' substituted by `cmy0' on input line 1353.
-Package xcolor Info: Model `RGB' extended on input line 1369.
-Package xcolor Info: Model `HTML' substituted by `rgb' on input line 1371.
-Package xcolor Info: Model `Hsb' substituted by `hsb' on input line 1372.
-Package xcolor Info: Model `tHsb' substituted by `hsb' on input line 1373.
-Package xcolor Info: Model `HSB' substituted by `hsb' on input line 1374.
-Package xcolor Info: Model `Gray' substituted by `gray' on input line 1375.
-Package xcolor Info: Model `wave' substituted by `hsb' on input line 1376.
-(c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/graphics/dvipsnam.def
+Package xcolor Info: Model `cmy' substituted by `cmy0' on input line 1350.
+Package xcolor Info: Model `RGB' extended on input line 1366.
+Package xcolor Info: Model `HTML' substituted by `rgb' on input line 1368.
+Package xcolor Info: Model `Hsb' substituted by `hsb' on input line 1369.
+Package xcolor Info: Model `tHsb' substituted by `hsb' on input line 1370.
+Package xcolor Info: Model `HSB' substituted by `hsb' on input line 1371.
+Package xcolor Info: Model `Gray' substituted by `gray' on input line 1372.
+Package xcolor Info: Model `wave' substituted by `hsb' on input line 1373.
+) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/graphics/dvipsnam.def
 File: dvipsnam.def 2016/06/17 v3.0m Driver-dependent file (DPC,SPQR)
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/xcolor/svgnam.def
-File: svgnam.def 2022/06/12 v2.14 Predefined colors according to SVG 1.1 (UK)
+File: svgnam.def 2023/11/15 v3.01 Predefined colors according to SVG 1.1 (UK)
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/xcolor/x11nam.def
-File: x11nam.def 2022/06/12 v2.14 Predefined colors according to Unix/X11 (UK)
-)) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/geometry/geometry.sty
+File: x11nam.def 2023/11/15 v3.01 Predefined colors according to Unix/X11 (UK)
+) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/geometry/geometry.sty
 Package: geometry 2020/01/02 v5.9 Page Geometry
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/graphics/keyval.sty
 Package: keyval 2022/05/29 v1.15 key=value parser (DPC)
 \KV@toks@=\toks22
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/iftex/ifvtex.sty
 Package: ifvtex 2019/10/25 v1.7 ifvtex legacy package. Use iftex instead.
 )
-\Gm@cnth=\count286
-\Gm@cntv=\count287
-\c@Gm@tempcnt=\count288
+\Gm@cnth=\count288
+\Gm@cntv=\count289
+\c@Gm@tempcnt=\count290
 \Gm@bindingoffset=\dimen153
 \Gm@wd@mp=\dimen154
 \Gm@odd@mp=\dimen155
 \Gm@even@mp=\dimen156
 \Gm@layoutwidth=\dimen157
 \Gm@layoutheight=\dimen158
 \Gm@layouthoffset=\dimen159
 \Gm@layoutvoffset=\dimen160
 \Gm@dimlist=\toks23
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/fancyvrb/fancyvrb.sty
-Package: fancyvrb 2023/01/19 4.5a verbatim text (tvz,hv)
-\FV@CodeLineNo=\count289
+Package: fancyvrb 2024/01/20 4.5c verbatim text (tvz,hv)
+\FV@CodeLineNo=\count291
 \FV@InFile=\read2
 \FV@TabBox=\box54
-\c@FancyVerbLine=\count290
-\FV@StepNumber=\count291
+\c@FancyVerbLine=\count292
+\FV@StepNumber=\count293
 \FV@OutFile=\write3
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/framed/framed.sty
 Package: framed 2011/10/22 v 0.96: framed or shaded text with page breaks
 \OuterFrameSep=\skip53
 \fb@frw=\dimen161
 \fb@frh=\dimen162
 \FrameRule=\dimen163
@@ -338,90 +338,90 @@
 Package graphics Info: Driver file: xetex.def on input line 107.
 )
 \Gin@req@height=\dimen165
 \Gin@req@width=\dimen166
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/pbox/pbox.sty
 Package: pbox 2011/12/07 v1.2 Dynamic parboxes
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/tools/calc.sty
-Package: calc 2017/05/25 v4.3 Infix arithmetic (KKT,FJ)
-\calc@Acount=\count292
-\calc@Bcount=\count293
+Package: calc 2023/07/08 v4.3 Infix arithmetic (KKT,FJ)
+\calc@Acount=\count294
+\calc@Bcount=\count295
 \calc@Adimen=\dimen167
 \calc@Bdimen=\dimen168
 \calc@Askip=\skip54
 \calc@Bskip=\skip55
 LaTeX Info: Redefining \setlength on input line 80.
 LaTeX Info: Redefining \addtolength on input line 81.
-\calc@Ccount=\count294
+\calc@Ccount=\count296
 \calc@Cskip=\skip56
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/base/ifthen.sty
 Package: ifthen 2022/04/13 v1.1d Standard LaTeX ifthen package (DPC)
 )
 \pb@xlen=\skip57
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/caption/caption.sty
-Package: caption 2023/07/31 v3.6n Customizing captions (AR)
+Package: caption 2023/08/05 v3.6o Customizing captions (AR)
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/caption/caption3.sty
 Package: caption3 2023/07/31 v2.4d caption3 kernel (AR)
 \caption@tempdima=\dimen169
 \captionmargin=\dimen170
 \caption@leftmargin=\dimen171
 \caption@rightmargin=\dimen172
 \caption@width=\dimen173
 \caption@indent=\dimen174
 \caption@parindent=\dimen175
 \caption@hangindent=\dimen176
 Package caption Info: Standard document class detected.
 )
-\c@caption@flags=\count295
-\c@continuedfloat=\count296
+\c@caption@flags=\count297
+\c@continuedfloat=\count298
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/natbib/natbib.sty
 Package: natbib 2010/09/13 8.31b (PWD, AO)
 \bibhang=\skip58
 \bibsep=\skip59
 LaTeX Info: Redefining \cite on input line 694.
-\c@NAT@ctr=\count297
+\c@NAT@ctr=\count299
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/base/inputenc.sty
 Package: inputenc 2021/02/14 v1.3d Input encoding file
 \inpenc@prehook=\toks24
 \inpenc@posthook=\toks25
 
 Package inputenc Warning: inputenc package ignored with utf8 based engines.
 
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/babel/babel.sty
-Package: babel 2023/07/15 v3.92 The Babel package
-\babel@savecnt=\count298
+Package: babel 2024/01/07 v24.1 The Babel package
+\babel@savecnt=\count300
 \U@D=\dimen177
 \l@unhyphenated=\language4
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/babel/xebabel.def)
 \bbl@readstream=\read3
-\bbl@dirlevel=\count299
+\bbl@dirlevel=\count301
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/babel-french/french.ldf
-Language: french 2023/03/08 v3.5q French support from the babel system
+Language: french 2023-12-19 v3.5r French support from the babel system
 Package babel Info: Hyphen rules for 'acadian' set to \l@french
 (babel)             (\language3). Reported on input line 91.
 Package babel Info: Hyphen rules for 'canadien' set to \l@french
 (babel)             (\language3). Reported on input line 92.
-\FB@nonchar=\count300
+\FB@stdchar=\count302
 Package french.ldf Info: No need for active punctuation characters
 (french.ldf)             with this version of XeTeX!
-(french.ldf)             reported on input line 310.
-\FB@punctthick=\XeTeXcharclass1
-\FB@punctthin=\XeTeXcharclass2
-\FB@punctnul=\XeTeXcharclass3
-\FB@guilo=\XeTeXcharclass4
-\FB@guilf=\XeTeXcharclass5
-\FB@guilnul=\XeTeXcharclass6
-\FBguill@level=\count301
+(french.ldf)             reported on input line 311.
+\FB@punctthick=\XeTeXcharclass4
+\FB@punctthin=\XeTeXcharclass5
+\FB@punctnul=\XeTeXcharclass6
+\FB@guilo=\XeTeXcharclass7
+\FB@guilf=\XeTeXcharclass8
+\FB@guilnul=\XeTeXcharclass9
+\FBguill@level=\count303
 \FBold@everypar=\toks26
 \FB@Mht=\dimen178
-\mc@charclass=\count302
-\mc@charfam=\count303
-\mc@charslot=\count304
-\std@mcc=\count305
-\dec@mcc=\count306
+\mc@charclass=\count304
+\mc@charfam=\count305
+\mc@charslot=\count306
+\std@mcc=\count307
+\dec@mcc=\count308
 \FB@parskip=\dimen179
 \listindentFB=\dimen180
 \descindentFB=\dimen181
 \labelindentFB=\dimen182
 \labelwidthFB=\dimen183
 \leftmarginFB=\dimen184
 \parindentFFN=\dimen185
@@ -460,34 +460,34 @@
 Package minitoc Info: I0031
 (minitoc)             ==> this version is configured for UNIX-like 
 (minitoc)                 (long extensions) file names.
 \openout4 = `main.mtc'.
 
 \openout4 = `main.mtc0'.
 
-\c@mtc=\count307
-\c@minitocdepth=\count308
-\c@ptc=\count309
-\c@parttocdepth=\count310
+\c@mtc=\count309
+\c@minitocdepth=\count310
+\c@ptc=\count311
+\c@parttocdepth=\count312
 \ptcindent=\skip62
 Package minitoc Info: I0010
 (minitoc)             The english language is selected.
 (minitoc)              on input line 4910.
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/minitoc/english.mld
 File: english.mld 2006/01/13
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/minitoc/english.mld
 File: english.mld 2006/01/13
 ))
 Package minitoc Info: I0013
 (minitoc)             \mtcsetdepth redefines the counter 
-(minitoc)             "minitocdepth" as "1" on input line 106.
+(minitoc)             "minitocdepth" as "1" on input line 109.
 Package minitoc Info: I0017
 (minitoc)             \mtcsettitle redefines the macro 
 (minitoc)             "mtctitle" as 
-(minitoc)             "Sommaire" on input line 107.
+(minitoc)             "Sommaire" on input line 110.
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/diagbox/diagbox.sty
 Package: diagbox 2020/02/09 v2.3 Making table heads with diagonal lines
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/pict2e/pict2e.sty
 Package: pict2e 2020/09/30 v0.4b Improved picture commands (HjG,RN,JT)
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/pict2e/pict2e.cfg
 File: pict2e.cfg 2016/02/05 v0.1u pict2e configuration for teTeX/TeXLive
 )
@@ -502,15 +502,15 @@
 \pIIe@tempdima=\dimen189
 \pIIe@tempdimb=\dimen190
 \pIIe@tempdimc=\dimen191
 \pIIe@tempdimd=\dimen192
 \pIIe@tempdime=\dimen193
 \pIIe@tempdimf=\dimen194
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/tools/array.sty
-Package: array 2022/09/04 v2.5g Tabular extension package (FMi)
+Package: array 2023/10/16 v2.5g Tabular extension package (FMi)
 \col@sep=\dimen195
 \ar@mcellbox=\box57
 \extrarowheight=\dimen196
 \NC@list=\toks29
 \extratabsurround=\skip63
 \backup@length=\skip64
 \ar@cellbox=\box58
@@ -521,29 +521,29 @@
 \diagbox@wd=\dimen197
 \diagbox@ht=\dimen198
 \diagbox@insepl=\dimen199
 \diagbox@insepr=\dimen256
 \diagbox@outsepl=\dimen257
 \diagbox@outsepr=\dimen258
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/lettrine/lettrine.sty
-File: lettrine.sty 2023-08-14 v2.52 (Daniel Flipo)
+File: lettrine.sty 2024-01-20 v2.60 (Daniel Flipo)
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/l3packages/xfp/xfp.sty
-Package: xfp 2023-02-02 L3 Floating point unit
+Package: xfp 2023-10-10 L3 Floating point unit
 )
-\c@DefaultLines=\count311
-\c@DefaultDepth=\count312
+\c@DefaultLines=\count313
+\c@DefaultDepth=\count314
 \DefaultFindent=\dimen259
 \DefaultNindent=\dimen260
 \DefaultSlope=\dimen261
 \DiscardVskip=\dimen262
 \L@lettrine=\box62
 \L@lbox=\box63
 \L@tbox=\box64
-\c@L@lines=\count313
-\c@L@depth=\count314
+\c@L@lines=\count315
+\c@L@depth=\count316
 \L@Pindent=\dimen263
 \L@Findent=\dimen264
 \L@Nindent=\dimen265
 \L@lraise=\dimen266
 \L@first=\dimen267
 \L@next=\dimen268
 \L@slope=\dimen269
@@ -567,90 +567,90 @@
 \belowrulesep=\dimen282
 \belowbottomsep=\dimen283
 \aboverulesep=\dimen284
 \abovetopsep=\dimen285
 \cmidrulesep=\dimen286
 \cmidrulekern=\dimen287
 \defaultaddspace=\dimen288
-\@cmidla=\count315
-\@cmidlb=\count316
+\@cmidla=\count317
+\@cmidlb=\count318
 \@aboverulesep=\dimen289
 \@belowrulesep=\dimen290
-\@thisruleclass=\count317
-\@lastruleclass=\count318
+\@thisruleclass=\count319
+\@lastruleclass=\count320
 \@thisrulewidth=\dimen291
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/threeparttable/threeparttable.sty
 Package: threeparttable 2003/06/13  v 3.0
 \@tempboxb=\box65
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/tools/longtable.sty
-Package: longtable 2021-09-01 v4.17 Multi-page Table package (DPC)
+Package: longtable 2023-11-01 v4.19 Multi-page Table package (DPC)
 \LTleft=\skip65
 \LTright=\skip66
 \LTpre=\skip67
 \LTpost=\skip68
-\LTchunksize=\count319
+\LTchunksize=\count321
 \LTcapwidth=\dimen292
 \LT@head=\box66
 \LT@firsthead=\box67
 \LT@foot=\box68
 \LT@lastfoot=\box69
 \LT@gbox=\box70
-\LT@cols=\count320
-\LT@rows=\count321
-\c@LT@tables=\count322
-\c@LT@chunks=\count323
+\LT@cols=\count322
+\LT@rows=\count323
+\c@LT@tables=\count324
+\c@LT@chunks=\count325
 \LT@p@ftn=\toks31
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/multirow/multirow.sty
 Package: multirow 2021/03/15 v2.8 Span multiple rows of a table
 \multirow@colwidth=\skip69
-\multirow@cntb=\count324
+\multirow@cntb=\count326
 \multirow@dima=\skip70
 \bigstrutjot=\dimen293
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/wrapfig/wrapfig.sty
 \wrapoverhang=\dimen294
 \WF@size=\dimen295
-\c@WF@wrappedlines=\count325
+\c@WF@wrappedlines=\count327
 \WF@box=\box71
 \WF@everypar=\toks32
 Package: wrapfig 2003/01/31  v 3.6
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/float/float.sty
 Package: float 2001/11/08 v1.3d Float enhancements (AL)
-\c@float@type=\count326
+\c@float@type=\count328
 \float@exts=\toks33
 \float@box=\box72
 \@float@everytoks=\toks34
 \@floatcapt=\box73
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/colortbl/colortbl.sty
 Package: colortbl 2022/06/20 v1.0f Color table columns (DPC)
 \everycr=\toks35
 \minrowclearance=\skip71
-\rownum=\count327
+\rownum=\count329
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/pdflscape/pdflscape.sty
 Package: pdflscape 2022-10-27 v0.13 Display of landscape pages in PDF
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/pdflscape/pdflscape-nometadata.sty
 Package: pdflscape-nometadata 2022-10-28 v0.13 Display of landscape pages in PDF (HO)
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/graphics/lscape.sty
 Package: lscape 2020/05/28 v3.02 Landscape Pages (DPC)
 )
 Package pdflscape Info: Auto-detected driver: dvipdfm (xetex) on input line 98.
 )) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/tabu/tabu.sty
 Package: tabu 2019/01/11 v2.9 - flexible LaTeX tabulars (FC+tabu-fixed)
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/varwidth/varwidth.sty
 Package: varwidth 2009/03/30 ver 0.92;  Variable-width minipages
 \@vwid@box=\box74
-\sift@deathcycles=\count328
+\sift@deathcycles=\count330
 \@vwid@loff=\dimen296
 \@vwid@roff=\dimen297
 )
-\c@taburow=\count329
-\tabu@nbcols=\count330
-\tabu@cnt=\count331
-\tabu@Xcol=\count332
-\tabu@alloc=\count333
-\tabu@nested=\count334
+\c@taburow=\count331
+\tabu@nbcols=\count332
+\tabu@cnt=\count333
+\tabu@Xcol=\count334
+\tabu@alloc=\count335
+\tabu@nested=\count336
 \tabu@target=\dimen298
 \tabu@spreadtarget=\dimen299
 \tabu@naturalX=\dimen300
 \tabucolX=\dimen301
 \tabu@Xsum=\dimen302
 \extrarowdepth=\dimen303
 \abovetabulinesep=\dimen304
@@ -673,23 +673,23 @@
 \TPTL@width=\skip73
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/ulem/ulem.sty
 \UL@box=\box79
 \UL@hyphenbox=\box80
 \UL@skip=\skip74
 \UL@hook=\toks38
 \UL@height=\dimen307
-\UL@pe=\count335
+\UL@pe=\count337
 \UL@pixel=\dimen308
 \ULC@box=\box81
 Package: ulem 2019/11/18
 \ULdepth=\dimen309
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/makecell/makecell.sty
 Package: makecell 2009/08/03 V0.1e Managing of Tab Column Heads and Cells
 \rotheadsize=\dimen310
-\c@nlinenum=\count336
+\c@nlinenum=\count338
 \TeXr@lab=\toks39
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/fncychap/fncychap.sty
 Package: fncychap 2007/07/30 v1.34 LaTeX package (Revised chapters)
 \RW=\skip75
 \mylen=\skip76
 \myhi=\skip77
 \px=\skip78
@@ -756,33 +756,33 @@
 
 Package geometry Warning: Over-specification in `v'-direction.
     `height' (682.86613pt) is ignored.
 
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/exercises/exercises.sty
 Package: exercises 2000/05/17 v1.1 .dtx exercises file
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/tools/verbatim.sty
-Package: verbatim 2022-07-02 v1.5u LaTeX2e package for verbatim enhancements
+Package: verbatim 2023-11-06 v1.5v LaTeX2e package for verbatim enhancements
 \every@verbatim=\toks40
 \verbatim@line=\toks41
 \verbatim@in@stream=\read4
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/kvoptions/kvoptions.sty
 Package: kvoptions 2022-06-15 v3.15 Key value format for package options (HO)
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/ltxcmds/ltxcmds.sty
-Package: ltxcmds 2020-05-10 v1.25 LaTeX kernel commands for general use (HO)
+Package: ltxcmds 2023-12-04 v1.26 LaTeX kernel commands for general use (HO)
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/kvsetkeys/kvsetkeys.sty
 Package: kvsetkeys 2022-10-05 v1.19 Key value parser (HO)
 )) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/marginnote/marginnote.sty
-Package: marginnote 2018/08/09 v1.4b non floating margin notes for LaTeX
-\c@mn@abspage=\count337
+Package: marginnote 2018/08/09 1.4b non floating margin notes for LaTeX
+\c@mn@abspage=\count339
 )
-\c@exercises@totalpoints=\count338
-\c@exercises@finaltotalpoints=\count339
-\c@exercises@exercisenumber=\count340
-\c@exercises@solutionnumber=\count341
-\c@i=\count342
+\c@exercises@totalpoints=\count340
+\c@exercises@finaltotalpoints=\count341
+\c@exercises@exercisenumber=\count342
+\c@exercises@solutionnumber=\count343
+\c@i=\count344
 \exercises@parskipsave=\skip91
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/pgf/frontendlayer/tikz.sty (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/pgf/basiclayer/pgf.sty (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/pgf/utilities/pgfrcs.sty (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/utilities/pgfutil-common.tex
 \pgfutil@everybye=\toks42
 \pgfutil@tempdima=\dimen311
 \pgfutil@tempdimb=\dimen312
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/utilities/pgfutil-latex.def
 \pgfutil@abb=\box82
@@ -806,51 +806,51 @@
 \pgf@yb=\dimen318
 \pgf@xc=\dimen319
 \pgf@yc=\dimen320
 \pgf@xd=\dimen321
 \pgf@yd=\dimen322
 \w@pgf@writea=\write5
 \r@pgf@reada=\read5
-\c@pgf@counta=\count343
-\c@pgf@countb=\count344
-\c@pgf@countc=\count345
-\c@pgf@countd=\count346
+\c@pgf@counta=\count345
+\c@pgf@countb=\count346
+\c@pgf@countc=\count347
+\c@pgf@countd=\count348
 \t@pgf@toka=\toks46
 \t@pgf@tokb=\toks47
 \t@pgf@tokc=\toks48
-\pgf@sys@id@count=\count347
+\pgf@sys@id@count=\count349
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/systemlayer/pgf.cfg
 File: pgf.cfg 2023-01-15 v3.1.10 (3.1.10)
 )
 Driver file for pgf: pgfsys-xetex.def
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/systemlayer/pgfsys-xetex.def
 File: pgfsys-xetex.def 2023-01-15 v3.1.10 (3.1.10)
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/systemlayer/pgfsys-dvipdfmx.def
 File: pgfsys-dvipdfmx.def 2023-01-15 v3.1.10 (3.1.10)
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/systemlayer/pgfsys-common-pdf.def
 File: pgfsys-common-pdf.def 2023-01-15 v3.1.10 (3.1.10)
 )
-\pgfsys@objnum=\count348
+\pgfsys@objnum=\count350
 ))) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/systemlayer/pgfsyssoftpath.code.tex
 File: pgfsyssoftpath.code.tex 2023-01-15 v3.1.10 (3.1.10)
-\pgfsyssoftpath@smallbuffer@items=\count349
-\pgfsyssoftpath@bigbuffer@items=\count350
+\pgfsyssoftpath@smallbuffer@items=\count351
+\pgfsyssoftpath@bigbuffer@items=\count352
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/systemlayer/pgfsysprotocol.code.tex
 File: pgfsysprotocol.code.tex 2023-01-15 v3.1.10 (3.1.10)
 )) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/basiclayer/pgfcore.code.tex
 Package: pgfcore 2023-01-15 v3.1.10 (3.1.10)
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/math/pgfmath.code.tex (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/math/pgfmathutil.code.tex) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/math/pgfmathparser.code.tex
 \pgfmath@dimen=\dimen323
-\pgfmath@count=\count351
+\pgfmath@count=\count353
 \pgfmath@box=\box83
 \pgfmath@toks=\toks49
 \pgfmath@stack@operand=\toks50
 \pgfmath@stack@operation=\toks51
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/math/pgfmathfunctions.code.tex) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/math/pgfmathfunctions.basic.code.tex) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/math/pgfmathfunctions.trigonometric.code.tex) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/math/pgfmathfunctions.random.code.tex) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/math/pgfmathfunctions.comparison.code.tex) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/math/pgfmathfunctions.base.code.tex) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/math/pgfmathfunctions.round.code.tex) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/math/pgfmathfunctions.misc.code.tex) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/math/pgfmathfunctions.integerarithmetics.code.tex) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/math/pgfmathcalc.code.tex) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/math/pgfmathfloat.code.tex
-\c@pgfmathroundto@lastzeros=\count352
+\c@pgfmathroundto@lastzeros=\count354
 )) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/math/pgfint.code.tex) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/basiclayer/pgfcorepoints.code.tex
 File: pgfcorepoints.code.tex 2023-01-15 v3.1.10 (3.1.10)
 \pgf@picminx=\dimen324
 \pgf@picmaxx=\dimen325
 \pgf@picminy=\dimen326
 \pgf@picmaxy=\dimen327
 \pgf@pathminx=\dimen328
@@ -872,15 +872,15 @@
 \pgf@shorten@end@additional=\dimen340
 \pgf@shorten@start@additional=\dimen341
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/basiclayer/pgfcorescopes.code.tex
 File: pgfcorescopes.code.tex 2023-01-15 v3.1.10 (3.1.10)
 \pgfpic=\box84
 \pgf@hbox=\box85
 \pgf@layerbox@main=\box86
-\pgf@picture@serial@count=\count353
+\pgf@picture@serial@count=\count355
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/basiclayer/pgfcoregraphicstate.code.tex
 File: pgfcoregraphicstate.code.tex 2023-01-15 v3.1.10 (3.1.10)
 \pgflinewidth=\dimen342
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/basiclayer/pgfcoretransformations.code.tex
 File: pgfcoretransformations.code.tex 2023-01-15 v3.1.10 (3.1.10)
 \pgf@pt@x=\dimen343
 \pgf@pt@y=\dimen344
@@ -893,16 +893,16 @@
 File: pgfcorepathprocessing.code.tex 2023-01-15 v3.1.10 (3.1.10)
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/basiclayer/pgfcorearrows.code.tex
 File: pgfcorearrows.code.tex 2023-01-15 v3.1.10 (3.1.10)
 \pgfarrowsep=\dimen346
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/basiclayer/pgfcoreshade.code.tex
 File: pgfcoreshade.code.tex 2023-01-15 v3.1.10 (3.1.10)
 \pgf@max=\dimen347
-\pgf@sys@shading@range@num=\count354
-\pgf@shadingcount=\count355
+\pgf@sys@shading@range@num=\count356
+\pgf@shadingcount=\count357
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/basiclayer/pgfcoreimage.code.tex
 File: pgfcoreimage.code.tex 2023-01-15 v3.1.10 (3.1.10)
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/basiclayer/pgfcoreexternal.code.tex
 File: pgfcoreexternal.code.tex 2023-01-15 v3.1.10 (3.1.10)
 \pgfexternal@startupbox=\box87
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/basiclayer/pgfcorelayers.code.tex
 File: pgfcorelayers.code.tex 2023-01-15 v3.1.10 (3.1.10)
@@ -929,183 +929,181 @@
 \pgffor@skip=\dimen351
 \pgffor@stack=\toks52
 \pgffor@toks=\toks53
 )) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/frontendlayer/tikz/tikz.code.tex
 Package: tikz 2023-01-15 v3.1.10 (3.1.10)
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/libraries/pgflibraryplothandlers.code.tex
 File: pgflibraryplothandlers.code.tex 2023-01-15 v3.1.10 (3.1.10)
-\pgf@plot@mark@count=\count356
+\pgf@plot@mark@count=\count358
 \pgfplotmarksize=\dimen352
 )
 \tikz@lastx=\dimen353
 \tikz@lasty=\dimen354
 \tikz@lastxsaved=\dimen355
 \tikz@lastysaved=\dimen356
 \tikz@lastmovetox=\dimen357
 \tikz@lastmovetoy=\dimen358
 \tikzleveldistance=\dimen359
 \tikzsiblingdistance=\dimen360
 \tikz@figbox=\box89
 \tikz@figbox@bg=\box90
 \tikz@tempbox=\box91
 \tikz@tempbox@bg=\box92
-\tikztreelevel=\count357
-\tikznumberofchildren=\count358
-\tikznumberofcurrentchild=\count359
-\tikz@fig@count=\count360
+\tikztreelevel=\count359
+\tikznumberofchildren=\count360
+\tikznumberofcurrentchild=\count361
+\tikz@fig@count=\count362
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/modules/pgfmodulematrix.code.tex
 File: pgfmodulematrix.code.tex 2023-01-15 v3.1.10 (3.1.10)
-\pgfmatrixcurrentrow=\count361
-\pgfmatrixcurrentcolumn=\count362
-\pgf@matrix@numberofcolumns=\count363
+\pgfmatrixcurrentrow=\count363
+\pgfmatrixcurrentcolumn=\count364
+\pgf@matrix@numberofcolumns=\count365
 )
-\tikz@expandcount=\count364
+\tikz@expandcount=\count366
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pgf/frontendlayer/tikz/libraries/tikzlibrarytopaths.code.tex
 File: tikzlibrarytopaths.code.tex 2023-01-15 v3.1.10 (3.1.10)
 ))) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/base/flafter.sty
 Package: flafter 2021/07/31 v1.4e Standard LaTeX floats after reference (FMi)
 Applying: [2015/01/01] float order in 2-column on input line 49.
 Already applied: [0000/00/00] float order in 2-column on input line 151.
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/hyperref/hyperref.sty
-Package: hyperref 2023-07-08 v7.01b Hypertext links for LaTeX
+Package: hyperref 2024-01-20 v7.01h Hypertext links for LaTeX
+(c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/kvdefinekeys/kvdefinekeys.sty
+Package: kvdefinekeys 2019-12-19 v1.6 Define keys (HO)
+) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pdfescape/pdfescape.sty
+Package: pdfescape 2019/12/09 v1.15 Implements pdfTeX's escape features (HO)
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pdftexcmds/pdftexcmds.sty
 Package: pdftexcmds 2020-06-27 v0.33 Utility functions of pdfTeX for LuaTeX (HO)
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/infwarerr/infwarerr.sty
 Package: infwarerr 2019/12/03 v1.5 Providing info/warning/error messages (HO)
 )
 Package pdftexcmds Info: \pdf@primitive is available.
 Package pdftexcmds Info: \pdf@ifprimitive is available.
 Package pdftexcmds Info: \pdfdraftmode not found.
-) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/kvdefinekeys/kvdefinekeys.sty
-Package: kvdefinekeys 2019-12-19 v1.6 Define keys (HO)
-) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/pdfescape/pdfescape.sty
-Package: pdfescape 2019/12/09 v1.15 Implements pdfTeX's escape features (HO)
-) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/hycolor/hycolor.sty
+)) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/hycolor/hycolor.sty
 Package: hycolor 2020-01-27 v1.10 Color options for hyperref/bookmark (HO)
-) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/letltxmacro/letltxmacro.sty
-Package: letltxmacro 2019/12/03 v1.6 Let assignment for LaTeX macros (HO)
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/auxhook/auxhook.sty
 Package: auxhook 2019-12-17 v1.6 Hooks for auxiliary files (HO)
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/hyperref/nameref.sty
-Package: nameref 2023-08-07 v2.53 Cross-referencing by name of section
+Package: nameref 2023-11-26 v2.56 Cross-referencing by name of section
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/refcount/refcount.sty
 Package: refcount 2019/12/15 v3.6 Data extraction from label references (HO)
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/gettitlestring/gettitlestring.sty
 Package: gettitlestring 2019/12/15 v1.6 Cleanup title references (HO)
 )
-\c@section@level=\count365
+\c@section@level=\count367
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/etoolbox/etoolbox.sty
 Package: etoolbox 2020/10/05 v2.5k e-TeX tools for LaTeX (JAW)
-\etb@tempcnta=\count366
+\etb@tempcnta=\count368
 )
 \@linkdim=\dimen361
-\Hy@linkcounter=\count367
-\Hy@pagecounter=\count368
+\Hy@linkcounter=\count369
+\Hy@pagecounter=\count370
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/hyperref/pd1enc.def
-File: pd1enc.def 2023-07-08 v7.01b Hyperref: PDFDocEncoding definition (HO)
+File: pd1enc.def 2024-01-20 v7.01h Hyperref: PDFDocEncoding definition (HO)
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/intcalc/intcalc.sty
 Package: intcalc 2019/12/15 v1.3 Expandable calculations with integers (HO)
 )
-\Hy@SavedSpaceFactor=\count369
+\Hy@SavedSpaceFactor=\count371
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/hyperref/puenc.def
-File: puenc.def 2023-07-08 v7.01b Hyperref: PDF Unicode definition (HO)
+File: puenc.def 2024-01-20 v7.01h Hyperref: PDF Unicode definition (HO)
 )
-Package hyperref Info: Option `unicode' set `true' on input line 4050.
-Package hyperref Info: Hyper figures OFF on input line 4167.
-Package hyperref Info: Link nesting OFF on input line 4172.
-Package hyperref Info: Hyper index ON on input line 4175.
-Package hyperref Info: Plain pages OFF on input line 4182.
-Package hyperref Info: Backreferencing OFF on input line 4187.
+Package hyperref Info: Option `unicode' set `true' on input line 4062.
+Package hyperref Info: Hyper figures OFF on input line 4179.
+Package hyperref Info: Link nesting OFF on input line 4184.
+Package hyperref Info: Hyper index ON on input line 4187.
+Package hyperref Info: Plain pages OFF on input line 4194.
+Package hyperref Info: Backreferencing OFF on input line 4199.
 Package hyperref Info: Implicit mode ON; LaTeX internals redefined.
-Package hyperref Info: Bookmarks ON on input line 4434.
-\c@Hy@tempcnt=\count370
+Package hyperref Info: Bookmarks ON on input line 4446.
+\c@Hy@tempcnt=\count372
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/url/url.sty
 \Urlmuskip=\muskip18
 Package: url 2013/09/16  ver 3.4  Verb mode for urls, etc.
 )
-LaTeX Info: Redefining \url on input line 4772.
+LaTeX Info: Redefining \url on input line 4784.
 \XeTeXLinkMargin=\dimen362
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/bitset/bitset.sty
 Package: bitset 2019/12/09 v1.3 Handle bit-vector datatype (HO)
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/bigintcalc/bigintcalc.sty
 Package: bigintcalc 2019/12/15 v1.5 Expandable calculations on big integers (HO)
 ))
-\Fld@menulength=\count371
+\Fld@menulength=\count373
 \Field@Width=\dimen363
 \Fld@charsize=\dimen364
-Package hyperref Info: Hyper figures OFF on input line 6051.
-Package hyperref Info: Link nesting OFF on input line 6056.
-Package hyperref Info: Hyper index ON on input line 6059.
-Package hyperref Info: backreferencing OFF on input line 6066.
-Package hyperref Info: Link coloring OFF on input line 6071.
-Package hyperref Info: Link coloring with OCG OFF on input line 6076.
-Package hyperref Info: PDF/A mode OFF on input line 6081.
+Package hyperref Info: Hyper figures OFF on input line 6063.
+Package hyperref Info: Link nesting OFF on input line 6068.
+Package hyperref Info: Hyper index ON on input line 6071.
+Package hyperref Info: backreferencing OFF on input line 6078.
+Package hyperref Info: Link coloring OFF on input line 6083.
+Package hyperref Info: Link coloring with OCG OFF on input line 6088.
+Package hyperref Info: PDF/A mode OFF on input line 6093.
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/base/atbegshi-ltx.sty
 Package: atbegshi-ltx 2021/01/10 v1.0c Emulation of the original atbegshi
 package with kernel methods
 )
-\Hy@abspage=\count372
-\c@Item=\count373
-\c@Hfootnote=\count374
+\Hy@abspage=\count374
+\c@Item=\count375
+\c@Hfootnote=\count376
 )
 Package hyperref Info: Driver (autodetected): hxetex.
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/hyperref/hxetex.def
-File: hxetex.def 2023-07-08 v7.01b Hyperref driver for XeTeX
+File: hxetex.def 2024-01-20 v7.01h Hyperref driver for XeTeX
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/stringenc/stringenc.sty
 Package: stringenc 2019/11/29 v1.12 Convert strings between diff. encodings (HO)
 )
 \pdfm@box=\box93
-\c@Hy@AnnotLevel=\count375
-\HyField@AnnotCount=\count376
-\Fld@listcount=\count377
-\c@bookmark@seq@number=\count378
+\c@Hy@AnnotLevel=\count377
+\HyField@AnnotCount=\count378
+\Fld@listcount=\count379
+\c@bookmark@seq@number=\count380
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/rerunfilecheck/rerunfilecheck.sty
 Package: rerunfilecheck 2022-07-10 v1.10 Rerun checks for auxiliary files (HO)
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/base/atveryend-ltx.sty
 Package: atveryend-ltx 2020/08/19 v1.0a Emulation of the original atveryend package
 with kernel methods
 ) (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/generic/uniquecounter/uniquecounter.sty
 Package: uniquecounter 2019/12/15 v1.4 Provide unlimited unique counter (HO)
 )
 Package uniquecounter Info: New unique counter `rerunfilecheck' on input line 285.
 )
 \Hy@SectionHShift=\skip92
 )
-Package hyperref Info: Option `colorlinks' set `true' on input line 166.
+Package hyperref Info: Option `colorlinks' set `true' on input line 169.
 (./main.aux)
 \openout1 = `main.aux'.
 
-LaTeX Font Info:    Checking defaults for OML/cmm/m/it on input line 179.
-LaTeX Font Info:    ... okay on input line 179.
-LaTeX Font Info:    Checking defaults for OMS/cmsy/m/n on input line 179.
-LaTeX Font Info:    ... okay on input line 179.
-LaTeX Font Info:    Checking defaults for OT1/cmr/m/n on input line 179.
-LaTeX Font Info:    ... okay on input line 179.
-LaTeX Font Info:    Checking defaults for T1/cmr/m/n on input line 179.
-LaTeX Font Info:    ... okay on input line 179.
-LaTeX Font Info:    Checking defaults for TS1/cmr/m/n on input line 179.
-LaTeX Font Info:    ... okay on input line 179.
-LaTeX Font Info:    Checking defaults for TU/lmr/m/n on input line 179.
-LaTeX Font Info:    ... okay on input line 179.
-LaTeX Font Info:    Checking defaults for OMX/cmex/m/n on input line 179.
-LaTeX Font Info:    ... okay on input line 179.
-LaTeX Font Info:    Checking defaults for U/cmr/m/n on input line 179.
-LaTeX Font Info:    ... okay on input line 179.
-LaTeX Font Info:    Checking defaults for PD1/pdf/m/n on input line 179.
-LaTeX Font Info:    ... okay on input line 179.
-LaTeX Font Info:    Checking defaults for PU/pdf/m/n on input line 179.
-LaTeX Font Info:    ... okay on input line 179.
+LaTeX Font Info:    Checking defaults for OML/cmm/m/it on input line 183.
+LaTeX Font Info:    ... okay on input line 183.
+LaTeX Font Info:    Checking defaults for OMS/cmsy/m/n on input line 183.
+LaTeX Font Info:    ... okay on input line 183.
+LaTeX Font Info:    Checking defaults for OT1/cmr/m/n on input line 183.
+LaTeX Font Info:    ... okay on input line 183.
+LaTeX Font Info:    Checking defaults for T1/cmr/m/n on input line 183.
+LaTeX Font Info:    ... okay on input line 183.
+LaTeX Font Info:    Checking defaults for TS1/cmr/m/n on input line 183.
+LaTeX Font Info:    ... okay on input line 183.
+LaTeX Font Info:    Checking defaults for TU/lmr/m/n on input line 183.
+LaTeX Font Info:    ... okay on input line 183.
+LaTeX Font Info:    Checking defaults for OMX/cmex/m/n on input line 183.
+LaTeX Font Info:    ... okay on input line 183.
+LaTeX Font Info:    Checking defaults for U/cmr/m/n on input line 183.
+LaTeX Font Info:    ... okay on input line 183.
+LaTeX Font Info:    Checking defaults for PD1/pdf/m/n on input line 183.
+LaTeX Font Info:    ... okay on input line 183.
+LaTeX Font Info:    Checking defaults for PU/pdf/m/n on input line 183.
+LaTeX Font Info:    ... okay on input line 183.
 LaTeX Font Info:    Overwriting math alphabet `\mathsf' in version `normal'
-(Font)                  OT1/lmss/m/n --> TU/lmss/m/n on input line 179.
+(Font)                  OT1/lmss/m/n --> TU/lmss/m/n on input line 183.
 LaTeX Font Info:    Overwriting math alphabet `\mathsf' in version `bold'
-(Font)                  OT1/lmss/bx/n --> TU/lmss/b/n on input line 179.
+(Font)                  OT1/lmss/bx/n --> TU/lmss/b/n on input line 183.
 LaTeX Font Info:    Overwriting math alphabet `\mathtt' in version `normal'
-(Font)                  OT1/lmtt/m/n --> TU/lmtt/m/n on input line 179.
+(Font)                  OT1/lmtt/m/n --> TU/lmtt/m/n on input line 183.
 LaTeX Font Info:    Overwriting math alphabet `\mathtt' in version `bold'
-(Font)                  OT1/lmtt/m/n --> TU/lmtt/b/n on input line 179.
+(Font)                  OT1/lmtt/m/n --> TU/lmtt/b/n on input line 183.
 
 Package fontspec Info: latinmodern-math scale = 1.093247546840395.
 
 
 Package fontspec Info: latinmodern-math scale = 1.093247546840395.
 
 
@@ -1123,15 +1121,15 @@
 (fontspec)             <->s*[1.093247546840395]"[latinmodern-math.otf]/OT:script=math;language=dflt;"
 (fontspec)             - 'small caps'  (m/sc) with NFSS spec.: 
 (fontspec)             - 'bold' (b/n) with NFSS spec.:
 (fontspec)             <->s*[1.093247546840395]"[latinmodern-math.otf]/OT:script=math;language=dflt;"
 (fontspec)             - 'bold small caps'  (b/sc) with NFSS spec.: 
 
 LaTeX Font Info:    Font shape `TU/latinmodern-math.otf(0)/m/n' will be
-(Font)              scaled to size 11.97104pt on input line 179.
+(Font)              scaled to size 11.97104pt on input line 183.
 
 Package fontspec Info: latinmodern-math scale = 1.093247546840395.
 
 
 Package fontspec Info: latinmodern-math scale = 1.093247546840395.
 
 
@@ -1155,23 +1153,23 @@
 (fontspec)             <9.3075->s*[1.093247546840395]"[latinmodern-math.otf]/OT:script=math;language=dflt;"<6.57-9.3075>s*[1.093247546840395]"[latinmodern-math.otf]/OT:script=math;language=dflt;+ssty=0;"<-6.57>s*[1.093247546840395]"[latinmodern-math.otf]/OT:script=math;language=dflt;+ssty=1;"
 (fontspec)             - 'small caps'  (m/sc) with NFSS spec.: 
 (fontspec)             - 'bold' (b/n) with NFSS spec.:
 (fontspec)             <->s*[1.093247546840395]"[latinmodern-math.otf]/OT:script=math;language=dflt;"
 (fontspec)             - 'bold small caps'  (b/sc) with NFSS spec.: 
 
 LaTeX Font Info:    Font shape `TU/latinmodern-math.otf(1)/m/n' will be
-(Font)              scaled to size 11.97104pt on input line 179.
+(Font)              scaled to size 11.97104pt on input line 183.
 LaTeX Font Info:    Encoding `OT1' has changed to `TU' for symbol font
-(Font)              `operators' in the math version `normal' on input line 179.
+(Font)              `operators' in the math version `normal' on input line 183.
 LaTeX Font Info:    Overwriting symbol font `operators' in version `normal'
-(Font)                  OT1/lmr/m/n --> TU/latinmodern-math.otf(1)/m/n on input line 179.
+(Font)                  OT1/lmr/m/n --> TU/latinmodern-math.otf(1)/m/n on input line 183.
 LaTeX Font Info:    Encoding `OT1' has changed to `TU' for symbol font
-(Font)              `operators' in the math version `bold' on input line 179.
+(Font)              `operators' in the math version `bold' on input line 183.
 LaTeX Font Info:    Overwriting symbol font `operators' in version `bold'
-(Font)                  OT1/lmr/bx/n --> TU/latinmodern-math.otf(1)/b/n on input line 179.
+(Font)                  OT1/lmr/bx/n --> TU/latinmodern-math.otf(1)/b/n on input line 183.
 
 Package fontspec Info: latinmodern-math scale = 1.093247546840395.
 
 
 Package fontspec Info: latinmodern-math scale = 1.093356871595079.
 
 
@@ -1242,21 +1240,21 @@
 (fontspec)             =3.45963pt\relax \fontdimen 16\font =2.95685pt\relax
 (fontspec)             \fontdimen 17\font =2.95685pt\relax \fontdimen 18\font
 (fontspec)             =2.99277pt\relax \fontdimen 19\font =2.39421pt\relax
 (fontspec)             \fontdimen 22\font =2.99277pt\relax \fontdimen 20\font
 (fontspec)             =0pt\relax \fontdimen 21\font =0pt\relax 
 
 LaTeX Font Info:    Encoding `OMS' has changed to `TU' for symbol font
-(Font)              `symbols' in the math version `normal' on input line 179.
+(Font)              `symbols' in the math version `normal' on input line 183.
 LaTeX Font Info:    Overwriting symbol font `symbols' in version `normal'
-(Font)                  OMS/lmsy/m/n --> TU/latinmodern-math.otf(2)/m/n on input line 179.
+(Font)                  OMS/lmsy/m/n --> TU/latinmodern-math.otf(2)/m/n on input line 183.
 LaTeX Font Info:    Encoding `OMS' has changed to `TU' for symbol font
-(Font)              `symbols' in the math version `bold' on input line 179.
+(Font)              `symbols' in the math version `bold' on input line 183.
 LaTeX Font Info:    Overwriting symbol font `symbols' in version `bold'
-(Font)                  OMS/lmsy/b/n --> TU/latinmodern-math.otf(2)/b/n on input line 179.
+(Font)                  OMS/lmsy/b/n --> TU/latinmodern-math.otf(2)/b/n on input line 183.
 
 Package fontspec Info: latinmodern-math scale = 1.093247546840395.
 
 
 Package fontspec Info: latinmodern-math scale = 1.093138222085711.
 
 
@@ -1309,21 +1307,21 @@
 (fontspec)             and font adjustment code:
 (fontspec)             \fontdimen 8\font =0.47884pt\relax \fontdimen 9\font
 (fontspec)             =2.39421pt\relax \fontdimen 10\font =1.99916pt\relax
 (fontspec)             \fontdimen 11\font =1.32878pt\relax \fontdimen 12\font
 (fontspec)             =7.18262pt\relax \fontdimen 13\font =0pt\relax 
 
 LaTeX Font Info:    Encoding `OMX' has changed to `TU' for symbol font
-(Font)              `largesymbols' in the math version `normal' on input line 179.
+(Font)              `largesymbols' in the math version `normal' on input line 183.
 LaTeX Font Info:    Overwriting symbol font `largesymbols' in version `normal'
-(Font)                  OMX/lmex/m/n --> TU/latinmodern-math.otf(3)/m/n on input line 179.
+(Font)                  OMX/lmex/m/n --> TU/latinmodern-math.otf(3)/m/n on input line 183.
 LaTeX Font Info:    Encoding `OMX' has changed to `TU' for symbol font
-(Font)              `largesymbols' in the math version `bold' on input line 179.
+(Font)              `largesymbols' in the math version `bold' on input line 183.
 LaTeX Font Info:    Overwriting symbol font `largesymbols' in version `bold'
-(Font)                  OMX/lmex/m/n --> TU/latinmodern-math.otf(3)/b/n on input line 179.
+(Font)                  OMX/lmex/m/n --> TU/latinmodern-math.otf(3)/b/n on input line 183.
 *geometry* driver: auto-detecting
 *geometry* detected driver: xetex
 *geometry* verbose mode - [ preamble ] result:
 * driver: xetex
 * paper: a4paper
 * layout: <same size as paper>
 * layoutoffset:(h,v)=(0.0pt,0.0pt)
@@ -1361,15 +1359,15 @@
 Package caption Info: longtable package is loaded.
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/caption/ltcaption.sty
 Package: ltcaption 2021/01/08 v1.4c longtable captions (AR)
 )
 Package caption Info: threeparttable package is loaded.
 Package caption Info: wrapfig package is loaded.
 Package caption Info: End \AtBeginDocument code.
-LaTeX Info: Redefining \up on input line 179.
+LaTeX Info: Redefining \up on input line 183.
 Package minitoc(hints) Info: I0049
 (minitoc(hints))             ==> You requested the hints option. 
 (minitoc(hints))             Some hints are eventually given below.
 
 Package minitoc(hints) Warning: W0030
 (minitoc(hints))                --- The \part command is altered 
 (minitoc(hints))                after minitoc.
@@ -1385,82 +1383,82 @@
 (minitoc(hints))                after minitoc.
 
 
 Package minitoc(hints) Warning: W0023
 (minitoc(hints))                --- It may be the consequence 
 (minitoc(hints))                of loading the ``hyperref'' package.
 
-Package hyperref Info: Link coloring ON on input line 179.
+Package hyperref Info: Link coloring ON on input line 183.
 (./main.out) (./main.out)
 \@outlinefile=\write6
 \openout6 = `main.out'.
 
 LaTeX Font Info:    Font shape `TU/BookmanOldStyle(0)/m/n' will be
-(Font)              scaled to size 17.28pt on input line 181.
+(Font)              scaled to size 17.28pt on input line 185.
 LaTeX Font Info:    Font shape `TU/BookmanOldStyle(0)/b/n' will be
-(Font)              scaled to size 17.28pt on input line 181.
+(Font)              scaled to size 17.28pt on input line 185.
 LaTeX Font Info:    Font shape `TU/BookmanOldStyle(0)/m/n' will be
-(Font)              scaled to size 12.0pt on input line 181.
+(Font)              scaled to size 12.0pt on input line 185.
 LaTeX Font Info:    Font shape `TU/latinmodern-math.otf(1)/m/n' will be
-(Font)              scaled to size 13.11896pt on input line 181.
+(Font)              scaled to size 13.11896pt on input line 185.
 LaTeX Font Info:    Font shape `TU/latinmodern-math.otf(1)/m/n' will be
-(Font)              scaled to size 8.74597pt on input line 181.
+(Font)              scaled to size 8.74597pt on input line 185.
 LaTeX Font Info:    Font shape `TU/latinmodern-math.otf(1)/m/n' will be
-(Font)              scaled to size 6.55948pt on input line 181.
-LaTeX Font Info:    Trying to load font information for OML+lmm on input line 181.
+(Font)              scaled to size 6.55948pt on input line 185.
+LaTeX Font Info:    Trying to load font information for OML+lmm on input line 185.
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/lm/omllmm.fd
 File: omllmm.fd 2015/05/01 v1.6.1 Font defs for Latin Modern
 )
 LaTeX Font Info:    Font shape `TU/latinmodern-math.otf(2)/m/n' will be
-(Font)              scaled to size 13.12024pt on input line 181.
+(Font)              scaled to size 13.12024pt on input line 185.
 LaTeX Font Info:    Font shape `TU/latinmodern-math.otf(2)/m/n' will be
-(Font)              scaled to size 8.74683pt on input line 181.
+(Font)              scaled to size 8.74683pt on input line 185.
 LaTeX Font Info:    Font shape `TU/latinmodern-math.otf(2)/m/n' will be
-(Font)              scaled to size 6.56012pt on input line 181.
+(Font)              scaled to size 6.56012pt on input line 185.
 LaTeX Font Info:    Font shape `TU/latinmodern-math.otf(3)/m/n' will be
-(Font)              scaled to size 13.11768pt on input line 181.
+(Font)              scaled to size 13.11768pt on input line 185.
 LaTeX Font Info:    Font shape `TU/latinmodern-math.otf(3)/m/n' will be
-(Font)              scaled to size 8.74512pt on input line 181.
+(Font)              scaled to size 8.74512pt on input line 185.
 LaTeX Font Info:    Font shape `TU/latinmodern-math.otf(3)/m/n' will be
-(Font)              scaled to size 6.55884pt on input line 181.
-LaTeX Font Info:    Trying to load font information for U+msa on input line 181.
+(Font)              scaled to size 6.55884pt on input line 185.
+LaTeX Font Info:    Trying to load font information for U+msa on input line 185.
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/amsfonts/umsa.fd
 File: umsa.fd 2013/01/14 v3.01 AMS symbols A
 )
-LaTeX Font Info:    Trying to load font information for U+msb on input line 181.
+LaTeX Font Info:    Trying to load font information for U+msb on input line 185.
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/amsfonts/umsb.fd
 File: umsb.fd 2013/01/14 v3.01 AMS symbols B
 ) [1
 
 ]
-\c@exemple=\count379
-\c@proposition=\count380
-\c@propriete=\count381
-\c@definition=\count382
-\c@remarque=\count383
-\c@exercice=\count384
-\c@theoreme=\count385
-\c@hypothese=\count386
+\c@exemple=\count381
+\c@proposition=\count382
+\c@propriete=\count383
+\c@definition=\count384
+\c@remarque=\count385
+\c@exercice=\count386
+\c@theoreme=\count387
+\c@hypothese=\count388
 Package minitoc Info: I0013
 (minitoc)             \mtcsetdepth redefines the counter 
-(minitoc)             "minitocdepth" as "1" on input line 204.
+(minitoc)             "minitocdepth" as "1" on input line 208.
 Package minitoc Info: I0017
 (minitoc)             \mtcsettitle redefines the macro 
 (minitoc)             "mtctitle" as 
-(minitoc)             "Sommaire" on input line 205.
+(minitoc)             "Sommaire" on input line 209.
 Package minitoc Info: I0024
-(minitoc)             PREPARING MINITOCS FROM main.toc on input line 212.
+(minitoc)             PREPARING MINITOCS FROM main.toc on input line 216.
 Package minitoc Info: I0033
 (minitoc)             Writing main.mtc1.
 \openout4 = `main.mtc1'.
 
 LaTeX Font Info:    Font shape `TU/BookmanOldStyle(0)/m/n' will be
-(Font)              scaled to size 14.4pt on input line 216.
+(Font)              scaled to size 14.4pt on input line 220.
 
-Overfull \hbox (16.78712pt too wide) in paragraph at lines 216--216
+Overfull \hbox (16.78712pt too wide) in paragraph at lines 220--220
 [][][][][][][]  
  []
 
 (./main.toc
 LaTeX Font Info:    Font shape `TU/BookmanOldStyle(0)/b/n' will be
 (Font)              scaled to size 10.95pt on input line 2.
 LaTeX Font Info:    Font shape `TU/latinmodern-math.otf(1)/m/n' will be
@@ -1491,73 +1489,239 @@
 (marginnote)                Note, it is not recommended to use consecutive
 (marginnote)                odd pages in a double-ended document.
 (marginnote)                The pages of your document should always
 (marginnote)                be a sequence: odd-even-odd-even-...
 (marginnote)                Maybe you've forgotten a \cleardoublepage before
 (marginnote)                changing the page numbering on page i.
 
-Package marginnote Info: Using workaround for absolute page number on input line 218.
+Package marginnote Info: Using workaround for absolute page number on input line 222.
 Chapitre 1.
-LaTeX Font Info:    Trying to load font information for OT1+pzc on input line 229.
+LaTeX Font Info:    Trying to load font information for OT1+pzc on input line 233.
 (c:/Users/duver/AppData/Roaming/TinyTeX/texmf-dist/tex/latex/psnfss/ot1pzc.fd
 File: ot1pzc.fd 2020/03/25 font definitions for OT1/pzc.
 )
 LaTeX Font Info:    Font shape `OT1/pzc/m/n' in size <76> not available
-(Font)              Font shape `OT1/pzc/m/it' tried instead on input line 229.
+(Font)              Font shape `OT1/pzc/m/it' tried instead on input line 233.
 
-Overfull \hbox (10.0pt too wide) in paragraph at lines 229--229
+Overfull \hbox (10.0pt too wide) in paragraph at lines 233--233
 [][][][][][][][][]  
  []
 
-LaTeX Font Info:    Font shape `TU/BookmanOldStyle(0)/b/n' will be
-(Font)              scaled to size 14.4pt on input line 229.
 
-Overfull \hbox (16.78712pt too wide) in paragraph at lines 229--229
+Overfull \hbox (16.78712pt too wide) in paragraph at lines 233--233
 [][][][][][][]  
  []
 
-LaTeX Font Info:    Font shape `TU/BookmanOldStyle(0)/b/n' will be
-(Font)              scaled to size 12.0pt on input line 240.
+\openout4 = `main.mtc'.
 
-Package hyperref Warning: Suppressing link with empty target on input line 245.
+\openout4 = `main.mtc'.
 
-LaTeX Font Info:    Font shape `TU/lmtt/bx/n' in size <10.95> not available
-(Font)              Font shape `TU/lmtt/b/n' tried instead on input line 255.
+LaTeX Font Info:    Font shape `TU/BookmanOldStyle(0)/m/n' will be
+(Font)              scaled to size 10.0pt on input line 234.
+LaTeX Font Info:    Font shape `TU/latinmodern-math.otf(1)/m/n' will be
+(Font)              scaled to size 10.93246pt on input line 234.
+LaTeX Font Info:    Font shape `TU/latinmodern-math.otf(1)/m/n' will be
+(Font)              scaled to size 7.65273pt on input line 234.
+LaTeX Font Info:    Font shape `TU/latinmodern-math.otf(1)/m/n' will be
+(Font)              scaled to size 5.46623pt on input line 234.
+LaTeX Font Info:    Font shape `TU/latinmodern-math.otf(2)/m/n' will be
+(Font)              scaled to size 10.93353pt on input line 234.
+LaTeX Font Info:    Font shape `TU/latinmodern-math.otf(2)/m/n' will be
+(Font)              scaled to size 7.65347pt on input line 234.
+LaTeX Font Info:    Font shape `TU/latinmodern-math.otf(2)/m/n' will be
+(Font)              scaled to size 5.46677pt on input line 234.
+LaTeX Font Info:    Font shape `TU/latinmodern-math.otf(3)/m/n' will be
+(Font)              scaled to size 10.9314pt on input line 234.
+LaTeX Font Info:    Font shape `TU/latinmodern-math.otf(3)/m/n' will be
+(Font)              scaled to size 7.65198pt on input line 234.
+LaTeX Font Info:    Font shape `TU/latinmodern-math.otf(3)/m/n' will be
+(Font)              scaled to size 5.4657pt on input line 234.
+LaTeX Font Info:    Font shape `TU/BookmanOldStyle(0)/b/n' will be
+(Font)              scaled to size 12.0pt on input line 234.
+(./main.mtc1
+LaTeX Font Info:    Font shape `TU/BookmanOldStyle(0)/b/n' will be
+(Font)              scaled to size 10.0pt on input line 1.
+)
+LaTeX Font Info:    Font shape `TU/BookmanOldStyle(0)/b/n' will be
+(Font)              scaled to size 14.4pt on input line 239.
 [1
 
 ]
 
 Package marginnote Warning: Consecutive odd pages found.
 (marginnote)                Note, it is not recommended to use consecutive
 (marginnote)                odd pages in a double-ended document.
 (marginnote)                The pages of your document should always
 (marginnote)                be a sequence: odd-even-odd-even-...
 (marginnote)                Maybe you've forgotten a \cleardoublepage before
 (marginnote)                changing the page numbering on page 1.
 
-Package marginnote Info: Using workaround for absolute page number on input line 282.
+Package marginnote Info: Using workaround for absolute page number on input line 272.
+LaTeX Font Info:    Font shape `TU/lmtt/bx/n' in size <10.95> not available
+(Font)              Font shape `TU/lmtt/b/n' tried instead on input line 328.
 
 Package fancyhdr Warning: \headheight is too small (12.0pt): 
 (fancyhdr)                Make it at least 13.59999pt, for example:
 (fancyhdr)                \setlength{\headheight}{13.59999pt}.
 (fancyhdr)                You might also make \topmargin smaller to compensate:
 (fancyhdr)                \addtolength{\topmargin}{-1.59999pt}.
 
 [2]
+
+Package hyperref Warning: Token not allowed in a PDF string (Unicode):
+(hyperref)                removing `math shift' on input line 357.
+
+
+Package hyperref Warning: Token not allowed in a PDF string (Unicode):
+(hyperref)                removing `superscript' on input line 357.
+
+
+Package hyperref Warning: Token not allowed in a PDF string (Unicode):
+(hyperref)                removing `math shift' on input line 357.
+
+LaTeX Font Info:    Font shape `TU/BookmanOldStyle(0)/m/n' will be
+(Font)              scaled to size 7.665pt on input line 371.
+LaTeX Font Info:    Font shape `TU/BookmanOldStyle(0)/m/n' will be
+(Font)              scaled to size 5.475pt on input line 371.
+LaTeX Font Info:    Font shape `TU/BookmanOldStyle(1)/m/n' will be
+(Font)              scaled to size 10.95pt on input line 395.
+LaTeX Font Info:    Font shape `TU/BookmanOldStyle(1)/m/n' will be
+(Font)              scaled to size 7.665pt on input line 395.
+LaTeX Font Info:    Font shape `TU/BookmanOldStyle(1)/m/n' will be
+(Font)              scaled to size 5.475pt on input line 395.
+
+Package fancyhdr Warning: \headheight is too small (12.0pt): 
+(fancyhdr)                Make it at least 13.59999pt, for example:
+(fancyhdr)                \setlength{\headheight}{13.59999pt}.
+(fancyhdr)                You might also make \topmargin smaller to compensate:
+(fancyhdr)                \addtolength{\topmargin}{-1.59999pt}.
+
+[3]
+
+Package fancyhdr Warning: \headheight is too small (12.0pt): 
+(fancyhdr)                Make it at least 13.59999pt, for example:
+(fancyhdr)                \setlength{\headheight}{13.59999pt}.
+(fancyhdr)                You might also make \topmargin smaller to compensate:
+(fancyhdr)                \addtolength{\topmargin}{-1.59999pt}.
+
+[4]
+
+Package fancyhdr Warning: \headheight is too small (12.0pt): 
+(fancyhdr)                Make it at least 13.59999pt, for example:
+(fancyhdr)                \setlength{\headheight}{13.59999pt}.
+(fancyhdr)                You might also make \topmargin smaller to compensate:
+(fancyhdr)                \addtolength{\topmargin}{-1.59999pt}.
+
+[5]
+File: ./images/cm-matrix.png Graphic file (type bmp)
+<./images/cm-matrix.png>
+
+LaTeX Font Warning: Font shape `TU/BookmanOldStyle(0)/m/sc' undefined
+(Font)              using `TU/BookmanOldStyle(0)/m/n' instead on input line 590.
+
+LaTeX Font Info:    Font shape `TU/BookmanOldStyle(0)/m/n' will be
+(Font)              scaled to size 8.0pt on input line 590.
+LaTeX Font Info:    Font shape `TU/BookmanOldStyle(0)/b/n' will be
+(Font)              scaled to size 8.0pt on input line 590.
+
+LaTeX Font Warning: Font shape `TU/BookmanOldStyle(0)/b/sc' undefined
+(Font)              using `TU/BookmanOldStyle(0)/b/n' instead on input line 590.
+
+LaTeX Font Info:    Font shape `TU/BookmanOldStyle(0)/m/sc' will be
+(Font)              scaled to size 10.95pt on input line 590.
+LaTeX Font Info:    Font shape `TU/BookmanOldStyle(0)/b/sc' will be
+(Font)              scaled to size 8.0pt on input line 590.
+
+Package fancyhdr Warning: \headheight is too small (12.0pt): 
+(fancyhdr)                Make it at least 13.59999pt, for example:
+(fancyhdr)                \setlength{\headheight}{13.59999pt}.
+(fancyhdr)                You might also make \topmargin smaller to compensate:
+(fancyhdr)                \addtolength{\topmargin}{-1.59999pt}.
+
+[6]
+
+Package fancyhdr Warning: \headheight is too small (12.0pt): 
+(fancyhdr)                Make it at least 13.59999pt, for example:
+(fancyhdr)                \setlength{\headheight}{13.59999pt}.
+(fancyhdr)                You might also make \topmargin smaller to compensate:
+(fancyhdr)                \addtolength{\topmargin}{-1.59999pt}.
+
+[7]
+
+Package fancyhdr Warning: \headheight is too small (12.0pt): 
+(fancyhdr)                Make it at least 13.59999pt, for example:
+(fancyhdr)                \setlength{\headheight}{13.59999pt}.
+(fancyhdr)                You might also make \topmargin smaller to compensate:
+(fancyhdr)                \addtolength{\topmargin}{-1.59999pt}.
+
+[8]
+
+Package fancyhdr Warning: \headheight is too small (12.0pt): 
+(fancyhdr)                Make it at least 13.59999pt, for example:
+(fancyhdr)                \setlength{\headheight}{13.59999pt}.
+(fancyhdr)                You might also make \topmargin smaller to compensate:
+(fancyhdr)                \addtolength{\topmargin}{-1.59999pt}.
+
+[9]
+File: main_files/figure-latex/unnamed-chunk-26-1.pdf Graphic file (type pdf)
+<use main_files/figure-latex/unnamed-chunk-26-1.pdf>
+LaTeX Font Info:    Font shape `TU/BookmanOldStyle(0)/m/it' will be
+(Font)              scaled to size 10.95pt on input line 855.
+
+Package fancyhdr Warning: \headheight is too small (12.0pt): 
+(fancyhdr)                Make it at least 13.59999pt, for example:
+(fancyhdr)                \setlength{\headheight}{13.59999pt}.
+(fancyhdr)                You might also make \topmargin smaller to compensate:
+(fancyhdr)                \addtolength{\topmargin}{-1.59999pt}.
+
+[10]
+
+Package fancyhdr Warning: \headheight is too small (12.0pt): 
+(fancyhdr)                Make it at least 13.59999pt, for example:
+(fancyhdr)                \setlength{\headheight}{13.59999pt}.
+(fancyhdr)                You might also make \topmargin smaller to compensate:
+(fancyhdr)                \addtolength{\topmargin}{-1.59999pt}.
+
+[11]
+
+Package fancyhdr Warning: \headheight is too small (12.0pt): 
+(fancyhdr)                Make it at least 13.59999pt, for example:
+(fancyhdr)                \setlength{\headheight}{13.59999pt}.
+(fancyhdr)                You might also make \topmargin smaller to compensate:
+(fancyhdr)                \addtolength{\topmargin}{-1.59999pt}.
+
+[12]
+LaTeX Font Info:    Font shape `TU/BookmanOldStyle(1)/m/n' will be
+(Font)              scaled to size 12.0pt on input line 1004.
+LaTeX Font Info:    Font shape `TU/BookmanOldStyle(1)/m/n' will be
+(Font)              scaled to size 8.0pt on input line 1004.
+LaTeX Font Info:    Font shape `TU/BookmanOldStyle(1)/m/n' will be
+(Font)              scaled to size 6.0pt on input line 1004.
+
+Package hyperref Warning: Token not allowed in a PDF string (Unicode):
+(hyperref)                removing `math shift' on input line 1004.
+
+
+Package hyperref Warning: Token not allowed in a PDF string (Unicode):
+(hyperref)                removing `math shift' on input line 1004.
+
+
+Package fancyhdr Warning: \headheight is too small (12.0pt): 
+(fancyhdr)                Make it at least 13.59999pt, for example:
+(fancyhdr)                \setlength{\headheight}{13.59999pt}.
+(fancyhdr)                You might also make \topmargin smaller to compensate:
+(fancyhdr)                \addtolength{\topmargin}{-1.59999pt}.
+
+[13]
 Package minitoc Info: I0009
 (minitoc)             Listing minitoc auxiliary files. 
 (minitoc)             Creating the main.maf file.
 \openout4 = `main.maf'.
 
 
-Package minitoc(hints) Warning: W0078
-(minitoc(hints))                You have used \dominitoc, 
-(minitoc(hints))                but not \minitoc.
-
-
 Package minitoc(hints) Warning: W0086
 (minitoc(hints))                The fncychap package should be 
 (minitoc(hints))                loaded BEFORE the minitoc package.
 
 Package minitoc(hints) Info: I0053
 (minitoc(hints))             You have loaded the float package; 
 (minitoc(hints))             please be aware that the minitoc package 
@@ -1571,25 +1735,28 @@
 
 Package fancyhdr Warning: \headheight is too small (12.0pt): 
 (fancyhdr)                Make it at least 13.59999pt, for example:
 (fancyhdr)                \setlength{\headheight}{13.59999pt}.
 (fancyhdr)                You might also make \topmargin smaller to compensate:
 (fancyhdr)                \addtolength{\topmargin}{-1.59999pt}.
 
-[3] (./main.aux)
+[14] (./main.aux)
  ***********
-LaTeX2e <2023-06-01> patch level 1
-L3 programming layer <2023-08-11>
+LaTeX2e <2023-11-01> patch level 1
+L3 programming layer <2024-01-22>
  ***********
+
+LaTeX Font Warning: Some font shapes were not available, defaults substituted.
+
 Package rerunfilecheck Info: File `main.out' has not changed.
-(rerunfilecheck)             Checksum: B9B0295EE9EE3EABB95F564D2BEEB0FF;500.
+(rerunfilecheck)             Checksum: 9CEC90D13278DFA3B806B0688D603357;1441.
  ) 
 Here is how much of TeX's memory you used:
- 35993 strings out of 477825
- 692032 string characters out of 5820236
- 1936879 words of memory out of 5000000
- 56319 multiletter control sequences out of 15000+600000
- 565252 words of font info for 105 fonts, out of 8000000 for 9000
+ 36155 strings out of 476864
+ 697196 string characters out of 5802875
+ 1936630 words of memory out of 5000000
+ 57415 multiletter control sequences out of 15000+600000
+ 568258 words of font info for 136 fonts, out of 8000000 for 9000
  14 hyphenation exceptions out of 8191
- 90i,11n,132p,414b,539s stack positions out of 10000i,1000n,20000p,200000b,200000s
+ 90i,12n,132p,414b,522s stack positions out of 10000i,1000n,20000p,200000b,200000s
 
-Output written on main.pdf (5 pages).
+Output written on main.pdf (16 pages).
```

### Comparing `scientistmetrics-0.0.3/setup.py` & `scientistmetrics-0.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # -*- coding: utf-8 -*-
-"""
-@author: enfantbenidedieu
-"""
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="scientistmetrics", 
-    version="0.0.3",
+    version="0.0.4",
     author="Duverier DJIFACK ZEBAZE",
     author_email="duverierdjifack@gmail.com",
     description="Python package for metrics and scoring : quantifying the quality of predictions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/enfantbenidedieu/scientistmetrics",
     packages=setuptools.find_packages(),
+    install_requires=["numpy>=1.26.4",
+                      "pandas>=2.2.2",
+                      "scikit-learn>=1.2.2",
+                      "plotnine>=0.10.1",
+                      "statsmodels>=0.14.0",
+                      "scipy>=1.10.1"],
+    python_requires=">=3.10",
+    include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
-    ],
-    python_requires='>=3.10',
+    ]
 )
```


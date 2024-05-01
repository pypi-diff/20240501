# Comparing `tmp/stepcount-3.5.0.tar.gz` & `tmp/stepcount-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stepcount-3.5.0.tar", last modified: Fri Apr 26 19:11:28 2024, max compression
+gzip compressed data, was "stepcount-3.6.0.tar", last modified: Wed May  1 06:45:58 2024, max compression
```

## Comparing `stepcount-3.5.0.tar` & `stepcount-3.6.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:11:28.266127 stepcount-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-04-26 19:11:19.000000 stepcount-3.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-04-26 19:11:28.258127 stepcount-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-26 19:11:19.000000 stepcount-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-26 19:11:19.000000 stepcount-3.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 19:11:28.266127 stepcount-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-26 19:11:19.000000 stepcount-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:11:28.254127 stepcount-3.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:11:28.266127 stepcount-3.5.0/src/stepcount/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-26 19:11:19.000000 stepcount-3.5.0/src/stepcount/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-26 19:11:28.266127 stepcount-3.5.0/src/stepcount/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-04-26 19:11:19.000000 stepcount-3.5.0/src/stepcount/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     9731 2024-04-26 19:11:19.000000 stepcount-3.5.0/src/stepcount/hmm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23588 2024-04-26 19:11:19.000000 stepcount-3.5.0/src/stepcount/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-04-26 19:11:19.000000 stepcount-3.5.0/src/stepcount/sslmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    23965 2024-04-26 19:11:19.000000 stepcount-3.5.0/src/stepcount/stepcount.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:11:28.258127 stepcount-3.5.0/src/stepcount/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-26 19:11:19.000000 stepcount-3.5.0/src/stepcount/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-26 19:11:19.000000 stepcount-3.5.0/src/stepcount/utils/collate_outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-26 19:11:19.000000 stepcount-3.5.0/src/stepcount/utils/generate_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:11:28.258127 stepcount-3.5.0/src/stepcount.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-04-26 19:11:28.000000 stepcount-3.5.0/src/stepcount.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-26 19:11:28.000000 stepcount-3.5.0/src/stepcount.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:11:28.000000 stepcount-3.5.0/src/stepcount.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-26 19:11:28.000000 stepcount-3.5.0/src/stepcount.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-26 19:11:28.000000 stepcount-3.5.0/src/stepcount.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 19:11:28.000000 stepcount-3.5.0/src/stepcount.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-04-26 19:11:19.000000 stepcount-3.5.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:45:58.177572 stepcount-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-05-01 06:45:50.000000 stepcount-3.6.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7575 2024-05-01 06:45:58.169571 stepcount-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-05-01 06:45:50.000000 stepcount-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-01 06:45:50.000000 stepcount-3.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 06:45:58.177572 stepcount-3.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-01 06:45:50.000000 stepcount-3.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:45:58.165572 stepcount-3.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:45:58.177572 stepcount-3.6.0/src/stepcount/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-01 06:45:50.000000 stepcount-3.6.0/src/stepcount/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-01 06:45:58.177572 stepcount-3.6.0/src/stepcount/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-01 06:45:50.000000 stepcount-3.6.0/src/stepcount/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9731 2024-05-01 06:45:50.000000 stepcount-3.6.0/src/stepcount/hmm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23588 2024-05-01 06:45:50.000000 stepcount-3.6.0/src/stepcount/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-05-01 06:45:50.000000 stepcount-3.6.0/src/stepcount/sslmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24407 2024-05-01 06:45:50.000000 stepcount-3.6.0/src/stepcount/stepcount.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:45:58.169571 stepcount-3.6.0/src/stepcount/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-01 06:45:50.000000 stepcount-3.6.0/src/stepcount/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-01 06:45:50.000000 stepcount-3.6.0/src/stepcount/utils/collate_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-01 06:45:50.000000 stepcount-3.6.0/src/stepcount/utils/generate_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:45:58.169571 stepcount-3.6.0/src/stepcount.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7575 2024-05-01 06:45:58.000000 stepcount-3.6.0/src/stepcount.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-01 06:45:58.000000 stepcount-3.6.0/src/stepcount.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 06:45:58.000000 stepcount-3.6.0/src/stepcount.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-01 06:45:58.000000 stepcount-3.6.0/src/stepcount.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-01 06:45:58.000000 stepcount-3.6.0/src/stepcount.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-01 06:45:58.000000 stepcount-3.6.0/src/stepcount.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-05-01 06:45:50.000000 stepcount-3.6.0/versioneer.py
```

### Comparing `stepcount-3.5.0/LICENSE.md` & `stepcount-3.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stepcount-3.5.0/PKG-INFO` & `stepcount-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepcount
-Version: 3.5.0
+Version: 3.6.0
 Summary: Step counter for wrist-worn accelerometers compatible with the UK Biobank Accelerometer Dataset
 Home-page: https://github.com/OxWearables/stepcount
 Download-URL: https://github.com/OxWearables/stepcount
 Author: Shing Chan, Scott Small, Gert Mertes, Aiden Doherty
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE file.
@@ -98,15 +98,15 @@
 2013-10-21     5368
 2013-10-22     7634
 2013-10-23    10009
 ...
 
 Output: outputs/sample/
 ```
-Refer to the [Data Dictionary](data-dictionary.md) for a comprehensive list of outputs.
+Refer to the [Data Dictionary](https://github.com/OxWearables/stepcount/blob/main/data-dictionary.md) for a comprehensive list of outputs.
 
 ### Troubleshooting 
 Some systems may face issues with Java when running the script. If this is your case, try fixing OpenJDK to version 8:
 ```console
 $ conda install -n stepcount openjdk=8
 ```
```

### Comparing `stepcount-3.5.0/README.md` & `stepcount-3.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 2013-10-21     5368
 2013-10-22     7634
 2013-10-23    10009
 ...
 
 Output: outputs/sample/
 ```
-Refer to the [Data Dictionary](data-dictionary.md) for a comprehensive list of outputs.
+Refer to the [Data Dictionary](https://github.com/OxWearables/stepcount/blob/main/data-dictionary.md) for a comprehensive list of outputs.
 
 ### Troubleshooting 
 Some systems may face issues with Java when running the script. If this is your case, try fixing OpenJDK to version 8:
 ```console
 $ conda install -n stepcount openjdk=8
 ```
```

### Comparing `stepcount-3.5.0/pyproject.toml` & `stepcount-3.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stepcount-3.5.0/setup.py` & `stepcount-3.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.5.0/src/stepcount/__init__.py` & `stepcount-3.6.0/src/stepcount/__init__.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.5.0/src/stepcount/features.py` & `stepcount-3.6.0/src/stepcount/features.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.5.0/src/stepcount/hmm_utils.py` & `stepcount-3.6.0/src/stepcount/hmm_utils.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.5.0/src/stepcount/models.py` & `stepcount-3.6.0/src/stepcount/models.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.5.0/src/stepcount/sslmodel.py` & `stepcount-3.6.0/src/stepcount/sslmodel.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.5.0/src/stepcount/stepcount.py` & `stepcount-3.6.0/src/stepcount/stepcount.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,22 @@
 
     model.wd.device = args.pytorch_device
 
     if verbose:
         print("Running step counter...")
     Y, W, T_steps = model.predict_from_frame(data)
 
+    # Quality control: Wear time coverage
+    coverage = Y.groupby(Y.index.hour).agg(lambda x: x.notna().mean())
+    if len(coverage) < 24 or coverage.min() < 0.01:
+        info['Covers24hOK'] = 0
+    else:
+        info['Covers24hOK'] = 1
+    del coverage  # free memory
+
     # Save step counts
     Y.to_csv(f"{outdir}/{basename}-Steps.csv.gz")
     # Save timestamps of each step
     T_steps.to_csv(f"{outdir}/{basename}-StepTimes.csv.gz", index=False)
 
     # ENMO summary
     enmo_summary = summarize_enmo(data)
@@ -141,50 +149,56 @@
     info['CadencePeak30Adjusted(steps/min)'] = cadence_summary_adj['cadence_peak30']
     info['Cadence95thAdjusted(steps/min)'] = cadence_summary_adj['cadence_p95']
 
     # Save Info.json
     with open(f"{outdir}/{basename}-Info.json", 'w') as f:
         json.dump(info, f, indent=4, cls=NpEncoder)
 
+    # Save hourly data
     hourly = pd.concat([
         steps_summary['hourly'],
         enmo_summary['hourly'],
     ], axis=1)
     hourly.to_csv(f"{outdir}/{basename}-Hourly.csv.gz")
     del hourly  # free memory
 
+    # Save hourly data, adjusted
     hourly_adj = pd.concat([
         steps_summary_adj['hourly'],
         enmo_summary_adj['hourly'],
     ], axis=1)
     hourly_adj.to_csv(f"{outdir}/{basename}-HourlyAdjusted.csv.gz")
     del hourly_adj  # free memory
 
+    # Save minutely data
     minutely = pd.concat([
         steps_summary['minutely'],
         enmo_summary['minutely'],
     ], axis=1)
     minutely.to_csv(f"{outdir}/{basename}-Minutely.csv.gz")
     del minutely  # free memory
 
+    # Save minutely data, adjusted
     minutely_adj = pd.concat([
         steps_summary_adj['minutely'],
         enmo_summary_adj['minutely'],
     ], axis=1)
     minutely_adj.to_csv(f"{outdir}/{basename}-MinutelyAdjusted.csv.gz")
     del minutely_adj  # free memory
 
+    # Save daily data
     daily = pd.concat([
         steps_summary['daily'],
         cadence_summary['daily'],
         enmo_summary['daily'],
     ], axis=1)
     daily.to_csv(f"{outdir}/{basename}-Daily.csv.gz")
     # del daily  # still needed for printing
 
+    # Save daily data, adjusted
     daily_adj = pd.concat([
         steps_summary_adj['daily'],
         cadence_summary_adj['daily'],
         enmo_summary_adj['daily'],
     ], axis=1)
     daily_adj.to_csv(f"{outdir}/{basename}-DailyAdjusted.csv.gz")
     # del daily_adj  # still needed for printing
```

### Comparing `stepcount-3.5.0/src/stepcount/utils/collate_outputs.py` & `stepcount-3.6.0/src/stepcount/utils/collate_outputs.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.5.0/src/stepcount/utils/generate_commands.py` & `stepcount-3.6.0/src/stepcount/utils/generate_commands.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.5.0/src/stepcount.egg-info/PKG-INFO` & `stepcount-3.6.0/src/stepcount.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepcount
-Version: 3.5.0
+Version: 3.6.0
 Summary: Step counter for wrist-worn accelerometers compatible with the UK Biobank Accelerometer Dataset
 Home-page: https://github.com/OxWearables/stepcount
 Download-URL: https://github.com/OxWearables/stepcount
 Author: Shing Chan, Scott Small, Gert Mertes, Aiden Doherty
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE file.
@@ -98,15 +98,15 @@
 2013-10-21     5368
 2013-10-22     7634
 2013-10-23    10009
 ...
 
 Output: outputs/sample/
 ```
-Refer to the [Data Dictionary](data-dictionary.md) for a comprehensive list of outputs.
+Refer to the [Data Dictionary](https://github.com/OxWearables/stepcount/blob/main/data-dictionary.md) for a comprehensive list of outputs.
 
 ### Troubleshooting 
 Some systems may face issues with Java when running the script. If this is your case, try fixing OpenJDK to version 8:
 ```console
 $ conda install -n stepcount openjdk=8
 ```
```

### Comparing `stepcount-3.5.0/src/stepcount.egg-info/SOURCES.txt` & `stepcount-3.6.0/src/stepcount.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stepcount-3.5.0/versioneer.py` & `stepcount-3.6.0/versioneer.py`

 * *Files identical despite different names*


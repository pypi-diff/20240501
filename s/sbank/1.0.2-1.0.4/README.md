# Comparing `tmp/sbank-1.0.2.tar.gz` & `tmp/sbank-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sbank-1.0.2.tar", last modified: Thu May  5 21:53:14 2022, max compression
+gzip compressed data, was "sbank-1.0.4.tar", last modified: Wed May  1 12:48:34 2024, max compression
```

## Comparing `sbank-1.0.2.tar` & `sbank-1.0.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 21:53:14.000000 sbank-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)    18092 2022-05-05 21:52:36.000000 sbank-1.0.2/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-05-05 21:52:36.000000 sbank-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3598 2022-05-05 21:53:14.000000 sbank-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2052 2022-05-05 21:52:36.000000 sbank-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 21:53:14.000000 sbank-1.0.2/bin/
--rw-r--r--   0 runner    (1001) docker     (121)    32072 2022-05-05 21:52:36.000000 sbank-1.0.2/bin/sbank
--rw-r--r--   0 runner    (1001) docker     (121)     5773 2022-05-05 21:52:36.000000 sbank-1.0.2/bin/sbank_choose_mchirp_boundaries
--rw-r--r--   0 runner    (1001) docker     (121)     3010 2022-05-05 21:52:36.000000 sbank-1.0.2/bin/sbank_hdf5_bankcombiner
--rw-r--r--   0 runner    (1001) docker     (121)     5585 2022-05-05 21:52:36.000000 sbank-1.0.2/bin/sbank_hdf5_choose_mchirp_boundaries
--rw-r--r--   0 runner    (1001) docker     (121)    14795 2022-05-05 21:52:36.000000 sbank-1.0.2/bin/sbank_pipe
--rw-r--r--   0 runner    (1001) docker     (121)    19585 2022-05-05 21:52:36.000000 sbank-1.0.2/bin/sbank_plot_sim
--rw-r--r--   0 runner    (1001) docker     (121)    11836 2022-05-05 21:52:36.000000 sbank-1.0.2/bin/sbank_sim
--rw-r--r--   0 runner    (1001) docker     (121)    12572 2022-05-05 21:52:36.000000 sbank-1.0.2/bin/sbank_sim_pipe
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 21:53:14.000000 sbank-1.0.2/debian/
--rw-r--r--   0 runner    (1001) docker     (121)      825 2022-05-05 21:52:36.000000 sbank-1.0.2/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (121)        2 2022-05-05 21:52:36.000000 sbank-1.0.2/debian/compat
--rw-r--r--   0 runner    (1001) docker     (121)     1627 2022-05-05 21:52:36.000000 sbank-1.0.2/debian/control
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2022-05-05 21:52:36.000000 sbank-1.0.2/debian/copyright
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-05-05 21:52:36.000000 sbank-1.0.2/debian/python3-sbank.install
--rwxr-xr-x   0 runner    (1001) docker     (121)      705 2022-05-05 21:52:36.000000 sbank-1.0.2/debian/rules
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-05-05 21:52:36.000000 sbank-1.0.2/debian/sbank.install
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 21:53:14.000000 sbank-1.0.2/debian/source/
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-05-05 21:52:36.000000 sbank-1.0.2/debian/source/format
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-05-05 21:52:36.000000 sbank-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     5050 2022-05-05 21:52:36.000000 sbank-1.0.2/python-sbank.spec
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-05-05 21:52:36.000000 sbank-1.0.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 21:53:14.000000 sbank-1.0.2/sbank/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-05-05 21:52:36.000000 sbank-1.0.2/sbank/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11787 2022-05-05 21:52:36.000000 sbank-1.0.2/sbank/bank.py
--rw-r--r--   0 runner    (1001) docker     (121)     2538 2022-05-05 21:52:36.000000 sbank-1.0.2/sbank/overlap.py
--rw-r--r--   0 runner    (1001) docker     (121)     4983 2022-05-05 21:52:36.000000 sbank-1.0.2/sbank/overlap_cpu.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    13184 2022-05-05 21:52:36.000000 sbank-1.0.2/sbank/overlap_cpu_lib.c
--rw-r--r--   0 runner    (1001) docker     (121)     3668 2022-05-05 21:52:36.000000 sbank-1.0.2/sbank/overlap_cuda.py
--rw-r--r--   0 runner    (1001) docker     (121)     5705 2022-05-05 21:52:36.000000 sbank-1.0.2/sbank/psds.py
--rw-r--r--   0 runner    (1001) docker     (121)    25640 2022-05-05 21:52:36.000000 sbank-1.0.2/sbank/tau0tau3.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 21:53:14.000000 sbank-1.0.2/sbank/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-05-05 21:52:36.000000 sbank-1.0.2/sbank/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2338 2022-05-05 21:52:36.000000 sbank-1.0.2/sbank/tests/test_psds.py
--rw-r--r--   0 runner    (1001) docker     (121)    38494 2022-05-05 21:52:36.000000 sbank-1.0.2/sbank/waveforms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-05 21:53:14.000000 sbank-1.0.2/sbank.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3598 2022-05-05 21:53:14.000000 sbank-1.0.2/sbank.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      786 2022-05-05 21:53:14.000000 sbank-1.0.2/sbank.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-05 21:53:14.000000 sbank-1.0.2/sbank.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-05-05 21:53:14.000000 sbank-1.0.2/sbank.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-05-05 21:53:14.000000 sbank-1.0.2/sbank.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1808 2022-05-05 21:53:14.000000 sbank-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1170 2022-05-05 21:52:36.000000 sbank-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:48:34.163091 sbank-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-01 12:48:02.000000 sbank-1.0.4/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-01 12:48:02.000000 sbank-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-01 12:48:34.163091 sbank-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-01 12:48:02.000000 sbank-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:48:34.163091 sbank-1.0.4/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)    32178 2024-05-01 12:48:02.000000 sbank-1.0.4/bin/sbank
+-rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-05-01 12:48:02.000000 sbank-1.0.4/bin/sbank_choose_mchirp_boundaries
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-01 12:48:02.000000 sbank-1.0.4/bin/sbank_hdf5_bankcombiner
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-05-01 12:48:02.000000 sbank-1.0.4/bin/sbank_hdf5_choose_mchirp_boundaries
+-rw-r--r--   0 runner    (1001) docker     (127)    14795 2024-05-01 12:48:02.000000 sbank-1.0.4/bin/sbank_pipe
+-rw-r--r--   0 runner    (1001) docker     (127)    19585 2024-05-01 12:48:02.000000 sbank-1.0.4/bin/sbank_plot_sim
+-rw-r--r--   0 runner    (1001) docker     (127)    11836 2024-05-01 12:48:02.000000 sbank-1.0.4/bin/sbank_sim
+-rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-05-01 12:48:02.000000 sbank-1.0.4/bin/sbank_sim_pipe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:48:34.163091 sbank-1.0.4/debian/
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-01 12:48:02.000000 sbank-1.0.4/debian/changelog
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-01 12:48:02.000000 sbank-1.0.4/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-01 12:48:02.000000 sbank-1.0.4/debian/control
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-01 12:48:02.000000 sbank-1.0.4/debian/copyright
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-01 12:48:02.000000 sbank-1.0.4/debian/python3-sbank.install
+-rwxr-xr-x   0 runner    (1001) docker     (127)      705 2024-05-01 12:48:02.000000 sbank-1.0.4/debian/rules
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-01 12:48:02.000000 sbank-1.0.4/debian/sbank.install
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:48:34.163091 sbank-1.0.4/debian/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 12:48:02.000000 sbank-1.0.4/debian/source/format
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-01 12:48:02.000000 sbank-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-01 12:48:02.000000 sbank-1.0.4/python-sbank.spec
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-01 12:48:02.000000 sbank-1.0.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:48:34.163091 sbank-1.0.4/sbank/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 12:48:02.000000 sbank-1.0.4/sbank/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11730 2024-05-01 12:48:02.000000 sbank-1.0.4/sbank/bank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-01 12:48:02.000000 sbank-1.0.4/sbank/overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-01 12:48:02.000000 sbank-1.0.4/sbank/overlap_cpu.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    13358 2024-05-01 12:48:02.000000 sbank-1.0.4/sbank/overlap_cpu_lib.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-01 12:48:02.000000 sbank-1.0.4/sbank/overlap_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-05-01 12:48:02.000000 sbank-1.0.4/sbank/psds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25786 2024-05-01 12:48:02.000000 sbank-1.0.4/sbank/tau0tau3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:48:34.163091 sbank-1.0.4/sbank/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-01 12:48:02.000000 sbank-1.0.4/sbank/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-01 12:48:02.000000 sbank-1.0.4/sbank/tests/test_psds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37968 2024-05-01 12:48:02.000000 sbank-1.0.4/sbank/waveforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:48:34.163091 sbank-1.0.4/sbank.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-01 12:48:33.000000 sbank-1.0.4/sbank.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-01 12:48:34.000000 sbank-1.0.4/sbank.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:48:33.000000 sbank-1.0.4/sbank.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-01 12:48:33.000000 sbank-1.0.4/sbank.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 12:48:33.000000 sbank-1.0.4/sbank.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-01 12:48:34.163091 sbank-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-01 12:48:02.000000 sbank-1.0.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sbank-1.0.2/COPYING` & `sbank-1.0.4/COPYING`

 * *Files identical despite different names*

### Comparing `sbank-1.0.2/PKG-INFO` & `sbank-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbank
-Version: 1.0.2
+Version: 1.0.4
 Summary: A library for generating template banks of compact binary mergers for gravitational-wave searches using the "stochastic" placement algorithm
 Home-page: https://github.com/gwastro/sbank
 Author: The Sbank team
 Maintainer: Ian Harry
 Maintainer-email: ian.harry@ligo.org
 License: GPL-2.0-or-later
 Project-URL: Bug Tracker, https://github.com/gwastro/sbank/issues/
@@ -36,15 +36,15 @@
         anyone.
         
         If you use sbank in scientific publication, please see our citation guidelines
         (which Ian will have to write, for now the PyCBC help page
         <https://pycbc.org/pycbc/latest/html/tmpltbank.html#tmpltbank-alignedstochbank>
         contains the important details).
         
-        ![Structure of sbank](./tools/sbank_structure_ini.svg?raw=true "Structure of sbank")
+        ![Structure of sbank](./tools/sbank_structure.png?raw=true "Structure of sbank")
         
         "Structure of sbank" image courtesy of Han Wang, Sun Yat-sen University.
         
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -54,10 +54,11 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/markdown
```

### Comparing `sbank-1.0.2/README.md` & `sbank-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,11 +25,11 @@
 anyone.
 
 If you use sbank in scientific publication, please see our citation guidelines
 (which Ian will have to write, for now the PyCBC help page
 <https://pycbc.org/pycbc/latest/html/tmpltbank.html#tmpltbank-alignedstochbank>
 contains the important details).
 
-![Structure of sbank](./tools/sbank_structure_ini.svg?raw=true "Structure of sbank")
+![Structure of sbank](./tools/sbank_structure.png?raw=true "Structure of sbank")
 
 "Structure of sbank" image courtesy of Han Wang, Sun Yat-sen University.
```

### Comparing `sbank-1.0.2/bin/sbank` & `sbank-1.0.4/bin/sbank`

 * *Files 0% similar despite different names*

```diff
@@ -372,15 +372,18 @@
 
 else:
     noise_model = noise_models[opts.noise_model]
 
 #
 # initialize the bank
 #
-bank = Bank(noise_model, opts.flow, opts.use_metric, opts.cache_waveforms, opts.neighborhood_size, opts.neighborhood_param, coarse_match_df=opts.coarse_match_df, iterative_match_df_max=opts.iterative_match_df_max, fhigh_max=opts.fhigh_max, optimize_flow=opts.optimize_flow, flow_column=opts.flow_column)
+bank = Bank(noise_model, opts.flow, opts.use_metric, opts.cache_waveforms, opts.neighborhood_size,
+            opts.neighborhood_param, coarse_match_df=opts.coarse_match_df,
+            iterative_match_df_max=opts.iterative_match_df_max, fhigh_max=opts.fhigh_max,
+            optimize_flow=opts.optimize_flow)
 for file_approx in opts.bank_seed:
 
     # if no approximant specified, use same approximant as the
     # templates we will add
     if len(file_approx.split(":")) == 1:
         seed_file = file_approx
         approx = opts.approximant
@@ -561,14 +564,16 @@
                 #curr_id = EventIDColumn()
                 #curr_id.id = len(bank)
                 #curr_id.snglInspiralTable = row
                 #row.event_id = curr_id
                 row.ifo = opts.instrument
                 row.process_id = process.process_id
                 row.event_id = tbl.get_next_id()
+                if opts.flow_column:
+                    setattr(row, opts.flow_column, tmplt.flow)
                 tbl.append(row)
             if opts.output_filename.endswith(('.hdf', '.h5', '.hdf5')):
                 row = tmplt.to_storage_arr()
                 if len(tbl) == 0:
                     tbl = row
                 else:
                     tbl = np.append(tbl, row)
```

### Comparing `sbank-1.0.2/bin/sbank_choose_mchirp_boundaries` & `sbank-1.0.4/bin/sbank_choose_mchirp_boundaries`

 * *Files identical despite different names*

### Comparing `sbank-1.0.2/bin/sbank_hdf5_bankcombiner` & `sbank-1.0.4/bin/sbank_hdf5_bankcombiner`

 * *Files identical despite different names*

### Comparing `sbank-1.0.2/bin/sbank_hdf5_choose_mchirp_boundaries` & `sbank-1.0.4/bin/sbank_hdf5_choose_mchirp_boundaries`

 * *Files identical despite different names*

### Comparing `sbank-1.0.2/bin/sbank_pipe` & `sbank-1.0.4/bin/sbank_pipe`

 * *Files identical despite different names*

### Comparing `sbank-1.0.2/bin/sbank_plot_sim` & `sbank-1.0.4/bin/sbank_plot_sim`

 * *Files identical despite different names*

### Comparing `sbank-1.0.2/bin/sbank_sim` & `sbank-1.0.4/bin/sbank_sim`

 * *Files identical despite different names*

### Comparing `sbank-1.0.2/bin/sbank_sim_pipe` & `sbank-1.0.4/bin/sbank_sim_pipe`

 * *Files identical despite different names*

### Comparing `sbank-1.0.2/debian/changelog` & `sbank-1.0.4/debian/changelog`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+sbank (1.0.4-1) stable; urgency=low
+  
+  * Actually get release right
+
+ -- Ian Harry <ian.harry@ligo.org>  Wed, 01 May 2024 13:06:00 +0000
+
+sbank (1.0.3-1) stable; urgency=low
+  
+  * See pypi for details
+
+ -- Ian Harry <ian.harry@ligo.org>  Wed, 01 May 2024 10:06:00 +0000
+
 sbank (1.0.2-1) stable; urgency=low
 
   * Ensure request_disk gets set
 
  -- Ian Harry <ian.harry@ligo.org>  Thu, 05 May 2022 16:06:00 +0000
 
 sbank (1.0.1-1) stable; urgency=low
```

### Comparing `sbank-1.0.2/debian/control` & `sbank-1.0.4/debian/control`

 * *Files 7% similar despite different names*

```diff
@@ -12,19 +12,19 @@
  dh-python,
  cython3,
  help2man,
  lalapps,
  liblal-dev,
  python3-all,
  python3-dev,
- python3-glue,
  python3-h5py,
  python3-lal,
  python3-lalsimulation,
  python3-ligo-lw-bin | ligo-lw-bin,
+ python3-lscsoft-glue,
  python3-matplotlib,
  python3-numpy,
  python3-pytest (>= 3.9.1),
  python3-scipy,
  python3-six,
  python3-setuptools (>= 30.3.0),
 
@@ -32,17 +32,17 @@
 
 Package: python3-sbank
 Architecture: any
 Depends:
  ${misc:Depends},
  ${python3:Depends},
  ${shlibs:Depends},
- python3-glue,
  python3-lal,
  python3-lalsimulation,
+ python3-lscsoft-glue,
  python3-numpy,
  python3-six,
 Description: Python 3 modules for Sbank
  Sbank provides a library for generating template banks of compact binary
  mergers for gravitational-wave searches using the "stochastic" placement
  algorithm.
  .
@@ -52,19 +52,19 @@
 
 Package: sbank
 Architecture: all
 Depends:
  ${misc:Depends},
  ${python3:Depends},
  lalapps,
- python3-glue,
  python3-h5py,
  python3-lal,
  python3-lalsimulation,
  python3-ligo-lw-bin | ligo-lw-bin,
+ python3-lscsoft-glue,
  python3-matplotlib,
  python3-numpy,
  python3-sbank (= ${binary:Version}),
  python3-scipy,
 Description: Command-line utilities for Sbank
  Sbank provides a library for generating template banks of compact binary
  mergers for gravitational-wave searches using the "stochastic" placement
```

### Comparing `sbank-1.0.2/debian/copyright` & `sbank-1.0.4/debian/copyright`

 * *Files identical despite different names*

### Comparing `sbank-1.0.2/debian/rules` & `sbank-1.0.4/debian/rules`

 * *Files identical despite different names*

### Comparing `sbank-1.0.2/python-sbank.spec` & `sbank-1.0.4/python-sbank.spec`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 %define srcname sbank
-%define version 1.0.2
+%define version 1.0.4
 %define release 1
 
 # -- src.rpm metadata -------
 
 Name:      python-%{srcname}
 Version:   %{version}
 Release:   %{release}%{?dist}
@@ -31,19 +31,19 @@
 BuildRequires: python%{python3_pkgversion}-Cython
 BuildRequires: python%{python3_pkgversion}-numpy
 BuildRequires: python%{python3_pkgversion}-setuptools >= 30.3.0
 
 # runtime dependencies (required for %check and help2man)
 BuildRequires: help2man
 BuildRequires: lalapps
-BuildRequires: python%{python3_pkgversion}-glue
 BuildRequires: python%{python3_pkgversion}-h5py
 BuildRequires: python%{python3_pkgversion}-lal
 BuildRequires: python%{python3_pkgversion}-lalsimulation
 BuildRequires: python%{python3_pkgversion}-ligo-lw-bin
+BuildRequires: python%{python3_pkgversion}-lscsoft-glue
 BuildRequires: python%{python3_pkgversion}-matplotlib
 BuildRequires: python%{python3_pkgversion}-scipy
 BuildRequires: python%{python3_pkgversion}-six
 
 # testing dependencies (required for %check)
 %if 0%{?rhel} == 0 || 0%{?rhel} >= 9
 BuildRequires: python%{python3_pkgversion}-pytest >= 3.9.1
@@ -69,34 +69,34 @@
 # -- packages ---------------
 
 %package -n %{srcname}
 Summary: Command-line utilities for Sbank
 BuildArch: noarch
 Requires: lalapps
 Requires: python%{python3_pkgversion}-%{srcname} = %{version}-%{release}
-Requires: python%{python3_pkgversion}-glue
 Requires: python%{python3_pkgversion}-h5py
 Requires: python%{python3_pkgversion}-lal
 Requires: python%{python3_pkgversion}-lalsimulation
 Requires: python%{python3_pkgversion}-ligo-lw-bin
+Requires: python%{python3_pkgversion}-lscsoft-glue
 Requires: python%{python3_pkgversion}-matplotlib
 Requires: python%{python3_pkgversion}-numpy
 Requires: python%{python3_pkgversion}-scipy
 Requires: python%{python3_pkgversion}-six
 %description -n %{srcname}
 Sbank provides a library for generating template banks of compact binary
 mergers for gravitational-wave searches using the "stochastic" placement
 algorithm.
 The package provides the command-line utilities.
 
 %package -n python%{python3_pkgversion}-%{srcname}
 Summary: Python %{python3_version} library for Sbank
-Requires: python%{python3_pkgversion}-glue
 Requires: python%{python3_pkgversion}-lal
 Requires: python%{python3_pkgversion}-lalsimulation
+Requires: python%{python3_pkgversion}-lscsoft-glue
 Requires: python%{python3_pkgversion}-numpy
 Requires: python%{python3_pkgversion}-six
 %{?python_provide:%python_provide python%{python3_pkgversion}-%{srcname}}
 %description -n python%{python3_pkgversion}-%{srcname}
 Sbank provides a library for generating template banks of compact binary
 mergers for gravitational-wave searches using the "stochastic" placement
 algorithm.
```

### Comparing `sbank-1.0.2/sbank/bank.py` & `sbank-1.0.4/sbank/bank.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,23 +44,22 @@
         return len(self.seq)
 
 
 class Bank(object):
 
     def __init__(self, noise_model, flow, use_metric=False, cache_waveforms=False, nhood_size=1.0,
                  nhood_param="tau0", coarse_match_df=None, iterative_match_df_max=None,
-                 fhigh_max=None, optimize_flow=None, flow_column=None):
+                 fhigh_max=None, optimize_flow=None):
         self.noise_model = noise_model
         self.flow = flow
         self.use_metric = use_metric
         self.cache_waveforms = cache_waveforms
         self.coarse_match_df = coarse_match_df
         self.iterative_match_df_max = iterative_match_df_max
         self.optimize_flow = optimize_flow
-        self.flow_column = flow_column
 
         if (
             self.coarse_match_df
             and self.iterative_match_df_max
             and self.coarse_match_df < self.iterative_match_df_max
         ):
             # If this case occurs coarse_match_df offers no improvement, turn off
```

### Comparing `sbank-1.0.2/sbank/overlap.py` & `sbank-1.0.4/sbank/overlap.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,32 +21,32 @@
     ADD ME
     """
     min_len = tmplt.data.length
     if inj.data.length <= tmplt.data.length:
         min_len = inj.data.length
     else:
         min_len = tmplt.data.length
-    assert(inj.deltaF == tmplt.deltaF)
+    assert (inj.deltaF == tmplt.deltaF)
     delta_f = inj.deltaF
     if phase_maximized:
         return SBankCythonComputeMatch(inj.data.data, tmplt.data.data, min_len,
                                        delta_f, workspace_cache)
     else:
         return SBankCythonComputeRealMatch(inj.data.data, tmplt.data.data,
                                            min_len, delta_f, workspace_cache)
 
 
 def SBankComputeMatchSkyLoc(hp, hc, hphccorr, proposal, workspace_cache1,
                             workspace_cache2, phase_maximized=False):
     """
     ADD ME
     """
-    assert(hp.deltaF == proposal.deltaF)
-    assert(hc.deltaF == proposal.deltaF)
-    assert(hp.data.length == hc.data.length)
+    assert (hp.deltaF == proposal.deltaF)
+    assert (hc.deltaF == proposal.deltaF)
+    assert (hp.data.length == hc.data.length)
     if proposal.data.length <= hp.data.length:
         min_len = proposal.data.length
     else:
         min_len = hp.data.length
     if phase_maximized:
         return SBankCythonComputeMatchMaxSkyLoc(hp.data.data, hc.data.data,
                                                 hphccorr, proposal.data.data,
```

### Comparing `sbank-1.0.2/sbank/overlap_cpu.pyx` & `sbank-1.0.4/sbank/overlap_cpu.pyx`

 * *Files identical despite different names*

### Comparing `sbank-1.0.2/sbank/overlap_cpu_lib.c` & `sbank-1.0.4/sbank/overlap_cpu_lib.c`

 * *Files 1% similar despite different names*

```diff
@@ -19,26 +19,30 @@
 #include <stdlib.h>
 #include <string.h>
 #include <math.h>
 #include <complex.h>
 #include <sys/types.h>
 
 /* ---------------- LAL STUFF NEEDED ----------------- */
+int XLALPrintError(const char *fmt, ...);
+
 typedef struct tagCOMPLEX8Vector {
      uint32_t length; /**< Number of elements in array. */
      float complex *data; /**< Pointer to the data array. */
 } COMPLEX8Vector;
 
 COMPLEX8Vector * XLALCreateCOMPLEX8Vector ( uint32_t length );
 void XLALDestroyCOMPLEX8Vector ( COMPLEX8Vector * vector );
 
 typedef struct tagCOMPLEX8FFTPlan COMPLEX8FFTPlan;
 
 COMPLEX8FFTPlan * XLALCreateReverseCOMPLEX8FFTPlan( uint32_t size, int measurelvl );
 
+int XLALCOMPLEX8VectorFFT (COMPLEX8Vector * restrict output, const COMPLEX8Vector * restrict input, const COMPLEX8FFTPlan *plan);
+
 void XLALDestroyCOMPLEX8FFTPlan( COMPLEX8FFTPlan *plan );
 
 /* ----------------------------------------------- */
 
 typedef struct tagWS {
     size_t n;
     COMPLEX8FFTPlan *plan;
```

### Comparing `sbank-1.0.2/sbank/overlap_cuda.py` & `sbank-1.0.4/sbank/overlap_cuda.py`

 * *Files identical despite different names*

### Comparing `sbank-1.0.2/sbank/psds.py` & `sbank-1.0.4/sbank/psds.py`

 * *Files identical despite different names*

### Comparing `sbank-1.0.2/sbank/tau0tau3.py` & `sbank-1.0.4/sbank/tau0tau3.py`

 * *Files 1% similar despite different names*

```diff
@@ -647,25 +647,28 @@
                           theta, phi, iota, psi, orb_phase, bank)
 
 
 proposals = {
     "IMRPhenomB": IMRPhenomB_param_generator,
     "IMRPhenomC": IMRPhenomC_param_generator,
     "IMRPhenomD": aligned_spin_param_generator,
+    "IMRPhenomXAS": aligned_spin_param_generator,
     "TaylorF2": aligned_spin_param_generator,
     "IMRPhenomP": double_spin_precessing_param_generator,
     "IMRPhenomPv2": double_spin_precessing_param_generator,
     "TaylorF2RedSpin": aligned_spin_param_generator,
     "EOBNRv2": nonspin_param_generator,
     "SEOBNRv1": aligned_spin_param_generator,
     "SEOBNRv2": aligned_spin_param_generator,
     "SEOBNRv2_ROM_DoubleSpin": aligned_spin_param_generator,
     "SEOBNRv2_ROM_DoubleSpin_HI": aligned_spin_param_generator,
     "SEOBNRv4": aligned_spin_param_generator,
     "SEOBNRv4_ROM": aligned_spin_param_generator,
+    "SEOBNRv5": aligned_spin_param_generator,
+    "SEOBNRv5_ROM": aligned_spin_param_generator,
     "SpinTaylorT4": SpinTaylorT4_param_generator,
     "SpinTaylorF2": single_spin_precessing_param_generator,
     "SpinTaylorT5Fourier": double_spin_precessing_param_generator,
     "SEOBNRv3": double_spin_precessing_param_generator,
     "EOBNRv2HM_ROM": nonspin_hom_param_generator,
     "EOBNRv2HM_ROM_AmpMax": nonspin_hom_param_generator,
     "EOBNRv2HM_ROM_PhaseMax": nonspin_hom_param_generator,
```

### Comparing `sbank-1.0.2/sbank/tests/test_psds.py` & `sbank-1.0.4/sbank/tests/test_psds.py`

 * *Files identical despite different names*

### Comparing `sbank-1.0.2/sbank/waveforms.py` & `sbank-1.0.4/sbank/waveforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
 from __future__ import (division, print_function)
 
 import logging
-import sys
 from math import isnan
 import numpy as np
 from numpy import float32
 import lal
 import lalsimulation as lalsim
 from lal import MSUN_SI, MTSUN_SI, PC_SI, PI
 from lal import CreateREAL8Vector, CreateCOMPLEX8FrequencySeries
@@ -36,26 +35,25 @@
 _sit_cols = llwsit.validcolumns
 
 
 class SnglInspiralTable(llwsit):
     def __init__(self, *args, **kwargs):
         llwsit.__init__(self, *args, **kwargs)
         for entry in _sit_cols.keys():
-            if not(hasattr(self, entry)):
+            if not hasattr(self, entry):
                 if _sit_cols[entry] in ['real_4', 'real_8']:
                     setattr(self, entry, 0.)
                 elif _sit_cols[entry] == 'int_4s':
                     setattr(self, entry, 0)
                 elif _sit_cols[entry] == 'lstring':
                     setattr(self, entry, '')
                 elif _sit_cols[entry] == 'ilwd:char':
                     setattr(self, entry, '')
             else:
-                print("Column %s not recognized" % entry, file=sys.stderr)
-                raise ValueError
+                raise ValueError(f"Column {entry} not recognized")
 
 
 def compute_mchirp(m1, m2):
     return (m1 * m1 * m1 * m2 * m2 * m2 / (m1 + m2))**0.2
 
 
 def ceil_pow_2(number):
@@ -177,15 +175,15 @@
       a sngl_inspiral object.
     * Provide a classmethod to_sngl, which creates a sngl_inspiral object
       from an instance of the subclass.
     * Provide a classmethod from_sim, which creates an instance based on
       a sim_inspiral object.
     """
     approximant = None
-    __slots__ = ("m1", "m2", "spin1z", "spin2z", "chieff", "bank", "tau0",
+    __slots__ = ("m1", "m2", "spin1z", "spin2z", "chieff", "tau0", "tau0_40", "flow",
                  "_dur", "_mchirp", "_wf", "_metric", "sigmasq",
                  "is_seed_point", "_f_final", "_fhigh_max")
     param_names = ("m1", "m2", "spin1z", "spin2z")
     param_formats = ("%.2f", "%.2f", "%.2f", "%.2f")
     hdf_dtype = [('mass1', float32), ('mass2', float32),
                  ('spin1z', float32), ('spin2z', float32),
                  ('template_duration', float32), ('f_lower', float32),
@@ -195,15 +193,14 @@
 
         self.m1 = float(m1)
         self.m2 = float(m2)
         self.spin1z = float(spin1z)
         self.spin2z = float(spin2z)
         self.chieff = lalsim.SimIMRPhenomBComputeChi(self.m1, self.m2,
                                                      self.spin1z, self.spin2z)
-        self.bank = bank
 
         if flow is None:
             self.flow = bank.flow
             if bank.optimize_flow is not None:
                 self.optimize_flow(bank.flow, bank.fhigh_max, bank.noise_model,
                                    sigma_frac=bank.optimize_flow)
         else:
@@ -320,27 +317,24 @@
         return cls(float(params['mass1'][idx]), float(params['mass2'][idx]),
                    float(params['spin1z'][idx]), float(params['spin2z'][idx]),
                    bank, flow=flow, duration=duration)
 
     def to_sngl(self):
         # All numerical values are initiated as 0 and all strings as ''
         row = SnglInspiralTable()
-
         row.mass1 = self.m1
         row.mass2 = self.m2
         row.mtotal = self.m1 + self.m2
         row.mchirp = self._mchirp
         row.eta = row.mass1 * row.mass2 / (row.mtotal * row.mtotal)
         row.tau0, row.tau3 = m1m2_to_tau0tau3(self.m1, self.m2, self.flow)
         row.template_duration = self.dur
         row.spin1z = self.spin1z
         row.spin2z = self.spin2z
         row.sigmasq = self.sigmasq
-        if self.bank.flow_column:
-            setattr(row, self.bank.flow_column, self.flow)
 
         return row
 
     def to_storage_arr(self):
         """Dump the template params to a numpy array."""
         new_tmplt = np.zeros(1, dtype=self.hdf_dtype)
         new_tmplt['mass1'] = self.m1
@@ -488,14 +482,30 @@
                                             self.m2 * MSUN_SI, self.spin1z,
                                             self.spin2z, self.flow)
         # add a 10% to be consistent with PyCBC's duration estimate,
         # may want to FIXME if that changes
         return dur * 1.1
 
 
+class IMRPhenomXASTemplate(IMRAlignedSpinTemplate):
+    approximant = "IMRPhenomXAS"
+
+    def _get_dur(self):
+        dur = lalsim.SimIMRPhenomXASDuration(
+            self.m1 * MSUN_SI,
+            self.m2 * MSUN_SI,
+            self.spin1z,
+            self.spin2z,
+            self.flow
+        )
+        # add a 10% to be consistent with PyCBC's duration estimate,
+        # may want to FIXME if that changes
+        return dur * 1.1
+
+
 class SEOBNRv2Template(IMRAlignedSpinTemplate):
     approximant = "SEOBNRv2"
 
     def _get_dur(self):
         seff = lalsim.SimIMRPhenomBComputeChi(self.m1, self.m2,
                                               self.spin1z, self.spin2z)
         dur = lalsim.SimIMRSEOBNRv2ChirpTimeSingleSpin(
@@ -524,14 +534,33 @@
         return dur * 1.1
 
 
 class SEOBNRv4ROMTemplate(SEOBNRv4Template):
     approximant = "SEOBNRv4_ROM"
 
 
+class SEOBNRv5Template(IMRAlignedSpinTemplate):
+    approximant = "SEOBNRv5"
+
+    def _get_dur(self):
+        dur = lalsim.SimIMRSEOBNRv5ROMTimeOfFrequency(
+            self.flow,
+            self.m1 * MSUN_SI,
+            self.m2 * MSUN_SI,
+            self.spin1z,
+            self.spin2z
+        )
+        # Allow a 10% margin of error
+        return dur * 1.1
+
+
+class SEOBNRv5ROMTemplate(SEOBNRv5Template):
+    approximant = "SEOBNRv5_ROM"
+
+
 class EOBNRv2Template(SEOBNRv2Template):
     approximant = "EOBNRv2"
     param_names = ("m1", "m2")
     param_formats = ("%.2f", "%.2f")
 
     def __init__(self, m1, m2, bank, flow=None, duration=None):
         # Use everything from SEOBNRv2Template class except call
@@ -542,15 +571,15 @@
 
 class TaylorF2RedSpinTemplate(InspiralAlignedSpinTemplate):
     approximant = "TaylorF2RedSpin"
     param_names = ("m1", "m2", "chired")
     param_formats = ("%.5f", "%.5f", "%+.4f")
 
     __slots__ = ("chired", "tau0", "_dur", "_mchirp", "_eta", "_theta0",
-                 "_theta3", "_theta3s")
+                 "_theta3", "_theta3s", "bank")
 
     def __init__(self, m1, m2, spin1z, spin2z, bank, flow=None, duration=None):
 
         warn_msg = ("DEPRECATION WARNING: It is not a good idea to use this "
                     "approximant. The TaylorF2 approximant is the best thing "
                     "to use if you are constructing a 'brute-force match' "
                     "bank. This allows the use of both spins correctly, and "
@@ -570,14 +599,15 @@
         self._eta = m1*m2/(m1+m2)**2
         self._theta0, self._theta3, self._theta3s = compute_chirptimes(
             self._mchirp,
             self._eta,
             self.chired,
             self.flow
         )
+        self.bank = bank
 
     def finalize_as_template(self):
         if not self.bank.use_metric:
             return
 
         df, PSD = get_neighborhood_PSD([self], self.flow,
                                        self.bank.noise_model)
@@ -820,36 +850,24 @@
                    params['latitude'][idx], params['longitude'][idx],
                    params['polarization'][idx], params['inclination'][idx],
                    params['orbital_phase'][idx], bank,
                    flow=flow, duration=duration)
 
     def to_sngl(self):
         # All numerical values are initiated as 0 and all strings as ''
-        row = SnglInspiralTable()
-        row.mass1 = self.m1
-        row.mass2 = self.m2
-        row.mtotal = self.m1 + self.m2
-        row.mchirp = self._mchirp
-        row.eta = row.mass1 * row.mass2 / (row.mtotal * row.mtotal)
-        row.tau0, row.tau3 = m1m2_to_tau0tau3(self.m1, self.m2, self.flow)
-        row.template_duration = self.dur
+        row = super(PrecessingSpinTemplate, self).to_sngl()
         row.spin1x = self.spin1x
         row.spin1y = self.spin1y
-        row.spin1z = self.spin1z
         row.spin2x = self.spin2x
         row.spin2y = self.spin2y
-        row.spin2z = self.spin2z
         row.alpha1 = self.theta
         row.alpha2 = self.phi
         row.alpha3 = self.iota
         row.alpha4 = self.psi
         row.alpha5 = self.orb_phase
-        row.sigmasq = self.sigmasq
-        if self.bank.flow_column:
-            setattr(row, self.bank.flow_column, self.flow)
         return row
 
     def to_storage_arr(self):
         """Dump the template params to a numpy array."""
         new_tmplt = super(PrecessingSpinTemplate, self).to_storage_arr()
         new_tmplt['spin1x'] = self.spin1x
         new_tmplt['spin1y'] = self.spin1y
@@ -923,40 +941,14 @@
                    sngl.spin1z, sngl.alpha1, sngl.alpha2, sngl.alpha3,
                    sngl.alpha4, sngl.alpha5, bank)
 
     @classmethod
     def from_dict(cls, hdf_fp, idx, bank):
         raise NotImplementedError('Please write this!')
 
-    def to_sngl(self):
-        # All numerical values are initiated as 0 and all strings as ''
-        row = SnglInspiralTable()
-        row.mass1 = self.m1
-        row.mass2 = self.m2
-        row.mtotal = self.m1 + self.m2
-        row.mchirp = self._mchirp
-        row.eta = row.mass1 * row.mass2 / (row.mtotal * row.mtotal)
-        row.tau0, row.tau3 = m1m2_to_tau0tau3(self.m1, self.m2, self.flow)
-        row.template_duration = self.dur
-        row.spin1x = self.spin1x
-        row.spin1y = self.spin1y
-        row.spin1z = self.spin1z
-        row.spin2x = 0
-        row.spin2y = 0
-        row.spin2z = 0
-        row.alpha1 = self.theta
-        row.alpha2 = self.phi
-        row.alpha3 = self.iota
-        row.alpha4 = self.psi
-        row.alpha5 = self.orb_phase
-        row.sigmasq = self.sigmasq
-        if self.bank.flow_column:
-            setattr(row, self.bank.flow_column, self.flow)
-        return row
-
 
 class SpinTaylorT5FourierTemplate(InspiralPrecessingSpinTemplate):
     approximant = "SpinTaylorT5Fourier"
 
 
 class SpinTaylorT4Template(InspiralPrecessingSpinTemplate):
     approximant = "SpinTaylorT4"
@@ -1029,19 +1021,22 @@
     "TaylorF2RedSpin": TaylorF2RedSpinTemplate,
     "TaylorF2": TaylorF2Template,
     "IMRPhenomB": IMRPhenomBTemplate,
     "IMRPhenomC": IMRPhenomCTemplate,
     "IMRPhenomD": IMRPhenomDTemplate,
     "IMRPhenomP": IMRPhenomPTemplate,
     "IMRPhenomPv2": IMRPhenomPv2Template,
+    "IMRPhenomXAS": IMRPhenomXASTemplate,
     "SEOBNRv2": SEOBNRv2Template,
     "SEOBNRv2_ROM_DoubleSpin": SEOBNRv2ROMDoubleSpinTemplate,
     "SEOBNRv2_ROM_DoubleSpin_HI": SEOBNRv2ROMDoubleSpinHITemplate,
-    "SEOBNRv4": SEOBNRv4ROMTemplate,
+    "SEOBNRv4": SEOBNRv4Template,
     "SEOBNRv4_ROM": SEOBNRv4ROMTemplate,
+    "SEOBNRv5": SEOBNRv5Template,
+    "SEOBNRv5_ROM": SEOBNRv5ROMTemplate,
     "EOBNRv2": EOBNRv2Template,
     "SpinTaylorT4": SpinTaylorT4Template,
     "SpinTaylorT5": SpinTaylorT5Template,
     "SpinTaylorF2": SpinTaylorF2Template,
     "SpinTaylorT5Fourier": SpinTaylorT5FourierTemplate,
     "SEOBNRv3": SEOBNRv3Template,
     "EOBNRv2HM_ROM": EOBNRHigherOrderModeTemplate,
```

### Comparing `sbank-1.0.2/sbank.egg-info/PKG-INFO` & `sbank-1.0.4/sbank.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbank
-Version: 1.0.2
+Version: 1.0.4
 Summary: A library for generating template banks of compact binary mergers for gravitational-wave searches using the "stochastic" placement algorithm
 Home-page: https://github.com/gwastro/sbank
 Author: The Sbank team
 Maintainer: Ian Harry
 Maintainer-email: ian.harry@ligo.org
 License: GPL-2.0-or-later
 Project-URL: Bug Tracker, https://github.com/gwastro/sbank/issues/
@@ -36,15 +36,15 @@
         anyone.
         
         If you use sbank in scientific publication, please see our citation guidelines
         (which Ian will have to write, for now the PyCBC help page
         <https://pycbc.org/pycbc/latest/html/tmpltbank.html#tmpltbank-alignedstochbank>
         contains the important details).
         
-        ![Structure of sbank](./tools/sbank_structure_ini.svg?raw=true "Structure of sbank")
+        ![Structure of sbank](./tools/sbank_structure.png?raw=true "Structure of sbank")
         
         "Structure of sbank" image courtesy of Han Wang, Sun Yat-sen University.
         
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -54,10 +54,11 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/markdown
```

### Comparing `sbank-1.0.2/sbank.egg-info/SOURCES.txt` & `sbank-1.0.4/sbank.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sbank-1.0.2/setup.cfg` & `sbank-1.0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 	Operating System :: Unix
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering :: Astronomy
 	Topic :: Scientific/Engineering :: Physics
 project_urls = 
 	Bug Tracker = https://github.com/gwastro/sbank/issues/
 	Source Code = https://github.com/gwastro/sbank
 
 [options]
```

### Comparing `sbank-1.0.2/setup.py` & `sbank-1.0.4/setup.py`

 * *Files identical despite different names*


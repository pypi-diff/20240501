# Comparing `tmp/hivclustering-1.6.8.tar.gz` & `tmp/hivclustering-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hivclustering-1.6.8.tar", last modified: Thu Sep 28 00:06:02 2023, max compression
+gzip compressed data, was "hivclustering-1.7.0.tar", last modified: Wed May  1 15:11:33 2024, max compression
```

## Comparing `hivclustering-1.6.8.tar` & `hivclustering-1.7.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 sweaver    (503) staff       (20)        0 2023-09-28 00:06:02.002731 hivclustering-1.6.8/
--rw-r--r--   0 sweaver    (503) staff       (20)      255 2023-09-28 00:06:02.002560 hivclustering-1.6.8/PKG-INFO
--rw-r--r--   0 sweaver    (503) staff       (20)     8869 2023-03-17 17:39:41.000000 hivclustering-1.6.8/README.md
-drwxr-xr-x   0 sweaver    (503) staff       (20)        0 2023-09-28 00:06:01.998960 hivclustering-1.6.8/hivclustering/
--rw-r--r--   0 sweaver    (503) staff       (20)       92 2022-07-09 20:43:17.000000 hivclustering-1.6.8/hivclustering/__init__.py
-drwxr-xr-x   0 sweaver    (503) staff       (20)        0 2023-09-28 00:06:01.997600 hivclustering-1.6.8/hivclustering/data/
-drwxr-xr-x   0 sweaver    (503) staff       (20)        0 2023-09-28 00:06:02.001316 hivclustering-1.6.8/hivclustering/data/HBL/
--rw-r--r--   0 sweaver    (503) staff       (20)    11479 2022-07-09 20:43:17.000000 hivclustering-1.6.8/hivclustering/data/HBL/CycleSupport.bf
--rw-r--r--   0 sweaver    (503) staff       (20)     6622 2022-07-09 20:43:17.000000 hivclustering-1.6.8/hivclustering/data/HBL/DegreeDistributions.bf
--rw-r--r--   0 sweaver    (503) staff       (20)      616 2022-07-09 20:43:17.000000 hivclustering-1.6.8/hivclustering/data/HBL/ExtractACluster.bf
--rw-r--r--   0 sweaver    (503) staff       (20)      837 2022-07-09 20:43:17.000000 hivclustering-1.6.8/hivclustering/data/HBL/ExtractSequences.bf
--rw-r--r--   0 sweaver    (503) staff       (20)     8264 2022-07-09 20:43:17.000000 hivclustering-1.6.8/hivclustering/data/HBL/SimulateSequence.bf
--rw-r--r--   0 sweaver    (503) staff       (20)     3512 2022-07-09 22:49:33.000000 hivclustering-1.6.8/hivclustering/data/HBL/TriangleSupport.bf
--rw-r--r--   0 sweaver    (503) staff       (20)   108297 2023-09-27 23:36:43.000000 hivclustering-1.6.8/hivclustering/mtnetwork.py
--rwxr-xr-x   0 sweaver    (503) staff       (20)    43771 2023-07-21 16:58:27.000000 hivclustering-1.6.8/hivclustering/networkbuild.py
-drwxr-xr-x   0 sweaver    (503) staff       (20)        0 2023-09-28 00:06:01.999653 hivclustering-1.6.8/hivclustering.egg-info/
--rw-r--r--   0 sweaver    (503) staff       (20)      255 2023-09-28 00:06:01.000000 hivclustering-1.6.8/hivclustering.egg-info/PKG-INFO
--rw-r--r--   0 sweaver    (503) staff       (20)      601 2023-09-28 00:06:01.000000 hivclustering-1.6.8/hivclustering.egg-info/SOURCES.txt
--rw-r--r--   0 sweaver    (503) staff       (20)        1 2023-09-28 00:06:01.000000 hivclustering-1.6.8/hivclustering.egg-info/dependency_links.txt
--rw-r--r--   0 sweaver    (503) staff       (20)       65 2023-09-28 00:06:01.000000 hivclustering-1.6.8/hivclustering.egg-info/requires.txt
--rw-r--r--   0 sweaver    (503) staff       (20)       14 2023-09-28 00:06:01.000000 hivclustering-1.6.8/hivclustering.egg-info/top_level.txt
-drwxr-xr-x   0 sweaver    (503) staff       (20)        0 2023-09-28 00:06:02.002327 hivclustering-1.6.8/scripts/
--rwxr-xr-x   0 sweaver    (503) staff       (20)    23567 2022-07-09 20:43:17.000000 hivclustering-1.6.8/scripts/TNS
--rwxr-xr-x   0 sweaver    (503) staff       (20)     9179 2023-07-19 16:48:18.000000 hivclustering-1.6.8/scripts/hivnetworkannotate
--rwxr-xr-x   0 sweaver    (503) staff       (20)    33290 2023-07-19 16:48:18.000000 hivclustering-1.6.8/scripts/hivnetworkcsv
--rw-r--r--   0 sweaver    (503) staff       (20)       38 2023-09-28 00:06:02.002786 hivclustering-1.6.8/setup.cfg
--rw-r--r--   0 sweaver    (503) staff       (20)      769 2023-09-28 00:01:02.000000 hivclustering-1.6.8/setup.py
+drwxr-xr-x   0 sweaver    (503) staff       (20)        0 2024-05-01 15:11:33.581426 hivclustering-1.7.0/
+-rw-r--r--   0 sweaver    (503) staff       (20)      426 2024-05-01 15:11:33.581176 hivclustering-1.7.0/PKG-INFO
+-rw-r--r--   0 sweaver    (503) staff       (20)     8869 2023-03-17 17:39:41.000000 hivclustering-1.7.0/README.md
+drwxr-xr-x   0 sweaver    (503) staff       (20)        0 2024-05-01 15:11:33.577038 hivclustering-1.7.0/hivclustering/
+-rw-r--r--   0 sweaver    (503) staff       (20)       92 2022-07-09 20:43:17.000000 hivclustering-1.7.0/hivclustering/__init__.py
+drwxr-xr-x   0 sweaver    (503) staff       (20)        0 2024-05-01 15:11:33.575300 hivclustering-1.7.0/hivclustering/data/
+drwxr-xr-x   0 sweaver    (503) staff       (20)        0 2024-05-01 15:11:33.579281 hivclustering-1.7.0/hivclustering/data/HBL/
+-rw-r--r--   0 sweaver    (503) staff       (20)    11479 2022-07-09 20:43:17.000000 hivclustering-1.7.0/hivclustering/data/HBL/CycleSupport.bf
+-rw-r--r--   0 sweaver    (503) staff       (20)     6622 2022-07-09 20:43:17.000000 hivclustering-1.7.0/hivclustering/data/HBL/DegreeDistributions.bf
+-rw-r--r--   0 sweaver    (503) staff       (20)      616 2022-07-09 20:43:17.000000 hivclustering-1.7.0/hivclustering/data/HBL/ExtractACluster.bf
+-rw-r--r--   0 sweaver    (503) staff       (20)      837 2022-07-09 20:43:17.000000 hivclustering-1.7.0/hivclustering/data/HBL/ExtractSequences.bf
+-rw-r--r--   0 sweaver    (503) staff       (20)     8264 2022-07-09 20:43:17.000000 hivclustering-1.7.0/hivclustering/data/HBL/SimulateSequence.bf
+-rw-r--r--   0 sweaver    (503) staff       (20)     3512 2022-07-09 22:49:33.000000 hivclustering-1.7.0/hivclustering/data/HBL/TriangleSupport.bf
+-rw-r--r--   0 sweaver    (503) staff       (20)   108297 2023-09-27 23:36:43.000000 hivclustering-1.7.0/hivclustering/mtnetwork.py
+-rwxr-xr-x   0 sweaver    (503) staff       (20)    44269 2024-05-01 15:10:58.000000 hivclustering-1.7.0/hivclustering/networkbuild.py
+drwxr-xr-x   0 sweaver    (503) staff       (20)        0 2024-05-01 15:11:33.577879 hivclustering-1.7.0/hivclustering.egg-info/
+-rw-r--r--   0 sweaver    (503) staff       (20)      426 2024-05-01 15:11:33.000000 hivclustering-1.7.0/hivclustering.egg-info/PKG-INFO
+-rw-r--r--   0 sweaver    (503) staff       (20)      601 2024-05-01 15:11:33.000000 hivclustering-1.7.0/hivclustering.egg-info/SOURCES.txt
+-rw-r--r--   0 sweaver    (503) staff       (20)        1 2024-05-01 15:11:33.000000 hivclustering-1.7.0/hivclustering.egg-info/dependency_links.txt
+-rw-r--r--   0 sweaver    (503) staff       (20)       65 2024-05-01 15:11:33.000000 hivclustering-1.7.0/hivclustering.egg-info/requires.txt
+-rw-r--r--   0 sweaver    (503) staff       (20)       14 2024-05-01 15:11:33.000000 hivclustering-1.7.0/hivclustering.egg-info/top_level.txt
+drwxr-xr-x   0 sweaver    (503) staff       (20)        0 2024-05-01 15:11:33.580275 hivclustering-1.7.0/scripts/
+-rwxr-xr-x   0 sweaver    (503) staff       (20)    23567 2022-07-09 20:43:17.000000 hivclustering-1.7.0/scripts/TNS
+-rwxr-xr-x   0 sweaver    (503) staff       (20)     9179 2023-07-19 16:48:18.000000 hivclustering-1.7.0/scripts/hivnetworkannotate
+-rwxr-xr-x   0 sweaver    (503) staff       (20)    33290 2023-07-19 16:48:18.000000 hivclustering-1.7.0/scripts/hivnetworkcsv
+-rw-r--r--   0 sweaver    (503) staff       (20)       38 2024-05-01 15:11:33.581480 hivclustering-1.7.0/setup.cfg
+-rw-r--r--   0 sweaver    (503) staff       (20)      769 2024-05-01 15:10:58.000000 hivclustering-1.7.0/setup.py
```

### Comparing `hivclustering-1.6.8/README.md` & `hivclustering-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.8/hivclustering/data/HBL/CycleSupport.bf` & `hivclustering-1.7.0/hivclustering/data/HBL/CycleSupport.bf`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.8/hivclustering/data/HBL/DegreeDistributions.bf` & `hivclustering-1.7.0/hivclustering/data/HBL/DegreeDistributions.bf`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.8/hivclustering/data/HBL/ExtractACluster.bf` & `hivclustering-1.7.0/hivclustering/data/HBL/ExtractACluster.bf`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.8/hivclustering/data/HBL/ExtractSequences.bf` & `hivclustering-1.7.0/hivclustering/data/HBL/ExtractSequences.bf`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.8/hivclustering/data/HBL/SimulateSequence.bf` & `hivclustering-1.7.0/hivclustering/data/HBL/SimulateSequence.bf`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.8/hivclustering/data/HBL/TriangleSupport.bf` & `hivclustering-1.7.0/hivclustering/data/HBL/TriangleSupport.bf`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.8/hivclustering/mtnetwork.py` & `hivclustering-1.7.0/hivclustering/mtnetwork.py`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.8/hivclustering/networkbuild.py` & `hivclustering-1.7.0/hivclustering/networkbuild.py`

 * *Files 0% similar despite different names*

```diff
@@ -447,15 +447,18 @@
     cluster_min = min (records, key = lambda x: x[2])[2]
     cluster_max = max (records, key = lambda x: x[2])[2]
 
     for i, v in enumerate (records):
         if i >= length and i < len (records) - 1:
             trailing = sum ([k[3] for k in records [i - length : i + 1]])
             leading  = sum ([k[3] for k in records [i + 1: i + length + 1]])
-            diffs.append ([i, trailing, leading, leading / trailing])
+            if trailing > 0:
+                diffs.append ([i, trailing, leading, leading / trailing])
+            else:
+                diffs.append ([i, trailing, leading, 1.])
 
     diffs.sort (key = lambda r : r[3])
     zs = zscores ([d[3] for d in diffs])
 
     for i,d in enumerate(diffs):
         cs = cluster_scaler (records[d[0]][2])
         full_records[d[0]][6] = zs[i] + cs
@@ -498,14 +501,15 @@
     arguments.add_argument('-M', '--multiple-edges', dest='multiple_edges',help='Permit multiple edges (e.g. different dates) to link the same pair of nodes in the network [default is to choose the one with the shortest distance]', default=False, action='store_true')
     arguments.add_argument('-B', '--bridges',help='Report all bridges (edges whose removal would cause the graph to disconnect)', default=False, action='store_true')
     arguments.add_argument('--no-degree-fit', dest = "skip_degrees", help='Do not perform degree distribution fitting', default=False, action='store_true')
     arguments.add_argument('-X', '--extract',help='If provided, extract all the sequences ', type = int)
     arguments.add_argument('-O', '--output',help='Write the output file to', default = sys.stdout, type = argparse.FileType('w'))
     arguments.add_argument('-P', '--prior',help='When running in JSON output mode, provide a JSON file storing a previous (subset) version of the network for consistent cluster naming', required=False, type=argparse.FileType('r'))
     arguments.add_argument('-A', '--auto-profile', dest = 'auto_prof', help='If provided supercedes most other output and inference settings; will add edges from shortest to longest and report network statistics as a function of distance cutoff ', type = float)
+    arguments.add_argument('--min-cluster-size', dest = 'min_profile_size', help='If provided, works in conjunction with automatic distance threshold determination to only count clusters that have this many or more members', type = int, default = 2)
     arguments.add_argument('--after', help='[assumes DATES are available] If provided (as YYYYMMDD) then only allow EDGES that connect nodes with dates at or AFTER this date', required=False, type = str)
     arguments.add_argument('--before', help='[assumes DATES are available] If provided (as YYYYMMDD) then only allow EDGES that connect nodes with dates at or BEFORE this date', required=False, type = str)
     arguments.add_argument('--import-attributes', dest = 'import_attr', help='Import node attributes from this JSON', required=False, type=argparse.FileType('r'))
     arguments.add_argument('--subcluster-annotation', dest = 'subcluster_annotation', help='As "dist" "field"". Use subcluster annotation for distance "dist" from node attribute "field"  ', required=False, nargs = 2)
     arguments.add_argument('-q', '--quiet', help='Enable quiet mode',  action='store_true', default=False)
 
 
@@ -645,22 +649,25 @@
         run_settings.after = time.strptime(run_settings.after, '%Y%m%d')
         edge_filter_function = lambda edge, ef = edge_filter_function: ef (edge) and  edge.check_exact_date (run_settings.after, newer = True)
 
     if run_settings.auto_prof is not None or run_settings.auto_threshold:
 
         profile = []
 
+        min_cluster_size = run_settings.min_profile_size
+        
 
         def network_report (threshold, network, max_clusters = [0]):
             clusters = network.retrieve_clusters(singletons=False)
             edges = len (network.edges)
-            cl = sorted ([len (c) for c in clusters.values()], reverse = True)
+            cl = [k for k in sorted ([len (c) for c in clusters.values()], reverse = True) if k >= min_cluster_size]
             nnodes = sum (cl)
-            profile.append ([threshold, sum (cl), edges, len (cl), cl[0] if len (cl) > 0 else 0, cl[1] if len (cl) > 1 else 0,0.])
-            max_clusters[0] = max (max_clusters[0], len (cl))
+            if nnodes > 0:
+                profile.append ([threshold, sum (cl), edges, len (cl), cl[0] if len (cl) > 0 else 0, cl[1] if len (cl) > 1 else 0,0.])
+                max_clusters[0] = max (max_clusters[0], len (cl))
             print('\rEvaluating distance threshold %8.5f %d %d' % (threshold, max_clusters[0], len (cl)), end = '\r', file = sys.stderr)
 
             #print ("%g\t%d\t%d\t%d\t%d\t%d\t%g" % (profile))
             sys.setrecursionlimit(max(sys.getrecursionlimit(), nnodes))
             return run_settings.auto_prof is not None or len (cl) == 0 or len (cl) > max_clusters[0] // 4
 
         network.read_from_csv_file_ordered(run_settings.input, network_report, formatter, run_settings.threshold if run_settings.threshold is not None else 1., 'BULK', run_settings.auto_prof if run_settings.auto_prof else 1e-5, filter = edge_filter_function)
```

### Comparing `hivclustering-1.6.8/hivclustering.egg-info/SOURCES.txt` & `hivclustering-1.7.0/hivclustering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.8/scripts/TNS` & `hivclustering-1.7.0/scripts/TNS`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.8/scripts/hivnetworkannotate` & `hivclustering-1.7.0/scripts/hivnetworkannotate`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.8/scripts/hivnetworkcsv` & `hivclustering-1.7.0/scripts/hivnetworkcsv`

 * *Files identical despite different names*

### Comparing `hivclustering-1.6.8/setup.py` & `hivclustering-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from os.path import abspath, join, split
 from setuptools import setup
 
 sys.path.insert(0, join(split(abspath(__file__))[0], 'lib'))
 
 setup(name='hivclustering',
-      version="1.6.8",
+      version="1.7.0",
       description='HIV molecular clustering tools',
       author='Sergei Kosakovsky Pond',
       author_email='spond@ucsd.edu',
       url='http://github.com/veg/hivclustering',
       license='MIT License',
       packages=['hivclustering'],
       package_data={'hivclustering': [
```


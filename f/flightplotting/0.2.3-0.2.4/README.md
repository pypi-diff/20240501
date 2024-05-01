# Comparing `tmp/flightplotting-0.2.3.tar.gz` & `tmp/flightplotting-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flightplotting-0.2.3.tar", last modified: Thu Apr 18 12:18:21 2024, max compression
+gzip compressed data, was "flightplotting-0.2.4.tar", last modified: Wed May  1 09:02:29 2024, max compression
```

## Comparing `flightplotting-0.2.3.tar` & `flightplotting-0.2.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:18:21.296183 flightplotting-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-18 12:17:36.000000 flightplotting-0.2.3/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-18 12:17:36.000000 flightplotting-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-18 12:18:21.296183 flightplotting-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-18 12:17:36.000000 flightplotting-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:18:21.296183 flightplotting-0.2.3/flightplotting/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-18 12:17:36.000000 flightplotting-0.2.3/flightplotting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:18:21.296183 flightplotting-0.2.3/flightplotting/data/
--rw-r--r--   0 runner    (1001) docker     (127)   142015 2024-04-18 12:17:36.000000 flightplotting-0.2.3/flightplotting/data/ColdDraftF3APlane.obj
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:17:36.000000 flightplotting-0.2.3/flightplotting/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-18 12:17:36.000000 flightplotting-0.2.3/flightplotting/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8156 2024-04-18 12:17:36.000000 flightplotting-0.2.3/flightplotting/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-18 12:17:36.000000 flightplotting-0.2.3/flightplotting/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-18 12:17:36.000000 flightplotting-0.2.3/flightplotting/titlerenderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-04-18 12:17:36.000000 flightplotting-0.2.3/flightplotting/traces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:18:21.296183 flightplotting-0.2.3/flightplotting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-18 12:18:21.000000 flightplotting-0.2.3/flightplotting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-18 12:18:21.000000 flightplotting-0.2.3/flightplotting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:18:21.000000 flightplotting-0.2.3/flightplotting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-18 12:18:21.000000 flightplotting-0.2.3/flightplotting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 12:18:21.000000 flightplotting-0.2.3/flightplotting.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-18 12:18:21.296183 flightplotting-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-18 12:17:36.000000 flightplotting-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:18:21.296183 flightplotting-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-18 12:17:36.000000 flightplotting-0.2.3/tests/test_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:02:29.066512 flightplotting-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-05-01 09:01:47.000000 flightplotting-0.2.4/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-01 09:01:47.000000 flightplotting-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-01 09:02:29.066512 flightplotting-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-01 09:01:47.000000 flightplotting-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:02:29.062512 flightplotting-0.2.4/flightplotting/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-01 09:01:47.000000 flightplotting-0.2.4/flightplotting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:02:29.066512 flightplotting-0.2.4/flightplotting/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   142015 2024-05-01 09:01:47.000000 flightplotting-0.2.4/flightplotting/data/ColdDraftF3APlane.obj
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 09:01:47.000000 flightplotting-0.2.4/flightplotting/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-01 09:01:47.000000 flightplotting-0.2.4/flightplotting/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-05-01 09:01:47.000000 flightplotting-0.2.4/flightplotting/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-01 09:01:47.000000 flightplotting-0.2.4/flightplotting/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-01 09:01:47.000000 flightplotting-0.2.4/flightplotting/titlerenderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-05-01 09:01:47.000000 flightplotting-0.2.4/flightplotting/traces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:02:29.066512 flightplotting-0.2.4/flightplotting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-01 09:02:29.000000 flightplotting-0.2.4/flightplotting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-01 09:02:29.000000 flightplotting-0.2.4/flightplotting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 09:02:29.000000 flightplotting-0.2.4/flightplotting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-01 09:02:29.000000 flightplotting-0.2.4/flightplotting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 09:02:29.000000 flightplotting-0.2.4/flightplotting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-01 09:02:29.066512 flightplotting-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-01 09:01:47.000000 flightplotting-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 09:02:29.066512 flightplotting-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-01 09:01:47.000000 flightplotting-0.2.4/tests/test_plots.py
```

### Comparing `flightplotting-0.2.3/COPYING` & `flightplotting-0.2.4/COPYING`

 * *Files identical despite different names*

### Comparing `flightplotting-0.2.3/PKG-INFO` & `flightplotting-0.2.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: flightplotting
-Version: 0.2.3
+Version: 0.2.4
 Summary: Tools for Plotting Flight Data in Plotly
 Home-page: https://github.com/PyFlightCoach/FlightPlotting
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
 Description-Content-Type: text/markdown
 License-File: COPYING
-Requires-Dist: setuptools
-Requires-Dist: plotly
 Requires-Dist: numpy
 Requires-Dist: pandas
+Requires-Dist: plotly
 Requires-Dist: pfc-geometry>=0.2.4
 Requires-Dist: flightdata>=0.2.6
 Requires-Dist: flightanalysis>=0.2.6
 
 # FlightPlotting
```

### Comparing `flightplotting-0.2.3/flightplotting/data/ColdDraftF3APlane.obj` & `flightplotting-0.2.4/flightplotting/data/ColdDraftF3APlane.obj`

 * *Files identical despite different names*

### Comparing `flightplotting-0.2.3/flightplotting/model.py` & `flightplotting-0.2.4/flightplotting/model.py`

 * *Files identical despite different names*

### Comparing `flightplotting-0.2.3/flightplotting/plots.py` & `flightplotting-0.2.4/flightplotting/plots.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     cgtrace,
     ribbon,
     vectors,
     axestrace
 )
     
 from flightdata import State
+from flightdata.base.labeling import get_appended_id
 from geometry import Coord
 from flightplotting.model import obj, OBJ
 import numpy as np
 from typing import List, Union
 
 
 def plotsec(secs: Union[State, list[State]], scale=5, nmodels=0, fig=None, 
@@ -95,18 +96,19 @@
             print("no data for manoeuvre {}, {}".format(name, ex))
     
     fig.add_traces(traces)
     
 
     return fig
 
-def plot_regions(st: State, lab_cols: list[str], span=3, colours=None, fig=None):
+def plot_regions(st: State, lab_cols: list[str], span=3, colours=None, fig=None, **kwargs):
     colours = px.colors.qualitative.Plotly if colours is None else colours
     lab_cols = [lab_cols] if isinstance(lab_cols, str) else lab_cols
 
+
     st = st.label(clabs=st.cumulative_labels(*lab_cols))
     
     def get_base_label(clab):
         base = clab
         try:
             id = int(clab.split('_')[-1])
             base = clab[:-len(f'_{id}')]
@@ -114,29 +116,30 @@
             pass
         return base
     
     colmap = {}
 
     traces = []
     for i, (k, seg) in enumerate(st.split_labels('clabs').items()):
-        blab = get_base_label(k)
+        if len(seg) < 3:
+            continue
+        blab, id = get_appended_id(k)
         if blab not in colmap:
             colmap[blab] = colours[len(colmap) % len(colours)]
-            leg = True
-        else:
-            leg = False
-
-        traces += ribbon(seg, span, colmap[blab], name=k, showlegend=leg)
-
+        traces += ribbon(
+            seg, span, colmap[blab], name=blab,
+            showlegend=int(id)==0,
+            **kwargs[blab] if blab in kwargs else {}
+        )
         traces.append(go.Scatter3d(
             x=seg.pos.x, 
             y=seg.pos.y, 
             z=seg.pos.z,
             mode='lines', 
-            line=dict(width=6, color=colmap[blab]), 
+            line=dict(width=0, color=colmap[blab]), 
             name=k,
             showlegend=False
         ))
     
     if fig is None:
         fig = go.Figure(layout=go.Layout(template="flight3d+judge_view"))
     fig.add_traces(traces)
```

### Comparing `flightplotting-0.2.3/flightplotting/templates.py` & `flightplotting-0.2.4/flightplotting/templates.py`

 * *Files identical despite different names*

### Comparing `flightplotting-0.2.3/flightplotting/titlerenderer.py` & `flightplotting-0.2.4/flightplotting/titlerenderer.py`

 * *Files identical despite different names*

### Comparing `flightplotting-0.2.3/flightplotting/traces.py` & `flightplotting-0.2.4/flightplotting/traces.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,14 +250,13 @@
 
     _js = np.array(range(1, len(points), 2))
     _j = _npinterzip(_js, _js)[1:-1] # 1 3 3 4 4 5 
 
     _ks = np.array(range(2, len(points) -1 , 2))
     _k = _npinterzip(_ks, _ks) # 2 2 4 4 6 6 
 
-
     return [go.Mesh3d(
         x=points.x, y=points.y, z=points.z, i=_i, j=_j, k=_k,
         intensitymode="cell",
         facecolor=np.full(len(_i), color),
         **kwargs
     )]
```

### Comparing `flightplotting-0.2.3/flightplotting.egg-info/PKG-INFO` & `flightplotting-0.2.4/flightplotting.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: flightplotting
-Version: 0.2.3
+Version: 0.2.4
 Summary: Tools for Plotting Flight Data in Plotly
 Home-page: https://github.com/PyFlightCoach/FlightPlotting
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
 Description-Content-Type: text/markdown
 License-File: COPYING
-Requires-Dist: setuptools
-Requires-Dist: plotly
 Requires-Dist: numpy
 Requires-Dist: pandas
+Requires-Dist: plotly
 Requires-Dist: pfc-geometry>=0.2.4
 Requires-Dist: flightdata>=0.2.6
 Requires-Dist: flightanalysis>=0.2.6
 
 # FlightPlotting
```

### Comparing `flightplotting-0.2.3/setup.py` & `flightplotting-0.2.4/setup.py`

 * *Files identical despite different names*


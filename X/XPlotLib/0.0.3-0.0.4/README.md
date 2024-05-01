# Comparing `tmp/xplotlib-0.0.3.tar.gz` & `tmp/xplotlib-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xplotlib-0.0.3.tar", last modified: Sun Apr 28 05:34:59 2024, max compression
+gzip compressed data, was "xplotlib-0.0.4.tar", last modified: Wed May  1 01:01:25 2024, max compression
```

## Comparing `xplotlib-0.0.3.tar` & `xplotlib-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:34:59.869901 xplotlib-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-28 05:34:51.000000 xplotlib-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-28 05:34:59.869901 xplotlib-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-28 05:34:51.000000 xplotlib-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-28 05:34:51.000000 xplotlib-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-28 05:34:59.869901 xplotlib-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:34:59.865901 xplotlib-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:34:59.869901 xplotlib-0.0.3/src/XPlotLib/
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-04-28 05:34:51.000000 xplotlib-0.0.3/src/XPlotLib/BandgapAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17939 2024-04-28 05:34:51.000000 xplotlib-0.0.3/src/XPlotLib/DOSAnalyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-28 05:34:51.000000 xplotlib-0.0.3/src/XPlotLib/XPlotLibUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 05:34:51.000000 xplotlib-0.0.3/src/XPlotLib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 05:34:59.869901 xplotlib-0.0.3/src/XPlotLib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-28 05:34:59.000000 xplotlib-0.0.3/src/XPlotLib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-28 05:34:59.000000 xplotlib-0.0.3/src/XPlotLib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 05:34:59.000000 xplotlib-0.0.3/src/XPlotLib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-28 05:34:59.000000 xplotlib-0.0.3/src/XPlotLib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-28 05:34:59.000000 xplotlib-0.0.3/src/XPlotLib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:01:25.039464 xplotlib-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-01 01:01:20.000000 xplotlib-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-01 01:01:25.039464 xplotlib-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-01 01:01:20.000000 xplotlib-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-01 01:01:20.000000 xplotlib-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-01 01:01:25.039464 xplotlib-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:01:25.035464 xplotlib-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:01:25.035464 xplotlib-0.0.4/src/XPlotLib/
+-rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-05-01 01:01:20.000000 xplotlib-0.0.4/src/XPlotLib/BandgapAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18473 2024-05-01 01:01:20.000000 xplotlib-0.0.4/src/XPlotLib/DOSAnalyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-01 01:01:20.000000 xplotlib-0.0.4/src/XPlotLib/XPlotLibUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 01:01:20.000000 xplotlib-0.0.4/src/XPlotLib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:01:25.039464 xplotlib-0.0.4/src/XPlotLib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-01 01:01:25.000000 xplotlib-0.0.4/src/XPlotLib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-01 01:01:25.000000 xplotlib-0.0.4/src/XPlotLib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 01:01:25.000000 xplotlib-0.0.4/src/XPlotLib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-01 01:01:25.000000 xplotlib-0.0.4/src/XPlotLib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 01:01:25.000000 xplotlib-0.0.4/src/XPlotLib.egg-info/top_level.txt
```

### Comparing `xplotlib-0.0.3/LICENSE` & `xplotlib-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xplotlib-0.0.3/PKG-INFO` & `xplotlib-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XPlotLib
-Version: 0.0.3
+Version: 0.0.4
 Summary: Libary to plot experimental and theoretical XRay data.
 Home-page: https://github.com/CMM02/XPlotLib
 Author: Carl Magnus Meier
 Author-email: magnus.meier@outook.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xplotlib-0.0.3/setup.cfg` & `xplotlib-0.0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = XPlotLib
-version = 0.0.3
+version = 0.0.4
 author = Carl Magnus Meier
 author_email = magnus.meier@outook.de
 description = Libary to plot experimental and theoretical XRay data.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CMM02/XPlotLib
 classifiers =
```

### Comparing `xplotlib-0.0.3/src/XPlotLib/BandgapAnalyzer.py` & `xplotlib-0.0.4/src/XPlotLib/BandgapAnalyzer.py`

 * *Files identical despite different names*

### Comparing `xplotlib-0.0.3/src/XPlotLib/DOSAnalyzer.py` & `xplotlib-0.0.4/src/XPlotLib/DOSAnalyzer.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,16 @@
         self.active_xas_dos = {}
         self.xes_spectra = {}
         self.xas_spectra = {}
         self.xes_shift = 0
         self.xas_shift = 0
         self.xes_DOS_scale = 1
         self.xas_DOS_scale = 1
+        self.xes_x_lims = None
+        self.xas_x_lims = None
         self.staggered_spacing = 0.2
         self.title = 'DOS Analyzer'
 
     def __init_plt__(self, show_spectra):
         self.figsize = (15, 6)
 
         # create figure and axis depending on number of spectra to show
@@ -109,17 +111,18 @@
         selected_dos_dfs = []
         for dos_df in dos_dfs:
             dos_df = dos_df[['ENERGY'] + [col for col in dos_df.columns if col!= 'ENERGY' and col in active_dos_cols]]
             if(len(dos_df.columns) > 1):
                 selected_dos_dfs.append(dos_df)      
         return selected_dos_dfs
     
-    def __configure_plot__(self, ax, spectra, x_min, label, fig_count):
+    def __configure_plot__(self, ax, spectra, x_min, label, fig_count, x_lims=None):
             ax.text(0.075*fig_count/self.figsize[0], 0.2/self.figsize[1], label, ha='left', va='top', color='white', size=12, bbox=dict(facecolor='black', edgecolor='none', pad=3.0), transform=ax.transAxes)   
-            x_lims = self.__get_x_lims__(spectra.values())
+            if x_lims is None:
+                x_lims = self.__get_x_lims__(spectra.values())
             ax.set_xlim(x_lims)
             ax.set_ylim(x_min, 1.1)
             ax.set_yticklabels([])
             return x_lims
     
     def __plot_dos__(self, ax, dos_dfs, x_lims, x_shift, scale, staggered):        
         DOS_scale = self.__get_dos_scale__(dos_dfs, x_lims, x_shift) * scale
@@ -361,14 +364,29 @@
         Spacing between DOS
     """
     def set_staggered_spacing(self, spacing):
         self.staggered_spacing = spacing
 
 
     """
+    Set x limits for XES and XAS DOS
+
+    Parameters
+    ----------
+    xes_x_limits : tuple of float
+        X limits for XES DOS
+    xas_x_limits : tuple of float
+        X limits for XAS DOS
+    """
+    def set_x_limits(self, xes_x_limits=None, xas_x_limits=None):
+        self.xes_x_lims = xes_x_limits
+        self.xas_x_lims = xas_x_limits
+
+
+    """
     Plot DOS with XES and XAS spectra
 
     Parameters
     ----------
     staggered : bool
         Staggered DOS
     show_spectra : list of str
@@ -399,37 +417,37 @@
         if 'XAS' in show_spectra:
             selected_xas_dos_dfs = self.__filter_cols__(self.dos_dfs, active_xas_dos_cols)
 
         # configure XES and XAS plots
         x_min =  -0.1 - (max(len(active_xes_dos_cols), len(active_xes_dos_cols))-1) * self.staggered_spacing if staggered else -0.1
 
         if 'XES' in show_spectra:
-            xes_x_lims = self.__configure_plot__(self.ax_xes, self.xes_spectra, x_min, 'nXES', len(show_spectra))
+            self.xes_x_lims = self.__configure_plot__(self.ax_xes, self.xes_spectra, x_min, 'nXES', len(show_spectra), x_lims=self.xes_x_lims)
         
         if 'XAS' in show_spectra:
-            xas_x_lims = self.__configure_plot__(self.ax_xas, self.xas_spectra, x_min, 'XAS', len(show_spectra))
+            self.xas_x_lims = self.__configure_plot__(self.ax_xas, self.xas_spectra, x_min, 'XAS', len(show_spectra), x_lims=self.xas_x_lims)
     
         # plot spectra
         if 'XES' in show_spectra:
             self.__plot_spectra__(self.ax_xes, self.xes_spectra)
 
         if 'XAS' in show_spectra:
             self.__plot_spectra__(self.ax_xas, self.xas_spectra)
 
         # plot DOS
         if 'XES' in show_spectra:
             if len(selected_xes_dos_dfs) == 0:
                 print('No XES DOS selected for plotting')
             else:
-                self.__plot_dos__(self.ax_xes, selected_xes_dos_dfs, xes_x_lims, self.xes_shift, self.xes_DOS_scale, staggered)
+                self.__plot_dos__(self.ax_xes, selected_xes_dos_dfs, self.xes_x_lims, self.xes_shift, self.xes_DOS_scale, staggered)
         if 'XAS' in show_spectra:
             if len(selected_xas_dos_dfs) == 0:
                 print('No XAS DOS selected for plotting')
             else:
-                self.__plot_dos__(self.ax_xas,selected_xas_dos_dfs, xas_x_lims, self.xas_shift, self.xas_DOS_scale, staggered)
+                self.__plot_dos__(self.ax_xas,selected_xas_dos_dfs, self.xas_x_lims, self.xas_shift, self.xas_DOS_scale, staggered)
 
 
 
         # add legend
         if 'XES' in show_spectra:
             self.ax_xes.legend()
         if 'XAS' in show_spectra:
```

### Comparing `xplotlib-0.0.3/src/XPlotLib/XPlotLibUtils.py` & `xplotlib-0.0.4/src/XPlotLib/XPlotLibUtils.py`

 * *Files identical despite different names*

### Comparing `xplotlib-0.0.3/src/XPlotLib.egg-info/PKG-INFO` & `xplotlib-0.0.4/src/XPlotLib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XPlotLib
-Version: 0.0.3
+Version: 0.0.4
 Summary: Libary to plot experimental and theoretical XRay data.
 Home-page: https://github.com/CMM02/XPlotLib
 Author: Carl Magnus Meier
 Author-email: magnus.meier@outook.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


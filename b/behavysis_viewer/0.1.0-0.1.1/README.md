# Comparing `tmp/behavysis_viewer-0.1.0.tar.gz` & `tmp/behavysis_viewer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "behavysis_viewer-0.1.0.tar", max compression
+gzip compressed data, was "behavysis_viewer-0.1.1.tar", max compression
```

## Comparing `behavysis_viewer-0.1.0.tar` & `behavysis_viewer-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,30 @@
--rw-r--r--   0        0        0     8196 2024-04-18 23:44:53.869414 behavysis_viewer-0.1.0/behavysis_viewer/.DS_Store
--rw-r--r--   0        0        0       54 2024-04-18 23:44:53.877936 behavysis_viewer-0.1.0/behavysis_viewer/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 23:44:53.896315 behavysis_viewer-0.1.0/behavysis_viewer/models/__init__.py
--rw-r--r--   0        0        0     2645 2024-04-23 04:47:47.920096 behavysis_viewer-0.1.0/behavysis_viewer/models/bout_inspect_list_model.py
--rw-r--r--   0        0        0     2411 2024-04-23 04:47:47.920194 behavysis_viewer-0.1.0/behavysis_viewer/models/bouts_list_model.py
--rw-r--r--   0        0        0     1170 2024-04-18 23:44:53.946072 behavysis_viewer-0.1.0/behavysis_viewer/models/exp_file_manager.py
--rw-r--r--   0        0        0     4067 2024-04-23 04:47:47.926541 behavysis_viewer-0.1.0/behavysis_viewer/models/keypoints_model.py
--rw-r--r--   0        0        0      967 2024-04-22 08:46:10.601001 behavysis_viewer-0.1.0/behavysis_viewer/models/vid_model.py
--rw-r--r--   0        0        0        0 2024-04-18 23:44:53.981013 behavysis_viewer-0.1.0/behavysis_viewer/pydantic_models/__init__.py
--rw-r--r--   0        0        0     5005 2024-04-23 04:47:47.931126 behavysis_viewer-0.1.0/behavysis_viewer/pydantic_models/experiment_configs.py
--rw-r--r--   0        0        0     9931 2024-04-18 23:44:54.045971 behavysis_viewer-0.1.0/behavysis_viewer/resources/base_palette.xml
--rw-r--r--   0        0        0      544 2024-04-23 04:48:04.270903 behavysis_viewer-0.1.0/behavysis_viewer/run.py
--rw-r--r--   0        0        0        0 2024-04-18 23:44:54.107858 behavysis_viewer-0.1.0/behavysis_viewer/ui/__init__.py
--rw-r--r--   0        0        0    16715 2024-04-23 04:48:09.491480 behavysis_viewer-0.1.0/behavysis_viewer/ui/main_ui.py
--rw-r--r--   0        0        0    19964 2024-04-23 04:47:29.271819 behavysis_viewer-0.1.0/behavysis_viewer/ui/main_ui.ui
--rw-r--r--   0        0        0     4208 2024-04-18 23:44:54.144984 behavysis_viewer-0.1.0/behavysis_viewer/ui/settings_ui.py
--rw-r--r--   0        0        0     2298 2024-04-18 23:44:54.156210 behavysis_viewer-0.1.0/behavysis_viewer/ui/settings_ui.ui
--rw-r--r--   0        0        0        0 2024-04-18 23:44:54.168121 behavysis_viewer-0.1.0/behavysis_viewer/utils/__init__.py
--rw-r--r--   0        0        0      514 2024-04-18 23:44:54.181422 behavysis_viewer-0.1.0/behavysis_viewer/utils/constants.py
--rw-r--r--   0        0        0     1002 2024-04-23 04:48:16.692517 behavysis_viewer-0.1.0/behavysis_viewer/utils/cv2_qt_mixin.py
--rw-r--r--   0        0        0        0 2024-04-18 23:44:54.238040 behavysis_viewer-0.1.0/behavysis_viewer/widgets/__init__.py
--rw-r--r--   0        0        0     1943 2024-04-23 04:48:16.119464 behavysis_viewer-0.1.0/behavysis_viewer/widgets/cv_view.py
--rw-r--r--   0        0        0     4956 2024-04-23 04:48:15.567833 behavysis_viewer-0.1.0/behavysis_viewer/widgets/graph_view.py
--rw-r--r--   0        0        0        0 2024-04-18 23:44:54.274711 behavysis_viewer-0.1.0/behavysis_viewer/windows/__init__.py
--rw-r--r--   0        0        0     2055 2024-04-23 04:48:14.644516 behavysis_viewer-0.1.0/behavysis_viewer/windows/help.py
--rw-r--r--   0        0        0    18926 2024-04-23 04:48:14.257556 behavysis_viewer-0.1.0/behavysis_viewer/windows/main.py
--rw-r--r--   0        0        0     2380 2024-04-23 04:48:13.458986 behavysis_viewer-0.1.0/behavysis_viewer/windows/settings.py
--rw-r--r--   0        0        0      172 2024-04-18 23:44:54.312223 behavysis_viewer-0.1.0/behavysis_viewer/windows/window_mixin.py
--rw-r--r--   0        0        0    35821 2024-04-18 23:44:53.826579 behavysis_viewer-0.1.0/LICENSE
--rw-r--r--   0        0        0      695 2024-04-23 05:14:49.025094 behavysis_viewer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1220 2024-04-23 04:47:29.475079 behavysis_viewer-0.1.0/README.md
--rw-r--r--   0        0        0     1938 1970-01-01 00:00:00.000000 behavysis_viewer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     8196 2024-04-18 23:44:53.869414 behavysis_viewer-0.1.1/behavysis_viewer/.DS_Store
+-rw-r--r--   0        0        0       54 2024-04-18 23:44:53.877936 behavysis_viewer-0.1.1/behavysis_viewer/__init__.py
+-rw-r--r--   0        0        0      573 2024-05-01 04:53:06.190475 behavysis_viewer-0.1.1/behavysis_viewer/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-18 23:44:53.896315 behavysis_viewer-0.1.1/behavysis_viewer/models/__init__.py
+-rw-r--r--   0        0        0     2645 2024-04-23 04:47:47.920096 behavysis_viewer-0.1.1/behavysis_viewer/models/bout_inspect_list_model.py
+-rw-r--r--   0        0        0     2407 2024-05-01 05:07:14.941294 behavysis_viewer-0.1.1/behavysis_viewer/models/bouts_list_model.py
+-rw-r--r--   0        0        0     1170 2024-04-18 23:44:53.946072 behavysis_viewer-0.1.1/behavysis_viewer/models/exp_file_manager.py
+-rw-r--r--   0        0        0     4055 2024-05-01 05:02:14.551802 behavysis_viewer-0.1.1/behavysis_viewer/models/keypoints_model.py
+-rw-r--r--   0        0        0      967 2024-04-22 08:46:10.601001 behavysis_viewer-0.1.1/behavysis_viewer/models/vid_model.py
+-rw-r--r--   0        0        0     9931 2024-04-18 23:44:54.045971 behavysis_viewer-0.1.1/behavysis_viewer/resources/base_palette.xml
+-rw-r--r--   0        0        0        0 2024-04-18 23:44:54.107858 behavysis_viewer-0.1.1/behavysis_viewer/ui/__init__.py
+-rw-r--r--   0        0        0    16715 2024-04-23 04:48:09.491480 behavysis_viewer-0.1.1/behavysis_viewer/ui/main_ui.py
+-rw-r--r--   0        0        0    19964 2024-04-23 04:47:29.271819 behavysis_viewer-0.1.1/behavysis_viewer/ui/main_ui.ui
+-rw-r--r--   0        0        0     4208 2024-04-18 23:44:54.144984 behavysis_viewer-0.1.1/behavysis_viewer/ui/settings_ui.py
+-rw-r--r--   0        0        0     2298 2024-04-18 23:44:54.156210 behavysis_viewer-0.1.1/behavysis_viewer/ui/settings_ui.ui
+-rw-r--r--   0        0        0        0 2024-04-18 23:44:54.168121 behavysis_viewer-0.1.1/behavysis_viewer/utils/__init__.py
+-rw-r--r--   0        0        0      514 2024-04-18 23:44:54.181422 behavysis_viewer-0.1.1/behavysis_viewer/utils/constants.py
+-rw-r--r--   0        0        0     1002 2024-04-23 04:48:16.692517 behavysis_viewer-0.1.1/behavysis_viewer/utils/cv2_qt_mixin.py
+-rw-r--r--   0        0        0        0 2024-04-18 23:44:54.238040 behavysis_viewer-0.1.1/behavysis_viewer/widgets/__init__.py
+-rw-r--r--   0        0        0     1943 2024-04-23 04:48:16.119464 behavysis_viewer-0.1.1/behavysis_viewer/widgets/cv_view.py
+-rw-r--r--   0        0        0     4959 2024-05-01 05:11:46.933752 behavysis_viewer-0.1.1/behavysis_viewer/widgets/graph_view.py
+-rw-r--r--   0        0        0        0 2024-04-18 23:44:54.274711 behavysis_viewer-0.1.1/behavysis_viewer/windows/__init__.py
+-rw-r--r--   0        0        0     2055 2024-04-23 04:48:14.644516 behavysis_viewer-0.1.1/behavysis_viewer/windows/help.py
+-rw-r--r--   0        0        0    18944 2024-05-01 05:02:54.785372 behavysis_viewer-0.1.1/behavysis_viewer/windows/main.py
+-rw-r--r--   0        0        0     2380 2024-04-23 04:48:13.458986 behavysis_viewer-0.1.1/behavysis_viewer/windows/settings.py
+-rw-r--r--   0        0        0      172 2024-04-18 23:44:54.312223 behavysis_viewer-0.1.1/behavysis_viewer/windows/window_mixin.py
+-rw-r--r--   0        0        0    35821 2024-04-18 23:44:53.826579 behavysis_viewer-0.1.1/LICENSE
+-rw-r--r--   0        0        0      771 2024-05-01 05:08:47.292554 behavysis_viewer-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1220 2024-04-23 04:47:29.475079 behavysis_viewer-0.1.1/README.md
+-rw-r--r--   0        0        0     1938 1970-01-01 00:00:00.000000 behavysis_viewer-0.1.1/PKG-INFO
```

### Comparing `behavysis_viewer-0.1.0/behavysis_viewer/.DS_Store` & `behavysis_viewer-0.1.1/behavysis_viewer/.DS_Store`

 * *Files identical despite different names*

### Comparing `behavysis_viewer-0.1.0/behavysis_viewer/models/bout_inspect_list_model.py` & `behavysis_viewer-0.1.1/behavysis_viewer/models/bout_inspect_list_model.py`

 * *Files identical despite different names*

### Comparing `behavysis_viewer-0.1.0/behavysis_viewer/models/bouts_list_model.py` & `behavysis_viewer-0.1.1/behavysis_viewer/models/bouts_list_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import numpy as np
 from behavysis_core.data_models.bouts import Bouts
+from behavysis_core.data_models.experiment_configs import ExperimentConfigs
 from behavysis_core.mixins.behaviour_mixin import BehaviourMixin
 from behavysis_core.mixins.df_io_mixin import DFIOMixin
-from behavysis_viewer.pydantic_models.experiment_configs import ExperimentConfigs
-from behavysis_viewer.utils.constants import VALUE2COLOR
 from PySide6.QtCore import QAbstractListModel, Qt
 from PySide6.QtGui import QColor
 
+from behavysis_viewer.utils.constants import VALUE2COLOR
+
 
 class BoutsListModel(QAbstractListModel):
 
     bouts: Bouts
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `behavysis_viewer-0.1.0/behavysis_viewer/models/exp_file_manager.py` & `behavysis_viewer-0.1.1/behavysis_viewer/models/exp_file_manager.py`

 * *Files identical despite different names*

### Comparing `behavysis_viewer-0.1.0/behavysis_viewer/models/keypoints_model.py` & `behavysis_viewer-0.1.1/behavysis_viewer/models/keypoints_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import cv2
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
+from behavysis_core.constants import PROCESS_COL
+from behavysis_core.data_models.experiment_configs import ExperimentConfigs
 from behavysis_core.mixins.df_io_mixin import DFIOMixin
 from behavysis_core.mixins.keypoints_mixin import KeypointsMixin
-from behavysis_core.utils.constants import PROCESS_COL
-from behavysis_viewer.pydantic_models.experiment_configs import ExperimentConfigs
 
 
 class KeypointsModel:
 
     raw_dlc_df: pd.DataFrame
     annot_dlc_df: pd.DataFrame
     indivs_bpts_ls: pd.MultiIndex
```

### Comparing `behavysis_viewer-0.1.0/behavysis_viewer/models/vid_model.py` & `behavysis_viewer-0.1.1/behavysis_viewer/models/vid_model.py`

 * *Files identical despite different names*

### Comparing `behavysis_viewer-0.1.0/behavysis_viewer/resources/base_palette.xml` & `behavysis_viewer-0.1.1/behavysis_viewer/resources/base_palette.xml`

 * *Files identical despite different names*

### Comparing `behavysis_viewer-0.1.0/behavysis_viewer/ui/main_ui.py` & `behavysis_viewer-0.1.1/behavysis_viewer/ui/main_ui.py`

 * *Files identical despite different names*

### Comparing `behavysis_viewer-0.1.0/behavysis_viewer/ui/main_ui.ui` & `behavysis_viewer-0.1.1/behavysis_viewer/ui/main_ui.ui`

 * *Files identical despite different names*

### Comparing `behavysis_viewer-0.1.0/behavysis_viewer/ui/settings_ui.py` & `behavysis_viewer-0.1.1/behavysis_viewer/ui/settings_ui.py`

 * *Files identical despite different names*

### Comparing `behavysis_viewer-0.1.0/behavysis_viewer/ui/settings_ui.ui` & `behavysis_viewer-0.1.1/behavysis_viewer/ui/settings_ui.ui`

 * *Files identical despite different names*

### Comparing `behavysis_viewer-0.1.0/behavysis_viewer/utils/constants.py` & `behavysis_viewer-0.1.1/behavysis_viewer/utils/constants.py`

 * *Files identical despite different names*

### Comparing `behavysis_viewer-0.1.0/behavysis_viewer/utils/cv2_qt_mixin.py` & `behavysis_viewer-0.1.1/behavysis_viewer/utils/cv2_qt_mixin.py`

 * *Files identical despite different names*

### Comparing `behavysis_viewer-0.1.0/behavysis_viewer/widgets/cv_view.py` & `behavysis_viewer-0.1.1/behavysis_viewer/widgets/cv_view.py`

 * *Files identical despite different names*

### Comparing `behavysis_viewer-0.1.0/behavysis_viewer/widgets/graph_view.py` & `behavysis_viewer-0.1.1/behavysis_viewer/widgets/graph_view.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import sys
 
 import cv2
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from behavysis_core.data_models.bouts import Bouts
-from behavysis_viewer.pydantic_models.experiment_configs import ExperimentConfigs
-from behavysis_viewer.utils.cv2_qt_mixin import Cv2QtMixin
+from behavysis_core.data_models.experiment_configs import ExperimentConfigs
 from pyqtgraph import BarGraphItem, InfiniteLine, PlotWidget, mkPen
 from pyqtgraph.exporters import ImageExporter
 from PySide6.QtWidgets import QApplication
 
+from behavysis_viewer.utils.cv2_qt_mixin import Cv2QtMixin
+
 
 class GraphView(PlotWidget):
 
     bars: list[BarGraphItem]
     time_marker_line: InfiniteLine
 
     def __init__(self, *args, **kwargs):
@@ -50,24 +51,24 @@
     def plot_init(self, start_ls, stop_ls, behavs_ls, **kwargs):
         behavs_ls_i, behavs = pd.factorize(behavs_ls)
         self.clear()
         self.bars = []
         # Plotting data
         # TODO: fix this up. Un-pythonic for loop
         # TODO: change colour of bar depending on bout "actual" value
-        for i in range(len(start_ls)):
-            bar = BarGraphItem(
+        for i, _ in enumerate(start_ls):
+            bar_ = BarGraphItem(
                 x0=start_ls[i],
                 x1=stop_ls[i],
                 y=behavs_ls_i[i],
                 height=0.5,
-                pen=mkPen(color="r"),
+                # pen=mkPen(color="r"),
             )
-            self.bars.append(bar)
-            self.addItem(bar)
+            self.bars.append(bar_)
+            self.addItem(bar_)
         # self.plot(x, y)
         # Setting current time marker line
         self.time_marker_line.setPos(0)
         self.addItem(self.time_marker_line)
         # Plot aesthetics
         self.set_plot_attr(**kwargs)
```

### Comparing `behavysis_viewer-0.1.0/behavysis_viewer/windows/help.py` & `behavysis_viewer-0.1.1/behavysis_viewer/windows/help.py`

 * *Files identical despite different names*

### Comparing `behavysis_viewer-0.1.0/behavysis_viewer/windows/main.py` & `behavysis_viewer-0.1.1/behavysis_viewer/windows/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 import sys
 import time
 from multiprocessing import Process, Value
 from multiprocessing.sharedctypes import Synchronized
 
 import cv2
 import numpy as np
+from behavysis_core.data_models.experiment_configs import ExperimentConfigs
 from behavysis_core.mixins.behaviour_mixin import BehaviourMixin
 from behavysis_core.mixins.df_io_mixin import DFIOMixin
-from behavysis_viewer.models.bout_inspect_list_model import BoutInspectListModel
-from behavysis_viewer.models.bouts_list_model import BoutsListModel
-from behavysis_viewer.models.exp_file_manager import ExpFileManager
-from behavysis_viewer.models.keypoints_model import KeypointsModel
-from behavysis_viewer.models.vid_model import VidModel
-from behavysis_viewer.pydantic_models.experiment_configs import ExperimentConfigs
-from behavysis_viewer.ui.main_ui import Ui_MainWindow
-from behavysis_viewer.utils.constants import STATUS_MSG_TIMEOUT
-from behavysis_viewer.widgets.graph_view import GraphView
-from behavysis_viewer.windows.help import HelpWindow
-from behavysis_viewer.windows.settings import SettingsWindow
-from behavysis_viewer.windows.window_mixin import WindowMixin
 from PySide6.QtCore import Qt, QTimer
 from PySide6.QtGui import QKeySequence, QShortcut
 from PySide6.QtWidgets import (
     QApplication,
     QDialog,
     QFileDialog,
     QLabel,
     QMainWindow,
     QMessageBox,
     QVBoxLayout,
 )
 from tqdm import trange
 
+from behavysis_viewer.models.bout_inspect_list_model import BoutInspectListModel
+from behavysis_viewer.models.bouts_list_model import BoutsListModel
+from behavysis_viewer.models.exp_file_manager import ExpFileManager
+from behavysis_viewer.models.keypoints_model import KeypointsModel
+from behavysis_viewer.models.vid_model import VidModel
+from behavysis_viewer.ui.main_ui import Ui_MainWindow
+from behavysis_viewer.utils.constants import STATUS_MSG_TIMEOUT
+from behavysis_viewer.widgets.graph_view import GraphView
+from behavysis_viewer.windows.help import HelpWindow
+from behavysis_viewer.windows.settings import SettingsWindow
+from behavysis_viewer.windows.window_mixin import WindowMixin
+
 
 class MainWindow(QMainWindow, WindowMixin):
     """__summary__"""
 
     ui: Ui_MainWindow
     preferences_window: SettingsWindow
     help_window: HelpWindow
@@ -280,14 +281,15 @@
             self.ui.statusbar.showMessage(
                 f"Opened video: {fp}", timeout=STATUS_MSG_TIMEOUT
             )
         except ValueError as e:
             self.ui.statusbar.showMessage(
                 f"Failed to open {fp}: {e}", timeout=STATUS_MSG_TIMEOUT
             )
+            print(e)
 
     def select_bout(self):
         """__summary__"""
         # Getting selected bout QIndex (if there exists one)
         if len(self.ui.bouts_view.selectedIndexes()) > 0:
             index = self.ui.bouts_view.selectedIndexes()[0]
             # Getting bout df row
```

### Comparing `behavysis_viewer-0.1.0/behavysis_viewer/windows/settings.py` & `behavysis_viewer-0.1.1/behavysis_viewer/windows/settings.py`

 * *Files identical despite different names*

### Comparing `behavysis_viewer-0.1.0/LICENSE` & `behavysis_viewer-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `behavysis_viewer-0.1.0/README.md` & `behavysis_viewer-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `behavysis_viewer-0.1.0/PKG-INFO` & `behavysis_viewer-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: behavysis_viewer
-Version: 0.1.0
+Version: 0.1.1
 Summary: A semi-automated behaviour verification, processing and analysis package.
 License: LGPL-3.0-or-later
 Author: BowenLab
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PySide6 (>=6.7.0,<7.0.0)
-Requires-Dist: behavysis_core (>=0.1.0,<0.2.0)
+Requires-Dist: behavysis_core (>=0.1.1,<0.2.0)
 Requires-Dist: pyqtgraph (>=0.13.6,<0.14.0)
 Description-Content-Type: text/markdown
 
 # behavysis_viewer
 
 Semi-automated scoring animal behaviour. Behaviour is first predicted by a classifier and then the user verifies &amp; further scores this behaviour.
```


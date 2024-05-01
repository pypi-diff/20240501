# Comparing `tmp/broh5-1.1.0.tar.gz` & `tmp/broh5-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "broh5-1.1.0.tar", last modified: Fri Dec  1 20:32:16 2023, max compression
+gzip compressed data, was "broh5-1.2.0.tar", last modified: Wed May  1 11:52:46 2024, max compression
```

## Comparing `broh5-1.1.0.tar` & `broh5-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-12-01 20:32:16.265088 broh5-1.1.0/
--rw-rw-rw-   0        0        0    11575 2023-10-11 15:07:33.000000 broh5-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     6256 2023-12-01 20:32:16.246222 broh5-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5374 2023-11-21 19:49:29.000000 broh5-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-12-01 20:32:16.044355 broh5-1.1.0/broh5/
--rw-rw-rw-   0        0        0       21 2023-12-01 17:23:43.000000 broh5-1.1.0/broh5/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:32:16.208181 broh5-1.1.0/broh5/lib/
--rw-rw-rw-   0        0        0        0 2023-10-18 01:14:31.000000 broh5-1.1.0/broh5/lib/__init__.py
--rw-rw-rw-   0        0        0    16225 2023-12-01 17:07:49.000000 broh5-1.1.0/broh5/lib/interactions.py
--rw-rw-rw-   0        0        0    16500 2023-11-18 19:17:21.000000 broh5-1.1.0/broh5/lib/rendering.py
--rw-rw-rw-   0        0        0     8340 2023-12-01 17:47:48.000000 broh5-1.1.0/broh5/lib/utilities.py
--rw-rw-rw-   0        0        0     2030 2023-11-29 21:30:46.000000 broh5-1.1.0/broh5/main.py
-drwxrwxrwx   0        0        0        0 2023-12-01 20:32:16.228248 broh5-1.1.0/broh5.egg-info/
--rw-rw-rw-   0        0        0     6256 2023-12-01 20:32:15.000000 broh5-1.1.0/broh5.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-12-01 20:32:15.000000 broh5-1.1.0/broh5.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-01 20:32:15.000000 broh5-1.1.0/broh5.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-12-01 20:32:15.000000 broh5-1.1.0/broh5.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       64 2023-12-01 20:32:15.000000 broh5-1.1.0/broh5.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-12-01 20:32:15.000000 broh5-1.1.0/broh5.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-01 20:32:16.266134 broh5-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1256 2023-12-01 17:06:36.000000 broh5-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:52:46.968273 broh5-1.2.0/
+-rw-rw-rw-   0        0        0    11575 2023-12-04 18:40:00.000000 broh5-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     4446 2024-05-01 11:52:46.950718 broh5-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3567 2024-04-30 15:49:04.000000 broh5-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 11:52:46.736573 broh5-1.2.0/broh5/
+-rw-rw-rw-   0        0        0       21 2023-12-04 18:40:00.000000 broh5-1.2.0/broh5/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:52:46.916073 broh5-1.2.0/broh5/lib/
+-rw-rw-rw-   0        0        0        0 2023-12-04 18:40:00.000000 broh5-1.2.0/broh5/lib/__init__.py
+-rw-rw-rw-   0        0        0    21650 2024-04-30 20:35:46.000000 broh5-1.2.0/broh5/lib/interactions.py
+-rw-rw-rw-   0        0        0    22145 2024-04-30 14:25:43.000000 broh5-1.2.0/broh5/lib/rendering.py
+-rw-rw-rw-   0        0        0    13379 2024-04-30 20:18:24.000000 broh5-1.2.0/broh5/lib/utilities.py
+-rw-rw-rw-   0        0        0     3044 2024-04-30 14:25:43.000000 broh5-1.2.0/broh5/main.py
+drwxrwxrwx   0        0        0        0 2024-05-01 11:52:46.931884 broh5-1.2.0/broh5.egg-info/
+-rw-rw-rw-   0        0        0     4446 2024-05-01 11:52:46.000000 broh5-1.2.0/broh5.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2024-05-01 11:52:46.000000 broh5-1.2.0/broh5.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 11:52:46.000000 broh5-1.2.0/broh5.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 11:52:46.000000 broh5-1.2.0/broh5.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       63 2024-05-01 11:52:46.000000 broh5-1.2.0/broh5.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-01 11:52:46.000000 broh5-1.2.0/broh5.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 11:52:46.969214 broh5-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1253 2024-04-30 14:25:43.000000 broh5-1.2.0/setup.py
```

### Comparing `broh5-1.1.0/LICENSE` & `broh5-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `broh5-1.1.0/broh5/lib/interactions.py` & `broh5-1.2.0/broh5/lib/interactions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,104 @@
+"""
+This module links user interactions to the responses of the Broh5 software.
+"""
+
 import os
 import h5py
 import hdf5plugin
 import numpy as np
 import matplotlib.pyplot as plt
 from nicegui import ui
 from nicegui.events import ValueChangeEventArguments
 import broh5.lib.rendering as re
 import broh5.lib.utilities as util
 from broh5.lib.rendering import GuiRendering, FilePicker, FileSaver
 
 
 class GuiInteraction(GuiRendering):
     """
-    Methods to link actions <-> response of the GUI.
+    A subclass of GuiRendering that provides specific functionalities for
+    interacting with the GUI elements in Broh5.
+
+    This class handles user actions such as file selection, branch/leaf
+    selection in an HDF tree, image saving, or data display; resets and
+    updates the GUI in response to these interactions.
+
+    Attributes
+    ----------
+    current_state : tuple or None
+        Current state of the GUI: file path, HDF key, slider values, ...
+    columns : list or None
+        Columns for displaying data in a table.
+    rows : list or None
+        Rows for displaying data in a table.
+    image : np.ndarray or None
+        Current slice from a 3D dataset.
+    current_slice : tuple or None
+        Information about the current slice being displayed.
+    data_1d_2d : np.ndarray or None
+        Current 1D or 2D data being displayed.
+    timer : UI object
+        To update the GUI in regular intervals.
+
+    Methods
+    -------
+    show_key(ValueChangeEventArguments, str)
+        Display the key of the HDF dataset/group when a tree node is clicked.
+    pick_file()
+        Open a file picker dialog to select a file.
+    display_hdf_tree(str)
+        Display the HDF file structure as an interactive tree.
+    disable_sliders()
+        Disable and reset the sliders for 3D-data slicing.
+    enable_ui_elements_3d_data()
+        Enable UI elements specific to 3D-data display.
+    enable_ui_elements_1d_2d_data()
+        Enable UI elements specific to 1D/2D data display.
+    reset(keep_display=False)
+        Reset the UI elements to their initial states.
+    reset_min_max()
+        Reset the minimum and maximum sliders for image contrast.
+    display_3d_data(data_obj)
+        Display a slice of a 3D dataset as an image.
+    display_1d_2d_data(data_obj, "plot")
+        Display 1D/2D data as a plot or table.
+    show_data()
+        Display data from an HDF file based on the current GUI state.
+    save_image()
+        Save the currently displayed image to a file.
+    save_data()
+        Save the currently displayed 1D/2D data to a file.
+    shutdown()
+        Routine to close the app.
     """
 
     def __init__(self):
         super().__init__()
         self.select_file_button.on("click", self.pick_file)
         self.save_image_button.on("click", self.save_image)
         self.save_data_button.on("click", self.save_data)
         self.reset_button.on("click", self.reset_min_max)
         self.current_state = None
         self.columns = None
         self.rows = None
         self.image = None
         self.current_slice = None
         self.data_1d_2d = None
-        ui.timer(re.UPDATE_RATE, lambda: self.show_data())
+        self.timer = ui.timer(re.UPDATE_RATE, lambda: self.show_data())
+        self.tab_one.on("click", self.select_tab_one)
+        self.tab_two.on("click", self.select_tab_two)
+        self.selected_tab = 1
+        self.last_folder = ""
+
+    def select_tab_one(self):
+        self.selected_tab = 1
+
+    def select_tab_two(self):
+        self.selected_tab = 2
 
     def show_key(self, event: ValueChangeEventArguments, file_path):
         """
         Show key to a dataset/group of a hdf file when users click
         to a branch of the hdf tree.
         """
         hdf_key = event.value
@@ -40,17 +107,32 @@
         else:
             self.hdf_value_display.set_text("")
         if file_path is not None:
             self.file_path_display.set_text(file_path)
 
     async def pick_file(self) -> None:
         """To pick a file when click the button 'Select file' """
-        file_path = await FilePicker("~",
-                                     allowed_extensions=re.INPUT_EXT)
+        config_data = util.load_config()
+        if config_data is None:
+            self.last_folder = ""
+        else:
+            try:
+                self.last_folder = config_data["last_folder"]
+            except KeyError:
+                self.last_folder = ""
+        if (self.last_folder == "") or (not os.path.exists(self.last_folder)):
+            file_path = await FilePicker("~",
+                                         allowed_extensions=re.INPUT_EXT)
+        else:
+            file_path = await FilePicker(self.last_folder,
+                                         allowed_extensions=re.INPUT_EXT)
         if file_path:
+            self.last_folder = os.path.dirname(file_path)
+            config_data = {'last_folder': self.last_folder}
+            util.save_config(config_data)
             self.display_hdf_tree(file_path)
 
     def display_hdf_tree(self, file_path):
         """Display interactive tree structure of a hdf file"""
         with self.tree_container:
             file_path = file_path.replace("\\", "/")
             self.file_path_display.set_text(file_path)
@@ -96,14 +178,16 @@
         self.main_slider.enable()
         self.max_slider.enable()
         self.min_slider.enable()
         self.main_plot.set_visibility(True)
         self.axis_list.enable()
         self.cmap_list.enable()
         self.save_image_button.enable()
+        self.histogram_plot.set_visibility(True)
+        self.image_info_table.set_visibility(True)
 
         # Disable other ui-components
         self.main_table.set_visibility(False)
         self.display_type.disable()
         self.marker_list.disable()
         self.save_data_button.disable()
         self.data_1d_2d = None
@@ -117,19 +201,23 @@
         # Disable ui-components related to image show
         self.disable_sliders()
         self.axis_list.value = re.AXIS_LIST[0]
         self.cmap_list.value = re.CMAP_LIST[0]
         self.axis_list.disable()
         self.cmap_list.disable()
         self.save_image_button.disable()
+        self.histogram_plot.set_visibility(False)
+        self.image_info_table.set_visibility(False)
 
         # Enable other ui-components
         self.display_type.enable()
         self.marker_list.enable()
         self.save_data_button.enable()
+        self.panel_tabs.set_value(self.tab_one)
+        self.selected_tab = 1
 
     def reset(self, keep_display=False):
         """Reset status of UI-elements"""
         if not keep_display:
             self.hdf_key_display.set_text("")
             self.file_path_display.set_text("")
             self.hdf_value_display.set_text("")
@@ -144,14 +232,18 @@
         self.disable_sliders()
         self.rows, self.columns = None, None
         self.image, self.data_1d_2d = None, None
         self.main_table.set_visibility(False)
         self.main_plot.set_visibility(True)
         self.save_image_button.disable()
         self.save_data_button.disable()
+        self.histogram_plot.set_visibility(False)
+        self.image_info_table.set_visibility(False)
+        self.panel_tabs.set_value(self.tab_one)
+        self.selected_tab = 1
 
     def reset_min_max(self):
         """Reset minimum and maximum values of sliders"""
         self.min_slider.set_value(0)
         self.max_slider.set_value(255)
 
     def display_3d_data(self, data_obj):
@@ -200,20 +292,42 @@
             if nmax != nmin:
                 image1 = np.uint8(255.0 * (self.image - nmin) / (nmax - nmin))
                 image1 = np.clip(image1, min_val, max_val)
             else:
                 image1 = np.zeros(self.image.shape)
         else:
             image1 = np.copy(self.image)
+
         with self.main_plot:
             plt.clf()
             plt.imshow(image1, cmap=self.cmap_list.value)
             plt.tight_layout()
             self.main_plot.update()
 
+        if self.selected_tab == 2:
+            rows = util.format_statistical_info(self.image)[0]
+            if self.image_info_table.rows is None:
+                self.image_info_table._props["rows"] = rows
+            else:
+                self.image_info_table.rows[:] = rows
+            self.image_info_table.update()
+            with self.histogram_plot:
+                plt.clf()
+                flat_data = self.image.ravel()
+                num_bins = min(255, len(flat_data))
+                hist, bin_edges = np.histogram(flat_data, bins=num_bins)
+                plt.hist(bin_edges[:-1], bins=bin_edges, weights=hist,
+                         color='skyblue', edgecolor='black', alpha=0.65,
+                         label=f"Num bins: {num_bins}")
+                plt.title("Histogram")
+                plt.xlabel("Grayscale")
+                plt.ylabel("Frequency")
+                plt.legend()
+                self.histogram_plot.update()
+
     def display_1d_2d_data(self, data_obj, disp_type="plot"):
         """Display 1d/2d array as a table or plot"""
         self.enable_ui_elements_1d_2d_data()
         self.data_1d_2d = data_obj[:]
         if disp_type == "table":
             self.main_plot.set_visibility(False)
             self.main_table.set_visibility(True)
@@ -239,73 +353,79 @@
                     img = True
             else:
                 size = len(data_obj)
                 x, y = np.arange(size), np.asarray(data_obj[:])
             if x is not None:
                 with self.main_plot:
                     plt.clf()
+                    plt.rcParams["font.family"] = "Arial"
                     title = self.hdf_key_display.text.split("/")[-1]
                     plt.title(title.capitalize())
                     plt.plot(x, y, marker=self.marker_list.value,
                              color=re.PLOT_COLOR)
                     plt.tight_layout()
                     self.main_plot.update()
+                    plt.rcdefaults()
             if img:
                 with self.main_plot:
                     plt.clf()
+                    plt.rcParams["font.family"] = "Arial"
                     plt.imshow(data_obj[:], cmap=self.cmap_list.value,
                                aspect="auto")
                     plt.tight_layout()
                     self.main_plot.update()
+                    plt.rcdefaults()
+
+    def __clear_plot(self):
+        with self.main_plot:
+            plt.clf()
+            self.main_plot.update()
+        with self.histogram_plot:
+            plt.clf()
+            self.histogram_plot.update()
 
     def show_data(self):
         """Display data getting from a hdf file"""
         file_path1 = self.file_path_display.text
         hdf_key1 = self.hdf_key_display.text
         if (file_path1 != "") and (hdf_key1 != "") and (hdf_key1 is not None):
             new_state = (file_path1, hdf_key1, self.main_slider.value,
                          self.hdf_value_display.text, self.axis_list.value,
                          self.cmap_list.value, self.display_type.value,
                          self.marker_list.value, self.min_slider.value,
-                         self.max_slider.value)
+                         self.max_slider.value, self.selected_tab)
             if new_state != self.current_state:
                 self.current_state = new_state
                 try:
                     (data_type, value) = util.get_hdf_data(file_path1,
                                                            hdf_key1)
                     if (data_type == "string" or data_type == "number"
                             or data_type == "boolean"):
                         self.hdf_value_display.set_text(str(value))
-                        with self.main_plot:
-                            plt.clf()
-                            self.main_plot.update()
+                        self.__clear_plot()
                         self.reset(keep_display=True)
                     elif data_type == "array":
                         self.hdf_value_display.set_text("Array shape: "
                                                         "" + str(value))
                         hdf_obj = h5py.File(file_path1, "r")
                         dim = len(value)
                         if dim == 3:
                             self.display_3d_data(hdf_obj[hdf_key1])
                         elif dim < 3:
                             self.display_1d_2d_data(
                                 hdf_obj[hdf_key1],
                                 disp_type=self.display_type.value)
                         else:
                             ui.notify("Can't display {}-d array!".format(dim))
-                            with self.main_plot:
-                                plt.clf()
-                                self.main_plot.update()
+                            self.__clear_plot()
                             self.reset(keep_display=True)
                         hdf_obj.close()
                     else:
                         self.hdf_value_display.set_text(data_type)
-                        with self.main_plot:
-                            plt.clf()
-                            self.main_plot.update()
+                        self.__clear_plot()
                         self.reset(keep_display=True)
                 except Exception as error:
                     self.reset(keep_display=True)
                     _, broken_link, msg = util.check_external_link(file_path1,
                                                                    hdf_key1)
                     if broken_link:
                         ui.notify(msg)
@@ -317,23 +437,26 @@
                         else:
                             ui.notify("Error: {}".format(error))
                             ui.notify("Dataset may be an external link and the"
                                       " target file is not accessible (moved, "
                                       "deleted, or corrupted) !!!")
         else:
             self.hdf_value_display.set_text("")
-            with self.main_plot:
-                plt.clf()
-                self.main_plot.update()
+            self.__clear_plot()
             self.reset(keep_display=True)
 
     async def save_image(self) -> None:
         """To save a slice to file when click 'Save image' """
-        file_path = await FileSaver("~", title="File name (ext: .tif, "
-                                               ".jpg, .png, or .csv)")
+        if (self.last_folder == "") or (not os.path.exists(self.last_folder)):
+            file_path = await FileSaver("~", title="File name (ext: .tif, "
+                                                   ".jpg, .png, or .csv)")
+        else:
+            file_path = await FileSaver(self.last_folder,
+                                        title="File name (ext: .tif, "
+                                              ".jpg, .png, or .csv)")
         if file_path and self.image is not None:
             file_ext = os.path.splitext(file_path)[-1]
             if (file_ext != ".tif" and file_ext != ".jpg"
                     and file_ext != ".png" and file_ext != ".csv"):
                 ui.notify("Please use .tif, .jpg, .png, or .csv as "
                           "file extension!")
             else:
@@ -349,15 +472,19 @@
                         ui.notify(
                             "File {} is overwritten".format(file_path))
                     else:
                         ui.notify("File is saved at: {}".format(file_path))
 
     async def save_data(self) -> None:
         """To save data to file when click the button 'Save data' """
-        file_path = await FileSaver("~", title="File name (ext: .csv)")
+        if (self.last_folder == "") or (not os.path.exists(self.last_folder)):
+            file_path = await FileSaver("~", title="File name (ext: .csv)")
+        else:
+            file_path = await FileSaver(self.last_folder,
+                                        title="File name (ext: .csv)")
         if file_path and self.data_1d_2d is not None:
             file_ext = os.path.splitext(file_path)[-1]
             if file_ext == "":
                 file_ext = ".csv"
                 file_path = file_path + file_ext
             if file_ext != ".csv":
                 ui.notify("Please use .csv as file extension!")
@@ -369,7 +496,12 @@
                 else:
                     if check:
                         ui.notify(
                             "File {} is overwritten".format(file_path))
                     else:
                         ui.notify(
                             "File is saved at: {}".format(file_path))
+
+    def shutdown(self):
+        """Routine to close the app"""
+        self.timer.cancel()
+        ui.notify("The server has been stopped. You can close this tab!")
```

### Comparing `broh5-1.1.0/broh5/lib/rendering.py` & `broh5-1.2.0/broh5/lib/rendering.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Module for GUI components:
+Module for constructing GUI components:
     -   Main window.
     -   Dialog for selecting a file.
     -   Dialog for saving a file.
 """
 
 import os
 import string
@@ -24,35 +24,90 @@
 AXIS_LIST = [0, 1, 2]
 FONT_STYLE = "font-size: 105%; font-weight: bold"
 DISPLAY_TYPE = ["plot", "table"]
 UPDATE_RATE = 0.2  # second
 DPI = 96
 RATIO = 0.65  # Ratio for adjusting size between image/plot and screen
 MAX_FIG_SIZE = [12.0, 9.0]
+MAX_PLOT_SIZE = [9.0, 7.0]
 INPUT_EXT = ["hdf", "nxs", "h5", "hdf5"]
 PLOT_COLOR = "blue"
 HEADER_COLOR = "#3874c8"
 HEADER_TITLE = "BROWSER-BASED HDF VIEWER"
 LEFT_DRAWER_COLOR = "#d7e3f4"
 TREE_BGR_COLOR = "#f8f8ff"
 
 
 class GuiRendering:
     """
-    Build the GUI
-    """
+    A class to build the graphical user interface for an HDF viewer.
+
+    This class creates various UI elements like headers, buttons,
+    sliders, tables, and plots to facilitate user interaction with HDF data.
 
+    Attributes
+    ----------
+    fig_size : tuple
+        Dimensions for the figure in the UI.
+    plot_size : tuple
+        Dimensions for the histogram plot in the UI.
+    tree_container : UI column
+        Container for the HDF tree structure.
+    select_file_button : UI button
+        Button to trigger file selection.
+    file_path_display : UI label
+        Label to display selected file path.
+    hdf_key_display : UI label
+        Label to display HDF key.
+    hdf_value_display : UI label
+        Label to display HDF value.
+    axis_list : UI select
+        Dropdown to select axis for slicing.
+    cmap_list : UI select
+        Dropdown to select color map for plots.
+    save_image_button : UI button
+        Button to save current image.
+    display_type : UI select
+        Dropdown to choose the display type (plot or table).
+    marker_list : UI select
+        Dropdown to select marker type for plots.
+    save_data_button : UI button
+        Button to save current data.
+    main_slider : UI slider
+        Slider to navigate through slices of 3D data.
+    main_table : UI table
+        Table to display data in tabular form.
+    main_plot : UI pyplot
+        Pyplot element to display plots.
+    min_slider : UI slider
+        Slider to adjust the minimum value for image contrast.
+    max_slider : UI slider
+        Slider to adjust the maximum value for image contrast.
+    reset_button : UI button
+        Button to reset adjustments.
+    histogram_plot : UI pyplot
+        Pyplot element to display histogram of an image.
+    image_info_table : UI table
+        Table to display statistical information of an image.
+
+    Methods
+    -------
+    init_gui()
+        Initializes and constructs the GUI elements.
+    """
     def __init__(self):
         super().__init__()
         # Initial parameters
         (sc_height, sc_width) = util.get_height_width_screen()
         hei_size = RATIO * sc_width / DPI
         wid_size = RATIO * sc_height / DPI
         self.fig_size = (min(hei_size, MAX_FIG_SIZE[0]),
                          min(wid_size, MAX_FIG_SIZE[1]))
+        self.plot_size = (min(hei_size, MAX_PLOT_SIZE[0]),
+                          min(wid_size, MAX_PLOT_SIZE[1]))
         self.tree_container = None
         self.select_file_button = None
         self.file_path_display = None
         self.hdf_key_display = None
         self.hdf_value_display = None
         self.axis_list = None
         self.cmap_list = None
@@ -62,17 +117,28 @@
         self.save_data_button = None
         self.main_slider = None
         self.main_table = None
         self.main_plot = None
         self.min_slider = None
         self.max_slider = None
         self.reset_button = None
+        self.histogram_plot = None
+        self.image_info_table = None
+        self.tab_one = None
+        self.tab_two = None
+        self.panel_tabs = None
         self.init_gui()
 
     def init_gui(self):
+        """
+        Initializes and constructs the various elements of the GUI.
+
+        This method sets up headers, drawers, rows, labels, buttons, sliders,
+        tables, and plots to create an interactive user interface.
+        """
         # For the header
         with ui.header().style("background-color: " + HEADER_COLOR).classes(
                 "items-center justify-between"):
             ui.label(HEADER_TITLE).style(FONT_STYLE)
 
         # For the left drawer, used to display a hdf tree.
         with ui.left_drawer(fixed=True, bottom_corner=True).style(
@@ -124,65 +190,98 @@
             with ui.row().classes("w-full items-center no-wrap"):
                 ui.label("Slice: ").style(FONT_STYLE)
                 self.main_slider = ui.slider(min=0, max=100, value=0).props(
                     "label-always").on("update:model-value",
                                        throttle=UPDATE_RATE,
                                        leading_events=False)
 
-            # For display data as an image, table, or plot
-            self.main_table = ui.table(columns=None, rows=None,
-                                       row_key="Index")
-            self.main_plot = ui.pyplot(figsize=self.fig_size,
-                                       close=False).classes("w-full")
-
-            # Sliders for adjust the contrast of an image.
-            with ui.row().classes(
-                    "w-full justify-between no-wrap items-center"):
-                ui.label("Min: ").style(FONT_STYLE)
-                self.min_slider = ui.slider(min=0, max=254, value=0).props(
-                    "label-always").on("update:model-value",
-                                       throttle=UPDATE_RATE,
-                                       leading_events=False)
-
-                ui.label("Max: ").style(FONT_STYLE)
-                self.max_slider = ui.slider(min=1, max=255, value=255).props(
-                    "label-always").on("update:model-value",
-                                       throttle=UPDATE_RATE,
-                                       leading_events=False)
-                self.reset_button = ui.button("Reset")
+            # Tabs for data visualization and displaying image information
+            tabs = ui.tabs().classes('w-full')
+            with tabs:
+                self.tab_one = ui.tab('Data visualization').style(
+                    "background-color: " + TREE_BGR_COLOR)
+                self.tab_two = ui.tab('Image information').style(
+                    "background-color: " + TREE_BGR_COLOR)
+            self.panel_tabs = ui.tab_panels(tabs, value=self.tab_one).classes(
+                'w-full')
+            with self.panel_tabs:
+                # Tab 1 for data visualization
+                with ui.tab_panel(self.tab_one):
+                    # For display data as an image, table, or plot
+                    self.main_table = ui.table(columns=None, rows=None,
+                                               row_key="Index")
+                    self.main_plot = ui.pyplot(figsize=self.fig_size,
+                                               close=False).classes("w-full")
+
+                    # Sliders for adjust the contrast of an image.
+                    with ui.row().classes(
+                            "w-full justify-between no-wrap items-center"):
+                        ui.label("Min: ").style(FONT_STYLE)
+                        self.min_slider = ui.slider(min=0, max=254,
+                                                    value=0).props(
+                            "label-always").on("update:model-value",
+                                               throttle=UPDATE_RATE,
+                                               leading_events=False)
+
+                        ui.label("Max: ").style(FONT_STYLE)
+                        self.max_slider = ui.slider(min=1, max=255,
+                                                    value=255).props(
+                            "label-always").on("update:model-value",
+                                               throttle=UPDATE_RATE,
+                                               leading_events=False)
+                        self.reset_button = ui.button("Reset")
+                # Tab 2 for showing image information
+                with ui.tab_panel(self.tab_two):
+                    with ui.row().classes(
+                            "w-full justify-between no-wrap items-center"):
+                        self.histogram_plot = ui.pyplot(figsize=self.plot_size,
+                                                        close=False,
+                                                        ).classes("w-full")
+                        self.image_info_table = ui.table(columns=None,
+                                                         rows=None,
+                                                         row_key="name")
 
 
 class FilePicker(ui.dialog):
-
+    """
+    A dialog class for file picking in the GUI. Codes are adapted from an
+    example of NiceGUI:
+    https://github.com/zauberzeug/nicegui/tree/main/examples/local_file_picker
+
+    Allows users to browse and select files from the local filesystem where
+    the application is running.
+
+    Parameters
+    ----------
+    directory : str
+        The starting directory for the file picker.
+    upper_limit : str, optional
+        The upper directory limit for browsing. None by default.
+    show_hidden_files : bool, optional
+        Flag to show hidden files. False by default.
+    allowed_extensions : List of str, optional
+        List of allowed file extensions for filtering. None by default.
+
+    Methods
+    -------
+    check_extension(filename: str)
+        Check if the given filename has an allowed extension.
+    add_drives_toggle()
+        Add a toggle for drive selection on Windows systems.
+    update_grid()
+        Update the file grid based on the current directory and filters.
+    handle_double_click(GenericEventArguments)
+        Handle double click events on the file grid.
+    handle_ok()
+        Handle the OK button, click to submit the selected file path.
+    """
     def __init__(self, directory: str, *,
                  upper_limit: Optional[str] = None,
                  show_hidden_files: bool = False,
                  allowed_extensions: Optional[List[str]] = None) -> None:
-        """
-        This is a simple file picker that allows users to select a file from
-        the local filesystem where the app is running.
-        Codes are adapted from an example of NiceGUI:
-        https://github.com/zauberzeug/nicegui/tree/main/examples/local_file_picker
-
-        Parameters
-        ----------
-
-        directory : str
-            Starting directory.
-        upper_limit : str
-            Stopping directory (None: no limit).
-        show_hidden_files : bool
-            Whether to show hidden files.
-        allowed_extensions : list of str
-            Only show files with given extension. E.g. ['hdf', 'h5', 'nxs']
-
-        Returns
-        -------
-            file path.
-        """
         super().__init__()
         self.show_hidden_files = show_hidden_files
         self.allowed_extensions = allowed_extensions
         self.drives_toggle = None
         self.path = Path(directory).expanduser()
         if upper_limit is None:
             self.upper_limit = None
@@ -208,16 +307,20 @@
             return filename.split('.')[-1].lower() in self.allowed_extensions
 
     def add_drives_toggle(self):
         """Give a list of available drivers in a WinOS computer"""
         if platform.system() == 'Windows':
             drives = ['%s:\\' % d for d in string.ascii_uppercase if
                       os.path.exists('%s:' % d)]
-            self.path = Path(drives[0]).expanduser()
-            self.drives_toggle = ui.toggle(drives, value=drives[0],
+            if self.path != "" or self.path != ".":
+                select_drive = os.path.splitdrive(self.path)[0] + "\\"
+            else:
+                self.path = Path(drives[0]).expanduser()
+                select_drive = drives[0]
+            self.drives_toggle = ui.toggle(drives, value=select_drive,
                                            on_change=self.__update_drive)
 
     def __update_drive(self):
         if self.drives_toggle:
             self.path = Path(self.drives_toggle.value).expanduser()
             self.update_grid()
 
@@ -251,54 +354,66 @@
             if self.path:
                 self.submit(str(self.path))
             else:
                 return
 
     async def handle_ok(self):
         try:
-            rows = await ui.run_javascript(
-                f'getElement({self.grid.id}).gridOptions.api.getSelectedRows()')
+            self.update_grid()
+            rows = await self.grid.get_selected_rows()
             if rows:
                 fpath = [r['path'] for r in rows]
                 if fpath:
                     self.submit(fpath[0])
                 else:
                     ui.notify("No file path found in the selected rows")
                     return
             else:
-                ui.notify("No rows selected.")
+                ui.notify("No rows selected. Try double-click instead !!!")
                 return
         except Exception as e:
             ui.notify(f"An error occurred: {e}")
             return
 
 
 class FileSaver(ui.dialog):
+    """
+    A dialog class for saving files in the GUI.
 
+    Allows users to specify a file name and directory for saving files.
+
+    Parameters
+    ----------
+    directory : str
+        Starting directory for the file saver.
+    upper_limit : str, optional
+        Upper directory limit for browsing. None by default.
+    show_hidden_files : bool, optional
+        Flag to show hidden files. False by default.
+    title : str, optional
+        Title for the file-name input-field. 'File name' by default.
+
+    Methods
+    -------
+    add_drives_toggle()
+        Add a toggle for drive selection on Windows systems.
+    update_grid() -> None
+        Update the file grid based on the current directory.
+    handle_double_click(e: GenericEventArguments) -> None
+        Handle double-click events on the file grid.
+    handle_save()
+        Handle the Save button, click to submit the specified file path.
+    create_folder_dialog()
+        Open a dialog for creating a new folder.
+    create_folder(folder_name: str, dialog: ui.dialog)
+        Create a new folder with the specified name.
+    """
     def __init__(self, directory: str, *, upper_limit: Optional[str] = None,
                  show_hidden_files: bool = False,
                  title: Optional[str] = 'File name') -> None:
-        """
-        This is a simple file saver dialog that allows users to specify a
-        file name and where the file should be saved.
-
-        Parameters
-        ----------
-
-        directory : str
-            Starting directory.
-        upper_limit : str
-            Stopping directory (None: no limit).
-        show_hidden_files : bool
-            Whether to show hidden files.
-
-        Returns
-        -------
-            file path.
-        """
         super().__init__()
         self.show_hidden_files = show_hidden_files
         self.drives_toggle = None
         self.path = Path(directory).expanduser()
         self.title = title
         if upper_limit is None:
             self.upper_limit = None
@@ -324,16 +439,20 @@
         self.update_grid()
 
     def add_drives_toggle(self):
         """Give a list of available drivers in a WinOS computer"""
         if platform.system() == 'Windows':
             drives = ['%s:\\' % d for d in string.ascii_uppercase if
                       os.path.exists('%s:' % d)]
-            self.path = Path(drives[0]).expanduser()
-            self.drives_toggle = ui.toggle(drives, value=drives[0],
+            if self.path != "" or self.path != ".":
+                select_drive = os.path.splitdrive(self.path)[0] + "\\"
+            else:
+                self.path = Path(drives[0]).expanduser()
+                select_drive = drives[0]
+            self.drives_toggle = ui.toggle(drives, value=select_drive,
                                            on_change=self.__update_drive)
 
     def __update_drive(self):
         if self.drives_toggle:
             self.path = Path(self.drives_toggle.value).expanduser()
             self.update_grid()
```

### Comparing `broh5-1.1.0/broh5/main.py` & `broh5-1.2.0/broh5/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,51 +17,93 @@
 Type: broh5 to run the software
 Exit the software by pressing: Ctrl + C
 
 ===============================================================================
 """
 
 
-def handle_shutdown():
+def handle_shutdown(main_app):
+    """
+    Handle the shutdown process of the application.
+    """
+    main_app.shutdown()
     print("\n===============")
     print(" Exit the app!")
     print("===============\n")
 
 
 def signal_handler(*args):
-    handle_shutdown()
+    """
+    Handle the signal for graceful shutdown of the application.
+
+    Parameters
+    ----------
+    *args
+        Variable length argument list.
+    """
     sys.exit(0)
 
 
 def check_port(port):
+    """
+    Check if a given port is available.
+
+    Parameters
+    ----------
+    port : int
+        The port number to check.
+
+    Returns
+    -------
+    bool
+        True if the port is already in use, False otherwise.
+    """
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
         return s.connect_ex(('localhost', port)) == 0
 
 
 def parse_args():
+    """
+    Parse command-line arguments.
+
+    Returns
+    -------
+    argparse.Namespace
+        Parsed arguments.
+    """
     parser = argparse.ArgumentParser(description=display_msg,
                                      formatter_class=
                                      argparse.RawDescriptionHelpFormatter)
     parser.add_argument("--version", action="version",
                         version=f"%(prog)s {__version__}")
     parser.add_argument("--port", type=int, default=8180,
                         help="Specify the port to run broh5 on "
                              "(default: 8180)")
     args = parser.parse_args()
     return args
 
 
 def main():
-    signal.signal(signal.SIGINT, signal_handler)
+    """
+    Main function to start the application.
+    """
     args = parse_args()
     if check_port(args.port):
         print("\n!!! Port {} is already in use. Please specify a "
               "different port using --port !!!\n".format(args.port))
         sys.exit(1)
-    GuiInteraction()
-    os.environ["NO_NETIFACES"] = "True"
-    app.on_shutdown(handle_shutdown)
-    ui.run(reload=False, title="Browser-based Hdf Viewer", port=args.port)
+    signal.signal(signal.SIGINT, signal_handler)  # Back-up shutdown
+    try:
+        broh5_app = GuiInteraction()
+        os.environ["NO_NETIFACES"] = "True"
+        app.on_shutdown(lambda: handle_shutdown(broh5_app))
+        app.on_startup(
+            lambda: print("Access Broh5 at urls: {}".format(app.urls.union())))
+        ui.run(reload=False, title="Browser-based Hdf Viewer", port=args.port,
+               show_welcome_message=False)
+    except Exception as error:
+        print(f"An error occurred: {error}")
+        sys.exit(0)
 
 
 if __name__ in {"__main__", "__mp_main__"}:
     main()
```

### Comparing `broh5-1.1.0/setup.py` & `broh5-1.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 
 dependencies = [
     "numpy>1.21",
     "h5py>3.7",
     "hdf5plugin",
     "pillow",
     "matplotlib",
-    "nicegui>1.3.16"
+    "nicegui>1.4.5"
 ]
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setuptools.setup(
     name="broh5",
-    version="1.1.0",
+    version="1.2.0",
     author="Nghia Vo",
     author_email="nvo@bnl.gov",
     description='Browser-based GUI HDF Viewer in Python',
     long_description=README,
     long_description_content_type="text/markdown",
     keywords=['HDF Viewer', 'NXS Viewer', 'Browser-based GUI'],
-    url="https://github.com/nghia-vo/broh5",
-    download_url="https://github.com/nghia-vo/broh5.git",
+    url="https://github.com/algotom/broh5",
+    download_url="https://github.com/algotom/broh5.git",
     license="Apache 2.0",
     platforms="Any",
     packages=setuptools.find_packages(include=["broh5", "broh5.*"]),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Intended Audience :: Science/Research",
```


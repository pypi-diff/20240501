# Comparing `tmp/phylo_match-0.1.0.tar.gz` & `tmp/phylo_match-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phylo_match-0.1.0.tar", last modified: Mon Apr 29 18:40:53 2024, max compression
+gzip compressed data, was "phylo_match-0.1.1.tar", last modified: Tue Apr 30 16:13:00 2024, max compression
```

## Comparing `phylo_match-0.1.0.tar` & `phylo_match-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 williamspear   (501) staff       (20)        0 2024-04-29 18:40:53.169985 phylo_match-0.1.0/
--rw-r--r--   0 williamspear   (501) staff       (20)    32474 2022-06-23 17:16:36.000000 phylo_match-0.1.0/COPYING
--rw-r--r--   0 williamspear   (501) staff       (20)     4714 2024-04-29 18:40:53.169910 phylo_match-0.1.0/PKG-INFO
--rw-r--r--   0 williamspear   (501) staff       (20)     4126 2024-04-29 18:38:43.000000 phylo_match-0.1.0/README.md
-drwxr-xr-x   0 williamspear   (501) staff       (20)        0 2024-04-29 18:40:53.167660 phylo_match-0.1.0/phylo_match/
--rw-r--r--   0 williamspear   (501) staff       (20)        0 2024-04-28 04:50:14.000000 phylo_match-0.1.0/phylo_match/__init__.py
-drwxr-xr-x   0 williamspear   (501) staff       (20)        0 2024-04-29 18:40:53.169020 phylo_match-0.1.0/phylo_match/definitions/
--rw-r--r--   0 williamspear   (501) staff       (20)        0 2022-06-23 17:16:36.000000 phylo_match-0.1.0/phylo_match/definitions/__init__.py
--rw-r--r--   0 williamspear   (501) staff       (20)     1065 2022-06-23 17:16:36.000000 phylo_match-0.1.0/phylo_match/definitions/definitions.py
--rw-r--r--   0 williamspear   (501) staff       (20)    27936 2024-04-29 18:26:17.000000 phylo_match-0.1.0/phylo_match/gui.py
-drwxr-xr-x   0 williamspear   (501) staff       (20)        0 2024-04-29 18:40:53.169391 phylo_match-0.1.0/phylo_match/match/
--rw-r--r--   0 williamspear   (501) staff       (20)        0 2024-04-28 04:50:14.000000 phylo_match-0.1.0/phylo_match/match/__init__.py
--rw-r--r--   0 williamspear   (501) staff       (20)     8622 2024-04-29 18:19:49.000000 phylo_match-0.1.0/phylo_match/match/match.py
-drwxr-xr-x   0 williamspear   (501) staff       (20)        0 2024-04-29 18:40:53.169702 phylo_match-0.1.0/phylo_match.egg-info/
--rw-r--r--   0 williamspear   (501) staff       (20)     4714 2024-04-29 18:40:53.000000 phylo_match-0.1.0/phylo_match.egg-info/PKG-INFO
--rw-r--r--   0 williamspear   (501) staff       (20)      429 2024-04-29 18:40:53.000000 phylo_match-0.1.0/phylo_match.egg-info/SOURCES.txt
--rw-r--r--   0 williamspear   (501) staff       (20)        1 2024-04-29 18:40:53.000000 phylo_match-0.1.0/phylo_match.egg-info/dependency_links.txt
--rw-r--r--   0 williamspear   (501) staff       (20)       53 2024-04-29 18:40:53.000000 phylo_match-0.1.0/phylo_match.egg-info/entry_points.txt
--rw-r--r--   0 williamspear   (501) staff       (20)       47 2024-04-29 18:40:53.000000 phylo_match-0.1.0/phylo_match.egg-info/requires.txt
--rw-r--r--   0 williamspear   (501) staff       (20)       12 2024-04-29 18:40:53.000000 phylo_match-0.1.0/phylo_match.egg-info/top_level.txt
--rw-r--r--   0 williamspear   (501) staff       (20)      213 2022-06-23 17:16:36.000000 phylo_match-0.1.0/pyproject.toml
--rw-r--r--   0 williamspear   (501) staff       (20)      705 2024-04-29 18:40:53.170257 phylo_match-0.1.0/setup.cfg
+drwxr-xr-x   0 williamspear   (501) staff       (20)        0 2024-04-30 16:13:00.493449 phylo_match-0.1.1/
+-rw-r--r--   0 williamspear   (501) staff       (20)    32474 2022-06-23 17:16:36.000000 phylo_match-0.1.1/COPYING
+-rw-r--r--   0 williamspear   (501) staff       (20)     4775 2024-04-30 16:13:00.493389 phylo_match-0.1.1/PKG-INFO
+-rw-r--r--   0 williamspear   (501) staff       (20)     4187 2024-04-29 22:49:12.000000 phylo_match-0.1.1/README.md
+drwxr-xr-x   0 williamspear   (501) staff       (20)        0 2024-04-30 16:13:00.491416 phylo_match-0.1.1/phylo_match/
+-rw-r--r--   0 williamspear   (501) staff       (20)        0 2024-04-28 04:50:14.000000 phylo_match-0.1.1/phylo_match/__init__.py
+drwxr-xr-x   0 williamspear   (501) staff       (20)        0 2024-04-30 16:13:00.492568 phylo_match-0.1.1/phylo_match/definitions/
+-rw-r--r--   0 williamspear   (501) staff       (20)        0 2022-06-23 17:16:36.000000 phylo_match-0.1.1/phylo_match/definitions/__init__.py
+-rw-r--r--   0 williamspear   (501) staff       (20)     1065 2022-06-23 17:16:36.000000 phylo_match-0.1.1/phylo_match/definitions/definitions.py
+-rw-r--r--   0 williamspear   (501) staff       (20)    28763 2024-04-30 15:46:39.000000 phylo_match-0.1.1/phylo_match/gui.py
+drwxr-xr-x   0 williamspear   (501) staff       (20)        0 2024-04-30 16:13:00.492920 phylo_match-0.1.1/phylo_match/match/
+-rw-r--r--   0 williamspear   (501) staff       (20)        0 2024-04-28 04:50:14.000000 phylo_match-0.1.1/phylo_match/match/__init__.py
+-rw-r--r--   0 williamspear   (501) staff       (20)     9510 2024-04-30 16:10:09.000000 phylo_match-0.1.1/phylo_match/match/match.py
+drwxr-xr-x   0 williamspear   (501) staff       (20)        0 2024-04-30 16:13:00.493201 phylo_match-0.1.1/phylo_match.egg-info/
+-rw-r--r--   0 williamspear   (501) staff       (20)     4775 2024-04-30 16:13:00.000000 phylo_match-0.1.1/phylo_match.egg-info/PKG-INFO
+-rw-r--r--   0 williamspear   (501) staff       (20)      429 2024-04-30 16:13:00.000000 phylo_match-0.1.1/phylo_match.egg-info/SOURCES.txt
+-rw-r--r--   0 williamspear   (501) staff       (20)        1 2024-04-30 16:13:00.000000 phylo_match-0.1.1/phylo_match.egg-info/dependency_links.txt
+-rw-r--r--   0 williamspear   (501) staff       (20)       53 2024-04-30 16:13:00.000000 phylo_match-0.1.1/phylo_match.egg-info/entry_points.txt
+-rw-r--r--   0 williamspear   (501) staff       (20)       47 2024-04-30 16:13:00.000000 phylo_match-0.1.1/phylo_match.egg-info/requires.txt
+-rw-r--r--   0 williamspear   (501) staff       (20)       12 2024-04-30 16:13:00.000000 phylo_match-0.1.1/phylo_match.egg-info/top_level.txt
+-rw-r--r--   0 williamspear   (501) staff       (20)      213 2022-06-23 17:16:36.000000 phylo_match-0.1.1/pyproject.toml
+-rw-r--r--   0 williamspear   (501) staff       (20)      705 2024-04-30 16:13:00.493723 phylo_match-0.1.1/setup.cfg
```

### Comparing `phylo_match-0.1.0/COPYING` & `phylo_match-0.1.1/COPYING`

 * *Files identical despite different names*

### Comparing `phylo_match-0.1.0/PKG-INFO` & `phylo_match-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phylo-match
-Version: 0.1.0
+Version: 0.1.1
 Summary: For matching species databases
 Home-page: https://github.com/spearw/phylo-match
 Author: William Spear
 Author-email: spearw@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -45,14 +45,19 @@
 ```
 
 Install Phylo-Match:
 ```bash
 pip3 install phylo-match
 ```
 
+Upgrade Phylo-Match:
+```bash
+pip install phylo-match -U
+```
+
 
 ## Usage
 
 ```bash
 phylo-match
 ```
 Use the gui to select a database file (.csv), and a taxa tree (.nexus) to match the database to. Enter the number of your species column in the box, if the taxa you are matching are not in the first column (index counts from 0, so enter 0 for first column, 1 for second, etc.)
```

### Comparing `phylo_match-0.1.0/README.md` & `phylo_match-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,19 @@
 ```
 
 Install Phylo-Match:
 ```bash
 pip3 install phylo-match
 ```
 
+Upgrade Phylo-Match:
+```bash
+pip install phylo-match -U
+```
+
 
 ## Usage
 
 ```bash
 phylo-match
 ```
 Use the gui to select a database file (.csv), and a taxa tree (.nexus) to match the database to. Enter the number of your species column in the box, if the taxa you are matching are not in the first column (index counts from 0, so enter 0 for first column, 1 for second, etc.)
```

### Comparing `phylo_match-0.1.0/phylo_match/definitions/definitions.py` & `phylo_match-0.1.1/phylo_match/definitions/definitions.py`

 * *Files identical despite different names*

### Comparing `phylo_match-0.1.0/phylo_match/gui.py` & `phylo_match-0.1.1/phylo_match/gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 '''
 
 import sys
 import datetime
 
 from argparse import ArgumentParser
 
-from PyQt6.QtGui import QIntValidator
+from PyQt6.QtGui import QIntValidator, QCloseEvent
 from PyQt6.uic.properties import QtWidgets
 from diskcache import Cache
 from PyQt6.QtCore import Qt
 from PyQt6.QtWidgets import QApplication, QWidget, QPushButton, QVBoxLayout, \
     QHBoxLayout, QGridLayout, QLabel, QLineEdit
 from phylo_match.definitions.definitions import *
 from phylo_match.match.match import *
@@ -81,14 +81,15 @@
         self.progress_layout = QGridLayout()
         self.main_layout.addLayout(self.progress_layout, 2, 0, 1, 4)
 
         # Add progress bar and label
         self.prog_label = QLabel("")
         self.progress_layout.addWidget(self.prog_label)
         self.prog_bar = QProgressBar(self)
+        self.prog_bar.hide()
         self.prog_bar.setValue(0)
         self.progress_layout.addWidget(self.prog_bar)
 
         # Add db selection button
         self.db_label = QLabel("Database File Selection")
         self.db_label.setAlignment(Qt.AlignmentFlag.AlignBottom)
         self.db_label.setFixedHeight(self.db_label.font().pointSize()*2)
@@ -195,14 +196,15 @@
         # Might include other functionality, such as loading bar
         self.run_match()
 
     def run_match(self):
         compare_window = Compare(self)
 
         self.prog_label.setText("Analyzing...")
+        self.prog_bar.show()
         self.prog_bar.setValue(0)
         QApplication.processEvents()
 
         self.dialogs.append(compare_window)
 
         self.species_index = self.species_index_textbox.text()
         if self.species_index == '':
@@ -275,21 +277,26 @@
                 cache.set(key, value)
 
         self.prog_label.setText("Done!")
         QApplication.processEvents()
 
         compare_window.__init__(self)
         compare_window.setParent(self)
+        compare_window.move(self.pos())
         compare_window.species_index = self.species_index
         compare_window.set_db_path(self.db_path)
         compare_window.set_do_lookup(self.do_lookup.isChecked())
 
         compare_window.set_cache(cache)
         compare_window.compare_mismatch(iter(taxa_list))
+
         self.hide()
+        self.prog_bar.hide()
+        self.prog_bar.setValue(0)
+        self.prog_label.setText("")
 
 
 # dialog.close()
 
 #
 # start_time = time.time()
 # taxa_list = db_match(DB_PATH, TREE_PATH, "_", 4)
@@ -379,19 +386,33 @@
         self.manual_entry_layout.addWidget(self.leave_btn)
         self.manual_entry_layout.setContentsMargins(10, 10, 10, 10)
 
         # Init global variables
         self.removed_suggestions = []
         self.taxa_list = []
         self.species_index = 0
+        self.force_quit = False
+
+    def closeEvent(self, event, *args, **kwargs):
 
-    def closeEvent(self, *args, **kwargs):
-        print("Force exit by user")
-        ## TODO: Add pop up box with option to save progress
-        quit()
+        if self.force_quit:
+            event.accept()
+        else:
+            ## TODO: Add pop up box with option to save progress
+            close = QMessageBox.question(self,
+                                         "QUIT",
+                                         "Are you sure want to quit? Progress will not be saved",
+                                         QMessageBox.StandardButton.Yes | QMessageBox.StandardButton.No)
+            if close == QMessageBox.StandardButton.Yes:
+                # Open main menu
+                self.parent().show()
+                self.parent().move(self.pos())
+                event.accept()
+            else:
+                event.ignore()
 
     def set_db_path(self, db_path):
         self.db_path = db_path
 
     def set_do_lookup(self, do_lookup):
         self.do_lookup = do_lookup
 
@@ -415,17 +436,27 @@
 
                 self.show_suggestions(next_taxa, taxa_iter, i)
 
                 self.taxa_label.setText(db_taxa)
                 self.show()
         else:
             # End of file, record results
-            write_file(self.taxa_list, self.db_path, self.species_index)
+            filepath = write_file(self.taxa_list, self.db_path, self.species_index)
+
+            # Success message
+            QMessageBox.information(self,
+                                     "Complete!",
+                                     f"Selections saved as {filepath}",)
+
             # Open main menu
             self.parent().show()
+            self.parent().move(self.pos())
+
+            # Close window
+            self.force_quit = True
             self.close()
 
     def make_confirm_function(self, suggestion, taxa_iter, compare_window):
         def confirm_suggestion():
             self.taxa_list.append(suggestion)
 
             self.line_edit.clear()
@@ -546,100 +577,95 @@
         scroll.setWidgetResizable(True)
         scroll.setAlignment(Qt.AlignmentFlag.AlignCenter)
         scroll.setFixedHeight(400)
         scroll.setMaximumWidth(800)
 
         return scroll
 
-    def show_suggestions(self, next_taxa, taxa_iter, i):
+    def show_suggestions(self, next_taxa, taxa_iter, match_type):
 
         # Clear old buttons + count_layout
         for j in reversed(range(self.suggestions_sub_layout.count())):
             layout = self.suggestions_sub_layout.itemAt(j).layout()
             self.suggestions_sub_layout.removeItem(layout)
             for k in reversed(range(layout.count())):
                 layout.itemAt(k).widget().setParent(None)
 
         self.suggestions_scroll_area.setParent(None)
+        self.taxa_info.setParent(None)
 
 
         self.removed_suggestions_scroll_area.setParent(None)
         self.removed_suggestions_count.setText(f"Removed Suggestions: {len(self.removed_suggestions)}")
         if self.removed_suggestions:
             self.removed_suggestions_scroll_area = self.create_removed_suggestions_scroll_area(", \n".join(self.removed_suggestions))
             self.taxa_layout.addWidget(self.removed_suggestions_scroll_area, 1)
 
         num_suggestions = [len(next_taxa[1]), len(next_taxa[2]), len(next_taxa[3])]
 
-        if i <= 3:
-            category_suggestions = next_taxa[i]
-            while not category_suggestions:
-                i += 1
-                if i > 3:
-                    break
-                category_suggestions = next_taxa[i]
-
-            if i <= 3:
-                # reset and load taxa, if possible
-                self.taxa_info.setParent(None)
-
-                if self.do_lookup:
-                    self.taxa_info = self.create_wiki_scroll_area(next_taxa[0])
-                    h_layout = QHBoxLayout()
-                    h_layout.addWidget(self.taxa_info)
-                    self.taxa_layout.insertLayout(0, h_layout)
-
-                for suggestion in category_suggestions:
-
-                    # Add info and image widget to page
-                    suggestion_layout = self.create_taxa_layout(suggestion, taxa_iter)
-                    self.suggestions_sub_layout.addLayout(suggestion_layout)
-
-                self.suggestions_scroll_area = self.create_suggestions_scroll_area()
-                self.suggestions_scrolling_layout.addWidget(self.suggestions_scroll_area)
-
-
-                # Check that all category_suggestions were not removed by being previously picked, continue if they were
-                if not category_suggestions:
-                    i += 1
-                    self.show_suggestions(next_taxa, taxa_iter, i)
-
-            # TODO: get this logic outside of the category_suggestions, so it's not doing it every time
-            # Set button text
-            self.similar_entries_count.setText(f"Similar Entries: {num_suggestions[0]}")
-            self.same_species_count.setText(f"Same Species: {num_suggestions[1]}")
-            self.same_genus_count.setText(f"Same Genus: {num_suggestions[2]}")
-
-            # Unlink buttons, if needed
-            try:
-                self.similar_entries_count.clicked.disconnect()
-            except Exception:
-                pass
-            try:
-                self.same_species_count.clicked.disconnect()
-            except Exception:
-                pass
-            try:
-                self.same_genus_count.clicked.disconnect()
-            except Exception:
-                pass
-
-            # Link buttons, if category_suggestions exist for those categories
-            if num_suggestions[0] > 0: self.similar_entries_count.clicked.connect(
-                lambda: self.show_suggestions(next_taxa, taxa_iter, 1))
-            if num_suggestions[1] > 0: self.same_species_count.clicked.connect(
-                lambda: self.show_suggestions(next_taxa, taxa_iter, 2))
-            if num_suggestions[2] > 0: self.same_genus_count.clicked.connect(
-                lambda: self.show_suggestions(next_taxa, taxa_iter, 3))
+        category_suggestions = next_taxa[match_type]
+        while not category_suggestions:
+            match_type += 1
+            if match_type > 3:
+                break
+            category_suggestions = next_taxa[match_type]
+
+        # reset and load taxa, if possible
+        self.taxa_info.setParent(None)
+
+        if self.do_lookup:
+            self.taxa_info = self.create_wiki_scroll_area(next_taxa[0])
+            h_layout = QHBoxLayout()
+            h_layout.addWidget(self.taxa_info)
+            self.taxa_layout.insertLayout(0, h_layout)
+
+        for suggestion in category_suggestions:
+
+            # Add info and image widget to page
+            suggestion_layout = self.create_taxa_layout(suggestion, taxa_iter)
+            self.suggestions_sub_layout.addLayout(suggestion_layout)
+
+        self.suggestions_scroll_area = self.create_suggestions_scroll_area()
+        self.suggestions_scrolling_layout.addWidget(self.suggestions_scroll_area)
+
+
+        # TODO: get this logic outside of the category_suggestions, so it's not doing it every time
+        # Set button text
+        self.similar_entries_count.setText(f"Similar Entries: {num_suggestions[0]}")
+        self.same_species_count.setText(f"Same Species: {num_suggestions[1]}")
+        self.same_genus_count.setText(f"Same Genus: {num_suggestions[2]}")
+
+        # Unlink buttons, if needed
+        try:
+            self.similar_entries_count.clicked.disconnect()
+        except Exception:
+            pass
+        try:
+            self.same_species_count.clicked.disconnect()
+        except Exception:
+            pass
+        try:
+            self.same_genus_count.clicked.disconnect()
+        except Exception:
+            pass
+
+        # Link buttons, if category_suggestions exist for those categories
+        ## TODO: Refactor to use strings instead of ints for clearer indications of what these numbers mean
+        if num_suggestions[0] > 0: self.similar_entries_count.clicked.connect(
+            lambda: self.show_suggestions(next_taxa, taxa_iter, 1))
+        if num_suggestions[1] > 0: self.same_species_count.clicked.connect(
+            lambda: self.show_suggestions(next_taxa, taxa_iter, 2))
+        if num_suggestions[2] > 0: self.same_genus_count.clicked.connect(
+            lambda: self.show_suggestions(next_taxa, taxa_iter, 3))
 
-        if i == 1:
+        if match_type == 1:
             self.setWindowTitle("Similar Entries")
-        elif i == 2:
+        elif match_type == 2:
             self.setWindowTitle("Same Species")
-        elif i == 3:
+        elif match_type == 3:
             self.setWindowTitle("Same Genus")
         else:
             self.setWindowTitle("No Suggestions")
 
         # Disconnect if already connected
         try:
             self.manual_btn.clicked.disconnect()
```

### Comparing `phylo_match-0.1.0/phylo_match/match/match.py` & `phylo_match-0.1.1/phylo_match/match/match.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,35 +33,51 @@
 
     output = []
     perfect_matches = []
     difference_threshold = int(levenshtein_num)
     for db in dbs:
         for db_name in db:
             suggestions = []
+            loose_suggestions = []
             genus_match = []
             species_match = []
             genus_name = db_name.split(db_separator, 1)[0]
             try:
                 species_name = db_name.split(db_separator, 1)[1]
             except:
                 species_name = ""
                 print(f"WARNING: entry [{db_name}] possibly malformed. Check database.")
 
             found_match = False
             for tree_name in tree:
+
+                tree_genus_name = tree_name.split(db_separator, 1)[0]
+                try:
+                    tree_species_name = tree_name.split(db_separator, 1)[1]
+                except:
+                    tree_species_name = ""
+                    print(f"WARNING: tree entry [{tree_name}] possibly malformed. Check tree.")
+
                 if db_name == tree_name:
                     found_match = True
                     break
                 elif levenshtein_distance(db_name, tree_name) < difference_threshold:
                     suggestions.append(tree_name)
-                elif re.match(rf".*[_| ]{species_name}$", tree_name):
-                    species_match.append(tree_name)
-                elif re.match(rf"^{genus_name}[_| ]", tree_name):
+                elif genus_name == tree_genus_name:
                     genus_match.append(tree_name)
+                elif levenshtein_distance(genus_name, tree_genus_name) < difference_threshold:
+                    loose_suggestions.append(tree_name)
+                elif species_name == tree_species_name:
+                    species_match.append(tree_name)
+                elif levenshtein_distance(species_name, tree_species_name) < difference_threshold:
+                    loose_suggestions.append(tree_name)
 
+            # If suggestions is empty, add loose suggestions (levenshtein applied to genus and species independently)
+            if len(suggestions) == 0:
+                suggestions = suggestions + loose_suggestions
             if found_match:
                 output.append(db_name)
                 perfect_matches.append(db_name)
             else:
                 output.append([db_name, suggestions, species_match, genus_match])
 
     return output, perfect_matches
@@ -150,14 +166,16 @@
                     csv_list = line.strip().split(",")
                     # Replace first line with new name, only if not blank
                     if taxa_list[i - 1] != "":
                         csv_list[species_index] = taxa_list[i - 1]
                     outf.write(f"{','.join(csv_list)}\n")
                     i += 1
 
+    return outfile_path
+
 
 def get_wiki_image(search_term):
     WIKI_REQUEST = 'http://en.wikipedia.org/w/api.php?action=query&prop=pageimages&format=json&piprop=original&titles='
     try:
         result = wikipedia.search(search_term, results=1)
         wikipedia.set_lang('en')
         wikipage = wikipedia.WikipediaPage(title=result[0])
```

### Comparing `phylo_match-0.1.0/phylo_match.egg-info/PKG-INFO` & `phylo_match-0.1.1/phylo_match.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phylo-match
-Version: 0.1.0
+Version: 0.1.1
 Summary: For matching species databases
 Home-page: https://github.com/spearw/phylo-match
 Author: William Spear
 Author-email: spearw@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
@@ -45,14 +45,19 @@
 ```
 
 Install Phylo-Match:
 ```bash
 pip3 install phylo-match
 ```
 
+Upgrade Phylo-Match:
+```bash
+pip install phylo-match -U
+```
+
 
 ## Usage
 
 ```bash
 phylo-match
 ```
 Use the gui to select a database file (.csv), and a taxa tree (.nexus) to match the database to. Enter the number of your species column in the box, if the taxa you are matching are not in the first column (index counts from 0, so enter 0 for first column, 1 for second, etc.)
```

### Comparing `phylo_match-0.1.0/setup.cfg` & `phylo_match-0.1.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = phylo-match
-version = 0.1.0
+version = 0.1.1
 author = William Spear
 author_email = spearw@gmail.com
 description = For matching species databases
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/spearw/phylo-match
 classifiers =
```


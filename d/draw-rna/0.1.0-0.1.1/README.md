# Comparing `tmp/draw_rna-0.1.0.tar.gz` & `tmp/draw_rna-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "draw_rna-0.1.0.tar", last modified: Fri Sep  8 22:26:23 2023, max compression
+gzip compressed data, was "/home/runner/work/draw_rna/draw_rna/dist/.tmp-2sr_jgz6/draw_rna-0.1.1.tar", last modified: Wed May  1 04:41:10 2024, max compression
```

## Comparing `draw_rna-0.1.0.tar` & `draw_rna-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-08 22:26:23.958058 draw_rna-0.1.0/
--rw-r--r--   0 thomas     (501) staff       (20)     1090 2023-09-08 21:30:47.000000 draw_rna-0.1.0/LICENSE
--rw-r--r--   0 thomas     (501) staff       (20)     3908 2023-09-08 22:26:23.957754 draw_rna-0.1.0/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)     3286 2023-09-08 20:53:33.000000 draw_rna-0.1.0/README.md
--rw-r--r--   0 thomas     (501) staff       (20)      673 2023-09-08 22:21:52.000000 draw_rna-0.1.0/pyproject.toml
--rw-r--r--   0 thomas     (501) staff       (20)       38 2023-09-08 22:26:23.958106 draw_rna-0.1.0/setup.cfg
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-08 22:26:23.951281 draw_rna-0.1.0/src/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-08 22:26:23.953171 draw_rna-0.1.0/src/Draw_RNA.egg-info/
--rw-r--r--   0 thomas     (501) staff       (20)     3908 2023-09-08 22:26:23.000000 draw_rna-0.1.0/src/Draw_RNA.egg-info/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)      671 2023-09-08 22:26:23.000000 draw_rna-0.1.0/src/Draw_RNA.egg-info/SOURCES.txt
--rw-r--r--   0 thomas     (501) staff       (20)        1 2023-09-08 22:26:23.000000 draw_rna-0.1.0/src/Draw_RNA.egg-info/dependency_links.txt
--rw-r--r--   0 thomas     (501) staff       (20)       56 2023-09-08 22:26:23.000000 draw_rna-0.1.0/src/Draw_RNA.egg-info/requires.txt
--rw-r--r--   0 thomas     (501) staff       (20)        9 2023-09-08 22:26:23.000000 draw_rna-0.1.0/src/Draw_RNA.egg-info/top_level.txt
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-09-08 22:26:23.957072 draw_rna-0.1.0/src/draw_rna/
--rw-r--r--   0 thomas     (501) staff       (20)        0 2023-09-08 20:53:33.000000 draw_rna-0.1.0/src/draw_rna/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)     6262 2023-09-08 20:53:33.000000 draw_rna-0.1.0/src/draw_rna/draw.py
--rw-r--r--   0 thomas     (501) staff       (20)     3182 2023-09-08 20:53:33.000000 draw_rna-0.1.0/src/draw_rna/draw_all.py
--rw-r--r--   0 thomas     (501) staff       (20)     2252 2023-09-08 20:53:33.000000 draw_rna-0.1.0/src/draw_rna/draw_from_rdat.py
--rw-r--r--   0 thomas     (501) staff       (20)      478 2023-09-08 20:53:33.000000 draw_rna-0.1.0/src/draw_rna/draw_utils.py
--rwxr-xr-x   0 thomas     (501) staff       (20)     3966 2023-09-08 20:53:33.000000 draw_rna-0.1.0/src/draw_rna/inv_utils.py
--rw-r--r--   0 thomas     (501) staff       (20)     1325 2023-09-08 20:53:33.000000 draw_rna-0.1.0/src/draw_rna/ipynb_draw.py
--rwxr-xr-x   0 thomas     (501) staff       (20)     1323 2023-09-08 20:53:33.000000 draw_rna-0.1.0/src/draw_rna/mpl.py
--rw-r--r--   0 thomas     (501) staff       (20)    13143 2023-09-08 20:53:33.000000 draw_rna-0.1.0/src/draw_rna/render_rna.py
--rwxr-xr-x   0 thomas     (501) staff       (20)    13483 2023-09-08 20:53:33.000000 draw_rna-0.1.0/src/draw_rna/render_rna_flip.py
--rwxr-xr-x   0 thomas     (501) staff       (20)     1881 2023-09-08 20:53:33.000000 draw_rna-0.1.0/src/draw_rna/svg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:41:10.000000 draw_rna-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-01 04:41:06.000000 draw_rna-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-05-01 04:41:10.000000 draw_rna-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-01 04:41:06.000000 draw_rna-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-01 04:41:06.000000 draw_rna-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 04:41:10.000000 draw_rna-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:41:10.000000 draw_rna-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:41:10.000000 draw_rna-0.1.1/src/draw_rna/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 04:41:06.000000 draw_rna-0.1.1/src/draw_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-05-01 04:41:06.000000 draw_rna-0.1.1/src/draw_rna/draw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-01 04:41:06.000000 draw_rna-0.1.1/src/draw_rna/draw_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-01 04:41:06.000000 draw_rna-0.1.1/src/draw_rna/draw_from_rdat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-01 04:41:06.000000 draw_rna-0.1.1/src/draw_rna/draw_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3966 2024-05-01 04:41:06.000000 draw_rna-0.1.1/src/draw_rna/inv_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-01 04:41:06.000000 draw_rna-0.1.1/src/draw_rna/ipynb_draw.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1323 2024-05-01 04:41:06.000000 draw_rna-0.1.1/src/draw_rna/mpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13143 2024-05-01 04:41:06.000000 draw_rna-0.1.1/src/draw_rna/render_rna.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13483 2024-05-01 04:41:06.000000 draw_rna-0.1.1/src/draw_rna/render_rna_flip.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1950 2024-05-01 04:41:06.000000 draw_rna-0.1.1/src/draw_rna/svg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:41:10.000000 draw_rna-0.1.1/src/draw_rna.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-05-01 04:41:10.000000 draw_rna-0.1.1/src/draw_rna.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-01 04:41:10.000000 draw_rna-0.1.1/src/draw_rna.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 04:41:10.000000 draw_rna-0.1.1/src/draw_rna.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-01 04:41:10.000000 draw_rna-0.1.1/src/draw_rna.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 04:41:10.000000 draw_rna-0.1.1/src/draw_rna.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `draw_rna-0.1.0/LICENSE` & `draw_rna-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `draw_rna-0.1.0/PKG-INFO` & `draw_rna-0.1.1/src/draw_rna.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,41 @@
 Metadata-Version: 2.1
-Name: draw_rna
-Version: 0.1.0
+Name: draw-rna
+Version: 0.1.1
 Summary: Draw RNA secondary structures in Python
 Author-email: Das Lab <thedaslab@stanford.edu>
 Project-URL: Homepage, https://github.com/DasLab/draw_rna
 Project-URL: Bug Tracker, https://github.com/DasLab/draw_rna/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: argparse>=1.4
-Requires-Dist: numpy>=1.15
-Requires-Dist: matplotlib>=3.2
-Requires-Dist: rdat-kit>=1.6
 
 # draw_rna
 
 Generate quick secondary structures of nucleic acids via jupyter notebook or command line.
 
 A communal and continuing effort by the Das Lab, Eterna Players, M. Wu, H. Wayment-Steele.
 
 ## Dependencies
 
 The default behavior is to output the secondary structure visualization to both svg and png. The png requires Inkscape, whose directory must be set by environmental variable `INKSCAPEDIR`.
 
 ## Install
+`draw_rna` is [available on PyPI](https://pypi.org/project/draw-rna/).
 
-Clone this repository to your hard drive and install as follows:
+`pip install draw_rna`
 
-```
-git clone git@github.com:DasLab/draw_rna.git
-cd draw_rna/
-python setup.py install
-```
+Alternatively, clone the Github repository to your hard drive as follows:
 
-*Warning* if you see errors in using the repository, it maybe due to your `draw_rna` directory sitting in a folder like `src/` which already is in your Python Path. in that case, *rename* `draw_rna` to `draw_rna_directory` and/or move it to another spot in your system.
+`git clone git@github.com:DasLab/draw_rna.git`
+
+*Warning* if you see errors in using the repository, it may be due to your `draw_rna` directory sitting in a folder like `src/` which already is in your Python Path. in that case, *rename* `draw_rna` to `draw_rna_directory` and/or move it to another spot in your system.
 
 ## Basic Usage
 
 ### Jupyter notebook
 
 See `example_files/demo.ipynb` for more. In brief:
```

### Comparing `draw_rna-0.1.0/README.md` & `draw_rna-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,24 +5,23 @@
 A communal and continuing effort by the Das Lab, Eterna Players, M. Wu, H. Wayment-Steele.
 
 ## Dependencies
 
 The default behavior is to output the secondary structure visualization to both svg and png. The png requires Inkscape, whose directory must be set by environmental variable `INKSCAPEDIR`.
 
 ## Install
+`draw_rna` is [available on PyPI](https://pypi.org/project/draw-rna/).
 
-Clone this repository to your hard drive and install as follows:
+`pip install draw_rna`
 
-```
-git clone git@github.com:DasLab/draw_rna.git
-cd draw_rna/
-python setup.py install
-```
+Alternatively, clone the Github repository to your hard drive as follows:
 
-*Warning* if you see errors in using the repository, it maybe due to your `draw_rna` directory sitting in a folder like `src/` which already is in your Python Path. in that case, *rename* `draw_rna` to `draw_rna_directory` and/or move it to another spot in your system.
+`git clone git@github.com:DasLab/draw_rna.git`
+
+*Warning* if you see errors in using the repository, it may be due to your `draw_rna` directory sitting in a folder like `src/` which already is in your Python Path. in that case, *rename* `draw_rna` to `draw_rna_directory` and/or move it to another spot in your system.
 
 ## Basic Usage
 
 ### Jupyter notebook
 
 See `example_files/demo.ipynb` for more. In brief:
```

### Comparing `draw_rna-0.1.0/pyproject.toml` & `draw_rna-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "draw_rna"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Das Lab", email="thedaslab@stanford.edu" },
 ]
 description = "Draw RNA secondary structures in Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `draw_rna-0.1.0/src/Draw_RNA.egg-info/PKG-INFO` & `draw_rna-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,41 @@
 Metadata-Version: 2.1
-Name: draw-rna
-Version: 0.1.0
+Name: draw_rna
+Version: 0.1.1
 Summary: Draw RNA secondary structures in Python
 Author-email: Das Lab <thedaslab@stanford.edu>
 Project-URL: Homepage, https://github.com/DasLab/draw_rna
 Project-URL: Bug Tracker, https://github.com/DasLab/draw_rna/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: argparse>=1.4
-Requires-Dist: numpy>=1.15
-Requires-Dist: matplotlib>=3.2
-Requires-Dist: rdat-kit>=1.6
 
 # draw_rna
 
 Generate quick secondary structures of nucleic acids via jupyter notebook or command line.
 
 A communal and continuing effort by the Das Lab, Eterna Players, M. Wu, H. Wayment-Steele.
 
 ## Dependencies
 
 The default behavior is to output the secondary structure visualization to both svg and png. The png requires Inkscape, whose directory must be set by environmental variable `INKSCAPEDIR`.
 
 ## Install
+`draw_rna` is [available on PyPI](https://pypi.org/project/draw-rna/).
 
-Clone this repository to your hard drive and install as follows:
+`pip install draw_rna`
 
-```
-git clone git@github.com:DasLab/draw_rna.git
-cd draw_rna/
-python setup.py install
-```
+Alternatively, clone the Github repository to your hard drive as follows:
 
-*Warning* if you see errors in using the repository, it maybe due to your `draw_rna` directory sitting in a folder like `src/` which already is in your Python Path. in that case, *rename* `draw_rna` to `draw_rna_directory` and/or move it to another spot in your system.
+`git clone git@github.com:DasLab/draw_rna.git`
+
+*Warning* if you see errors in using the repository, it may be due to your `draw_rna` directory sitting in a folder like `src/` which already is in your Python Path. in that case, *rename* `draw_rna` to `draw_rna_directory` and/or move it to another spot in your system.
 
 ## Basic Usage
 
 ### Jupyter notebook
 
 See `example_files/demo.ipynb` for more. In brief:
```

### Comparing `draw_rna-0.1.0/src/draw_rna/draw.py` & `draw_rna-0.1.1/src/draw_rna/draw.py`

 * *Files identical despite different names*

### Comparing `draw_rna-0.1.0/src/draw_rna/draw_all.py` & `draw_rna-0.1.1/src/draw_rna/draw_all.py`

 * *Files identical despite different names*

### Comparing `draw_rna-0.1.0/src/draw_rna/draw_from_rdat.py` & `draw_rna-0.1.1/src/draw_rna/draw_from_rdat.py`

 * *Files identical despite different names*

### Comparing `draw_rna-0.1.0/src/draw_rna/inv_utils.py` & `draw_rna-0.1.1/src/draw_rna/inv_utils.py`

 * *Files identical despite different names*

### Comparing `draw_rna-0.1.0/src/draw_rna/ipynb_draw.py` & `draw_rna-0.1.1/src/draw_rna/ipynb_draw.py`

 * *Files identical despite different names*

### Comparing `draw_rna-0.1.0/src/draw_rna/mpl.py` & `draw_rna-0.1.1/src/draw_rna/mpl.py`

 * *Files identical despite different names*

### Comparing `draw_rna-0.1.0/src/draw_rna/render_rna.py` & `draw_rna-0.1.1/src/draw_rna/render_rna.py`

 * *Files identical despite different names*

### Comparing `draw_rna-0.1.0/src/draw_rna/render_rna_flip.py` & `draw_rna-0.1.1/src/draw_rna/render_rna_flip.py`

 * *Files identical despite different names*

### Comparing `draw_rna-0.1.0/src/draw_rna/svg.py` & `draw_rna-0.1.1/src/draw_rna/svg.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Methods for outputting SVG files."""
 
-from draw_rna.draw_utils import * 
+from draw_rna.draw_utils import *
 
 class svg(object):
 	def __init__(self, filename, w, h):
 		# create the file
 		self.__out = open(filename, 'w')
-		
+
 		# write the header
 		self.__out.write("""
 		<?xml version="1.0" encoding="utf-8"?>
 		  <svg version="1.1" id="Layer_1"
 		  x="0px" y="0px"
 		  width="%spx" height="%spx"
 		  viewBox="0 0 %s %s"
@@ -19,33 +19,33 @@
 		self.__out.write('\n')
 
 	def __del__(self):
 		# write a footer
 		self.__out.write('</svg>\n')
 		self.__out.close()
 		del self.__out
-	
-	def line(self, x1, y1, x2, y2, stroke, width=1):
+
+	def line(self, x1, y1, x2, y2, stroke, width=1, alpha=1):
 		""""""
 		# print 'Line (%s %s %s %s %s)' % (x1, y1, x2, y2, color)
 		stroke = convert_color(stroke)
-		self.__out.write('<line fill="none" stroke="%s" stroke-width="%dpx" x1="%s" y1="%s" x2="%s" y2="%s" x3="0.0" y3="0.0"/>\n' %
-			(stroke, width, x1, y1, x2, y2))
-      
+		self.__out.write('<line fill="none" stroke="%s" stroke-width="%dpx" x1="%s" y1="%s" x2="%s" y2="%s" x3="0.0" y3="0.0" alpha="%s"/>\n' %
+			(stroke, width, x1, y1, x2, y2,alpha))
+
 	def polygon(self, points, fill, stroke, opacity = 1.0):
 		fill = convert_color(fill)
 		stroke = convert_color(stroke)
 		points = ' '.join('%s,%s' % (x,y) for (x,y) in points)
 		self.__out.write('<polygon fill="%s" stroke="%s" points="%s" opacity="%f"/>\n' %
 			(fill, stroke, points,opacity))
 
-	def circle(self, x, y, radius, fill, stroke):
+	def circle(self, x, y, radius, fill, stroke, alpha=1):
 		fill = convert_color(fill)
-		self.__out.write('<circle cx="%s" cy="%s" r="%s" fill="%s" stroke="%s"/>\n' %
-			(x, y, radius, fill, stroke))
-	
-	def text(self, x, y, size, fill, align, str):
+		self.__out.write('<circle cx="%s" cy="%s" r="%s" fill="%s" stroke="%s" alpha="%s"/>\n' %
+			(x, y, radius, fill, stroke,alpha))
+
+	def text(self, x, y, size, fill, align, string,alpha=1):
 		fill = convert_color(fill)
-		self.__out.write(' <text x="%d" y="%d" font-family="sans_serif" font-size="%d" fill="%s" text-anchor="%s">%s</text>' % (x,y,size,fill,align,str))
-        ## rotated 
+		self.__out.write(' <text x="%d" y="%d" font-family="sans_serif" font-size="%d" fill="%s" text-anchor="%s" alpha="%s">%s</text>' % (x,y,size,fill,align,alpha,string))
+        ## rotated
 		#self.__out.write(' <text x="%d" y="%d" font-family="sans_serif" font-size="%d" fill="%s" text-anchor="%s" transform="rotate(180 %d,%d)">%s</text>' % (x-10,y+10,size,fill,align,x,y,str))
-		
+
```


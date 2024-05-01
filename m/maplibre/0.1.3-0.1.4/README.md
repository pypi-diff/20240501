# Comparing `tmp/maplibre-0.1.3.tar.gz` & `tmp/maplibre-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maplibre-0.1.3.tar", max compression
+gzip compressed data, was "maplibre-0.1.4.tar", max compression
```

## Comparing `maplibre-0.1.3.tar` & `maplibre-0.1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1068 2023-12-21 16:45:19.535649 maplibre-0.1.3/LICENSE.md
--rw-r--r--   0        0        0     1683 2024-02-06 10:47:07.125958 maplibre-0.1.3/README.md
--rw-r--r--   0        0        0      263 2024-01-22 14:14:20.992661 maplibre-0.1.3/maplibre/__init__.py
--rw-r--r--   0        0        0      667 2024-02-06 10:43:25.436787 maplibre-0.1.3/maplibre/_constants.py
--rw-r--r--   0        0        0      563 2024-01-09 14:57:27.782365 maplibre-0.1.3/maplibre/_templates.py
--rw-r--r--   0        0        0     1027 2024-01-09 14:57:27.782365 maplibre-0.1.3/maplibre/_utils.py
--rw-r--r--   0        0        0     1800 2024-01-09 14:57:27.782365 maplibre-0.1.3/maplibre/basemaps.py
--rw-r--r--   0        0        0     4154 2024-01-22 09:04:44.041263 maplibre-0.1.3/maplibre/controls.py
--rw-r--r--   0        0        0     1250 2024-01-09 14:57:27.782365 maplibre-0.1.3/maplibre/experimental.py
--rw-r--r--   0        0        0     2242 2024-01-22 09:38:42.511359 maplibre-0.1.3/maplibre/ipywidget.py
--rw-r--r--   0        0        0     2752 2024-01-09 14:57:27.782365 maplibre-0.1.3/maplibre/layer.py
--rw-r--r--   0        0        0     9145 2024-02-06 10:43:25.436787 maplibre-0.1.3/maplibre/map.py
--rw-r--r--   0        0        0      964 2024-01-22 09:04:44.041263 maplibre-0.1.3/maplibre/mapcontext.py
--rw-r--r--   0        0        0      526 2024-02-06 10:43:33.772980 maplibre-0.1.3/maplibre/server.py
--rw-r--r--   0        0        0     2456 2024-01-09 14:57:27.782365 maplibre-0.1.3/maplibre/sources.py
--rw-r--r--   0        0        0     9210 2024-02-06 10:43:25.436787 maplibre-0.1.3/maplibre/srcjs/index.js
--rw-r--r--   0        0        0     8544 2024-02-06 10:43:25.436787 maplibre-0.1.3/maplibre/srcjs/ipywidget.js
--rw-r--r--   0        0        0    63722 2024-01-09 14:57:27.782365 maplibre-0.1.3/maplibre/srcjs/maplibre-gl.css
--rw-r--r--   0        0        0   762783 2024-01-09 14:57:27.782365 maplibre-0.1.3/maplibre/srcjs/maplibre-gl.js
--rw-r--r--   0        0        0     1017 2024-02-06 09:58:53.357444 maplibre-0.1.3/maplibre/ui.py
--rw-r--r--   0        0        0     1341 2024-01-15 16:37:23.103118 maplibre-0.1.3/maplibre/utils.py
--rw-r--r--   0        0        0      886 2024-02-06 10:43:25.436787 maplibre-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1665 2024-01-09 09:11:36.997960 maplibre-0.1.3/srcjs/index.js
--rw-r--r--   0        0        0     2105 2024-01-15 16:37:23.107118 maplibre-0.1.3/srcjs/ipywidget.js
--rw-r--r--   0        0        0     1963 2024-02-06 10:43:25.436787 maplibre-0.1.3/srcjs/mapmethods.js
--rw-r--r--   0        0        0     3321 2024-02-06 10:43:25.436787 maplibre-0.1.3/srcjs/pymaplibregl.js
--rw-r--r--   0        0        0      662 2024-01-15 16:37:23.107118 maplibre-0.1.3/srcjs/rwidget.js
--rw-r--r--   0        0        0      434 2024-02-06 10:43:25.436787 maplibre-0.1.3/srcjs/utils.js
--rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 maplibre-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-12-21 16:45:19.535649 maplibre-0.1.4/LICENSE.md
+-rw-r--r--   0        0        0     1683 2024-02-06 10:58:05.129502 maplibre-0.1.4/README.md
+-rw-r--r--   0        0        0      263 2024-01-22 14:14:20.992661 maplibre-0.1.4/maplibre/__init__.py
+-rw-r--r--   0        0        0      667 2024-02-06 10:43:25.436787 maplibre-0.1.4/maplibre/_constants.py
+-rw-r--r--   0        0        0      563 2024-01-09 14:57:27.782365 maplibre-0.1.4/maplibre/_templates.py
+-rw-r--r--   0        0        0     1027 2024-01-09 14:57:27.782365 maplibre-0.1.4/maplibre/_utils.py
+-rw-r--r--   0        0        0     1800 2024-01-09 14:57:27.782365 maplibre-0.1.4/maplibre/basemaps.py
+-rw-r--r--   0        0        0     4154 2024-01-22 09:04:44.041263 maplibre-0.1.4/maplibre/controls.py
+-rw-r--r--   0        0        0     1250 2024-01-09 14:57:27.782365 maplibre-0.1.4/maplibre/experimental.py
+-rw-r--r--   0        0        0     2242 2024-01-22 09:38:42.511359 maplibre-0.1.4/maplibre/ipywidget.py
+-rw-r--r--   0        0        0     2752 2024-01-09 14:57:27.782365 maplibre-0.1.4/maplibre/layer.py
+-rw-r--r--   0        0        0     9134 2024-05-01 10:52:24.031761 maplibre-0.1.4/maplibre/map.py
+-rw-r--r--   0        0        0      964 2024-01-22 09:04:44.041263 maplibre-0.1.4/maplibre/mapcontext.py
+-rw-r--r--   0        0        0      526 2024-04-15 12:42:11.262001 maplibre-0.1.4/maplibre/server.py
+-rw-r--r--   0        0        0     2456 2024-01-09 14:57:27.782365 maplibre-0.1.4/maplibre/sources.py
+-rw-r--r--   0        0        0     9210 2024-02-06 10:43:25.436787 maplibre-0.1.4/maplibre/srcjs/index.js
+-rw-r--r--   0        0        0     8544 2024-02-06 10:43:25.436787 maplibre-0.1.4/maplibre/srcjs/ipywidget.js
+-rw-r--r--   0        0        0    63722 2024-01-09 14:57:27.782365 maplibre-0.1.4/maplibre/srcjs/maplibre-gl.css
+-rw-r--r--   0        0        0   762783 2024-01-09 14:57:27.782365 maplibre-0.1.4/maplibre/srcjs/maplibre-gl.js
+-rw-r--r--   0        0        0     1017 2024-04-15 12:41:10.848600 maplibre-0.1.4/maplibre/ui.py
+-rw-r--r--   0        0        0     1341 2024-01-15 16:37:23.103118 maplibre-0.1.4/maplibre/utils.py
+-rw-r--r--   0        0        0      887 2024-05-01 11:08:50.693392 maplibre-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1665 2024-01-09 09:11:36.997960 maplibre-0.1.4/srcjs/index.js
+-rw-r--r--   0        0        0     2105 2024-01-15 16:37:23.107118 maplibre-0.1.4/srcjs/ipywidget.js
+-rw-r--r--   0        0        0     1963 2024-02-06 10:43:25.436787 maplibre-0.1.4/srcjs/mapmethods.js
+-rw-r--r--   0        0        0     3321 2024-02-06 10:43:25.436787 maplibre-0.1.4/srcjs/pymaplibregl.js
+-rw-r--r--   0        0        0      662 2024-01-15 16:37:23.107118 maplibre-0.1.4/srcjs/rwidget.js
+-rw-r--r--   0        0        0      434 2024-02-06 10:43:25.436787 maplibre-0.1.4/srcjs/utils.js
+-rw-r--r--   0        0        0     2501 1970-01-01 00:00:00.000000 maplibre-0.1.4/PKG-INFO
```

### Comparing `maplibre-0.1.3/LICENSE.md` & `maplibre-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `maplibre-0.1.3/README.md` & `maplibre-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `maplibre-0.1.3/maplibre/_constants.py` & `maplibre-0.1.4/maplibre/_constants.py`

 * *Files identical despite different names*

### Comparing `maplibre-0.1.3/maplibre/_templates.py` & `maplibre-0.1.4/maplibre/_templates.py`

 * *Files identical despite different names*

### Comparing `maplibre-0.1.3/maplibre/_utils.py` & `maplibre-0.1.4/maplibre/_utils.py`

 * *Files identical despite different names*

### Comparing `maplibre-0.1.3/maplibre/basemaps.py` & `maplibre-0.1.4/maplibre/basemaps.py`

 * *Files identical despite different names*

### Comparing `maplibre-0.1.3/maplibre/controls.py` & `maplibre-0.1.4/maplibre/controls.py`

 * *Files identical despite different names*

### Comparing `maplibre-0.1.3/maplibre/experimental.py` & `maplibre-0.1.4/maplibre/experimental.py`

 * *Files identical despite different names*

### Comparing `maplibre-0.1.3/maplibre/ipywidget.py` & `maplibre-0.1.4/maplibre/ipywidget.py`

 * *Files identical despite different names*

### Comparing `maplibre-0.1.3/maplibre/layer.py` & `maplibre-0.1.4/maplibre/layer.py`

 * *Files identical despite different names*

### Comparing `maplibre-0.1.3/maplibre/map.py` & `maplibre-0.1.4/maplibre/map.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from .sources import Source
 
 
 class MapOptions(BaseModel):
     """Map options
 
     Note:
-        See [mapOptions](https://maplibre.org/maplibre-gl-js/docs/API/types/maplibregl.MapOptions/) for more details.
+        See [MapOptions](https://maplibre.org/maplibre-gl-js/docs/API/types/MapOptions/) for more details.
     """
 
     model_config = ConfigDict(
         validate_assignment=True, extra="forbid", use_enum_values=False
     )
     antialias: bool = None
     attribution_control: bool = Field(None, serialization_alias="attributionControl")
```

### Comparing `maplibre-0.1.3/maplibre/mapcontext.py` & `maplibre-0.1.4/maplibre/mapcontext.py`

 * *Files identical despite different names*

### Comparing `maplibre-0.1.3/maplibre/server.py` & `maplibre-0.1.4/maplibre/server.py`

 * *Files identical despite different names*

### Comparing `maplibre-0.1.3/maplibre/sources.py` & `maplibre-0.1.4/maplibre/sources.py`

 * *Files identical despite different names*

### Comparing `maplibre-0.1.3/maplibre/srcjs/index.js` & `maplibre-0.1.4/maplibre/srcjs/index.js`

 * *Files identical despite different names*

### Comparing `maplibre-0.1.3/maplibre/srcjs/ipywidget.js` & `maplibre-0.1.4/maplibre/srcjs/ipywidget.js`

 * *Files identical despite different names*

### Comparing `maplibre-0.1.3/maplibre/srcjs/maplibre-gl.css` & `maplibre-0.1.4/maplibre/srcjs/maplibre-gl.css`

 * *Files identical despite different names*

### Comparing `maplibre-0.1.3/maplibre/srcjs/maplibre-gl.js` & `maplibre-0.1.4/maplibre/srcjs/maplibre-gl.js`

 * *Files identical despite different names*

### Comparing `maplibre-0.1.3/maplibre/ui.py` & `maplibre-0.1.4/maplibre/ui.py`

 * *Files identical despite different names*

### Comparing `maplibre-0.1.3/maplibre/utils.py` & `maplibre-0.1.4/maplibre/utils.py`

 * *Files identical despite different names*

### Comparing `maplibre-0.1.3/pyproject.toml` & `maplibre-0.1.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "maplibre"
-version = "0.1.3"
+version = "0.1.4"
 description = "Python bindings for MapLibre GL JS"
 authors = ["Stefan Kuethe <stefan.kuethe@eoda.de>"]
 readme = "README.md"
 license = "MIT"
 include = [
     { path = "srcjs", format = ["sdist", "wheel"] }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
 shiny = "^0.6.1"
 htmltools = "^0.5.1"
 jinja2 = "^3.1.3"
 pydantic = "^2.5.3"
-anywidget = "^0.8.1"
+anywidget = ">=0.9.0"
 pandas = {version = "^2.1.4", optional = true}
 geopandas = {version = "^0.14.2", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.12.0"
 isort = "^5.13.2"
 pytest = "^7.4.3"
```

### Comparing `maplibre-0.1.3/srcjs/index.js` & `maplibre-0.1.4/srcjs/index.js`

 * *Files identical despite different names*

### Comparing `maplibre-0.1.3/srcjs/ipywidget.js` & `maplibre-0.1.4/srcjs/ipywidget.js`

 * *Files identical despite different names*

### Comparing `maplibre-0.1.3/srcjs/mapmethods.js` & `maplibre-0.1.4/srcjs/mapmethods.js`

 * *Files identical despite different names*

### Comparing `maplibre-0.1.3/srcjs/pymaplibregl.js` & `maplibre-0.1.4/srcjs/pymaplibregl.js`

 * *Files identical despite different names*

### Comparing `maplibre-0.1.3/srcjs/rwidget.js` & `maplibre-0.1.4/srcjs/rwidget.js`

 * *Files identical despite different names*

### Comparing `maplibre-0.1.3/PKG-INFO` & `maplibre-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: maplibre
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python bindings for MapLibre GL JS
 License: MIT
 Author: Stefan Kuethe
 Author-email: stefan.kuethe@eoda.de
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
-Requires-Dist: anywidget (>=0.8.1,<0.9.0)
+Requires-Dist: anywidget (>=0.9.0)
 Requires-Dist: geopandas (>=0.14.2,<0.15.0) ; extra == "all"
 Requires-Dist: htmltools (>=0.5.1,<0.6.0)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: pandas (>=2.1.4,<3.0.0) ; extra == "all"
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: shiny (>=0.6.1,<0.7.0)
 Description-Content-Type: text/markdown
```


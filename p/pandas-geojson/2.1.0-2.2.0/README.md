# Comparing `tmp/pandas_geojson-2.1.0.tar.gz` & `tmp/pandas_geojson-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_geojson-2.1.0.tar", last modified: Wed Apr 24 03:11:20 2024, max compression
+gzip compressed data, was "pandas_geojson-2.2.0.tar", last modified: Wed May  1 06:21:51 2024, max compression
```

## Comparing `pandas_geojson-2.1.0.tar` & `pandas_geojson-2.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 03:11:20.221367 pandas_geojson-2.1.0/
--rw-rw-rw-   0        0        0     1097 2024-03-18 19:56:01.000000 pandas_geojson-2.1.0/LICENSE
--rw-rw-rw-   0        0        0    53354 2024-04-24 03:11:20.219366 pandas_geojson-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    52944 2024-03-27 02:11:25.000000 pandas_geojson-2.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 03:11:20.194786 pandas_geojson-2.1.0/pandas_geojson/
--rw-rw-rw-   0        0        0      491 2024-04-22 22:20:20.000000 pandas_geojson-2.1.0/pandas_geojson/__init__.py
--rw-rw-rw-   0        0        0    10534 2024-04-23 02:53:14.000000 pandas_geojson-2.1.0/pandas_geojson/core.py
--rw-rw-rw-   0        0        0      645 2024-03-18 19:56:01.000000 pandas_geojson-2.1.0/pandas_geojson/io.py
-drwxrwxrwx   0        0        0        0 2024-04-24 03:11:20.218367 pandas_geojson-2.1.0/pandas_geojson.egg-info/
--rw-rw-rw-   0        0        0    53354 2024-04-24 03:11:20.000000 pandas_geojson-2.1.0/pandas_geojson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2024-04-24 03:11:20.000000 pandas_geojson-2.1.0/pandas_geojson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 03:11:20.000000 pandas_geojson-2.1.0/pandas_geojson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-24 03:11:20.000000 pandas_geojson-2.1.0/pandas_geojson.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 03:11:20.221367 pandas_geojson-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0      815 2024-04-22 23:35:36.000000 pandas_geojson-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 06:21:51.087011 pandas_geojson-2.2.0/
+-rw-rw-rw-   0        0        0     1097 2024-03-18 19:56:01.000000 pandas_geojson-2.2.0/LICENSE
+-rw-rw-rw-   0        0        0    16534 2024-05-01 06:21:51.083990 pandas_geojson-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    16124 2024-05-01 06:11:36.000000 pandas_geojson-2.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 06:21:51.053930 pandas_geojson-2.2.0/pandas_geojson/
+-rw-rw-rw-   0        0        0      491 2024-05-01 06:11:36.000000 pandas_geojson-2.2.0/pandas_geojson/__init__.py
+-rw-rw-rw-   0        0        0    10815 2024-05-01 06:11:36.000000 pandas_geojson-2.2.0/pandas_geojson/core.py
+-rw-rw-rw-   0        0        0     1333 2024-05-01 06:12:26.000000 pandas_geojson-2.2.0/pandas_geojson/io.py
+drwxrwxrwx   0        0        0        0 2024-05-01 06:21:51.082481 pandas_geojson-2.2.0/pandas_geojson.egg-info/
+-rw-rw-rw-   0        0        0    16534 2024-05-01 06:21:51.000000 pandas_geojson-2.2.0/pandas_geojson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2024-05-01 06:21:51.000000 pandas_geojson-2.2.0/pandas_geojson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 06:21:51.000000 pandas_geojson-2.2.0/pandas_geojson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-01 06:21:51.000000 pandas_geojson-2.2.0/pandas_geojson.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 06:21:51.088014 pandas_geojson-2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      815 2024-05-01 06:11:36.000000 pandas_geojson-2.2.0/setup.py
```

### Comparing `pandas_geojson-2.1.0/LICENSE` & `pandas_geojson-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas_geojson-2.1.0/pandas_geojson/core.py` & `pandas_geojson-2.2.0/pandas_geojson/core.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,289 +1,266 @@
 from dataclasses import dataclass, field
 from typing import List, Any, Dict, Union
 import pandas as pd
 import json
 
+
 @dataclass
-class Point:
+class Geometry:
     '''
-    GeoJSON Compliant Point Geometry 
+    Base class for GeoJSON compliant geometries
     '''
-    type: str = 'Point'
-    geometry: List[float] = field(default_factory=list)
+    geometry: Dict[str, Any] = field(default_factory=dict)
     properties: Dict[str, Any] = field(default_factory=dict)
 
+    def __post_init__(self):
+        self.type = self.__class__.__name__
+        if self.geometry:
+            self.geometry['type'] = self.type
+            self.validate()
 
     def __repr__(self):
         return json.dumps(self.to_dict(), indent=4)
 
-    def __post_init__(self):
-        self.validate()
-
     def to_dict(self) -> Dict[str, Any]:
         return {
-            'type': self.type,
+            'type': 'Feature',
             'geometry': self.geometry,
-            'properties': self.properties
+            'properties': self.properties if self.properties else {}   
         }
 
     def validate(self):
-        if self.type != "Point":
-            raise ValueError("Type must be 'Point' for Point geometry.")
-        if len(self.geometry) != 2:
-            raise ValueError("Point must have a single pair of coordinates (latitude and longitude).")
-        if not all(isinstance(coord, (int, float)) for coord in self.geometry):
-            raise ValueError("Coordinates must be numerical values.")
+        raise NotImplementedError("Validation method must be implemented in subclasses.")
 
 @dataclass
-class MultiPoint:
+class Point(Geometry):
     '''
-    GeoJSON Compliant MultiPoint Geometry 
+    GeoJSON Compliant Point Geometry 
     '''
-    type: str = 'MultiPoint'
-    geometry: List[List[float]] = field(default_factory=list)
-    properties: Dict[str, Any] = field(default_factory=dict)
+    def __init__(self, geometry: Dict[str, Any], properties: Dict[str, Any] = None):
+        super().__init__(geometry={'type': 'Point', 'coordinates': geometry}, properties=properties)
     
     def __repr__(self):
         return json.dumps(self.to_dict(), indent=4)
+    
 
-    def __post_init__(self):
-        self.validate()
+    def validate(self):
+        if self.geometry:
+            if self.geometry.get('type') != "Point":
+                raise ValueError("Geometry type must be 'Point' for Point geometry.")
+            coordinates = self.geometry.get('coordinates', [])
+            if not isinstance(coordinates, list) or len(coordinates) != 2:
+                raise ValueError("Coordinates must be provided as a list of two numerical values (longitude and latitude).")
+            if not all(isinstance(coord, (int, float)) for coord in coordinates):
+                raise ValueError("Coordinates must be numerical values.")
 
-    def to_dict(self) -> Dict[str, Any]:
-        return {
-            'type': self.type,
-            'geometry': self.geometry,
-            'properties': self.properties
-        }    
+@dataclass
+class MultiPoint(Geometry):
+    '''
+    GeoJSON Compliant MultiPoint Geometry 
+    '''
+    def __init__(self, geometry: List[List[float]], properties: Dict[str, Any] = None):
+        super().__init__(geometry={'type': 'MultiPoint', 'coordinates': geometry}, properties=properties)
+
+    def __repr__(self):
+        return json.dumps(self.to_dict(), indent=4)
 
     def validate(self):
-        if self.type != "MultiPoint":
-            raise ValueError("Type must be 'MultiPoint' for MultiPoint geometry.")
-        if not isinstance(self.geometry, list) or len(self.geometry) < 2 or not all(isinstance(coord, list) and len(coord) == 2 for coord in self.geometry):
-            raise ValueError("MultiPoint must have at least two pairs of coordinates.")
+        if self.geometry:
+            if self.geometry.get('type') != "MultiPoint":
+                raise ValueError("Geometry type must be 'MultiPoint' for MultiPoint geometry.")
+            coordinates = self.geometry.get('coordinates', [])
+            if not isinstance(coordinates, list) or not all(isinstance(coord, list) and len(coord) == 2 for coord in coordinates):
+                raise ValueError("Each coordinate pair in MultiPoint geometry must contain two elements (longitude and latitude).")
 
 @dataclass
-class LineString:
+class LineString(Geometry):
     '''
     GeoJSON Compliant LineString Geometry 
     '''
-    type: str = 'LineString'
-    geometry: List[List[float]] = field(default_factory=list)
-    properties: Dict[str, Any] = field(default_factory=dict)
-    
+    def __init__(self, geometry: List[List[float]], properties: Dict[str, Any] = None):
+        super().__init__(geometry={'type': 'LineString', 'coordinates': geometry}, properties=properties)
 
     def __repr__(self):
         return json.dumps(self.to_dict(), indent=4)
 
-    def __post_init__(self):
-        self.validate()
-
-    def to_dict(self) -> Dict[str, Any]:
-        return {
-            'type': self.type,
-            'geometry': self.geometry,
-            'properties': self.properties
-        }    
-
     def validate(self):
-        if self.type != "LineString":
-            raise ValueError("Type must be 'LineString' for LineString geometry.")
-        if not isinstance(self.geometry, list) or len(self.geometry) < 2 or not all(isinstance(coord, list) and len(coord) == 2 for coord in self.geometry):
-            raise ValueError("LineString must have a list of coordinate pairs with at least two coordinates.")
+        if self.geometry:
+            if self.geometry.get('type') != "LineString":
+                raise ValueError("Geometry type must be 'LineString' for LineString geometry.")
+            coordinates = self.geometry.get('coordinates', [])
+            if not isinstance(coordinates, list) or not all(isinstance(coord, list) and len(coord) == 2 for coord in coordinates):
+                raise ValueError("Each coordinate pair in LineString geometry must contain two elements (longitude and latitude).")
 
 @dataclass
-class MultiLineString:
+class MultiLineString(Geometry):
     '''
     GeoJSON Compliant MultiLineString Geometry 
     '''
-    type: str = 'MultiLineString'
-    geometry: List[List[List[float]]] = field(default_factory=list)
-    properties: Dict[str, Any] = field(default_factory=dict)
-    
+    def __init__(self, geometry: List[List[List[float]]], properties: Dict[str, Any] = None):
+        super().__init__(geometry={'type': 'MultiLineString', 'coordinates': geometry}, properties=properties)
+
     def __repr__(self):
         return json.dumps(self.to_dict(), indent=4)
 
-    def __post_init__(self):
-        self.validate()
-
-    def to_dict(self) -> Dict[str, Any]:
-        return {
-            'type': self.type,
-            'geometry': self.geometry,
-            'properties': self.properties
-        }    
-
     def validate(self):
-        if self.type != "MultiLineString":
-            raise ValueError("Type must be 'MultiLineString' for MultiLineString geometry.")
-        if len(self.geometry) < 2:
-            raise ValueError("MultiLineString must have at least two LineString geometries.")
-        for line_string in self.geometry:
-            if len(line_string) < 2:
-                raise ValueError("Each LineString in MultiLineString must have at least two coordinates.")
-            for point in line_string:
-                if len(point) != 2:
-                    raise ValueError("Each point in MultiLineString geometry must have exactly two coordinates (longitude and latitude).")
+        if self.geometry:
+            if self.geometry.get('type') != "MultiLineString":
+                raise ValueError("Geometry type must be 'MultiLineString' for MultiLineString geometry.")
+            for line_string in self.geometry.get('coordinates', []):
+                if not isinstance(line_string, list) or not all(isinstance(coord, list) and len(coord) == 2 for coord in line_string):
+                    raise ValueError("Each coordinate pair in MultiLineString geometry must contain two elements (longitude and latitude).")
 
 @dataclass
-class Polygon:
+class Polygon(Geometry):
     '''
     GeoJSON Compliant Polygon Geometry 
     '''
-    type: str = 'Polygon'
-    geometry: List[List[List[float]]] = field(default_factory=list)
-    properties: Dict[str, Any] = field(default_factory=dict)
-    
+    def __init__(self, geometry: List[List[List[float]]], properties: Dict[str, Any] = None):
+        super().__init__(geometry={'type': 'Polygon', 'coordinates': geometry}, properties=properties)
 
     def __repr__(self):
         return json.dumps(self.to_dict(), indent=4)
 
-    def __post_init__(self):
-        self.validate()
-
-    def to_dict(self) -> Dict[str, Any]:
-        return {
-            'type': self.type,
-            'geometry': self.geometry,
-            'properties': self.properties
-        }    
-
     def validate(self):
-        if self.type != "Polygon":
-            raise ValueError("Type must be 'Polygon' for Polygon geometry.")
-        if len(self.geometry) < 4:
-            raise ValueError("Polygon must have at least four coordinates (outer ring).")
-        for coords in self.geometry:
-            if len(coords) < 2:
-                raise ValueError("Each coordinate sublist must contain at least two elements.")
-        if self.geometry[0] != self.geometry[-1]:
-            raise ValueError("First and last points of the geometry must be the same.")
+        if self.geometry:
+            if self.geometry.get('type') != "Polygon":
+                raise ValueError("Geometry type must be 'Polygon' for Polygon geometry.")
+            for ring in self.geometry.get('coordinates', []):
+                if not isinstance(ring, list) or not all(isinstance(coord, list) and len(coord) == 2 for coord in ring):
+                    raise ValueError("Each coordinate pair in Polygon geometry must contain two elements (longitude and latitude).")
 
 @dataclass
-class MultiPolygon:
+class MultiPolygon(Geometry):
     '''
-    GeoJSON Compliant MutliPolygon Geometry 
+    GeoJSON Compliant MultiPolygon Geometry 
     '''
-    type: str = 'MultiPolygon'
-    geometry: List[List[List[List[float]]]] = field(default_factory=list)
-    properties: Dict[str, Any] = field(default_factory=dict)
-    
+    def __init__(self, geometry: List[List[List[List[float]]]], properties: Dict[str, Any] = None):
+        super().__init__(geometry={'type': 'MultiPolygon', 'coordinates': geometry}, properties=properties)
 
     def __repr__(self):
         return json.dumps(self.to_dict(), indent=4)
 
-    def __post_init__(self):
-        self.validate()
-
-    def to_dict(self) -> Dict[str, Any]:
-        return {
-            'type': self.type,
-            'geometry': self.geometry,
-            'properties': self.properties
-        }   
-
     def validate(self):
-        if self.type != "MultiPolygon":
-            raise ValueError("Type must be 'MultiPolygon' for MultiPolygon geometry.")
-        if len(self.geometry) < 2:
-            raise ValueError("MultiPolygon must have at least two polygons.")
-
-        for polygon in self.geometry:
-            if len(polygon) < 1:
-                raise ValueError("Each Polygon in MultiPolygon must have at least one ring.")
-            for ring in polygon:
-                if len(ring) < 4 or ring[0] != ring[-1]:
-                    raise ValueError("Each ring in MultiPolygon must have at least four coordinates and be closed.")
+        if self.geometry:
+            if self.geometry.get('type') != "MultiPolygon":
+                raise ValueError("Geometry type must be 'MultiPolygon' for MultiPolygon geometry.")
+            for polygon in self.geometry.get('coordinates', []):
+                for ring in polygon:
+                    if not isinstance(ring, list) or not all(isinstance(coord, list) and len(coord) == 2 for coord in ring):
+                        raise ValueError("Each coordinate pair in MultiPolygon geometry must contain two elements (longitude and latitude).")
 
-@dataclass
-class GeoJSONFeature:
-    type: str
-    geometry: Dict[str, Any] = field(default_factory=list)
-    properties: Dict[str, Any] = field(default_factory=dict)
 
 @dataclass
 class GeoJSON:
     '''
     Main Object for GeoJSON data. 
     '''
     type: str = 'FeatureCollection'
-    features: List[Union[GeoJSONFeature,Point,MultiPoint,LineString,MultiLineString,Polygon,MultiPolygon]] = field(default_factory=list)
+    features: List[Union[Point,MultiPoint,LineString,MultiLineString,Polygon,MultiPolygon]] = field(default_factory=list)
 
     def __repr__(self):
         return json.dumps(self.to_dict(), indent=4)
     
-    def add_features(self, feature_list: List[Union[GeoJSONFeature,Point,MultiPoint,LineString,MultiLineString,Polygon,MultiPolygon]]):
+    def __iter__(self):
+        return iter(self.features)
+    
+    def add_features(self, feature_list: List[Union[Point,MultiPoint,LineString,MultiLineString,Polygon,MultiPolygon]]):
         '''
         Add Multiple Features at once
         '''
+        instantiated_features = []
+        for feature in feature_list:
+            # Instantiate the class if it's not already an instance
+            if not isinstance(feature, (Point, MultiPoint, LineString, MultiLineString, Polygon, MultiPolygon)):
+                print(f"Invalid feature type: {type(feature)}")
+                raise ValueError("Each feature must be a geometry subclasses.")
+            instantiated_features.append(feature.to_dict())
+        self.features.extend(instantiated_features)
 
-        self.features.extend(feature_list)
-
-    def add_feature(self, feature_type: str, coordinates: Any = [], properties: dict = {}):
-        '''
-        Allows you to add features to the GeoJSON object.
-        '''
-        geometry = {'type': feature_type, 'coordinates': coordinates}
-        feature = GeoJSONFeature(type='Feature', geometry=geometry, properties=properties)
-        self.features.append(feature)
 
     def get_properties(self) -> List[str]:
-        properties = list(self.features[0].properties.keys()) if self.features else []
+        properties = list(self.features[0]['properties'].keys()) if self.features else []
         return properties
 
     def to_dict(self) -> Dict[str, Any]:
         return {
             'type': self.type,
-            'features': [feature.__dict__ for feature in self.features]
+            'features': self.features
         }
     
     def to_dataframe(self) -> pd.DataFrame:
         data = pd.json_normalize(self.to_dict(), record_path=['features'])
         return data
     
     def filter_geojson(self, property_values: List[str], property_key: str) -> 'GeoJSON':
         '''
         Filters GeoJSON features based on values in properties object.
 
         :return: GeoJSON
         '''
-        filtered_features = [feature for feature in self.features if feature.properties.get(property_key) in property_values]
+        # for feature in self.features:
+        #     print(feature)
+
+        filtered_features = []
+        for feature in self.features:
+            if feature['properties'].get(property_key) in property_values:
+                filtered_features.append(feature)  
         return GeoJSON(type='FeatureCollection', features=filtered_features)
-    
 
+    
     @classmethod
-    def from_dict(cls, data):
+    def from_dict(self, data):
         features = []
         for feature_data in data['features']:
             properties = feature_data.get('properties', {})
-            feature = GeoJSONFeature(type='Feature', geometry=feature_data['geometry'], properties=properties)
-            features.append(feature)
-        return cls(type=data['type'], features=features)
+            geometry_data = feature_data['geometry']
+
+            if geometry_data is None:
+                # Skip this feature if geometry data is missing
+                continue
+
+            geometry_type = geometry_data['type']
+            geometry_coordinates = geometry_data['coordinates']
+
+            geometry_class = {
+                "Point": Point,
+                "MultiPoint": MultiPoint,
+                "LineString": LineString,
+                "MultiLineString": MultiLineString,
+                "Polygon": Polygon,
+                "MultiPolygon": MultiPolygon
+            }.get(geometry_type)
+
+            if geometry_class is None:
+                raise ValueError(f"Invalid geometry type: {geometry_type}")
+                
+            geometry_instance = geometry_class(geometry=geometry_coordinates, properties=properties)
+            features.append(geometry_instance.to_dict())
+
+        return self(type='Feature Collection', features=features)
     
     @classmethod
-    def from_dataframe(cls
-                       ,df
-                       ,geometry_type_col: str = 'geometry.type'
-                       ,coordinate_col: str = 'geometry.coordinates'
-                       ,property_col_list: List[str] = []
-                       ):
+    def from_dataframe(cls,
+                    df,
+                    geometry_type_col: str = 'geometry.type',
+                    coordinate_col: str = 'geometry.coordinates',
+                    property_col_list: List[str] = []):
+        
         geojson = cls(type='FeatureCollection')
+
         for _, row in df.iterrows():
             coordinates = row[coordinate_col]
             geometry = {'type': row[geometry_type_col], 'coordinates': coordinates}
             properties = {col: row[col] for col in property_col_list}
-            feature = GeoJSONFeature(type='Feature', geometry=geometry, properties=properties)
-            geojson.features.append(feature)
-        return geojson
-    
-    @classmethod
-    def from_coordinates(cls, df, lat: str, lon: str, properties: List[str]) -> 'GeoJSON':
-        geojson = cls(type='FeatureCollection')
-        for _, row in df.iterrows():
-            coordinates = [row[lon], row[lat]]
-            feature_properties = {prop: row[prop] for prop in properties}
-            feature = GeoJSONFeature(type='Point', coordinates=coordinates, properties=feature_properties)
+            # Construct the feature directly as a dictionary
+            feature = {
+                'type': 'Feature',
+                'geometry': geometry,
+                'properties': properties
+            }
             geojson.features.append(feature)
+
         return geojson
 
+
```

### Comparing `pandas_geojson-2.1.0/setup.py` & `pandas_geojson-2.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="pandas_geojson",
-    version="2.1.0",
+    version="2.2.0",
     description="Convert Pandas Dataframe to GeoJSON",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/jrasband-dev/pandas-geojson",
     author="Jayden Rasband",
     author_email="jayden.rasband@gmail.com",
     license="MIT",
```


# Comparing `tmp/dctrackclient-1.3.0.tar.gz` & `tmp/dctrackclient-1.3.1.tar.gz`

## Comparing `dctrackclient-1.3.0.tar` & `dctrackclient-1.3.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    46773 2020-02-02 00:00:00.000000 dctrackclient-1.3.0/src/dcTrackClient/__init__.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 dctrackclient-1.3.0/.gitignore
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 dctrackclient-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    48348 2020-02-02 00:00:00.000000 dctrackclient-1.3.0/../README.md
--rw-r--r--   0        0        0    49038 2020-02-02 00:00:00.000000 dctrackclient-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    46775 2020-02-02 00:00:00.000000 dctrackclient-1.3.1/src/dcTrackClient/__init__.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 dctrackclient-1.3.1/.gitignore
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 dctrackclient-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0    48351 2020-02-02 00:00:00.000000 dctrackclient-1.3.1/../README.md
+-rw-r--r--   0        0        0    49041 2020-02-02 00:00:00.000000 dctrackclient-1.3.1/PKG-INFO
```

### Comparing `dctrackclient-1.3.0/src/dcTrackClient/__init__.py` & `dctrackclient-1.3.1/src/dcTrackClient/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 
 
 class Client:
-    """Sunbird dcTrack API client version 1.3.0 in Python"""
+    """Sunbird dcTrack API client version 1.3.1 in Python"""
 
     def __init__(self, baseUrl: str, username: str = '', password: str = '', apiToken: str = '', httpProxy: str = '', httpsProxy: str = ''):
         """Provide either a username and password, or an API token to access the dcTrack database with Python."""
         self.__BASE_URL = baseUrl
         self.__USERNAME = username
         self.__PASSWORD = password
         self.__APITOKEN = apiToken
@@ -161,37 +161,37 @@
         """Use the REST API to create power ports for an existing item. If ports are already defined for the item because it is included in the Item Models Library, you can use the REST API to create additional ports for the item."""
         return self.__request('PUT', '/api/v1/items/' + str(itemId) + '/powerports/' + str(portId) + '?proceedOnWarning=' + str(proceedOnWarning) + '&', payload)
 
     def getCompatibleConnector(self, itemId: int, portId: int, connectorId: int):
         """Use the REST API to determine if a Connector is compatible with a specific Power Port."""
         return self.__request('GET', '/api/v1/items/' + str(itemId) + '/powerports/' + str(portId) + '/connectors/' + str(connectorId) + '/isCompatible?')
 
-    def getBreakers(self, panelItemID: int):
+    def getBreakers(self, panelItemId: int):
         """Get a list of all Breakers for a given Panel Item. Returns JSON entity containing an array of all the Breakers for the specified Panel Item."""
-        return self.__request('GET', '/api/v2/dcimoperations/items/' + str(panelItemID) + '/breakers?')
+        return self.__request('GET', '/api/v2/dcimoperations/items/' + str(panelItemId) + '/breakers?')
 
-    def getBreaker(self, panelItemID: int, breakerPortId: int):
+    def getBreaker(self, panelItemId: int, breakerPortId: int):
         """Get a list of all Breakers for a given Panel Item. Returns JSON entity containing information for a single Panel Item Breaker."""
-        return self.__request('GET', '/api/v2/dcimoperations/items/' + str(panelItemID) + '/breakers/' + str(breakerPortId) + '?')
+        return self.__request('GET', '/api/v2/dcimoperations/items/' + str(panelItemId) + '/breakers/' + str(breakerPortId) + '?')
 
-    def updateBreaker(self, panelItemD: str, beakerPortID: int, payload: dict):
+    def updateBreaker(self, panelItemId: int, beakerPortId: int, payload: dict):
         """Update a single Breaker for a given Panel Item. Returns JSON entity containing information for the updated Panel Item Breaker. Note: This API performs as a true PUT and not a PATCH. Unlike with a PATCH, you must specify all attributes even if you want to change only one. Attributes that are not included in the Request will be considered as removed."""
-        return self.__request('PUT', '/api/v2/dcimoperations/items/' + str(panelItemD) + '/breakers/' + str(beakerPortID) + '?', payload)
+        return self.__request('PUT', '/api/v2/dcimoperations/items/' + str(panelItemId) + '/breakers/' + str(beakerPortId) + '?', payload)
 
     def createBreaker(self, panelItemId: int, payload: dict):
         """Create a single Breaker for a given Panel Item. Returns JSON entity containing information for the created Panel Item Breaker. Note: Breaker State is set based on the connection status of the Breaker. If the breaker is connected it will always be set to "Closed", even if "Open" is specified in the Request."""
         return self.__request('POST', '/api/v2/dcimoperations/items/' + str(panelItemId) + '/breakers?', payload)
 
-    def deleteBreaker(self, panelItemID: int, breakerPortId: int):
+    def deleteBreaker(self, panelItemId: int, breakerPortId: int):
         """Delete a Breaker for a given Panel Item. Returns empty JSON."""
-        return self.__request('DELETE', '/api/v2/dcimoperations/items/' + str(panelItemID) + '/breakers/' + str(breakerPortId) + '?')
+        return self.__request('DELETE', '/api/v2/dcimoperations/items/' + str(panelItemId) + '/breakers/' + str(breakerPortId) + '?')
 
-    def createBreakersBulk(self, panelItemID: int, payload: dict):
+    def createBreakersBulk(self, panelItemId: int, payload: dict):
         """Add/Update/Delete Breakers for a given Panel Item."""
-        return self.__request('POST', '/api/v2/dcimoperations/items/' + str(panelItemID) + '/breakers/bulk?', payload)
+        return self.__request('POST', '/api/v2/dcimoperations/items/' + str(panelItemId) + '/breakers/bulk?', payload)
 
     def getLocations(self):
         """Returns a list for all Locations."""
         return self.__request('GET', '/api/v1/locations?')
 
     def getLocation(self, locationId: int):
         """Get a single Location. Returns json containing location data for the specified ID."""
```

### Comparing `dctrackclient-1.3.0/pyproject.toml` & `dctrackclient-1.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "dcTrackClient"
-version = "1.3.0"
+version = "1.3.1"
 authors = [
   { name="Nicolas Ventura", email="ventura@lbl.gov" },
 ]
 description = "Sunbird dcTrack API client in Python"
 readme = "../README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dctrackclient-1.3.0/../README.md` & `dctrackclient-1.3.1/../README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 Sunbird [dcTrack](https://www.sunbirddcim.com/) API clients in Python and JavaScript
 
 ## Installation
 > dcTrackClient can be installed from the package manager of your choice.
 
 ### Python
 ```shell
-pip install dcTrackClient==1.3.0
+pip install dcTrackClient==1.3.1
 ```
 
 ### JavaScript
 ```shell
-npm i dctrackclient@1.3.0
+npm i dctrackclient@1.3.1
 ```
 
 ## Initialize a connection to the dcTrack API
 > Authentication is by using a base URL (the same URL to access the GUI) and a username and password, or a base URL and an API token.
 
 ### Python
 ```py
@@ -542,72 +542,72 @@
 ```
 |Parameter|Type|
 |---|---|
 |itemId|number|
 |portId|number|
 |connectorId|number|
 
-## getBreakers(panelItemID)
+## getBreakers(panelItemId)
 > Get a list of all Breakers for a given Panel Item. Returns JSON entity containing an array of all the Breakers for the specified Panel Item.
 ```
-GET api/v2/dcimoperations/items/{panelItemID}/breakers
+GET api/v2/dcimoperations/items/{panelItemId}/breakers
 ```
 |Parameter|Type|
 |---|---|
-|panelItemID|number|
+|panelItemId|number|
 
-## getBreaker(panelItemID, breakerPortId)
+## getBreaker(panelItemId, breakerPortId)
 > Get a list of all Breakers for a given Panel Item. Returns JSON entity containing information for a single Panel Item Breaker.
 ```
-GET api/v2/dcimoperations/items/{panelItemID}/breakers/{breakerPortId}
+GET api/v2/dcimoperations/items/{panelItemId}/breakers/{breakerPortId}
 ```
 |Parameter|Type|
 |---|---|
-|panelItemID|number|
+|panelItemId|number|
 |breakerPortId|number|
 
-## updateBreaker(panelItemD, beakerPortID, payload)
+## updateBreaker(panelItemId, beakerPortId, payload)
 > Update a single Breaker for a given Panel Item. Returns JSON entity containing information for the updated Panel Item Breaker. Note: This API performs as a true PUT and not a PATCH. Unlike with a PATCH, you must specify all attributes even if you want to change only one. Attributes that are not included in the Request will be considered as removed.
 ```
-PUT api/v2/dcimoperations/items/{panelItemD}/breakers/{beakerPortID} payload
+PUT api/v2/dcimoperations/items/{panelItemId}/breakers/{beakerPortId} payload
 ```
 |Parameter|Type|
 |---|---|
-|panelItemD|string|
-|beakerPortID|number|
+|panelItemId|number|
+|beakerPortId|number|
 |payload|object|
 
 ## createBreaker(panelItemId, payload)
 > Create a single Breaker for a given Panel Item. Returns JSON entity containing information for the created Panel Item Breaker. Note: Breaker State is set based on the connection status of the Breaker. If the breaker is connected it will always be set to "Closed", even if "Open" is specified in the Request.
 ```
 POST api/v2/dcimoperations/items/{panelItemId}/breakers payload
 ```
 |Parameter|Type|
 |---|---|
 |panelItemId|number|
 |payload|object|
 
-## deleteBreaker(panelItemID, breakerPortId)
+## deleteBreaker(panelItemId, breakerPortId)
 > Delete a Breaker for a given Panel Item. Returns empty JSON.
 ```
-DELETE api/v2/dcimoperations/items/{panelItemID}/breakers/{breakerPortId}
+DELETE api/v2/dcimoperations/items/{panelItemId}/breakers/{breakerPortId}
 ```
 |Parameter|Type|
 |---|---|
-|panelItemID|number|
+|panelItemId|number|
 |breakerPortId|number|
 
-## createBreakersBulk(panelItemID, payload)
+## createBreakersBulk(panelItemId, payload)
 > Add/Update/Delete Breakers for a given Panel Item.
 ```
-POST api/v2/dcimoperations/items/{panelItemID}/breakers/bulk payload
+POST api/v2/dcimoperations/items/{panelItemId}/breakers/bulk payload
 ```
 |Parameter|Type|
 |---|---|
-|panelItemID|number|
+|panelItemId|number|
 |payload|object|
 
 ## getLocations()
 > Returns a list for all Locations.
 ```
 GET api/v1/locations
 ```
```

### Comparing `dctrackclient-1.3.0/PKG-INFO` & `dctrackclient-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dcTrackClient
-Version: 1.3.0
+Version: 1.3.1
 Summary: Sunbird dcTrack API client in Python
 Project-URL: Homepage, https://github.com/nicfv/dcTrackClient/
 Project-URL: Bug Tracker, https://github.com/nicfv/dcTrackClient/pulls
 Author-email: Nicolas Ventura <ventura@lbl.gov>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -20,20 +20,20 @@
 Sunbird [dcTrack](https://www.sunbirddcim.com/) API clients in Python and JavaScript
 
 ## Installation
 > dcTrackClient can be installed from the package manager of your choice.
 
 ### Python
 ```shell
-pip install dcTrackClient==1.3.0
+pip install dcTrackClient==1.3.1
 ```
 
 ### JavaScript
 ```shell
-npm i dctrackclient@1.3.0
+npm i dctrackclient@1.3.1
 ```
 
 ## Initialize a connection to the dcTrack API
 > Authentication is by using a base URL (the same URL to access the GUI) and a username and password, or a base URL and an API token.
 
 ### Python
 ```py
@@ -560,72 +560,72 @@
 ```
 |Parameter|Type|
 |---|---|
 |itemId|number|
 |portId|number|
 |connectorId|number|
 
-## getBreakers(panelItemID)
+## getBreakers(panelItemId)
 > Get a list of all Breakers for a given Panel Item. Returns JSON entity containing an array of all the Breakers for the specified Panel Item.
 ```
-GET api/v2/dcimoperations/items/{panelItemID}/breakers
+GET api/v2/dcimoperations/items/{panelItemId}/breakers
 ```
 |Parameter|Type|
 |---|---|
-|panelItemID|number|
+|panelItemId|number|
 
-## getBreaker(panelItemID, breakerPortId)
+## getBreaker(panelItemId, breakerPortId)
 > Get a list of all Breakers for a given Panel Item. Returns JSON entity containing information for a single Panel Item Breaker.
 ```
-GET api/v2/dcimoperations/items/{panelItemID}/breakers/{breakerPortId}
+GET api/v2/dcimoperations/items/{panelItemId}/breakers/{breakerPortId}
 ```
 |Parameter|Type|
 |---|---|
-|panelItemID|number|
+|panelItemId|number|
 |breakerPortId|number|
 
-## updateBreaker(panelItemD, beakerPortID, payload)
+## updateBreaker(panelItemId, beakerPortId, payload)
 > Update a single Breaker for a given Panel Item. Returns JSON entity containing information for the updated Panel Item Breaker. Note: This API performs as a true PUT and not a PATCH. Unlike with a PATCH, you must specify all attributes even if you want to change only one. Attributes that are not included in the Request will be considered as removed.
 ```
-PUT api/v2/dcimoperations/items/{panelItemD}/breakers/{beakerPortID} payload
+PUT api/v2/dcimoperations/items/{panelItemId}/breakers/{beakerPortId} payload
 ```
 |Parameter|Type|
 |---|---|
-|panelItemD|string|
-|beakerPortID|number|
+|panelItemId|number|
+|beakerPortId|number|
 |payload|object|
 
 ## createBreaker(panelItemId, payload)
 > Create a single Breaker for a given Panel Item. Returns JSON entity containing information for the created Panel Item Breaker. Note: Breaker State is set based on the connection status of the Breaker. If the breaker is connected it will always be set to "Closed", even if "Open" is specified in the Request.
 ```
 POST api/v2/dcimoperations/items/{panelItemId}/breakers payload
 ```
 |Parameter|Type|
 |---|---|
 |panelItemId|number|
 |payload|object|
 
-## deleteBreaker(panelItemID, breakerPortId)
+## deleteBreaker(panelItemId, breakerPortId)
 > Delete a Breaker for a given Panel Item. Returns empty JSON.
 ```
-DELETE api/v2/dcimoperations/items/{panelItemID}/breakers/{breakerPortId}
+DELETE api/v2/dcimoperations/items/{panelItemId}/breakers/{breakerPortId}
 ```
 |Parameter|Type|
 |---|---|
-|panelItemID|number|
+|panelItemId|number|
 |breakerPortId|number|
 
-## createBreakersBulk(panelItemID, payload)
+## createBreakersBulk(panelItemId, payload)
 > Add/Update/Delete Breakers for a given Panel Item.
 ```
-POST api/v2/dcimoperations/items/{panelItemID}/breakers/bulk payload
+POST api/v2/dcimoperations/items/{panelItemId}/breakers/bulk payload
 ```
 |Parameter|Type|
 |---|---|
-|panelItemID|number|
+|panelItemId|number|
 |payload|object|
 
 ## getLocations()
 > Returns a list for all Locations.
 ```
 GET api/v1/locations
 ```
```


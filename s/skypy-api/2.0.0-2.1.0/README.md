# Comparing `tmp/skypy-api-2.0.0.tar.gz` & `tmp/skypy_api-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skypy-api-2.0.0.tar", last modified: Tue Apr 30 20:12:43 2024, max compression
+gzip compressed data, was "skypy_api-2.1.0.tar", last modified: Wed May  1 12:37:37 2024, max compression
```

## Comparing `skypy-api-2.0.0.tar` & `skypy_api-2.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-30 20:12:43.195075 skypy-api-2.0.0/
--rw-r--r--   0 david     (1000) david     (1000)     2251 2024-04-30 19:28:37.000000 skypy-api-2.0.0/LICENSE
--rw-r--r--   0 david     (1000) david     (1000)      841 2024-04-30 20:12:43.195075 skypy-api-2.0.0/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      456 2024-04-30 19:28:37.000000 skypy-api-2.0.0/README.md
--rw-r--r--   0 david     (1000) david     (1000)       38 2024-04-30 20:12:43.195075 skypy-api-2.0.0/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)      658 2024-04-30 19:28:37.000000 skypy-api-2.0.0/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-30 20:12:43.195075 skypy-api-2.0.0/skypy/
--rw-r--r--   0 david     (1000) david     (1000)       30 2024-04-30 19:28:37.000000 skypy-api-2.0.0/skypy/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)     9506 2024-04-30 19:28:37.000000 skypy-api-2.0.0/skypy/main.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2024-04-30 20:12:43.195075 skypy-api-2.0.0/skypy_api.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)      841 2024-04-30 20:12:43.000000 skypy-api-2.0.0/skypy_api.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)      222 2024-04-30 20:12:43.000000 skypy-api-2.0.0/skypy_api.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2024-04-30 20:12:43.000000 skypy-api-2.0.0/skypy_api.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)       14 2024-04-30 20:12:43.000000 skypy-api-2.0.0/skypy_api.egg-info/requires.txt
--rw-r--r--   0 david     (1000) david     (1000)        6 2024-04-30 20:12:43.000000 skypy-api-2.0.0/skypy_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:37:37.588147 skypy_api-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-01 12:37:29.000000 skypy_api-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-01 12:37:37.588147 skypy_api-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-01 12:37:29.000000 skypy_api-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 12:37:37.588147 skypy_api-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-01 12:37:29.000000 skypy_api-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:37:37.588147 skypy_api-2.1.0/skypy/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-01 12:37:29.000000 skypy_api-2.1.0/skypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15936 2024-05-01 12:37:29.000000 skypy_api-2.1.0/skypy/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:37:37.588147 skypy_api-2.1.0/skypy_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-01 12:37:37.000000 skypy_api-2.1.0/skypy_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-01 12:37:37.000000 skypy_api-2.1.0/skypy_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:37:37.000000 skypy_api-2.1.0/skypy_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 12:37:37.000000 skypy_api-2.1.0/skypy_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 12:37:37.000000 skypy_api-2.1.0/skypy_api.egg-info/top_level.txt
```

### Comparing `skypy-api-2.0.0/setup.py` & `skypy_api-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="skypy-api",
     url="https://github.com/FuchsCrafter/skypy",
-    version="2.0.0",
+    version="2.1.0",
     author="FuchsCrafter",
     license="GPL2",
     description="Framework to connect to the Hypixel Skyblock API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `skypy-api-2.0.0/skypy/main.py` & `skypy_api-2.1.0/skypy/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 import requests
 import json
 
 class skypy:
     """ The main class for the module. Uses an api key"""
     def __init__(self, key:str, blockKeyTest:bool=False) -> None:
         global apikey
+        self.changeApiKey(key=key, blockKeyTest=blockKeyTest)
+
+    def changeApiKey(self, key:str, blockKeyTest:bool=False):
+        global apikey
         assert key != ""
         apikey = str(key)
         if not blockKeyTest:
             r = requests.get("https://api.hypixel.net/v2/skyblock/news?key="+ key)
             returns = json.loads(r.text)
             returns = returns["success"]
             if not returns:
@@ -46,14 +50,78 @@
         for element in r:
             returns[element["id"]] = element
         return returns
 
     def getCurrentBingo(self):
         return json.loads(requests.get("https://api.hypixel.net/v2/resources/skyblock/bingo").text)
     
+    def getAllCollectionCategories(self, shortmode:bool=False) -> dict:
+        """Gets all collection categories"""
+        r = requests.get("https://api.hypixel.net/v2/resources/skyblock/collections")
+        r = json.loads(r.text)
+        allCollections = r["collections"]
+        if shortmode:
+            return list(allCollections.keys())
+        else: 
+            return allCollections
+    
+    class collection:
+        """Methods for working with collections"""
+        def __init__(self, category:str):
+            """Ctaegory: sets the category of the collection"""
+            self.category = category.upper()
+            self.renewCache()
+            
+        def __getitem__(self,key):
+            """Shortcut for getCollection()"""
+            return self.getCollection(key)
+
+        def renewCache(self) -> None:
+            """Renews the cache"""
+            r = requests.get("https://api.hypixel.net/v2/resources/skyblock/collections")
+            r = json.loads(r.text)
+
+            self.allCollections = r["collections"]
+            self.all = self.allCollections
+
+            self.collectionCategories = list(self.allCollections.keys())
+            self.categories = self.collectionCategories
+
+            self.categoryData = self.getCategory()
+            self.collections = self.getAllCollections()
+
+            self.version = r["version"]
+            self.lastUpdated = r["lastUpdated"]
+
+        def getCategory(self) -> dict:
+            """Gets the whole category that was selected prior"""
+            out = self.all
+            try:
+                out = out[self.category.upper()]
+            except KeyError:
+                raise ValueError(f"Invalid category name: {self.category.upper()}")
+            else:
+                return out["items"]
+            
+        def getAllCollections(self):
+            """Gets all the names of the collections of the selected category"""
+            return [element["name"] for element in list(self.categoryData.values())]
+
+        def getCollection(self, collection:str, full:bool=False) -> list:
+            """Gets a collection of the selected category"""
+            collectionCategory = self.categoryData
+            collectionName = collection.upper().replace(" ","")
+
+            for element in list(collectionCategory.values()):
+                if element["name"].upper().replace(" ","") == collectionName:
+                    if full:
+                        return element
+                    else:
+                        return element["tiers"]
+                
 
     class bazaar:
         """ The bazaar class was made to get bazaar values from certain items. """
         def __init__(self):
             pass
 
         def fetchAllProducts(self) -> dict:
@@ -87,22 +155,16 @@
             if not returns["success"]:
                 print("Failed! Make sure, that you api key and the uuid is correct!")
             else:
                 return returns["auctions"]
 
         def getAuctionByPlayerName(self, player:str) -> list: 
             """ Uses the Mojang API to get the uuid of a player. """
-            r = requests.get("https://api.mojang.com/users/profiles/minecraft/" + player) # TODO: Create dedicated function for this
-            returns = json.loads(r.text)
-            try:
-                playeruuid = returns["id"]
-            except:
-                print("Invalid Playername!")
-            else: 
-                return self.getAuctionByPlayer(playeruuid)
+            uuid = utility.getPlayerUUID(player=player)
+            return self.getAuctionByPlayer(uuid)
         
         def getAuctionsByPlayer(self, uuid:str) -> list:
             """Alias function for getAuctionByPlayer"""
             return self.getAuctionByPlayer(uuid=uuid)
             
         def getAuctionsByPlayerName(self, player:str) -> list:
             """Alias function for getAuctionByPlayerName"""
@@ -155,19 +217,18 @@
             """ Gets the current mayor an his perks. """
             currentMayor = self.currentElectionCache["mayor"]
             if quickmode:
                 return {"name": currentMayor["name"],"key": currentMayor["key"]}
             else:
                 return currentMayor
 
-        def getCurrentElection(self, quickmode:bool=False, full:bool=True, updateCache:bool=False) -> dict: #TODO: Remaining rewrite, testing
-            """ Gets the current election results.
-            
-            Use the updateCache parameter to update the election cache, or call 
-            the updateElectionCache method of the mayor class to do so."""
+        def getCurrentElection(self, quickmode:bool=False, full:bool=True, updateCache:bool=False) -> dict:
+            """ ### (Deprecated)
+            Gets the current election results.
+            """
             if updateCache:
                 self.updateElectionCache()
             else:
                 returns = self.currentElectionCache
             if "current" in returns:
                 if not quickmode:
                     return returns["current"]
@@ -178,32 +239,111 @@
                         if full:
                             returns[element["name"]] = {"name": element["name"],"key": element["key"], "votes": element["votes"], "perks": element["perks"]}
                         else:
                             returns[element["name"]] = {"name": element["name"],"key": element["key"], "votes": element["votes"]}
                     return returns
             else:
                 return False
+        
+        def getCurrentElectionCandidates(self, full:bool=False, keys:bool=False, updateCache:bool=False):
+            """Gets the current election candidates. 
+                ## Parameters
+                - keys:bool
+                    - If the names should be returned alingside their keys in a dictionary
+                - full:bool
+                    - If the full data set should be returned
+            """
+            if updateCache: self.updateElectionCache()
+            if "current" in self.currentElectionCache:
+                if full:
+                    return self.currentElectionCache["current"]["candidates"]
+                elif keys:
+                    candidates = [element["name"] for element in self.currentElectionCache["current"]["candidates"]]
+                    ckeys = [element["key"] for element in self.currentElectionCache["current"]["candidates"]]
 
-        def getElectionResults(self, updateCache):  #TODO: Remaining rewrite, testing
-            """ Gets only the election votes.
+                    return dict(zip(candidates, ckeys))
+                else:
+                    return [element["name"] for element in self.currentElectionCache["current"]["candidates"]]
+        
+        def getCurrentElectionPerks(self,candidate:str, short:bool=False) -> list:
+            """Gets the Perks of a specific candidate in the current election.
+                ## Parameters
+                - (required) candidate:str 
+                    - The candidate's name (not case-sensitive)
+                - short:bool
+                    - If only the titles of perks should be provided without any description
+            """
+            candidate_org = candidate
+            candidate = candidate.upper()
+            electionCandidates = [el.upper() for el in self.getCurrentElectionCandidates()]
+            if candidate in electionCandidates:
+                fullElection = self.getCurrentElectionCandidates(full=True)
+                for element in fullElection:
+                    if element["name"].upper() == candidate:
+                        if short:
+                            return [el["name"] for el in element["perks"]]
+                        else:
+                            return element["perks"]
+            else: raise ValueError(f"Candidate not in current election: {candidate_org}")
 
-            Use the updateCache parameter to update the election cache, or call 
-            the updateElectionCache method of the mayor class to do so."""
+        def getCurrentElectionVotes(self, candidate:str, updateCache:bool=False) -> int:
+            """Returns the votes of a specific candidate.
+                ## Parameters
+                - (required) candidate:str
+                    - The candidate's name (not case-sensitive)
+            """
             if updateCache:
                 self.updateElectionCache()
-            else:
-                returns = self.currentElectionCache
-            if "current" in returns:
-                _ = returns["current"]["candidates"]
-                returns = {}
-                for element in _:
-                    returns[element["name"]] = element["votes"]
-                return returns
-            else:
-                return False
+            candidate_org = candidate
+            candidate = candidate.upper()
+            electionCandidates = [el.upper() for el in self.getCurrentElectionCandidates()]
+            if candidate in electionCandidates:
+                fullElection = self.getCurrentElectionCandidates(full=True)
+                for element in fullElection:
+                    if element["name"].upper() == candidate:
+                        return element["votes"]
+            else: raise ValueError(f"Candidate not in current election: {candidate_org}")
+        
+        def getCurrentElectionKeys(self, updateCache:bool=False) -> list:
+            """Gets the key of all candidates in the current election into a list"""
+            return list(self.getCurrentElectionCandidates(keys=True, updateCache=updateCache).values())
+
+
+        def getElectionResults(self, updateCache:bool=False) -> dict[str, int]:
+            """ Gets all the election votes with the candidates in a dict"""
+            if updateCache: self.updateElectionCache()
+            candidates = self.getCurrentElectionCandidates()
+            votes = []
+            for candidate in candidates:
+                votes.append(self.getCurrentElectionVotes(candidate=candidate, updateCache=False))
+            return dict(zip(candidates,votes))
+        
+        def getCurrentElectionResults(self, updateCache:bool=False) -> dict[str, int]:
+            """ Gets all the election votes with the candidates in a dict"""
+            return self.getElectionResults(updateCache=updateCache)
+
+
     class politics(mayor):
         """# Attention: Class was renamed!
             This class was renamed to 'mayor', but remains as a synonym of 'mayor'. 
             
             Please do not use it when writing new code!
         """
         pass
+
+class utility:
+    """Utility class"""
+    def getPlayerUUID(player:str) -> str:
+        r = requests.get("https://api.mojang.com/users/profiles/minecraft/" + player)
+        returns = json.loads(r.text)
+        try:
+            uuid = returns["id"]
+        except KeyError:
+            raise ValueError(f"Invalid player name: {player}")
+        else: 
+            return uuid
+    def capitalize_keys(d): # Source: https://stackoverflow.com/a/9700528
+        result = {}
+        for key, value in d.items():
+            upper_key = key.upper()
+            result[upper_key] = result.get(upper_key, 0) + value
+        return result
```


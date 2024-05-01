# Comparing `tmp/LanusStats-1.2.0.tar.gz` & `tmp/LanusStats-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LanusStats-1.2.0.tar", last modified: Mon Apr 29 03:45:13 2024, max compression
+gzip compressed data, was "LanusStats-1.3.0.tar", last modified: Wed May  1 19:30:56 2024, max compression
```

## Comparing `LanusStats-1.2.0.tar` & `LanusStats-1.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 03:45:13.707935 LanusStats-1.2.0/
-drwxrwxrwx   0        0        0        0 2024-04-29 03:45:13.684503 LanusStats-1.2.0/LanusStats/
--rw-rw-rw-   0        0        0      222 2024-04-07 03:06:19.000000 LanusStats-1.2.0/LanusStats/__init__.py
--rw-rw-rw-   0        0        0      234 2024-04-13 23:20:47.000000 LanusStats-1.2.0/LanusStats/config.py
--rw-rw-rw-   0        0        0     1759 2024-04-04 03:40:59.000000 LanusStats-1.2.0/LanusStats/exceptions.py
--rw-rw-rw-   0        0        0    14960 2024-04-29 02:16:12.000000 LanusStats-1.2.0/LanusStats/fbref.py
--rw-rw-rw-   0        0        0    11508 2024-04-13 23:20:47.000000 LanusStats-1.2.0/LanusStats/fotmob.py
--rw-rw-rw-   0        0        0    17922 2024-04-14 02:10:59.000000 LanusStats-1.2.0/LanusStats/functions.py
--rw-rw-rw-   0        0        0     3984 2024-04-14 02:31:00.000000 LanusStats-1.2.0/LanusStats/sofascore.py
--rw-rw-rw-   0        0        0     9140 2024-04-29 03:44:07.000000 LanusStats-1.2.0/LanusStats/threesixfivescores.py
--rw-rw-rw-   0        0        0     8640 2024-04-07 03:10:29.000000 LanusStats-1.2.0/LanusStats/visualizations.py
-drwxrwxrwx   0        0        0        0 2024-04-29 03:45:13.702464 LanusStats-1.2.0/LanusStats.egg-info/
--rw-rw-rw-   0        0        0     8177 2024-04-29 03:45:13.000000 LanusStats-1.2.0/LanusStats.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      407 2024-04-29 03:45:13.000000 LanusStats-1.2.0/LanusStats.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 03:45:13.000000 LanusStats-1.2.0/LanusStats.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-29 03:45:13.000000 LanusStats-1.2.0/LanusStats.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-29 03:45:13.000000 LanusStats-1.2.0/LanusStats.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8177 2024-04-29 03:45:13.706219 LanusStats-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     7795 2024-04-29 02:16:12.000000 LanusStats-1.2.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 03:45:13.708721 LanusStats-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1012 2024-04-29 03:44:17.000000 LanusStats-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 19:30:56.056651 LanusStats-1.3.0/
+drwxrwxrwx   0        0        0        0 2024-05-01 19:30:56.029708 LanusStats-1.3.0/LanusStats/
+-rw-rw-rw-   0        0        0      222 2024-04-07 03:06:19.000000 LanusStats-1.3.0/LanusStats/__init__.py
+-rw-rw-rw-   0        0        0     1189 2024-05-01 19:28:29.000000 LanusStats-1.3.0/LanusStats/config.py
+-rw-rw-rw-   0        0        0     1731 2024-05-01 19:28:29.000000 LanusStats-1.3.0/LanusStats/exceptions.py
+-rw-rw-rw-   0        0        0    14960 2024-05-01 19:28:29.000000 LanusStats-1.3.0/LanusStats/fbref.py
+-rw-rw-rw-   0        0        0    11603 2024-05-01 19:28:29.000000 LanusStats-1.3.0/LanusStats/fotmob.py
+-rw-rw-rw-   0        0        0    16880 2024-05-01 19:28:29.000000 LanusStats-1.3.0/LanusStats/functions.py
+-rw-rw-rw-   0        0        0      303 2024-05-01 19:28:29.000000 LanusStats-1.3.0/LanusStats/sofascore.py
+-rw-rw-rw-   0        0        0     9558 2024-05-01 19:28:29.000000 LanusStats-1.3.0/LanusStats/threesixfivescores.py
+-rw-rw-rw-   0        0        0    17372 2024-05-01 19:28:29.000000 LanusStats-1.3.0/LanusStats/visualizations.py
+drwxrwxrwx   0        0        0        0 2024-05-01 19:30:56.047589 LanusStats-1.3.0/LanusStats.egg-info/
+-rw-rw-rw-   0        0        0     8177 2024-05-01 19:30:55.000000 LanusStats-1.3.0/LanusStats.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      407 2024-05-01 19:30:55.000000 LanusStats-1.3.0/LanusStats.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 19:30:55.000000 LanusStats-1.3.0/LanusStats.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-01 19:30:55.000000 LanusStats-1.3.0/LanusStats.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-01 19:30:55.000000 LanusStats-1.3.0/LanusStats.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8177 2024-05-01 19:30:56.054643 LanusStats-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7795 2024-05-01 19:28:29.000000 LanusStats-1.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-01 19:30:56.057699 LanusStats-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1012 2024-05-01 19:30:31.000000 LanusStats-1.3.0/setup.py
```

### Comparing `LanusStats-1.2.0/LanusStats/exceptions.py` & `LanusStats-1.3.0/LanusStats/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class InvalidSeasonException(Exception):
     def __init__(self, season, possible_seasons_list):
         self.message = f"Season {season} is not valid for any of the possible seasons for this league {possible_seasons_list}."
         super().__init__(self.message)
 
 class PlayerDoesntHaveInfo(Exception):
     def __init__(self, path):
-        self.message = f"Player in path {path} doesn't have percentiles or similarities in his scouting report, try with another one.\nEl jugador en el path {path} no tiene percentiles o similitudes en su reporte de scouting, pruebe con otro."
+        self.message = f"Player in path {path} doesn't have enough information for this functions, try with another one.\nEl jugador en el path {path} no tiene la información para estas funciones, pruebe con otro."
         super().__init__(self.message)
 
 class MatchDoesntHaveInfo(Exception):
     def __init__(self, path):
         self.message = f"Match in path {path} doesn't have enough information for this functions, try with another one.\nEl partido en el path {path} no tiene la información para estas funciones, pruebe con otro."
         super().__init__(self.message)
```

### Comparing `LanusStats-1.2.0/LanusStats/fbref.py` & `LanusStats-1.3.0/LanusStats/fbref.py`

 * *Files identical despite different names*

### Comparing `LanusStats-1.2.0/LanusStats/fotmob.py` & `LanusStats-1.3.0/LanusStats/fotmob.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,9 +249,12 @@
             shotmap: DataFrame with the data for all the shots shown in the FotMob UI.
         """
         leagues = get_possible_leagues_for_page(league, season, 'Fotmob')
         league_id = leagues[league]['id']
         season_string = season.replace('/', '%2F')
         response = requests.get(f'https://www.fotmob.com/api/playerStats?playerId={player_id}&seasonId={season_string}-{league_id}', headers=headers)
         time.sleep(3)
-        shotmap = pd.DataFrame(response.json()['shotmap'])
+        try:
+            shotmap = pd.DataFrame(response.json()['shotmap'])
+        except TypeError:
+            raise MatchDoesntHaveInfo(player_id)
         return shotmap
```

### Comparing `LanusStats-1.2.0/LanusStats/functions.py` & `LanusStats-1.3.0/LanusStats/functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,9 @@
 from .exceptions import *
-from IPython.display import clear_output
-import pandas as pd
-from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.common.by import By
-import random
 import numpy as np
-import undetected_chromedriver as uc
 
 def get_possible_leagues(league, season, page):
     """Dictionary with all the possible pages, leagues and season for the scraper.
     Also contains some exception to prevent errors such as a league or page that is not a part of the scraper.
 
     Args:
         league (str): League to scrape
@@ -487,42 +481,15 @@
 
     Returns:
         dict: League data with the seasons inside
     """
     league_data = get_possible_leagues('Argentina Copa de la Liga', '2023', 'Fotmob')[page][league]
     return league_data
 
-def get_proxy():
-    ''' Gets a proxy address.
-
-    Code used by Owen Seymour in ScraperFC, here:
-    https://github.com/oseymour/ScraperFC/blob/main/ScraperFC/shared_functions.py#L628 
-    
-    Returns
-    -------
-    proxy : str
-        In the form <IP address>:<port>
-    '''
-    options = Options()
-    options.add_argument('--headless')
-    driver = uc.Chrome(headless=True,use_subprocess=False,option=options)
-    clear_output()
-    
-    try:
-        driver.get('https://sslproxies.org/')
-        table = driver.find_elements(By.TAG_NAME, 'table')[0]
-        df = pd.read_html(table.get_attribute('outerHTML'))[0]
-        df = df.iloc[np.where(~np.isnan(df['Port']))[0],:] # ignore nans
-
-        ips = df['IP Address'].values
-        ports = df['Port'].astype('int').values
-
-        driver.quit()
-        proxies = list()
-        for i in range(len(ips)):
-            proxies.append('{}:{}'.format(ips[i], ports[i]))
-        i = random.randint(0, len(proxies)-1)
-        return proxies[i]
-    except Exception as e:
-        driver.close()
-        driver.quit()
-        raise e
+def semicircle(r, h, k):
+    x0 = h - r  # determine x start
+    x1 = h + r  # determine x finish
+    x = np.linspace(x0, x1, 10000)  # many points to solve for y
+
+    # use numpy for array solving of the semicircle equation
+    y = k - np.sqrt(r**2 - (x - h)**2)  
+    return x, y
```

### Comparing `LanusStats-1.2.0/LanusStats/threesixfivescores.py` & `LanusStats-1.3.0/LanusStats/threesixfivescores.py`

 * *Files 8% similar despite different names*

```diff
@@ -145,14 +145,17 @@
         """
         match_data = self.get_match_data(match_url)
         try:
             json_tiros = match_data['chartEvents']['events']
         except KeyError:
             raise MatchDoesntHaveInfo(match_url)
         df = pd.DataFrame(json_tiros)
+        df['xgot'] = df.xgot.str.replace('-','0')
+        df[['xg', 'xgot']] = df[['xg', 'xgot']].astype(float)
+        df = pd.concat([df, df['outcome'].apply(pd.Series).rename(columns={'name': 'shot_outcome'})],axis=1).drop(columns='outcome')
         return df
     
     def get_players_info(self, match_url):
         """Get players info for a certain match
 
         Args:
             match_url (url): 365Scores match URL. Example: https://www.365scores.com/es-mx/football/match/copa-de-la-liga-profesional-7214/lanus-union-santa-fe-869-7206-7214#id=4033824
@@ -165,28 +168,32 @@
         teams_df = pd.DataFrame(teams_json)
         return teams_df
     
     def get_team_data(self, match_url):
         values = ['home', 'away']
         names = []
         ids = []
+        colors = []
         match_data = self.get_match_data(match_url)
         for value in values:
-            nombre = match_data[f'{value}Competitor']['name']
+            name = match_data[f'{value}Competitor']['name']
             id = match_data[f'{value}Competitor']['id']
-            names.append(nombre), ids.append(id)
+            color = match_data[f'{value}Competitor']['color']
+            names.append(name), ids.append(id), colors.append(color)
         
         home = {
             'name': names[0],
-            'id': id[0]
+            'id': ids[0],
+            'color': colors[0]
         }
         
         away = {
             'name': names[1],
-            'id': id[1]
+            'id': ids[1],
+            'color': colors[1]
         }
         
         return home, away
     
     def get_general_match_stats(self, match_url):
         """Get general statistics for teams from a match
```

### Comparing `LanusStats-1.2.0/LanusStats.egg-info/PKG-INFO` & `LanusStats-1.3.0/LanusStats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LanusStats
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python library for scraping football data and visualize it / Libreria de Python para scrapear data de fútbol y visualizarla
 Home-page: https://github.com/federicorabanos
 Author: Federico Rábanos
 Author-email: lanusstats@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `LanusStats-1.2.0/PKG-INFO` & `LanusStats-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LanusStats
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python library for scraping football data and visualize it / Libreria de Python para scrapear data de fútbol y visualizarla
 Home-page: https://github.com/federicorabanos
 Author: Federico Rábanos
 Author-email: lanusstats@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `LanusStats-1.2.0/README.md` & `LanusStats-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `LanusStats-1.2.0/setup.py` & `LanusStats-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.2.0'
+VERSION = '1.3.0'
 PACKAGE_NAME = 'LanusStats'
 AUTHOR = 'Federico Rábanos'
 AUTHOR_EMAIL = 'lanusstats@gmail.com'
 URL = 'https://github.com/federicorabanos'
 
 LICENSE = 'MIT'
 DESCRIPTION = 'Python library for scraping football data and visualize it / Libreria de Python para scrapear data de fútbol y visualizarla'
```


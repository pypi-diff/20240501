# Comparing `tmp/dwdhandler-0.2.1.tar.gz` & `tmp/dwdhandler-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwdhandler-0.2.1.tar", last modified: Sat Apr 27 17:13:52 2024, max compression
+gzip compressed data, was "dwdhandler-0.2.2.tar", last modified: Wed May  1 19:51:39 2024, max compression
```

## Comparing `dwdhandler-0.2.1.tar` & `dwdhandler-0.2.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-04-27 17:13:52.155254 dwdhandler-0.2.1/
--rw-rw-r--   0 tobias    (1000) tobias    (1000)    35148 2024-03-21 19:39:06.000000 dwdhandler-0.2.1/LICENSE
--rw-r--r--   0 tobias    (1000) tobias    (1000)    41886 2024-04-27 17:13:52.155254 dwdhandler-0.2.1/PKG-INFO
--rw-rw-r--   0 tobias    (1000) tobias    (1000)      478 2024-03-23 11:22:42.000000 dwdhandler-0.2.1/README.md
--rw-rw-r--   0 tobias    (1000) tobias    (1000)      968 2024-04-27 17:12:45.000000 dwdhandler-0.2.1/pyproject.toml
--rw-rw-r--   0 tobias    (1000) tobias    (1000)      751 2024-04-27 17:13:52.155254 dwdhandler-0.2.1/setup.cfg
-drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-04-27 17:13:52.151254 dwdhandler-0.2.1/src/
-drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-04-27 17:13:52.151254 dwdhandler-0.2.1/src/dwdhandler/
--rw-rw-r--   0 tobias    (1000) tobias    (1000)      196 2024-04-27 12:45:25.000000 dwdhandler-0.2.1/src/dwdhandler/__init__.py
-drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-04-27 17:13:52.151254 dwdhandler-0.2.1/src/dwdhandler/calculation/
--rw-rw-r--   0 tobias    (1000) tobias    (1000)        0 2022-02-21 20:37:50.000000 dwdhandler-0.2.1/src/dwdhandler/calculation/__init__.py
--rw-rw-r--   0 tobias    (1000) tobias    (1000)    22878 2023-10-23 18:15:18.000000 dwdhandler-0.2.1/src/dwdhandler/calculation/calc_stats.py
--rw-rw-r--   0 tobias    (1000) tobias    (1000)     1550 2024-04-22 11:36:15.000000 dwdhandler-0.2.1/src/dwdhandler/calculation/geo.py
--rw-rw-r--   0 tobias    (1000) tobias    (1000)     5010 2023-08-17 16:59:09.000000 dwdhandler-0.2.1/src/dwdhandler/calculation/return_period.py
-drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-04-27 17:13:52.155254 dwdhandler-0.2.1/src/dwdhandler/constants/
--rw-rw-r--   0 tobias    (1000) tobias    (1000)        0 2021-06-08 15:54:47.000000 dwdhandler-0.2.1/src/dwdhandler/constants/__init__.py
--rw-rw-r--   0 tobias    (1000) tobias    (1000)     1742 2024-03-24 17:56:23.000000 dwdhandler-0.2.1/src/dwdhandler/constants/constpar.py
--rw-rw-r--   0 tobias    (1000) tobias    (1000)     6062 2023-07-02 12:20:04.000000 dwdhandler-0.2.1/src/dwdhandler/constants/filedata.py
--rw-rw-r--   0 tobias    (1000) tobias    (1000)      542 2022-01-22 16:29:40.000000 dwdhandler-0.2.1/src/dwdhandler/constants/serverdata.py
--rw-rw-r--   0 tobias    (1000) tobias    (1000)    44023 2024-03-23 11:08:12.000000 dwdhandler-0.2.1/src/dwdhandler/dow_handler.py
-drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-04-27 17:13:52.155254 dwdhandler-0.2.1/src/dwdhandler/helper/
--rw-rw-r--   0 tobias    (1000) tobias    (1000)        0 2021-06-08 15:54:47.000000 dwdhandler-0.2.1/src/dwdhandler/helper/__init__.py
--rw-rw-r--   0 tobias    (1000) tobias    (1000)     1447 2023-06-05 18:14:27.000000 dwdhandler-0.2.1/src/dwdhandler/helper/ftp.py
--rw-rw-r--   0 tobias    (1000) tobias    (1000)    20327 2024-04-27 12:41:53.000000 dwdhandler-0.2.1/src/dwdhandler/helper/hfunctions.py
-drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-04-27 17:13:52.155254 dwdhandler-0.2.1/src/dwdhandler/plotting/
--rw-rw-r--   0 tobias    (1000) tobias    (1000)        0 2021-12-04 10:40:07.000000 dwdhandler-0.2.1/src/dwdhandler/plotting/__init__.py
--rw-rw-r--   0 tobias    (1000) tobias    (1000)   105384 2024-03-30 13:14:30.000000 dwdhandler-0.2.1/src/dwdhandler/plotting/plotconstr.py
-drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-04-27 17:13:52.155254 dwdhandler-0.2.1/src/dwdhandler.egg-info/
--rw-r--r--   0 tobias    (1000) tobias    (1000)    41886 2024-04-27 17:13:52.000000 dwdhandler-0.2.1/src/dwdhandler.egg-info/PKG-INFO
--rw-rw-r--   0 tobias    (1000) tobias    (1000)      769 2024-04-27 17:13:52.000000 dwdhandler-0.2.1/src/dwdhandler.egg-info/SOURCES.txt
--rw-rw-r--   0 tobias    (1000) tobias    (1000)        1 2024-04-27 17:13:52.000000 dwdhandler-0.2.1/src/dwdhandler.egg-info/dependency_links.txt
--rw-rw-r--   0 tobias    (1000) tobias    (1000)       83 2024-04-27 17:13:52.000000 dwdhandler-0.2.1/src/dwdhandler.egg-info/requires.txt
--rw-rw-r--   0 tobias    (1000) tobias    (1000)       11 2024-04-27 17:13:52.000000 dwdhandler-0.2.1/src/dwdhandler.egg-info/top_level.txt
+drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-05-01 19:51:39.669787 dwdhandler-0.2.2/
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)    35148 2024-03-21 19:39:06.000000 dwdhandler-0.2.2/LICENSE
+-rw-r--r--   0 tobias    (1000) tobias    (1000)    41886 2024-05-01 19:51:39.669787 dwdhandler-0.2.2/PKG-INFO
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)      478 2024-03-23 11:22:42.000000 dwdhandler-0.2.2/README.md
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)      968 2024-04-27 17:12:45.000000 dwdhandler-0.2.2/pyproject.toml
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)      762 2024-05-01 19:51:39.669787 dwdhandler-0.2.2/setup.cfg
+drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-05-01 19:51:39.661787 dwdhandler-0.2.2/src/
+drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-05-01 19:51:39.665787 dwdhandler-0.2.2/src/dwdhandler/
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)      196 2024-05-01 19:50:44.000000 dwdhandler-0.2.2/src/dwdhandler/__init__.py
+drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-05-01 19:51:39.665787 dwdhandler-0.2.2/src/dwdhandler/calculation/
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)        0 2022-02-21 20:37:50.000000 dwdhandler-0.2.2/src/dwdhandler/calculation/__init__.py
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)    22878 2023-10-23 18:15:18.000000 dwdhandler-0.2.2/src/dwdhandler/calculation/calc_stats.py
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)     1550 2024-04-22 11:36:15.000000 dwdhandler-0.2.2/src/dwdhandler/calculation/geo.py
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)     5010 2023-08-17 16:59:09.000000 dwdhandler-0.2.2/src/dwdhandler/calculation/return_period.py
+drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-05-01 19:51:39.665787 dwdhandler-0.2.2/src/dwdhandler/constants/
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)        0 2021-06-08 15:54:47.000000 dwdhandler-0.2.2/src/dwdhandler/constants/__init__.py
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)     1742 2024-03-24 17:56:23.000000 dwdhandler-0.2.2/src/dwdhandler/constants/constpar.py
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)     6062 2023-07-02 12:20:04.000000 dwdhandler-0.2.2/src/dwdhandler/constants/filedata.py
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)      542 2022-01-22 16:29:40.000000 dwdhandler-0.2.2/src/dwdhandler/constants/serverdata.py
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)    44023 2024-03-23 11:08:12.000000 dwdhandler-0.2.2/src/dwdhandler/dow_handler.py
+drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-05-01 19:51:39.665787 dwdhandler-0.2.2/src/dwdhandler/helper/
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)        0 2021-06-08 15:54:47.000000 dwdhandler-0.2.2/src/dwdhandler/helper/__init__.py
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)     1447 2023-06-05 18:14:27.000000 dwdhandler-0.2.2/src/dwdhandler/helper/ftp.py
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)    19564 2024-05-01 19:41:59.000000 dwdhandler-0.2.2/src/dwdhandler/helper/hfunctions.py
+drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-05-01 19:51:39.665787 dwdhandler-0.2.2/src/dwdhandler/plotting/
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)        0 2021-12-04 10:40:07.000000 dwdhandler-0.2.2/src/dwdhandler/plotting/__init__.py
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)   105384 2024-03-30 13:14:30.000000 dwdhandler-0.2.2/src/dwdhandler/plotting/plotconstr.py
+drwxrwxr-x   0 tobias    (1000) tobias    (1000)        0 2024-05-01 19:51:39.669787 dwdhandler-0.2.2/src/dwdhandler.egg-info/
+-rw-r--r--   0 tobias    (1000) tobias    (1000)    41886 2024-05-01 19:51:39.000000 dwdhandler-0.2.2/src/dwdhandler.egg-info/PKG-INFO
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)      769 2024-05-01 19:51:39.000000 dwdhandler-0.2.2/src/dwdhandler.egg-info/SOURCES.txt
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)        1 2024-05-01 19:51:39.000000 dwdhandler-0.2.2/src/dwdhandler.egg-info/dependency_links.txt
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)       83 2024-05-01 19:51:39.000000 dwdhandler-0.2.2/src/dwdhandler.egg-info/requires.txt
+-rw-rw-r--   0 tobias    (1000) tobias    (1000)       11 2024-05-01 19:51:39.000000 dwdhandler-0.2.2/src/dwdhandler.egg-info/top_level.txt
```

### Comparing `dwdhandler-0.2.1/LICENSE` & `dwdhandler-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dwdhandler-0.2.1/PKG-INFO` & `dwdhandler-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwdhandler
-Version: 0.2.1
+Version: 0.2.2
 Summary: Package to handle data from German Weather Service and some simple plotting routines
 Home-page: https://github.com/MrTscha/dwdhandler
 Author: Tobias Schad
 Author-email: Tobias Schad <tobias.schad@googlemail.com>
 Maintainer-email: Tobias Schad <tobias.schad@googlemail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `dwdhandler-0.2.1/pyproject.toml` & `dwdhandler-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dwdhandler-0.2.1/setup.cfg` & `dwdhandler-0.2.2/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
 	numpy
 	pandas
+	pysqlite3
 	seaborn
 	matplotlib
 	folium
 	plotly
 	scipy
 
 [options.packages.find]
```

### Comparing `dwdhandler-0.2.1/src/dwdhandler/calculation/calc_stats.py` & `dwdhandler-0.2.2/src/dwdhandler/calculation/calc_stats.py`

 * *Files identical despite different names*

### Comparing `dwdhandler-0.2.1/src/dwdhandler/calculation/geo.py` & `dwdhandler-0.2.2/src/dwdhandler/calculation/geo.py`

 * *Files identical despite different names*

### Comparing `dwdhandler-0.2.1/src/dwdhandler/calculation/return_period.py` & `dwdhandler-0.2.2/src/dwdhandler/calculation/return_period.py`

 * *Files identical despite different names*

### Comparing `dwdhandler-0.2.1/src/dwdhandler/constants/constpar.py` & `dwdhandler-0.2.2/src/dwdhandler/constants/constpar.py`

 * *Files identical despite different names*

### Comparing `dwdhandler-0.2.1/src/dwdhandler/constants/filedata.py` & `dwdhandler-0.2.2/src/dwdhandler/constants/filedata.py`

 * *Files identical despite different names*

### Comparing `dwdhandler-0.2.1/src/dwdhandler/constants/serverdata.py` & `dwdhandler-0.2.2/src/dwdhandler/constants/serverdata.py`

 * *Files identical despite different names*

### Comparing `dwdhandler-0.2.1/src/dwdhandler/dow_handler.py` & `dwdhandler-0.2.2/src/dwdhandler/dow_handler.py`

 * *Files identical despite different names*

### Comparing `dwdhandler-0.2.1/src/dwdhandler/helper/ftp.py` & `dwdhandler-0.2.2/src/dwdhandler/helper/ftp.py`

 * *Files identical despite different names*

### Comparing `dwdhandler-0.2.1/src/dwdhandler/helper/hfunctions.py` & `dwdhandler-0.2.2/src/dwdhandler/helper/hfunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,47 +31,26 @@
     """ Reads DWD station list metadata """
 
     if(debug):
         print("Open file {} and read station list".format(dir_in+file_in))
 
     check_file_encoding(dir_in,file_in)
 
-    input_file = open(dir_in+file_in,"r")
-
-    lines = input_file.readlines()
-
-    i = 0
-
-    station_list = {}
-
-    for line in lines:
-        if(i == 0):
-            header = line.split()
-        elif(i > 1): # skip second line...
-            station_key = line[0:5]
-            year, month, day = extract_yyyymmdd(line[21:30])
-            b_date      = datetime.datetime(int(year), int(month), int(day))
-            year, month, day = extract_yyyymmdd(line[30:38])
-            e_date      = datetime.datetime(int(year), int(month), int(day))
-            height      = line[49:53].replace(" ","")
-            height      = np.float(height)
-            lat         = float(line[58:65])
-            lon         = float(line[68:75])
-            name        = line[76:156].rstrip()
-            state       = line[157:204].rstrip()
-            station_list[station_key] = {'von':b_date,'bis':e_date,
-                                     'hoehe':height,'lat':lat,'lon':lon,
-                                     'name':name,'bundesland':state}
-        i += 1
+    # First Line and Line with ------ ----- are skipped
+    df_out = pd.read_fwf(dir_in+file_in,skiprows=[0,1],
+                          names=['Stations_id', 'von', 'bis', 'hoehe','lat','lon','name','bundesland']) 
+    df_out['Stations_id'] = df_out['Stations_id'].apply(lambda x: '{0:0>5}'.format(x))
+    df_out['von'] = pd.to_datetime(df_out['von'],format="%Y%m%d")
+    df_out['bis'] = pd.to_datetime(df_out['bis'],format="%Y%m%d")
+    df_out.set_index('Stations_id', inplace=True)
 
     if(debug):
-        print("{} stations read".format(i-2))                                                                     
-        #print(station_list)                                                                                      
+        print("{} stations read".format(df_out.shape[0]))
 
-    return pd.DataFrame(station_list).T 
+    return df_out
 
 def extract_yyyymmdd(date,sep=''):                                                                                                                                                                                                           
     """ extracts hour day month year from string of yyyymmddhh or with seperator                                      
     and returns it as string. 
     if the date is seperated specify the seperator:                                                                   
         for exammple: sep='.' in case of a dot as seperator                                                           
     """
```

### Comparing `dwdhandler-0.2.1/src/dwdhandler/plotting/plotconstr.py` & `dwdhandler-0.2.2/src/dwdhandler/plotting/plotconstr.py`

 * *Files identical despite different names*

### Comparing `dwdhandler-0.2.1/src/dwdhandler.egg-info/PKG-INFO` & `dwdhandler-0.2.2/src/dwdhandler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwdhandler
-Version: 0.2.1
+Version: 0.2.2
 Summary: Package to handle data from German Weather Service and some simple plotting routines
 Home-page: https://github.com/MrTscha/dwdhandler
 Author: Tobias Schad
 Author-email: Tobias Schad <tobias.schad@googlemail.com>
 Maintainer-email: Tobias Schad <tobias.schad@googlemail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `dwdhandler-0.2.1/src/dwdhandler.egg-info/SOURCES.txt` & `dwdhandler-0.2.2/src/dwdhandler.egg-info/SOURCES.txt`

 * *Files identical despite different names*


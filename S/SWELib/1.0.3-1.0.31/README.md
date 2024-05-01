# Comparing `tmp/SWELib-1.0.3.tar.gz` & `tmp/SWELib-1.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SWELib-1.0.3.tar", last modified: Wed May  1 04:51:25 2024, max compression
+gzip compressed data, was "SWELib-1.0.31.tar", last modified: Wed May  1 05:00:22 2024, max compression
```

## Comparing `SWELib-1.0.3.tar` & `SWELib-1.0.31.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 felixfernando   (501) staff       (20)        0 2024-05-01 04:51:25.889476 SWELib-1.0.3/
--rw-r--r--   0 felixfernando   (501) staff       (20)      382 2024-05-01 04:51:25.889344 SWELib-1.0.3/PKG-INFO
-drwxr-xr-x   0 felixfernando   (501) staff       (20)        0 2024-05-01 04:51:25.888515 SWELib-1.0.3/SWELib/
--rw-r--r--   0 felixfernando   (501) staff       (20)       22 2024-04-30 13:33:32.000000 SWELib-1.0.3/SWELib/__init__.py
--rw-r--r--   0 felixfernando   (501) staff       (20)    12384 2024-05-01 04:50:49.000000 SWELib-1.0.3/SWELib/main.py
-drwxr-xr-x   0 felixfernando   (501) staff       (20)        0 2024-05-01 04:51:25.889162 SWELib-1.0.3/SWELib.egg-info/
--rw-r--r--   0 felixfernando   (501) staff       (20)      382 2024-05-01 04:51:25.000000 SWELib-1.0.3/SWELib.egg-info/PKG-INFO
--rw-r--r--   0 felixfernando   (501) staff       (20)      191 2024-05-01 04:51:25.000000 SWELib-1.0.3/SWELib.egg-info/SOURCES.txt
--rw-r--r--   0 felixfernando   (501) staff       (20)        1 2024-05-01 04:51:25.000000 SWELib-1.0.3/SWELib.egg-info/dependency_links.txt
--rw-r--r--   0 felixfernando   (501) staff       (20)       32 2024-05-01 04:51:25.000000 SWELib-1.0.3/SWELib.egg-info/requires.txt
--rw-r--r--   0 felixfernando   (501) staff       (20)        7 2024-05-01 04:51:25.000000 SWELib-1.0.3/SWELib.egg-info/top_level.txt
--rw-r--r--   0 felixfernando   (501) staff       (20)       38 2024-05-01 04:51:25.889528 SWELib-1.0.3/setup.cfg
--rw-r--r--   0 felixfernando   (501) staff       (20)      354 2024-05-01 04:51:02.000000 SWELib-1.0.3/setup.py
+drwxr-xr-x   0 felixfernando   (501) staff       (20)        0 2024-05-01 05:00:22.008467 SWELib-1.0.31/
+-rw-r--r--   0 felixfernando   (501) staff       (20)      383 2024-05-01 05:00:22.008336 SWELib-1.0.31/PKG-INFO
+drwxr-xr-x   0 felixfernando   (501) staff       (20)        0 2024-05-01 05:00:22.007353 SWELib-1.0.31/SWELib/
+-rw-r--r--   0 felixfernando   (501) staff       (20)       22 2024-04-30 13:33:32.000000 SWELib-1.0.31/SWELib/__init__.py
+-rw-r--r--   0 felixfernando   (501) staff       (20)    12505 2024-05-01 05:00:04.000000 SWELib-1.0.31/SWELib/main.py
+drwxr-xr-x   0 felixfernando   (501) staff       (20)        0 2024-05-01 05:00:22.008149 SWELib-1.0.31/SWELib.egg-info/
+-rw-r--r--   0 felixfernando   (501) staff       (20)      383 2024-05-01 05:00:21.000000 SWELib-1.0.31/SWELib.egg-info/PKG-INFO
+-rw-r--r--   0 felixfernando   (501) staff       (20)      191 2024-05-01 05:00:21.000000 SWELib-1.0.31/SWELib.egg-info/SOURCES.txt
+-rw-r--r--   0 felixfernando   (501) staff       (20)        1 2024-05-01 05:00:21.000000 SWELib-1.0.31/SWELib.egg-info/dependency_links.txt
+-rw-r--r--   0 felixfernando   (501) staff       (20)       32 2024-05-01 05:00:21.000000 SWELib-1.0.31/SWELib.egg-info/requires.txt
+-rw-r--r--   0 felixfernando   (501) staff       (20)        7 2024-05-01 05:00:21.000000 SWELib-1.0.31/SWELib.egg-info/top_level.txt
+-rw-r--r--   0 felixfernando   (501) staff       (20)       38 2024-05-01 05:00:22.008525 SWELib-1.0.31/setup.cfg
+-rw-r--r--   0 felixfernando   (501) staff       (20)      355 2024-05-01 05:00:13.000000 SWELib-1.0.31/setup.py
```

### Comparing `SWELib-1.0.3/SWELib/main.py` & `SWELib-1.0.31/SWELib/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,38 +149,40 @@
             print('Please use plot_across_spatial_2d instead')
             return
         if (t > self.get_computational_domain('T')):
             print('Inputted t is too big')
             return
 
         Nx = self.get_computational_domain('Nx')
+        Nt = self.get_computational_domain('Nt')
         L = self.get_computational_domain('L')
         L_arr = np.linspace(0, L, Nx)
 
         plt.figure()
-        plt.plot(L_arr[:Nx], self.get_eta()[:Nx, t])
+        plt.plot(L_arr[:Nx], self.get_eta()[:Nx, int(t // Nt)])
         plt.xlabel('$x$')
         plt.title(f'$t={t}$')
         plt.grid()
 
     def plot_across_time(self, x):
         if (self.type == '2d'):
             print('Please use plot_across_time_2d instead')
             return
 
-        if (x > self.get_computational_domain('L')):
+        if (Nx > self.get_computational_domain('L')):
             print('Inputted x is too big')
             return
 
         Nt = self.get_computational_domain('Nt')
+        Nx = self.get_computational_domain('Nx')
         T = self.get_computational_domain('T')
         T_arr = np.linspace(0, T, Nt)
 
         plt.figure()
-        plt.plot(T_arr[:Nt], self.get_eta()[x, :Nt])
+        plt.plot(T_arr[:Nt], self.get_eta()[int(x // Nx), :Nt])
         plt.xlabel('t')
         plt.title(f'$x={x}$')
 
     def generate_animation(self, y_lim, Nt):
         if (self.type == '2d'):
             print('Please use generate_animation_2d instead')
             return
```


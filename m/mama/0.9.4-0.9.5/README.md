# Comparing `tmp/mama-0.9.4.tar.gz` & `tmp/mama-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mama-0.9.4.tar", last modified: Tue Apr 30 10:39:02 2024, max compression
+gzip compressed data, was "mama-0.9.5.tar", last modified: Wed May  1 11:07:00 2024, max compression
```

## Comparing `mama-0.9.4.tar` & `mama-0.9.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-04-30 10:39:02.811510 mama-0.9.4/
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1062 2024-01-20 16:30:57.000000 mama-0.9.4/LICENSE
--rw-r--r--   0 jorma     (1000) jorma     (1000)    12342 2024-04-30 10:39:02.811510 mama-0.9.4/PKG-INFO
--rw-r--r--   0 jorma     (1000) jorma     (1000)    11351 2024-03-25 09:35:15.000000 mama-0.9.4/README.md
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-04-30 10:39:02.801510 mama-0.9.4/mama/
--rw-r--r--   0 jorma     (1000) jorma     (1000)      141 2024-01-20 16:30:57.000000 mama-0.9.4/mama/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    11805 2024-03-25 09:35:15.000000 mama-0.9.4/mama/artifactory.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    40005 2024-04-30 10:22:46.000000 mama-0.9.4/mama/build_config.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    24912 2024-03-25 09:35:15.000000 mama-0.9.4/mama/build_dependency.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    55207 2024-04-07 19:34:43.000000 mama-0.9.4/mama/build_target.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    11779 2024-04-07 19:34:43.000000 mama-0.9.4/mama/cmake_configure.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    16670 2024-04-30 10:10:25.000000 mama-0.9.4/mama/dependency_chain.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     5368 2024-01-20 16:30:57.000000 mama-0.9.4/mama/init_project.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    12378 2024-03-25 09:35:15.000000 mama-0.9.4/mama/main.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1796 2024-01-20 16:30:57.000000 mama-0.9.4/mama/msbuild.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     9665 2024-04-30 10:23:16.000000 mama-0.9.4/mama/package.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     7757 2024-03-25 09:35:15.000000 mama-0.9.4/mama/papa_deploy.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     3778 2024-03-25 09:35:15.000000 mama-0.9.4/mama/papa_upload.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1763 2024-03-25 09:35:15.000000 mama-0.9.4/mama/parse_mamafile.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-04-30 10:39:02.811510 mama-0.9.4/mama/platforms/
--rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2024-01-20 16:30:57.000000 mama-0.9.4/mama/platforms/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     8558 2024-01-20 16:30:57.000000 mama-0.9.4/mama/platforms/android.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     5376 2024-01-20 16:30:57.000000 mama-0.9.4/mama/platforms/mips.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     5644 2024-03-25 09:35:15.000000 mama-0.9.4/mama/platforms/oclea.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-04-30 10:39:02.811510 mama-0.9.4/mama/types/
--rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2024-01-20 16:30:57.000000 mama-0.9.4/mama/types/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1051 2024-01-20 16:30:57.000000 mama-0.9.4/mama/types/artifactory_pkg.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)      789 2024-01-20 16:30:57.000000 mama-0.9.4/mama/types/asset.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)      830 2024-01-20 16:30:57.000000 mama-0.9.4/mama/types/dep_source.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    15161 2024-04-07 19:34:43.000000 mama-0.9.4/mama/types/git.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1065 2024-01-20 16:30:57.000000 mama-0.9.4/mama/types/local_source.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    17510 2024-03-25 09:35:15.000000 mama-0.9.4/mama/util.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-04-30 10:39:02.811510 mama-0.9.4/mama/utils/
--rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2024-01-20 16:30:57.000000 mama-0.9.4/mama/utils/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1637 2024-01-20 16:30:57.000000 mama-0.9.4/mama/utils/gdb.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    17034 2024-03-25 09:35:15.000000 mama-0.9.4/mama/utils/gnu_project.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)      923 2024-01-20 16:30:57.000000 mama-0.9.4/mama/utils/gtest.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1038 2024-01-20 16:30:57.000000 mama-0.9.4/mama/utils/nonblocking_io.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     3789 2024-04-30 09:51:39.000000 mama-0.9.4/mama/utils/run.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    10345 2024-04-07 19:34:43.000000 mama-0.9.4/mama/utils/sub_process.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1245 2024-04-30 10:15:36.000000 mama-0.9.4/mama/utils/system.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-04-30 10:39:02.811510 mama-0.9.4/mama.egg-info/
--rw-r--r--   0 jorma     (1000) jorma     (1000)    12342 2024-04-30 10:39:02.000000 mama-0.9.4/mama.egg-info/PKG-INFO
--rw-r--r--   0 jorma     (1000) jorma     (1000)      921 2024-04-30 10:39:02.000000 mama-0.9.4/mama.egg-info/SOURCES.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)        1 2024-04-30 10:39:02.000000 mama-0.9.4/mama.egg-info/dependency_links.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)       40 2024-04-30 10:39:02.000000 mama-0.9.4/mama.egg-info/entry_points.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)       76 2024-04-30 10:39:02.000000 mama-0.9.4/mama.egg-info/requires.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)        5 2024-04-30 10:39:02.000000 mama-0.9.4/mama.egg-info/top_level.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1180 2024-04-30 10:38:41.000000 mama-0.9.4/pyproject.toml
--rw-r--r--   0 jorma     (1000) jorma     (1000)       38 2024-04-30 10:39:02.811510 mama-0.9.4/setup.cfg
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-01 11:07:00.778757 mama-0.9.5/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1062 2022-10-15 13:42:02.000000 mama-0.9.5/LICENSE
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12342 2024-05-01 11:07:00.778757 mama-0.9.5/PKG-INFO
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    11351 2024-02-02 11:55:24.000000 mama-0.9.5/README.md
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-01 11:07:00.778757 mama-0.9.5/mama/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      141 2022-10-15 12:52:32.000000 mama-0.9.5/mama/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    11805 2024-03-24 12:54:08.000000 mama-0.9.5/mama/artifactory.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    40005 2024-05-01 11:06:08.000000 mama-0.9.5/mama/build_config.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    24912 2024-03-24 13:57:15.000000 mama-0.9.5/mama/build_dependency.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    55602 2024-05-01 11:06:10.000000 mama-0.9.5/mama/build_target.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    11779 2024-03-26 11:44:52.000000 mama-0.9.5/mama/cmake_configure.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    16670 2024-05-01 11:06:08.000000 mama-0.9.5/mama/dependency_chain.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     5368 2022-10-14 21:28:27.000000 mama-0.9.5/mama/init_project.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12378 2024-02-20 10:18:01.000000 mama-0.9.5/mama/main.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1796 2022-10-14 21:35:20.000000 mama-0.9.5/mama/msbuild.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     9665 2024-05-01 11:06:08.000000 mama-0.9.5/mama/package.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     7757 2024-03-24 13:37:47.000000 mama-0.9.5/mama/papa_deploy.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     3778 2024-03-24 22:17:15.000000 mama-0.9.5/mama/papa_upload.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1763 2024-03-24 13:50:55.000000 mama-0.9.5/mama/parse_mamafile.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-01 11:07:00.778757 mama-0.9.5/mama/platforms/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2023-02-10 12:13:25.000000 mama-0.9.5/mama/platforms/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     8558 2023-08-24 17:06:29.000000 mama-0.9.5/mama/platforms/android.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     5376 2023-10-05 15:21:24.000000 mama-0.9.5/mama/platforms/mips.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     5644 2024-01-24 19:36:51.000000 mama-0.9.5/mama/platforms/oclea.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-01 11:07:00.778757 mama-0.9.5/mama/types/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2022-10-14 22:47:55.000000 mama-0.9.5/mama/types/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1051 2023-01-31 19:23:36.000000 mama-0.9.5/mama/types/artifactory_pkg.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      789 2024-03-24 13:38:20.000000 mama-0.9.5/mama/types/asset.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      830 2023-01-31 19:23:36.000000 mama-0.9.5/mama/types/dep_source.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    15161 2024-04-01 21:45:25.000000 mama-0.9.5/mama/types/git.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1065 2022-10-13 16:33:15.000000 mama-0.9.5/mama/types/local_source.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    17510 2024-03-24 21:19:55.000000 mama-0.9.5/mama/util.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-01 11:07:00.778757 mama-0.9.5/mama/utils/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2022-10-14 22:47:54.000000 mama-0.9.5/mama/utils/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1637 2023-10-14 09:10:27.000000 mama-0.9.5/mama/utils/gdb.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    17034 2024-03-24 13:15:53.000000 mama-0.9.5/mama/utils/gnu_project.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      923 2023-10-14 09:10:17.000000 mama-0.9.5/mama/utils/gtest.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1038 2022-10-14 18:37:11.000000 mama-0.9.5/mama/utils/nonblocking_io.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     3789 2024-05-01 11:06:08.000000 mama-0.9.5/mama/utils/run.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    10345 2024-03-26 12:29:05.000000 mama-0.9.5/mama/utils/sub_process.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1245 2024-05-01 11:06:08.000000 mama-0.9.5/mama/utils/system.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2024-05-01 11:07:00.778757 mama-0.9.5/mama.egg-info/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12342 2024-05-01 11:07:00.000000 mama-0.9.5/mama.egg-info/PKG-INFO
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      921 2024-05-01 11:07:00.000000 mama-0.9.5/mama.egg-info/SOURCES.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        1 2024-05-01 11:07:00.000000 mama-0.9.5/mama.egg-info/dependency_links.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)       40 2024-05-01 11:07:00.000000 mama-0.9.5/mama.egg-info/entry_points.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)       76 2024-05-01 11:07:00.000000 mama-0.9.5/mama.egg-info/requires.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        5 2024-05-01 11:07:00.000000 mama-0.9.5/mama.egg-info/top_level.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1180 2024-05-01 11:06:15.000000 mama-0.9.5/pyproject.toml
+-rw-r--r--   0 jorma     (1000) jorma     (1000)       38 2024-05-01 11:07:00.778757 mama-0.9.5/setup.cfg
```

### Comparing `mama-0.9.4/LICENSE` & `mama-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/PKG-INFO` & `mama-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mama
-Version: 0.9.4
+Version: 0.9.5
 Summary: A modular C++ build tool even your mama can use
 Author-email: Jorma Rebane <jorma.rebane@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/RedFox20/Mama
 Project-URL: Bug Tracker, https://github.com/RedFox20/Mama/issues
 Keywords: mama,build,mamabuild,c,c++,tool,cmake,simple,easy,package,manager,cross-platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mama-0.9.4/README.md` & `mama-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama/artifactory.py` & `mama-0.9.5/mama/artifactory.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama/build_config.py` & `mama-0.9.5/mama/build_config.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama/build_dependency.py` & `mama-0.9.5/mama/build_dependency.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama/build_target.py` & `mama-0.9.5/mama/build_target.py`

 * *Files 1% similar despite different names*

```diff
@@ -686,14 +686,26 @@
         ```
         """
         for option in options:
             if isinstance(option, list): self.cmake_opts += option
             else:                        self.cmake_opts.append(option)
 
 
+    def enable_from_env(self, name, enabled='ON', force=False):
+        """
+        Adds a CMake option if the environment variable `name` is set.
+        ```
+            self.enable_from_env('BUILD_TESTS')
+        ```
+        """
+        env = os.getenv(name)
+        if force or (env and (env == '1' or env == 'ON' or env == 'TRUE')):
+            self.add_cmake_options(f'{name}={enabled}')
+
+
     def add_platform_options(self, windows=None, linux=None, macos=None, ios=None, android=None):
         """
         Selectively applies CMake options depending on configuration platform.
         ```
             self.add_platform_options(windows='ZLIB_STATIC=TRUE')
         ```
         """
```

### Comparing `mama-0.9.4/mama/cmake_configure.py` & `mama-0.9.5/mama/cmake_configure.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama/dependency_chain.py` & `mama-0.9.5/mama/dependency_chain.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama/init_project.py` & `mama-0.9.5/mama/init_project.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama/main.py` & `mama-0.9.5/mama/main.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama/msbuild.py` & `mama-0.9.5/mama/msbuild.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama/package.py` & `mama-0.9.5/mama/package.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama/papa_deploy.py` & `mama-0.9.5/mama/papa_deploy.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama/papa_upload.py` & `mama-0.9.5/mama/papa_upload.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama/parse_mamafile.py` & `mama-0.9.5/mama/parse_mamafile.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama/platforms/android.py` & `mama-0.9.5/mama/platforms/android.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama/platforms/mips.py` & `mama-0.9.5/mama/platforms/mips.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama/platforms/oclea.py` & `mama-0.9.5/mama/platforms/oclea.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama/types/artifactory_pkg.py` & `mama-0.9.5/mama/types/artifactory_pkg.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama/types/asset.py` & `mama-0.9.5/mama/types/asset.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama/types/dep_source.py` & `mama-0.9.5/mama/types/dep_source.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama/types/git.py` & `mama-0.9.5/mama/types/git.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama/types/local_source.py` & `mama-0.9.5/mama/types/local_source.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama/util.py` & `mama-0.9.5/mama/util.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama/utils/gdb.py` & `mama-0.9.5/mama/utils/gdb.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama/utils/gnu_project.py` & `mama-0.9.5/mama/utils/gnu_project.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama/utils/gtest.py` & `mama-0.9.5/mama/utils/gtest.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama/utils/nonblocking_io.py` & `mama-0.9.5/mama/utils/nonblocking_io.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama/utils/run.py` & `mama-0.9.5/mama/utils/run.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama/utils/sub_process.py` & `mama-0.9.5/mama/utils/sub_process.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama/utils/system.py` & `mama-0.9.5/mama/utils/system.py`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/mama.egg-info/PKG-INFO` & `mama-0.9.5/mama.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mama
-Version: 0.9.4
+Version: 0.9.5
 Summary: A modular C++ build tool even your mama can use
 Author-email: Jorma Rebane <jorma.rebane@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/RedFox20/Mama
 Project-URL: Bug Tracker, https://github.com/RedFox20/Mama/issues
 Keywords: mama,build,mamabuild,c,c++,tool,cmake,simple,easy,package,manager,cross-platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mama-0.9.4/mama.egg-info/SOURCES.txt` & `mama-0.9.5/mama.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mama-0.9.4/pyproject.toml` & `mama-0.9.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mama"
-version = "0.9.4"
+version = "0.9.5"
 description = "A modular C++ build tool even your mama can use"
 license = { text = "MIT" }
 authors = [
     { name="Jorma Rebane", email="jorma.rebane@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.6"
```


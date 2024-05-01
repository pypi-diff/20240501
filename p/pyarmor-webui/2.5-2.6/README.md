# Comparing `tmp/pyarmor-webui-2.5.zip` & `tmp/pyarmor-webui-2.6.zip`

## zipinfo {}

```diff
@@ -1,58 +1,58 @@
-Zip file size: 362802 bytes, number of entries: 56
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-22 19:33 pyarmor-webui-2.5/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-22 19:33 pyarmor-webui-2.5/pyarmor_webui.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-22 19:33 pyarmor-webui-2.5/test/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-22 19:33 pyarmor-webui-2.5/static/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-22 19:33 pyarmor-webui-2.5/data/
--rw-r--r--  2.0 unx     6498 b- defN 24-Apr-22 19:33 pyarmor-webui-2.5/PKG-INFO
--rw-r--r--  2.0 unx     9109 b- defN 24-Apr-22 10:19 pyarmor-webui-2.5/server.py
--rw-r--r--  2.0 unx    19099 b- defN 24-Apr-19 15:49 pyarmor-webui-2.5/handler.py
--rw-r--r--  2.0 unx     1068 b- defN 19-Dec-31 08:11 pyarmor-webui-2.5/LICENSE
--rwxr-xr-x  2.0 unx        0 b- defN 20-Mar-27 08:49 pyarmor-webui-2.5/__init__.py
--rw-r--r--  2.0 unx    18042 b- defN 24-Apr-22 15:12 pyarmor-webui-2.5/handler8.py
--rw-r--r--  2.0 unx     2241 b- defN 24-Apr-22 10:22 pyarmor-webui-2.5/setup.py
--rw-r--r--  2.0 unx       59 b- defN 24-Apr-22 19:33 pyarmor-webui-2.5/setup.cfg
--rw-r--r--  2.0 unx     4198 b- defN 24-Apr-22 10:20 pyarmor-webui-2.5/README.rst
--rw-r--r--  2.0 unx     6498 b- defN 24-Apr-22 19:33 pyarmor-webui-2.5/pyarmor_webui.egg-info/PKG-INFO
--rw-r--r--  2.0 unx     1323 b- defN 24-Apr-22 19:33 pyarmor-webui-2.5/pyarmor_webui.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       61 b- defN 24-Apr-22 19:33 pyarmor-webui-2.5/pyarmor_webui.egg-info/entry_points.txt
--rw-r--r--  2.0 unx       15 b- defN 24-Apr-22 19:33 pyarmor-webui-2.5/pyarmor_webui.egg-info/requires.txt
--rw-r--r--  2.0 unx        8 b- defN 24-Apr-22 19:33 pyarmor-webui-2.5/pyarmor_webui.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-22 19:33 pyarmor-webui-2.5/pyarmor_webui.egg-info/dependency_links.txt
--rwxr-xr-x  2.0 unx     1086 b- defN 24-Apr-22 15:01 pyarmor-webui-2.5/test/pack_one_folder_bundle.robot
--rwxr-xr-x  2.0 unx      693 b- defN 20-Oct-30 08:30 pyarmor-webui-2.5/test/generate_expired_license.robot
--rwxr-xr-x  2.0 unx     1476 b- defN 24-Apr-22 15:21 pyarmor-webui-2.5/test/pack_one_file_bundle_with_outer_license.robot
--rwxr-xr-x  2.0 unx     1245 b- defN 20-Jan-19 10:10 pyarmor-webui-2.5/test/obfuscate_multiple_entries.robot
--rwxr-xr-x  2.0 unx      890 b- defN 20-Apr-27 09:40 pyarmor-webui-2.5/test/generate_machine_license.robot
--rwxr-xr-x  2.0 unx     1164 b- defN 20-Jan-19 10:08 pyarmor-webui-2.5/test/obfuscate_one_script.robot
--rw-r--r--  2.0 unx     1899 b- defN 20-Apr-27 09:25 pyarmor-webui-2.5/test/README.md
--rwxr-xr-x  2.0 unx      850 b- defN 24-Apr-22 14:37 pyarmor-webui-2.5/test/generate_extra_data_license.robot
--rwxr-xr-x  2.0 unx     1230 b- defN 20-Jan-19 10:30 pyarmor-webui-2.5/test/obfuscate_one_package.robot
--rwxr-xr-x  2.0 unx     6422 b- defN 23-May-12 10:17 pyarmor-webui-2.5/test/resource.robot
--rwxr-xr-x  2.0 unx     1358 b- defN 20-Apr-27 09:39 pyarmor-webui-2.5/test/pack_with_data_file.robot
--rwxr-xr-x  2.0 unx     1194 b- defN 24-Apr-22 14:51 pyarmor-webui-2.5/test/pack_one_file_bundle.robot
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-22 19:33 pyarmor-webui-2.5/static/css/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-22 19:33 pyarmor-webui-2.5/static/js/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-22 19:33 pyarmor-webui-2.5/static/img/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-22 19:33 pyarmor-webui-2.5/static/fonts/
--rw-r--r--  2.0 unx     4286 b- defN 24-Apr-19 19:05 pyarmor-webui-2.5/static/favicon.ico
--rw-r--r--  2.0 unx      898 b- defN 24-Apr-19 19:05 pyarmor-webui-2.5/static/index.html
--rw-r--r--  2.0 unx    19211 b- defN 24-Apr-19 19:05 pyarmor-webui-2.5/static/reqwest.js
--rw-r--r--  2.0 unx   191299 b- defN 24-Apr-19 19:05 pyarmor-webui-2.5/static/css/chunk-vendors.b79ff3a2.css
--rw-r--r--  2.0 unx     1166 b- defN 24-Apr-19 19:05 pyarmor-webui-2.5/static/css/app.85ddf991.css
--rw-r--r--  2.0 unx   127774 b- defN 24-Apr-19 19:05 pyarmor-webui-2.5/static/js/app.19b525d6.js
--rw-r--r--  2.0 unx   718117 b- defN 24-Apr-19 19:05 pyarmor-webui-2.5/static/js/chunk-vendors.4afc1da0.js
--rw-r--r--  2.0 unx      890 b- defN 24-Apr-19 19:05 pyarmor-webui-2.5/static/img/cog.svg
--rw-r--r--  2.0 unx      207 b- defN 24-Apr-19 19:05 pyarmor-webui-2.5/static/img/folder-solid.svg
--rw-r--r--  2.0 unx      356 b- defN 24-Apr-19 19:05 pyarmor-webui-2.5/static/img/tablet-alt.svg
--rw-r--r--  2.0 unx      339 b- defN 24-Apr-19 19:05 pyarmor-webui-2.5/static/img/shield-alt.svg
--rw-r--r--  2.0 unx      935 b- defN 24-Apr-19 19:05 pyarmor-webui-2.5/static/img/calendar-alt.svg
--rw-r--r--  2.0 unx    14781 b- defN 24-Apr-19 19:05 pyarmor-webui-2.5/static/img/logo.a8954ff0.png
--rw-r--r--  2.0 unx      734 b- defN 24-Apr-19 19:05 pyarmor-webui-2.5/static/img/registered.svg
--rw-r--r--  2.0 unx      446 b- defN 24-Apr-19 19:05 pyarmor-webui-2.5/static/img/calendar-minus.svg
--rw-r--r--  2.0 unx      349 b- defN 24-Apr-19 19:05 pyarmor-webui-2.5/static/img/calendar.svg
--rw-r--r--  2.0 unx      307 b- defN 24-Apr-19 19:05 pyarmor-webui-2.5/static/img/folder.svg
--rw-r--r--  2.0 unx    28200 b- defN 24-Apr-19 19:05 pyarmor-webui-2.5/static/fonts/element-icons.535877f5.woff
--rw-r--r--  2.0 unx    55956 b- defN 24-Apr-19 19:05 pyarmor-webui-2.5/static/fonts/element-icons.732389de.ttf
--rw-r--r--  2.0 unx      218 b- defN 24-Apr-22 15:43 pyarmor-webui-2.5/data/copy_license.py
-56 files, 1254196 bytes uncompressed, 353920 bytes compressed:  71.8%
+Zip file size: 362664 bytes, number of entries: 56
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 07:41 pyarmor-webui-2.6/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 07:41 pyarmor-webui-2.6/pyarmor_webui.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 07:41 pyarmor-webui-2.6/test/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 07:41 pyarmor-webui-2.6/static/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 07:41 pyarmor-webui-2.6/data/
+-rw-r--r--  2.0 unx     5077 b- defN 24-Apr-24 07:41 pyarmor-webui-2.6/PKG-INFO
+-rw-r--r--  2.0 unx     9109 b- defN 24-Apr-24 07:16 pyarmor-webui-2.6/server.py
+-rw-r--r--  2.0 unx    19099 b- defN 24-Apr-19 15:49 pyarmor-webui-2.6/handler.py
+-rw-r--r--  2.0 unx     1068 b- defN 19-Dec-31 08:11 pyarmor-webui-2.6/LICENSE
+-rwxr-xr-x  2.0 unx        0 b- defN 20-Mar-27 08:49 pyarmor-webui-2.6/__init__.py
+-rw-r--r--  2.0 unx    18039 b- defN 24-Apr-24 07:15 pyarmor-webui-2.6/handler8.py
+-rw-r--r--  2.0 unx     2241 b- defN 24-Apr-24 07:16 pyarmor-webui-2.6/setup.py
+-rw-r--r--  2.0 unx       38 b- defN 24-Apr-24 07:41 pyarmor-webui-2.6/setup.cfg
+-rw-r--r--  2.0 unx     4238 b- defN 24-Apr-24 07:17 pyarmor-webui-2.6/README.rst
+-rw-r--r--  2.0 unx     5077 b- defN 24-Apr-24 07:41 pyarmor-webui-2.6/pyarmor_webui.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx     1331 b- defN 24-Apr-24 07:41 pyarmor-webui-2.6/pyarmor_webui.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       61 b- defN 24-Apr-24 07:41 pyarmor-webui-2.6/pyarmor_webui.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx       15 b- defN 24-Apr-24 07:41 pyarmor-webui-2.6/pyarmor_webui.egg-info/requires.txt
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-24 07:41 pyarmor-webui-2.6/pyarmor_webui.egg-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-24 07:41 pyarmor-webui-2.6/pyarmor_webui.egg-info/dependency_links.txt
+-rwxr-xr-x  2.0 unx     1086 b- defN 24-Apr-22 15:01 pyarmor-webui-2.6/test/pack_one_folder_bundle.robot
+-rwxr-xr-x  2.0 unx      693 b- defN 20-Oct-30 08:30 pyarmor-webui-2.6/test/generate_expired_license.robot
+-rwxr-xr-x  2.0 unx     1476 b- defN 24-Apr-22 15:21 pyarmor-webui-2.6/test/pack_one_file_bundle_with_outer_license.robot
+-rwxr-xr-x  2.0 unx     1245 b- defN 20-Jan-19 10:10 pyarmor-webui-2.6/test/obfuscate_multiple_entries.robot
+-rwxr-xr-x  2.0 unx      890 b- defN 20-Apr-27 09:40 pyarmor-webui-2.6/test/generate_machine_license.robot
+-rwxr-xr-x  2.0 unx     1164 b- defN 20-Jan-19 10:08 pyarmor-webui-2.6/test/obfuscate_one_script.robot
+-rw-r--r--  2.0 unx     1899 b- defN 20-Apr-27 09:25 pyarmor-webui-2.6/test/README.md
+-rwxr-xr-x  2.0 unx      850 b- defN 24-Apr-22 14:37 pyarmor-webui-2.6/test/generate_extra_data_license.robot
+-rwxr-xr-x  2.0 unx     1230 b- defN 20-Jan-19 10:30 pyarmor-webui-2.6/test/obfuscate_one_package.robot
+-rwxr-xr-x  2.0 unx     6422 b- defN 23-May-12 10:17 pyarmor-webui-2.6/test/resource.robot
+-rwxr-xr-x  2.0 unx     1358 b- defN 20-Apr-27 09:39 pyarmor-webui-2.6/test/pack_with_data_file.robot
+-rwxr-xr-x  2.0 unx     1194 b- defN 24-Apr-22 14:51 pyarmor-webui-2.6/test/pack_one_file_bundle.robot
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 07:41 pyarmor-webui-2.6/static/css/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 07:41 pyarmor-webui-2.6/static/js/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 07:41 pyarmor-webui-2.6/static/img/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 07:41 pyarmor-webui-2.6/static/fonts/
+-rw-r--r--  2.0 unx     4286 b- defN 24-Apr-19 19:05 pyarmor-webui-2.6/static/favicon.ico
+-rw-r--r--  2.0 unx      898 b- defN 24-Apr-19 19:05 pyarmor-webui-2.6/static/index.html
+-rw-r--r--  2.0 unx    19211 b- defN 24-Apr-19 19:05 pyarmor-webui-2.6/static/reqwest.js
+-rw-r--r--  2.0 unx   191299 b- defN 24-Apr-19 19:05 pyarmor-webui-2.6/static/css/chunk-vendors.b79ff3a2.css
+-rw-r--r--  2.0 unx     1166 b- defN 24-Apr-19 19:05 pyarmor-webui-2.6/static/css/app.85ddf991.css
+-rw-r--r--  2.0 unx   127774 b- defN 24-Apr-19 19:05 pyarmor-webui-2.6/static/js/app.19b525d6.js
+-rw-r--r--  2.0 unx   718117 b- defN 24-Apr-19 19:05 pyarmor-webui-2.6/static/js/chunk-vendors.4afc1da0.js
+-rw-r--r--  2.0 unx      890 b- defN 24-Apr-19 19:05 pyarmor-webui-2.6/static/img/cog.svg
+-rw-r--r--  2.0 unx      207 b- defN 24-Apr-19 19:05 pyarmor-webui-2.6/static/img/folder-solid.svg
+-rw-r--r--  2.0 unx      356 b- defN 24-Apr-19 19:05 pyarmor-webui-2.6/static/img/tablet-alt.svg
+-rw-r--r--  2.0 unx      339 b- defN 24-Apr-19 19:05 pyarmor-webui-2.6/static/img/shield-alt.svg
+-rw-r--r--  2.0 unx      935 b- defN 24-Apr-19 19:05 pyarmor-webui-2.6/static/img/calendar-alt.svg
+-rw-r--r--  2.0 unx    14781 b- defN 24-Apr-19 19:05 pyarmor-webui-2.6/static/img/logo.a8954ff0.png
+-rw-r--r--  2.0 unx      734 b- defN 24-Apr-19 19:05 pyarmor-webui-2.6/static/img/registered.svg
+-rw-r--r--  2.0 unx      446 b- defN 24-Apr-19 19:05 pyarmor-webui-2.6/static/img/calendar-minus.svg
+-rw-r--r--  2.0 unx      349 b- defN 24-Apr-19 19:05 pyarmor-webui-2.6/static/img/calendar.svg
+-rw-r--r--  2.0 unx      307 b- defN 24-Apr-19 19:05 pyarmor-webui-2.6/static/img/folder.svg
+-rw-r--r--  2.0 unx    28200 b- defN 24-Apr-19 19:05 pyarmor-webui-2.6/static/fonts/element-icons.535877f5.woff
+-rw-r--r--  2.0 unx    55956 b- defN 24-Apr-19 19:05 pyarmor-webui-2.6/static/fonts/element-icons.732389de.ttf
+-rw-r--r--  2.0 unx      218 b- defN 24-Apr-22 15:43 pyarmor-webui-2.6/data/copy_license.py
+56 files, 1251378 bytes uncompressed, 353782 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -1,169 +1,169 @@
-Filename: pyarmor-webui-2.5/
+Filename: pyarmor-webui-2.6/
 Comment: 
 
-Filename: pyarmor-webui-2.5/pyarmor_webui.egg-info/
+Filename: pyarmor-webui-2.6/pyarmor_webui.egg-info/
 Comment: 
 
-Filename: pyarmor-webui-2.5/test/
+Filename: pyarmor-webui-2.6/test/
 Comment: 
 
-Filename: pyarmor-webui-2.5/static/
+Filename: pyarmor-webui-2.6/static/
 Comment: 
 
-Filename: pyarmor-webui-2.5/data/
+Filename: pyarmor-webui-2.6/data/
 Comment: 
 
-Filename: pyarmor-webui-2.5/PKG-INFO
+Filename: pyarmor-webui-2.6/PKG-INFO
 Comment: 
 
-Filename: pyarmor-webui-2.5/server.py
+Filename: pyarmor-webui-2.6/server.py
 Comment: 
 
-Filename: pyarmor-webui-2.5/handler.py
+Filename: pyarmor-webui-2.6/handler.py
 Comment: 
 
-Filename: pyarmor-webui-2.5/LICENSE
+Filename: pyarmor-webui-2.6/LICENSE
 Comment: 
 
-Filename: pyarmor-webui-2.5/__init__.py
+Filename: pyarmor-webui-2.6/__init__.py
 Comment: 
 
-Filename: pyarmor-webui-2.5/handler8.py
+Filename: pyarmor-webui-2.6/handler8.py
 Comment: 
 
-Filename: pyarmor-webui-2.5/setup.py
+Filename: pyarmor-webui-2.6/setup.py
 Comment: 
 
-Filename: pyarmor-webui-2.5/setup.cfg
+Filename: pyarmor-webui-2.6/setup.cfg
 Comment: 
 
-Filename: pyarmor-webui-2.5/README.rst
+Filename: pyarmor-webui-2.6/README.rst
 Comment: 
 
-Filename: pyarmor-webui-2.5/pyarmor_webui.egg-info/PKG-INFO
+Filename: pyarmor-webui-2.6/pyarmor_webui.egg-info/PKG-INFO
 Comment: 
 
-Filename: pyarmor-webui-2.5/pyarmor_webui.egg-info/SOURCES.txt
+Filename: pyarmor-webui-2.6/pyarmor_webui.egg-info/SOURCES.txt
 Comment: 
 
-Filename: pyarmor-webui-2.5/pyarmor_webui.egg-info/entry_points.txt
+Filename: pyarmor-webui-2.6/pyarmor_webui.egg-info/entry_points.txt
 Comment: 
 
-Filename: pyarmor-webui-2.5/pyarmor_webui.egg-info/requires.txt
+Filename: pyarmor-webui-2.6/pyarmor_webui.egg-info/requires.txt
 Comment: 
 
-Filename: pyarmor-webui-2.5/pyarmor_webui.egg-info/top_level.txt
+Filename: pyarmor-webui-2.6/pyarmor_webui.egg-info/top_level.txt
 Comment: 
 
-Filename: pyarmor-webui-2.5/pyarmor_webui.egg-info/dependency_links.txt
+Filename: pyarmor-webui-2.6/pyarmor_webui.egg-info/dependency_links.txt
 Comment: 
 
-Filename: pyarmor-webui-2.5/test/pack_one_folder_bundle.robot
+Filename: pyarmor-webui-2.6/test/pack_one_folder_bundle.robot
 Comment: 
 
-Filename: pyarmor-webui-2.5/test/generate_expired_license.robot
+Filename: pyarmor-webui-2.6/test/generate_expired_license.robot
 Comment: 
 
-Filename: pyarmor-webui-2.5/test/pack_one_file_bundle_with_outer_license.robot
+Filename: pyarmor-webui-2.6/test/pack_one_file_bundle_with_outer_license.robot
 Comment: 
 
-Filename: pyarmor-webui-2.5/test/obfuscate_multiple_entries.robot
+Filename: pyarmor-webui-2.6/test/obfuscate_multiple_entries.robot
 Comment: 
 
-Filename: pyarmor-webui-2.5/test/generate_machine_license.robot
+Filename: pyarmor-webui-2.6/test/generate_machine_license.robot
 Comment: 
 
-Filename: pyarmor-webui-2.5/test/obfuscate_one_script.robot
+Filename: pyarmor-webui-2.6/test/obfuscate_one_script.robot
 Comment: 
 
-Filename: pyarmor-webui-2.5/test/README.md
+Filename: pyarmor-webui-2.6/test/README.md
 Comment: 
 
-Filename: pyarmor-webui-2.5/test/generate_extra_data_license.robot
+Filename: pyarmor-webui-2.6/test/generate_extra_data_license.robot
 Comment: 
 
-Filename: pyarmor-webui-2.5/test/obfuscate_one_package.robot
+Filename: pyarmor-webui-2.6/test/obfuscate_one_package.robot
 Comment: 
 
-Filename: pyarmor-webui-2.5/test/resource.robot
+Filename: pyarmor-webui-2.6/test/resource.robot
 Comment: 
 
-Filename: pyarmor-webui-2.5/test/pack_with_data_file.robot
+Filename: pyarmor-webui-2.6/test/pack_with_data_file.robot
 Comment: 
 
-Filename: pyarmor-webui-2.5/test/pack_one_file_bundle.robot
+Filename: pyarmor-webui-2.6/test/pack_one_file_bundle.robot
 Comment: 
 
-Filename: pyarmor-webui-2.5/static/css/
+Filename: pyarmor-webui-2.6/static/css/
 Comment: 
 
-Filename: pyarmor-webui-2.5/static/js/
+Filename: pyarmor-webui-2.6/static/js/
 Comment: 
 
-Filename: pyarmor-webui-2.5/static/img/
+Filename: pyarmor-webui-2.6/static/img/
 Comment: 
 
-Filename: pyarmor-webui-2.5/static/fonts/
+Filename: pyarmor-webui-2.6/static/fonts/
 Comment: 
 
-Filename: pyarmor-webui-2.5/static/favicon.ico
+Filename: pyarmor-webui-2.6/static/favicon.ico
 Comment: 
 
-Filename: pyarmor-webui-2.5/static/index.html
+Filename: pyarmor-webui-2.6/static/index.html
 Comment: 
 
-Filename: pyarmor-webui-2.5/static/reqwest.js
+Filename: pyarmor-webui-2.6/static/reqwest.js
 Comment: 
 
-Filename: pyarmor-webui-2.5/static/css/chunk-vendors.b79ff3a2.css
+Filename: pyarmor-webui-2.6/static/css/chunk-vendors.b79ff3a2.css
 Comment: 
 
-Filename: pyarmor-webui-2.5/static/css/app.85ddf991.css
+Filename: pyarmor-webui-2.6/static/css/app.85ddf991.css
 Comment: 
 
-Filename: pyarmor-webui-2.5/static/js/app.19b525d6.js
+Filename: pyarmor-webui-2.6/static/js/app.19b525d6.js
 Comment: 
 
-Filename: pyarmor-webui-2.5/static/js/chunk-vendors.4afc1da0.js
+Filename: pyarmor-webui-2.6/static/js/chunk-vendors.4afc1da0.js
 Comment: 
 
-Filename: pyarmor-webui-2.5/static/img/cog.svg
+Filename: pyarmor-webui-2.6/static/img/cog.svg
 Comment: 
 
-Filename: pyarmor-webui-2.5/static/img/folder-solid.svg
+Filename: pyarmor-webui-2.6/static/img/folder-solid.svg
 Comment: 
 
-Filename: pyarmor-webui-2.5/static/img/tablet-alt.svg
+Filename: pyarmor-webui-2.6/static/img/tablet-alt.svg
 Comment: 
 
-Filename: pyarmor-webui-2.5/static/img/shield-alt.svg
+Filename: pyarmor-webui-2.6/static/img/shield-alt.svg
 Comment: 
 
-Filename: pyarmor-webui-2.5/static/img/calendar-alt.svg
+Filename: pyarmor-webui-2.6/static/img/calendar-alt.svg
 Comment: 
 
-Filename: pyarmor-webui-2.5/static/img/logo.a8954ff0.png
+Filename: pyarmor-webui-2.6/static/img/logo.a8954ff0.png
 Comment: 
 
-Filename: pyarmor-webui-2.5/static/img/registered.svg
+Filename: pyarmor-webui-2.6/static/img/registered.svg
 Comment: 
 
-Filename: pyarmor-webui-2.5/static/img/calendar-minus.svg
+Filename: pyarmor-webui-2.6/static/img/calendar-minus.svg
 Comment: 
 
-Filename: pyarmor-webui-2.5/static/img/calendar.svg
+Filename: pyarmor-webui-2.6/static/img/calendar.svg
 Comment: 
 
-Filename: pyarmor-webui-2.5/static/img/folder.svg
+Filename: pyarmor-webui-2.6/static/img/folder.svg
 Comment: 
 
-Filename: pyarmor-webui-2.5/static/fonts/element-icons.535877f5.woff
+Filename: pyarmor-webui-2.6/static/fonts/element-icons.535877f5.woff
 Comment: 
 
-Filename: pyarmor-webui-2.5/static/fonts/element-icons.732389de.ttf
+Filename: pyarmor-webui-2.6/static/fonts/element-icons.732389de.ttf
 Comment: 
 
-Filename: pyarmor-webui-2.5/data/copy_license.py
+Filename: pyarmor-webui-2.6/data/copy_license.py
 Comment: 
 
 Zip file comment:
```

## Comparing `pyarmor-webui-2.5/server.py` & `pyarmor-webui-2.6/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     from .handler import RootHandler
     from .handler8 import RootHandler as RootHandler8
 except Exception:
     from .handler import RootHandler
     from .handler8 import RootHandler as RootHandler8
 
 
-__version__ = '2.5'
+__version__ = '2.6'
 
 __config__ = {
     'version': __version__,
     'wwwroot': os.path.join(os.path.dirname(__file__), 'static'),
     'basepath': os.path.dirname(__file__),
     'homepath': os.path.expanduser(os.path.join('~', '.pyarmor')),
 }
```

## Comparing `pyarmor-webui-2.5/handler.py` & `pyarmor-webui-2.6/handler.py`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.5/LICENSE` & `pyarmor-webui-2.6/LICENSE`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.5/handler8.py` & `pyarmor-webui-2.6/handler8.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,15 @@
             if not os.path.isabs(s):
                 s = os.path.join(src, s)
             s = s.replace('\\', '/')
             return ("'%s'" % s) if s.find(' ') > -1 else s
 
         while i < n:
             v = str(result[i])
-            if v in ('--onefile', '-F', '--onefolder', '-D', '--name', '-N',
+            if v in ('--onefile', '-F', '--onedir', '-D', '--name', '-n',
                      '--noconfirm', '-y', '--distpath', '--specpath'):
                 raise RuntimeError('Option "%s" could not be used here' % v)
             if v in ('--add-data', '--add-binary'):
                 i += 1
                 if result[i].find(os.pathsep) == -1:
                     result[i] += os.pathsep + '.'
                 result[i] = _quote_path(result[i])
```

## Comparing `pyarmor-webui-2.5/setup.py` & `pyarmor-webui-2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from sys import platform
 from setuptools import setup
 
-__version__ = '2.5'
+__version__ = '2.6'
 
 with open('README.rst') as f:
     long_description = f.read()
 
 setup(
     name='pyarmor-webui',
     version=__version__,
@@ -59,10 +59,10 @@
 
     entry_points={
         'console_scripts': [
             'pyarmor-webui=pyarmor.webui.server:main',
         ],
     },
 
-    install_requires=['pyarmor>=8.5.4'] + (
+    install_requires=['pyarmor>=8.5.7'] + (
         ['pywin32'] if platform == 'win32' else []),
 )
```

## Comparing `pyarmor-webui-2.5/README.rst` & `pyarmor-webui-2.6/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,18 @@
 - `snapshots <https://github.com/dashingsoft/pyarmor-webui/tree/master/snapshots>`_
 - `pyarmor <https://github.com/dashingsoft/pyarmor>`_
 - `pyarmor-vue <https://github.com/dashingsoft/pyarmor-vue>`_
 
 Change Logs
 -----------
 
+2.6
+~~~~~
+* Fix some pack options bugs
+
 2.5
 ~~~~~
 * Support PyInstaller 6.0+ for pack
 
 2.4
 ~~~~~
 * Fix Windows issue: create new path failed
```

## Comparing `pyarmor-webui-2.5/pyarmor_webui.egg-info/SOURCES.txt` & `pyarmor-webui-2.6/pyarmor_webui.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.rst
 setup.py
 ./LICENSE
 ./README.rst
 ./__init__.py
 ./handler.py
 ./handler8.py
```

## Comparing `pyarmor-webui-2.5/test/pack_one_folder_bundle.robot` & `pyarmor-webui-2.6/test/pack_one_folder_bundle.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.5/test/generate_expired_license.robot` & `pyarmor-webui-2.6/test/generate_expired_license.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.5/test/pack_one_file_bundle_with_outer_license.robot` & `pyarmor-webui-2.6/test/pack_one_file_bundle_with_outer_license.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.5/test/obfuscate_multiple_entries.robot` & `pyarmor-webui-2.6/test/obfuscate_multiple_entries.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.5/test/generate_machine_license.robot` & `pyarmor-webui-2.6/test/generate_machine_license.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.5/test/obfuscate_one_script.robot` & `pyarmor-webui-2.6/test/obfuscate_one_script.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.5/test/README.md` & `pyarmor-webui-2.6/test/README.md`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.5/test/generate_extra_data_license.robot` & `pyarmor-webui-2.6/test/generate_extra_data_license.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.5/test/obfuscate_one_package.robot` & `pyarmor-webui-2.6/test/obfuscate_one_package.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.5/test/resource.robot` & `pyarmor-webui-2.6/test/resource.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.5/test/pack_with_data_file.robot` & `pyarmor-webui-2.6/test/pack_with_data_file.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.5/test/pack_one_file_bundle.robot` & `pyarmor-webui-2.6/test/pack_one_file_bundle.robot`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.5/static/favicon.ico` & `pyarmor-webui-2.6/static/favicon.ico`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.5/static/index.html` & `pyarmor-webui-2.6/static/index.html`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.5/static/reqwest.js` & `pyarmor-webui-2.6/static/reqwest.js`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.5/static/css/chunk-vendors.b79ff3a2.css` & `pyarmor-webui-2.6/static/css/chunk-vendors.b79ff3a2.css`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.5/static/css/app.85ddf991.css` & `pyarmor-webui-2.6/static/css/app.85ddf991.css`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.5/static/js/app.19b525d6.js` & `pyarmor-webui-2.6/static/js/app.19b525d6.js`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.5/static/js/chunk-vendors.4afc1da0.js` & `pyarmor-webui-2.6/static/js/chunk-vendors.4afc1da0.js`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.5/static/img/cog.svg` & `pyarmor-webui-2.6/static/img/cog.svg`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.5/static/img/calendar-alt.svg` & `pyarmor-webui-2.6/static/img/calendar-alt.svg`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.5/static/img/logo.a8954ff0.png` & `pyarmor-webui-2.6/static/img/logo.a8954ff0.png`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.5/static/img/registered.svg` & `pyarmor-webui-2.6/static/img/registered.svg`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.5/static/fonts/element-icons.535877f5.woff` & `pyarmor-webui-2.6/static/fonts/element-icons.535877f5.woff`

 * *Files identical despite different names*

## Comparing `pyarmor-webui-2.5/static/fonts/element-icons.732389de.ttf` & `pyarmor-webui-2.6/static/fonts/element-icons.732389de.ttf`

 * *Files identical despite different names*


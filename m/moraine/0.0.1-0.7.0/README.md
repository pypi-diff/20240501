# Comparing `tmp/moraine-0.0.1.tar.gz` & `tmp/moraine-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moraine-0.0.1.tar", last modified: Sat Oct 21 01:09:00 2023, max compression
+gzip compressed data, was "moraine-0.7.0.tar", last modified: Wed May  1 04:32:58 2024, max compression
```

## Comparing `moraine-0.0.1.tar` & `moraine-0.7.0.tar`

### file list

```diff
@@ -1,20 +1,40 @@
-drwxrwxr-x   0 kangl    (509674) kangl    (509674)        0 2023-10-21 01:09:00.000000 moraine-0.0.1/
--rw-rw-r--   0 kangl    (509674) kangl    (509674)    11337 2023-04-27 10:12:58.000000 moraine-0.0.1/LICENSE
--rw-rw-r--   0 kangl    (509674) kangl    (509674)      111 2023-04-27 10:12:58.000000 moraine-0.0.1/MANIFEST.in
--rw-rw-r--   0 kangl    (509674) kangl    (509674)     1052 2023-10-21 01:09:00.000000 moraine-0.0.1/PKG-INFO
--rw-rw-r--   0 kangl    (509674) kangl    (509674)      284 2023-10-21 01:04:48.000000 moraine-0.0.1/README.md
-drwxrwxr-x   0 kangl    (509674) kangl    (509674)        0 2023-10-21 01:08:59.000000 moraine-0.0.1/moraine/
--rw-rw-r--   0 kangl    (509674) kangl    (509674)       22 2023-10-21 01:04:43.000000 moraine-0.0.1/moraine/__init__.py
--rw-rw-r--   0 kangl    (509674) kangl    (509674)      357 2023-10-21 01:04:43.000000 moraine-0.0.1/moraine/_modidx.py
--rw-rw-r--   0 kangl    (509674) kangl    (509674)      142 2023-10-21 01:04:43.000000 moraine-0.0.1/moraine/core.py
-drwxrwxr-x   0 kangl    (509674) kangl    (509674)        0 2023-10-21 01:08:59.000000 moraine-0.0.1/moraine.egg-info/
--rw-rw-r--   0 kangl    (509674) kangl    (509674)     1052 2023-10-21 01:08:59.000000 moraine-0.0.1/moraine.egg-info/PKG-INFO
--rw-rw-r--   0 kangl    (509674) kangl    (509674)      324 2023-10-21 01:08:59.000000 moraine-0.0.1/moraine.egg-info/SOURCES.txt
--rw-rw-r--   0 kangl    (509674) kangl    (509674)        1 2023-10-21 01:08:59.000000 moraine-0.0.1/moraine.egg-info/dependency_links.txt
--rw-rw-r--   0 kangl    (509674) kangl    (509674)       36 2023-10-21 01:08:59.000000 moraine-0.0.1/moraine.egg-info/entry_points.txt
--rw-rw-r--   0 kangl    (509674) kangl    (509674)        1 2023-10-21 01:08:18.000000 moraine-0.0.1/moraine.egg-info/not-zip-safe
--rw-rw-r--   0 kangl    (509674) kangl    (509674)        7 2023-10-21 01:08:59.000000 moraine-0.0.1/moraine.egg-info/requires.txt
--rw-rw-r--   0 kangl    (509674) kangl    (509674)        8 2023-10-21 01:08:59.000000 moraine-0.0.1/moraine.egg-info/top_level.txt
--rw-rw-r--   0 kangl    (509674) kangl    (509674)      949 2023-10-21 01:04:42.000000 moraine-0.0.1/settings.ini
--rw-rw-r--   0 kangl    (509674) kangl    (509674)       38 2023-10-21 01:09:00.000000 moraine-0.0.1/setup.cfg
--rw-rw-r--   0 kangl    (509674) kangl    (509674)     2596 2023-04-27 10:12:58.000000 moraine-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:32:58.597674 moraine-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    33253 2024-05-01 04:32:06.000000 moraine-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-01 04:32:06.000000 moraine-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-05-01 04:32:58.597674 moraine-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8082 2024-05-01 04:32:06.000000 moraine-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:32:58.597674 moraine-0.7.0/moraine/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-01 04:32:06.000000 moraine-0.7.0/moraine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16416 2024-05-01 04:32:06.000000 moraine-0.7.0/moraine/_modidx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:32:58.597674 moraine-0.7.0/moraine/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-01 04:32:06.000000 moraine-0.7.0/moraine/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7262 2024-05-01 04:32:06.000000 moraine-0.7.0/moraine/cli/co.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-05-01 04:32:06.000000 moraine-0.7.0/moraine/cli/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-01 04:32:06.000000 moraine-0.7.0/moraine/cli/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-01 04:32:06.000000 moraine-0.7.0/moraine/cli/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26890 2024-05-01 04:32:06.000000 moraine-0.7.0/moraine/cli/pc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-05-01 04:32:06.000000 moraine-0.7.0/moraine/cli/pl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22427 2024-05-01 04:32:06.000000 moraine-0.7.0/moraine/cli/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-01 04:32:06.000000 moraine-0.7.0/moraine/cli/ps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-01 04:32:06.000000 moraine-0.7.0/moraine/cli/shp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-01 04:32:06.000000 moraine-0.7.0/moraine/cli/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10033 2024-05-01 04:32:06.000000 moraine-0.7.0/moraine/co.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-01 04:32:06.000000 moraine-0.7.0/moraine/coord_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11793 2024-05-01 04:32:06.000000 moraine-0.7.0/moraine/pc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-01 04:32:06.000000 moraine-0.7.0/moraine/pl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-05-01 04:32:06.000000 moraine-0.7.0/moraine/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-01 04:32:06.000000 moraine-0.7.0/moraine/ps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13999 2024-05-01 04:32:06.000000 moraine-0.7.0/moraine/rtree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-01 04:32:06.000000 moraine-0.7.0/moraine/shp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-01 04:32:06.000000 moraine-0.7.0/moraine/utils_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 04:32:58.597674 moraine-0.7.0/moraine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-05-01 04:32:58.000000 moraine-0.7.0/moraine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-01 04:32:58.000000 moraine-0.7.0/moraine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 04:32:58.000000 moraine-0.7.0/moraine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-01 04:32:58.000000 moraine-0.7.0/moraine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 04:32:56.000000 moraine-0.7.0/moraine.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-01 04:32:58.000000 moraine-0.7.0/moraine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 04:32:58.000000 moraine-0.7.0/moraine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-01 04:32:07.000000 moraine-0.7.0/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 04:32:58.597674 moraine-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-01 04:32:07.000000 moraine-0.7.0/setup.py
```

### Comparing `moraine-0.0.1/setup.py` & `moraine-0.7.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from pkg_resources import parse_version
 from configparser import ConfigParser
-import setuptools, shlex
+import setuptools
 assert parse_version(setuptools.__version__)>=parse_version('36.2')
 
 # note: all settings are in settings.ini; edit there, not here
 config = ConfigParser(delimiters=['='])
-config.read('settings.ini', encoding='utf-8')
+config.read('settings.ini')
 cfg = config['DEFAULT']
 
 cfg_keys = 'version description keywords author author_email'.split()
 expected = cfg_keys + "lib_name user branch license status min_python audience language".split()
 for o in expected: assert o in cfg, "missing expected setting: {}".format(o)
 setup_cfg = {o:cfg[o] for o in cfg_keys}
 
 licenses = {
     'apache2': ('Apache Software License 2.0','OSI Approved :: Apache Software License'),
     'mit': ('MIT License', 'OSI Approved :: MIT License'),
     'gpl2': ('GNU General Public License v2', 'OSI Approved :: GNU General Public License v2 (GPLv2)'),
-    'gpl3': ('GNU General Public License v3', 'OSI Approved :: GNU General Public License v3 (GPLv3)'),
+    'gpl3': ('GNU General Public License v3.0 only', 'OSI Approved :: GNU General Public License v3 (GPLv3)'),
     'bsd3': ('BSD License', 'OSI Approved :: BSD License'),
 }
 statuses = [ '1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
     '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
 py_versions = '3.6 3.7 3.8 3.9 3.10'.split()
 
-requirements = shlex.split(cfg.get('requirements', ''))
-if cfg.get('pip_requirements'): requirements += shlex.split(cfg.get('pip_requirements', ''))
+requirements = cfg.get('requirements','').split()
+if cfg.get('pip_requirements'): requirements += cfg.get('pip_requirements','').split()
 min_python = cfg['min_python']
 lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
 dev_requirements = (cfg.get('dev_requirements') or '').split()
 
 setuptools.setup(
     name = cfg['lib_name'],
     license = lic[0],
@@ -41,15 +41,15 @@
     url = cfg['git_url'],
     packages = setuptools.find_packages(),
     include_package_data = True,
     install_requires = requirements,
     extras_require={ 'dev': dev_requirements },
     dependency_links = cfg.get('dep_links','').split(),
     python_requires  = '>=' + cfg['min_python'],
-    long_description = open('README.md', encoding='utf-8').read(),
+    long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     zip_safe = False,
     entry_points = {
         'console_scripts': cfg.get('console_scripts','').split(),
         'nbdev': [f'{cfg.get("lib_path")}={cfg.get("lib_path")}._modidx:d']
     },
     **setup_cfg)
```


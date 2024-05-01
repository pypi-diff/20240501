# Comparing `tmp/skillsnetwork_authoring_extension-0.6.6rc1.tar.gz` & `tmp/skillsnetwork-authoring-extension-0.7.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skillsnetwork_authoring_extension-0.6.6rc1.tar", last modified: Wed May  1 18:40:57 2024, max compression
+gzip compressed data, was "skillsnetwork-authoring-extension-0.7.0rc0.tar", last modified: Wed Mar 27 01:21:59 2024, max compression
```

## Comparing `skillsnetwork_authoring_extension-0.6.6rc1.tar` & `skillsnetwork-authoring-extension-0.7.0rc0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:40:57.336169 skillsnetwork_authoring_extension-0.6.6rc1/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 18:39:53.000000 skillsnetwork_authoring_extension-0.6.6rc1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 18:39:53.000000 skillsnetwork_authoring_extension-0.6.6rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-01 18:39:53.000000 skillsnetwork_authoring_extension-0.6.6rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-05-01 18:40:57.336169 skillsnetwork_authoring_extension-0.6.6rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-01 18:39:53.000000 skillsnetwork_authoring_extension-0.6.6rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-01 18:39:53.000000 skillsnetwork_authoring_extension-0.6.6rc1/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-01 18:39:53.000000 skillsnetwork_authoring_extension-0.6.6rc1/install.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:40:57.328169 skillsnetwork_authoring_extension-0.6.6rc1/jupyter-config/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:40:57.332169 skillsnetwork_authoring_extension-0.6.6rc1/jupyter-config/nb-config/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-01 18:39:53.000000 skillsnetwork_authoring_extension-0.6.6rc1/jupyter-config/nb-config/skillsnetwork_authoring_extension.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:40:57.332169 skillsnetwork_authoring_extension-0.6.6rc1/jupyter-config/server-config/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-01 18:39:53.000000 skillsnetwork_authoring_extension-0.6.6rc1/jupyter-config/server-config/skillsnetwork_authoring_extension.json
--rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-05-01 18:39:55.000000 skillsnetwork_authoring_extension-0.6.6rc1/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-01 18:39:53.000000 skillsnetwork_authoring_extension-0.6.6rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 18:40:57.336169 skillsnetwork_authoring_extension-0.6.6rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-05-01 18:39:53.000000 skillsnetwork_authoring_extension-0.6.6rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:40:57.332169 skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork-authoring-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-01 18:39:53.000000 skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork-authoring-extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-01 18:39:53.000000 skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork-authoring-extension/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-01 18:39:53.000000 skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork-authoring-extension/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:40:57.332169 skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork-authoring-extension/labextension/
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-05-01 18:40:57.000000 skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork-authoring-extension/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:40:57.332169 skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork-authoring-extension/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (127)    19777 2024-05-01 18:40:57.000000 skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork-authoring-extension/labextension/static/505.e4551d8523c0fb8d36d4.js
--rw-r--r--   0 runner    (1001) docker     (127)    15750 2024-05-01 18:40:57.000000 skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork-authoring-extension/labextension/static/509.152a0e252b536935854a.js
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-01 18:40:57.000000 skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork-authoring-extension/labextension/static/728.17aa88ce4e40d4de8f04.js
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-01 18:40:57.000000 skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork-authoring-extension/labextension/static/765.0109e566eb5dbbda5866.js
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-01 18:40:57.000000 skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork-authoring-extension/labextension/static/894.044de1667e70e686bf5d.js
--rw-r--r--   0 runner    (1001) docker     (127)     8656 2024-05-01 18:40:57.000000 skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork-authoring-extension/labextension/static/remoteEntry.0d0e3d0a04bfed37ab40.js
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-01 18:40:55.000000 skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork-authoring-extension/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-01 18:40:57.000000 skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:40:57.336169 skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork_authoring_extension.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-05-01 18:40:57.000000 skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork_authoring_extension.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-01 18:40:57.000000 skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork_authoring_extension.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:40:57.000000 skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork_authoring_extension.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:40:14.000000 skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork_authoring_extension.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 18:40:57.000000 skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork_authoring_extension.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-01 18:40:57.000000 skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork_authoring_extension.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:40:57.336169 skillsnetwork_authoring_extension-0.6.6rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:40:57.336169 skillsnetwork_authoring_extension-0.6.6rc1/src/button/
--rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-05-01 18:39:53.000000 skillsnetwork_authoring_extension-0.6.6rc1/src/button/index.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-01 18:39:53.000000 skillsnetwork_authoring_extension-0.6.6rc1/src/button/sample.json
--rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-05-01 18:39:53.000000 skillsnetwork_authoring_extension-0.6.6rc1/src/config.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-01 18:39:53.000000 skillsnetwork_authoring_extension-0.6.6rc1/src/dialog.ts
--rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-05-01 18:39:53.000000 skillsnetwork_authoring_extension-0.6.6rc1/src/handler.ts
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-01 18:39:53.000000 skillsnetwork_authoring_extension-0.6.6rc1/src/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:40:57.336169 skillsnetwork_authoring_extension-0.6.6rc1/src/menu/
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-01 18:39:53.000000 skillsnetwork_authoring_extension-0.6.6rc1/src/menu/index.ts
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-01 18:39:53.000000 skillsnetwork_authoring_extension-0.6.6rc1/src/sn-file-library.ts
--rw-r--r--   0 runner    (1001) docker     (127)    16577 2024-05-01 18:39:53.000000 skillsnetwork_authoring_extension-0.6.6rc1/src/tools.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:40:57.336169 skillsnetwork_authoring_extension-0.6.6rc1/style/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-01 18:39:53.000000 skillsnetwork_authoring_extension-0.6.6rc1/style/base.css
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-01 18:39:53.000000 skillsnetwork_authoring_extension-0.6.6rc1/style/index.css
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-01 18:39:53.000000 skillsnetwork_authoring_extension-0.6.6rc1/style/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-01 18:39:53.000000 skillsnetwork_authoring_extension-0.6.6rc1/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)   229847 2024-05-01 18:40:44.000000 skillsnetwork_authoring_extension-0.6.6rc1/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:21:59.861663 skillsnetwork-authoring-extension-0.7.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-27 01:20:53.000000 skillsnetwork-authoring-extension-0.7.0rc0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-27 01:20:53.000000 skillsnetwork-authoring-extension-0.7.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-27 01:20:53.000000 skillsnetwork-authoring-extension-0.7.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-03-27 01:21:59.861663 skillsnetwork-authoring-extension-0.7.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-03-27 01:20:53.000000 skillsnetwork-authoring-extension-0.7.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-03-27 01:20:53.000000 skillsnetwork-authoring-extension-0.7.0rc0/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-27 01:20:53.000000 skillsnetwork-authoring-extension-0.7.0rc0/install.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:21:59.853663 skillsnetwork-authoring-extension-0.7.0rc0/jupyter-config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:21:59.857663 skillsnetwork-authoring-extension-0.7.0rc0/jupyter-config/nb-config/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-27 01:20:53.000000 skillsnetwork-authoring-extension-0.7.0rc0/jupyter-config/nb-config/skillsnetwork_authoring_extension.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:21:59.857663 skillsnetwork-authoring-extension-0.7.0rc0/jupyter-config/server-config/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-27 01:20:53.000000 skillsnetwork-authoring-extension-0.7.0rc0/jupyter-config/server-config/skillsnetwork_authoring_extension.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-03-27 01:20:55.000000 skillsnetwork-authoring-extension-0.7.0rc0/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-27 01:20:53.000000 skillsnetwork-authoring-extension-0.7.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 01:21:59.861663 skillsnetwork-authoring-extension-0.7.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-03-27 01:20:53.000000 skillsnetwork-authoring-extension-0.7.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:21:59.857663 skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork-authoring-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-03-27 01:20:53.000000 skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork-authoring-extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-27 01:20:53.000000 skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork-authoring-extension/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-27 01:20:53.000000 skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork-authoring-extension/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:21:59.857663 skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork-authoring-extension/labextension/
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-03-27 01:21:59.000000 skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork-authoring-extension/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:21:59.857663 skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork-authoring-extension/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    19777 2024-03-27 01:21:59.000000 skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork-authoring-extension/labextension/static/505.e4551d8523c0fb8d36d4.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16295 2024-03-27 01:21:59.000000 skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork-authoring-extension/labextension/static/509.434f2efdf9ae2f28d497.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-03-27 01:21:59.000000 skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork-authoring-extension/labextension/static/728.17aa88ce4e40d4de8f04.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-03-27 01:21:59.000000 skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork-authoring-extension/labextension/static/765.0109e566eb5dbbda5866.js
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-27 01:21:59.000000 skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork-authoring-extension/labextension/static/894.044de1667e70e686bf5d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8656 2024-03-27 01:21:59.000000 skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork-authoring-extension/labextension/static/remoteEntry.4b06ce2af7b9cb16edfa.js
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-27 01:21:57.000000 skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork-authoring-extension/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-03-27 01:21:59.000000 skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:21:59.861663 skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork_authoring_extension.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-03-27 01:21:59.000000 skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork_authoring_extension.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-03-27 01:21:59.000000 skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork_authoring_extension.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 01:21:59.000000 skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork_authoring_extension.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 01:21:17.000000 skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork_authoring_extension.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-27 01:21:59.000000 skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork_authoring_extension.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-27 01:21:59.000000 skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork_authoring_extension.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:21:59.861663 skillsnetwork-authoring-extension-0.7.0rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:21:59.861663 skillsnetwork-authoring-extension-0.7.0rc0/src/button/
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-03-27 01:20:53.000000 skillsnetwork-authoring-extension-0.7.0rc0/src/button/index.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-03-27 01:20:53.000000 skillsnetwork-authoring-extension-0.7.0rc0/src/button/sample.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-03-27 01:20:53.000000 skillsnetwork-authoring-extension-0.7.0rc0/src/config.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-03-27 01:20:53.000000 skillsnetwork-authoring-extension-0.7.0rc0/src/dialog.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-03-27 01:20:53.000000 skillsnetwork-authoring-extension-0.7.0rc0/src/handler.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-27 01:20:53.000000 skillsnetwork-authoring-extension-0.7.0rc0/src/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:21:59.861663 skillsnetwork-authoring-extension-0.7.0rc0/src/menu/
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-03-27 01:20:53.000000 skillsnetwork-authoring-extension-0.7.0rc0/src/menu/index.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-03-27 01:20:53.000000 skillsnetwork-authoring-extension-0.7.0rc0/src/sn-file-library.ts
+-rw-r--r--   0 runner    (1001) docker     (127)    16631 2024-03-27 01:20:53.000000 skillsnetwork-authoring-extension-0.7.0rc0/src/tools.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 01:21:59.861663 skillsnetwork-authoring-extension-0.7.0rc0/style/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-27 01:20:53.000000 skillsnetwork-authoring-extension-0.7.0rc0/style/base.css
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-27 01:20:53.000000 skillsnetwork-authoring-extension-0.7.0rc0/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-27 01:20:53.000000 skillsnetwork-authoring-extension-0.7.0rc0/style/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-27 01:20:53.000000 skillsnetwork-authoring-extension-0.7.0rc0/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)   229896 2024-03-27 01:21:46.000000 skillsnetwork-authoring-extension-0.7.0rc0/yarn.lock
```

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/LICENSE` & `skillsnetwork-authoring-extension-0.7.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/PKG-INFO` & `skillsnetwork-authoring-extension-0.7.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: skillsnetwork-authoring-extension
-Version: 0.6.6rc1
+Version: 0.7.0rc0
 Summary: JupyterLab/JupyterLite extension for Skills Network Authoring
 Home-page: https://github.com/ibm-skills-network/skillsnetwork-authoring-extension
-Author: IBM Skills Network
-Author-email: skills.network@ibm.com
+Author: Jenny Cao
+Author-email: jenny.cao@ibm.com
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
 Platform: Windows
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
@@ -48,15 +48,15 @@
 ```bash
 pip install skillsnetwork-authoring-extension
 ```
 
 After installing, enable the extension:
 
 ```bash
-jupyter server extension enable skillsnetwork-authoring-extension
+jupyter serverextension enable skillsnetwork-authoring-extension
 ```
 
 ### Launch JupyterLab
 
 To launch Jupyter Lab visit [http://localhost:8888/](http://localhost:8888/)
 
 ### Uninstall
@@ -84,32 +84,36 @@
 pip install jupyterlab==<version>
 ```
 
 ### Development install
 
 Note: You will need NodeJS to build the extension package.
 
+The `jlpm` command is JupyterLab's pinned version of
+[yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
+`yarn` or `npm` in lieu of `jlpm` below.
+
 ```bash
 # Clone the repo to your local environment
 # Change directory to the skillsnetwork-authoring-extension directory
 # Install package in development mode
 pip install -e .
 # Install jupyter-packaging
 pip install jupyter-packaging
 # Link your development version of the extension with JupyterLab
 jupyter labextension develop . --overwrite
 # Rebuild extension Typescript source after making changes
-npm run build
+jlpm build
 ```
 
 You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.
 
 ```bash
 # Watch the source directory in one terminal, automatically rebuilding when needed
-npm run watch
+jlpm watch
 # Run JupyterLab in another terminal
 jupyter lab
 ```
 
 With the watch command running, every saved change will immediately be built locally and available in your running JupyterLab. Refresh JupyterLab to load the change in your browser (you may need to wait several seconds for the extension to be rebuilt).
 
 By default, the `jlpm build` command generates the source maps for this extension to make it easier to debug using the browser dev tools. To also generate source maps for the JupyterLab core extensions, you can run the following command:
```

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/README.md` & `skillsnetwork-authoring-extension-0.7.0rc0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ```bash
 pip install skillsnetwork-authoring-extension
 ```
 
 After installing, enable the extension:
 
 ```bash
-jupyter server extension enable skillsnetwork-authoring-extension
+jupyter serverextension enable skillsnetwork-authoring-extension
 ```
 
 ### Launch JupyterLab
 
 To launch Jupyter Lab visit [http://localhost:8888/](http://localhost:8888/)
 
 ### Uninstall
@@ -55,32 +55,36 @@
 pip install jupyterlab==<version>
 ```
 
 ### Development install
 
 Note: You will need NodeJS to build the extension package.
 
+The `jlpm` command is JupyterLab's pinned version of
+[yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
+`yarn` or `npm` in lieu of `jlpm` below.
+
 ```bash
 # Clone the repo to your local environment
 # Change directory to the skillsnetwork-authoring-extension directory
 # Install package in development mode
 pip install -e .
 # Install jupyter-packaging
 pip install jupyter-packaging
 # Link your development version of the extension with JupyterLab
 jupyter labextension develop . --overwrite
 # Rebuild extension Typescript source after making changes
-npm run build
+jlpm build
 ```
 
 You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.
 
 ```bash
 # Watch the source directory in one terminal, automatically rebuilding when needed
-npm run watch
+jlpm watch
 # Run JupyterLab in another terminal
 jupyter lab
 ```
 
 With the watch command running, every saved change will immediately be built locally and available in your running JupyterLab. Refresh JupyterLab to load the change in your browser (you may need to wait several seconds for the extension to be rebuilt).
 
 By default, the `jlpm build` command generates the source maps for this extension to make it easier to debug using the browser dev tools. To also generate source maps for the JupyterLab core extensions, you can run the following command:
```

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/RELEASE.md` & `skillsnetwork-authoring-extension-0.7.0rc0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/package.json` & `skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork-authoring-extension/labextension/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9602272727272727%*

 * *Differences: {"'author'": "{'name': 'Jenny Cao', 'email': 'jenny.cao@ibm.com'}",*

 * * "'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.4b06ce2af7b9cb16edfa.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}",*

 * * "'version'": "'0.7.0-rc0'"}*

```diff
@@ -1,11 +1,11 @@
 {
     "author": {
-        "email": "skills.network@ibm.com",
-        "name": "IBM Skills Network"
+        "email": "jenny.cao@ibm.com",
+        "name": "Jenny Cao"
     },
     "bugs": {
         "url": "https://github.com/ibm-skills-network/skillsnetwork-authoring-extension/issues"
     },
     "dependencies": {
         "@jupyterlab/application": "^3.3.0",
         "@jupyterlab/apputils": "^3.3.0",
@@ -55,14 +55,19 @@
             ],
             "before-build-python": [
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.4b06ce2af7b9cb16edfa.js",
+            "style": "./style"
+        },
         "extension": true,
         "outputDir": "skillsnetwork-authoring-extension/labextension",
         "webpackConfig": "./webpack.config.js"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -109,9 +114,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.6.6-rc1"
+    "version": "0.7.0-rc0"
 }
```

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/pyproject.toml` & `skillsnetwork-authoring-extension-0.7.0rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/setup.py` & `skillsnetwork-authoring-extension-0.7.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork-authoring-extension/__init__.py` & `skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork-authoring-extension/__init__.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork-authoring-extension/_version.py` & `skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork-authoring-extension/_version.py`

 * *Files identical despite different names*

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork-authoring-extension/handlers.py` & `skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork-authoring-extension/handlers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,31 @@
+import json
+import os
+
 import tornado
-from jupyter_server.base.handlers import APIHandler
-from jupyter_server.utils import url_path_join
+from notebook.base.handlers import IPythonHandler
+from notebook.utils import url_path_join
+
+from urllib.parse import urlencode, unquote
 
-class AppHandler(APIHandler):
-  """Thin wrapper around the APIHandler handler which injects common properties."""
+class AppHandler(IPythonHandler):
+  """Thin wrapper around the IPython handler which injects common properties."""
   @property
   def config(self):
       return self.settings["sn_config"]
 
 class ConfigurationEndpointHandler(AppHandler):
   """
   Route handler for the /skillsnetwork-authoring-extension/config endpoint.
 
-  A single endpoint that returns various configuration values to the frontend.
+  A single endpoint that returns the Atlas base URL.
   """
-  @tornado.web.authenticated
   def get(self) -> None:
-    self.finish({
-      "ATLAS_BASE_URL": self.config.atlas_base_url,
-      "SN_FILE_LIBRARY_URL": self.config.sn_file_library_url,
-      "AWB_BASE_URL": self.config.awb_base_url
-    })
+    print('test', type(self.config))
+    self.finish({"ATLAS_BASE_URL": self.config.atlas_base_url, "SN_FILE_LIBRARY_URL": self.config.sn_file_library_url, "AWB_BASE_URL": self.config.awb_base_url})
 
 
 def setup_handlers(web_app, url_path: str) -> None:
   """Setup handlers in the jupyter server web app.
 
   Args:
     - web_app: Jupyter server web application instance to add handlers to.
```

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork-authoring-extension/labextension/package.json` & `skillsnetwork-authoring-extension-0.7.0rc0/package.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9602272727272727%*

 * *Differences: {"'author'": "{'name': 'Jenny Cao', 'email': 'jenny.cao@ibm.com'}",*

 * * "'jupyterlab'": "{delete: ['_build']}",*

 * * "'version'": "'0.7.0-rc0'"}*

```diff
@@ -1,11 +1,11 @@
 {
     "author": {
-        "email": "skills.network@ibm.com",
-        "name": "IBM Skills Network"
+        "email": "jenny.cao@ibm.com",
+        "name": "Jenny Cao"
     },
     "bugs": {
         "url": "https://github.com/ibm-skills-network/skillsnetwork-authoring-extension/issues"
     },
     "dependencies": {
         "@jupyterlab/application": "^3.3.0",
         "@jupyterlab/apputils": "^3.3.0",
@@ -55,19 +55,14 @@
             ],
             "before-build-python": [
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.0d0e3d0a04bfed37ab40.js",
-            "style": "./style"
-        },
         "extension": true,
         "outputDir": "skillsnetwork-authoring-extension/labextension",
         "webpackConfig": "./webpack.config.js"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -114,9 +109,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.6.6-rc1"
+    "version": "0.7.0-rc0"
 }
```

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork-authoring-extension/labextension/static/505.e4551d8523c0fb8d36d4.js` & `skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork-authoring-extension/labextension/static/505.e4551d8523c0fb8d36d4.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork-authoring-extension/labextension/static/509.152a0e252b536935854a.js` & `skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork-authoring-extension/labextension/static/509.434f2efdf9ae2f28d497.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -13,25 +13,25 @@
                         l = o(1290),
                         s = o(8474),
                         c = o(4089),
                         u = o(5729),
                         d = o(7887),
                         h = o(9677),
                         p = o.n(h),
-                        b = o(7271),
-                        w = o(8225),
-                        y = t([d, c, s]);
-                    [d, c, s] = y.then ? (await y)() : y;
+                        w = o(7271),
+                        b = o(8225),
+                        y = t([d, c, s, b]);
+                    [d, c, s, b] = y.then ? (await y)() : y;
                     const g = {
                         activate: k,
                         id: "skillsnetwork-authoring-extension:plugin",
                         autoStart: !0,
-                        requires: [l.IMainMenu, b.INotebookTracker, a.IDocumentManager]
+                        requires: [l.IMainMenu, w.INotebookTracker, a.IDocumentManager]
                     };
-                    class m {
+                    class f {
                         createNew(t, e) {
                             if (d.RV.SHOW_PUBLISH_BUTTON_FOR !== e.path) return new r.DisposableDelegate((() => {}));
                             {
                                 const o = async () => {
                                     const o = e.path.split("/").pop() || "",
                                         n = d.RV.TOKENS.get(o);
                                     if (void 0 === n) return console.log("No atlas or awb token found for id", t.id), void await (0, i.showDialog)({
@@ -59,35 +59,35 @@
                                     className: "publish-lab-button",
                                     label: "Publish on SN",
                                     onClick: o,
                                     tooltip: "Publish Lab"
                                 }), u = new i.ToolbarButton({
                                     className: "sn-file-library-button",
                                     label: "SN File Library",
-                                    onClick: () => (new w.C).launch(),
+                                    onClick: () => new b.C(e.path).launch(),
                                     tooltip: "Skills Network File Library"
                                 });
                                 return t.toolbar.insertItem(8, "download", a), t.toolbar.insertItem(9, "sn-file-library", u), t.toolbar.insertItem(10, "publish", l), new r.DisposableDelegate((() => {
                                     a.dispose(), l.dispose(), u.dispose()
                                 }))
                             }
                         }
                     }
-                    async function f(t, e) {
+                    async function m(t, e) {
                         e.forEach((t => {
                             t.dispose()
                         }))
                     }
                     async function k(t, e, o, n) {
                         if (console.log("Activating skillsnetwork-authoring-extension button plugin!"), "learn" == await (0, d.g)()) return;
                         const a = await (0, d.oK)(),
                             r = await (0, d.RJ)(),
                             l = await (0, d.By)();
-                        console.log("Using default kernel: ", d.RV.PY_KERNEL_NAME), t.docRegistry.addWidgetExtension("Notebook", new m), await t.serviceManager.ready, t.restored.then((async () => {
-                            if (await f(0, o), "NO_TOKEN" !== a && "local" !== l) try {
+                        console.log("Using default kernel: ", d.RV.PY_KERNEL_NAME), t.docRegistry.addWidgetExtension("Notebook", new f), await t.serviceManager.ready, t.restored.then((async () => {
+                            if (await m(0, o), "NO_TOKEN" !== a && "local" !== l) try {
                                 await (0, s.oh)(a, n, t.serviceManager.contents)
                             } catch (t) {
                                 i.Dialog.flush(), (0, u.ep)(), console.log(t)
                             } else if ("NO_TOKEN" !== r && "local" !== l) try {
                                 await (0, s.qu)(r, n, t.serviceManager.contents)
                             } catch (t) {
                                 i.Dialog.flush(), (0, u.ep)(), console.log(t)
@@ -255,34 +255,34 @@
                     }).then((t => {})).catch((t => {}))
                 }
         },
         4089: (t, e, o) => {
             o.a(t, (async (t, n) => {
                 try {
                     o.d(e, {
-                        $w: () => m,
-                        BD: () => f,
+                        $w: () => f,
+                        BD: () => m,
                         P0: () => y,
                         Xu: () => k,
                         zO: () => g,
-                        zU: () => w
+                        zU: () => b
                     });
                     var a = o(9645),
                         i = o.n(a),
                         r = o(5729),
                         l = o(9604),
                         s = o(7887),
                         c = o(8474),
                         u = o(5674),
                         d = o.n(u),
                         h = o(9677),
                         p = o.n(h),
-                        b = t([s, c]);
-                    [s, c] = b.then ? (await b)() : b;
-                    const w = t => d().create({
+                        w = t([s, c]);
+                    [s, c] = w.then ? (await w)() : w;
+                    const b = t => d().create({
                             baseURL: s.GX,
                             headers: {
                                 Authorization: `Bearer ${t}`,
                                 "Content-Type": "application/json",
                                 "Access-Control-Allow-Origin": "*",
                                 Accept: "application/json"
                             }
@@ -306,15 +306,15 @@
                                 return l.Dialog.flush(), {
                                     labFilename: i,
                                     body: r
                                 }
                             } catch (t) {
                                 throw console.log(t), "Failed to fetch notebook"
                             }
-                        }, m = async (t, e, o, n) => {
+                        }, f = async (t, e, o, n) => {
                             if (!await (0, r.t5)("Publishing your lab onto Skills Network...").then((t => !0)).catch((t => !1))) return;
                             (0, r.ms)("Publishing your changes...");
                             const a = p()(n),
                                 s = a.version_id,
                                 u = a.lab_id;
                             await (0, c.rA)(e, o);
                             const d = await (0, c.FH)(e, o),
@@ -322,15 +322,15 @@
                             return h.append("publish", "true"), h.append("draft[changelog]", "updated notebook"), h.append("file", d), new Promise((async (e, o) => {
                                 await t.post(`api/v1/labs/${u}/lab_versions/${s}/drafts`, h).then((t => {
                                     console.log("SUCCESSFULLY PUSHED", t), l.Dialog.flush(), (0, r.oY)()
                                 })).catch((t => {
                                     console.log(t), l.Dialog.flush(), (0, r.VQ)()
                                 }))
                             }))
-                        }, f = t => t.get("v1/labs").then((t => (l.Dialog.flush(), t.data))).catch((t => {
+                        }, m = t => t.get("v1/labs").then((t => (l.Dialog.flush(), t.data))).catch((t => {
                             throw console.log(t), "Failed to fetch notebook"
                         })), k = async (t, e, o) => {
                             if (!await (0, r.t5)("Publishing your lab onto Skills Network...").then((t => !0)).catch((t => !1))) return;
                             (0, r.ms)("Publishing your changes..."), await (0, c.rA)(e, o);
                             const n = await (0, c.FH)(e, o);
                             return new Promise((async (e, o) => {
                                 await t.post("v1/labs", {
@@ -365,29 +365,29 @@
                 }
             }))
         },
         7809: (t, e, o) => {
             o.a(t, (async (t, n) => {
                 try {
                     o.d(e, {
-                        M: () => w
+                        M: () => b
                     });
                     var a = o(1290),
                         i = o(4112),
                         r = o(9604),
                         l = o(7271),
                         s = o(2615),
                         c = o(5729),
                         u = o(7887),
                         d = o(8474),
                         h = o(9677),
                         p = o.n(h),
-                        b = t([u, d]);
-                    [u, d] = b.then ? (await b)() : b;
-                    const w = {
+                        w = t([u, d]);
+                    [u, d] = w.then ? (await w)() : w;
+                    const b = {
                         id: "skillsnetwork-authoring-extension:menu",
                         autoStart: !0,
                         requires: [a.IMainMenu, l.INotebookTracker, s.IDocumentManager],
                         activate: async (t, e, o, n) => {
                             if (console.log("Activating skillsnetwork-authoring-extension menu plugin!"), "learn" == await (0, u.g)()) return;
                             const a = "edit-lab-from-token";
                             t.commands.addCommand(a, {
@@ -432,57 +432,83 @@
                     n()
                 } catch (g) {
                     n(g)
                 }
             }))
         },
         8225: (t, e, o) => {
-            o.d(e, {
-                C: () => r
-            });
-            var n = o(4112),
-                a = o(9604);
-            class i extends n.Widget {
-                constructor() {
-                    function t(t, e) {
-                        const o = document.createElement("li"),
-                            n = document.createElement("a");
-                        return n.textContent = t, n.style.color = "brown", n.href = e, n.style.textDecoration = "underline", n.style.cursor = "pointer", o.appendChild(n), o
-                    }
-                    const e = document.createElement("div"),
-                        o = document.createElement("h2");
-                    o.textContent = "File Library is not available for JupyterLab Classic.", e.appendChild(o);
-                    const n = document.createElement("p");
-                    n.style.textAlign = "left", n.textContent = "Try opening the File Library from Author Workbench or upgrade your JupyterLab Classic to JupyterLab Current.";
-                    const a = document.createElement("ul");
-                    a.style.textAlign = "left", a.appendChild(t("How to access File Library from Author Workbench", "https://author.skills.network/docs/labs/jupyterlab-filelibrary")), a.appendChild(t("How to upgrade to JupyterLab Current", "https://author.skills.network/docs/labs/upgrade-jupyterlab")), e.appendChild(n), e.appendChild(a), e.style.padding = "20px", e.style.margin = "10px", e.style.textAlign = "center", super({
-                        node: e
-                    })
-                }
-            }
-            class r {
-                launch() {
-                    const t = new a.Dialog({
-                            title: "Skills Network File Library",
-                            body: new i,
-                            hasClose: !0,
-                            buttons: [a.Dialog.cancelButton()]
-                        }),
-                        e = t.node.querySelector(".jp-Dialog-content");
-                    e && e.classList.add("sn-file-library-dialog"), t.launch()
+            o.a(t, (async (t, n) => {
+                try {
+                    o.d(e, {
+                        C: () => h
+                    });
+                    var a = o(4112),
+                        i = o(9604),
+                        r = o(7887),
+                        l = o(9677),
+                        s = o.n(l),
+                        c = t([r]);
+                    r = (c.then ? (await c)() : c)[0];
+                    var u;
+                    class d extends a.Widget {
+                        constructor(t) {
+                            function e(t, e) {
+                                const o = document.createElement("li"),
+                                    n = document.createElement("a");
+                                return n.textContent = t, n.style.color = "brown", n.href = e, n.style.textDecoration = "underline", n.style.cursor = "pointer", o.appendChild(n), o
+                            }
+                            const o = document.createElement("div"),
+                                n = document.createElement("h2");
+                            n.textContent = "File Library is not available for JupyterLab Classic.", o.appendChild(n);
+                            const a = document.createElement("p");
+                            a.style.textAlign = "left", a.textContent = "Try opening the File Library from Author Workbench or upgrade your JupyterLab Classic to JupyterLab Current.";
+                            const i = document.createElement("ul");
+                            i.style.textAlign = "left", i.appendChild(e("How to access File Library from Author Workbench", "https://author.skills.network/docs/labs/jupyterlab-filelibrary")), i.appendChild(e("How to upgrade to JupyterLab Current", "https://author.skills.network/docs/labs/upgrade-jupyterlab")), o.appendChild(a), o.appendChild(i), o.style.padding = "20px", o.style.margin = "10px", o.style.textAlign = "center", super({
+                                node: o
+                            })
+                        }
+                    }
+                    class h {
+                        constructor(t) {
+                            u.set(this, void 0),
+                                function(t, e, o) {
+                                    if (!e.has(t)) throw new TypeError("attempted to set private field on non-instance");
+                                    e.set(t, o)
+                                }(this, u, t)
+                        }
+                        launch() {
+                            const t = r.RV.TOKENS.get(function(t, e) {
+                                    if (!e.has(t)) throw new TypeError("attempted to get private field on non-instance");
+                                    return e.get(t)
+                                }(this, u).split("/").pop() || ""),
+                                e = t ? s()(t) : {},
+                                o = r.p_ + "/labs/" + e.lab_id + "?show=content",
+                                n = new i.Dialog({
+                                    title: "Skills Network File Library",
+                                    body: new d(o),
+                                    hasClose: !0,
+                                    buttons: [i.Dialog.cancelButton()]
+                                }),
+                                a = n.node.querySelector(".jp-Dialog-content");
+                            a && a.classList.add("sn-file-library-dialog"), n.launch()
+                        }
+                    }
+                    u = new WeakMap, n()
+                } catch (t) {
+                    n(t)
                 }
-            }
+            }))
         },
         8474: (t, e, o) => {
             o.a(t, (async (t, n) => {
                 try {
                     o.d(e, {
                         FH: () => u,
                         oh: () => y,
-                        qu: () => w,
+                        qu: () => b,
                         rA: () => d
                     });
                     var a = o(9604),
                         i = o(7887),
                         r = o(4089),
                         l = t([i, r]);
                     [i, r] = l.then ? (await l)() : l;
@@ -514,15 +540,15 @@
                                     metadata: n,
                                     nbformat: a,
                                     nbformat_minor: i
                                 };
                             return JSON.stringify(r, null, 2)
                         };
                     async function d(t, e) {
-                        const o = await b(t, e),
+                        const o = await w(t, e),
                             n = await R(o);
                         await e.ready, e.model.metadata.set(i.RV.PREV_PUB_HASH, n), e.save().then((() => {
                             console.log("Notebook saved with updated metadata.")
                         })).catch((t => {
                             console.error("Failed to save notebook:", t)
                         }))
                     }
@@ -539,47 +565,47 @@
                         } catch (t) {
                             return console.error("Error parsing lab content string: ", t), !1
                         }
                         if ("object" != typeof t || null === t || !("cells" in t) && (!t.content || !("cells" in t.content))) return console.error("Lab content is of unknown type or missing 'cells': ", typeof t, "\n Value: \n", t), !1;
                         const o = t.cells || (null === (e = t.content) || void 0 === e ? void 0 : e.cells);
                         return 0 === o.length || 1 === o.length && 0 === o[0].source.length
                     }
-                    const b = (t, e) => {
+                    const w = (t, e) => {
                             const o = [];
                             return t.content.widgets.forEach((t => {
                                 const e = c(t);
                                 o.push(e)
                             })), JSON.stringify(o, null, 2)
                         },
-                        w = async (t, e, o) => {
+                        b = async (t, e, o) => {
                             let n, {
                                 labFilename: a,
                                 body: l
                             } = await (0, r.zO)((0, r.P0)(t), t);
-                            if (await m(a, o, e), await g(a, l, o, e), i.RV.SHOW_PUBLISH_BUTTON_FOR = a, i.RV.TOKENS.set(a, t), await v(`./${a}`, o)) n = e.openOrReveal(a);
+                            if (a = a.replace(/^.*[\\\/]/, ""), await f(a, o, e), await g(a, l, o, e), i.RV.SHOW_PUBLISH_BUTTON_FOR = a, i.RV.TOKENS.set(a, t), await v(`./${a}`, o)) n = e.openOrReveal(a);
                             else {
                                 if (n = e.createNew(a, "notebook", {
                                         name: i.RV.PY_KERNEL_NAME
                                     }), void 0 === n) throw Error("Error loading lab");
-                                await f(n, l)
+                                await m(n, l)
                             }
                             return n
                         }, y = async (t, e, o) => {
                             let {
                                 instructions_file_path: n,
                                 body: a
                             } = await (0, r.BD)((0, r.zU)(t));
                             const l = k(n);
                             let s;
-                            if (await m(l, o, e), await g(l, a, o, e), i.RV.SHOW_PUBLISH_BUTTON_FOR = l, i.RV.TOKENS.set(l, t), await v(`./${l}`, o)) s = e.openOrReveal(l);
+                            if (await f(l, o, e), await g(l, a, o, e), i.RV.SHOW_PUBLISH_BUTTON_FOR = l, i.RV.TOKENS.set(l, t), await v(`./${l}`, o)) s = e.openOrReveal(l);
                             else {
                                 if (s = e.createNew(l, "notebook", {
                                         name: i.RV.PY_KERNEL_NAME
                                     }), void 0 === s) throw Error("Error loading lab");
-                                await f(s, JSON.parse(a))
+                                await m(s, JSON.parse(a))
                             }
                             return s
                         };
                     async function g(t, e, o, n) {
                         const r = `./${t}`,
                             l = await v(r, o);
                         if (l && h(e) !== h(l)) try {
@@ -596,20 +622,20 @@
                                 body: `While trying to load your lab: "${t}", we found that you have another file named "${t}" that already exists in this folder, please delete it or rename it so we can load your published version"`,
                                 buttons: [a.Dialog.okButton({
                                     label: "Dismiss"
                                 })]
                             })
                         }
                     }
-                    async function m(t, e, o) {
+                    async function f(t, e, o) {
                         const n = `./${t}`,
                             a = await v(n, e);
                         a && (await E(n, o), p(a) && await e.delete(n))
                     }
-                    const f = async (t, e, o) => {
+                    const m = async (t, e, o) => {
                         if (await t.context.ready, "local" !== o)
                             if (t.context && t.context.model) {
                                 t.context.model.fromJSON(e);
                                 try {
                                     await t.context.save()
                                 } catch (t) {
                                     console.error("Error saving notebook:", t)
```

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork-authoring-extension/labextension/static/728.17aa88ce4e40d4de8f04.js` & `skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork-authoring-extension/labextension/static/728.17aa88ce4e40d4de8f04.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork-authoring-extension/labextension/static/765.0109e566eb5dbbda5866.js` & `skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork-authoring-extension/labextension/static/765.0109e566eb5dbbda5866.js`

 * *Files identical despite different names*

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork-authoring-extension/labextension/static/remoteEntry.0d0e3d0a04bfed37ab40.js` & `skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork-authoring-extension/labextension/static/remoteEntry.4b06ce2af7b9cb16edfa.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, s, f, d, p, c, h, v, b, m, g, y, w, k, _, S, x = {
+    var e, r, t, n, o, a, i, u, f, l, s, d, c, p, h, v, b, m, g, y, w, k, _, S, x = {
             8375: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(509).then((() => () => t(8509))),
                         "./extension": () => t.e(509).then((() => () => t(8509))),
                         "./style": () => t.e(728).then((() => () => t(9728)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -37,22 +37,22 @@
         return x[e](t, t.exports, E), t.exports
     }
     E.m = x, E.c = j, e = "function" == typeof Symbol ? Symbol("webpack queues") : "__webpack_queues__", r = "function" == typeof Symbol ? Symbol("webpack exports") : "__webpack_exports__", t = "function" == typeof Symbol ? Symbol("webpack error") : "__webpack_error__", n = e => {
         e && e.d < 1 && (e.d = 1, e.forEach((e => e.r--)), e.forEach((e => e.r-- ? e.r++ : e())))
     }, E.a = (o, a, i) => {
         var u;
         i && ((u = []).d = -1);
-        var l, s, f, d = new Set,
-            p = o.exports,
-            c = new Promise(((e, r) => {
-                f = r, s = e
+        var f, l, s, d = new Set,
+            c = o.exports,
+            p = new Promise(((e, r) => {
+                s = r, l = e
             }));
-        c[r] = p, c[e] = e => (u && e(u), d.forEach(e), c.catch((e => {}))), o.exports = c, a((o => {
+        p[r] = c, p[e] = e => (u && e(u), d.forEach(e), p.catch((e => {}))), o.exports = p, a((o => {
             var a;
-            l = (o => o.map((o => {
+            f = (o => o.map((o => {
                 if (null !== o && "object" == typeof o) {
                     if (o[e]) return o;
                     if (o.then) {
                         var a = [];
                         a.d = 0, o.then((e => {
                             i[r] = e, n(a)
                         }), (e => {
@@ -61,44 +61,44 @@
                         var i = {};
                         return i[e] = e => e(a), i
                     }
                 }
                 var u = {};
                 return u[e] = e => {}, u[r] = o, u
             })))(o);
-            var i = () => l.map((e => {
+            var i = () => f.map((e => {
                     if (e[t]) throw e[t];
                     return e[r]
                 })),
-                s = new Promise((r => {
+                l = new Promise((r => {
                     (a = () => r(i)).r = 0;
                     var t = e => e !== u && !d.has(e) && (d.add(e), e && !e.d && (a.r++, e.push(a)));
-                    l.map((r => r[e](t)))
+                    f.map((r => r[e](t)))
                 }));
-            return a.r ? s : i()
-        }), (e => (e ? f(c[t] = e) : s(p), n(u)))), u && u.d < 0 && (u.d = 0)
+            return a.r ? l : i()
+        }), (e => (e ? s(p[t] = e) : l(c), n(u)))), u && u.d < 0 && (u.d = 0)
     }, E.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
         return E.d(r, {
             a: r
         }), r
     }, E.d = (e, r) => {
         for (var t in r) E.o(r, t) && !E.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, E.f = {}, E.e = e => Promise.all(Object.keys(E.f).reduce(((r, t) => (E.f[t](e, r), r)), [])), E.u = e => e + "." + {
         505: "e4551d8523c0fb8d36d4",
-        509: "152a0e252b536935854a",
+        509: "434f2efdf9ae2f28d497",
         728: "17aa88ce4e40d4de8f04",
         765: "0109e566eb5dbbda5866",
         894: "044de1667e70e686bf5d"
     } [e] + ".js?v=" + {
         505: "e4551d8523c0fb8d36d4",
-        509: "152a0e252b536935854a",
+        509: "434f2efdf9ae2f28d497",
         728: "17aa88ce4e40d4de8f04",
         765: "0109e566eb5dbbda5866",
         894: "044de1667e70e686bf5d"
     } [e], E.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
@@ -106,28 +106,28 @@
             if ("object" == typeof window) return window
         }
     }(), E.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), o = {}, a = "skillsnetwork-authoring-extension:", E.l = (e, r, t, n) => {
         if (o[e]) o[e].push(r);
         else {
             var i, u;
             if (void 0 !== t)
-                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var f = l[s];
-                    if (f.getAttribute("src") == e || f.getAttribute("data-webpack") == a + t) {
-                        i = f;
+                for (var f = document.getElementsByTagName("script"), l = 0; l < f.length; l++) {
+                    var s = f[l];
+                    if (s.getAttribute("src") == e || s.getAttribute("data-webpack") == a + t) {
+                        i = s;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, E.nc && i.setAttribute("nonce", E.nc), i.setAttribute("data-webpack", a + t), i.src = e), o[e] = [r];
             var d = (r, t) => {
-                    i.onerror = i.onload = null, clearTimeout(p);
+                    i.onerror = i.onload = null, clearTimeout(c);
                     var n = o[e];
                     if (delete o[e], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(t))), r) return r(t)
                 },
-                p = setTimeout(d.bind(null, void 0, {
+                c = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, E.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
@@ -152,16 +152,16 @@
                             u = o[r];
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
-                    l = [];
-                return "default" === t && (u("axios", "0.21.4", (() => E.e(505).then((() => () => E(2505))))), u("form-data", "4.0.0", (() => E.e(894).then((() => () => E(1894))))), u("jwt-decode", "3.1.2", (() => E.e(765).then((() => () => E(6765))))), u("skillsnetwork-authoring-extension", "0.6.6-rc1", (() => E.e(509).then((() => () => E(8509)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                    f = [];
+                return "default" === t && (u("axios", "0.21.4", (() => E.e(505).then((() => () => E(2505))))), u("form-data", "4.0.0", (() => E.e(894).then((() => () => E(1894))))), u("jwt-decode", "3.1.2", (() => E.e(765).then((() => () => E(6765))))), u("skillsnetwork-authoring-extension", "0.7.0-rc0", (() => E.e(509).then((() => () => E(8509)))))), e[t] = f.length ? Promise.all(f).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var r = E.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -185,87 +185,87 @@
             if (t >= r.length) return "u" == o;
             var a = r[t],
                 u = (typeof a)[0];
             if (o != u) return "o" == o && "n" == u || "s" == u || "u" == o;
             if ("o" != o && "u" != o && n != a) return n < a;
             t++
         }
-    }, l = e => {
+    }, f = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(i = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, i);
             return t
         }
         var a = [];
         for (o = 1; o < e.length; o++) {
             var i = e[o];
-            a.push(0 === i ? "not(" + u() + ")" : 1 === i ? "(" + u() + " || " + u() + ")" : 2 === i ? a.pop() + " " + a.pop() : l(i))
+            a.push(0 === i ? "not(" + u() + ")" : 1 === i ? "(" + u() + " || " + u() + ")" : 2 === i ? a.pop() + " " + a.pop() : f(i))
         }
         return u();
 
         function u() {
             return a.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, s = (e, r) => {
+    }, l = (e, r) => {
         if (0 in e) {
             r = i(r);
             var t = e[0],
                 n = t < 0;
             n && (t = -t - 1);
             for (var o = 0, a = 1, u = !0;; a++, o++) {
-                var l, f, d = a < e.length ? (typeof e[a])[0] : "";
-                if (o >= r.length || "o" == (f = (typeof(l = r[o]))[0])) return !u || ("u" == d ? a > t && !n : "" == d != n);
-                if ("u" == f) {
+                var f, s, d = a < e.length ? (typeof e[a])[0] : "";
+                if (o >= r.length || "o" == (s = (typeof(f = r[o]))[0])) return !u || ("u" == d ? a > t && !n : "" == d != n);
+                if ("u" == s) {
                     if (!u || "u" != d) return !1
                 } else if (u)
-                    if (d == f)
+                    if (d == s)
                         if (a <= t) {
-                            if (l != e[a]) return !1
+                            if (f != e[a]) return !1
                         } else {
-                            if (n ? l > e[a] : l < e[a]) return !1;
-                            l != e[a] && (u = !1)
+                            if (n ? f > e[a] : f < e[a]) return !1;
+                            f != e[a] && (u = !1)
                         }
                 else if ("s" != d && "n" != d) {
                     if (n || a <= t) return !1;
                     u = !1, a--
                 } else {
-                    if (a <= t || f < d != n) return !1;
+                    if (a <= t || s < d != n) return !1;
                     u = !1
                 } else "s" != d && "n" != d && (u = !1, a--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
+        var c = [],
+            p = c.pop.bind(c);
         for (o = 1; o < e.length; o++) {
             var h = e[o];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? s(h, r) : !c())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? l(h, r) : !p())
         }
-        return !!c()
-    }, f = (e, r) => {
+        return !!p()
+    }, s = (e, r) => {
         var t = E.S[e];
         if (!t || !E.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, d = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && u(e, r) ? r : e), 0)
-    }, p = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + l(n) + ")", c = (e, r, t, n) => {
+    }, c = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + f(n) + ")", p = (e, r, t, n) => {
         var o = d(e, t);
-        return s(n, o) || v(p(e, t, o, n)), b(e[t][o])
+        return l(n, o) || v(c(e, t, o, n)), b(e[t][o])
     }, h = (e, r, t) => {
         var n = e[r];
-        return (r = Object.keys(n).reduce(((e, r) => !s(t, r) || e && !u(e, r) ? e : r), 0)) && n[r]
+        return (r = Object.keys(n).reduce(((e, r) => !l(t, r) || e && !u(e, r) ? e : r), 0)) && n[r]
     }, v = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, b = e => (e.loaded = 1, e.get()), g = (m = e => function(r, t, n, o) {
         var a = E.I(r);
         return a && a.then ? a.then(e.bind(e, r, E.S[r], t, n, o)) : e(r, E.S[r], t, n, o)
-    })(((e, r, t, n) => (f(e, t), c(r, 0, t, n)))), y = m(((e, r, t, n, o) => {
+    })(((e, r, t, n) => (s(e, t), p(r, 0, t, n)))), y = m(((e, r, t, n, o) => {
         var a = r && E.o(r, t) && h(r, t, n);
         return a ? b(a) : o()
     })), w = {}, k = {
         454: () => g("default", "@lumino/disposable", [1, 1, 10, 0]),
         1290: () => g("default", "@jupyterlab/mainmenu", [1, 3, 6, 7]),
         2615: () => g("default", "@jupyterlab/docmanager", [1, 3, 6, 7]),
         4112: () => g("default", "@lumino/widgets", [1, 1, 37, 2]),
@@ -320,20 +320,20 @@
                             i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
                 var n, o, [a, i, u] = t,
-                    l = 0;
+                    f = 0;
                 if (a.some((r => 0 !== e[r]))) {
                     for (n in i) E.o(i, n) && (E.m[n] = i[n]);
                     u && u(E)
                 }
-                for (r && r(t); l < a.length; l++) o = a[l], E.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); f < a.length; f++) o = a[f], E.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkskillsnetwork_authoring_extension = self.webpackChunkskillsnetwork_authoring_extension || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), E.nc = void 0;
     var P = E(8375);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["skillsnetwork-authoring-extension"] = P
 })();
```

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json` & `skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork_authoring_extension.egg-info/PKG-INFO` & `skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork_authoring_extension.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: skillsnetwork-authoring-extension
-Version: 0.6.6rc1
+Version: 0.7.0rc0
 Summary: JupyterLab/JupyterLite extension for Skills Network Authoring
 Home-page: https://github.com/ibm-skills-network/skillsnetwork-authoring-extension
-Author: IBM Skills Network
-Author-email: skills.network@ibm.com
+Author: Jenny Cao
+Author-email: jenny.cao@ibm.com
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
 Platform: Windows
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
@@ -48,15 +48,15 @@
 ```bash
 pip install skillsnetwork-authoring-extension
 ```
 
 After installing, enable the extension:
 
 ```bash
-jupyter server extension enable skillsnetwork-authoring-extension
+jupyter serverextension enable skillsnetwork-authoring-extension
 ```
 
 ### Launch JupyterLab
 
 To launch Jupyter Lab visit [http://localhost:8888/](http://localhost:8888/)
 
 ### Uninstall
@@ -84,32 +84,36 @@
 pip install jupyterlab==<version>
 ```
 
 ### Development install
 
 Note: You will need NodeJS to build the extension package.
 
+The `jlpm` command is JupyterLab's pinned version of
+[yarn](https://yarnpkg.com/) that is installed with JupyterLab. You may use
+`yarn` or `npm` in lieu of `jlpm` below.
+
 ```bash
 # Clone the repo to your local environment
 # Change directory to the skillsnetwork-authoring-extension directory
 # Install package in development mode
 pip install -e .
 # Install jupyter-packaging
 pip install jupyter-packaging
 # Link your development version of the extension with JupyterLab
 jupyter labextension develop . --overwrite
 # Rebuild extension Typescript source after making changes
-npm run build
+jlpm build
 ```
 
 You can watch the source directory and run JupyterLab at the same time in different terminals to watch for changes in the extension's source and automatically rebuild the extension.
 
 ```bash
 # Watch the source directory in one terminal, automatically rebuilding when needed
-npm run watch
+jlpm watch
 # Run JupyterLab in another terminal
 jupyter lab
 ```
 
 With the watch command running, every saved change will immediately be built locally and available in your running JupyterLab. Refresh JupyterLab to load the change in your browser (you may need to wait several seconds for the extension to be rebuilt).
 
 By default, the `jlpm build` command generates the source maps for this extension to make it easier to debug using the browser dev tools. To also generate source maps for the JupyterLab core extensions, you can run the following command:
```

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/skillsnetwork_authoring_extension.egg-info/SOURCES.txt` & `skillsnetwork-authoring-extension-0.7.0rc0/skillsnetwork_authoring_extension.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 jupyter-config/nb-config/skillsnetwork_authoring_extension.json
 jupyter-config/server-config/skillsnetwork_authoring_extension.json
 skillsnetwork-authoring-extension/__init__.py
 skillsnetwork-authoring-extension/_version.py
 skillsnetwork-authoring-extension/handlers.py
 skillsnetwork-authoring-extension/labextension/package.json
 skillsnetwork-authoring-extension/labextension/static/505.e4551d8523c0fb8d36d4.js
-skillsnetwork-authoring-extension/labextension/static/509.152a0e252b536935854a.js
+skillsnetwork-authoring-extension/labextension/static/509.434f2efdf9ae2f28d497.js
 skillsnetwork-authoring-extension/labextension/static/728.17aa88ce4e40d4de8f04.js
 skillsnetwork-authoring-extension/labextension/static/765.0109e566eb5dbbda5866.js
 skillsnetwork-authoring-extension/labextension/static/894.044de1667e70e686bf5d.js
-skillsnetwork-authoring-extension/labextension/static/remoteEntry.0d0e3d0a04bfed37ab40.js
+skillsnetwork-authoring-extension/labextension/static/remoteEntry.4b06ce2af7b9cb16edfa.js
 skillsnetwork-authoring-extension/labextension/static/style.js
 skillsnetwork-authoring-extension/labextension/static/third-party-licenses.json
 skillsnetwork_authoring_extension.egg-info/PKG-INFO
 skillsnetwork_authoring_extension.egg-info/SOURCES.txt
 skillsnetwork_authoring_extension.egg-info/dependency_links.txt
 skillsnetwork_authoring_extension.egg-info/not-zip-safe
 skillsnetwork_authoring_extension.egg-info/requires.txt
```

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/src/button/index.ts` & `skillsnetwork-authoring-extension-0.7.0rc0/src/button/index.ts`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         onClick: start,
         tooltip: 'Publish Lab'
       });
 
       const snFileLibraryButton = new ToolbarButton({
         className: 'sn-file-library-button',
         label: 'SN File Library',
-        onClick: () => new SkillsNetworkFileLibrary().launch(),
+        onClick: () => new SkillsNetworkFileLibrary(context.path).launch(),
         tooltip: 'Skills Network File Library'
       });
 
       panel.toolbar.insertItem(8, 'download', downloadButton);
       panel.toolbar.insertItem(9, 'sn-file-library', snFileLibraryButton);
       panel.toolbar.insertItem(10, 'publish', publishButton);
       return new DisposableDelegate(() => {
```

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/src/button/sample.json` & `skillsnetwork-authoring-extension-0.7.0rc0/src/button/sample.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/src/config.ts` & `skillsnetwork-authoring-extension-0.7.0rc0/src/config.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/src/dialog.ts` & `skillsnetwork-authoring-extension-0.7.0rc0/src/dialog.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/src/handler.ts` & `skillsnetwork-authoring-extension-0.7.0rc0/src/handler.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/src/menu/index.ts` & `skillsnetwork-authoring-extension-0.7.0rc0/src/menu/index.ts`

 * *Files identical despite different names*

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/src/sn-file-library.ts` & `skillsnetwork-authoring-extension-0.7.0rc0/src/sn-file-library.ts`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import { Widget } from '@lumino/widgets';
 import { Dialog } from '@jupyterlab/apputils';
+import { Globals, AWB_BASE_URL } from './config';
+import jwt_decode from 'jwt-decode';
 
 export class SkillsNetworkFileLibraryWidget extends Widget {
 
-  constructor() {
+  constructor(contextPath: string) {
 
     function constructList(content: string, content_url: string) {
       const list = document.createElement('li');
       const link = document.createElement('a');
       link.textContent = content;
       link.style.color = "brown";
       link.href = content_url;
@@ -41,17 +43,28 @@
     container.style.textAlign = "center";
 
     super({ node: container });
   }
 }
 
 export class SkillsNetworkFileLibrary {
+    #contextPath: string;
+
+    constructor(contextPath: string) {
+      this.#contextPath = contextPath;
+    }
+
     launch(){
+      const token = Globals.TOKENS.get(this.#contextPath.split('/').pop() || '');
+      const token_info = token
+      ? (jwt_decode(token) as { [key: string]: any })
+      : {};
+      const lab_content_url = AWB_BASE_URL + "/labs/" + token_info.lab_id + "?show=content";
       const imgLibDialog = new Dialog({title: "Skills Network File Library",
-        body:  new SkillsNetworkFileLibraryWidget(),
+        body:  new SkillsNetworkFileLibraryWidget(lab_content_url),
         hasClose: true,
         buttons: [Dialog.cancelButton()]
       });
       const dialogContent = imgLibDialog.node.querySelector(".jp-Dialog-content")
       if (dialogContent){
         dialogContent.classList.add("sn-file-library-dialog");
       }
```

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/src/tools.ts` & `skillsnetwork-authoring-extension-0.7.0rc0/src/tools.ts`

 * *Files 1% similar despite different names*

```diff
@@ -207,14 +207,15 @@
   return JSON.stringify(allCells, null, 2);
 };
 
 
 
 export const openIndependentLab = async (awb_token: string, docManager: IDocumentManager, contentsManager: ContentsManager): Promise<NotebookPanel> => {
   let {labFilename, body: instructions_content} = await getIndependentLabModel(awbAxiosHandler(awb_token), awb_token);
+  labFilename = labFilename.replace(/^.*[\\\/]/, '');
   await deleteIfEmptyFile(labFilename, contentsManager, docManager)
   await checkAndBackupSaveFile(labFilename, instructions_content, contentsManager, docManager);
 
   // Set the publish button to only show for the lab with title labFilename
   Globals.SHOW_PUBLISH_BUTTON_FOR = labFilename;
   // Set the publish button to only work for the lab with title labFilename
   Globals.TOKENS.set(labFilename, awb_token);
```

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/tsconfig.json` & `skillsnetwork-authoring-extension-0.7.0rc0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `skillsnetwork_authoring_extension-0.6.6rc1/yarn.lock` & `skillsnetwork-authoring-extension-0.7.0rc0/yarn.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # THIS IS AN AUTOGENERATED FILE. DO NOT EDIT THIS FILE DIRECTLY.
 # yarn lockfile v1
 
 
+"@aashutoshrathi/word-wrap@^1.2.3":
+  version "1.2.6"
+  resolved "https://registry.yarnpkg.com/@aashutoshrathi/word-wrap/-/word-wrap-1.2.6.tgz#bd9154aec9983f77b3a034ecaa015c2e4201f6cf"
+  integrity sha512-1Yjs2SvM8TflER/OD3cOjhWWOZb58A2t7wpE2S9XfBYTiIl+XFhQG2bjy4Pu1I+EAlCNUzRDYDdFwFYUKvXcIA==
+
 "@babel/code-frame@7.12.11":
   version "7.12.11"
   resolved "https://registry.yarnpkg.com/@babel/code-frame/-/code-frame-7.12.11.tgz#f4ad435aa263db935b8f10f2c552d23fb716a63f"
   integrity sha512-Zt1yodBx1UcyiePMSkWnU4hPqhwq7hGi2nFL1LeA3EUl+q2LQx16MISgJ0+z7dnmgvP9QtIleuETGOiOH1RcIw==
   dependencies:
     "@babel/highlight" "^7.10.4"
 
@@ -13,33 +18,33 @@
   version "7.24.2"
   resolved "https://registry.yarnpkg.com/@babel/code-frame/-/code-frame-7.24.2.tgz#718b4b19841809a58b29b68cde80bc5e1aa6d9ae"
   integrity sha512-y5+tLQyV8pg3fsiln67BVLD1P13Eg4lh5RW9mF0zUuvLrv9uIQ4MCL+CRT+FTsBlBjcIan6PGsLcBN0m3ClUyQ==
   dependencies:
     "@babel/highlight" "^7.24.2"
     picocolors "^1.0.0"
 
-"@babel/helper-validator-identifier@^7.24.5":
-  version "7.24.5"
-  resolved "https://registry.yarnpkg.com/@babel/helper-validator-identifier/-/helper-validator-identifier-7.24.5.tgz#918b1a7fa23056603506370089bd990d8720db62"
-  integrity sha512-3q93SSKX2TWCG30M2G2kwaKeTYgEUp5Snjuj8qm729SObL6nbtUldAi37qbxkD5gg3xnBio+f9nqpSepGZMvxA==
+"@babel/helper-validator-identifier@^7.22.20":
+  version "7.22.20"
+  resolved "https://registry.yarnpkg.com/@babel/helper-validator-identifier/-/helper-validator-identifier-7.22.20.tgz#c4ae002c61d2879e724581d96665583dbc1dc0e0"
+  integrity sha512-Y4OZ+ytlatR8AI+8KZfKuL5urKp7qey08ha31L8b3BwewJAoJamTzyvxPR/5D+KkdJCGPq/+8TukHBlY10FX9A==
 
 "@babel/highlight@^7.10.4", "@babel/highlight@^7.24.2":
-  version "7.24.5"
-  resolved "https://registry.yarnpkg.com/@babel/highlight/-/highlight-7.24.5.tgz#bc0613f98e1dd0720e99b2a9ee3760194a704b6e"
-  integrity sha512-8lLmua6AVh/8SLJRRVD6V8p73Hir9w5mJrhE+IPpILG31KKlI9iz5zmBYKcWPS59qSfgP9RaSBQSHHE81WKuEw==
+  version "7.24.2"
+  resolved "https://registry.yarnpkg.com/@babel/highlight/-/highlight-7.24.2.tgz#3f539503efc83d3c59080a10e6634306e0370d26"
+  integrity sha512-Yac1ao4flkTxTteCDZLEvdxg2fZfz1v8M4QpaGypq/WPDqg3ijHYbDfs+LG5hvzSoqaSZ9/Z9lKSP3CjZjv+pA==
   dependencies:
-    "@babel/helper-validator-identifier" "^7.24.5"
+    "@babel/helper-validator-identifier" "^7.22.20"
     chalk "^2.4.2"
     js-tokens "^4.0.0"
     picocolors "^1.0.0"
 
 "@babel/runtime@^7.1.2":
-  version "7.24.5"
-  resolved "https://registry.yarnpkg.com/@babel/runtime/-/runtime-7.24.5.tgz#230946857c053a36ccc66e1dd03b17dd0c4ed02c"
-  integrity sha512-Nms86NXrsaeU9vbBJKni6gXiEXZ4CVpYVzEjDH9Sb8vmZ3UljyA1GSOJl/6LGPO8EHLuSF9H+IxNXHPX8QHJ4g==
+  version "7.24.1"
+  resolved "https://registry.yarnpkg.com/@babel/runtime/-/runtime-7.24.1.tgz#431f9a794d173b53720e69a6464abc6f0e2a5c57"
+  integrity sha512-+BIznRzyqBf+2wCTxcKE3wDjfGeCoVE61KSHGpkzqrLi8qxqFwBeUFyId2cxkTmm55fzDGnm0+yCxaxygrLUnQ==
   dependencies:
     regenerator-runtime "^0.14.0"
 
 "@blueprintjs/colors@^4.0.0-alpha.3":
   version "4.2.1"
   resolved "https://registry.yarnpkg.com/@blueprintjs/colors/-/colors-4.2.1.tgz#603b2512caee84feddcb3dbd536534c140b9a1f3"
   integrity sha512-Cx7J2YnUuxn+fi+y5XtXnBB7+cFHN4xBrRkaAetp78i3VTCXjUk+d1omrOr8TqbRucUXTdrhbZOUHpzRLFcJpQ==
@@ -486,17 +491,17 @@
     "@jupyterlab/ui-components" "^3.6.7"
     "@lumino/algorithm" "^1.9.0"
     "@lumino/commands" "^1.19.0"
     "@lumino/coreutils" "^1.11.0"
     "@lumino/widgets" "^1.37.2"
 
 "@jupyterlab/nbformat@^3.0.0 || ^4.0.0-alpha.15":
-  version "4.1.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/nbformat/-/nbformat-4.1.8.tgz#2fb9ef4a6326e9dd9d6d1ea53999a9e9fbac6261"
-  integrity sha512-uwGLaiIEsSox6zZ9WIsHbKaPO4Yovrp9LW6NXSafFhHeNdEaVGJ05C4mZTDAXWGgV+EWEBx5U2PrGmsYiHRLlQ==
+  version "4.1.5"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/nbformat/-/nbformat-4.1.5.tgz#de651b01a0fd0c96eecb5d638a8f701171dd8e84"
+  integrity sha512-N9X3wxeh8BS5+pGIJGd7CyhVJI7l4XybAHnsN3sVJmL6RIlhji/zWzT0L/oAl3490sQdm+P/sLdiTWJqMHVYbg==
   dependencies:
     "@lumino/coreutils" "^2.1.2"
 
 "@jupyterlab/nbformat@^3.3.3", "@jupyterlab/nbformat@^3.6.7":
   version "3.6.7"
   resolved "https://registry.yarnpkg.com/@jupyterlab/nbformat/-/nbformat-3.6.7.tgz#8810dd403daffca5a4910a9eecc1ef29f70ff957"
   integrity sha512-CR7Lcgcnh+kYt4pLcxXne7en6zyp5Pl81VP1xT88UssA6e0HS7wtXvaA398On+2Xw7DXogh+5jU9dKM+HtxU2Q==
@@ -561,17 +566,17 @@
     "@lumino/messaging" "^1.10.0"
     "@lumino/properties" "^1.8.0"
     "@lumino/signaling" "^1.10.0"
     "@lumino/widgets" "^1.37.2"
     resize-observer-polyfill "^1.5.1"
 
 "@jupyterlab/rendermime-interfaces@^3.6.7":
-  version "3.9.8"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime-interfaces/-/rendermime-interfaces-3.9.8.tgz#1e048ebc7f0d067770523a46cea17e61ebf7df1c"
-  integrity sha512-I9+g4ZIb+6cDgieKUj3Vh5MQb5Vpger7fcMGopbAhnD5N8JiFVdpmO84pnORmOd3G4k7bTkrbHiREgtpWzcg7w==
+  version "3.9.5"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime-interfaces/-/rendermime-interfaces-3.9.5.tgz#a0c4aa1fe062449611305c69ca2ccab95942aac5"
+  integrity sha512-GAK16huX5JbHlnxJYJnwMe8V3ECgywA1Td6VFKgZXE6QnAuONCQtpIYCiTEWKBgleIVFUZ8t8q3xTDg0mxM5wg==
   dependencies:
     "@lumino/coreutils" "^1.11.0 || ^2.1.2"
     "@lumino/widgets" "^1.37.2 || ^2.3.1"
 
 "@jupyterlab/rendermime@^3.6.7":
   version "3.6.7"
   resolved "https://registry.yarnpkg.com/@jupyterlab/rendermime/-/rendermime-3.6.7.tgz#24939caf48ae98fc02aac60793a56d60eb461018"
@@ -900,17 +905,17 @@
   resolved "https://registry.yarnpkg.com/@types/eslint-scope/-/eslint-scope-3.7.7.tgz#3108bd5f18b0cdb277c867b3dd449c9ed7079ac5"
   integrity sha512-MzMFlSLBqNF2gcHWO0G1vP/YQyfvrxZ0bF+u7mzUdZ1/xK4A4sru+nraZz5i3iEIk1l1uyicaDVTB4QbbEkAYg==
   dependencies:
     "@types/eslint" "*"
     "@types/estree" "*"
 
 "@types/eslint@*":
-  version "8.56.10"
-  resolved "https://registry.yarnpkg.com/@types/eslint/-/eslint-8.56.10.tgz#eb2370a73bf04a901eeba8f22595c7ee0f7eb58d"
-  integrity sha512-Shavhk87gCtY2fhXDctcfS3e6FdxWkCx1iUZ9eEUbh7rTqlZT0/IzOkCOVt0fCjcFuZ9FPYfuezTBImfHCDBGQ==
+  version "8.56.6"
+  resolved "https://registry.yarnpkg.com/@types/eslint/-/eslint-8.56.6.tgz#d5dc16cac025d313ee101108ba5714ea10eb3ed0"
+  integrity sha512-ymwc+qb1XkjT/gfoQwxIeHZ6ixH23A+tCT2ADSA/DPVKzAjwYkTXBMCQ/f6fe4wEa85Lhp26VPeUxI7wMhAi7A==
   dependencies:
     "@types/estree" "*"
     "@types/json-schema" "*"
 
 "@types/estree@*", "@types/estree@^1.0.5":
   version "1.0.5"
   resolved "https://registry.yarnpkg.com/@types/estree/-/estree-1.0.5.tgz#a6ce3e556e00fd9895dd872dd172ad0d4bd687f4"
@@ -930,17 +935,17 @@
 
 "@types/minimist@^1.2.0":
   version "1.2.5"
   resolved "https://registry.yarnpkg.com/@types/minimist/-/minimist-1.2.5.tgz#ec10755e871497bcd83efe927e43ec46e8c0747e"
   integrity sha512-hov8bUuiLiyFPGyFPE1lwWhmzYbirOXQNNo40+y3zow8aFVTeyn3VWL0VFFfdNddA8S4Vf0Tc062rzyNr7Paag==
 
 "@types/node@*":
-  version "20.12.8"
-  resolved "https://registry.yarnpkg.com/@types/node/-/node-20.12.8.tgz#35897bf2bfe3469847ab04634636de09552e8256"
-  integrity sha512-NU0rJLJnshZWdE/097cdCBbyW1h4hEg0xpovcoAQYHl8dnEyp/NAOiE45pvc+Bd1Dt+2r94v2eGFpQJ4R7g+2w==
+  version "20.11.30"
+  resolved "https://registry.yarnpkg.com/@types/node/-/node-20.11.30.tgz#9c33467fc23167a347e73834f788f4b9f399d66f"
+  integrity sha512-dHM6ZxwlmuZaRmUPfv1p+KrdD1Dci04FbdEm/9wEMouFqxYoFl5aMkt0VMAUtYRQDyYvD41WJLukhq/ha3YuTw==
   dependencies:
     undici-types "~5.26.4"
 
 "@types/node@^17.0.29":
   version "17.0.45"
   resolved "https://registry.yarnpkg.com/@types/node/-/node-17.0.45.tgz#2c0fafd78705e7a18b7906b5201a522719dc5190"
   integrity sha512-w+tIMs3rq2afQdsPJlODhoUEKzFP1ayaoyl1CcnwtIlsVe7K7bA1NGm4s3PraqTLlXnbIN84zuBlxBWo1u9BLw==
@@ -1280,22 +1285,22 @@
   dependencies:
     fast-deep-equal "^3.1.1"
     fast-json-stable-stringify "^2.0.0"
     json-schema-traverse "^0.4.1"
     uri-js "^4.2.2"
 
 ajv@^8.0.1:
-  version "8.13.0"
-  resolved "https://registry.yarnpkg.com/ajv/-/ajv-8.13.0.tgz#a3939eaec9fb80d217ddf0c3376948c023f28c91"
-  integrity sha512-PRA911Blj99jR5RMeTunVbNXMF6Lp4vZXnk5GQjcnUWUTsrXtekg/pnmFFI2u/I36Y/2bITGS30GZCXei6uNkA==
+  version "8.12.0"
+  resolved "https://registry.yarnpkg.com/ajv/-/ajv-8.12.0.tgz#d1a0527323e22f53562c567c00991577dfbe19d1"
+  integrity sha512-sRu1kpcO9yLtYxBKvqfTeh9KzZEwO3STyX1HT+4CaDzC6HpTGYhIhPIzj9XuKU7KYDwnaeh5hcOwjy1QuJzBPA==
   dependencies:
-    fast-deep-equal "^3.1.3"
+    fast-deep-equal "^3.1.1"
     json-schema-traverse "^1.0.0"
     require-from-string "^2.0.2"
-    uri-js "^4.4.1"
+    uri-js "^4.2.2"
 
 ansi-colors@^4.1.1:
   version "4.1.3"
   resolved "https://registry.yarnpkg.com/ansi-colors/-/ansi-colors-4.1.3.tgz#37611340eb2243e70cc604cad35d63270d48781b"
   integrity sha512-/6w/C21Pm1A7aZitlI5Ni/2J6FFQN8i1Cvz3kHABAAbw93v/NlvKdVOqz7CCWz/3iv/JplRSEEZ83XION15ovw==
 
 ansi-regex@^5.0.1:
@@ -1507,17 +1512,17 @@
 
 camelcase@^5.3.1:
   version "5.3.1"
   resolved "https://registry.yarnpkg.com/camelcase/-/camelcase-5.3.1.tgz#e3c9b31569e106811df242f715725a1f4c494320"
   integrity sha512-L28STB170nwWS63UjtlEOE3dldQApaJXZkOI1uMFfzf3rRuPegHaHesyee+YxQ+W6SvRDQV6UrdOdRiR153wJg==
 
 caniuse-lite@^1.0.30001587:
-  version "1.0.30001614"
-  resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001614.tgz#f894b4209376a0bf923d67d9c361d96b1dfebe39"
-  integrity sha512-jmZQ1VpmlRwHgdP1/uiKzgiAuGOfLEJsYFP4+GBou/QQ4U6IOJCB4NP1c+1p9RGLpwObcT94jA5/uO+F1vBbog==
+  version "1.0.30001600"
+  resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001600.tgz#93a3ee17a35aa6a9f0c6ef1b2ab49507d1ab9079"
+  integrity sha512-+2S9/2JFhYmYaDpZvo0lKkfvuKIglrx68MwOBqMGHhQsNkLjB5xtc/TGoEPs+MxjSyN/72qer2g97nzR641mOQ==
 
 chalk@^2.3.0, chalk@^2.4.1, chalk@^2.4.2:
   version "2.4.2"
   resolved "https://registry.yarnpkg.com/chalk/-/chalk-2.4.2.tgz#cd42541677a54333cf541a49108c1432b44c9424"
   integrity sha512-Mti+f9lpJNcwF4tWV8/OrTTtF1gZi+f8FqlyAdouralcFWFQWF2+NgCHShjkCb+IFBLq9buZwE1xckQU4peSuQ==
   dependencies:
     ansi-styles "^3.2.1"
@@ -1648,17 +1653,17 @@
 
 concat-map@0.0.1:
   version "0.0.1"
   resolved "https://registry.yarnpkg.com/concat-map/-/concat-map-0.0.1.tgz#d8a96bd77fd68df7793a73036a3ba0d5405d477b"
   integrity sha512-/Srv4dswyQNBfohGpz9o6Yb3Gz3SrUDqBH5rTuhGR7ahtlbYKnVxw2bCFMRljaA7EXHaXZ8wsHdodFvbkhKmqg==
 
 core-js-pure@^3.6.5:
-  version "3.37.0"
-  resolved "https://registry.yarnpkg.com/core-js-pure/-/core-js-pure-3.37.0.tgz#ce99fb4a7cec023fdbbe5b5bd1f06bbcba83316e"
-  integrity sha512-d3BrpyFr5eD4KcbRvQ3FTUx/KWmaDesr7+a3+1+P46IUnNoEt+oiLijPINZMEon7w9oGkIINWxrBAU9DEciwFQ==
+  version "3.36.1"
+  resolved "https://registry.yarnpkg.com/core-js-pure/-/core-js-pure-3.36.1.tgz#1461c89e76116528b54eba20a0aff30164087a94"
+  integrity sha512-NXCvHvSVYSrewP0L5OhltzXeWFJLo2AL2TYnj6iLV3Bw8mM62wAQMNgUCRI6EBu6hVVpbCxmOPlxh1Ikw2PfUA==
 
 cosmiconfig@^7.1.0:
   version "7.1.0"
   resolved "https://registry.yarnpkg.com/cosmiconfig/-/cosmiconfig-7.1.0.tgz#1443b9afa596b670082ea46cbd8f6a62b84635f6"
   integrity sha512-AdmX6xUzdNASswsFtmwSt7Vj8po9IuqXm0UXz7QKPuEUmPB4XyjGfaAr2PSuELMwkRMVH1EpIkX5bTZGRB3eCA==
   dependencies:
     "@types/parse-json" "^4.0.0"
@@ -1684,17 +1689,17 @@
   integrity sha512-iRDPJKUPVEND7dHPO8rkbOnPpyDygcDFtWjpeWNCgy8WP2rXcxXL8TskReQl6OrB2G7+UJrags1q15Fudc7G6w==
   dependencies:
     path-key "^3.1.0"
     shebang-command "^2.0.0"
     which "^2.0.1"
 
 css-functions-list@^3.1.0:
-  version "3.2.2"
-  resolved "https://registry.yarnpkg.com/css-functions-list/-/css-functions-list-3.2.2.tgz#9a54c6dd8416ed25c1079cd88234e927526c1922"
-  integrity sha512-c+N0v6wbKVxTu5gOBBFkr9BEdBWaqqjQeiJ8QvSRIJOf+UxlJh930m8e6/WNeODIK0mYLFkoONrnj16i2EcvfQ==
+  version "3.2.1"
+  resolved "https://registry.yarnpkg.com/css-functions-list/-/css-functions-list-3.2.1.tgz#2eb205d8ce9f9ce74c5c1d7490b66b77c45ce3ea"
+  integrity sha512-Nj5YcaGgBtuUmn1D7oHqPW0c9iui7xsTsj5lIX8ZgevdfhmjFfKB3r8moHJtNJnctnYXJyYX5I1pp90HM4TPgQ==
 
 css-loader@^5.0.1:
   version "5.2.7"
   resolved "https://registry.yarnpkg.com/css-loader/-/css-loader-5.2.7.tgz#9b9f111edf6fb2be5dc62525644cbc9c232064ae"
   integrity sha512-Q7mOvpBNBG7YrVGMxRxcBJZFL75o+cH2abNASdibkj/fffYD8qWbInZrD0S9ccI6vZclF3DsHE7njGlLtaHbhg==
   dependencies:
     icss-utils "^5.1.0"
@@ -1819,15 +1824,15 @@
   resolved "https://registry.yarnpkg.com/define-data-property/-/define-data-property-1.1.4.tgz#894dc141bb7d3060ae4366f6a0107e68fbe48c5e"
   integrity sha512-rBMvIzlpA8v6E+SJZoo++HAYqsLrkg7MSfIinMPFhmkorw7X+dOXVJQs+QT69zGkzMyfDnIMN2Wid1+NbL3T+A==
   dependencies:
     es-define-property "^1.0.0"
     es-errors "^1.3.0"
     gopd "^1.0.1"
 
-define-properties@^1.2.0, define-properties@^1.2.1:
+define-properties@^1.1.3, define-properties@^1.2.0, define-properties@^1.2.1:
   version "1.2.1"
   resolved "https://registry.yarnpkg.com/define-properties/-/define-properties-1.2.1.tgz#10781cc616eb951a80a034bafcaa7377f6af2b6c"
   integrity sha512-8QmQKqEASLd5nx0U1B1okLElbUuuttJ/AnYmRXbbbGDWh6uS208EjD4Xqq/I9wK7u0v6O08XhTWnt5XtEbR6Dg==
   dependencies:
     define-data-property "^1.0.1"
     has-property-descriptors "^1.0.0"
     object-keys "^1.1.1"
@@ -1900,17 +1905,17 @@
   dependencies:
     chalk "^2.3.0"
     find-root "^1.0.0"
     lodash "^4.17.4"
     semver "^5.4.1"
 
 electron-to-chromium@^1.4.668:
-  version "1.4.752"
-  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.752.tgz#99227455547c8254488e3dab7d316c34a2c067b8"
-  integrity sha512-P3QJreYI/AUTcfBVrC4zy9KvnZWekViThgQMX/VpJ+IsOBbcX5JFpORM4qWapwWQ+agb2nYAOyn/4PMXOk0m2Q==
+  version "1.4.717"
+  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.717.tgz#99db370cae8cd090d5b01f8748e9ad369924d0f8"
+  integrity sha512-6Fmg8QkkumNOwuZ/5mIbMU9WI3H2fmn5ajcVya64I5Yr5CcNmO7vcLt0Y7c96DCiMO5/9G+4sI2r6eEvdg1F7A==
 
 emoji-regex@^8.0.0:
   version "8.0.0"
   resolved "https://registry.yarnpkg.com/emoji-regex/-/emoji-regex-8.0.0.tgz#e818fd69ce5ccfcb404594f842963bf53164cc37"
   integrity sha512-MSjYzcWNOA0ewAHpz0MxpYFvwg6yjy1NG3xteoqz644VCo/RPgnr1/GGt+ic3iJTzQ8Eu3TdM14SawnVUmGE6A==
 
 emojis-list@^3.0.0:
@@ -1946,17 +1951,17 @@
 
 entities@^2.0.0:
   version "2.2.0"
   resolved "https://registry.yarnpkg.com/entities/-/entities-2.2.0.tgz#098dc90ebb83d8dffa089d55256b351d34c4da55"
   integrity sha512-p92if5Nz619I0w+akJrLZH0MX0Pb5DX39XOwQTtXSdQQOaYH03S1uIQp4mhOZtAXrxq4ViO67YTiLBo2638o9A==
 
 envinfo@^7.7.3:
-  version "7.13.0"
-  resolved "https://registry.yarnpkg.com/envinfo/-/envinfo-7.13.0.tgz#81fbb81e5da35d74e814941aeab7c325a606fb31"
-  integrity sha512-cvcaMr7KqXVh4nyzGTVqTum+gAiL265x5jUWQIDLq//zOGbW+gSW/C+OWLleY/rs9Qole6AZLMXPbtIFQbqu+Q==
+  version "7.11.1"
+  resolved "https://registry.yarnpkg.com/envinfo/-/envinfo-7.11.1.tgz#2ffef77591057081b0129a8fd8cf6118da1b94e1"
+  integrity sha512-8PiZgZNIB4q/Lw4AhOvAfB/ityHAd2bli3lESSWmWSzSsl5dKpy5N1d1Rfkd2teq/g9xN90lc6o98DOjMeYHpg==
 
 errno@~0.1.1:
   version "0.1.8"
   resolved "https://registry.yarnpkg.com/errno/-/errno-0.1.8.tgz#8bb3e9c7d463be4976ff888f76b4809ebc2e811f"
   integrity sha512-dJ6oBr5SQ1VSd9qkk7ByRgb/1SH4JZjCHSW/mr63/QcXO9zLVxvJ6Oy13nio03rxpSnVDDjFor75SjVeZWPW/A==
   dependencies:
     prr "~1.0.1"
@@ -1965,17 +1970,17 @@
   version "1.3.2"
   resolved "https://registry.yarnpkg.com/error-ex/-/error-ex-1.3.2.tgz#b4ac40648107fdcdcfae242f428bea8a14d4f1bf"
   integrity sha512-7dFHNmqeFSEt2ZBsCriorKnn3Z2pj+fd9kmI6QoWw4//DL+icEBfc0U7qJCisqrTsKTjw4fNFy2pW9OqStD84g==
   dependencies:
     is-arrayish "^0.2.1"
 
 es-abstract@^1.22.1, es-abstract@^1.22.3, es-abstract@^1.23.0, es-abstract@^1.23.2:
-  version "1.23.3"
-  resolved "https://registry.yarnpkg.com/es-abstract/-/es-abstract-1.23.3.tgz#8f0c5a35cd215312573c5a27c87dfd6c881a0aa0"
-  integrity sha512-e+HfNH61Bj1X9/jLc5v1owaLYuHdeHHSQlkhCBiTK8rBvKaULl/beGMxwrMXjpYrv4pz22BlY570vVePA2ho4A==
+  version "1.23.2"
+  resolved "https://registry.yarnpkg.com/es-abstract/-/es-abstract-1.23.2.tgz#693312f3940f967b8dd3eebacb590b01712622e0"
+  integrity sha512-60s3Xv2T2p1ICykc7c+DNDPLDMm9t4QxCOUU0K9JxiLjM3C1zB9YVdN7tjxrFd4+AkZ8CdX1ovUga4P2+1e+/w==
   dependencies:
     array-buffer-byte-length "^1.0.1"
     arraybuffer.prototype.slice "^1.0.3"
     available-typed-arrays "^1.0.7"
     call-bind "^1.0.7"
     data-view-buffer "^1.0.1"
     data-view-byte-length "^1.0.1"
@@ -2008,19 +2013,19 @@
     object-keys "^1.1.1"
     object.assign "^4.1.5"
     regexp.prototype.flags "^1.5.2"
     safe-array-concat "^1.1.2"
     safe-regex-test "^1.0.3"
     string.prototype.trim "^1.2.9"
     string.prototype.trimend "^1.0.8"
-    string.prototype.trimstart "^1.0.8"
+    string.prototype.trimstart "^1.0.7"
     typed-array-buffer "^1.0.2"
     typed-array-byte-length "^1.0.1"
     typed-array-byte-offset "^1.0.2"
-    typed-array-length "^1.0.6"
+    typed-array-length "^1.0.5"
     unbox-primitive "^1.0.2"
     which-typed-array "^1.1.15"
 
 es-define-property@^1.0.0:
   version "1.0.0"
   resolved "https://registry.yarnpkg.com/es-define-property/-/es-define-property-1.0.0.tgz#c7faefbdff8b2696cf5f46921edfb77cc4ba3845"
   integrity sha512-jxayLKShrEqqzJ0eumQbVhTYQM27CfT1T35+gCgDFoL82JLsXqTJ76zv6A0YLOgEnLUMvLzsDsGIrl8NFpT2gQ==
@@ -2029,17 +2034,17 @@
 
 es-errors@^1.2.1, es-errors@^1.3.0:
   version "1.3.0"
   resolved "https://registry.yarnpkg.com/es-errors/-/es-errors-1.3.0.tgz#05f75a25dab98e4fb1dcd5e1472c0546d5057c8f"
   integrity sha512-Zf5H2Kxt2xjTvbJvP2ZWLEICxA6j+hAmMzIlypy4xcBg1vKVnx89Wy0GbS+kf5cwCVFFzdCFh2XSCFNULS6csw==
 
 es-module-lexer@^1.2.1:
-  version "1.5.2"
-  resolved "https://registry.yarnpkg.com/es-module-lexer/-/es-module-lexer-1.5.2.tgz#00b423304f2500ac59359cc9b6844951f372d497"
-  integrity sha512-l60ETUTmLqbVbVHv1J4/qj+M8nq7AwMzEcg3kmJDt9dCNrTk+yHcYFf/Kw75pMDwd9mPcIGCG5LcS20SxYRzFA==
+  version "1.5.0"
+  resolved "https://registry.yarnpkg.com/es-module-lexer/-/es-module-lexer-1.5.0.tgz#4878fee3789ad99e065f975fdd3c645529ff0236"
+  integrity sha512-pqrTKmwEIgafsYZAGw9kszYzmagcE/n4dbgwGWLEXg7J4QFJVQRBld8j3Q3GNez79jzxZshq0bcT962QHOghjw==
 
 es-object-atoms@^1.0.0:
   version "1.0.0"
   resolved "https://registry.yarnpkg.com/es-object-atoms/-/es-object-atoms-1.0.0.tgz#ddb55cd47ac2e240701260bc2a8e31ecb643d941"
   integrity sha512-MZ4iQ6JwHOBQjahnjwaC1ZtIBH+2ohjamzAO3oaHcXYup7qxjF2fixyH+Q71voWHeOkI2q/TnJao/KfXYIZWbw==
   dependencies:
     es-errors "^1.3.0"
@@ -2058,15 +2063,15 @@
   resolved "https://registry.yarnpkg.com/es-to-primitive/-/es-to-primitive-1.2.1.tgz#e55cd4c9cdc188bcefb03b366c736323fc5c898a"
   integrity sha512-QCOllgZJtaUo9miYBcLChTUaHNjJF3PYs1VidD7AwiEj1kYxKeQTctLAezAOH5ZKRH0g2IgPn6KwB4IT8iRpvA==
   dependencies:
     is-callable "^1.1.4"
     is-date-object "^1.0.1"
     is-symbol "^1.0.2"
 
-escalade@^3.1.2:
+escalade@^3.1.1:
   version "3.1.2"
   resolved "https://registry.yarnpkg.com/escalade/-/escalade-3.1.2.tgz#54076e9ab29ea5bf3d8f1ed62acffbb88272df27"
   integrity sha512-ErCHMCae19vR8vQGe50xIsVomy19rg6gFu3+r3jkEO46suLMWBksvVyoGgQV+jOfl84ZSOSlmv6Gxa89PmTGmA==
 
 escape-string-regexp@^1.0.5:
   version "1.0.5"
   resolved "https://registry.yarnpkg.com/escape-string-regexp/-/escape-string-regexp-1.0.5.tgz#1b61c0562190a8dff6ae3bb2cf0200ca130b86d4"
@@ -2477,20 +2482,19 @@
   version "13.24.0"
   resolved "https://registry.yarnpkg.com/globals/-/globals-13.24.0.tgz#8432a19d78ce0c1e833949c36adb345400bb1171"
   integrity sha512-AhO5QUcj8llrbG09iWhPU2B204J1xnPeL8kQmVorSsy+Sjj1sk8gIyh6cUocGmH4L0UuhAJy+hJMRA4mgA4mFQ==
   dependencies:
     type-fest "^0.20.2"
 
 globalthis@^1.0.3:
-  version "1.0.4"
-  resolved "https://registry.yarnpkg.com/globalthis/-/globalthis-1.0.4.tgz#7430ed3a975d97bfb59bcce41f5cabbafa651236"
-  integrity sha512-DpLKbNU4WylpxJykQujfCcwYWiV/Jhm50Goo0wrVILAv5jOr9d+H+UR3PhSCD2rCCEIg0uc+G+muBTwD54JhDQ==
+  version "1.0.3"
+  resolved "https://registry.yarnpkg.com/globalthis/-/globalthis-1.0.3.tgz#5852882a52b80dc301b0660273e1ed082f0b6ccf"
+  integrity sha512-sFdI5LyBiNTHjRd7cGPWapiHWMOXKyuBNX/cWJ3NfzrZQVa8GI/8cofCl74AOVqq9W5kNmguTIzJ/1s2gyI9wA==
   dependencies:
-    define-properties "^1.2.1"
-    gopd "^1.0.1"
+    define-properties "^1.1.3"
 
 globby@^11.0.3, globby@^11.1.0:
   version "11.1.0"
   resolved "https://registry.yarnpkg.com/globby/-/globby-11.1.0.tgz#bd4be98bb042f83d796f7e3811991fbe82a0d34b"
   integrity sha512-jhIXaOzy1sb8IyocaruWSn1TjmnBVs8Ayhcy83rmxNJ8q2uWKCAj3CnJY+KpGSXCueAPc0i05kVvVKtP1t9S3g==
   dependencies:
     array-union "^2.1.0"
@@ -3490,24 +3494,24 @@
   version "1.4.0"
   resolved "https://registry.yarnpkg.com/once/-/once-1.4.0.tgz#583b1aa775961d4b113ac17d9c50baef9dd76bd1"
   integrity sha512-lNaJgI+2Q5URQBkccEKHTQOPaXdUxnZZElQTZY0MFUAuaEqe1E+Nyvgdz/aIyNi6Z9MzO5dv1H8n58/GELp3+w==
   dependencies:
     wrappy "1"
 
 optionator@^0.9.1:
-  version "0.9.4"
-  resolved "https://registry.yarnpkg.com/optionator/-/optionator-0.9.4.tgz#7ea1c1a5d91d764fb282139c88fe11e182a3a734"
-  integrity sha512-6IpQ7mKUxRcZNLIObR0hz7lxsapSSIYNZJwXPGeF0mTVqGKFIXj1DQcMoT22S3ROcLyY/rz0PWaWZ9ayWmad9g==
+  version "0.9.3"
+  resolved "https://registry.yarnpkg.com/optionator/-/optionator-0.9.3.tgz#007397d44ed1872fdc6ed31360190f81814e2c64"
+  integrity sha512-JjCoypp+jKn1ttEFExxhetCKeJt9zhAgAve5FXHixTvFDW/5aEktX9bufBKLRRMdU7bNtpLfcGu94B3cdEJgjg==
   dependencies:
+    "@aashutoshrathi/word-wrap" "^1.2.3"
     deep-is "^0.1.3"
     fast-levenshtein "^2.0.6"
     levn "^0.4.1"
     prelude-ls "^1.2.1"
     type-check "^0.4.0"
-    word-wrap "^1.2.5"
 
 p-limit@^2.2.0:
   version "2.3.0"
   resolved "https://registry.yarnpkg.com/p-limit/-/p-limit-2.3.0.tgz#3dd33c647a214fdfffd835933eb086da0dc21db1"
   integrity sha512-//88mFWSJx8lxCzwdAABTJL2MyWB12+eIY7MDL2SqLmAkeKU9qxRvWuSyTjm3FUmpBEMuFfckAIqEaVGUDxb6w==
   dependencies:
     p-try "^2.0.0"
@@ -3649,31 +3653,31 @@
 
 postcss-media-query-parser@^0.2.3:
   version "0.2.3"
   resolved "https://registry.yarnpkg.com/postcss-media-query-parser/-/postcss-media-query-parser-0.2.3.tgz#27b39c6f4d94f81b1a73b8f76351c609e5cef244"
   integrity sha512-3sOlxmbKcSHMjlUXQZKQ06jOswE7oVkXPxmZdoB1r5l0q6gTFTQSHxNxOrCccElbW7dxNytifNEo8qidX2Vsig==
 
 postcss-modules-extract-imports@^3.0.0:
-  version "3.1.0"
-  resolved "https://registry.yarnpkg.com/postcss-modules-extract-imports/-/postcss-modules-extract-imports-3.1.0.tgz#b4497cb85a9c0c4b5aabeb759bb25e8d89f15002"
-  integrity sha512-k3kNe0aNFQDAZGbin48pL2VNidTF0w4/eASDsxlyspobzU3wZQLOGj7L9gfRe0Jo9/4uud09DsjFNH7winGv8Q==
+  version "3.0.0"
+  resolved "https://registry.yarnpkg.com/postcss-modules-extract-imports/-/postcss-modules-extract-imports-3.0.0.tgz#cda1f047c0ae80c97dbe28c3e76a43b88025741d"
+  integrity sha512-bdHleFnP3kZ4NYDhuGlVK+CMrQ/pqUm8bx/oGL93K6gVwiclvX5x0n76fYMKuIGKzlABOy13zsvqjb0f92TEXw==
 
 postcss-modules-local-by-default@^4.0.0:
-  version "4.0.5"
-  resolved "https://registry.yarnpkg.com/postcss-modules-local-by-default/-/postcss-modules-local-by-default-4.0.5.tgz#f1b9bd757a8edf4d8556e8d0f4f894260e3df78f"
-  integrity sha512-6MieY7sIfTK0hYfafw1OMEG+2bg8Q1ocHCpoWLqOKj3JXlKu4G7btkmM/B7lFubYkYWmRSPLZi5chid63ZaZYw==
+  version "4.0.4"
+  resolved "https://registry.yarnpkg.com/postcss-modules-local-by-default/-/postcss-modules-local-by-default-4.0.4.tgz#7cbed92abd312b94aaea85b68226d3dec39a14e6"
+  integrity sha512-L4QzMnOdVwRm1Qb8m4x8jsZzKAaPAgrUF1r/hjDR2Xj7R+8Zsf97jAlSQzWtKx5YNiNGN8QxmPFIc/sh+RQl+Q==
   dependencies:
     icss-utils "^5.0.0"
     postcss-selector-parser "^6.0.2"
     postcss-value-parser "^4.1.0"
 
 postcss-modules-scope@^3.0.0:
-  version "3.2.0"
-  resolved "https://registry.yarnpkg.com/postcss-modules-scope/-/postcss-modules-scope-3.2.0.tgz#a43d28289a169ce2c15c00c4e64c0858e43457d5"
-  integrity sha512-oq+g1ssrsZOsx9M96c5w8laRmvEu9C3adDSjI8oTcbfkrTE8hx/zfyobUoWIxaKPO8bt6S62kxpw5GqypEw1QQ==
+  version "3.1.1"
+  resolved "https://registry.yarnpkg.com/postcss-modules-scope/-/postcss-modules-scope-3.1.1.tgz#32cfab55e84887c079a19bbb215e721d683ef134"
+  integrity sha512-uZgqzdTleelWjzJY+Fhti6F3C9iF1JR/dODLs/JDefozYcKTBCdD8BIl6nNPbTbcLnGrk56hzwZC2DaGNvYjzA==
   dependencies:
     postcss-selector-parser "^6.0.4"
 
 postcss-modules-values@^4.0.0:
   version "4.0.0"
   resolved "https://registry.yarnpkg.com/postcss-modules-values/-/postcss-modules-values-4.0.0.tgz#d7c5e7e68c3bb3c9b27cbf48ca0bb3ffb4602c9c"
   integrity sha512-RDxHkAiEGI78gS2ofyvCsu7iycRv7oqw5xMWn9iMoR0N/7mf9D50ecQqUo5BZ9Zh2vH4bCUR/ktCqbB9m8vJjQ==
@@ -3765,17 +3769,17 @@
 
 punycode@^2.1.0, punycode@^2.1.1:
   version "2.3.1"
   resolved "https://registry.yarnpkg.com/punycode/-/punycode-2.3.1.tgz#027422e2faec0b25e1549c3e1bd8309b9133b6e5"
   integrity sha512-vYt7UD1U9Wg6138shLtLOvdAu+8DsC/ilFtEVHcH+wydcSpNE20AfSOduf6MkRFahL5FY7X1oU7nKVZFtfq8Fg==
 
 qs@^6.11.2:
-  version "6.12.1"
-  resolved "https://registry.yarnpkg.com/qs/-/qs-6.12.1.tgz#39422111ca7cbdb70425541cba20c7d7b216599a"
-  integrity sha512-zWmv4RSuB9r2mYQw3zxQuHWeU+42aKi1wWig/j4ele4ygELZ7PEO6MM7rim9oAQH2A5MWfsAVf/jPvTPgCbvUQ==
+  version "6.12.0"
+  resolved "https://registry.yarnpkg.com/qs/-/qs-6.12.0.tgz#edd40c3b823995946a8a0b1f208669c7a200db77"
+  integrity sha512-trVZiI6RMOkO476zLGaBIzszOdFPnCCXHPG9kn0yuS1uz6xdVxPfZdB3vUig9pxPFDM9BRAgz/YUIVQ1/vuiUg==
   dependencies:
     side-channel "^1.0.6"
 
 querystringify@^2.1.1:
   version "2.2.0"
   resolved "https://registry.yarnpkg.com/querystringify/-/querystringify-2.2.0.tgz#3345941b4153cb9d082d8eee4cda2016a9aef7f6"
   integrity sha512-FIqgj2EUvTa7R50u0rGsyTftzjYmv/a3hO345bZNrqabNqjtgiDMgmo4mkUjd+nzU5oF3dClKqFIPUKybUyqoQ==
@@ -4278,15 +4282,15 @@
   resolved "https://registry.yarnpkg.com/string.prototype.trimend/-/string.prototype.trimend-1.0.8.tgz#3651b8513719e8a9f48de7f2f77640b26652b229"
   integrity sha512-p73uL5VCHCO2BZZ6krwwQE3kCzM7NKmis8S//xEC6fQonchbum4eP6kR4DLEjQFO3Wnj3Fuo8NM0kOSjVdHjZQ==
   dependencies:
     call-bind "^1.0.7"
     define-properties "^1.2.1"
     es-object-atoms "^1.0.0"
 
-string.prototype.trimstart@^1.0.8:
+string.prototype.trimstart@^1.0.7:
   version "1.0.8"
   resolved "https://registry.yarnpkg.com/string.prototype.trimstart/-/string.prototype.trimstart-1.0.8.tgz#7ee834dda8c7c17eff3118472bb35bfedaa34dde"
   integrity sha512-UXSH262CSZY1tfu3G3Secr6uGLCFVPMhIqHjlgCUtCCcgihYc/xKs9djMTMUOb2j1mVSeU8EU6NWc/iQKU6Gfg==
   dependencies:
     call-bind "^1.0.7"
     define-properties "^1.2.1"
     es-object-atoms "^1.0.0"
@@ -4501,17 +4505,17 @@
     "@jridgewell/trace-mapping" "^0.3.20"
     jest-worker "^27.4.5"
     schema-utils "^3.1.1"
     serialize-javascript "^6.0.1"
     terser "^5.26.0"
 
 terser@^5.26.0, terser@^5.3.4:
-  version "5.31.0"
-  resolved "https://registry.yarnpkg.com/terser/-/terser-5.31.0.tgz#06eef86f17007dbad4593f11a574c7f5eb02c6a1"
-  integrity sha512-Q1JFAoUKE5IMfI4Z/lkE/E6+SwgzO+x4tq4v1AyBLRj8VSYvRO6A/rQrPg1yud4g0En9EKI1TvFRF2tQFcoUkg==
+  version "5.29.2"
+  resolved "https://registry.yarnpkg.com/terser/-/terser-5.29.2.tgz#c17d573ce1da1b30f21a877bffd5655dd86fdb35"
+  integrity sha512-ZiGkhUBIM+7LwkNjXYJq8svgkd+QK3UUr0wJqY4MieaezBSAIPgbSPZyIx0idM6XWK5CMzSWa8MJIzmRcB8Caw==
   dependencies:
     "@jridgewell/source-map" "^0.3.3"
     acorn "^8.8.2"
     commander "^2.20.0"
     source-map-support "~0.5.20"
 
 text-table@^0.2.0:
@@ -4627,15 +4631,15 @@
     available-typed-arrays "^1.0.7"
     call-bind "^1.0.7"
     for-each "^0.3.3"
     gopd "^1.0.1"
     has-proto "^1.0.3"
     is-typed-array "^1.1.13"
 
-typed-array-length@^1.0.6:
+typed-array-length@^1.0.5:
   version "1.0.6"
   resolved "https://registry.yarnpkg.com/typed-array-length/-/typed-array-length-1.0.6.tgz#57155207c76e64a3457482dfdc1c9d1d3c4c73a3"
   integrity sha512-/OxDN6OtAk5KBpGb28T+HZc2M+ADtvRxXrKKbUwtsLgdoxgX13hyy7ek6bFRl5+aBs2yZzB0c4CnQfAtVypW/g==
   dependencies:
     call-bind "^1.0.7"
     for-each "^0.3.3"
     gopd "^1.0.1"
@@ -4692,22 +4696,22 @@
 
 universalify@^2.0.0:
   version "2.0.1"
   resolved "https://registry.yarnpkg.com/universalify/-/universalify-2.0.1.tgz#168efc2180964e6386d061e094df61afe239b18d"
   integrity sha512-gptHNQghINnc/vTGIk0SOFGFNXw7JVrlRUtConJRlvaw6DuX0wO5Jeko9sWrMBhh+PsYAZ7oXAiOnf/UKogyiw==
 
 update-browserslist-db@^1.0.13:
-  version "1.0.14"
-  resolved "https://registry.yarnpkg.com/update-browserslist-db/-/update-browserslist-db-1.0.14.tgz#46a9367c323f8ade9a9dddb7f3ae7814b3a0b31c"
-  integrity sha512-JixKH8GR2pWYshIPUg/NujK3JO7JiqEEUiNArE86NQyrgUuZeTlZQN3xuS/yiV5Kb48ev9K6RqNkaJjXsdg7Jw==
+  version "1.0.13"
+  resolved "https://registry.yarnpkg.com/update-browserslist-db/-/update-browserslist-db-1.0.13.tgz#3c5e4f5c083661bd38ef64b6328c26ed6c8248c4"
+  integrity sha512-xebP81SNcPuNpPP3uzeW1NYXxI3rxyJzF3pD6sH4jE7o/IX+WtSpwnVU+qIsDPyk0d3hmFQ7mjqc6AtV604hbg==
   dependencies:
-    escalade "^3.1.2"
+    escalade "^3.1.1"
     picocolors "^1.0.0"
 
-uri-js@^4.2.2, uri-js@^4.4.1:
+uri-js@^4.2.2:
   version "4.4.1"
   resolved "https://registry.yarnpkg.com/uri-js/-/uri-js-4.4.1.tgz#9b1a52595225859e55f669d928f88c6c57f2a77e"
   integrity sha512-7rKUyy33Q1yc98pQ1DAmLtwX109F7TIfWlW1Ydo8Wl1ii1SeHieeh0HHfPeL2fMXK6z0s8ecKs9frCuLJvndBg==
   dependencies:
     punycode "^2.1.0"
 
 url-loader@~4.1.0:
@@ -4937,19 +4941,14 @@
     isexe "^2.0.0"
 
 wildcard@^2.0.0:
   version "2.0.1"
   resolved "https://registry.yarnpkg.com/wildcard/-/wildcard-2.0.1.tgz#5ab10d02487198954836b6349f74fff961e10f67"
   integrity sha512-CC1bOL87PIWSBhDcTrdeLo6eGT7mCFtrg0uIJtqJUFyK+eJnzl8A1niH56uu7KMa5XFrtiV+AQuHO3n7DsHnLQ==
 
-word-wrap@^1.2.5:
-  version "1.2.5"
-  resolved "https://registry.yarnpkg.com/word-wrap/-/word-wrap-1.2.5.tgz#d2c45c6dd4fbce621a66f136cbe328afd0410b34"
-  integrity sha512-BN22B5eaMMI9UMtjrGd5g5eCYPpCPDUy0FJXbYsaT5zYxjFOckS53SQDE3pWkVoWpHXVb3BrYcEN4Twa55B5cA==
-
 worker-loader@^3.0.2:
   version "3.0.8"
   resolved "https://registry.yarnpkg.com/worker-loader/-/worker-loader-3.0.8.tgz#5fc5cda4a3d3163d9c274a4e3a811ce8b60dbb37"
   integrity sha512-XQyQkIFeRVC7f7uRhFdNMe/iJOdO6zxAaR3EWbDp45v3mDhrTi+++oswKNxShUNjPC/1xUp5DB29YKLhFo129g==
   dependencies:
     loader-utils "^2.0.0"
     schema-utils "^3.0.0"
@@ -5030,17 +5029,17 @@
 
 yargs-parser@^20.2.3:
   version "20.2.9"
   resolved "https://registry.yarnpkg.com/yargs-parser/-/yargs-parser-20.2.9.tgz#2eb7dc3b0289718fc295f362753845c41a0c94ee"
   integrity sha512-y11nGElTIV+CT3Zv9t7VKl+Q3hTQoT9a1Qzezhhl6Rp21gJ/IVTW7Z3y9EWXhuUBC2Shnf+DX0antecpAwSP8w==
 
 yjs@^13.5.40:
-  version "13.6.15"
-  resolved "https://registry.yarnpkg.com/yjs/-/yjs-13.6.15.tgz#5a2402632aabf83e5baf56342b4c82fe40859306"
-  integrity sha512-moFv4uNYhp8BFxIk3AkpoAnnjts7gwdpiG8RtyFiKbMtxKCS0zVZ5wPaaGpwC3V2N/K8TK8MwtSI3+WO9CHWjQ==
+  version "13.6.14"
+  resolved "https://registry.yarnpkg.com/yjs/-/yjs-13.6.14.tgz#9326dfa03d1be3fb9af9ef7e41de4bfc78849a9f"
+  integrity sha512-D+7KcUr0j+vBCUSKXXEWfA+bG4UQBviAwP3gYBhkstkgwy5+8diOPMx0iqLIOxNo/HxaREUimZRxqHGAHCL2BQ==
   dependencies:
     lib0 "^0.2.86"
 
 yocto-queue@^0.1.0:
   version "0.1.0"
   resolved "https://registry.yarnpkg.com/yocto-queue/-/yocto-queue-0.1.0.tgz#0294eb3dee05028d31ee1a5fa2c556a6aaf10a1b"
   integrity sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==
```


# Comparing `tmp/quarto-cli-1.4.553.tar.gz` & `tmp/quarto_cli-1.4.554.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quarto-cli-1.4.553.tar", last modified: Wed Apr  3 18:38:17 2024, max compression
+gzip compressed data, was "quarto_cli-1.4.554.tar", last modified: Wed May  1 21:54:47 2024, max compression
```

## Comparing `quarto-cli-1.4.553.tar` & `quarto_cli-1.4.554.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:38:17.935815 quarto-cli-1.4.553/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-03 18:38:13.000000 quarto-cli-1.4.553/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 18:38:13.000000 quarto-cli-1.4.553/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-03 18:38:17.935815 quarto-cli-1.4.553/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-03 18:38:13.000000 quarto-cli-1.4.553/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-03 18:38:13.000000 quarto-cli-1.4.553/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:38:17.935815 quarto-cli-1.4.553/quarto_cli/
--rwxr-xr-x   0 runner    (1001) docker     (127)      160 2024-04-03 18:38:13.000000 quarto-cli-1.4.553/quarto_cli/quarto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:38:17.935815 quarto-cli-1.4.553/quarto_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-03 18:38:17.000000 quarto-cli-1.4.553/quarto_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-03 18:38:17.000000 quarto-cli-1.4.553/quarto_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:38:17.000000 quarto-cli-1.4.553/quarto_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 18:38:17.000000 quarto-cli-1.4.553/quarto_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 18:38:17.000000 quarto-cli-1.4.553/quarto_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 18:38:17.000000 quarto-cli-1.4.553/quarto_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:38:17.935815 quarto-cli-1.4.553/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-03 18:38:13.000000 quarto-cli-1.4.553/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 18:38:13.000000 quarto-cli-1.4.553/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:54:47.869159 quarto_cli-1.4.554/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-01 21:54:44.000000 quarto_cli-1.4.554/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 21:54:44.000000 quarto_cli-1.4.554/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-01 21:54:47.869159 quarto_cli-1.4.554/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-01 21:54:44.000000 quarto_cli-1.4.554/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-01 21:54:44.000000 quarto_cli-1.4.554/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:54:47.865159 quarto_cli-1.4.554/quarto_cli/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      160 2024-05-01 21:54:44.000000 quarto_cli-1.4.554/quarto_cli/quarto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:54:47.869159 quarto_cli-1.4.554/quarto_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-01 21:54:47.000000 quarto_cli-1.4.554/quarto_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-01 21:54:47.000000 quarto_cli-1.4.554/quarto_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:54:47.000000 quarto_cli-1.4.554/quarto_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 21:54:47.000000 quarto_cli-1.4.554/quarto_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 21:54:47.000000 quarto_cli-1.4.554/quarto_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 21:54:47.000000 quarto_cli-1.4.554/quarto_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 21:54:47.869159 quarto_cli-1.4.554/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-01 21:54:44.000000 quarto_cli-1.4.554/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 21:54:44.000000 quarto_cli-1.4.554/version.txt
```

### Comparing `quarto-cli-1.4.553/LICENSE` & `quarto_cli-1.4.554/LICENSE`

 * *Files identical despite different names*

### Comparing `quarto-cli-1.4.553/PKG-INFO` & `quarto_cli-1.4.554/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quarto-cli
-Version: 1.4.553
+Version: 1.4.554
 Summary: Open-source scientific and technical publishing system built on Pandoc.
 Author: Charles Teague, Carlos Scheidegger
 License: MIT License
         
         Copyright (c) 2023 Posit Software, PBC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quarto-cli-1.4.553/README.md` & `quarto_cli-1.4.554/README.md`

 * *Files identical despite different names*

### Comparing `quarto-cli-1.4.553/pyproject.toml` & `quarto_cli-1.4.554/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quarto-cli-1.4.553/quarto_cli.egg-info/PKG-INFO` & `quarto_cli-1.4.554/quarto_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quarto-cli
-Version: 1.4.553
+Version: 1.4.554
 Summary: Open-source scientific and technical publishing system built on Pandoc.
 Author: Charles Teague, Carlos Scheidegger
 License: MIT License
         
         Copyright (c) 2023 Posit Software, PBC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quarto-cli-1.4.553/setup.py` & `quarto_cli-1.4.554/setup.py`

 * *Files identical despite different names*


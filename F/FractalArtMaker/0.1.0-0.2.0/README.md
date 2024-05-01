# Comparing `tmp/FractalArtMaker-0.1.0.tar.gz` & `tmp/fractalartmaker-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FractalArtMaker-0.1.0.tar", last modified: Wed Mar  9 04:03:38 2022, max compression
+gzip compressed data, was "fractalartmaker-0.2.0.tar", last modified: Tue Apr 30 20:52:56 2024, max compression
```

## Comparing `FractalArtMaker-0.1.0.tar` & `fractalartmaker-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-03-09 04:03:38.798678 FractalArtMaker-0.1.0/
--rw-rw-rw-   0        0        0     1072 2022-03-09 01:24:41.000000 FractalArtMaker-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     9731 2022-03-09 04:03:38.797680 FractalArtMaker-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     8974 2022-03-09 03:12:28.000000 FractalArtMaker-0.1.0/README.md
--rw-rw-rw-   0        0        0        0 2022-03-09 01:24:41.000000 FractalArtMaker-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-03-09 04:03:38.798678 FractalArtMaker-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1522 2022-03-09 01:31:03.000000 FractalArtMaker-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-03-09 04:03:38.569467 FractalArtMaker-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2022-03-09 04:03:38.734679 FractalArtMaker-0.1.0/src/FractalArtMaker.egg-info/
--rw-rw-rw-   0        0        0     9731 2022-03-09 04:03:37.000000 FractalArtMaker-0.1.0/src/FractalArtMaker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2022-03-09 04:03:37.000000 FractalArtMaker-0.1.0/src/FractalArtMaker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-09 04:03:37.000000 FractalArtMaker-0.1.0/src/FractalArtMaker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2022-03-09 04:03:37.000000 FractalArtMaker-0.1.0/src/FractalArtMaker.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-03-09 04:03:38.792694 FractalArtMaker-0.1.0/src/fractalartmaker/
--rw-rw-rw-   0        0        0     6698 2022-03-09 01:54:25.000000 FractalArtMaker-0.1.0/src/fractalartmaker/__init__.py
--rw-rw-rw-   0        0        0       64 2022-03-09 01:24:42.000000 FractalArtMaker-0.1.0/src/fractalartmaker/__main__.py
+drwxr-xr-x   0 al         (501) staff       (20)        0 2024-04-30 20:52:56.701619 fractalartmaker-0.2.0/
+-rw-r--r--   0 al         (501) staff       (20)    20280 2024-04-30 20:52:56.701417 fractalartmaker-0.2.0/PKG-INFO
+-rw-r--r--   0 al         (501) staff       (20)    19238 2024-04-30 20:28:25.000000 fractalartmaker-0.2.0/README.md
+-rw-r--r--   0 al         (501) staff       (20)       38 2024-04-30 20:52:56.701655 fractalartmaker-0.2.0/setup.cfg
+-rw-r--r--   0 al         (501) staff       (20)     1825 2024-04-30 20:52:49.000000 fractalartmaker-0.2.0/setup.py
+drwxr-xr-x   0 al         (501) staff       (20)        0 2024-04-30 20:52:56.700164 fractalartmaker-0.2.0/src/
+drwxr-xr-x   0 al         (501) staff       (20)        0 2024-04-30 20:52:56.701246 fractalartmaker-0.2.0/src/FractalArtMaker.egg-info/
+-rw-r--r--   0 al         (501) staff       (20)    20280 2024-04-30 20:52:56.000000 fractalartmaker-0.2.0/src/FractalArtMaker.egg-info/PKG-INFO
+-rw-r--r--   0 al         (501) staff       (20)      254 2024-04-30 20:52:56.000000 fractalartmaker-0.2.0/src/FractalArtMaker.egg-info/SOURCES.txt
+-rw-r--r--   0 al         (501) staff       (20)        1 2024-04-30 20:52:56.000000 fractalartmaker-0.2.0/src/FractalArtMaker.egg-info/dependency_links.txt
+-rw-r--r--   0 al         (501) staff       (20)       16 2024-04-30 20:52:56.000000 fractalartmaker-0.2.0/src/FractalArtMaker.egg-info/top_level.txt
+drwxr-xr-x   0 al         (501) staff       (20)        0 2024-04-30 20:52:56.701114 fractalartmaker-0.2.0/src/fractalartmaker/
+-rw-r--r--   0 al         (501) staff       (20)    13415 2024-04-30 20:47:11.000000 fractalartmaker-0.2.0/src/fractalartmaker/__init__.py
+-rw-r--r--   0 al         (501) staff       (20)      939 2024-04-13 18:44:15.000000 fractalartmaker-0.2.0/src/fractalartmaker/__main__.py
```


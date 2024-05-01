# Comparing `tmp/tidal_wave-2024.4.3.tar.gz` & `tmp/tidal_wave-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidal_wave-2024.4.3.tar", last modified: Wed Apr 24 04:32:19 2024, max compression
+gzip compressed data, was "tidal_wave-2024.5.1.tar", last modified: Wed May  1 21:54:49 2024, max compression
```

## Comparing `tidal_wave-2024.4.3.tar` & `tidal_wave-2024.5.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:32:19.075366 tidal_wave-2024.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    40189 2024-04-24 04:32:19.075366 tidal_wave-2024.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26032 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 04:32:19.075366 tidal_wave-2024.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:32:19.071366 tidal_wave-2024.4.3/tidal_wave/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9900 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/album.py
--rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/artist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/dash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/hls.py
--rw-r--r--   0 runner    (1001) docker     (127)    12144 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/media.py
--rw-r--r--   0 runner    (1001) docker     (127)    20082 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/mix.py
--rw-r--r--   0 runner    (1001) docker     (127)    26637 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)    23923 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)    18615 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/requesting.py
--rw-r--r--   0 runner    (1001) docker     (127)    37425 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/track.py
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14843 2024-04-24 04:31:59.000000 tidal_wave-2024.4.3/tidal_wave/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 04:32:19.075366 tidal_wave-2024.4.3/tidal_wave.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    40189 2024-04-24 04:32:19.000000 tidal_wave-2024.4.3/tidal_wave.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-24 04:32:19.000000 tidal_wave-2024.4.3/tidal_wave.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 04:32:19.000000 tidal_wave-2024.4.3/tidal_wave.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 04:32:19.000000 tidal_wave-2024.4.3/tidal_wave.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-24 04:32:19.000000 tidal_wave-2024.4.3/tidal_wave.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 04:32:19.000000 tidal_wave-2024.4.3/tidal_wave.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:54:49.607175 tidal_wave-2024.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    41707 2024-05-01 21:54:49.607175 tidal_wave-2024.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27550 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 21:54:49.607175 tidal_wave-2024.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:54:49.607175 tidal_wave-2024.5.1/tidal_wave/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9900 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/album.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/hls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12144 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20082 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/mix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26637 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23923 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18725 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/requesting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37440 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14928 2024-05-01 21:54:33.000000 tidal_wave-2024.5.1/tidal_wave/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:54:49.607175 tidal_wave-2024.5.1/tidal_wave.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    41707 2024-05-01 21:54:49.000000 tidal_wave-2024.5.1/tidal_wave.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-01 21:54:49.000000 tidal_wave-2024.5.1/tidal_wave.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:54:49.000000 tidal_wave-2024.5.1/tidal_wave.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-01 21:54:49.000000 tidal_wave-2024.5.1/tidal_wave.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-01 21:54:49.000000 tidal_wave-2024.5.1/tidal_wave.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 21:54:49.000000 tidal_wave-2024.5.1/tidal_wave.egg-info/top_level.txt
```

### Comparing `tidal_wave-2024.4.3/LICENSE` & `tidal_wave-2024.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.4.3/PKG-INFO` & `tidal_wave-2024.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidal-wave
-Version: 2024.4.3
+Version: 2024.5.1
 Summary: A tool to wave at the TIDAL music service.
 Author-email: colinho <pypi@colin.technology>
 Maintainer-email: colinho <pypi@colin.technology>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -222,15 +222,15 @@
 License-File: LICENSE
 Requires-Dist: backoff==2.2.1
 Requires-Dist: cachecontrol==0.14.0
 Requires-Dist: dataclass-wizard==0.22.3
 Requires-Dist: ffmpeg-python==0.2.0
 Requires-Dist: mutagen==1.47.0
 Requires-Dist: m3u8==4.1.0
-Requires-Dist: platformdirs==4.2.0
+Requires-Dist: platformdirs==4.2.1
 Requires-Dist: pycryptodome==3.20.0
 Requires-Dist: requests[socks]==2.31.0
 Requires-Dist: typer==0.12.3
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI - Version](https://img.shields.io/pypi/v/tidal-wave)](https://pypi.org/project/tidal-wave/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/tidal-wave)](https://pypi.org/project/tidal-wave/)
@@ -314,20 +314,37 @@
 $ git clone --depth=1 https://github.com/ebb-earl-co/tidal-wave.git
 $ cd tidal-wave
 $ python3 -m venv .venv
 $ source .venv/bin/activate
 $ (.venv) pip install .
 ```
 ### PyInstaller executable
-These release artifacts are created with [PyInstaller](https://pyinstaller.org). It bundles Python 3.12.2, FFmpeg 7.0, and the `tidal-wave` program into one binary, licensed under the terms of FFmpeg: with the [GNU Lesser General Public License (LGPL) version 2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html). Installation is as simple as downloading the correct binary for your platform giving it execute permissions, and running it.
+The release artifacts for this project are created with [PyInstaller](https://pyinstaller.org). It bundles Python 3.12.2, FFmpeg 7.0, and the `tidal-wave` program into one binary, licensed under the terms of FFmpeg: with the [GNU Lesser General Public License (LGPL) version 2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html). Installation is as simple as downloading the correct binary for your platform giving it execute permissions, and running it. **Please make sure that the SHA256 checksum of the file that you have downloaded matches the corresponding `.sha256` file on the releases page!**
+#### On Unix-Like
 ```bash
 $ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_22.04_amd64
+$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_22.04_amd64.sha256
+$ sha256sum --check tidal-wave_ubuntu_22.04_amd64.sha256
+# ONLY CONTINUE IF THE OUTPUT IS THE FOLLOWING: 'tidal-wave_ubuntu_22.04_amd64.sha256: OK'
+# Otherwise, delete the downloaded binary and try to download it again
 $ chmod +x ./tidal-wave_ubuntu_22.04_amd64
 $ ./tidal-wave_ubuntu_22.04_amd64 --help
 ```
+#### On Windows
+```powershell
+# For just the lifetime of this PowerShell process, don't block the download from GitHub
+PS > Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope Process
+PS > Invoke-WebRequest "https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_windows.exe" -OutFile "tidal-wave_windows.exe"
+PS > Invoke-WebRequest "https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_windows.exe.sha256" -OutFile "tidal-wave_windows.exe.sha256"
+# Get the checksum value from the tidal-wave_windows.exe.sha256 file and compare it to the just-downloaded EXE
+# (Get-FileHash .\tidal-wave_windows.exe -Algorithm SHA256).Hash -eq (Get-Content .\tidal-wave_windows.exe.sha256)
+PS > (Get-FileHash .\tidal-wave_windows.exe -Algorithm SHA256).Hash -eq "e02f69eb850a98e6e1df2bc033fd12566cf27305421a36ec5372fd432ccc8e70"  # This checksum is from version 2024.4.3
+# ONLY CONTINUE IF THE OUTPUT OF THE PREVIOUS COMMAND IS 'True'
+PS > & .\tidal-wave_windows.exe --help
+```
 
 ### Docker
 Pull the image from GitHub container repo:
 ```bash
 $ docker pull ghcr.io/ebb-earl-co/tidal-wave:latest
 # Or, the main branch of this repository, which will be ahead of `latest`:
 $ docker pull ghcr.io/ebb-earl-co/tidal-wave:trunk
```

### Comparing `tidal_wave-2024.4.3/README.md` & `tidal_wave-2024.5.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -81,20 +81,37 @@
 $ git clone --depth=1 https://github.com/ebb-earl-co/tidal-wave.git
 $ cd tidal-wave
 $ python3 -m venv .venv
 $ source .venv/bin/activate
 $ (.venv) pip install .
 ```
 ### PyInstaller executable
-These release artifacts are created with [PyInstaller](https://pyinstaller.org). It bundles Python 3.12.2, FFmpeg 7.0, and the `tidal-wave` program into one binary, licensed under the terms of FFmpeg: with the [GNU Lesser General Public License (LGPL) version 2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html). Installation is as simple as downloading the correct binary for your platform giving it execute permissions, and running it.
+The release artifacts for this project are created with [PyInstaller](https://pyinstaller.org). It bundles Python 3.12.2, FFmpeg 7.0, and the `tidal-wave` program into one binary, licensed under the terms of FFmpeg: with the [GNU Lesser General Public License (LGPL) version 2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html). Installation is as simple as downloading the correct binary for your platform giving it execute permissions, and running it. **Please make sure that the SHA256 checksum of the file that you have downloaded matches the corresponding `.sha256` file on the releases page!**
+#### On Unix-Like
 ```bash
 $ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_22.04_amd64
+$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_22.04_amd64.sha256
+$ sha256sum --check tidal-wave_ubuntu_22.04_amd64.sha256
+# ONLY CONTINUE IF THE OUTPUT IS THE FOLLOWING: 'tidal-wave_ubuntu_22.04_amd64.sha256: OK'
+# Otherwise, delete the downloaded binary and try to download it again
 $ chmod +x ./tidal-wave_ubuntu_22.04_amd64
 $ ./tidal-wave_ubuntu_22.04_amd64 --help
 ```
+#### On Windows
+```powershell
+# For just the lifetime of this PowerShell process, don't block the download from GitHub
+PS > Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope Process
+PS > Invoke-WebRequest "https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_windows.exe" -OutFile "tidal-wave_windows.exe"
+PS > Invoke-WebRequest "https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_windows.exe.sha256" -OutFile "tidal-wave_windows.exe.sha256"
+# Get the checksum value from the tidal-wave_windows.exe.sha256 file and compare it to the just-downloaded EXE
+# (Get-FileHash .\tidal-wave_windows.exe -Algorithm SHA256).Hash -eq (Get-Content .\tidal-wave_windows.exe.sha256)
+PS > (Get-FileHash .\tidal-wave_windows.exe -Algorithm SHA256).Hash -eq "e02f69eb850a98e6e1df2bc033fd12566cf27305421a36ec5372fd432ccc8e70"  # This checksum is from version 2024.4.3
+# ONLY CONTINUE IF THE OUTPUT OF THE PREVIOUS COMMAND IS 'True'
+PS > & .\tidal-wave_windows.exe --help
+```
 
 ### Docker
 Pull the image from GitHub container repo:
 ```bash
 $ docker pull ghcr.io/ebb-earl-co/tidal-wave:latest
 # Or, the main branch of this repository, which will be ahead of `latest`:
 $ docker pull ghcr.io/ebb-earl-co/tidal-wave:trunk
```

### Comparing `tidal_wave-2024.4.3/pyproject.toml` & `tidal_wave-2024.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 [bdist_wheel]
 universal = 0  # Make the generated wheels have "py3" tag
 [project]
 name = "tidal-wave"
-version = "2024.4.3"
+version = "2024.5.1"
 description = "A tool to wave at the TIDAL music service."
 authors = [
     {name = "colinho", email = "pypi@colin.technology"}
 ]
 maintainers = [
     {name = "colinho", email = "pypi@colin.technology"}
 ]
@@ -30,15 +30,15 @@
 dependencies = [
     "backoff==2.2.1",
     "cachecontrol==0.14.0",
     "dataclass-wizard==0.22.3",
     "ffmpeg-python==0.2.0",
     "mutagen==1.47.0",
     "m3u8==4.1.0",
-    "platformdirs==4.2.0",
+    "platformdirs==4.2.1",
     "pycryptodome==3.20.0",
     "requests[socks]==2.31.0",
     "typer==0.12.3"
 ]
 [project.scripts]
 tidal-wave = "tidal_wave.main:app"
 [project.urls]
```

### Comparing `tidal_wave-2024.4.3/tidal_wave/album.py` & `tidal_wave-2024.5.1/tidal_wave/album.py`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.4.3/tidal_wave/artist.py` & `tidal_wave-2024.5.1/tidal_wave/artist.py`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.4.3/tidal_wave/dash.py` & `tidal_wave-2024.5.1/tidal_wave/dash.py`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.4.3/tidal_wave/hls.py` & `tidal_wave-2024.5.1/tidal_wave/hls.py`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.4.3/tidal_wave/login.py` & `tidal_wave-2024.5.1/tidal_wave/login.py`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.4.3/tidal_wave/main.py` & `tidal_wave-2024.5.1/tidal_wave/main.py`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.4.3/tidal_wave/media.py` & `tidal_wave-2024.5.1/tidal_wave/media.py`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.4.3/tidal_wave/mix.py` & `tidal_wave-2024.5.1/tidal_wave/mix.py`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.4.3/tidal_wave/models.py` & `tidal_wave-2024.5.1/tidal_wave/models.py`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.4.3/tidal_wave/oauth.py` & `tidal_wave-2024.5.1/tidal_wave/oauth.py`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.4.3/tidal_wave/playlist.py` & `tidal_wave-2024.5.1/tidal_wave/playlist.py`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.4.3/tidal_wave/requesting.py` & `tidal_wave-2024.5.1/tidal_wave/requesting.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,19 @@
                 )
                 return
             else:
                 logger.exception(he)
                 return
 
         if t:
-            json_name: str = f"{e}-{i}-{u.strip('/')}_{uuid4().hex}.json"
+            json_name: str = (
+                f"{e}-{i}-{u.strip('/')}_{uuid4().hex}.json"
+                if u != ""
+                else f"{e}-{i}_{uuid4().hex}.json"
+            )
             Path(json_name).write_text(
                 json.dumps(resp.json(), ensure_ascii=True, indent=4, sort_keys=True)
             )
 
         if cf:
             data = sc.from_dict({"credits": resp.json()})
         else:
```

### Comparing `tidal_wave-2024.4.3/tidal_wave/track.py` & `tidal_wave-2024.5.1/tidal_wave/track.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,15 +263,15 @@
         """This method writes a JPEG file with the name of each of
         self.metadata.artists to self.album_dir"""
         for a in self.metadata.artists:
             track_artist_image: Path = (
                 self.album_dir / f"{a.name.replace('..', '')}.jpg"
             )
             if not track_artist_image.exists():
-                download_artist_image(session, a, self.album_dir)
+                download_artist_image(session, a, self.album_dir, dimension=750)
 
     def save_artist_bio(self, session: Session):
         """This method writes a JSON file with the name of each of
         self.metadata.artists to self.album_dir"""
         for a in self.metadata.artists:
             track_artist_bio_json: Path = self.album_dir / f"{a.name}-bio.json"
             if not track_artist_bio_json.exists():
```

### Comparing `tidal_wave-2024.4.3/tidal_wave/utils.py` & `tidal_wave-2024.5.1/tidal_wave/utils.py`

 * *Files identical despite different names*

### Comparing `tidal_wave-2024.4.3/tidal_wave/video.py` & `tidal_wave-2024.5.1/tidal_wave/video.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,16 +96,17 @@
         self.artist_dir: Path = out_dir / self.metadata.artist.name
         self.artist_dir.mkdir(parents=True, exist_ok=True)
 
     def set_filename(self, out_dir: Path):
         """Set self.filename, which is constructed from self.metadata.name
         and self.stream.video_quality and self.codec"""
         self.filename: str = (
-            f"{self.metadata.name} [{self.stream.video_quality}].{self.codec}"
+            f"{self.metadata.name} [{self.metadata.id}].{self.codec}"
         )
+        self.filename: str = f"{self.metadata.name} [{self.metadata.id}].{self.codec}"
 
     def set_outfile(self):
         """Uses self.artist_dir and self.metadata and self.filename
         to craft the pathlib.Path object, self.outfile, that is a
         reference to where the video will be written on disk."""
         self.outfile: Path = self.artist_dir / self.filename
         self.absolute_outfile: str = str(self.outfile.absolute())
@@ -116,29 +117,29 @@
                 "and therefore will not be overwritten"
             )
             return
         else:
             return self.outfile
 
     def download(self, session: Session, out_dir: Path) -> Optional[Path]:
-        """Requests the HLS video files that constitute self.video_id.
+        """Requests the HLS video files that constitute self.urls.
         Writes HLS bytes to a temporary file, then uses FFmpeg to write the
         video data to self.outfile"""
         download_params: Dict[str, None] = {k: None for k in session.params}
         # self.outfile should already have been set by self.set_outfile()
+        request_headers: Dict[str, str] = (
+            {"sessionId": session.session_id}
+            if session.session_id is not None
+            else dict()
+        )
         logger.info(
             f"Writing video {self.video_id} to '{str(self.outfile.absolute())}'"
         )
 
         with temporary_file(suffix=".m2t") as tf:
-            request_headers: Dict[str, str] = (
-                {"sessionId": session.session_id}
-                if session.session_id is not None
-                else dict()
-            )
             for i, u in enumerate(self.urls, 1):
                 logger.debug(
                     f"\tRequesting part {i} of video {self.video_id}: {u.split('?')[0]}"
                 )
                 with session.get(
                     url=u, headers=request_headers, params=download_params
                 ) as download_response:
@@ -170,16 +171,17 @@
                     "metadata will not be added and format will stay as MPEG-TS"
                 )
 
         return self.outfile
 
     def craft_tags(self):
         """Using the TAG_MAPPING dictionary, write the correct values of
-        various metadata tags to the file. Videos are AVC1 + AAC MP4s, so see Kodi
-        reference: https://kodi.wiki/view/Video_file_tagging#Overview_and_Comparison"""
+        various metadata tags to the file. Videos are AVC1 video, AAC audio in
+        MP4 container, so see Kodi reference:
+        https://kodi.wiki/view/Video_file_tagging#Overview_and_Comparison"""
         tags = dict()
         tag_map = {k: v["m4a"] for k, v in TAG_MAPPING.items()}
 
         logger.info(
             f"Adding metadata tags to video {self.video_id} using "
             f"data returned from videos/{self.video_id} API endpoint"
         )
```

### Comparing `tidal_wave-2024.4.3/tidal_wave.egg-info/PKG-INFO` & `tidal_wave-2024.5.1/tidal_wave.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidal-wave
-Version: 2024.4.3
+Version: 2024.5.1
 Summary: A tool to wave at the TIDAL music service.
 Author-email: colinho <pypi@colin.technology>
 Maintainer-email: colinho <pypi@colin.technology>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -222,15 +222,15 @@
 License-File: LICENSE
 Requires-Dist: backoff==2.2.1
 Requires-Dist: cachecontrol==0.14.0
 Requires-Dist: dataclass-wizard==0.22.3
 Requires-Dist: ffmpeg-python==0.2.0
 Requires-Dist: mutagen==1.47.0
 Requires-Dist: m3u8==4.1.0
-Requires-Dist: platformdirs==4.2.0
+Requires-Dist: platformdirs==4.2.1
 Requires-Dist: pycryptodome==3.20.0
 Requires-Dist: requests[socks]==2.31.0
 Requires-Dist: typer==0.12.3
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI - Version](https://img.shields.io/pypi/v/tidal-wave)](https://pypi.org/project/tidal-wave/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/tidal-wave)](https://pypi.org/project/tidal-wave/)
@@ -314,20 +314,37 @@
 $ git clone --depth=1 https://github.com/ebb-earl-co/tidal-wave.git
 $ cd tidal-wave
 $ python3 -m venv .venv
 $ source .venv/bin/activate
 $ (.venv) pip install .
 ```
 ### PyInstaller executable
-These release artifacts are created with [PyInstaller](https://pyinstaller.org). It bundles Python 3.12.2, FFmpeg 7.0, and the `tidal-wave` program into one binary, licensed under the terms of FFmpeg: with the [GNU Lesser General Public License (LGPL) version 2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html). Installation is as simple as downloading the correct binary for your platform giving it execute permissions, and running it.
+The release artifacts for this project are created with [PyInstaller](https://pyinstaller.org). It bundles Python 3.12.2, FFmpeg 7.0, and the `tidal-wave` program into one binary, licensed under the terms of FFmpeg: with the [GNU Lesser General Public License (LGPL) version 2.1](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html). Installation is as simple as downloading the correct binary for your platform giving it execute permissions, and running it. **Please make sure that the SHA256 checksum of the file that you have downloaded matches the corresponding `.sha256` file on the releases page!**
+#### On Unix-Like
 ```bash
 $ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_22.04_amd64
+$ wget https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_ubuntu_22.04_amd64.sha256
+$ sha256sum --check tidal-wave_ubuntu_22.04_amd64.sha256
+# ONLY CONTINUE IF THE OUTPUT IS THE FOLLOWING: 'tidal-wave_ubuntu_22.04_amd64.sha256: OK'
+# Otherwise, delete the downloaded binary and try to download it again
 $ chmod +x ./tidal-wave_ubuntu_22.04_amd64
 $ ./tidal-wave_ubuntu_22.04_amd64 --help
 ```
+#### On Windows
+```powershell
+# For just the lifetime of this PowerShell process, don't block the download from GitHub
+PS > Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope Process
+PS > Invoke-WebRequest "https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_windows.exe" -OutFile "tidal-wave_windows.exe"
+PS > Invoke-WebRequest "https://github.com/ebb-earl-co/tidal-wave/releases/latest/download/tidal-wave_windows.exe.sha256" -OutFile "tidal-wave_windows.exe.sha256"
+# Get the checksum value from the tidal-wave_windows.exe.sha256 file and compare it to the just-downloaded EXE
+# (Get-FileHash .\tidal-wave_windows.exe -Algorithm SHA256).Hash -eq (Get-Content .\tidal-wave_windows.exe.sha256)
+PS > (Get-FileHash .\tidal-wave_windows.exe -Algorithm SHA256).Hash -eq "e02f69eb850a98e6e1df2bc033fd12566cf27305421a36ec5372fd432ccc8e70"  # This checksum is from version 2024.4.3
+# ONLY CONTINUE IF THE OUTPUT OF THE PREVIOUS COMMAND IS 'True'
+PS > & .\tidal-wave_windows.exe --help
+```
 
 ### Docker
 Pull the image from GitHub container repo:
 ```bash
 $ docker pull ghcr.io/ebb-earl-co/tidal-wave:latest
 # Or, the main branch of this repository, which will be ahead of `latest`:
 $ docker pull ghcr.io/ebb-earl-co/tidal-wave:trunk
```

### Comparing `tidal_wave-2024.4.3/tidal_wave.egg-info/SOURCES.txt` & `tidal_wave-2024.5.1/tidal_wave.egg-info/SOURCES.txt`

 * *Files identical despite different names*


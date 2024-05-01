# Comparing `tmp/golpy-0.2.0.tar.gz` & `tmp/golpy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golpy-0.2.0.tar", last modified: Wed Feb 17 14:56:18 2021, max compression
+gzip compressed data, was "golpy-0.3.0.tar", max compression
```

## Comparing `golpy-0.2.0.tar` & `golpy-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2021-02-13 13:46:02.591009 golpy-0.2.0/LICENSE
--rw-r--r--   0        0        0     2145 2021-02-17 14:56:01.333974 golpy-0.2.0/README.md
--rw-r--r--   0        0        0     9085 2021-02-17 14:54:06.918158 golpy-0.2.0/golpy/__init__.py
--rw-r--r--   0        0        0       27 2021-02-15 13:48:11.709379 golpy-0.2.0/golpy/__main__.py
--rw-r--r--   0        0        0      680 2021-01-31 14:51:48.548154 golpy-0.2.0/golpy/util.py
--rw-r--r--   0        0        0      604 2021-02-17 14:54:50.941165 golpy-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2992 2021-02-17 14:56:18.738678 golpy-0.2.0/setup.py
--rw-r--r--   0        0        0     2802 2021-02-17 14:56:18.739056 golpy-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-01 03:33:42.692828 golpy-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2263 2024-05-01 03:45:56.093138 golpy-0.3.0/README.md
+-rw-r--r--   0        0        0     6148 2024-05-01 03:48:18.885551 golpy-0.3.0/golpy/.DS_Store
+-rw-r--r--   0        0        0     9066 2024-05-01 04:28:58.363209 golpy-0.3.0/golpy/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-01 03:33:42.695033 golpy-0.3.0/golpy/__main__.py
+-rw-r--r--   0        0        0      656 2024-05-01 03:47:28.017278 golpy-0.3.0/golpy/util.py
+-rw-r--r--   0        0        0      603 2024-05-01 03:56:46.877947 golpy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3025 1970-01-01 00:00:00.000000 golpy-0.3.0/PKG-INFO
```

### Comparing `golpy-0.2.0/LICENSE` & `golpy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `golpy-0.2.0/README.md` & `golpy-0.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,56 @@
+Metadata-Version: 2.1
+Name: golpy
+Version: 0.3.0
+Summary: Efficient Conway's Game of Life using NumPy
+Home-page: https://github.com/zeta611/py-game-of-life
+License: MIT
+Keywords: Game of Life
+Author: Jay Lee
+Author-email: jaeho.lee@snu.ac.kr
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: Pillow (>=10.3.0,<11.0.0)
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Project-URL: Repository, https://github.com/zeta611/py-game-of-life
+Description-Content-Type: text/markdown
+
 # GoLPy
+
 [![GitHub
 license](https://img.shields.io/github/license/Zeta611/golpy?style=flat-square)](https://github.com/Zeta611/golpy/blob/master/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/golpy?style=flat-square)](https://pypi.org/project/golpy/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/psf/black)
 
 GoLPy is an efficient Conway's Game of Life implemented in Python using NumPy.
 
 ## Example Output
+
 The following GIF can be generated using the command:
+
 ```sh
 life --demo glidergun --out glider_gun.gif --ppc 10 --pos TL -W60 -H40
 ```
 
 ![The Gosper Glider Gun](glider_gun.gif)
 
-## Usage
+## Installation
+
+```sh
+pip install golpy
 ```
+
+## Usage
+
+```sh
 usage: life [-h] (-i GRID_INPUT | -d DEMO) [-o FILE | --debug-print]
             [-W WIDTH] [-H HEIGHT] [-M MAX_GEN] [--ppc PIXELS] [-P POSITION]
             [-p]
 
 optional arguments:
   -h, --help            show this help message and exit
   -i GRID_INPUT, --in GRID_INPUT
@@ -41,24 +72,33 @@
   -P POSITION, --pos POSITION
                         One of 'C', 'T', 'B', 'L', 'R', 'TL', 'TR', 'BL', and
                         'BR'
 
   -p, --profile         Measure the performance
 ```
 
-## Input Format
+To use without installing,
+
+```sh
+python -m golpy # ...
 ```
+
+## Input Format
+
+```txt
 ........................O
 ......................O.O
 ............OO......OO............OO
 ...........O...O....OO............OO
 OO........O.....O...OO
 OO........O...O.OO....O.O
 ..........O.....O.......O
 ...........O...O
 ............OO
 ```
 
 Use `.` for a dead cell, `O` (`chr(79)`) for a live cell.
 
 ## License
+
 [MIT](LICENSE)
+
```

### Comparing `golpy-0.2.0/golpy/__init__.py` & `golpy-0.3.0/golpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 import functools
 import textwrap
 from pathlib import Path
-from typing import Callable, Dict, List, Tuple
+from typing import Callable
 
 import numpy as np
 from PIL import Image
 
 from .util import timeit
 
 
@@ -121,29 +121,29 @@
             else:
                 print("□", end="")
         print()
 
 
 @timeit()
 def parse_grid(
-    text: str, size: Tuple[int, int], pos: str = "C", live: str = "O"
+    text: str, size: tuple[int, int], pos: str = "C", live: str = "O"
 ) -> np.ndarray:
     lines = textwrap.dedent(text).strip().splitlines()
     text_width = max(len(line) for line in lines)
     text_height = len(lines)
 
     width, height = size
     if width < text_width or height < text_height:
         raise ValueError(
             f"given text of size {(text_width, text_height)} larger than grid size {size}"
         )
 
     grid = np.zeros((height, width), dtype="uint8")
 
-    pos_idx: Dict[str, Tuple[int, int]] = {
+    pos_idx: dict[str, tuple[int, int]] = {
         "C": (height // 2 - text_height // 2, width // 2 - text_width // 2),
         "T": (0, width // 2 - text_width // 2),
         "B": (height - text_height, width // 2 - text_width // 2),
         "L": (height // 2 - text_height // 2, 0),
         "R": (height // 2 - text_height // 2, width - text_width),
         "TL": (0, 0),
         "TR": (0, width - text_width),
@@ -162,15 +162,15 @@
     return grid
 
 
 @timeit()
 def add_grid_frame(
     grid: np.ndarray,
     generation: int,
-    grid_frames: List[np.ndarray],
+    grid_frames: list[np.ndarray],
     pixels_per_cell: int,
 ) -> None:
     """Add the grid to the grid_frames"""
 
     arr_grid = enlarge_image(grid * 255, pixels_per_cell)
     image = Image.fromarray(arr_grid, mode="L").convert("P")
     grid_frames.append(image)
@@ -181,26 +181,26 @@
     """Enlarges each pixel in the image to a ratio * ratio square block."""
 
     return np.kron(image, np.ones((ratio, ratio), dtype="uint8"))
 
 
 @timeit()
 def save_frames(
-    grid_frames: List[Image.Image], filename: str, duration: int = 50
+    grid_frames: list[Image.Image], filename: str, duration: int = 50
 ) -> None:
     grid_frames[0].save(
         filename,
         save_all=True,
         append_images=grid_frames[1:],
         duration=duration,
         loop=0,
     )
 
 
-def get_demo(name: str, size: Tuple[int, int], pos: str = "C") -> np.ndarray:
+def get_demo(name: str, size: tuple[int, int], pos: str = "C") -> np.ndarray:
     if name == "random":
         return np.random.randint(0, 2, size, dtype="uint8")
 
     demos = {
         "glidergun": lambda: parse_grid(
             """\
     ........................O
@@ -317,15 +317,15 @@
 
     if in_file := getattr(args, "in"):
         grid = parse_grid(Path(in_file).read_text(), size, pos)
     else:  # demo mode
         grid = get_demo(args.demo, size, pos)
 
     # Run Game of Life
-    grid_frames: List[Image.Image] = []
+    grid_frames: list[Image.Image] = []
 
     if args.debug_print:
         driver(grid, handler=grid_print, max_gen=max_gen)
     else:
         driver(
             grid,
             handler=functools.partial(
```

### Comparing `golpy-0.2.0/golpy/util.py` & `golpy-0.3.0/golpy/util.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import time
 from functools import wraps
-from typing import Dict
 
 
 class timeit:
-    records: Dict[str, float] = {}
+    records: dict[str, float] = {}
     on = False
 
     def __call__(self, func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             if not self.on:
                 return func(*args, **kwargs)
```

### Comparing `golpy-0.2.0/pyproject.toml` & `golpy-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "golpy"
-version = "0.2.0"
+version = "0.3.0"
 description = "Efficient Conway's Game of Life using NumPy"
 authors = ["Jay Lee <jaeho.lee@snu.ac.kr>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/zeta611/py-game-of-life"
 repository = "https://github.com/zeta611/py-game-of-life"
 keywords = ["Game of Life"]
 
 [tool.poetry.dependencies]
-python = "^3.8"
-Pillow = "^8.1.0"
-numpy = "^1.20.1"
+python = "^3.9"
+Pillow = "^10.3.0"
+numpy = "^1.26.4"
 
 [tool.poetry.dev-dependencies]
-black = "^20.8b1"
+black = "^24.4"
 
 [tool.poetry.scripts]
 life = "golpy.__init__:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```


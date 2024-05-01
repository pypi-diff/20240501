# Comparing `tmp/avenger-0.0.3.tar.gz` & `tmp/avenger-0.0.4.tar.gz`

## Comparing `avenger-0.0.3.tar` & `avenger-0.0.4.tar`

### file list

```diff
@@ -1,75 +1,76 @@
--rw-r--r--   0      501       20     1175 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-wgpu/Cargo.toml
--rw-r--r--   0      501       20       78 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-wgpu/README.md
--rw-r--r--   0      501       20    27626 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-wgpu/src/canvas.rs
--rw-r--r--   0      501       20     1145 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-wgpu/src/error.rs
--rw-r--r--   0      501       20      188 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-wgpu/src/lib.rs
--rw-r--r--   0      501       20    19147 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-wgpu/src/marks/cosmic.rs
--rw-r--r--   0      501       20     6491 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-wgpu/src/marks/gradient.rs
--rw-r--r--   0      501       20     4996 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-wgpu/src/marks/image.rs
--rw-r--r--   0      501       20    12646 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-wgpu/src/marks/instanced_mark.rs
--rw-r--r--   0      501       20      151 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-wgpu/src/marks/mod.rs
--rw-r--r--   0      501       20    73975 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-wgpu/src/marks/multi.rs
--rw-r--r--   0      501       20     8508 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-wgpu/src/marks/multi.wgsl
--rw-r--r--   0      501       20     8857 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-wgpu/src/marks/symbol.rs
--rw-r--r--   0      501       20     3130 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-wgpu/src/marks/symbol.wgsl
--rw-r--r--   0      501       20     1710 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-wgpu/src/marks/text.rs
--rw-r--r--   0      501       20     1329 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-wgpu/src/util.rs
--rw-r--r--   0      501       20    10498 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-wgpu/tests/test_image_baselines.rs
--rw-r--r--   0      501       20      489 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger/Cargo.toml
--rw-r--r--   0      501       20      129 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger/README.md
--rw-r--r--   0      501       20      396 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger/src/error.rs
--rw-r--r--   0      501       20       51 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger/src/lib.rs
--rw-r--r--   0      501       20     3689 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger/src/marks/arc.rs
--rw-r--r--   0      501       20     2414 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger/src/marks/area.rs
--rw-r--r--   0      501       20     2962 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger/src/marks/group.rs
--rw-r--r--   0      501       20     2212 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger/src/marks/image.rs
--rw-r--r--   0      501       20     1634 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger/src/marks/line.rs
--rw-r--r--   0      501       20     1329 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger/src/marks/mark.rs
--rw-r--r--   0      501       20      187 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger/src/marks/mod.rs
--rw-r--r--   0      501       20     2882 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger/src/marks/path.rs
--rw-r--r--   0      501       20     3831 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger/src/marks/rect.rs
--rw-r--r--   0      501       20     2873 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger/src/marks/rule.rs
--rw-r--r--   0      501       20     4506 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger/src/marks/symbol.rs
--rw-r--r--   0      501       20     5005 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger/src/marks/text.rs
--rw-r--r--   0      501       20     1551 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger/src/marks/trail.rs
--rw-r--r--   0      501       20     3215 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger/src/marks/value.rs
--rw-r--r--   0      501       20      249 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger/src/scene_graph.rs
--rw-r--r--   0      501       20       89 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger/tests/test_scene_graph.rs
--rw-r--r--   0      501       20     1101 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-vega/Cargo.toml
--rw-r--r--   0      501       20      109 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-vega/README.md
--rw-r--r--   0      501       20     1490 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-vega/src/error.rs
--rw-r--r--   0      501       20      757 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-vega/src/image/mod.rs
--rw-r--r--   0      501       20     1504 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-vega/src/image/reqwest_fetcher.rs
--rw-r--r--   0      501       20     1724 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-vega/src/image/svg.rs
--rw-r--r--   0      501       20      131 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-vega/src/lib.rs
--rw-r--r--   0      501       20     5463 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-vega/src/marks/arc.rs
--rw-r--r--   0      501       20     4329 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-vega/src/marks/area.rs
--rw-r--r--   0      501       20     4379 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-vega/src/marks/group.rs
--rw-r--r--   0      501       20     3727 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-vega/src/marks/image.rs
--rw-r--r--   0      501       20     3183 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-vega/src/marks/line.rs
--rw-r--r--   0      501       20     1522 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-vega/src/marks/mark.rs
--rw-r--r--   0      501       20      203 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-vega/src/marks/mod.rs
--rw-r--r--   0      501       20     5562 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-vega/src/marks/path.rs
--rw-r--r--   0      501       20     4275 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-vega/src/marks/rect.rs
--rw-r--r--   0      501       20     4350 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-vega/src/marks/rule.rs
--rw-r--r--   0      501       20     4955 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-vega/src/marks/shape.rs
--rw-r--r--   0      501       20    13941 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-vega/src/marks/symbol.rs
--rw-r--r--   0      501       20     6368 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-vega/src/marks/text.rs
--rw-r--r--   0      501       20     2763 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-vega/src/marks/trail.rs
--rw-r--r--   0      501       20     6163 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-vega/src/marks/values.rs
--rw-r--r--   0      501       20      744 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-vega/src/scene_graph.rs
--rw-r--r--   0      501       20      757 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-vega/tests/test_parsing.rs
--rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 avenger-0.0.3/avenger-python/Cargo.toml
--rw-r--r--   0      501       20     1453 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-python/LICENSE
--rw-r--r--   0      501       20     2375 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-python/README.md
--rw-r--r--   0      501       20      172 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-python/avenger/__init__.py
--rw-r--r--   0      501       20     1663 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-python/avenger/altair_utils.py
--rw-r--r--   0      501       20     2468 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger-python/src/lib.rs
--rw-r--r--   0      501       20   190938 2024-02-15 15:00:57.000000 avenger-0.0.3/Cargo.lock
--rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 avenger-0.0.3/Cargo.toml
--rw-r--r--   0        0        0      436 1970-01-01 00:00:00.000000 avenger-0.0.3/pyproject.toml
--rw-r--r--   0      501       20      172 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger/__init__.py
--rw-r--r--   0      501       20     1663 2024-02-15 15:00:57.000000 avenger-0.0.3/avenger/altair_utils.py
--rw-r--r--   0      501       20     2375 2024-02-15 15:00:57.000000 avenger-0.0.3/README.md
--rw-r--r--   0      501       20     1453 2024-02-15 15:00:57.000000 avenger-0.0.3/LICENSE
--rw-r--r--   0        0        0     2585 1970-01-01 00:00:00.000000 avenger-0.0.3/PKG-INFO
+-rw-r--r--   0      501       20     1485 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-wgpu/Cargo.toml
+-rw-r--r--   0      501       20       78 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-wgpu/README.md
+-rw-r--r--   0      501       20    28421 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-wgpu/src/canvas.rs
+-rw-r--r--   0      501       20     1800 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-wgpu/src/error.rs
+-rw-r--r--   0      501       20     6818 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-wgpu/src/html_canvas.rs
+-rw-r--r--   0      501       20      273 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-wgpu/src/lib.rs
+-rw-r--r--   0      501       20    11018 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-wgpu/src/marks/cosmic.rs
+-rw-r--r--   0      501       20     6491 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-wgpu/src/marks/gradient.rs
+-rw-r--r--   0      501       20     4996 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-wgpu/src/marks/image.rs
+-rw-r--r--   0      501       20    12845 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-wgpu/src/marks/instanced_mark.rs
+-rw-r--r--   0      501       20      151 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-wgpu/src/marks/mod.rs
+-rw-r--r--   0      501       20    83346 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-wgpu/src/marks/multi.rs
+-rw-r--r--   0      501       20     8946 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-wgpu/src/marks/multi.wgsl
+-rw-r--r--   0      501       20     8759 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-wgpu/src/marks/symbol.rs
+-rw-r--r--   0      501       20     3130 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-wgpu/src/marks/symbol.wgsl
+-rw-r--r--   0      501       20    15441 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-wgpu/src/marks/text.rs
+-rw-r--r--   0      501       20     1329 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-wgpu/src/util.rs
+-rw-r--r--   0      501       20    10704 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-wgpu/tests/test_image_baselines.rs
+-rw-r--r--   0      501       20      533 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger/Cargo.toml
+-rw-r--r--   0      501       20      129 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger/README.md
+-rw-r--r--   0      501       20      735 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger/src/error.rs
+-rw-r--r--   0      501       20       51 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger/src/lib.rs
+-rw-r--r--   0      501       20     3689 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger/src/marks/arc.rs
+-rw-r--r--   0      501       20     2414 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger/src/marks/area.rs
+-rw-r--r--   0      501       20     4672 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger/src/marks/group.rs
+-rw-r--r--   0      501       20     3031 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger/src/marks/image.rs
+-rw-r--r--   0      501       20     1634 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger/src/marks/line.rs
+-rw-r--r--   0      501       20     1329 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger/src/marks/mark.rs
+-rw-r--r--   0      501       20      187 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger/src/marks/mod.rs
+-rw-r--r--   0      501       20     2882 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger/src/marks/path.rs
+-rw-r--r--   0      501       20     3831 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger/src/marks/rect.rs
+-rw-r--r--   0      501       20     2873 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger/src/marks/rule.rs
+-rw-r--r--   0      501       20    10808 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger/src/marks/symbol.rs
+-rw-r--r--   0      501       20     5005 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger/src/marks/text.rs
+-rw-r--r--   0      501       20     1551 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger/src/marks/trail.rs
+-rw-r--r--   0      501       20     3215 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger/src/marks/value.rs
+-rw-r--r--   0      501       20      249 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger/src/scene_graph.rs
+-rw-r--r--   0      501       20       89 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger/tests/test_scene_graph.rs
+-rw-r--r--   0      501       20     1101 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-vega/Cargo.toml
+-rw-r--r--   0      501       20      109 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-vega/README.md
+-rw-r--r--   0      501       20     1490 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-vega/src/error.rs
+-rw-r--r--   0      501       20      757 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-vega/src/image/mod.rs
+-rw-r--r--   0      501       20     1504 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-vega/src/image/reqwest_fetcher.rs
+-rw-r--r--   0      501       20     1724 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-vega/src/image/svg.rs
+-rw-r--r--   0      501       20      131 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-vega/src/lib.rs
+-rw-r--r--   0      501       20     5495 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-vega/src/marks/arc.rs
+-rw-r--r--   0      501       20     4361 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-vega/src/marks/area.rs
+-rw-r--r--   0      501       20     6737 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-vega/src/marks/group.rs
+-rw-r--r--   0      501       20     3759 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-vega/src/marks/image.rs
+-rw-r--r--   0      501       20     3215 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-vega/src/marks/line.rs
+-rw-r--r--   0      501       20     1522 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-vega/src/marks/mark.rs
+-rw-r--r--   0      501       20      203 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-vega/src/marks/mod.rs
+-rw-r--r--   0      501       20     5626 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-vega/src/marks/path.rs
+-rw-r--r--   0      501       20     4307 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-vega/src/marks/rect.rs
+-rw-r--r--   0      501       20     4382 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-vega/src/marks/rule.rs
+-rw-r--r--   0      501       20     5019 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-vega/src/marks/shape.rs
+-rw-r--r--   0      501       20     8093 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-vega/src/marks/symbol.rs
+-rw-r--r--   0      501       20     6400 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-vega/src/marks/text.rs
+-rw-r--r--   0      501       20     2795 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-vega/src/marks/trail.rs
+-rw-r--r--   0      501       20     6163 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-vega/src/marks/values.rs
+-rw-r--r--   0      501       20      749 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-vega/src/scene_graph.rs
+-rw-r--r--   0      501       20      757 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-vega/tests/test_parsing.rs
+-rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 avenger-0.0.4/avenger-python/Cargo.toml
+-rw-r--r--   0      501       20     1453 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-python/LICENSE
+-rw-r--r--   0      501       20     2375 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-python/README.md
+-rw-r--r--   0      501       20      172 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-python/avenger/__init__.py
+-rw-r--r--   0      501       20     3532 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-python/avenger/altair_utils.py
+-rw-r--r--   0      501       20     2547 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger-python/src/lib.rs
+-rw-r--r--   0      501       20   195804 2024-04-30 22:52:02.000000 avenger-0.0.4/Cargo.lock
+-rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 avenger-0.0.4/Cargo.toml
+-rw-r--r--   0        0        0      496 1970-01-01 00:00:00.000000 avenger-0.0.4/pyproject.toml
+-rw-r--r--   0      501       20      172 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger/__init__.py
+-rw-r--r--   0      501       20     3532 2024-04-30 22:52:02.000000 avenger-0.0.4/avenger/altair_utils.py
+-rw-r--r--   0      501       20     2375 2024-04-30 22:52:02.000000 avenger-0.0.4/README.md
+-rw-r--r--   0      501       20     1453 2024-04-30 22:52:02.000000 avenger-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2585 1970-01-01 00:00:00.000000 avenger-0.0.4/PKG-INFO
```

### Comparing `avenger-0.0.3/avenger-wgpu/src/canvas.rs` & `avenger-0.0.4/avenger-wgpu/src/canvas.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 use image::imageops::crop_imm;
+use std::sync::Arc;
 use wgpu::{
     Adapter, Buffer, BufferAddress, BufferDescriptor, BufferUsages, CommandBuffer,
     CommandEncoderDescriptor, Device, DeviceDescriptor, Extent3d, ImageCopyBuffer,
     ImageCopyTexture, ImageDataLayout, LoadOp, MapMode, Operations, Origin3d, PowerPreference,
     Queue, RenderPassColorAttachment, RenderPassDescriptor, RequestAdapterOptions, StoreOp,
     Surface, SurfaceConfiguration, Texture, TextureAspect, TextureDescriptor, TextureDimension,
     TextureFormat, TextureFormatFeatureFlags, TextureUsages, TextureView, TextureViewDescriptor,
@@ -11,54 +12,32 @@
 use winit::event::WindowEvent;
 use winit::window::Window;
 
 use crate::error::AvengerWgpuError;
 use crate::marks::instanced_mark::InstancedMarkRenderer;
 use crate::marks::multi::MultiMarkRenderer;
 use crate::marks::symbol::SymbolShader;
+use crate::marks::text::TextAtlasBuilderTrait;
 use avenger::marks::arc::ArcMark;
 use avenger::marks::area::AreaMark;
-use avenger::marks::group::GroupBounds;
+use avenger::marks::group::Clip;
 use avenger::marks::image::ImageMark;
 use avenger::marks::line::LineMark;
 use avenger::marks::path::PathMark;
 use avenger::marks::trail::TrailMark;
 use avenger::{
     marks::group::SceneGroup, marks::mark::SceneMark, marks::rect::RectMark, marks::rule::RuleMark,
     marks::symbol::SymbolMark, marks::text::TextMark, scene_graph::SceneGraph,
 };
 
 pub enum MarkRenderer {
     Instanced(InstancedMarkRenderer),
     Multi(Box<MultiMarkRenderer>),
 }
 
-#[derive(Clone, Copy)]
-pub struct ClipRect {
-    pub x: u32,
-    pub y: u32,
-    pub width: u32,
-    pub height: u32,
-}
-
-impl ClipRect {
-    pub fn maybe_from_group_bounds(scale: f32, bounds: GroupBounds, clip: bool) -> Option<Self> {
-        if let (true, Some(width), Some(height)) = (clip, bounds.width, bounds.height) {
-            Some(Self {
-                x: (bounds.x * scale) as u32,
-                y: (bounds.y * scale) as u32,
-                width: (width * scale) as u32,
-                height: (height * scale) as u32,
-            })
-        } else {
-            None
-        }
-    }
-}
-
 #[derive(Debug, Copy, Clone)]
 pub struct CanvasDimensions {
     pub size: [f32; 2],
     pub scale: f32,
 }
 
 impl CanvasDimensions {
@@ -74,14 +53,21 @@
         winit::dpi::PhysicalSize {
             width: self.to_physical_width(),
             height: self.to_physical_height(),
         }
     }
 }
 
+pub type TextBuildCtor = Arc<fn() -> Box<dyn TextAtlasBuilderTrait>>;
+
+#[derive(Default)]
+pub struct CanvasConfig {
+    pub text_builder_ctor: Option<TextBuildCtor>,
+}
+
 pub trait Canvas {
     fn add_mark_renderer(&mut self, mark_renderer: MarkRenderer);
     fn clear_mark_renderer(&mut self);
     fn device(&self) -> &Device;
     fn queue(&self) -> &Queue;
     fn dimensions(&self) -> CanvasDimensions;
 
@@ -90,225 +76,237 @@
     fn sample_count(&self) -> u32;
 
     fn get_multi_renderer(&mut self) -> &mut MultiMarkRenderer;
 
     fn add_arc_mark(
         &mut self,
         mark: &ArcMark,
-        group_bounds: GroupBounds,
+        origin: [f32; 2],
+        group_clip: &Clip,
     ) -> Result<(), AvengerWgpuError> {
-        self.get_multi_renderer().add_arc_mark(mark, group_bounds)?;
+        self.get_multi_renderer()
+            .add_arc_mark(mark, origin, group_clip)?;
         Ok(())
     }
 
     fn add_path_mark(
         &mut self,
         mark: &PathMark,
-        group_bounds: GroupBounds,
+        origin: [f32; 2],
+        group_clip: &Clip,
     ) -> Result<(), AvengerWgpuError> {
         self.get_multi_renderer()
-            .add_path_mark(mark, group_bounds)?;
+            .add_path_mark(mark, origin, group_clip)?;
         Ok(())
     }
 
     fn add_line_mark(
         &mut self,
         mark: &LineMark,
-        group_bounds: GroupBounds,
+        origin: [f32; 2],
+        group_clip: &Clip,
     ) -> Result<(), AvengerWgpuError> {
         self.get_multi_renderer()
-            .add_line_mark(mark, group_bounds)?;
+            .add_line_mark(mark, origin, group_clip)?;
         Ok(())
     }
 
     fn add_trail_mark(
         &mut self,
         mark: &TrailMark,
-        group_bounds: GroupBounds,
+        origin: [f32; 2],
+        group_clip: &Clip,
     ) -> Result<(), AvengerWgpuError> {
         self.get_multi_renderer()
-            .add_trail_mark(mark, group_bounds)?;
+            .add_trail_mark(mark, origin, group_clip)?;
         Ok(())
     }
 
     fn add_area_mark(
         &mut self,
         mark: &AreaMark,
-        group_bounds: GroupBounds,
+        origin: [f32; 2],
+        group_clip: &Clip,
     ) -> Result<(), AvengerWgpuError> {
         self.get_multi_renderer()
-            .add_area_mark(mark, group_bounds)?;
+            .add_area_mark(mark, origin, group_clip)?;
         Ok(())
     }
 
     fn add_symbol_mark(
         &mut self,
         mark: &SymbolMark,
-        group_bounds: GroupBounds,
+        origin: [f32; 2],
+        group_clip: &Clip,
     ) -> Result<(), AvengerWgpuError> {
-        if mark.len >= 10000 && mark.gradients.is_empty() {
+        if mark.len >= 10000
+            && mark.gradients.is_empty()
+            && matches!(group_clip, Clip::None | Clip::Rect { .. })
+        {
             self.add_mark_renderer(MarkRenderer::Instanced(InstancedMarkRenderer::new(
                 self.device(),
                 self.texture_format(),
                 self.sample_count(),
                 Box::new(SymbolShader::from_symbol_mark(
                     mark,
                     self.dimensions(),
-                    group_bounds,
+                    origin,
                 )?),
-                ClipRect::maybe_from_group_bounds(self.dimensions().scale, group_bounds, mark.clip),
+                group_clip.maybe_clip(mark.clip),
+                self.dimensions().scale,
             )));
         } else {
             self.get_multi_renderer()
-                .add_symbol_mark(mark, group_bounds)?;
+                .add_symbol_mark(mark, origin, group_clip)?;
         }
 
         Ok(())
     }
 
     fn add_rect_mark(
         &mut self,
         mark: &RectMark,
-        group_bounds: GroupBounds,
+        origin: [f32; 2],
+        group_clip: &Clip,
     ) -> Result<(), AvengerWgpuError> {
         self.get_multi_renderer()
-            .add_rect_mark(mark, group_bounds)?;
+            .add_rect_mark(mark, origin, group_clip)?;
         Ok(())
     }
 
     fn add_rule_mark(
         &mut self,
         mark: &RuleMark,
-        group_bounds: GroupBounds,
+        origin: [f32; 2],
+        group_clip: &Clip,
     ) -> Result<(), AvengerWgpuError> {
         self.get_multi_renderer()
-            .add_rule_mark(mark, group_bounds)?;
+            .add_rule_mark(mark, origin, group_clip)?;
         Ok(())
     }
 
     fn add_text_mark(
         &mut self,
         mark: &TextMark,
-        group_bounds: GroupBounds,
+        origin: [f32; 2],
+        group_clip: &Clip,
     ) -> Result<(), AvengerWgpuError> {
-        cfg_if::cfg_if! {
-            if #[cfg(feature = "cosmic-text")] {
-                self.get_multi_renderer().add_text_mark(mark, group_bounds)?;
-                Ok(())
-            } else {
-                Err(AvengerWgpuError::TextNotEnabled("Use the cosmic-text feature flag to enable text".to_string()))
-            }
-        }
+        self.get_multi_renderer()
+            .add_text_mark(mark, origin, group_clip)?;
+        Ok(())
     }
 
     fn add_image_mark(
         &mut self,
         mark: &ImageMark,
-        group_bounds: GroupBounds,
+        origin: [f32; 2],
+        group_clip: &Clip,
     ) -> Result<(), AvengerWgpuError> {
         self.get_multi_renderer()
-            .add_image_mark(mark, group_bounds)?;
+            .add_image_mark(mark, origin, group_clip)?;
         Ok(())
     }
 
     fn add_group_mark(
         &mut self,
         group: &SceneGroup,
-        group_bounds: GroupBounds,
+        parent_origin: [f32; 2],
+        parent_clip: &Clip,
     ) -> Result<(), AvengerWgpuError> {
         // Maybe add rect around group boundary
-        if let Some(rect) = group.make_rect() {
-            self.add_rect_mark(&rect, group_bounds)?;
+        if let Some(rect) = group.make_path_mark() {
+            self.add_path_mark(&rect, parent_origin, &group.clip)?;
         }
 
         // Add groups in order of zindex
         let zindex = group.marks.iter().map(|m| m.zindex()).collect::<Vec<_>>();
         let mut indices: Vec<usize> = (0..zindex.len()).collect();
         indices.sort_by_key(|i| zindex[*i].unwrap_or(0));
 
-        // Compute new group bounds
-        let group_bounds = GroupBounds {
-            x: group_bounds.x + group.bounds.x,
-            y: group_bounds.y + group.bounds.y,
-            ..group.bounds
+        // Compute new origin
+        let origin = [
+            parent_origin[0] + group.origin[0],
+            parent_origin[1] + group.origin[1],
+        ];
+
+        // Compute new clip
+        let clip = if let Clip::None = group.clip {
+            // No clip defined for this group, propagate parent clip down
+            parent_clip.clone()
+        } else {
+            // Translate clip to absolute coordinates
+            group.clip.translate(origin[0], origin[1])
         };
+
         for mark_ind in indices {
             let mark = &group.marks[mark_ind];
             match mark {
                 SceneMark::Arc(mark) => {
-                    self.add_arc_mark(mark, group_bounds)?;
+                    self.add_arc_mark(mark, origin, &clip)?;
                 }
                 SceneMark::Symbol(mark) => {
-                    self.add_symbol_mark(mark, group_bounds)?;
+                    self.add_symbol_mark(mark, origin, &clip)?;
                 }
                 SceneMark::Rect(mark) => {
-                    self.add_rect_mark(mark, group_bounds)?;
+                    self.add_rect_mark(mark, origin, &clip)?;
                 }
                 SceneMark::Rule(mark) => {
-                    self.add_rule_mark(mark, group_bounds)?;
+                    self.add_rule_mark(mark, origin, &clip)?;
                 }
                 SceneMark::Path(mark) => {
-                    self.add_path_mark(mark, group_bounds)?;
+                    self.add_path_mark(mark, origin, &clip)?;
                 }
                 SceneMark::Line(mark) => {
-                    self.add_line_mark(mark, group_bounds)?;
+                    self.add_line_mark(mark, origin, &clip)?;
                 }
                 SceneMark::Trail(mark) => {
-                    self.add_trail_mark(mark, group_bounds)?;
+                    self.add_trail_mark(mark, origin, &clip)?;
                 }
                 SceneMark::Area(mark) => {
-                    self.add_area_mark(mark, group_bounds)?;
+                    self.add_area_mark(mark, origin, &clip)?;
                 }
                 SceneMark::Text(mark) => {
-                    self.add_text_mark(mark, group_bounds)?;
+                    self.add_text_mark(mark, origin, &clip)?;
                 }
                 SceneMark::Image(mark) => {
-                    self.add_image_mark(mark, group_bounds)?;
+                    self.add_image_mark(mark, origin, &clip)?;
                 }
                 SceneMark::Group(group) => {
-                    self.add_group_mark(group, group_bounds)?;
+                    self.add_group_mark(group, origin, &clip)?;
                 }
             }
         }
         Ok(())
     }
 
     #[tracing::instrument(skip_all)]
     fn set_scene(&mut self, scene_graph: &SceneGraph) -> Result<(), AvengerWgpuError> {
         // Clear existing marks
         self.clear_mark_renderer();
 
-        // Add marks
-        let group_bounds = GroupBounds {
-            x: scene_graph.origin[0],
-            y: scene_graph.origin[1],
-            width: None,
-            height: None,
-        };
-
         // Sort groups by zindex
         let zindex = scene_graph
             .groups
             .iter()
             .map(|g| g.zindex)
             .collect::<Vec<_>>();
         let mut indices: Vec<usize> = (0..zindex.len()).collect();
         indices.sort_by_key(|i| zindex[*i].unwrap_or(0));
 
         for group_ind in &indices {
             let group = &scene_graph.groups[*group_ind];
-            self.add_group_mark(group, group_bounds)?;
+            self.add_group_mark(group, scene_graph.origin, &Clip::None)?;
         }
 
         Ok(())
     }
 }
 
 // Private shared canvas logic
-fn make_background_command<C: Canvas>(
+pub(crate) fn make_background_command<C: Canvas>(
     canvas: &C,
     texture_view: &TextureView,
     resolve_target: Option<&TextureView>,
 ) -> CommandBuffer {
     let mut background_encoder =
         canvas
             .device()
@@ -336,55 +334,57 @@
             occlusion_query_set: None,
             timestamp_writes: None,
         });
     }
     background_encoder.finish()
 }
 
-fn make_wgpu_instance() -> wgpu::Instance {
+pub(crate) fn make_wgpu_instance() -> wgpu::Instance {
     wgpu::Instance::new(wgpu::InstanceDescriptor {
         backends: wgpu::Backends::all(),
         ..Default::default()
     })
 }
 
-async fn make_wgpu_adapter(
+pub(crate) async fn make_wgpu_adapter(
     instance: &wgpu::Instance,
-    compatible_surface: Option<&Surface>,
+    compatible_surface: Option<&Surface<'_>>,
 ) -> Result<Adapter, AvengerWgpuError> {
     instance
         .request_adapter(&RequestAdapterOptions {
             power_preference: PowerPreference::default(),
             compatible_surface,
             force_fallback_adapter: false,
         })
         .await
         .ok_or(AvengerWgpuError::MakeWgpuAdapterError)
 }
 
-async fn request_wgpu_device(adapter: &Adapter) -> Result<(Device, Queue), AvengerWgpuError> {
+pub(crate) async fn request_wgpu_device(
+    adapter: &Adapter,
+) -> Result<(Device, Queue), AvengerWgpuError> {
     Ok(adapter
         .request_device(
             &DeviceDescriptor {
                 label: None,
-                features: wgpu::Features::empty(),
+                required_features: wgpu::Features::empty(),
                 // WebGL doesn't support all of wgpu's features, so if
                 // we're building for the web we'll have to disable some.
-                limits: if cfg!(target_arch = "wasm32") {
+                required_limits: if cfg!(target_arch = "wasm32") {
                     wgpu::Limits::downlevel_webgl2_defaults()
                 } else {
                     wgpu::Limits::default()
                 },
             },
             None,
         )
         .await?)
 }
 
-fn create_multisampled_framebuffer(
+pub(crate) fn create_multisampled_framebuffer(
     device: &Device,
     width: u32,
     height: u32,
     format: TextureFormat,
     sample_count: u32,
 ) -> TextureView {
     let multisampled_texture_extent = wgpu::Extent3d {
@@ -404,91 +404,99 @@
     };
 
     device
         .create_texture(multisampled_frame_descriptor)
         .create_view(&TextureViewDescriptor::default())
 }
 
-fn get_supported_sample_count(sample_flags: TextureFormatFeatureFlags) -> u32 {
+pub(crate) fn get_supported_sample_count(sample_flags: TextureFormatFeatureFlags) -> u32 {
     // Get max supported sample count up to 4
     if sample_flags.contains(wgpu::TextureFormatFeatureFlags::MULTISAMPLE_X4) {
         4
     } else if sample_flags.contains(wgpu::TextureFormatFeatureFlags::MULTISAMPLE_X2) {
         2
     } else {
         1
     }
 }
 
-pub struct WindowCanvas {
-    window: Window,
-    surface: Surface,
-    device: Device,
-    queue: Queue,
-    multisampled_framebuffer: TextureView,
+pub struct WindowCanvas<'window> {
     sample_count: u32,
-    config: SurfaceConfiguration,
+    surface_config: SurfaceConfiguration,
     dimensions: CanvasDimensions,
     marks: Vec<MarkRenderer>,
     multi_renderer: Option<MultiMarkRenderer>,
+    config: CanvasConfig,
+
+    // Order of properties determines drop order.
+    // Device must be dropped after the buffers and textures associated with marks
+    multisampled_framebuffer: TextureView,
+    queue: Queue,
+    device: Device,
+    surface: Surface<'window>,
+    window: Arc<Window>,
 }
 
-impl WindowCanvas {
+impl<'window> WindowCanvas<'window> {
     pub async fn new(
         window: Window,
         dimensions: CanvasDimensions,
+        config: CanvasConfig,
     ) -> Result<Self, AvengerWgpuError> {
-        window.set_inner_size(Size::Physical(dimensions.to_physical_size()));
+        let _ = window.request_inner_size(Size::Physical(dimensions.to_physical_size()));
         let instance = make_wgpu_instance();
-        let surface = unsafe { instance.create_surface(&window) }?;
+        let window = Arc::new(window);
+        let surface = instance.create_surface(window.clone())?;
         let adapter = make_wgpu_adapter(&instance, Some(&surface)).await?;
         let (device, queue) = request_wgpu_device(&adapter).await?;
 
         let surface_caps = surface.get_capabilities(&adapter);
 
         // Select first non-srgb texture format
         let surface_format = surface_caps
             .formats
             .iter()
             .copied()
             .find(|f| !f.is_srgb())
             .unwrap_or(surface_caps.formats[0]);
 
-        let config = SurfaceConfiguration {
+        let surface_config = SurfaceConfiguration {
             usage: TextureUsages::RENDER_ATTACHMENT,
             format: surface_format,
             width: dimensions.to_physical_width(),
             height: dimensions.to_physical_height(),
             present_mode: surface_caps.present_modes[0],
             alpha_mode: surface_caps.alpha_modes[0],
             view_formats: vec![],
+            desired_maximum_frame_latency: 2,
         };
-        surface.configure(&device, &config);
+        surface.configure(&device, &surface_config);
 
         let format_flags = adapter.get_texture_format_features(surface_format).flags;
         let sample_count = get_supported_sample_count(format_flags);
         let multisampled_framebuffer = create_multisampled_framebuffer(
             &device,
-            config.width,
-            config.height,
+            surface_config.width,
+            surface_config.height,
             surface_format,
             sample_count,
         );
 
         Ok(Self {
             surface,
             device,
             queue,
             multisampled_framebuffer,
             sample_count,
-            config,
+            surface_config,
             dimensions,
             window,
             marks: Vec::new(),
             multi_renderer: None,
+            config,
         })
     }
 
     pub fn get_size(&self) -> winit::dpi::PhysicalSize<u32> {
         self.dimensions.to_physical_size()
     }
 
@@ -569,18 +577,21 @@
         self.queue.submit(commands);
         output.present();
 
         Ok(())
     }
 }
 
-impl Canvas for WindowCanvas {
+impl<'window> Canvas for WindowCanvas<'window> {
     fn get_multi_renderer(&mut self) -> &mut MultiMarkRenderer {
         if self.multi_renderer.is_none() {
-            self.multi_renderer = Some(MultiMarkRenderer::new(self.dimensions));
+            self.multi_renderer = Some(MultiMarkRenderer::new(
+                self.dimensions,
+                self.config.text_builder_ctor.clone(),
+            ));
         }
         self.multi_renderer.as_mut().unwrap()
     }
 
     fn add_mark_renderer(&mut self, mark_renderer: MarkRenderer) {
         if let Some(multi_renderer) = self.multi_renderer.take() {
             self.marks
@@ -602,41 +613,49 @@
     }
 
     fn dimensions(&self) -> CanvasDimensions {
         self.dimensions
     }
 
     fn texture_format(&self) -> TextureFormat {
-        self.config.format
+        self.surface_config.format
     }
 
     fn sample_count(&self) -> u32 {
         self.sample_count
     }
 }
 
 pub struct PngCanvas {
-    device: Device,
-    queue: Queue,
-    multisampled_framebuffer: TextureView,
     sample_count: u32,
     marks: Vec<MarkRenderer>,
-    pub dimensions: CanvasDimensions,
-    pub texture_view: TextureView,
-    pub output_buffer: Buffer,
-    pub texture: Texture,
-    pub texture_size: Extent3d,
-    pub padded_width: u32,
-    pub padded_height: u32,
+    dimensions: CanvasDimensions,
+    texture_view: TextureView,
+    output_buffer: Buffer,
+    texture: Texture,
+    texture_size: Extent3d,
+    padded_width: u32,
+    padded_height: u32,
     multi_renderer: Option<MultiMarkRenderer>,
+    config: CanvasConfig,
+
+    // The order of properties in a struct is the order in which items are dropped.
+    // wgpu seems to require that the device be dropped last, otherwise there is a resouce
+    // leak.
+    multisampled_framebuffer: TextureView,
+    queue: Queue,
+    device: Device,
 }
 
 impl PngCanvas {
     #[tracing::instrument(skip_all)]
-    pub async fn new(dimensions: CanvasDimensions) -> Result<Self, AvengerWgpuError> {
+    pub async fn new(
+        dimensions: CanvasDimensions,
+        config: CanvasConfig,
+    ) -> Result<Self, AvengerWgpuError> {
         let instance = make_wgpu_instance();
         let adapter = make_wgpu_adapter(&instance, None).await?;
         let (device, queue) = request_wgpu_device(&adapter).await?;
         let texture_format = TextureFormat::Rgba8Unorm;
         let format_flags = adapter.get_texture_format_features(texture_format).flags;
         let sample_count = get_supported_sample_count(format_flags);
         let texture_desc = TextureDescriptor {
@@ -695,14 +714,15 @@
             texture_view,
             output_buffer,
             texture_size,
             padded_width,
             padded_height,
             marks: Vec::new(),
             multi_renderer: None,
+            config,
         })
     }
 
     #[tracing::instrument(skip_all)]
     pub async fn render(&mut self) -> Result<image::RgbaImage, AvengerWgpuError> {
         // Commit open multi mark renderer
         if let Some(multi_renderer) = self.multi_renderer.take() {
@@ -827,15 +847,18 @@
         Ok(img)
     }
 }
 
 impl Canvas for PngCanvas {
     fn get_multi_renderer(&mut self) -> &mut MultiMarkRenderer {
         if self.multi_renderer.is_none() {
-            self.multi_renderer = Some(MultiMarkRenderer::new(self.dimensions));
+            self.multi_renderer = Some(MultiMarkRenderer::new(
+                self.dimensions,
+                self.config.text_builder_ctor.clone(),
+            ));
         }
         self.multi_renderer.as_mut().unwrap()
     }
 
     fn add_mark_renderer(&mut self, mark_renderer: MarkRenderer) {
         if let Some(multi_renderer) = self.multi_renderer.take() {
             self.marks
```

### Comparing `avenger-0.0.3/avenger-wgpu/src/marks/cosmic.rs` & `avenger-0.0.4/avenger-wgpu/src/marks/text.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,144 +1,85 @@
 use crate::canvas::CanvasDimensions;
 use crate::error::AvengerWgpuError;
 use crate::marks::multi::{MultiVertex, TEXT_TEXTURE_CODE};
-use crate::marks::text::{TextAtlasBuilder, TextAtlasRegistration, TextInstance};
 use avenger::marks::path::PathTransform;
-use avenger::marks::text::{FontWeightNameSpec, FontWeightSpec, TextAlignSpec, TextBaselineSpec};
-use cosmic_text::fontdb::Database;
-use cosmic_text::{
-    Attrs, Buffer, Family, FontSystem, Metrics, Shaping, SwashCache, SwashContent, Weight,
-};
+use avenger::marks::text::{FontStyleSpec, FontWeightSpec, TextAlignSpec, TextBaselineSpec};
+use etagere::euclid::{Angle, Point2D, Vector2D};
 use image::DynamicImage;
-use lazy_static;
-use lyon::geom::euclid::{Point2D, Vector2D};
-use lyon::geom::Angle;
-use std::collections::{HashMap, HashSet};
-use std::sync::Mutex;
+use std::collections::HashMap;
+use std::hash::Hash;
+use std::sync::Arc;
 use wgpu::Extent3d;
 
-lazy_static! {
-    static ref FONT_SYSTEM: Mutex<FontSystem> = Mutex::new(build_font_system());
-    static ref SWASH_CACHE: Mutex<SwashCache> = Mutex::new(SwashCache::new());
-}
-
-fn build_font_system() -> FontSystem {
-    let mut font_system = FontSystem::new();
-
-    // Override default families based on what system fonts are available
-    let fontdb = font_system.db_mut();
-    setup_default_fonts(fontdb);
-    font_system
-}
-
-fn setup_default_fonts(fontdb: &mut Database) {
-    let families: HashSet<String> = fontdb
-        .faces()
-        .flat_map(|face| {
-            face.families
-                .iter()
-                .map(|(fam, _lang)| fam.clone())
-                .collect::<Vec<_>>()
-        })
-        .collect();
-
-    // Set default sans serif
-    for family in ["Helvetica", "Arial", "Liberation Sans"] {
-        if families.contains(family) {
-            fontdb.set_sans_serif_family(family);
-            break;
-        }
-    }
-
-    // Set default monospace font family
-    for family in [
-        "Courier New",
-        "Courier",
-        "Liberation Mono",
-        "DejaVu Sans Mono",
-    ] {
-        if families.contains(family) {
-            fontdb.set_monospace_family(family);
-            break;
-        }
-    }
+pub trait TextAtlasBuilderTrait {
+    fn register_text(
+        &mut self,
+        text: TextInstance,
+        dimensions: CanvasDimensions,
+    ) -> Result<Vec<TextAtlasRegistration>, AvengerWgpuError>;
 
-    // Set default serif font family
-    for family in [
-        "Times New Roman",
-        "Times",
-        "Liberation Serif",
-        "DejaVu Serif",
-    ] {
-        if families.contains(family) {
-            fontdb.set_serif_family(family);
-            break;
-        }
-    }
+    fn build(&self) -> (Extent3d, Vec<DynamicImage>);
 }
 
-pub fn register_font_directory(dir: &str) {
-    let mut font_system = FONT_SYSTEM
-        .lock()
-        .expect("Failed to acquire lock on FONT_SYSTEM");
-    let fontdb = font_system.db_mut();
-    fontdb.load_fonts_dir(dir);
-    setup_default_fonts(fontdb);
-}
+#[derive(Clone)]
+pub struct NullTextAtlasBuilder;
 
-#[derive(Copy, Clone)]
-pub struct TextAtlasCoords {
-    pub x0: f32,
-    pub y0: f32,
-    pub x1: f32,
-    pub y1: f32,
-}
+impl TextAtlasBuilderTrait for NullTextAtlasBuilder {
+    fn register_text(
+        &mut self,
+        _text: TextInstance,
+        _dimensions: CanvasDimensions,
+    ) -> Result<Vec<TextAtlasRegistration>, AvengerWgpuError> {
+        Err(AvengerWgpuError::TextNotEnabled(
+            "Text support is not enabled".to_string(),
+        ))
+    }
 
-#[derive(Clone)]
-pub struct GlyphDetails {
-    top: f32,
-    left: f32,
-    width: f32,
-    height: f32,
-    tex_coords: TextAtlasCoords,
+    fn build(&self) -> (Extent3d, Vec<DynamicImage>) {
+        (
+            Extent3d {
+                width: 1,
+                height: 1,
+                depth_or_array_layers: 1,
+            },
+            vec![DynamicImage::ImageRgba8(image::RgbaImage::new(1, 1))],
+        )
+    }
 }
 
-pub struct CosmicTextAtlasBuilder {
+#[derive(Clone)]
+pub struct TextAtlasBuilder<CacheKey: Hash + Eq + Clone> {
+    rasterizer: Arc<dyn TextRasterizer<CacheKey = CacheKey>>,
     extent: Extent3d,
     next_atlas: image::RgbaImage,
-    next_cache: HashMap<(cosmic_text::CacheKey, [u8; 4]), GlyphDetails>,
+    next_cache: HashMap<CacheKey, GlyphBBoxAndAtlasCoords>,
     atlases: Vec<DynamicImage>,
     initialized: bool,
     allocator: etagere::AtlasAllocator,
 }
 
-impl Default for CosmicTextAtlasBuilder {
-    fn default() -> Self {
-        Self::new()
-    }
-}
-
-impl CosmicTextAtlasBuilder {
-    pub fn new() -> Self {
+impl<CacheKey: Hash + Eq + Clone> TextAtlasBuilder<CacheKey> {
+    pub fn new(rasterizer: Arc<dyn TextRasterizer<CacheKey = CacheKey>>) -> Self {
         Self {
+            rasterizer,
             extent: Extent3d {
                 width: 1,
                 height: 1,
                 depth_or_array_layers: 1,
             },
             next_atlas: image::RgbaImage::new(1, 1),
             next_cache: Default::default(),
             atlases: vec![],
             initialized: false,
             allocator: etagere::AtlasAllocator::new(etagere::Size::new(1, 1)),
         }
     }
 }
 
-impl TextAtlasBuilder for CosmicTextAtlasBuilder {
+impl<CacheKey: Hash + Eq + Clone> TextAtlasBuilderTrait for TextAtlasBuilder<CacheKey> {
     fn register_text(
         &mut self,
         text: TextInstance,
         dimensions: CanvasDimensions,
     ) -> Result<Vec<TextAtlasRegistration>, AvengerWgpuError> {
         if !self.initialized {
             let limits = wgpu::Limits::downlevel_webgl2_defaults();
@@ -159,126 +100,66 @@
                 self.extent.height as i32,
             ));
 
             // Set initialized
             self.initialized = true;
         }
 
-        let mut font_system = FONT_SYSTEM
-            .lock()
-            .expect("Failed to acquire lock on FONT_SYSTEM");
-        let mut cache = SWASH_CACHE
-            .lock()
-            .expect("Failed to acquire lock on SWASH_CACHE");
-
-        // Build cosmic-text Buffer
-        let mut buffer = Buffer::new(
-            &mut font_system,
-            Metrics::new(text.font_size, text.font_size),
-        );
-        let family = match text.font.to_lowercase().as_str() {
-            "serif" => Family::Serif,
-            "sans serif" | "sans-serif" => Family::SansSerif,
-            "cursive" => Family::Cursive,
-            "fantasy" => Family::Fantasy,
-            "monospace" => Family::Monospace,
-            _ => Family::Name(text.font.as_str()),
-        };
-        let weight = match text.font_weight {
-            FontWeightSpec::Name(FontWeightNameSpec::Bold) => Weight::BOLD,
-            FontWeightSpec::Name(FontWeightNameSpec::Normal) => Weight::NORMAL,
-            FontWeightSpec::Number(w) => Weight(*w as u16),
-        };
-
-        buffer.set_text(
-            &mut font_system,
-            text.text,
-            Attrs::new().family(family).weight(weight),
-            Shaping::Advanced,
-        );
-
-        buffer.set_size(&mut font_system, dimensions.size[0], dimensions.size[1]);
-        buffer.shape_until_scroll(&mut font_system, false);
-
-        let (buffer_width, line_y, buffer_height) = measure(&buffer);
-        let buffer_left = match text.align {
-            TextAlignSpec::Left => text.position[0],
-            TextAlignSpec::Center => text.position[0] - buffer_width / 2.0,
-            TextAlignSpec::Right => text.position[0] - buffer_width,
+        // Extract values we need from text instance before passing to buffer constructor
+        let align = *text.align;
+        let baseline = *text.baseline;
+        let position = text.position;
+        let angle = text.angle;
+
+        let buffer = self.rasterizer.rasterize(
+            dimensions,
+            &TextRasterizationConfig::from(text),
+            &self.next_cache,
+        )?;
+
+        let buffer_left = match align {
+            TextAlignSpec::Left => position[0],
+            TextAlignSpec::Center => position[0] - buffer.buffer_width / 2.0,
+            TextAlignSpec::Right => position[0] - buffer.buffer_width,
         };
 
-        let buffer_top = match text.baseline {
-            TextBaselineSpec::Alphabetic => text.position[1] - line_y,
-            TextBaselineSpec::Top => text.position[1],
-            TextBaselineSpec::Middle => text.position[1] - buffer_height * 0.5,
-            TextBaselineSpec::Bottom => text.position[1] - buffer_height,
+        let buffer_top = match baseline {
+            TextBaselineSpec::Alphabetic => position[1] - buffer.buffer_line_y,
+            TextBaselineSpec::Top => position[1],
+            TextBaselineSpec::Middle => position[1] - buffer.buffer_height * 0.5,
+            TextBaselineSpec::Bottom => position[1] - buffer.buffer_height,
             TextBaselineSpec::LineTop => todo!(),
             TextBaselineSpec::LineBottom => todo!(),
         };
 
         // Build rotation_transform
-        let rotation_transform = if text.angle != 0.0 {
-            PathTransform::translation(-text.position[0], -text.position[1])
-                .then_rotate(Angle::degrees(text.angle))
-                .then_translate(Vector2D::new(text.position[0], text.position[1]))
+        let rotation_transform = if angle != 0.0 {
+            PathTransform::translation(-position[0], -position[1])
+                .then_rotate(Angle::degrees(angle))
+                .then_translate(Vector2D::new(position[0], position[1]))
         } else {
             PathTransform::identity()
         };
 
         let mut registrations: Vec<TextAtlasRegistration> = Vec::new();
         let mut verts: Vec<MultiVertex> = Vec::new();
         let mut indices: Vec<u32> = Vec::new();
 
-        let text_color = [
-            (text.color[0] * 255.0).round() as u8,
-            (text.color[1] * 255.0).round() as u8,
-            (text.color[2] * 255.0).round() as u8,
-            (text.color[3] * 255.0).round() as u8,
-        ];
-
-        for run in buffer.layout_runs() {
-            for glyph in run.glyphs.iter() {
-                let physical_glyph = glyph.physical(
-                    (
-                        buffer_left * dimensions.scale,
-                        buffer_top * dimensions.scale,
-                    ),
-                    dimensions.scale,
-                );
-
-                // Compute cache key which combines glyph and color
-                let cache_key = (physical_glyph.cache_key, text_color);
-
-                let details = if let Some(details) = self.next_cache.get(&cache_key) {
-                    // Glyph has already been rasterize and written to next_atlas
-                    details
+        for (glyph_image, phys_position) in &buffer.glyphs {
+            let glyph_bbox_and_atlas_coords =
+                if let Some(glyph_position) = self.next_cache.get(&glyph_image.cache_key) {
+                    // Glyph has already been written to atlas
+                    glyph_position
                 } else {
-                    // We need to rasterize glyph and write it to next_atlas
-                    let Some(image) = cache
-                        .get_image(&mut font_system, physical_glyph.cache_key)
-                        .as_ref()
-                    else {
-                        return Err(AvengerWgpuError::ImageAllocationError(
-                            "Failed to create glyph image".to_string(),
-                        ));
-                    };
-
-                    let width = image.placement.width as usize;
-                    let height = image.placement.height as usize;
-                    let should_rasterize = width > 0 && height > 0;
-
-                    if !should_rasterize {
-                        continue;
-                    }
-
                     // Allocate space in active atlas image, leaving space for 1 pixel empty border
-                    let allocation = if let Some(allocation) = self
-                        .allocator
-                        .allocate(etagere::Size::new((width + 2) as i32, (height + 2) as i32))
-                    {
+                    let allocation = if let Some(allocation) =
+                        self.allocator.allocate(etagere::Size::new(
+                            (glyph_image.bbox.width + 2) as i32,
+                            (glyph_image.bbox.height + 2) as i32,
+                        )) {
                         // Successfully allocated space in the active atlas
                         allocation
                     } else {
                         // No more room in active atlas
 
                         // Commit current registration
                         let mut full_verts = Vec::new();
@@ -305,166 +186,128 @@
                         // Create fresh allocator
                         self.allocator = etagere::AtlasAllocator::new(etagere::Size::new(
                             self.extent.width as i32,
                             self.extent.height as i32,
                         ));
 
                         // Try allocation again
-                        if let Some(allocation) = self
-                            .allocator
-                            .allocate(etagere::Size::new((width + 2) as i32, (height + 2) as i32))
-                        {
+                        if let Some(allocation) = self.allocator.allocate(etagere::Size::new(
+                            (glyph_image.bbox.width + 2) as i32,
+                            (glyph_image.bbox.height + 2) as i32,
+                        )) {
                             allocation
                         } else {
                             return Err(AvengerWgpuError::ImageAllocationError(
                                 "Failed to allocate space for glyph".to_string(),
                             ));
                         }
                     };
 
                     // Write image to allocated portion of final texture image
                     // Use one pixel offset to avoid aliasing artifacts in linear interpolation
                     let p0 = allocation.rectangle.min;
                     let atlas_x0 = p0.x + 1;
-                    let atlas_x1 = atlas_x0 + width as i32;
+                    let atlas_x1 = atlas_x0 + glyph_image.bbox.width as i32;
                     let atlas_y0 = p0.y + 1;
-                    let atlas_y1 = atlas_y0 + height as i32;
+                    let atlas_y1 = atlas_y0 + glyph_image.bbox.height as i32;
 
-                    match image.content {
-                        SwashContent::Color => {
-                            // Image is rgba (like an emoji)
-                            let Some(img) = image::RgbaImage::from_vec(
-                                width as u32,
-                                height as u32,
-                                image.data.clone(),
-                            ) else {
-                                return Err(AvengerWgpuError::ImageAllocationError(
-                                    "Failed to parse text rasterization as Rgba image".to_string(),
-                                ));
-                            };
-                            for (src_x, dest_x) in (atlas_x0..atlas_x1).enumerate() {
-                                for (src_y, dest_y) in (atlas_y0..atlas_y1).enumerate() {
-                                    self.next_atlas.put_pixel(
-                                        dest_x as u32,
-                                        dest_y as u32,
-                                        *img.get_pixel(src_x as u32, src_y as u32),
-                                    );
-                                }
-                            }
-                        }
-                        SwashContent::Mask | SwashContent::SubpixelMask => {
-                            // Image is monochrome (like regular text)
-                            let Some(img) = image::GrayImage::from_vec(
-                                width as u32,
-                                height as u32,
-                                image.data.clone(),
-                            ) else {
-                                return Err(AvengerWgpuError::ImageAllocationError(
-                                    "Failed to parse text rasterization as Grayscale image"
-                                        .to_string(),
-                                ));
-                            };
-                            for (src_x, dest_x) in (atlas_x0..atlas_x1).enumerate() {
-                                for (src_y, dest_y) in (atlas_y0..atlas_y1).enumerate() {
-                                    // Compute alpha, combining the text color alpha and the pixel alpha
-                                    let pixel_lum = img.get_pixel(src_x as u32, src_y as u32).0[0];
-
-                                    // Compute pixel color, adjusting alpha by pixel luminance
-                                    let mut pixel_color = text_color;
-                                    pixel_color[3] =
-                                        ((text_color[3] as f32) * (pixel_lum as f32 / 255.0))
-                                            .round() as u8;
-
-                                    let pixel = image::Rgba::from(pixel_color);
-                                    self.next_atlas
-                                        .put_pixel(dest_x as u32, dest_y as u32, pixel);
-                                }
-                            }
+                    let Some(img) = glyph_image.image.as_ref() else {
+                        return Err(AvengerWgpuError::TextError(
+                            "Expected glyph image to be available on first use".to_string(),
+                        ));
+                    };
+
+                    for (src_x, dest_x) in (atlas_x0..atlas_x1).enumerate() {
+                        for (src_y, dest_y) in (atlas_y0..atlas_y1).enumerate() {
+                            self.next_atlas.put_pixel(
+                                dest_x as u32,
+                                dest_y as u32,
+                                *img.get_pixel(src_x as u32, src_y as u32),
+                            );
                         }
                     }
 
                     self.next_cache.insert(
-                        cache_key,
-                        GlyphDetails {
-                            top: image.placement.top as f32,
-                            left: image.placement.left as f32,
-                            width: width as f32,
-                            height: height as f32,
+                        glyph_image.cache_key.clone(),
+                        GlyphBBoxAndAtlasCoords {
+                            bbox: glyph_image.bbox,
                             tex_coords: TextAtlasCoords {
                                 x0: (atlas_x0 as f32) / self.extent.width as f32,
                                 y0: (atlas_y0 as f32) / self.extent.height as f32,
                                 x1: (atlas_x1 as f32) / self.extent.width as f32,
                                 y1: (atlas_y1 as f32) / self.extent.height as f32,
                             },
                         },
                     );
-                    self.next_cache.get(&cache_key).unwrap()
+                    self.next_cache.get(&glyph_image.cache_key).unwrap()
                 };
 
-                // Create verts for rectangle around glyph
-                let x0 = (physical_glyph.x as f32 + details.left) / dimensions.scale;
-                let y0 = (run.line_y).round()
-                    + (physical_glyph.y as f32 - details.top) / dimensions.scale;
-                let x1 = x0 + details.width / dimensions.scale;
-                let y1 = y0 + details.height / dimensions.scale;
-
-                let top_left = rotation_transform
-                    .transform_point(Point2D::new(x0, y0))
-                    .to_array();
-                let bottom_left = rotation_transform
-                    .transform_point(Point2D::new(x0, y1))
-                    .to_array();
-                let bottom_right = rotation_transform
-                    .transform_point(Point2D::new(x1, y1))
-                    .to_array();
-                let top_right = rotation_transform
-                    .transform_point(Point2D::new(x1, y0))
-                    .to_array();
-
-                let tex_x0 = details.tex_coords.x0;
-                let tex_y0 = details.tex_coords.y0;
-                let tex_x1 = details.tex_coords.x1;
-                let tex_y1 = details.tex_coords.y1;
-
-                let offset = verts.len() as u32;
-
-                verts.push(MultiVertex {
-                    position: top_left,
-                    color: [TEXT_TEXTURE_CODE, tex_x0, tex_y0, 0.0],
-                    top_left,
-                    bottom_right,
-                });
-                verts.push(MultiVertex {
-                    position: bottom_left,
-                    color: [TEXT_TEXTURE_CODE, tex_x0, tex_y1, 0.0],
-                    top_left,
-                    bottom_right,
-                });
-                verts.push(MultiVertex {
-                    position: bottom_right,
-                    color: [TEXT_TEXTURE_CODE, tex_x1, tex_y1, 0.0],
-                    top_left,
-                    bottom_right,
-                });
-                verts.push(MultiVertex {
-                    position: top_right,
-                    color: [TEXT_TEXTURE_CODE, tex_x1, tex_y0, 0.0],
-                    top_left,
-                    bottom_right,
-                });
-
-                indices.extend([
-                    offset,
-                    offset + 1,
-                    offset + 2,
-                    offset,
-                    offset + 2,
-                    offset + 3,
-                ])
-            }
+            // Create verts for rectangle around glyph
+            let bbox = &glyph_bbox_and_atlas_coords.bbox;
+            let x0 = (phys_position.x + bbox.left as f32) / dimensions.scale + buffer_left;
+            let y0 = (buffer.buffer_line_y).round()
+                + (phys_position.y - bbox.top as f32) / dimensions.scale
+                + buffer_top;
+            let x1 = x0 + bbox.width as f32 / dimensions.scale;
+            let y1 = y0 + bbox.height as f32 / dimensions.scale;
+
+            let top_left = rotation_transform
+                .transform_point(Point2D::new(x0, y0))
+                .to_array();
+            let bottom_left = rotation_transform
+                .transform_point(Point2D::new(x0, y1))
+                .to_array();
+            let bottom_right = rotation_transform
+                .transform_point(Point2D::new(x1, y1))
+                .to_array();
+            let top_right = rotation_transform
+                .transform_point(Point2D::new(x1, y0))
+                .to_array();
+
+            let tex_coords = glyph_bbox_and_atlas_coords.tex_coords;
+            let tex_x0 = tex_coords.x0;
+            let tex_y0 = tex_coords.y0;
+            let tex_x1 = tex_coords.x1;
+            let tex_y1 = tex_coords.y1;
+
+            let offset = verts.len() as u32;
+
+            verts.push(MultiVertex {
+                position: top_left,
+                color: [TEXT_TEXTURE_CODE, tex_x0, tex_y0, 0.0],
+                top_left,
+                bottom_right,
+            });
+            verts.push(MultiVertex {
+                position: bottom_left,
+                color: [TEXT_TEXTURE_CODE, tex_x0, tex_y1, 0.0],
+                top_left,
+                bottom_right,
+            });
+            verts.push(MultiVertex {
+                position: bottom_right,
+                color: [TEXT_TEXTURE_CODE, tex_x1, tex_y1, 0.0],
+                top_left,
+                bottom_right,
+            });
+            verts.push(MultiVertex {
+                position: top_right,
+                color: [TEXT_TEXTURE_CODE, tex_x1, tex_y0, 0.0],
+                top_left,
+                bottom_right,
+            });
+
+            indices.extend([
+                offset,
+                offset + 1,
+                offset + 2,
+                offset,
+                offset + 2,
+                offset + 3,
+            ])
         }
 
         // Add final registration
         registrations.push(TextAtlasRegistration {
             atlas_index: self.atlases.len(),
             verts,
             indices,
@@ -476,24 +319,120 @@
     fn build(&self) -> (Extent3d, Vec<DynamicImage>) {
         let mut images = self.atlases.clone();
         images.push(image::DynamicImage::ImageRgba8(self.next_atlas.clone()));
         (self.extent, images)
     }
 }
 
-pub fn measure(buffer: &Buffer) -> (f32, f32, f32) {
-    let (width, line_y, total_lines) =
-        buffer
-            .layout_runs()
-            .fold((0.0, 0.0, 0usize), |(width, line_y, total_lines), run| {
-                (
-                    run.line_w.max(width),
-                    run.line_y.max(line_y),
-                    total_lines + 1,
-                )
-            });
-    (
-        width,
-        line_y,
-        total_lines as f32 * buffer.metrics().line_height,
-    )
+#[derive(Clone)]
+pub struct TextAtlasRegistration {
+    pub atlas_index: usize,
+    pub verts: Vec<MultiVertex>,
+    pub indices: Vec<u32>,
+}
+
+#[derive(Clone, Debug)]
+pub struct TextInstance<'a> {
+    pub position: [f32; 2],
+    pub text: &'a String,
+    pub color: &'a [f32; 4],
+    pub align: &'a TextAlignSpec,
+    pub angle: f32,
+    pub baseline: &'a TextBaselineSpec,
+    pub font: &'a String,
+    pub font_size: f32,
+    pub font_weight: &'a FontWeightSpec,
+    pub font_style: &'a FontStyleSpec,
+    pub limit: f32,
+}
+
+// Position of glyph in text buffer
+#[derive(Debug, Clone)]
+pub struct PhysicalGlyphPosition {
+    pub x: f32,
+    pub y: f32,
+}
+
+// Position of glyph in text atlas
+#[derive(Copy, Clone)]
+pub struct TextAtlasCoords {
+    pub x0: f32,
+    pub y0: f32,
+    pub x1: f32,
+    pub y1: f32,
+}
+
+// Glyph bounding box relative to glyph origin
+#[derive(Clone, Copy)]
+pub struct GlyphBBox {
+    pub top: i32,
+    pub left: i32,
+    pub width: u32,
+    pub height: u32,
+}
+
+#[derive(Clone)]
+pub struct GlyphImage<CacheKey: Hash + Eq + Clone> {
+    pub cache_key: CacheKey,
+    // None if image for same CacheKey was already included
+    pub image: Option<image::RgbaImage>,
+    pub bbox: GlyphBBox,
+}
+
+impl<CacheKey: Hash + Eq + Clone> GlyphImage<CacheKey> {
+    pub fn without_image(&self) -> Self {
+        Self {
+            cache_key: self.cache_key.clone(),
+            image: None,
+            bbox: self.bbox,
+        }
+    }
+}
+
+#[derive(Clone)]
+pub struct GlyphBBoxAndAtlasCoords {
+    pub bbox: GlyphBBox,
+    pub tex_coords: TextAtlasCoords,
+}
+
+#[derive(Debug, Clone)]
+pub struct TextRasterizationConfig<'a> {
+    pub text: &'a String,
+    pub color: &'a [f32; 4],
+    pub font: &'a String,
+    pub font_size: f32,
+    pub font_weight: &'a FontWeightSpec,
+    pub font_style: &'a FontStyleSpec,
+    pub limit: f32,
+}
+
+impl<'a> From<TextInstance<'a>> for TextRasterizationConfig<'a> {
+    fn from(value: TextInstance<'a>) -> Self {
+        Self {
+            text: value.text,
+            color: value.color,
+            font: value.font,
+            font_size: value.font_size,
+            font_weight: value.font_weight,
+            font_style: value.font_style,
+            limit: value.limit,
+        }
+    }
+}
+
+#[derive(Clone)]
+pub struct TextRasterizationBuffer<CacheKey: Hash + Eq + Clone> {
+    pub glyphs: Vec<(GlyphImage<CacheKey>, PhysicalGlyphPosition)>,
+    pub buffer_width: f32,
+    pub buffer_height: f32,
+    pub buffer_line_y: f32,
+}
+
+pub trait TextRasterizer {
+    type CacheKey: Hash + Eq + Clone;
+    fn rasterize(
+        &self,
+        dimensions: CanvasDimensions,
+        config: &TextRasterizationConfig,
+        cached_glyphs: &HashMap<Self::CacheKey, GlyphBBoxAndAtlasCoords>,
+    ) -> Result<TextRasterizationBuffer<Self::CacheKey>, AvengerWgpuError>;
 }
```

### Comparing `avenger-0.0.3/avenger-wgpu/src/marks/gradient.rs` & `avenger-0.0.4/avenger-wgpu/src/marks/gradient.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.3/avenger-wgpu/src/marks/image.rs` & `avenger-0.0.4/avenger-wgpu/src/marks/image.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.3/avenger-wgpu/src/marks/instanced_mark.rs` & `avenger-0.0.4/avenger-wgpu/src/marks/instanced_mark.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use crate::canvas::ClipRect;
+use avenger::marks::group::Clip;
 use std::ops::Range;
 use wgpu::util::DeviceExt;
 use wgpu::{CommandBuffer, Device, Extent3d, ImageDataLayout, TextureFormat, TextureView};
 
 #[derive(Clone)]
 pub struct InstancedMarkBatch {
     pub instances_range: Range<u32>,
@@ -45,24 +45,26 @@
     pub num_indices: u32,
     pub instance_buffer: wgpu::Buffer,
     pub batches: Vec<InstancedMarkBatch>,
     pub uniform_bind_group: wgpu::BindGroup,
     pub texture: wgpu::Texture,
     pub texture_size: wgpu::Extent3d,
     pub texture_bind_group: wgpu::BindGroup,
-    pub clip_rect: Option<ClipRect>,
+    pub clip: Clip,
+    pub scale: f32,
 }
 
 impl InstancedMarkRenderer {
     pub fn new<I, V, U>(
         device: &Device,
         texture_format: TextureFormat,
         sample_count: u32,
         mark_shader: Box<dyn InstancedMarkShader<Instance = I, Vertex = V, Uniform = U>>,
-        clip_rect: Option<ClipRect>,
+        clip: Clip,
+        scale: f32,
     ) -> Self
     where
         I: bytemuck::Pod + bytemuck::Zeroable,
         V: bytemuck::Pod + bytemuck::Zeroable,
         U: bytemuck::Pod + bytemuck::Zeroable,
     {
         // Uniforms
@@ -234,15 +236,16 @@
             batches: Vec::from(mark_shader.batches()),
             num_indices,
             instance_buffer,
             uniform_bind_group,
             texture,
             texture_size: mark_shader.texture_size(),
             texture_bind_group,
-            clip_rect,
+            clip,
+            scale,
         }
     }
 
     pub fn render(
         &self,
         device: &Device,
         texture_view: &TextureView,
@@ -298,20 +301,26 @@
                 render_pass.set_bind_group(0, &self.uniform_bind_group, &[]);
                 render_pass.set_bind_group(1, &self.texture_bind_group, &[]);
                 render_pass.set_vertex_buffer(0, self.vertex_buffer.slice(..));
                 render_pass.set_vertex_buffer(1, self.instance_buffer.slice(..));
                 render_pass
                     .set_index_buffer(self.index_buffer.slice(..), wgpu::IndexFormat::Uint16);
 
-                if let Some(clip_rect) = self.clip_rect {
+                if let Clip::Rect {
+                    x,
+                    y,
+                    width,
+                    height,
+                } = self.clip
+                {
                     render_pass.set_scissor_rect(
-                        clip_rect.x,
-                        clip_rect.y,
-                        clip_rect.width,
-                        clip_rect.height,
+                        (x * self.scale) as u32,
+                        (y * self.scale) as u32,
+                        (width * self.scale) as u32,
+                        (height * self.scale) as u32,
                     );
                 }
 
                 render_pass.draw_indexed(0..self.num_indices, 0, batch.instances_range.clone());
             }
         }
```

### Comparing `avenger-0.0.3/avenger-wgpu/src/marks/multi.rs` & `avenger-0.0.4/avenger-wgpu/src/marks/multi.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-use crate::canvas::{CanvasDimensions, ClipRect};
+use crate::canvas::{CanvasDimensions, TextBuildCtor};
 use crate::error::AvengerWgpuError;
 
 use crate::marks::gradient::{to_color_or_gradient_coord, GradientAtlasBuilder};
 use crate::marks::image::ImageAtlasBuilder;
 use avenger::marks::area::{AreaMark, AreaOrientation};
-use avenger::marks::group::GroupBounds;
 use avenger::marks::image::ImageMark;
 use avenger::marks::line::LineMark;
 use avenger::marks::path::{PathMark, PathTransform};
 use avenger::marks::rect::RectMark;
 use avenger::marks::rule::RuleMark;
 use avenger::marks::symbol::SymbolMark;
 use avenger::marks::trail::TrailMark;
@@ -26,24 +25,26 @@
     StrokeVertexConstructor, VertexBuffers,
 };
 use lyon::path::builder::SvgPathBuilder;
 use lyon::path::builder::{BorderRadii, WithSvg};
 use lyon::path::path::BuilderImpl;
 use lyon::path::{Path, Winding};
 use std::ops::{Mul, Neg, Range};
+
 use wgpu::util::DeviceExt;
 use wgpu::{
     BindGroup, BindGroupLayout, CommandBuffer, Device, Extent3d, Queue, TextureFormat, TextureView,
     VertexBufferLayout,
 };
 
 // Import rayon prelude as required by par_izip.
-use crate::marks::text::{TextAtlasBuilder, TextInstance};
+use crate::marks::text::{TextAtlasBuilderTrait, TextInstance};
 
 use avenger::marks::arc::ArcMark;
+use avenger::marks::group::Clip;
 use avenger::marks::text::TextMark;
 
 #[cfg(feature = "rayon")]
 use {crate::par_izip, rayon::prelude::*};
 
 pub const GRADIENT_TEXTURE_CODE: f32 = -1.0;
 pub const IMAGE_TEXTURE_CODE: f32 = -2.0;
@@ -84,62 +85,116 @@
         }
     }
 }
 
 #[derive(Clone)]
 pub struct MultiMarkBatch {
     pub indices_range: Range<u32>,
-    pub clip: Option<ClipRect>,
+    pub clip: Clip,
+    pub clip_indices_range: Option<Range<u32>>,
     pub image_atlas_index: Option<usize>,
     pub gradient_atlas_index: Option<usize>,
     pub text_atlas_index: Option<usize>,
 }
 
 pub struct MultiMarkRenderer {
     verts_inds: Vec<(Vec<MultiVertex>, Vec<u32>)>,
+    clip_verts_inds: Vec<(Vec<MultiVertex>, Vec<u32>)>,
     batches: Vec<MultiMarkBatch>,
     uniform: MultiUniform,
     gradient_atlas_builder: GradientAtlasBuilder,
     image_atlas_builder: ImageAtlasBuilder,
-    text_atlas_builder: Box<dyn TextAtlasBuilder>,
+    text_atlas_builder: Box<dyn TextAtlasBuilderTrait>,
     dimensions: CanvasDimensions,
 }
 
 impl MultiMarkRenderer {
-    pub fn new(dimensions: CanvasDimensions) -> Self {
-        cfg_if::cfg_if! {
-            if #[cfg(feature = "cosmic-text")] {
-                use crate::marks::cosmic::CosmicTextAtlasBuilder;
-                let text_atlas_builder: Box<dyn TextAtlasBuilder> = Box::new(CosmicTextAtlasBuilder::new());
-            } else {
-                use crate::marks::text::NullTextAtlasBuilder;
-                let text_atlas_builder: Box<dyn TextAtlasBuilder> = Box::new(NullTextAtlasBuilder);
-            }
+    pub fn new(
+        dimensions: CanvasDimensions,
+        text_atlas_builder_ctor: Option<TextBuildCtor>,
+    ) -> Self {
+        let text_atlas_builder = if let Some(text_atlas_builder_ctor) = text_atlas_builder_ctor {
+            text_atlas_builder_ctor()
+        } else {
+            cfg_if::cfg_if! {
+                if #[cfg(feature = "cosmic-text")] {
+                    use crate::marks::cosmic::CosmicTextRasterizer;
+                    use crate::marks::text::TextAtlasBuilder;
+                    use std::sync::Arc;
+                    let inner_text_atlas_builder: Box<dyn TextAtlasBuilderTrait> = Box::new(TextAtlasBuilder::new(Arc::new(CosmicTextRasterizer)));
+                } else {
+                    use crate::marks::text::NullTextAtlasBuilder;
+                    let inner_text_atlas_builder: Box<dyn TextAtlasBuilderTrait> = Box::new(NullTextAtlasBuilder);
+                }
+            };
+            inner_text_atlas_builder
         };
 
         Self {
             verts_inds: vec![],
+            clip_verts_inds: vec![],
             batches: vec![],
             dimensions,
             uniform: MultiUniform {
                 size: dimensions.size,
                 scale: dimensions.scale,
                 _pad: [0.0],
             },
             gradient_atlas_builder: GradientAtlasBuilder::new(),
             image_atlas_builder: ImageAtlasBuilder::new(),
             text_atlas_builder,
         }
     }
 
+    fn add_clip_path(
+        &mut self,
+        clip: &Clip,
+        should_clip: bool,
+    ) -> Result<Option<Range<u32>>, AvengerWgpuError> {
+        if !should_clip {
+            return Ok(None);
+        }
+
+        if let Clip::Path(path) = &clip {
+            // Tesselate path
+            let bbox = bounding_box(path);
+
+            // Create vertex/index buffer builder
+            let mut buffers: VertexBuffers<MultiVertex, u32> = VertexBuffers::new();
+            let mut builder = BuffersBuilder::new(
+                &mut buffers,
+                crate::marks::multi::VertexPositions {
+                    fill: [0.0, 0.0, 0.0, 1.0],
+                    stroke: [0.0, 0.0, 0.0, 0.0],
+                    top_left: bbox.min.to_array(),
+                    bottom_right: bbox.max.to_array(),
+                },
+            );
+
+            // Tesselate fill
+            let mut fill_tessellator = FillTessellator::new();
+            let fill_options = FillOptions::default().with_tolerance(0.05);
+            fill_tessellator.tessellate_path(path, &fill_options, &mut builder)?;
+
+            let start_index = self.num_clip_indices() as u32;
+            self.clip_verts_inds
+                .push((buffers.vertices, buffers.indices));
+            let end_index = self.num_clip_indices() as u32;
+            Ok(Some(start_index..end_index))
+        } else {
+            Ok(None)
+        }
+    }
+
     #[tracing::instrument(skip_all)]
     pub fn add_rule_mark(
         &mut self,
         mark: &RuleMark,
-        bounds: GroupBounds,
+        origin: [f32; 2],
+        clip: &Clip,
     ) -> Result<(), AvengerWgpuError> {
         let (gradient_atlas_index, grad_coords) = self
             .gradient_atlas_builder
             .register_gradients(&mark.gradients);
 
         let verts_inds = if let Some(stroke_dash_iter) = mark.stroke_dash_iter() {
             izip!(
@@ -183,16 +238,16 @@
 
                     if draw {
                         let dash_x0 = x0 + xhat * start_dash_dist;
                         let dash_y0 = y0 + yhat * start_dash_dist;
                         let dash_x1 = x0 + xhat * end_dash_dist;
                         let dash_y1 = y0 + yhat * end_dash_dist;
 
-                        path_builder.move_to(Point::new(dash_x0 + bounds.x, dash_y0 + bounds.y));
-                        path_builder.line_to(Point::new(dash_x1 + bounds.x, dash_y1 + bounds.y));
+                        path_builder.move_to(Point::new(dash_x0 + origin[0], dash_y0 + origin[1]));
+                        path_builder.line_to(Point::new(dash_x1 + origin[0], dash_y1 + origin[1]));
                     }
 
                     // update start dist for next dash/gap
                     start_dash_dist = end_dash_dist;
 
                     // increment index and cycle back to start of start of dash array
                     dash_idx = (dash_idx + 1) % stroke_dash.len();
@@ -237,16 +292,16 @@
                 mark.x1_iter(),
                 mark.y1_iter(),
                 mark.stroke_iter(),
                 mark.stroke_width_iter(),
                 mark.stroke_cap_iter(),
             ).map(|(x0, y0, x1, y1, stroke, stroke_width, cap)| -> Result<(Vec<MultiVertex>, Vec<u32>), AvengerWgpuError> {
                 let mut path_builder = lyon::path::Path::builder().with_svg();
-                path_builder.move_to(Point::new(*x0 + bounds.x, *y0 + bounds.y));
-                path_builder.line_to(Point::new(*x1 + bounds.x, *y1 + bounds.y));
+                path_builder.move_to(Point::new(*x0 + origin[0], *y0 + origin[1]));
+                path_builder.line_to(Point::new(*x1 + origin[0], *y1 + origin[1]));
                 let path = path_builder.build();
                 let bbox = bounding_box(&path);
 
                 // Create vertex/index buffer builder
                 let mut buffers: VertexBuffers<MultiVertex, u32> = VertexBuffers::new();
                 let mut builder = BuffersBuilder::new(
                     &mut buffers,
@@ -277,30 +332,32 @@
 
         let start_ind = self.num_indices();
         let inds_len: usize = verts_inds.iter().map(|(_, i)| i.len()).sum();
         let indices_range = (start_ind as u32)..((start_ind + inds_len) as u32);
 
         let batch = MultiMarkBatch {
             indices_range,
-            clip: ClipRect::maybe_from_group_bounds(self.uniform.scale, bounds, mark.clip),
+            clip: clip.maybe_clip(mark.clip),
+            clip_indices_range: self.add_clip_path(clip, mark.clip)?,
             image_atlas_index: None,
             gradient_atlas_index,
             text_atlas_index: None,
         };
 
         self.verts_inds.extend(verts_inds);
         self.batches.push(batch);
         Ok(())
     }
 
     #[tracing::instrument(skip_all)]
     pub fn add_rect_mark(
         &mut self,
         mark: &RectMark,
-        bounds: GroupBounds,
+        origin: [f32; 2],
+        clip: &Clip,
     ) -> Result<(), AvengerWgpuError> {
         let (gradient_atlas_index, grad_coords) = self
             .gradient_atlas_builder
             .register_gradients(&mark.gradients);
 
         let verts_inds = if mark.gradients.is_empty()
             && mark.stroke_width.equals_scalar(0.0)
@@ -316,16 +373,16 @@
                 0..mark.len,
                 mark.x_iter(),
                 mark.y_iter(),
                 mark.width_iter(),
                 mark.height_iter(),
                 mark.fill_iter()
             ) {
-                let x0 = *x + bounds.x;
-                let y0 = *y + bounds.y;
+                let x0 = *x + origin[0];
+                let y0 = *y + origin[1];
                 let x1 = x0 + width;
                 let y1 = y0 + height;
                 let top_left = [x0, y0];
                 let bottom_right = [x1, y1];
                 let color = fill.color_or_transparent();
                 verts.push(MultiVertex {
                     position: [x0, y0],
@@ -373,16 +430,16 @@
                  fill: &ColorOrGradient,
                  stroke: &ColorOrGradient,
                  stroke_width: &f32,
                  corner_radius: &f32|
                  -> Result<(Vec<MultiVertex>, Vec<u32>), AvengerWgpuError> {
                     // Create rect path
                     let mut path_builder = lyon::path::Path::builder();
-                    let x0 = *x + bounds.x;
-                    let y0 = *y + bounds.y;
+                    let x0 = *x + origin[0];
+                    let y0 = *y + origin[1];
                     let x1 = x0 + width;
                     let y1 = y0 + height;
                     if *corner_radius > 0.0 {
                         path_builder.add_rounded_rectangle(
                             &Box2D::new(Point2D::new(x0, y0), Point2D::new(x1, y1)),
                             &BorderRadii {
                                 top_left: *corner_radius,
@@ -466,44 +523,46 @@
 
         let start_ind = self.num_indices();
         let inds_len: usize = verts_inds.iter().map(|(_, i)| i.len()).sum();
         let indices_range = (start_ind as u32)..((start_ind + inds_len) as u32);
 
         let batch = MultiMarkBatch {
             indices_range,
-            clip: ClipRect::maybe_from_group_bounds(self.uniform.scale, bounds, mark.clip),
+            clip: clip.maybe_clip(mark.clip),
+            clip_indices_range: self.add_clip_path(clip, mark.clip)?,
             image_atlas_index: None,
             gradient_atlas_index,
             text_atlas_index: None,
         };
 
         self.verts_inds.extend(verts_inds);
         self.batches.push(batch);
         Ok(())
     }
 
     #[tracing::instrument(skip_all)]
     pub fn add_path_mark(
         &mut self,
         mark: &PathMark,
-        bounds: GroupBounds,
+        origin: [f32; 2],
+        clip: &Clip,
     ) -> Result<(), AvengerWgpuError> {
         let (gradient_atlas_index, grad_coords) = self
             .gradient_atlas_builder
             .register_gradients(&mark.gradients);
 
         let build_verts_inds = |path: &lyon::path::Path,
                                 fill: &ColorOrGradient,
                                 stroke: &ColorOrGradient,
                                 transform: &PathTransform|
          -> Result<(Vec<MultiVertex>, Vec<u32>), AvengerWgpuError> {
             // Apply transform to path
             let path = path
                 .clone()
-                .transformed(&transform.then_translate(Vector2D::new(bounds.x, bounds.y)));
+                .transformed(&transform.then_translate(Vector2D::new(origin[0], origin[1])));
             let bbox = bounding_box(&path);
 
             // Create vertex/index buffer builder
             let mut buffers: VertexBuffers<MultiVertex, u32> = VertexBuffers::new();
             let mut builder = BuffersBuilder::new(
                 &mut buffers,
                 crate::marks::multi::VertexPositions {
@@ -566,30 +625,32 @@
 
         let start_ind = self.num_indices();
         let inds_len: usize = verts_inds.iter().map(|(_, i)| i.len()).sum();
         let indices_range = (start_ind as u32)..((start_ind + inds_len) as u32);
 
         let batch = MultiMarkBatch {
             indices_range,
-            clip: ClipRect::maybe_from_group_bounds(self.uniform.scale, bounds, mark.clip),
+            clip: clip.maybe_clip(mark.clip),
+            clip_indices_range: self.add_clip_path(clip, mark.clip)?,
             image_atlas_index: None,
             gradient_atlas_index,
             text_atlas_index: None,
         };
 
         self.verts_inds.extend(verts_inds);
         self.batches.push(batch);
         Ok(())
     }
 
     #[tracing::instrument(skip_all)]
     pub fn add_symbol_mark(
         &mut self,
         mark: &SymbolMark,
-        bounds: GroupBounds,
+        origin: [f32; 2],
+        clip: &Clip,
     ) -> Result<(), AvengerWgpuError> {
         let paths = mark.shapes.iter().map(|s| s.as_path()).collect::<Vec<_>>();
 
         // Compute cradients
         let (gradient_atlas_index, grad_coords) = self
             .gradient_atlas_builder
             .register_gradients(&mark.gradients);
@@ -648,16 +709,16 @@
             let stroke = to_color_or_gradient_coord(stroke, &grad_coords);
 
             let multi_verts = symbol_verts
                 .iter()
                 .map(|sv| {
                     sv.as_multi_vertex(
                         *size,
-                        *x + bounds.x,
-                        *y + bounds.y,
+                        *x + origin[0],
+                        *y + origin[1],
                         *angle,
                         fill,
                         stroke,
                         stroke_width,
                     )
                 })
                 .collect::<Vec<_>>();
@@ -694,48 +755,50 @@
 
         let start_ind = self.num_indices();
         let inds_len: usize = verts_inds.iter().map(|(_, i)| i.len()).sum();
         let indices_range = (start_ind as u32)..((start_ind + inds_len) as u32);
 
         let batch = MultiMarkBatch {
             indices_range,
-            clip: ClipRect::maybe_from_group_bounds(self.uniform.scale, bounds, mark.clip),
+            clip: clip.maybe_clip(mark.clip),
+            clip_indices_range: self.add_clip_path(clip, mark.clip)?,
             image_atlas_index: None,
             gradient_atlas_index,
             text_atlas_index: None,
         };
 
         self.verts_inds.extend(verts_inds);
         self.batches.push(batch);
         Ok(())
     }
 
     #[tracing::instrument(skip_all)]
     pub fn add_line_mark(
         &mut self,
         mark: &LineMark,
-        bounds: GroupBounds,
+        origin: [f32; 2],
+        clip: &Clip,
     ) -> Result<(), AvengerWgpuError> {
         let (gradient_atlas_index, grad_coords) = self
             .gradient_atlas_builder
             .register_gradients(&mark.gradients);
 
         let mut defined_paths: Vec<Path> = Vec::new();
 
         // Build path for each defined line segment
         let mut path_builder = lyon::path::Path::builder().with_svg();
         let mut path_len = 0;
         for (x, y, defined) in izip!(mark.x_iter(), mark.y_iter(), mark.defined_iter()) {
             if *defined {
                 if path_len > 0 {
                     // Continue path
-                    path_builder.line_to(lyon::geom::point(*x + bounds.x, *y + bounds.y));
+                    path_builder.line_to(lyon::geom::point(*x + origin[0], *y + origin[1]));
                 } else {
                     // New path
-                    path_builder.move_to(lyon::geom::point(*x + bounds.x, *y + bounds.y));
+                    path_builder.move_to(lyon::geom::point(*x + origin[0], *y + origin[1]));
                 }
                 path_len += 1;
             } else {
                 if path_len == 1 {
                     // Finishing single point line. Add extra point at the same location
                     // so that stroke caps are drawn
                     path_builder.close();
@@ -838,30 +901,32 @@
         }
 
         let start_ind = self.num_indices();
         let indices_range = (start_ind as u32)..((start_ind + indices.len()) as u32);
 
         let batch = MultiMarkBatch {
             indices_range,
-            clip: ClipRect::maybe_from_group_bounds(self.uniform.scale, bounds, mark.clip),
+            clip: clip.maybe_clip(mark.clip),
+            clip_indices_range: self.add_clip_path(clip, mark.clip)?,
             image_atlas_index: None,
             gradient_atlas_index,
             text_atlas_index: None,
         };
 
         self.verts_inds.push((verts, indices));
         self.batches.push(batch);
         Ok(())
     }
 
     #[tracing::instrument(skip_all)]
     pub fn add_area_mark(
         &mut self,
         mark: &AreaMark,
-        bounds: GroupBounds,
+        origin: [f32; 2],
+        clip: &Clip,
     ) -> Result<(), AvengerWgpuError> {
         let (gradient_atlas_index, grad_coords) = self
             .gradient_atlas_builder
             .register_gradients(&mark.gradients);
 
         let mut path_builder = lyon::path::Path::builder().with_svg();
         let mut tail: Vec<(f32, f32)> = Vec::new();
@@ -884,40 +949,40 @@
                 mark.y_iter(),
                 mark.y2_iter(),
                 mark.defined_iter(),
             ) {
                 if *defined {
                     if !tail.is_empty() {
                         // Continue path
-                        path_builder.line_to(lyon::geom::point(*x + bounds.x, *y + bounds.y));
+                        path_builder.line_to(lyon::geom::point(*x + origin[0], *y + origin[1]));
                     } else {
                         // New path
-                        path_builder.move_to(lyon::geom::point(*x + bounds.x, *y + bounds.y));
+                        path_builder.move_to(lyon::geom::point(*x + origin[0], *y + origin[1]));
                     }
-                    tail.push((*x + bounds.x, *y2 + bounds.y));
+                    tail.push((*x + origin[0], *y2 + origin[1]));
                 } else {
                     close_area(&mut path_builder, &mut tail);
                 }
             }
         } else {
             for (y, x, x2, defined) in izip!(
                 mark.y_iter(),
                 mark.x_iter(),
                 mark.x2_iter(),
                 mark.defined_iter(),
             ) {
                 if *defined {
                     if !tail.is_empty() {
                         // Continue path
-                        path_builder.line_to(lyon::geom::point(*x + bounds.x, *y + bounds.y));
+                        path_builder.line_to(lyon::geom::point(*x + origin[0], *y + origin[1]));
                     } else {
                         // New path
-                        path_builder.move_to(lyon::geom::point(*x + bounds.x, *y + bounds.y));
+                        path_builder.move_to(lyon::geom::point(*x + origin[0], *y + origin[1]));
                     }
-                    tail.push((*x2 + bounds.x, *y + bounds.y));
+                    tail.push((*x2 + origin[0], *y + origin[1]));
                 } else {
                     close_area(&mut path_builder, &mut tail);
                 }
             }
         }
 
         close_area(&mut path_builder, &mut tail);
@@ -961,30 +1026,32 @@
         }
 
         let start_ind = self.num_indices();
         let indices_range = (start_ind as u32)..((start_ind + buffers.indices.len()) as u32);
 
         let batch = MultiMarkBatch {
             indices_range,
-            clip: ClipRect::maybe_from_group_bounds(self.uniform.scale, bounds, mark.clip),
+            clip: clip.maybe_clip(mark.clip),
+            clip_indices_range: self.add_clip_path(clip, mark.clip)?,
             image_atlas_index: None,
             gradient_atlas_index,
             text_atlas_index: None,
         };
 
         self.verts_inds.push((buffers.vertices, buffers.indices));
         self.batches.push(batch);
         Ok(())
     }
 
     #[tracing::instrument(skip_all)]
     pub fn add_trail_mark(
         &mut self,
         mark: &TrailMark,
-        bounds: GroupBounds,
+        origin: [f32; 2],
+        clip: &Clip,
     ) -> Result<(), AvengerWgpuError> {
         let (gradient_atlas_index, grad_coords) = self
             .gradient_atlas_builder
             .register_gradients(&mark.gradients);
 
         let size_idx: AttributeIndex = 0;
         let mut path_builder = lyon::path::Path::builder_with_attributes(1);
@@ -994,18 +1061,19 @@
             mark.y_iter(),
             mark.size_iter(),
             mark.defined_iter()
         ) {
             if *defined {
                 if path_len > 0 {
                     // Continue path
-                    path_builder.line_to(lyon::geom::point(*x + bounds.x, *y + bounds.y), &[*size]);
+                    path_builder
+                        .line_to(lyon::geom::point(*x + origin[0], *y + origin[1]), &[*size]);
                 } else {
                     // New path
-                    path_builder.begin(lyon::geom::point(*x + bounds.x, *y + bounds.y), &[*size]);
+                    path_builder.begin(lyon::geom::point(*x + origin[0], *y + origin[1]), &[*size]);
                 }
                 path_len += 1;
             } else {
                 if path_len == 1 {
                     // Finishing single point line. Add extra point at the same location
                     // so that stroke caps are drawn
                     path_builder.end(true);
@@ -1044,30 +1112,32 @@
         stroke_tessellator.tessellate_path(&path, &stroke_options, &mut buffers_builder)?;
 
         let start_ind = self.num_indices();
         let indices_range = (start_ind as u32)..((start_ind + buffers.indices.len()) as u32);
 
         let batch = MultiMarkBatch {
             indices_range,
-            clip: ClipRect::maybe_from_group_bounds(self.uniform.scale, bounds, mark.clip),
+            clip: clip.maybe_clip(mark.clip),
+            clip_indices_range: self.add_clip_path(clip, mark.clip)?,
             image_atlas_index: None,
             gradient_atlas_index,
             text_atlas_index: None,
         };
 
         self.verts_inds.push((buffers.vertices, buffers.indices));
         self.batches.push(batch);
         Ok(())
     }
 
     #[tracing::instrument(skip_all)]
     pub fn add_arc_mark(
         &mut self,
         mark: &ArcMark,
-        bounds: GroupBounds,
+        origin: [f32; 2],
+        clip: &Clip,
     ) -> Result<(), AvengerWgpuError> {
         let (gradient_atlas_index, grad_coords) = self
             .gradient_atlas_builder
             .register_gradients(&mark.gradients);
 
         let verts_inds = izip!(
             mark.x_iter(),
@@ -1141,15 +1211,15 @@
 
                 path_builder.close();
                 let path = path_builder.build();
 
                 // Transform path to account for start angle and position
                 let path = path.transformed(
                     &PathTransform::rotation(lyon::geom::Angle::radians(*start_angle))
-                        .then_translate(Vector2D::new(*x + bounds.x, *y + bounds.y)),
+                        .then_translate(Vector2D::new(*x + origin[0], *y + origin[1])),
                 );
 
                 // Compute bounding box
                 let bbox = bounding_box(&path);
 
                 // Create vertex/index buffer builder
                 let mut buffers: VertexBuffers<MultiVertex, u32> = VertexBuffers::new();
@@ -1186,42 +1256,44 @@
 
         let start_ind = self.num_indices();
         let inds_len: usize = verts_inds.iter().map(|(_, i)| i.len()).sum();
         let indices_range = (start_ind as u32)..((start_ind + inds_len) as u32);
 
         let batch = MultiMarkBatch {
             indices_range,
-            clip: ClipRect::maybe_from_group_bounds(self.uniform.scale, bounds, mark.clip),
+            clip: clip.maybe_clip(mark.clip),
+            clip_indices_range: self.add_clip_path(clip, mark.clip)?,
             image_atlas_index: None,
             gradient_atlas_index,
             text_atlas_index: None,
         };
 
         self.verts_inds.extend(verts_inds);
         self.batches.push(batch);
         Ok(())
     }
 
     #[tracing::instrument(skip_all)]
     pub fn add_image_mark(
         &mut self,
         mark: &ImageMark,
-        bounds: GroupBounds,
+        origin: [f32; 2],
+        clip: &Clip,
     ) -> Result<(), AvengerWgpuError> {
         let verts_inds = izip!(
             mark.image_iter(),
             mark.x_iter(),
             mark.y_iter(),
             mark.width_iter(),
             mark.height_iter(),
             mark.baseline_iter(),
             mark.align_iter(),
         ).map(|(img, x, y, width, height, baseline, align)| -> Result<(usize, Vec<MultiVertex>, Vec<u32>), AvengerWgpuError> {
-            let x = *x + bounds.x;
-            let y = *y + bounds.y;
+            let x = *x + origin[0];
+            let y = *y + origin[1];
 
             let Some(rgba_image) = img.to_image() else {
                 return Err(AvengerWgpuError::ConversionError("Failed to convert raw image to rgba image".to_string()))
             };
 
             let (atlas_index, tex_coords) = self.image_atlas_builder.register_image(&rgba_image)?;
 
@@ -1298,15 +1370,16 @@
             Ok((atlas_index, verts, indices))
         }).collect::<Result<Vec<_>, AvengerWgpuError>>()?;
 
         // Construct batches, one batch per image atlas index
         let start_ind = self.num_indices() as u32;
         let mut next_batch = MultiMarkBatch {
             indices_range: start_ind..start_ind,
-            clip: ClipRect::maybe_from_group_bounds(self.uniform.scale, bounds, mark.clip),
+            clip: clip.maybe_clip(mark.clip),
+            clip_indices_range: self.add_clip_path(clip, mark.clip)?,
             image_atlas_index: None,
             gradient_atlas_index: None,
             text_atlas_index: None,
         };
 
         for (atlas_index, verts, inds) in verts_inds {
             if next_batch.image_atlas_index.unwrap_or(atlas_index) == atlas_index {
@@ -1316,15 +1389,16 @@
                     ..(next_batch.indices_range.end + inds.len() as u32);
             } else {
                 // create new batch
                 let start_ind = next_batch.indices_range.end;
                 // Initialize new next_batch and swap to avoid extra mem copy
                 let mut full_batch = MultiMarkBatch {
                     indices_range: start_ind..(start_ind + inds.len() as u32),
-                    clip: ClipRect::maybe_from_group_bounds(self.uniform.scale, bounds, mark.clip),
+                    clip: clip.maybe_clip(mark.clip),
+                    clip_indices_range: self.add_clip_path(clip, mark.clip)?,
                     image_atlas_index: Some(atlas_index),
                     gradient_atlas_index: None,
                     text_atlas_index: None,
                 };
                 std::mem::swap(&mut full_batch, &mut next_batch);
                 self.batches.push(full_batch);
             }
@@ -1337,15 +1411,16 @@
         Ok(())
     }
 
     #[tracing::instrument(skip_all)]
     pub fn add_text_mark(
         &mut self,
         mark: &TextMark,
-        bounds: GroupBounds,
+        origin: [f32; 2],
+        clip: &Clip,
     ) -> Result<(), AvengerWgpuError> {
         let registrations = izip!(
             mark.text_iter(),
             mark.x_iter(),
             mark.y_iter(),
             mark.color_iter(),
             mark.align_iter(),
@@ -1370,15 +1445,15 @@
                 font_size,
                 font_weight,
                 font_style,
                 limit,
             )| {
                 let instance = TextInstance {
                     text,
-                    position: [*x + bounds.x, *y + bounds.y],
+                    position: [*x + origin[0], *y + origin[1]],
                     color,
                     align,
                     angle: *angle,
                     baseline,
                     font,
                     font_size: *font_size,
                     font_weight,
@@ -1394,15 +1469,16 @@
         .flatten()
         .collect::<Vec<_>>();
 
         // Construct batches, one batch per text atlas index
         let start_ind = self.num_indices() as u32;
         let mut next_batch = MultiMarkBatch {
             indices_range: start_ind..start_ind,
-            clip: ClipRect::maybe_from_group_bounds(self.uniform.scale, bounds, mark.clip),
+            clip: clip.maybe_clip(mark.clip),
+            clip_indices_range: self.add_clip_path(clip, mark.clip)?,
             image_atlas_index: None,
             gradient_atlas_index: None,
             text_atlas_index: None,
         };
 
         for registration in registrations {
             let atlas_index = registration.atlas_index;
@@ -1417,15 +1493,16 @@
                     ..(next_batch.indices_range.end + inds.len() as u32);
             } else {
                 // create new batch
                 let start_ind = next_batch.indices_range.end;
                 // Initialize new next_batch and swap to avoid extra mem copy
                 let mut full_batch = MultiMarkBatch {
                     indices_range: start_ind..(start_ind + inds.len() as u32),
-                    clip: ClipRect::maybe_from_group_bounds(self.uniform.scale, bounds, mark.clip),
+                    clip: clip.maybe_clip(mark.clip),
+                    clip_indices_range: self.add_clip_path(clip, mark.clip)?,
                     image_atlas_index: None,
                     gradient_atlas_index: None,
                     text_atlas_index: Some(atlas_index),
                 };
                 std::mem::swap(&mut full_batch, &mut next_batch);
                 self.batches.push(full_batch);
             }
@@ -1438,14 +1515,21 @@
         Ok(())
     }
 
     fn num_indices(&self) -> usize {
         self.verts_inds.iter().map(|(_, inds)| inds.len()).sum()
     }
 
+    fn num_clip_indices(&self) -> usize {
+        self.clip_verts_inds
+            .iter()
+            .map(|(_, inds)| inds.len())
+            .sum()
+    }
+
     #[tracing::instrument(skip_all)]
     pub fn render(
         &self,
         device: &Device,
         queue: &Queue,
         texture_format: TextureFormat,
         sample_count: u32,
@@ -1555,87 +1639,238 @@
                 strip_index_format: None,
                 front_face: wgpu::FrontFace::Ccw,
                 cull_mode: Some(wgpu::Face::Back),
                 polygon_mode: wgpu::PolygonMode::Fill,
                 unclipped_depth: false,
                 conservative: false,
             },
-            depth_stencil: None,
+            depth_stencil: Some(wgpu::DepthStencilState {
+                format: wgpu::TextureFormat::Stencil8,
+                depth_write_enabled: false,
+                depth_compare: wgpu::CompareFunction::Always,
+                stencil: wgpu::StencilState {
+                    front: wgpu::StencilFaceState {
+                        // Draw pixel if stencil reference value is less than or equal to stencil value
+                        compare: wgpu::CompareFunction::LessEqual,
+                        ..Default::default()
+                    },
+                    back: wgpu::StencilFaceState::IGNORE,
+                    read_mask: !0,
+                    write_mask: !0,
+                },
+                bias: Default::default(),
+            }),
+            multisample: wgpu::MultisampleState {
+                count: sample_count,
+                mask: !0,
+                alpha_to_coverage_enabled: false,
+            },
+            multiview: None,
+        });
+
+        let stencil_pipeline = device.create_render_pipeline(&wgpu::RenderPipelineDescriptor {
+            label: None,
+            layout: Some(&render_pipeline_layout),
+            vertex: wgpu::VertexState {
+                module: &shader,
+                entry_point: "vs_main",
+                buffers: &[MultiVertex::desc()],
+            },
+            fragment: Some(wgpu::FragmentState {
+                module: &shader,
+                entry_point: "fs_main",
+                targets: &[Some(wgpu::ColorTargetState {
+                    format: texture_format,
+                    blend: None,
+                    write_mask: wgpu::ColorWrites::empty(),
+                })],
+            }),
+            primitive: Default::default(),
+            depth_stencil: Some(wgpu::DepthStencilState {
+                format: wgpu::TextureFormat::Stencil8,
+                depth_write_enabled: false,
+                depth_compare: wgpu::CompareFunction::Always,
+                stencil: wgpu::StencilState {
+                    front: wgpu::StencilFaceState {
+                        compare: wgpu::CompareFunction::Always,
+                        pass_op: wgpu::StencilOperation::Replace,
+                        ..Default::default()
+                    },
+                    back: wgpu::StencilFaceState::IGNORE,
+                    read_mask: !0,
+                    write_mask: !0,
+                },
+                bias: Default::default(),
+            }),
             multisample: wgpu::MultisampleState {
                 count: sample_count,
                 mask: !0,
                 alpha_to_coverage_enabled: false,
             },
             multiview: None,
         });
 
+        let stencil_buffer = device.create_texture(&wgpu::TextureDescriptor {
+            label: Some("Stencil buffer"),
+            size: Extent3d {
+                width: self.dimensions.to_physical_width(),
+                height: self.dimensions.to_physical_height(),
+                depth_or_array_layers: 1,
+            },
+            mip_level_count: 1,
+            sample_count,
+            dimension: wgpu::TextureDimension::D2,
+            format: wgpu::TextureFormat::Stencil8,
+            view_formats: &[],
+            usage: wgpu::TextureUsages::RENDER_ATTACHMENT,
+        });
+
         // flatten verts and inds
         let num_verts: usize = self.verts_inds.iter().map(|(v, _)| v.len()).sum();
         let num_inds: usize = self.verts_inds.iter().map(|(_, inds)| inds.len()).sum();
         let mut verticies: Vec<MultiVertex> = Vec::with_capacity(num_verts);
         let mut indices: Vec<u32> = Vec::with_capacity(num_inds);
 
         for (vs, inds) in &self.verts_inds {
             let offset = verticies.len() as u32;
             indices.extend(inds.iter().map(|i| *i + offset));
             verticies.extend(vs);
         }
 
+        let num_clip_verts = self.clip_verts_inds.iter().map(|(v, _)| v.len()).sum();
+        let num_clip_inds = self
+            .clip_verts_inds
+            .iter()
+            .map(|(_, inds)| inds.len())
+            .sum();
+        let mut clip_verticies: Vec<MultiVertex> = Vec::with_capacity(num_clip_verts);
+        let mut clip_indices: Vec<u32> = Vec::with_capacity(num_clip_inds);
+
+        for (vs, inds) in &self.clip_verts_inds {
+            let offset = clip_verticies.len() as u32;
+            clip_indices.extend(inds.iter().map(|i| *i + offset));
+            clip_verticies.extend(vs);
+        }
+
         // Create vertex and index buffers
         let vertex_buffer = device.create_buffer_init(&wgpu::util::BufferInitDescriptor {
             label: Some("Vertex Buffer"),
             contents: bytemuck::cast_slice(verticies.as_slice()),
             usage: wgpu::BufferUsages::VERTEX,
         });
 
         let index_buffer = device.create_buffer_init(&wgpu::util::BufferInitDescriptor {
             label: Some("Index Buffer"),
             contents: bytemuck::cast_slice(indices.as_slice()),
             usage: wgpu::BufferUsages::INDEX,
         });
 
+        let clip_vertex_buffer = device.create_buffer_init(&wgpu::util::BufferInitDescriptor {
+            label: Some("Clip Vertex Buffer"),
+            contents: bytemuck::cast_slice(clip_verticies.as_slice()),
+            usage: wgpu::BufferUsages::VERTEX,
+        });
+
+        let clip_index_buffer = device.create_buffer_init(&wgpu::util::BufferInitDescriptor {
+            label: Some("Clip Index Buffer"),
+            contents: bytemuck::cast_slice(clip_indices.as_slice()),
+            usage: wgpu::BufferUsages::INDEX,
+        });
+
         // Create command encoder for marks
         let mut mark_encoder = device.create_command_encoder(&wgpu::CommandEncoderDescriptor {
             label: Some("Multi Mark Render Encoder"),
         });
 
         // Render batches
         {
+            let depth_view = stencil_buffer.create_view(&Default::default());
             let mut render_pass = mark_encoder.begin_render_pass(&wgpu::RenderPassDescriptor {
                 label: Some("Multi Mark Render Pass"),
                 color_attachments: &[Some(wgpu::RenderPassColorAttachment {
                     view: texture_view,
                     resolve_target,
                     ops: wgpu::Operations {
                         load: wgpu::LoadOp::Load,
                         store: wgpu::StoreOp::Store,
                     },
                 })],
-                depth_stencil_attachment: None,
+                depth_stencil_attachment: Some(wgpu::RenderPassDepthStencilAttachment {
+                    view: &depth_view,
+                    depth_ops: if cfg!(feature = "deno") {
+                        // depth_ops shouldn't be needed, but setting to None results in validation
+                        // error in Deno. However, setting it to the below causes a validation error
+                        // in Chrome.
+                        Some(wgpu::Operations {
+                            load: wgpu::LoadOp::Clear(0.0),
+                            store: wgpu::StoreOp::Discard,
+                        })
+                    } else {
+                        None
+                    },
+                    stencil_ops: Some(wgpu::Operations {
+                        load: wgpu::LoadOp::Clear(0),
+                        store: wgpu::StoreOp::Store,
+                    }),
+                }),
                 occlusion_query_set: None,
                 timestamp_writes: None,
             });
 
             render_pass.set_pipeline(&render_pipeline);
             render_pass.set_bind_group(0, &uniform_bind_group, &[]);
             let mut last_grad_ind = 0;
             let mut last_img_ind = 0;
             let mut last_text_ind = 0;
+            let mut stencil_index: u32 = 1;
             render_pass.set_bind_group(1, &gradient_texture_bind_groups[last_grad_ind], &[]);
             render_pass.set_bind_group(2, &image_texture_bind_groups[last_img_ind], &[]);
             render_pass.set_bind_group(3, &text_texture_bind_groups[last_img_ind], &[]);
             render_pass.set_vertex_buffer(0, vertex_buffer.slice(..));
             render_pass.set_index_buffer(index_buffer.slice(..), wgpu::IndexFormat::Uint32);
 
             // Initialze textures with first entry
             for batch in &self.batches {
-                // Update clip
-                if let Some(clip) = batch.clip {
-                    render_pass.set_scissor_rect(clip.x, clip.y, clip.width, clip.height);
+                if let Some(clip_inds_range) = &batch.clip_indices_range {
+                    render_pass.set_stencil_reference(stencil_index);
+                    render_pass.set_pipeline(&stencil_pipeline);
+                    render_pass.set_vertex_buffer(0, clip_vertex_buffer.slice(..));
+                    render_pass
+                        .set_index_buffer(clip_index_buffer.slice(..), wgpu::IndexFormat::Uint32);
+                    render_pass.draw_indexed(clip_inds_range.clone(), 0, 0..1);
+
+                    // Restore buffers
+                    render_pass.set_pipeline(&render_pipeline);
+                    render_pass.set_vertex_buffer(0, vertex_buffer.slice(..));
+                    render_pass.set_index_buffer(index_buffer.slice(..), wgpu::IndexFormat::Uint32);
+
+                    // increment stencil index for next draw
+                    stencil_index += 1;
+                } else {
+                    // Set stencil reference back to zero so that everything is drawn
+                    render_pass.set_stencil_reference(0);
+                }
+
+                // Update scissors
+                if let Clip::Rect {
+                    x,
+                    y,
+                    width,
+                    height,
+                } = batch.clip
+                {
+                    // Set scissors rect
+                    render_pass.set_scissor_rect(
+                        (x * self.uniform.scale) as u32,
+                        (y * self.uniform.scale) as u32,
+                        (width * self.uniform.scale) as u32,
+                        (height * self.uniform.scale) as u32,
+                    );
                 } else {
+                    // Clear scissors rect
                     render_pass.set_scissor_rect(
                         0,
                         0,
                         self.dimensions.to_physical_width(),
                         self.dimensions.to_physical_height(),
                     );
                 }
```

### Comparing `avenger-0.0.3/avenger-wgpu/src/marks/multi.wgsl` & `avenger-0.0.4/avenger-wgpu/src/marks/multi.wgsl`

 * *Files 14% similar despite different names*

```diff
@@ -74,25 +74,31 @@
 const GRADIENT_RADIAL = 1.0;
 const COLORWAY_LENGTH = 250.0;
 const GRADIENT_TEXTURE_WIDTH = 256.0;
 const GRADIENT_TEXTURE_HEIGHT = 256.0;
 
 // Compute final color, potentially computing gradient
 fn lookup_color(color: vec4<f32>, clip_position: vec4<f32>, top_left: vec2<f32>, bottom_right: vec2<f32>) -> vec4<f32> {
+    // Use textureSampleGrad instead of textureSample to avoid Uniform Control Flow error in WebGPU
+    // https://github.com/gpuweb/gpuweb/discussions/2899
+    let texXy = vec2<f32>(clip_position[0], clip_position[1]);
+    let dx = dpdx(texXy);
+    let dy = dpdx(texXy);
+
     if (color[0] == GRADIENT_TEXTURE_CODE) {
         // If the first color coordinate is a negative value, this indicates that we are computing a color from a texture
         // For gradient texture, the second color component stores the gradient texture y-coordinate
         let tex_coord_y = color[1];
 
         // Extract gradient type from fist pixel
-        let control0 = textureSample(gradient_texture, gradient_sampler, vec2<f32>(0.0, tex_coord_y));
+        let control0 = textureSampleGrad(gradient_texture, gradient_sampler, vec2<f32>(0.0, tex_coord_y), dx, dy);
         let gradient_type = control0[0];
 
         // Extract x/y control points from second pixel
-        let control1 = textureSample(gradient_texture, gradient_sampler, vec2<f32>(1.0 / GRADIENT_TEXTURE_WIDTH, tex_coord_y));
+        let control1 = textureSampleGrad(gradient_texture, gradient_sampler, vec2<f32>(1.0 / GRADIENT_TEXTURE_WIDTH, tex_coord_y), dx, dy);
         let x0 = control1[0];
         let y0 = control1[1];
         let x1 = control1[2];
         let y1 = control1[3];
         let p0 = vec2<f32>(x0, y0);
         let p1 = vec2<f32>(x1, y1);
 
@@ -103,19 +109,19 @@
            // Convert fragment coordinate into coordinate normalized to rect bounding box
             let norm_xy = (frag_xy - top_left) / width_height;
 
             let control_dist = distance(p0, p1);
             let projected_dist = dot(norm_xy - p0, p1 - p0) / control_dist;
 
             let tex_coord_x = compute_tex_x_coord(projected_dist / control_dist);
-
-            return textureSample(gradient_texture, gradient_sampler, vec2<f32>(tex_coord_x, tex_coord_y));
+            let tex_coords = vec2<f32>(tex_coord_x, tex_coord_y);
+            return textureSampleGrad(gradient_texture, gradient_sampler, tex_coords, dx, dy);
         } else {
            // Extract additional radius gradient control points from third pixel
-            let control2 = textureSample(gradient_texture, gradient_sampler, vec2<f32>(2.0 / GRADIENT_TEXTURE_WIDTH, tex_coord_y));
+            let control2 = textureSampleGrad(gradient_texture, gradient_sampler, vec2<f32>(2.0 / GRADIENT_TEXTURE_WIDTH, tex_coord_y), dx, dy);
             let r0 = control2[0];
             let r1 = control2[1];
 
             // Expand top_left and bottom_right so they form a square
             var square_top_left: vec2<f32>;
             var square_bottom_right: vec2<f32>;
             var side: f32;
@@ -181,24 +187,25 @@
                     -pow(d,2.0) + pow(r1,2.0)
                 );
                 frag_radius = r1 * t;
             }
 
             let grad_dist = (frag_radius - r0) / r_delta;
             let tex_coord_x = compute_tex_x_coord(grad_dist);
-            return textureSample(gradient_texture, gradient_sampler, vec2<f32>(tex_coord_x, tex_coord_y));
+            let tex_coords = vec2<f32>(tex_coord_x, tex_coord_y);
+            return textureSampleGrad(gradient_texture, gradient_sampler, tex_coords, dx, dy);
         }
     } else if (color[0] == IMAGE_TEXTURE_CODE) {
         // Image texture coordinates are stored in the second and third color components
         let tex_coords = vec2<f32>(color[1], color[2]);
-        return textureSample(image_texture, image_sampler, tex_coords);
+        return textureSampleGrad(image_texture, image_sampler, tex_coords, dx, dy);
     } else if (color[0] == TEXT_TEXTURE_CODE) {
         // Text texture coordinates are stored in the second and third color components
         let tex_coords = vec2<f32>(color[1], color[2]);
-        return textureSample(text_texture, text_sampler, tex_coords);
+        return textureSampleGrad(text_texture, text_sampler, tex_coords, dx, dy);
     } else {
         return color;
     }
 }
 
 fn compute_tex_x_coord(grad_dist: f32) -> f32 {
     let col_offset = GRADIENT_TEXTURE_WIDTH - COLORWAY_LENGTH;
```

### Comparing `avenger-0.0.3/avenger-wgpu/src/marks/symbol.rs` & `avenger-0.0.4/avenger-wgpu/src/marks/symbol.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 use crate::canvas::CanvasDimensions;
 use crate::error::AvengerWgpuError;
 use crate::marks::instanced_mark::{InstancedMarkBatch, InstancedMarkShader};
-use avenger::marks::group::GroupBounds;
 use avenger::marks::path::PathTransform;
 use avenger::marks::symbol::SymbolMark;
 use itertools::izip;
 use lyon::lyon_tessellation::{
     BuffersBuilder, FillVertex, FillVertexConstructor, StrokeVertex, StrokeVertexConstructor,
 };
 use lyon::tessellation::geometry_builder::VertexBuffers;
@@ -21,19 +20,19 @@
     pub size: [f32; 2],
     pub origin: [f32; 2],
     pub scale: f32,
     _pad: [f32; 5],
 }
 
 impl SymbolUniform {
-    pub fn new(dimensions: CanvasDimensions, group_bounds: GroupBounds) -> Self {
+    pub fn new(dimensions: CanvasDimensions, origin: [f32; 2]) -> Self {
         Self {
             size: dimensions.size,
             scale: dimensions.scale,
-            origin: [group_bounds.x, group_bounds.y],
+            origin,
             _pad: [0.0, 0.0, 0.0, 0.0, 0.0],
         }
     }
 }
 
 #[repr(C)]
 #[derive(Copy, Clone, Debug, bytemuck::Pod, bytemuck::Zeroable)]
@@ -129,15 +128,15 @@
     fragment_entry_point: String,
 }
 
 impl SymbolShader {
     pub fn from_symbol_mark(
         mark: &SymbolMark,
         dimensions: CanvasDimensions,
-        group_bounds: GroupBounds,
+        origin: [f32; 2],
     ) -> Result<Self, AvengerWgpuError> {
         let shapes = &mark.shapes;
         let max_size = mark.max_size();
         let max_scale = max_size.sqrt();
         let mut verts: Vec<SymbolVertex> = Vec::new();
         let mut indices: Vec<u16> = Vec::new();
         for (shape_index, shape) in shapes.iter().enumerate() {
@@ -176,15 +175,15 @@
             instances_range: 0..instances.len() as u32,
             image: img,
         }];
         Ok(Self {
             verts,
             indices,
             instances,
-            uniform: SymbolUniform::new(dimensions, group_bounds),
+            uniform: SymbolUniform::new(dimensions, origin),
             batches,
             texture_size,
             shader: include_str!("symbol.wgsl").into(),
             vertex_entry_point: "vs_main".to_string(),
             fragment_entry_point: "fs_main".to_string(),
         })
     }
```

### Comparing `avenger-0.0.3/avenger-wgpu/src/marks/symbol.wgsl` & `avenger-0.0.4/avenger-wgpu/src/marks/symbol.wgsl`

 * *Files identical despite different names*

### Comparing `avenger-0.0.3/avenger-wgpu/src/util.rs` & `avenger-0.0.4/avenger-wgpu/src/util.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.3/avenger-wgpu/tests/test_image_baselines.rs` & `avenger-0.0.4/avenger-wgpu/tests/test_image_baselines.rs`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         case("symbol", "mixed_symbols", 0.001),
         case("rule", "wide_rule_axes", 0.0001),
 
         // lyon seems to omit closing square cap, need to investigate
         case("rule", "wide_transparent_caps", 0.08),
         case("rule", "dashed_rules", 0.004),
 
-        case("text", "bar_axis_labels", 0.03),
+        case("text", "bar_axis_labels", 0.033),
         case("text", "text_alignment", 0.015),
         case("text", "text_rotation", 0.015),
         case("text", "letter_scatter", 0.03),
         case("text", "lasagna_plot", 0.02),
         case("text", "arc_radial", 0.01),
 
         // vl-convert doesn't support emoji at all
@@ -174,14 +174,17 @@
         case("vl-convert", "table_heatmap", 0.04),
         case("vl-convert", "stacked_bar_h", 0.02),
         case("vl-convert", "geoScale", 0.01),
         case("vl-convert", "maptile_background", 0.01),
         case("vl-convert", "no_text_in_font_metrics", 0.03),
         case("clip", "clip_mixed_marks", 0.0001),
         case("clip", "text_clip", 0.02),
+        case("clip", "clip_rounded", 0.0001),
+        case("clip", "text_clip_rounded", 0.02),
+        case("clip", "bar_rounded", 0.02),
     )]
     fn test_image_baseline(category: &str, spec_name: &str, tolerance: f64) {
         initialize();
 
         println!("{spec_name}");
         let specs_dir = format!(
             "{}/../avenger-vega-test-data/vega-scenegraphs/{category}",
@@ -207,18 +210,21 @@
         // Build scene graph
         let scene_graph: SceneGraph = scene_spec
             .to_scene_graph()
             .expect("Failed to parse scene graph");
 
         // println!("{}", serde_json::to_string_pretty(&scene_graph).unwrap());
 
-        let mut png_canvas = pollster::block_on(PngCanvas::new(CanvasDimensions {
-            size: [scene_graph.width, scene_graph.height],
-            scale: 2.0,
-        }))
+        let mut png_canvas = pollster::block_on(PngCanvas::new(
+            CanvasDimensions {
+                size: [scene_graph.width, scene_graph.height],
+                scale: 2.0,
+            },
+            Default::default(),
+        ))
         .unwrap();
         png_canvas.set_scene(&scene_graph).unwrap();
         let img = pollster::block_on(png_canvas.render()).expect("Failed to render PNG image");
         let result_path = format!("{output_dir}/{category}-{spec_name}.png");
         img.save(&result_path).unwrap();
         let result_dssim = dssim::load_image(&Dssim::new(), result_path).unwrap();
```

### Comparing `avenger-0.0.3/avenger/src/marks/arc.rs` & `avenger-0.0.4/avenger/src/marks/arc.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.3/avenger/src/marks/area.rs` & `avenger-0.0.4/avenger/src/marks/area.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.3/avenger/src/marks/image.rs` & `avenger-0.0.4/avenger/src/marks/rule.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,80 @@
-use crate::marks::value::{EncodingValue, ImageAlign, ImageBaseline};
+use crate::marks::value::{ColorOrGradient, EncodingValue, Gradient, StrokeCap};
 use serde::{Deserialize, Serialize};
 
 #[derive(Debug, Clone, Serialize, Deserialize)]
 #[serde(rename_all = "kebab-case")]
-pub struct ImageMark {
+pub struct RuleMark {
     pub name: String,
     pub clip: bool,
     pub len: u32,
-    pub aspect: bool,
-    pub smooth: bool,
-    pub image: EncodingValue<RgbaImage>,
-    pub x: EncodingValue<f32>,
-    pub y: EncodingValue<f32>,
-    pub width: EncodingValue<f32>,
-    pub height: EncodingValue<f32>,
-    pub align: EncodingValue<ImageAlign>,
-    pub baseline: EncodingValue<ImageBaseline>,
+    pub gradients: Vec<Gradient>,
+    pub stroke_dash: Option<EncodingValue<Vec<f32>>>,
+    pub x0: EncodingValue<f32>,
+    pub y0: EncodingValue<f32>,
+    pub x1: EncodingValue<f32>,
+    pub y1: EncodingValue<f32>,
+    pub stroke: EncodingValue<ColorOrGradient>,
+    pub stroke_width: EncodingValue<f32>,
+    pub stroke_cap: EncodingValue<StrokeCap>,
     pub indices: Option<Vec<usize>>,
     pub zindex: Option<i32>,
 }
 
-impl ImageMark {
-    pub fn image_iter(&self) -> Box<dyn Iterator<Item = &RgbaImage> + '_> {
-        self.image.as_iter(self.len as usize, self.indices.as_ref())
+impl RuleMark {
+    pub fn x0_iter(&self) -> Box<dyn Iterator<Item = &f32> + '_> {
+        self.x0.as_iter(self.len as usize, self.indices.as_ref())
     }
-    pub fn x_iter(&self) -> Box<dyn Iterator<Item = &f32> + '_> {
-        self.x.as_iter(self.len as usize, self.indices.as_ref())
+    pub fn y0_iter(&self) -> Box<dyn Iterator<Item = &f32> + '_> {
+        self.y0.as_iter(self.len as usize, self.indices.as_ref())
     }
-    pub fn y_iter(&self) -> Box<dyn Iterator<Item = &f32> + '_> {
-        self.y.as_iter(self.len as usize, self.indices.as_ref())
+    pub fn x1_iter(&self) -> Box<dyn Iterator<Item = &f32> + '_> {
+        self.x1.as_iter(self.len as usize, self.indices.as_ref())
     }
-    pub fn width_iter(&self) -> Box<dyn Iterator<Item = &f32> + '_> {
-        self.width.as_iter(self.len as usize, self.indices.as_ref())
+    pub fn y1_iter(&self) -> Box<dyn Iterator<Item = &f32> + '_> {
+        self.y1.as_iter(self.len as usize, self.indices.as_ref())
     }
-    pub fn height_iter(&self) -> Box<dyn Iterator<Item = &f32> + '_> {
-        self.height
+    pub fn stroke_iter(&self) -> Box<dyn Iterator<Item = &ColorOrGradient> + '_> {
+        self.stroke
             .as_iter(self.len as usize, self.indices.as_ref())
     }
-    pub fn align_iter(&self) -> Box<dyn Iterator<Item = &ImageAlign> + '_> {
-        self.align.as_iter(self.len as usize, self.indices.as_ref())
+    pub fn stroke_width_iter(&self) -> Box<dyn Iterator<Item = &f32> + '_> {
+        self.stroke_width
+            .as_iter(self.len as usize, self.indices.as_ref())
     }
-    pub fn baseline_iter(&self) -> Box<dyn Iterator<Item = &ImageBaseline> + '_> {
-        self.baseline
+    pub fn stroke_cap_iter(&self) -> Box<dyn Iterator<Item = &StrokeCap> + '_> {
+        self.stroke_cap
             .as_iter(self.len as usize, self.indices.as_ref())
     }
-}
-
-#[derive(Debug, Clone, Serialize, Deserialize)]
-pub struct RgbaImage {
-    pub width: u32,
-    pub height: u32,
-    pub data: Vec<u8>,
-}
-
-impl RgbaImage {
-    pub fn to_image(&self) -> Option<image::RgbaImage> {
-        image::RgbaImage::from_raw(self.width, self.height, self.data.clone())
+    pub fn stroke_dash_iter(&self) -> Option<Box<dyn Iterator<Item = &Vec<f32>> + '_>> {
+        if let Some(stroke_dash) = &self.stroke_dash {
+            Some(stroke_dash.as_iter(self.len as usize, self.indices.as_ref()))
+        } else {
+            None
+        }
     }
+}
 
-    pub fn from_image(img: &image::RgbaImage) -> Self {
+impl Default for RuleMark {
+    fn default() -> Self {
         Self {
-            width: img.width(),
-            height: img.height(),
-            data: img.to_vec(),
+            name: "rule_mark".to_string(),
+            clip: true,
+            len: 1,
+            gradients: vec![],
+            stroke_dash: None,
+            x0: EncodingValue::Scalar { value: 0.0 },
+            y0: EncodingValue::Scalar { value: 0.0 },
+            x1: EncodingValue::Scalar { value: 0.0 },
+            y1: EncodingValue::Scalar { value: 0.0 },
+            stroke: EncodingValue::Scalar {
+                value: ColorOrGradient::Color([0.0, 0.0, 0.0, 1.0]),
+            },
+            stroke_width: EncodingValue::Scalar { value: 1.0 },
+            stroke_cap: EncodingValue::Scalar {
+                value: StrokeCap::Butt,
+            },
+            indices: None,
+            zindex: None,
         }
     }
 }
```

### Comparing `avenger-0.0.3/avenger/src/marks/line.rs` & `avenger-0.0.4/avenger/src/marks/line.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.3/avenger/src/marks/mark.rs` & `avenger-0.0.4/avenger/src/marks/mark.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.3/avenger/src/marks/path.rs` & `avenger-0.0.4/avenger/src/marks/path.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.3/avenger/src/marks/rect.rs` & `avenger-0.0.4/avenger/src/marks/rect.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.3/avenger/src/marks/rule.rs` & `avenger-0.0.4/avenger/src/marks/image.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,80 +1,95 @@
-use crate::marks::value::{ColorOrGradient, EncodingValue, Gradient, StrokeCap};
+use crate::marks::value::{EncodingValue, ImageAlign, ImageBaseline};
 use serde::{Deserialize, Serialize};
 
 #[derive(Debug, Clone, Serialize, Deserialize)]
 #[serde(rename_all = "kebab-case")]
-pub struct RuleMark {
+pub struct ImageMark {
     pub name: String,
     pub clip: bool,
     pub len: u32,
-    pub gradients: Vec<Gradient>,
-    pub stroke_dash: Option<EncodingValue<Vec<f32>>>,
-    pub x0: EncodingValue<f32>,
-    pub y0: EncodingValue<f32>,
-    pub x1: EncodingValue<f32>,
-    pub y1: EncodingValue<f32>,
-    pub stroke: EncodingValue<ColorOrGradient>,
-    pub stroke_width: EncodingValue<f32>,
-    pub stroke_cap: EncodingValue<StrokeCap>,
+    pub aspect: bool,
+    pub smooth: bool,
+    pub image: EncodingValue<RgbaImage>,
+    pub x: EncodingValue<f32>,
+    pub y: EncodingValue<f32>,
+    pub width: EncodingValue<f32>,
+    pub height: EncodingValue<f32>,
+    pub align: EncodingValue<ImageAlign>,
+    pub baseline: EncodingValue<ImageBaseline>,
     pub indices: Option<Vec<usize>>,
     pub zindex: Option<i32>,
 }
 
-impl RuleMark {
-    pub fn x0_iter(&self) -> Box<dyn Iterator<Item = &f32> + '_> {
-        self.x0.as_iter(self.len as usize, self.indices.as_ref())
+impl ImageMark {
+    pub fn image_iter(&self) -> Box<dyn Iterator<Item = &RgbaImage> + '_> {
+        self.image.as_iter(self.len as usize, self.indices.as_ref())
     }
-    pub fn y0_iter(&self) -> Box<dyn Iterator<Item = &f32> + '_> {
-        self.y0.as_iter(self.len as usize, self.indices.as_ref())
+    pub fn x_iter(&self) -> Box<dyn Iterator<Item = &f32> + '_> {
+        self.x.as_iter(self.len as usize, self.indices.as_ref())
     }
-    pub fn x1_iter(&self) -> Box<dyn Iterator<Item = &f32> + '_> {
-        self.x1.as_iter(self.len as usize, self.indices.as_ref())
+    pub fn y_iter(&self) -> Box<dyn Iterator<Item = &f32> + '_> {
+        self.y.as_iter(self.len as usize, self.indices.as_ref())
     }
-    pub fn y1_iter(&self) -> Box<dyn Iterator<Item = &f32> + '_> {
-        self.y1.as_iter(self.len as usize, self.indices.as_ref())
+    pub fn width_iter(&self) -> Box<dyn Iterator<Item = &f32> + '_> {
+        self.width.as_iter(self.len as usize, self.indices.as_ref())
     }
-    pub fn stroke_iter(&self) -> Box<dyn Iterator<Item = &ColorOrGradient> + '_> {
-        self.stroke
+    pub fn height_iter(&self) -> Box<dyn Iterator<Item = &f32> + '_> {
+        self.height
             .as_iter(self.len as usize, self.indices.as_ref())
     }
-    pub fn stroke_width_iter(&self) -> Box<dyn Iterator<Item = &f32> + '_> {
-        self.stroke_width
-            .as_iter(self.len as usize, self.indices.as_ref())
+    pub fn align_iter(&self) -> Box<dyn Iterator<Item = &ImageAlign> + '_> {
+        self.align.as_iter(self.len as usize, self.indices.as_ref())
     }
-    pub fn stroke_cap_iter(&self) -> Box<dyn Iterator<Item = &StrokeCap> + '_> {
-        self.stroke_cap
+    pub fn baseline_iter(&self) -> Box<dyn Iterator<Item = &ImageBaseline> + '_> {
+        self.baseline
             .as_iter(self.len as usize, self.indices.as_ref())
     }
-    pub fn stroke_dash_iter(&self) -> Option<Box<dyn Iterator<Item = &Vec<f32>> + '_>> {
-        if let Some(stroke_dash) = &self.stroke_dash {
-            Some(stroke_dash.as_iter(self.len as usize, self.indices.as_ref()))
-        } else {
-            None
-        }
-    }
 }
 
-impl Default for RuleMark {
+impl Default for ImageMark {
     fn default() -> Self {
         Self {
-            name: "rule_mark".to_string(),
+            name: "image_mark".to_string(),
             clip: true,
             len: 1,
-            gradients: vec![],
-            stroke_dash: None,
-            x0: EncodingValue::Scalar { value: 0.0 },
-            y0: EncodingValue::Scalar { value: 0.0 },
-            x1: EncodingValue::Scalar { value: 0.0 },
-            y1: EncodingValue::Scalar { value: 0.0 },
-            stroke: EncodingValue::Scalar {
-                value: ColorOrGradient::Color([0.0, 0.0, 0.0, 1.0]),
+            aspect: true,
+            indices: None,
+            smooth: true,
+            x: EncodingValue::Scalar { value: 0.0 },
+            y: EncodingValue::Scalar { value: 0.0 },
+            width: EncodingValue::Scalar { value: 0.0 },
+            height: EncodingValue::Scalar { value: 0.0 },
+            align: EncodingValue::Scalar {
+                value: Default::default(),
             },
-            stroke_width: EncodingValue::Scalar { value: 1.0 },
-            stroke_cap: EncodingValue::Scalar {
-                value: StrokeCap::Butt,
+            baseline: EncodingValue::Scalar {
+                value: Default::default(),
+            },
+            image: EncodingValue::Scalar {
+                value: Default::default(),
             },
-            indices: None,
             zindex: None,
         }
     }
 }
+
+#[derive(Debug, Clone, Default, Serialize, Deserialize)]
+pub struct RgbaImage {
+    pub width: u32,
+    pub height: u32,
+    pub data: Vec<u8>,
+}
+
+impl RgbaImage {
+    pub fn to_image(&self) -> Option<image::RgbaImage> {
+        image::RgbaImage::from_raw(self.width, self.height, self.data.clone())
+    }
+
+    pub fn from_image(img: &image::RgbaImage) -> Self {
+        Self {
+            width: img.width(),
+            height: img.height(),
+            data: img.to_vec(),
+        }
+    }
+}
```

### Comparing `avenger-0.0.3/avenger/src/marks/symbol.rs` & `avenger-0.0.4/avenger/src/marks/text.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,143 +1,155 @@
-use crate::marks::value::{ColorOrGradient, EncodingValue, Gradient};
-use lyon_path::Winding;
+use crate::marks::value::EncodingValue;
 use serde::{Deserialize, Serialize};
-use std::borrow::Cow;
 
 #[derive(Debug, Clone, Serialize, Deserialize)]
 #[serde(rename_all = "kebab-case")]
-pub struct SymbolMark {
+pub struct TextMark {
     pub name: String,
     pub clip: bool,
     pub len: u32,
-    pub gradients: Vec<Gradient>,
-    pub shapes: Vec<SymbolShape>,
-    pub stroke_width: Option<f32>,
-    pub shape_index: EncodingValue<usize>,
+    pub text: EncodingValue<String>,
     pub x: EncodingValue<f32>,
     pub y: EncodingValue<f32>,
-    pub fill: EncodingValue<ColorOrGradient>,
-    pub size: EncodingValue<f32>,
-    pub stroke: EncodingValue<ColorOrGradient>,
+    pub align: EncodingValue<TextAlignSpec>,
+    pub baseline: EncodingValue<TextBaselineSpec>,
     pub angle: EncodingValue<f32>,
+    pub color: EncodingValue<[f32; 4]>,
+    pub font: EncodingValue<String>,
+    pub font_size: EncodingValue<f32>,
+    pub font_weight: EncodingValue<FontWeightSpec>,
+    pub font_style: EncodingValue<FontStyleSpec>,
+    pub limit: EncodingValue<f32>,
     pub indices: Option<Vec<usize>>,
     pub zindex: Option<i32>,
 }
 
-impl SymbolMark {
+impl TextMark {
+    pub fn text_iter(&self) -> Box<dyn Iterator<Item = &String> + '_> {
+        self.text.as_iter(self.len as usize, self.indices.as_ref())
+    }
     pub fn x_iter(&self) -> Box<dyn Iterator<Item = &f32> + '_> {
         self.x.as_iter(self.len as usize, self.indices.as_ref())
     }
-
-    pub fn x_vec(&self) -> Vec<f32> {
-        self.x.as_vec(self.len as usize, self.indices.as_ref())
-    }
-
     pub fn y_iter(&self) -> Box<dyn Iterator<Item = &f32> + '_> {
         self.y.as_iter(self.len as usize, self.indices.as_ref())
     }
-
-    pub fn y_vec(&self) -> Vec<f32> {
-        self.y.as_vec(self.len as usize, self.indices.as_ref())
-    }
-
-    pub fn fill_iter(&self) -> Box<dyn Iterator<Item = &ColorOrGradient> + '_> {
-        self.fill.as_iter(self.len as usize, self.indices.as_ref())
-    }
-
-    pub fn fill_vec(&self) -> Vec<ColorOrGradient> {
-        self.fill.as_vec(self.len as usize, self.indices.as_ref())
+    pub fn align_iter(&self) -> Box<dyn Iterator<Item = &TextAlignSpec> + '_> {
+        self.align.as_iter(self.len as usize, self.indices.as_ref())
     }
-
-    pub fn size_iter(&self) -> Box<dyn Iterator<Item = &f32> + '_> {
-        self.size.as_iter(self.len as usize, self.indices.as_ref())
-    }
-
-    pub fn size_vec(&self) -> Vec<f32> {
-        self.size.as_vec(self.len as usize, self.indices.as_ref())
-    }
-
-    pub fn stroke_iter(&self) -> Box<dyn Iterator<Item = &ColorOrGradient> + '_> {
-        self.stroke
+    pub fn baseline_iter(&self) -> Box<dyn Iterator<Item = &TextBaselineSpec> + '_> {
+        self.baseline
             .as_iter(self.len as usize, self.indices.as_ref())
     }
-
-    pub fn stroke_vec(&self) -> Vec<ColorOrGradient> {
-        self.stroke.as_vec(self.len as usize, self.indices.as_ref())
-    }
-
     pub fn angle_iter(&self) -> Box<dyn Iterator<Item = &f32> + '_> {
         self.angle.as_iter(self.len as usize, self.indices.as_ref())
     }
-
-    pub fn angle_vec(&self) -> Vec<f32> {
-        self.angle.as_vec(self.len as usize, self.indices.as_ref())
+    pub fn color_iter(&self) -> Box<dyn Iterator<Item = &[f32; 4]> + '_> {
+        self.color.as_iter(self.len as usize, self.indices.as_ref())
     }
-
-    pub fn shape_index_iter(&self) -> Box<dyn Iterator<Item = &usize> + '_> {
-        self.shape_index
+    pub fn font_iter(&self) -> Box<dyn Iterator<Item = &String> + '_> {
+        self.font.as_iter(self.len as usize, self.indices.as_ref())
+    }
+    pub fn font_size_iter(&self) -> Box<dyn Iterator<Item = &f32> + '_> {
+        self.font_size
             .as_iter(self.len as usize, self.indices.as_ref())
     }
-
-    pub fn shape_index_vec(&self) -> Vec<usize> {
-        self.shape_index
-            .as_vec(self.len as usize, self.indices.as_ref())
+    pub fn font_weight_iter(&self) -> Box<dyn Iterator<Item = &FontWeightSpec> + '_> {
+        self.font_weight
+            .as_iter(self.len as usize, self.indices.as_ref())
     }
-
-    pub fn max_size(&self) -> f32 {
-        match &self.size {
-            EncodingValue::Scalar { value: size } => *size,
-            EncodingValue::Array { values } => *values
-                .iter()
-                .max_by(|a, b| a.partial_cmp(b).unwrap())
-                .unwrap_or(&1.0),
-        }
+    pub fn font_style_iter(&self) -> Box<dyn Iterator<Item = &FontStyleSpec> + '_> {
+        self.font_style
+            .as_iter(self.len as usize, self.indices.as_ref())
+    }
+    pub fn limit_iter(&self) -> Box<dyn Iterator<Item = &f32> + '_> {
+        self.limit.as_iter(self.len as usize, self.indices.as_ref())
     }
 }
 
-impl Default for SymbolMark {
+impl Default for TextMark {
     fn default() -> Self {
         Self {
-            name: "".to_string(),
+            name: "text_mark".to_string(),
             clip: true,
-            shapes: vec![Default::default()],
-            stroke_width: None,
             len: 1,
+            text: EncodingValue::Scalar {
+                value: String::new(),
+            },
             x: EncodingValue::Scalar { value: 0.0 },
             y: EncodingValue::Scalar { value: 0.0 },
-            shape_index: EncodingValue::Scalar { value: 0 },
-            fill: EncodingValue::Scalar {
-                value: ColorOrGradient::Color([0.0, 0.0, 0.0, 0.0]),
-            },
-            size: EncodingValue::Scalar { value: 20.0 },
-            stroke: EncodingValue::Scalar {
-                value: ColorOrGradient::Color([0.0, 0.0, 0.0, 0.0]),
+            align: EncodingValue::Scalar {
+                value: TextAlignSpec::Left,
+            },
+            baseline: EncodingValue::Scalar {
+                value: TextBaselineSpec::Alphabetic,
             },
             angle: EncodingValue::Scalar { value: 0.0 },
+            color: EncodingValue::Scalar {
+                value: [0.0, 0.0, 0.0, 1.0],
+            },
+            font: EncodingValue::Scalar {
+                value: "sans serif".to_string(),
+            },
+            font_size: EncodingValue::Scalar { value: 10.0 },
+            font_weight: EncodingValue::Scalar {
+                value: FontWeightSpec::Name(FontWeightNameSpec::Normal),
+            },
+            font_style: EncodingValue::Scalar {
+                value: FontStyleSpec::Normal,
+            },
+            limit: EncodingValue::Scalar { value: 0.0 },
             indices: None,
-            gradients: vec![],
             zindex: None,
         }
     }
 }
 
-#[derive(Default, Debug, Clone, Serialize, Deserialize)]
+#[derive(Default, Debug, Clone, Copy, PartialEq, Serialize, Deserialize)]
+#[serde(rename_all = "lowercase")]
+pub enum TextAlignSpec {
+    #[default]
+    Left,
+    Center,
+    Right,
+}
+
+#[derive(Default, Debug, Clone, Copy, PartialEq, Serialize, Deserialize)]
 #[serde(rename_all = "kebab-case")]
-pub enum SymbolShape {
+pub enum TextBaselineSpec {
+    Alphabetic,
+    Top,
+    Middle,
     #[default]
-    Circle,
-    /// Path with origin top-left
-    Path(lyon_path::Path),
+    Bottom,
+    LineTop,
+    LineBottom,
 }
 
-impl SymbolShape {
-    pub fn as_path(&self) -> Cow<lyon_path::Path> {
-        match self {
-            SymbolShape::Circle => {
-                let mut builder = lyon_path::Path::builder();
-                builder.add_circle(lyon_path::geom::point(0.0, 0.0), 0.5, Winding::Positive);
-                Cow::Owned(builder.build())
-            }
-            SymbolShape::Path(path) => Cow::Borrowed(path),
-        }
+#[derive(Debug, Clone, Copy, PartialEq, Serialize, Deserialize)]
+#[serde(untagged)]
+pub enum FontWeightSpec {
+    Name(FontWeightNameSpec),
+    Number(f32),
+}
+
+impl Default for FontWeightSpec {
+    fn default() -> Self {
+        Self::Name(FontWeightNameSpec::Normal)
     }
 }
+
+#[derive(Default, Debug, Clone, Copy, PartialEq, Serialize, Deserialize)]
+#[serde(rename_all = "lowercase")]
+pub enum FontWeightNameSpec {
+    #[default]
+    Normal,
+    Bold,
+}
+
+#[derive(Default, Debug, Clone, Copy, PartialEq, Serialize, Deserialize)]
+#[serde(rename_all = "lowercase")]
+pub enum FontStyleSpec {
+    #[default]
+    Normal,
+    Italic,
+}
```

### Comparing `avenger-0.0.3/avenger/src/marks/trail.rs` & `avenger-0.0.4/avenger/src/marks/trail.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.3/avenger/src/marks/value.rs` & `avenger-0.0.4/avenger/src/marks/value.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.3/avenger-vega/Cargo.toml` & `avenger-0.0.4/avenger-vega/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "avenger-vega"
-version = "0.0.3"
+version = "0.0.4"
 edition = "2021"
 description = "Utilities for importing Vega scenegraphs into Avenger"
 license = "BSD-3-Clause"
 
 [features]
 image-request = [ "reqwest",]
 svg = [ "resvg", "usvg", "tiny-skia",]
@@ -29,15 +29,15 @@
 workspace = true
 
 [dependencies.tracing]
 workspace = true
 
 [dependencies.avenger]
 path = "../avenger"
-version = "0.0.3"
+version = "0.0.4"
 
 [dependencies.thiserror]
 workspace = true
 
 [dependencies.serde]
 workspace = true
```

### Comparing `avenger-0.0.3/avenger-vega/src/error.rs` & `avenger-0.0.4/avenger-vega/src/error.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.3/avenger-vega/src/image/mod.rs` & `avenger-0.0.4/avenger-vega/src/image/mod.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.3/avenger-vega/src/image/reqwest_fetcher.rs` & `avenger-0.0.4/avenger-vega/src/image/reqwest_fetcher.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.3/avenger-vega/src/image/svg.rs` & `avenger-0.0.4/avenger-vega/src/image/svg.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.3/avenger-vega/src/marks/arc.rs` & `avenger-0.0.4/avenger-vega/src/marks/arc.rs`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,18 @@
     pub opacity: Option<f32>,
     pub zindex: Option<i32>,
 }
 
 impl VegaMarkItem for VegaArcItem {}
 
 impl VegaMarkContainer<VegaArcItem> {
-    pub fn to_scene_graph(&self) -> Result<SceneMark, AvengerVegaError> {
+    pub fn to_scene_graph(&self, force_clip: bool) -> Result<SceneMark, AvengerVegaError> {
         // Init mark with scalar defaults
         let mut mark = ArcMark {
-            clip: self.clip,
+            clip: self.clip || force_clip,
             zindex: self.zindex,
             ..Default::default()
         };
         if let Some(name) = &self.name {
             mark.name = name.clone();
         }
```

### Comparing `avenger-0.0.3/avenger-vega/src/marks/area.rs` & `avenger-0.0.4/avenger-vega/src/marks/area.rs`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     pub stroke_dash: Option<StrokeDashSpec>,
     pub opacity: Option<f32>,
 }
 
 impl VegaMarkItem for VegaAreaItem {}
 
 impl VegaMarkContainer<VegaAreaItem> {
-    pub fn to_scene_graph(&self) -> Result<SceneMark, AvengerVegaError> {
+    pub fn to_scene_graph(&self, force_clip: bool) -> Result<SceneMark, AvengerVegaError> {
         // Get shape of first item and use that for all items for now
         let first = self.items.first();
         let stroke_cap = first.and_then(|item| item.stroke_cap).unwrap_or_default();
         let stroke_join = first.and_then(|item| item.stroke_join).unwrap_or_default();
         let orientation = first.and_then(|item| item.orient).unwrap_or_default();
 
         // Parse stroke color
@@ -57,15 +57,15 @@
                 let base_opacity = item.opacity.unwrap_or(1.0);
                 let fill_opacity = item.fill_opacity.unwrap_or(1.0) * base_opacity;
                 fill = fill_css.to_color_or_grad(fill_opacity, &mut gradients)?;
             }
         }
 
         let mut mark = AreaMark {
-            clip: self.clip,
+            clip: self.clip || force_clip,
             zindex: self.zindex,
             orientation,
             fill,
             stroke,
             stroke_width,
             stroke_cap,
             stroke_dash,
```

### Comparing `avenger-0.0.3/avenger-vega/src/marks/image.rs` & `avenger-0.0.4/avenger-vega/src/marks/image.rs`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 fn default_true() -> bool {
     true
 }
 
 impl VegaMarkItem for VegaImageItem {}
 
 impl VegaMarkContainer<VegaImageItem> {
-    pub fn to_scene_graph(&self) -> Result<SceneMark, AvengerVegaError> {
+    pub fn to_scene_graph(&self, force_clip: bool) -> Result<SceneMark, AvengerVegaError> {
         let name = self
             .name
             .clone()
             .unwrap_or_else(|| "image_mark".to_string());
 
         let first = self.items.first();
         let aspect = first.map(|f| f.aspect).unwrap_or(true);
@@ -92,15 +92,15 @@
             Some(indices)
         } else {
             None
         };
 
         Ok(SceneMark::Image(Box::new(ImageMark {
             name,
-            clip: self.clip,
+            clip: self.clip || force_clip,
             len: self.items.len() as u32,
             aspect,
             smooth,
             align: EncodingValue::Array { values: align },
             baseline: EncodingValue::Array { values: baseline },
             image: EncodingValue::Array { values: images },
             x: EncodingValue::Array { values: x },
```

### Comparing `avenger-0.0.3/avenger-vega/src/marks/line.rs` & `avenger-0.0.4/avenger-vega/src/marks/line.rs`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     pub stroke_dash: Option<StrokeDashSpec>,
     pub opacity: Option<f32>,
 }
 
 impl VegaMarkItem for VegaLineItem {}
 
 impl VegaMarkContainer<VegaLineItem> {
-    pub fn to_scene_graph(&self) -> Result<SceneMark, AvengerVegaError> {
+    pub fn to_scene_graph(&self, force_clip: bool) -> Result<SceneMark, AvengerVegaError> {
         // Get shape of first item and use that for all items for now
         let first = self.items.first();
         let stroke_width = first.and_then(|item| item.stroke_width).unwrap_or(1.0);
         let stroke_cap = first.and_then(|item| item.stroke_cap).unwrap_or_default();
         let stroke_join = first.and_then(|item| item.stroke_join).unwrap_or_default();
         let mut gradients = Vec::<Gradient>::new();
 
@@ -43,15 +43,15 @@
             }
             if let Some(d) = &item.stroke_dash {
                 stroke_dash = Some(d.to_array()?.to_vec());
             }
         }
 
         let mut mark = LineMark {
-            clip: self.clip,
+            clip: self.clip || force_clip,
             zindex: self.zindex,
             stroke,
             stroke_width,
             stroke_cap,
             stroke_dash,
             stroke_join,
             gradients,
```

### Comparing `avenger-0.0.3/avenger-vega/src/marks/mark.rs` & `avenger-0.0.4/avenger-vega/src/marks/mark.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.3/avenger-vega/src/marks/path.rs` & `avenger-0.0.4/avenger-vega/src/marks/path.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 use crate::error::AvengerVegaError;
 use crate::marks::mark::{VegaMarkContainer, VegaMarkItem};
-use crate::marks::symbol::parse_svg_path;
 use crate::marks::values::CssColorOrGradient;
+use avenger::error::AvengerError;
 use avenger::marks::mark::SceneMark;
 use avenger::marks::path::{PathMark, PathTransform};
+use avenger::marks::symbol::parse_svg_path;
 use avenger::marks::value::{ColorOrGradient, EncodingValue, Gradient, StrokeCap, StrokeJoin};
 use lyon_extra::euclid::Vector2D;
 use lyon_path::geom::Angle;
 use serde::{Deserialize, Serialize};
 use std::collections::HashSet;
 
 #[derive(Default, Debug, Clone, PartialEq, Serialize, Deserialize)]
@@ -29,15 +30,15 @@
     pub angle: Option<f32>,
     pub zindex: Option<i32>,
 }
 
 impl VegaMarkItem for VegaPathItem {}
 
 impl VegaMarkContainer<VegaPathItem> {
-    pub fn to_scene_graph(&self) -> Result<SceneMark, AvengerVegaError> {
+    pub fn to_scene_graph(&self, force_clip: bool) -> Result<SceneMark, AvengerVegaError> {
         // Get shape of first item and use that for all items for now
         let first = self.items.first();
         let first_has_stroke = first.map(|item| item.stroke.is_some()).unwrap_or(false);
         let stroke_width = if first_has_stroke {
             // Default stroke_width to 1.0 if a stroke is specified
             Some(first.and_then(|item| item.stroke_width).unwrap_or(1.0))
         } else {
@@ -45,15 +46,15 @@
         };
 
         let first_cap = first.and_then(|item| item.stroke_cap).unwrap_or_default();
         let first_join = first.and_then(|item| item.stroke_join).unwrap_or_default();
 
         // Init mark with scalar defaults
         let mut mark = PathMark {
-            clip: self.clip,
+            clip: self.clip || force_clip,
             zindex: self.zindex,
             stroke_cap: first_cap,
             stroke_join: first_join,
             stroke_width,
             ..Default::default()
         };
 
@@ -136,15 +137,15 @@
                 value: parse_svg_path(path_str)?,
             };
         } else {
             // Parse each path individually
             let paths = path_str
                 .iter()
                 .map(|p| parse_svg_path(p))
-                .collect::<Result<Vec<_>, AvengerVegaError>>()?;
+                .collect::<Result<Vec<_>, AvengerError>>()?;
 
             mark.path = EncodingValue::Array { values: paths };
         }
 
         // Add gradients
         mark.gradients = gradients;
```

### Comparing `avenger-0.0.3/avenger-vega/src/marks/rect.rs` & `avenger-0.0.4/avenger-vega/src/marks/rect.rs`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,17 @@
     pub stroke_opacity: Option<f32>,
     pub zindex: Option<i32>,
 }
 
 impl VegaMarkItem for VegaRectItem {}
 
 impl VegaMarkContainer<VegaRectItem> {
-    pub fn to_scene_graph(&self) -> Result<SceneMark, AvengerVegaError> {
+    pub fn to_scene_graph(&self, force_clip: bool) -> Result<SceneMark, AvengerVegaError> {
         let mut mark = RectMark {
-            clip: self.clip,
+            clip: self.clip || force_clip,
             zindex: self.zindex,
             ..Default::default()
         };
 
         if let Some(name) = &self.name {
             mark.name = name.clone();
         }
```

### Comparing `avenger-0.0.3/avenger-vega/src/marks/rule.rs` & `avenger-0.0.4/avenger-vega/src/marks/rule.rs`

 * *Files 2% similar despite different names*

```diff
@@ -21,18 +21,18 @@
     pub opacity: Option<f32>,
     pub zindex: Option<i32>,
 }
 
 impl VegaMarkItem for VegaRuleItem {}
 
 impl VegaMarkContainer<VegaRuleItem> {
-    pub fn to_scene_graph(&self) -> Result<SceneMark, AvengerVegaError> {
+    pub fn to_scene_graph(&self, force_clip: bool) -> Result<SceneMark, AvengerVegaError> {
         // Init mark with scalar defaults
         let mut mark = RuleMark {
-            clip: self.clip,
+            clip: self.clip || force_clip,
             zindex: self.zindex,
             ..Default::default()
         };
         if let Some(name) = &self.name {
             mark.name = name.clone();
         }
```

### Comparing `avenger-0.0.3/avenger-vega/src/marks/shape.rs` & `avenger-0.0.4/avenger-vega/src/marks/shape.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 use crate::error::AvengerVegaError;
 use crate::marks::mark::{VegaMarkContainer, VegaMarkItem};
-use crate::marks::symbol::parse_svg_path;
 use crate::marks::values::CssColorOrGradient;
+use avenger::error::AvengerError;
 use avenger::marks::mark::SceneMark;
 use avenger::marks::path::{PathMark, PathTransform};
+use avenger::marks::symbol::parse_svg_path;
 use avenger::marks::value::{ColorOrGradient, EncodingValue, Gradient, StrokeCap, StrokeJoin};
 use serde::{Deserialize, Serialize};
 use std::collections::HashSet;
 
 #[derive(Default, Debug, Clone, PartialEq, Serialize, Deserialize)]
 #[serde(rename_all = "camelCase")]
 pub struct VegaShapeItem {
@@ -24,15 +25,15 @@
     pub stroke_width: Option<f32>,
     pub zindex: Option<i32>,
 }
 
 impl VegaMarkItem for VegaShapeItem {}
 
 impl VegaMarkContainer<VegaShapeItem> {
-    pub fn to_scene_graph(&self) -> Result<SceneMark, AvengerVegaError> {
+    pub fn to_scene_graph(&self, force_clip: bool) -> Result<SceneMark, AvengerVegaError> {
         // Get shape of first item and use that for all items for now
         let first = self.items.first();
         let first_has_stroke = first.map(|item| item.stroke.is_some()).unwrap_or(false);
         let stroke_width = if first_has_stroke {
             // Default stroke_width to 1.0 if a stroke is specified
             Some(first.and_then(|item| item.stroke_width).unwrap_or(1.0))
         } else {
@@ -40,15 +41,15 @@
         };
 
         let first_cap = first.and_then(|item| item.stroke_cap).unwrap_or_default();
         let first_join = first.and_then(|item| item.stroke_join).unwrap_or_default();
 
         // Init mark with scalar defaults
         let mut mark = PathMark {
-            clip: self.clip,
+            clip: self.clip || force_clip,
             zindex: self.zindex,
             stroke_cap: first_cap,
             stroke_join: first_join,
             stroke_width,
             ..Default::default()
         };
 
@@ -120,15 +121,15 @@
                 value: parse_svg_path(path_str)?,
             };
         } else {
             // Parse each path individually
             let paths = path_str
                 .iter()
                 .map(|p| parse_svg_path(p))
-                .collect::<Result<Vec<_>, AvengerVegaError>>()?;
+                .collect::<Result<Vec<_>, AvengerError>>()?;
 
             mark.path = EncodingValue::Array { values: paths };
         }
 
         // Add gradients
         mark.gradients = gradients;
```

### Comparing `avenger-0.0.3/avenger-vega/src/marks/text.rs` & `avenger-0.0.4/avenger-vega/src/marks/text.rs`

 * *Files 1% similar despite different names*

```diff
@@ -34,18 +34,18 @@
     pub limit: Option<f32>,
     pub zindex: Option<i32>,
 }
 
 impl VegaMarkItem for VegaTextItem {}
 
 impl VegaMarkContainer<VegaTextItem> {
-    pub fn to_scene_graph(&self) -> Result<SceneMark, AvengerVegaError> {
+    pub fn to_scene_graph(&self, force_clip: bool) -> Result<SceneMark, AvengerVegaError> {
         // Init mark with scalar defaults
         let mut mark = TextMark {
-            clip: self.clip,
+            clip: self.clip || force_clip,
             zindex: self.zindex,
             ..Default::default()
         };
         if let Some(name) = &self.name {
             mark.name = name.clone();
         }
```

### Comparing `avenger-0.0.3/avenger-vega/src/marks/trail.rs` & `avenger-0.0.4/avenger-vega/src/marks/trail.rs`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     pub fill_opacity: Option<f32>,
     pub opacity: Option<f32>,
 }
 
 impl VegaMarkItem for VegaTrailItem {}
 
 impl VegaMarkContainer<VegaTrailItem> {
-    pub fn to_scene_graph(&self) -> Result<SceneMark, AvengerVegaError> {
+    pub fn to_scene_graph(&self, force_clip: bool) -> Result<SceneMark, AvengerVegaError> {
         // Get shape of first item and use that for all items for now
         let first = self.items.first();
         let mut gradients = Vec::<Gradient>::new();
 
         // Parse stroke color (Note, vega uses "fill" for the trail, but we use stroke
         let mut stroke = ColorOrGradient::Color([0.0, 0.0, 0.0, 1.0]);
         if let Some(item) = &first {
@@ -33,15 +33,15 @@
                 let base_opacity = item.opacity.unwrap_or(1.0);
                 let stroke_opacity = item.fill_opacity.unwrap_or(1.0) * base_opacity;
                 stroke = stroke_css.to_color_or_grad(stroke_opacity, &mut gradients)?;
             }
         }
 
         let mut mark = TrailMark {
-            clip: self.clip,
+            clip: self.clip || force_clip,
             zindex: self.zindex,
             gradients,
             stroke,
             ..Default::default()
         };
 
         // Init vector for each encoding channel
```

### Comparing `avenger-0.0.3/avenger-vega/src/marks/values.rs` & `avenger-0.0.4/avenger-vega/src/marks/values.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.3/avenger-vega/src/scene_graph.rs` & `avenger-0.0.4/avenger-vega/src/scene_graph.rs`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,14 @@
     pub scenegraph: VegaMarkContainer<VegaGroupItem>,
 }
 
 impl VegaSceneGraph {
     #[tracing::instrument(skip_all)]
     pub fn to_scene_graph(&self) -> Result<SceneGraph, AvengerVegaError> {
         Ok(SceneGraph {
-            groups: self.scenegraph.to_scene_graph()?,
+            groups: self.scenegraph.to_scene_graph(false)?,
             width: self.width,
             height: self.height,
             origin: self.origin,
         })
     }
 }
```

### Comparing `avenger-0.0.3/avenger-vega/tests/test_parsing.rs` & `avenger-0.0.4/avenger-vega/tests/test_parsing.rs`

 * *Files identical despite different names*

### Comparing `avenger-0.0.3/avenger-python/Cargo.toml` & `avenger-0.0.4/avenger-python/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "avenger-python"
-version = "0.0.3"
+version = "0.0.4"
 edition = "2021"
 license = "BSD-3-Clause"
 description = "Python API to Avenger visualization framework"
 publish = false
 
 [lib]
 name = "avenger"
@@ -13,25 +13,25 @@
 [dependencies]
 pythonize = "0.20.0"
 pollster = "0.3"
 
 [dependencies.avenger]
 path = "../avenger"
 features = [ "pyo3",]
-version = "0.0.3"
+version = "0.0.4"
 
 [dependencies.avenger-vega]
 path = "../avenger-vega"
 features = [ "pyo3",]
-version = "0.0.3"
+version = "0.0.4"
 
 [dependencies.avenger-wgpu]
 path = "../avenger-wgpu"
 features = [ "pyo3",]
-version = "0.0.3"
+version = "0.0.4"
 
 [dependencies.pyo3]
 workspace = true
 features = [ "extension-module", "abi3-py38",]
 
 [dependencies.serde]
 workspace = true
```

### Comparing `avenger-0.0.3/avenger-python/LICENSE` & `avenger-0.0.4/avenger-python/LICENSE`

 * *Files identical despite different names*

### Comparing `avenger-0.0.3/avenger-python/README.md` & `avenger-0.0.4/avenger-python/README.md`

 * *Files identical despite different names*

### Comparing `avenger-0.0.3/avenger-python/src/lib.rs` & `avenger-0.0.4/avenger-python/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -25,18 +25,21 @@
         let inner = vega_sg.to_scene_graph()?;
         Ok(Self { inner })
     }
 
     #[allow(clippy::wrong_self_convention)]
     fn to_png(&mut self, py: Python, scale: Option<f32>) -> PyResult<PyObject> {
         let img = pollster::block_on(async {
-            let mut png_canvas = PngCanvas::new(CanvasDimensions {
-                size: [self.inner.width, self.inner.height],
-                scale: scale.unwrap_or(1.0),
-            })
+            let mut png_canvas = PngCanvas::new(
+                CanvasDimensions {
+                    size: [self.inner.width, self.inner.height],
+                    scale: scale.unwrap_or(1.0),
+                },
+                Default::default(),
+            )
             .await?;
             png_canvas.set_scene(&self.inner)?;
 
             png_canvas.render().await
         })?;
 
         let mut png_data = Vec::new();
```

### Comparing `avenger-0.0.3/Cargo.lock` & `avenger-0.0.4/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,15 @@
 [[package]]
 name = "ahash"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "91429305e9f0a25f6205c5b8e0d2db09e0708a7a6df0f42212bb56c32c8ac97a"
 dependencies = [
  "cfg-if",
+ "getrandom",
  "once_cell",
  "version_check",
  "zerocopy",
 ]
 
 [[package]]
 name = "aho-corasick"
@@ -141,28 +142,31 @@
 name = "allocator-api2"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0942ffc6dcaadf03badf6e6a2d0228460359d5e34b57ccdc720b7382dfbd5ec5"
 
 [[package]]
 name = "android-activity"
-version = "0.4.3"
+version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "64529721f27c2314ced0890ce45e469574a73e5e6fdd6e9da1860eb29285f5e0"
+checksum = "ee91c0c2905bae44f84bfa4e044536541df26b7703fd0888deeb9060fcc44289"
 dependencies = [
  "android-properties",
- "bitflags 1.3.2",
+ "bitflags 2.4.1",
  "cc",
+ "cesu8",
+ "jni",
  "jni-sys",
  "libc",
  "log",
  "ndk",
  "ndk-context",
  "ndk-sys",
- "num_enum 0.6.1",
+ "num_enum",
+ "thiserror",
 ]
 
 [[package]]
 name = "android-properties"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fc7eb209b1518d6bb87b283c20095f5228ecda460da70b44f0802523dea6da04"
@@ -200,14 +204,20 @@
 [[package]]
 name = "arrayvec"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
 
 [[package]]
+name = "as-raw-xcb-connection"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "175571dd1d178ced59193a6fc02dde1b972eb0bc56c892cde9beeceac5bf0f6b"
+
+[[package]]
 name = "ash"
 version = "0.37.3+1.3.251"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "39e9c3835d686b0a6084ab4234fcd1b07dbf6e4767dce60874b12356a25ecd4a"
 dependencies = [
  "libloading 0.7.4",
 ]
@@ -286,14 +296,20 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.47",
 ]
 
 [[package]]
+name = "atomic-waker"
+version = "1.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1505bd5d3d116872e7271a6d4e16d81d0c8570876c8de68093a09ac269d8aac0"
+
+[[package]]
 name = "auto_impl"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fee3da8ef1276b0bee5dd1c7258010d8fffd31801447323115a25560e1327b89"
 dependencies = [
  "proc-macro-error",
  "proc-macro2",
@@ -305,28 +321,29 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "avenger"
-version = "0.0.3"
+version = "0.0.4"
 dependencies = [
  "image",
+ "lyon_extra",
  "lyon_path",
  "pyo3",
  "rayon",
  "serde",
  "thiserror",
  "tracing",
 ]
 
 [[package]]
 name = "avenger-python"
-version = "0.0.3"
+version = "0.0.4"
 dependencies = [
  "avenger",
  "avenger-vega",
  "avenger-wgpu",
  "image",
  "lazy_static",
  "pollster",
@@ -335,46 +352,70 @@
  "serde",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "avenger-vega"
-version = "0.0.3"
+version = "0.0.4"
 dependencies = [
  "avenger",
  "cfg-if",
  "csscolorparser",
  "image",
  "lazy_static",
  "lyon_extra",
  "lyon_path",
  "pyo3",
  "reqwest",
  "resvg 0.38.0",
  "serde",
  "serde_json",
  "thiserror",
- "tiny-skia 0.11.3",
+ "tiny-skia",
  "tracing",
  "usvg 0.38.0",
 ]
 
 [[package]]
+name = "avenger-vega-renderer"
+version = "0.0.4"
+dependencies = [
+ "avenger",
+ "avenger-vega",
+ "avenger-wgpu",
+ "console_error_panic_hook",
+ "csscolorparser",
+ "gloo-utils",
+ "image",
+ "itertools 0.12.0",
+ "js-sys",
+ "lazy_static",
+ "lyon_path",
+ "serde-wasm-bindgen",
+ "serde_json",
+ "unicode-segmentation",
+ "wasm-bindgen",
+ "wasm-bindgen-futures",
+ "web-sys",
+ "wgpu",
+]
+
+[[package]]
 name = "avenger-vega-test-data"
-version = "0.0.3"
+version = "0.0.4"
 dependencies = [
  "pollster",
  "serde_json",
  "vl-convert-rs",
 ]
 
 [[package]]
 name = "avenger-wgpu"
-version = "0.0.3"
+version = "0.0.4"
 dependencies = [
  "avenger",
  "avenger-vega",
  "bytemuck",
  "cfg-if",
  "cgmath",
  "colorgrad",
@@ -391,14 +432,15 @@
  "pollster",
  "pyo3",
  "rayon",
  "rstest",
  "serde_json",
  "thiserror",
  "tracing",
+ "web-sys",
  "wgpu",
  "winit",
 ]
 
 [[package]]
 name = "backtrace"
 version = "0.3.69"
@@ -512,29 +554,29 @@
 checksum = "a8894febbff9f758034a5b8e12d87918f56dfc64a8e1fe757d65e29041538d93"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "block-sys"
-version = "0.1.0-beta.1"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fa55741ee90902547802152aaf3f8e5248aab7e21468089560d4c8840561146"
+checksum = "ae85a0696e7ea3b835a453750bf002770776609115e6d25c6d2ff28a8200f7e7"
 dependencies = [
  "objc-sys",
 ]
 
 [[package]]
 name = "block2"
-version = "0.2.0-alpha.6"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8dd9e63c1744f755c2f60332b88de39d341e5e86239014ad839bd71c106dec42"
+checksum = "15b55663a85f33501257357e6421bb33e769d5c9ffb5ba0921c975a123e35e68"
 dependencies = [
  "block-sys",
- "objc2-encode",
+ "objc2",
 ]
 
 [[package]]
 name = "brotli"
 version = "3.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "516074a47ef4bce09577a3b379392300159ce5b1ba2e501ff1c819950066100f"
@@ -596,24 +638,36 @@
 name = "cache_control"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bf2a5fb3207c12b5d208ebc145f967fea5cac41a021c37417ccc31ba40f39ee"
 
 [[package]]
 name = "calloop"
-version = "0.10.6"
+version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "52e0d00eb1ea24371a97d2da6201c6747a633dc6dc1988ef503403b4c59504a8"
+checksum = "fba7adb4dd5aa98e5553510223000e7148f621165ec5f9acd7113f6ca4995298"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.4.1",
  "log",
- "nix 0.25.1",
- "slotmap",
+ "polling",
+ "rustix",
+ "slab",
  "thiserror",
- "vec_map",
+]
+
+[[package]]
+name = "calloop-wayland-source"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0f0ea9b9476c7fad82841a8dbb380e2eae480c21910feba80725b46931ed8f02"
+dependencies = [
+ "calloop",
+ "rustix",
+ "wayland-backend",
+ "wayland-client",
 ]
 
 [[package]]
 name = "cbc"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26b52a9543ae338f279b96b0b9fed9c8093744685043739079ce85cd58f289a6"
@@ -628,14 +682,20 @@
 checksum = "f1174fb0b6ec23863f8b971027804a42614e347eafb0a95bf0b12cdae21fc4d0"
 dependencies = [
  "jobserver",
  "libc",
 ]
 
 [[package]]
+name = "cesu8"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6d43a04d8753f35258c91f8ec639f792891f748a1edbd759cf1dcea3382ad83c"
+
+[[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "cfg_aliases"
@@ -695,18 +755,72 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a5f405d474b9d05e0a093d3120e77e9bf26461b57a84b40aa2a221ac5617fb6"
 dependencies = [
  "csscolorparser",
 ]
 
 [[package]]
-name = "com-rs"
-version = "0.2.1"
+name = "com"
+version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf43edc576402991846b093a7ca18a3477e0ef9c588cde84964b5d3e43016642"
+checksum = "7e17887fd17353b65b1b2ef1c526c83e26cd72e74f598a8dc1bee13a48f3d9f6"
+dependencies = [
+ "com_macros",
+]
+
+[[package]]
+name = "com_macros"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d375883580a668c7481ea6631fc1a8863e33cc335bf56bfad8d7e6d4b04b13a5"
+dependencies = [
+ "com_macros_support",
+ "proc-macro2",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "com_macros_support"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ad899a1087a9296d5644792d7cb72b8e34c1bec8e7d4fbc002230169a6e8710c"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "combine"
+version = "4.6.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "35ed6e9d84f0b51a7f52daf1c7d71dd136fd7a3f41a8462b8cdb8c78d920fad4"
+dependencies = [
+ "bytes",
+ "memchr",
+]
+
+[[package]]
+name = "concurrent-queue"
+version = "2.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d16048cd947b08fa32c24458a22f5dc5e835264f689f4f5653210c69fd107363"
+dependencies = [
+ "crossbeam-utils",
+]
+
+[[package]]
+name = "console_error_panic_hook"
+version = "0.1.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a06aeb73f470f66dcdbf7223caeebb85984942f22f1adb2a088cf9668146bbbc"
+dependencies = [
+ "cfg-if",
+ "wasm-bindgen",
+]
 
 [[package]]
 name = "console_static_text"
 version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f4be93df536dfbcbd39ff7c129635da089901116b88bfc29ec1acb9b56f8ff35"
 dependencies = [
@@ -740,22 +854,22 @@
 name = "core-foundation-sys"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
 
 [[package]]
 name = "core-graphics"
-version = "0.22.3"
+version = "0.23.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2581bbab3b8ffc6fcbd550bf46c355135d16e9ff2a6ea032ad6b9bf1d7efe4fb"
+checksum = "970a29baf4110c26fedbc7f82107d42c23f7e88e404c4577ed73fe99ff85a212"
 dependencies = [
  "bitflags 1.3.2",
  "core-foundation",
  "core-graphics-types",
- "foreign-types 0.3.2",
+ "foreign-types 0.5.0",
  "libc",
 ]
 
 [[package]]
 name = "core-graphics-types"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -907,14 +1021,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0369ee1ad671834580515889b80f2ea915f23b8be8d0daa4bbaf2ac5c7590835"
 dependencies = [
  "cipher",
 ]
 
 [[package]]
+name = "cursor-icon"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "96a6ac251f4a2aca6b3f91340350eab87ae57c3f127ffeb585e92bd336717991"
+
+[[package]]
 name = "curve25519-dalek"
 version = "4.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e89b8c6a2e4b1f45971ad09761aafb85514a84744b67a95e32c3cc1352d1f65c"
 dependencies = [
  "cfg-if",
  "cpufeatures",
@@ -935,17 +1055,17 @@
  "proc-macro2",
  "quote",
  "syn 2.0.47",
 ]
 
 [[package]]
 name = "d3d12"
-version = "0.7.0"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e16e44ab292b1dddfdaf7be62cfd8877df52f2f3fde5858d95bab606be259f20"
+checksum = "3e3d747f100290a1ca24b752186f61f6637e1deffe3bf6320de6fcb29510a307"
 dependencies = [
  "bitflags 2.4.1",
  "libloading 0.8.1",
  "winapi",
 ]
 
 [[package]]
@@ -1194,15 +1314,15 @@
  "async-trait",
  "deno_core",
  "deno_io",
  "filetime",
  "fs3",
  "libc",
  "log",
- "nix 0.26.2",
+ "nix",
  "rand",
  "serde",
  "tokio",
  "winapi",
 ]
 
 [[package]]
@@ -1214,15 +1334,15 @@
  "anyhow",
  "async-trait",
  "data-url",
  "deno_ast",
  "deno_semver",
  "futures",
  "import_map",
- "indexmap 2.1.0",
+ "indexmap 2.2.5",
  "log",
  "monch",
  "once_cell",
  "parking_lot 0.12.1",
  "regex",
  "serde",
  "serde_json",
@@ -1393,15 +1513,15 @@
  "elliptic-curve",
  "errno 0.2.8",
  "h2",
  "hex",
  "hkdf",
  "http",
  "idna 0.3.0",
- "indexmap 2.1.0",
+ "indexmap 2.2.5",
  "k256",
  "lazy-regex",
  "libc",
  "libz-sys",
  "md-5",
  "md4",
  "num-bigint",
@@ -1485,15 +1605,15 @@
  "fs3",
  "fwdansi",
  "http",
  "hyper 0.14.28",
  "libc",
  "log",
  "netif",
- "nix 0.26.2",
+ "nix",
  "notify",
  "ntapi",
  "once_cell",
  "regex",
  "ring",
  "serde",
  "signal-hook-registry",
@@ -2180,17 +2300,14 @@
 
 [[package]]
 name = "flume"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "55ac459de2512911e4b674ce33cf20befaba382d05b62b008afc1c8b57cbf181"
 dependencies = [
- "futures-core",
- "futures-sink",
- "nanorand",
  "spin 0.9.8",
 ]
 
 [[package]]
 name = "fly-accept-encoding"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2467,14 +2584,24 @@
 dependencies = [
  "typenum",
  "version_check",
  "zeroize",
 ]
 
 [[package]]
+name = "gethostname"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0176e0459c2e4a1fe232f984bca6890e681076abb9934f6cea7c326f3fc47818"
+dependencies = [
+ "libc",
+ "windows-targets 0.48.5",
+]
+
+[[package]]
 name = "getopts"
 version = "0.2.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14dbbfd5c71d70241ecf9e6f13737f7b5ce823821063188d7e46c41d371eebd5"
 dependencies = [
  "unicode-width",
 ]
@@ -2482,18 +2609,16 @@
 [[package]]
 name = "getrandom"
 version = "0.2.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fe9006bed769170c11f845cf00c7c1e9092aeb3f268e007c3e760ac68008070f"
 dependencies = [
  "cfg-if",
- "js-sys",
  "libc",
  "wasi",
- "wasm-bindgen",
 ]
 
 [[package]]
 name = "ghash"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d930750de5717d2dd0b8c0d42c076c0e884c81a73e6cab859bbd2339c71e3e40"
@@ -2532,18 +2657,31 @@
 [[package]]
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
+name = "gloo-utils"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0b5555354113b18c547c1d3a98fbf7fb32a9ff4f6fa112ce823a21641a0ba3aa"
+dependencies = [
+ "js-sys",
+ "serde",
+ "serde_json",
+ "wasm-bindgen",
+ "web-sys",
+]
+
+[[package]]
 name = "glow"
-version = "0.13.0"
+version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "886c2a30b160c4c6fec8f987430c26b526b7988ca71f664e6a699ddf6f9601e4"
+checksum = "bd348e04c43b32574f2de31c8bb397d96c9fcfa1371bd4ca6d8bdc464ab121b1"
 dependencies = [
  "js-sys",
  "slotmap",
  "wasm-bindgen",
  "web-sys",
 ]
 
@@ -2573,19 +2711,18 @@
 checksum = "98ff03b468aa837d70984d55f5d3f846f6ec31fe34bbb97c4f85219caeee1ca4"
 dependencies = [
  "bitflags 2.4.1",
 ]
 
 [[package]]
 name = "gpu-allocator"
-version = "0.23.0"
+version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "40fe17c8a05d60c38c0a4e5a3c802f2f1ceb66b76c67d96ffb34bef0475a7fad"
+checksum = "6f56f6318968d03c18e1bcf4857ff88c61157e9da8e47c5f29055d60e1228884"
 dependencies = [
- "backtrace",
  "log",
  "presser",
  "thiserror",
  "winapi",
  "windows",
 ]
 
@@ -2628,15 +2765,15 @@
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
- "indexmap 2.1.0",
+ "indexmap 2.2.5",
  "slab",
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
@@ -2680,22 +2817,22 @@
 checksum = "e8094feaf31ff591f651a2664fb9cfd92bba7a60ce3197265e9482ebe753c8f7"
 dependencies = [
  "hashbrown 0.14.3",
 ]
 
 [[package]]
 name = "hassle-rs"
-version = "0.10.0"
+version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1397650ee315e8891a0df210707f0fc61771b0cc518c3023896064c5407cb3b0"
+checksum = "af2a7e73e1f34c48da31fb668a907f250794837e08faa144fd24f0b8b741e890"
 dependencies = [
- "bitflags 1.3.2",
- "com-rs",
+ "bitflags 2.4.1",
+ "com",
  "libc",
- "libloading 0.7.4",
+ "libloading 0.8.1",
  "thiserror",
  "widestring",
  "winapi",
 ]
 
 [[package]]
 name = "heck"
@@ -2891,14 +3028,25 @@
  "hyper 0.14.28",
  "native-tls",
  "tokio",
  "tokio-native-tls",
 ]
 
 [[package]]
+name = "icrate"
+version = "0.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "99d3aaff8a54577104bafdf686ff18565c3b6903ca5782a2026ef06e2c7aa319"
+dependencies = [
+ "block2",
+ "dispatch",
+ "objc2",
+]
+
+[[package]]
 name = "idna"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "418a0a6fab821475f634efe3ccc45c013f742efe03d853e8d3355d5cb850ecf8"
 dependencies = [
  "matches",
  "unicode-bidi",
@@ -2983,17 +3131,17 @@
  "autocfg",
  "hashbrown 0.12.3",
  "serde",
 ]
 
 [[package]]
 name = "indexmap"
-version = "2.1.0"
+version = "2.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d530e1a18b1cb4c484e6e34556a0d948706958449fca0cab753d649f2bce3d1f"
+checksum = "7b0b929d511467233429c45a44ac1dcaa21ba0f5ba11e4879e6ed28ddb4f9df4"
 dependencies = [
  "equivalent",
  "hashbrown 0.14.3",
  "serde",
 ]
 
 [[package]]
@@ -3035,17 +3183,14 @@
 [[package]]
 name = "instant"
 version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if",
- "js-sys",
- "wasm-bindgen",
- "web-sys",
 ]
 
 [[package]]
 name = "ipconfig"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b58db92f96b720de98181bbbe63c831e87005ab460c1bf306eb2622b4707997f"
@@ -3106,14 +3251,30 @@
 [[package]]
 name = "itoa"
 version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
 
 [[package]]
+name = "jni"
+version = "0.21.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1a87aa2bb7d2af34197c04845522473242e1aa17c12f4935d5856491a7fb8c97"
+dependencies = [
+ "cesu8",
+ "cfg-if",
+ "combine",
+ "jni-sys",
+ "log",
+ "thiserror",
+ "walkdir",
+ "windows-sys 0.45.0",
+]
+
+[[package]]
 name = "jni-sys"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8eaf4bc02d17cbdd7ff4c7438cafcdf7fb9a4613313ad11b4f8fefe7d3fa0130"
 
 [[package]]
 name = "jobserver"
@@ -3131,17 +3292,17 @@
 checksum = "bc0000e42512c92e31c2252315bda326620a4e034105e900c98ec492fa077b3e"
 dependencies = [
  "rayon",
 ]
 
 [[package]]
 name = "js-sys"
-version = "0.3.64"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
+checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "k256"
 version = "0.13.2"
@@ -3568,23 +3729,14 @@
 name = "memmem"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a64a92489e2744ce060c349162be1c5f33c6969234104dbd99ddb5feb08b8c15"
 
 [[package]]
 name = "memoffset"
-version = "0.6.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
-dependencies = [
- "autocfg",
-]
-
-[[package]]
-name = "memoffset"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5de893c32cde5f383baa4c04c5d6dbdd735cfd4a794b0debdb2bb1b421da5ff4"
 dependencies = [
  "autocfg",
 ]
 
@@ -3656,42 +3808,33 @@
 name = "multimap"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5ce46fe64a9d73be07dcbe690a38ce1b293be448fd8ce1e6c1b8062c9f72c6a"
 
 [[package]]
 name = "naga"
-version = "0.14.2"
+version = "0.19.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae585df4b6514cf8842ac0f1ab4992edc975892704835b549cf818dc0191249e"
+checksum = "50e3524642f53d9af419ab5e8dd29d3ba155708267667c2f3f06c88c9e130843"
 dependencies = [
  "bit-set",
  "bitflags 2.4.1",
  "codespan-reporting",
  "hexf-parse",
- "indexmap 2.1.0",
+ "indexmap 2.2.5",
  "log",
  "num-traits",
  "rustc-hash",
  "spirv",
  "termcolor",
  "thiserror",
  "unicode-xid",
 ]
 
 [[package]]
-name = "nanorand"
-version = "0.7.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a51313c5820b0b02bd422f4b44776fbf47961755c74ce64afc73bfad10226c3"
-dependencies = [
- "getrandom",
-]
-
-[[package]]
 name = "native-tls"
 version = "0.2.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "07226173c32f2926027b63cce4bcd8076c3552846cbe7925f3aaffeac0a3b92e"
 dependencies = [
  "lazy_static",
  "libc",
@@ -3703,37 +3846,38 @@
  "security-framework",
  "security-framework-sys",
  "tempfile",
 ]
 
 [[package]]
 name = "ndk"
-version = "0.7.0"
+version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "451422b7e4718271c8b5b3aadf5adedba43dc76312454b387e98fae0fc951aa0"
+checksum = "2076a31b7010b17a38c01907c45b945e8f11495ee4dd588309718901b1f7a5b7"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.4.1",
  "jni-sys",
+ "log",
  "ndk-sys",
- "num_enum 0.5.11",
+ "num_enum",
  "raw-window-handle",
  "thiserror",
 ]
 
 [[package]]
 name = "ndk-context"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "27b02d87554356db9e9a873add8782d4ea6e3e58ea071a9adb9a2e8ddb884a8b"
 
 [[package]]
 name = "ndk-sys"
-version = "0.4.1+23.1.7779620"
+version = "0.5.0+25.2.9519653"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3cf2aae958bd232cac5069850591667ad422d263686d75b52a065f9badeee5a3"
+checksum = "8c196769dd60fd4f363e11d948139556a344e79d451aeb2fa2fd040738ef7691"
 dependencies = [
  "jni-sys",
 ]
 
 [[package]]
 name = "netif"
 version = "0.1.6"
@@ -3748,39 +3892,14 @@
 name = "new_debug_unreachable"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e4a24736216ec316047a1fc4252e27dabb04218aa4a3f37c6e7ddbf1f9782b54"
 
 [[package]]
 name = "nix"
-version = "0.24.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa52e972a9a719cecb6864fb88568781eb706bac2cd1d4f04a648542dbf78069"
-dependencies = [
- "bitflags 1.3.2",
- "cfg-if",
- "libc",
- "memoffset 0.6.5",
-]
-
-[[package]]
-name = "nix"
-version = "0.25.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f346ff70e7dbfd675fe90590b92d59ef2de15a8779ae305ebcbfd3f0caf59be4"
-dependencies = [
- "autocfg",
- "bitflags 1.3.2",
- "cfg-if",
- "libc",
- "memoffset 0.6.5",
-]
-
-[[package]]
-name = "nix"
 version = "0.26.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfdda3d196821d6af13126e40375cdf7da646a96114af134d5f417a9a1dc8e1a"
 dependencies = [
  "bitflags 1.3.2",
  "cfg-if",
  "libc",
@@ -3951,47 +4070,26 @@
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "num_enum"
-version = "0.5.11"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f646caf906c20226733ed5b1374287eb97e3c2a5c227ce668c1f2ce20ae57c9"
-dependencies = [
- "num_enum_derive 0.5.11",
-]
-
-[[package]]
-name = "num_enum"
-version = "0.6.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a015b430d3c108a207fd776d2e2196aaf8b1cf8cf93253e3a097ff3085076a1"
-dependencies = [
- "num_enum_derive 0.6.1",
-]
-
-[[package]]
-name = "num_enum_derive"
-version = "0.5.11"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dcbff9bc912032c62bf65ef1d5aea88983b420f4f839db1e9b0c281a25c9c799"
+checksum = "02339744ee7253741199f897151b38e72257d13802d4ee837285cc2990a90845"
 dependencies = [
- "proc-macro-crate",
- "proc-macro2",
- "quote",
- "syn 1.0.109",
+ "num_enum_derive",
 ]
 
 [[package]]
 name = "num_enum_derive"
-version = "0.6.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "96667db765a921f7b295ffee8b60472b686a51d4f21c2ee4ffdb94c7013b65a6"
+checksum = "681030a937600a36906c185595136d26abfebb4aa9c65701cefcaf8578bb982b"
 dependencies = [
  "proc-macro-crate",
  "proc-macro2",
  "quote",
  "syn 2.0.47",
 ]
 
@@ -4003,37 +4101,33 @@
 dependencies = [
  "malloc_buf",
  "objc_exception",
 ]
 
 [[package]]
 name = "objc-sys"
-version = "0.2.0-beta.2"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "df3b9834c1e95694a05a828b59f55fa2afec6288359cda67146126b3f90a55d7"
+checksum = "c7c71324e4180d0899963fc83d9d241ac39e699609fc1025a850aadac8257459"
 
 [[package]]
 name = "objc2"
-version = "0.3.0-beta.3.patch-leaks.3"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7e01640f9f2cb1220bbe80325e179e532cb3379ebcd1bf2279d703c19fe3a468"
+checksum = "559c5a40fdd30eb5e344fbceacf7595a81e242529fb4e21cf5f43fb4f11ff98d"
 dependencies = [
- "block2",
  "objc-sys",
  "objc2-encode",
 ]
 
 [[package]]
 name = "objc2-encode"
-version = "2.0.0-pre.2"
+version = "3.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abfcac41015b00a120608fdaa6938c44cb983fee294351cc4bac7638b4e50512"
-dependencies = [
- "objc-sys",
-]
+checksum = "d079845b37af429bfe5dfa76e6d087d788031045b25cfc6fd898486fd9847666"
 
 [[package]]
 name = "objc_exception"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ad970fb455818ad6cba4c122ad012fae53ae8b4795f86378bce65e4f6bab2ca4"
 dependencies = [
@@ -4306,15 +4400,15 @@
 [[package]]
 name = "petgraph"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1d3afd2628e69da2be385eb6f2fd57c8ac7977ceeff6dc166ff1657b0e386a9"
 dependencies = [
  "fixedbitset",
- "indexmap 2.1.0",
+ "indexmap 2.2.5",
 ]
 
 [[package]]
 name = "phf"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ade2d8b8f33c7333b51bcf0428d37e217e9f32192ae4772156f65063b8ce03dc"
@@ -4447,14 +4541,28 @@
  "crc32fast",
  "fdeflate",
  "flate2",
  "miniz_oxide",
 ]
 
 [[package]]
+name = "polling"
+version = "3.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "30054e72317ab98eddd8561db0f6524df3367636884b7b21b703e4b280a84a14"
+dependencies = [
+ "cfg-if",
+ "concurrent-queue",
+ "pin-project-lite",
+ "rustix",
+ "tracing",
+ "windows-sys 0.52.0",
+]
+
+[[package]]
 name = "pollster"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "22686f4785f02a4fcc856d3b3bb19bf6c8160d103f7a99cc258bddd0251dc7f2"
 
 [[package]]
 name = "polyval"
@@ -4729,14 +4837,23 @@
 [[package]]
 name = "quick-error"
 version = "2.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a993555f31e5a609f617c12db6250dedcac1b0a85076912c436e6fc9b2c8e6a3"
 
 [[package]]
+name = "quick-xml"
+version = "0.31.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1004a344b30a54e2ee58d66a71b32d2db2feb0a31f9a2d302bf0536f15de2a33"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "quote"
 version = "1.0.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
 dependencies = [
  "proc-macro2",
 ]
@@ -4787,17 +4904,17 @@
 name = "rangemap"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "977b1e897f9d764566891689e642653e5ed90c6895106acd005eb4c1d0203991"
 
 [[package]]
 name = "raw-window-handle"
-version = "0.5.2"
+version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f2ff9a1f06a88b01621b7ae906ef0211290d1c8a168a15542486a8f61c0833b9"
+checksum = "42a9830a0e1b9fb145ebb365b8bc4ccd75f290f98c0247deafbbe2c75cefb544"
 
 [[package]]
 name = "rayon"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fa7237101a77a10773db45d62004a272517633fbcc3df19d96455ede1122e051"
 dependencies = [
@@ -4979,15 +5096,15 @@
  "gif",
  "jpeg-decoder",
  "log",
  "pico-args",
  "png",
  "rgb",
  "svgtypes 0.12.0",
- "tiny-skia 0.11.3",
+ "tiny-skia",
  "usvg 0.36.0",
 ]
 
 [[package]]
 name = "resvg"
 version = "0.38.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -4996,15 +5113,15 @@
  "gif",
  "jpeg-decoder",
  "log",
  "pico-args",
  "png",
  "rgb",
  "svgtypes 0.13.0",
- "tiny-skia 0.11.3",
+ "tiny-skia",
  "usvg 0.38.0",
 ]
 
 [[package]]
 name = "rexif"
 version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -5359,23 +5476,23 @@
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
 name = "sctk-adwaita"
-version = "0.5.4"
+version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cda4e97be1fd174ccc2aae81c8b694e803fa99b34e8fd0f057a9d70698e3ed09"
+checksum = "82b2eaf3a5b264a521b988b2e73042e742df700c4f962cde845d1541adb46550"
 dependencies = [
  "ab_glyph",
  "log",
- "memmap2 0.5.10",
+ "memmap2 0.9.4",
  "smithay-client-toolkit",
- "tiny-skia 0.8.4",
+ "tiny-skia",
 ]
 
 [[package]]
 name = "sec1"
 version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d3e97a565f76233a6003f9f5c54be1d9c5bdfa3eccfb189469f11ec4901c47dc"
@@ -5454,14 +5571,25 @@
 checksum = "f3a1a3341211875ef120e117ea7fd5228530ae7e7036a779fdc9117be6b3282c"
 dependencies = [
  "ordered-float",
  "serde",
 ]
 
 [[package]]
+name = "serde-wasm-bindgen"
+version = "0.6.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8302e169f0eddcc139c70f139d19d6467353af16f9fce27e8c30158036a1e16b"
+dependencies = [
+ "js-sys",
+ "serde",
+ "wasm-bindgen",
+]
+
+[[package]]
 name = "serde_bytes"
 version = "0.11.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ab33ec92f677585af6d88c65593ae2375adde54efdbf16d597f2cbc7a6d368ff"
 dependencies = [
  "serde",
 ]
@@ -5475,19 +5603,19 @@
  "proc-macro2",
  "quote",
  "syn 2.0.47",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.111"
+version = "1.0.114"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "176e46fa42316f18edd598015a5166857fc835ec732f5215eac6b7bdbf0a84f4"
+checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
 dependencies = [
- "indexmap 2.1.0",
+ "indexmap 2.2.5",
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_urlencoded"
@@ -5643,29 +5771,44 @@
  "autocfg",
  "static_assertions",
  "version_check",
 ]
 
 [[package]]
 name = "smithay-client-toolkit"
-version = "0.16.1"
+version = "0.18.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "870427e30b8f2cbe64bf43ec4b86e88fe39b0a84b3f15efd9c9c2d020bc86eb9"
+checksum = "922fd3eeab3bd820d76537ce8f582b1cf951eceb5475c28500c7457d9d17f53a"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.4.1",
  "calloop",
- "dlib",
- "lazy_static",
+ "calloop-wayland-source",
+ "cursor-icon",
+ "libc",
  "log",
- "memmap2 0.5.10",
- "nix 0.24.3",
- "pkg-config",
+ "memmap2 0.9.4",
+ "rustix",
+ "thiserror",
+ "wayland-backend",
  "wayland-client",
+ "wayland-csd-frame",
  "wayland-cursor",
  "wayland-protocols",
+ "wayland-protocols-wlr",
+ "wayland-scanner",
+ "xkeysym",
+]
+
+[[package]]
+name = "smol_str"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e6845563ada680337a52d43bb0b29f396f2d911616f6573012645b9e3d048a49"
+dependencies = [
+ "serde",
 ]
 
 [[package]]
 name = "socket2"
 version = "0.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b5fac59a5cb5dd637972e5fca70daf0523c9067fcdc4842f053dae04a18f8e9"
@@ -5719,20 +5862,19 @@
 checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
 dependencies = [
  "lock_api",
 ]
 
 [[package]]
 name = "spirv"
-version = "0.2.0+1.5.4"
+version = "0.3.0+sdk-1.3.268.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "246bfa38fe3db3f1dfc8ca5a2cdeb7348c78be2112740cc0ec8ef18b6d94f830"
+checksum = "eda41003dc44290527a59b13432d4a0379379fa074b70174882adfbdfd917844"
 dependencies = [
- "bitflags 1.3.2",
- "num-traits",
+ "bitflags 2.4.1",
 ]
 
 [[package]]
 name = "spki"
 version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d91ed6c858b01f942cd56b37a94b3e0a1798290327d1236e4d9cf4eaca44d29d"
@@ -6365,17 +6507,17 @@
  "redox_syscall 0.4.1",
  "rustix",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "termcolor"
-version = "1.4.0"
+version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ff1bc3d3f05aff0403e8ac0d92ced918ec05b666a43f83297ccef5bea8a3d449"
+checksum = "06794f8f6c5c898b3275aebefa6b8a1cb24cd2c6c79397ab15774837a0bc5755"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "text_lines"
 version = "0.6.0"
@@ -6383,26 +6525,26 @@
 checksum = "7fd5828de7deaa782e1dd713006ae96b3bee32d3279b79eb67ecf8072c059bcf"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.52"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "83a48fd946b02c0a526b2e9481c8e2a17755e47039164a86c4070446e3a4614d"
+checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.52"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7fbe9b594d6568a6a1443250a7e67d80b74e1e96f6d1715e1e21cc1888291d3"
+checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.47",
 ]
 
 [[package]]
@@ -6453,50 +6595,25 @@
 checksum = "26197e33420244aeb70c3e8c78376ca46571bc4e701e4791c2cd9f57dcb3a43f"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
 name = "tiny-skia"
-version = "0.8.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "df8493a203431061e901613751931f047d1971337153f96d0e5e363d6dbf6a67"
-dependencies = [
- "arrayref",
- "arrayvec",
- "bytemuck",
- "cfg-if",
- "png",
- "tiny-skia-path 0.8.4",
-]
-
-[[package]]
-name = "tiny-skia"
 version = "0.11.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6a067b809476893fce6a254cf285850ff69c847e6cfbade6a20b655b6c7e80d"
 dependencies = [
  "arrayref",
  "arrayvec",
  "bytemuck",
  "cfg-if",
  "log",
  "png",
- "tiny-skia-path 0.11.3",
-]
-
-[[package]]
-name = "tiny-skia-path"
-version = "0.8.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "adbfb5d3f3dd57a0e11d12f4f13d4ebbbc1b5c15b7ab0a156d030b21da5f677c"
-dependencies = [
- "arrayref",
- "bytemuck",
- "strict-num",
+ "tiny-skia-path",
 ]
 
 [[package]]
 name = "tiny-skia-path"
 version = "0.11.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5de35e8a90052baaaf61f171680ac2f8e925a1e43ea9d2e3a00514772250e541"
@@ -6637,15 +6754,15 @@
 
 [[package]]
 name = "toml_edit"
 version = "0.19.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b5bb770da30e5cbfde35a2d7b9b8a2c4b8ef89548a7a6aeab5c9a576e3e7421"
 dependencies = [
- "indexmap 2.1.0",
+ "indexmap 2.2.5",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
 name = "tower-service"
 version = "0.3.2"
@@ -7062,26 +7179,26 @@
 version = "0.36.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6cacb0c5edeaf3e80e5afcf5b0d4004cc1d36318befc9a7c6606507e5d0f4062"
 dependencies = [
  "rctree",
  "strict-num",
  "svgtypes 0.12.0",
- "tiny-skia-path 0.11.3",
+ "tiny-skia-path",
 ]
 
 [[package]]
 name = "usvg-tree"
 version = "0.38.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "18863e0404ed153d6e56362c5b1146db9f4f262a3244e3cf2dbe7d8a85909f05"
 dependencies = [
  "strict-num",
  "svgtypes 0.13.0",
- "tiny-skia-path 0.11.3",
+ "tiny-skia-path",
 ]
 
 [[package]]
 name = "utf-8"
 version = "0.7.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "09cc8ee72d2a9becf2f2febe0205bbed8fc6615b7cb429ad062dc7b7ddd036a9"
@@ -7123,20 +7240,14 @@
 [[package]]
 name = "vcpkg"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "accd4ea62f7bb7a82fe23066fb0957d48ef677f6eeb8215f372f52e48bb32426"
 
 [[package]]
-name = "vec_map"
-version = "0.8.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1bddf1187be692e79c5ffeab891132dfb0f236ed36a43c7ed39f1165ee20191"
-
-[[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "vl-convert-pdf"
@@ -7178,15 +7289,15 @@
  "png",
  "regex",
  "reqwest",
  "resvg 0.36.0",
  "serde",
  "serde_json",
  "tempfile",
- "tiny-skia 0.11.3",
+ "tiny-skia",
  "tokio",
  "usvg 0.36.0",
  "vl-convert-pdf",
 ]
 
 [[package]]
 name = "vsimd"
@@ -7238,77 +7349,77 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
  "syn 2.0.47",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.37"
+version = "0.4.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c02dbc21516f9f1f04f187958890d7e6026df8d16540b7ad9492bc34a67cea03"
+checksum = "76bc14366121efc8dbb487ab05bcc9d346b3b5ec0eaa76e46594cabbe51762c0"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.47",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.87"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
 name = "wasm-streams"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b4609d447824375f43e1ffbc051b50ad8f4b3ae8219680c94452ea05eb240ac7"
 dependencies = [
@@ -7316,91 +7427,137 @@
  "js-sys",
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
 ]
 
 [[package]]
-name = "wayland-client"
-version = "0.29.5"
+name = "wayland-backend"
+version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3f3b068c05a039c9f755f881dc50f01732214f5685e379829759088967c46715"
+checksum = "9d50fa61ce90d76474c87f5fc002828d81b32677340112b4ef08079a9d459a40"
 dependencies = [
- "bitflags 1.3.2",
+ "cc",
  "downcast-rs",
- "libc",
- "nix 0.24.3",
+ "rustix",
  "scoped-tls",
- "wayland-commons",
- "wayland-scanner",
+ "smallvec",
  "wayland-sys",
 ]
 
 [[package]]
-name = "wayland-commons"
-version = "0.29.5"
+name = "wayland-client"
+version = "0.31.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8691f134d584a33a6606d9d717b95c4fa20065605f798a3f350d78dced02a902"
+checksum = "82fb96ee935c2cea6668ccb470fb7771f6215d1691746c2d896b447a00ad3f1f"
 dependencies = [
- "nix 0.24.3",
- "once_cell",
- "smallvec",
- "wayland-sys",
+ "bitflags 2.4.1",
+ "rustix",
+ "wayland-backend",
+ "wayland-scanner",
+]
+
+[[package]]
+name = "wayland-csd-frame"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "625c5029dbd43d25e6aa9615e88b829a5cad13b2819c4ae129fdbb7c31ab4c7e"
+dependencies = [
+ "bitflags 2.4.1",
+ "cursor-icon",
+ "wayland-backend",
 ]
 
 [[package]]
 name = "wayland-cursor"
-version = "0.29.5"
+version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6865c6b66f13d6257bef1cd40cbfe8ef2f150fb8ebbdb1e8e873455931377661"
+checksum = "71ce5fa868dd13d11a0d04c5e2e65726d0897be8de247c0c5a65886e283231ba"
 dependencies = [
- "nix 0.24.3",
+ "rustix",
  "wayland-client",
  "xcursor",
 ]
 
 [[package]]
 name = "wayland-protocols"
-version = "0.29.5"
+version = "0.31.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b950621f9354b322ee817a23474e479b34be96c2e909c14f7bc0100e9a970bc6"
+checksum = "8f81f365b8b4a97f422ac0e8737c438024b5951734506b0e1d775c73030561f4"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.4.1",
+ "wayland-backend",
+ "wayland-client",
+ "wayland-scanner",
+]
+
+[[package]]
+name = "wayland-protocols-plasma"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "23803551115ff9ea9bce586860c5c5a971e360825a0309264102a9495a5ff479"
+dependencies = [
+ "bitflags 2.4.1",
+ "wayland-backend",
  "wayland-client",
- "wayland-commons",
+ "wayland-protocols",
+ "wayland-scanner",
+]
+
+[[package]]
+name = "wayland-protocols-wlr"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ad1f61b76b6c2d8742e10f9ba5c3737f6530b4c243132c2a2ccc8aa96fe25cd6"
+dependencies = [
+ "bitflags 2.4.1",
+ "wayland-backend",
+ "wayland-client",
+ "wayland-protocols",
  "wayland-scanner",
 ]
 
 [[package]]
 name = "wayland-scanner"
-version = "0.29.5"
+version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f4303d8fa22ab852f789e75a967f0a2cdc430a607751c0499bada3e451cbd53"
+checksum = "63b3a62929287001986fb58c789dce9b67604a397c15c611ad9f747300b6c283"
 dependencies = [
  "proc-macro2",
+ "quick-xml",
  "quote",
- "xml-rs",
 ]
 
 [[package]]
 name = "wayland-sys"
-version = "0.29.5"
+version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be12ce1a3c39ec7dba25594b97b42cb3195d54953ddb9d3d95a7c3902bc6e9d4"
+checksum = "15a0c8eaff5216d07f226cb7a549159267f3467b289d9a2e52fd3ef5aae2b7af"
 dependencies = [
  "dlib",
- "lazy_static",
+ "log",
+ "once_cell",
  "pkg-config",
 ]
 
 [[package]]
 name = "web-sys"
-version = "0.3.64"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b85cbef8c220a6abc02aefd892dfc0fc23afb1c6a426316ec33253a3877249b"
+checksum = "77afa9a11836342370f4817622a2f0f418b134426d91a82dfb48f532d2ec13ef"
+dependencies = [
+ "js-sys",
+ "wasm-bindgen",
+]
+
+[[package]]
+name = "web-time"
+version = "0.2.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aa30049b1c872b72c89866d458eae9f20380ab280ffd1b1e18df2d3e2d98cfe0"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "webpki-roots"
@@ -7412,21 +7569,21 @@
 name = "weezl"
 version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9193164d4de03a926d909d3bc7c30543cecb35400c02114792c2cae20d5e2dbb"
 
 [[package]]
 name = "wgpu"
-version = "0.18.0"
+version = "0.19.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "30e7d227c9f961f2061c26f4cb0fbd4df0ef37e056edd0931783599d6c94ef24"
+checksum = "a4b1213b52478a7631d6e387543ed8f642bc02c578ef4e3b49aca2a29a7df0cb"
 dependencies = [
  "arrayvec",
  "cfg-if",
- "flume",
+ "cfg_aliases",
  "js-sys",
  "log",
  "naga",
  "parking_lot 0.12.1",
  "profiling",
  "raw-window-handle",
  "smallvec",
@@ -7437,47 +7594,51 @@
  "wgpu-core",
  "wgpu-hal",
  "wgpu-types",
 ]
 
 [[package]]
 name = "wgpu-core"
-version = "0.18.1"
+version = "0.19.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ef91c1d62d1e9e81c79e600131a258edf75c9531cbdbde09c44a011a47312726"
+checksum = "f9f6b033c2f00ae0bc8ea872c5989777c60bc241aac4e58b24774faa8b391f78"
 dependencies = [
  "arrayvec",
  "bit-vec",
  "bitflags 2.4.1",
+ "cfg_aliases",
  "codespan-reporting",
+ "indexmap 2.2.5",
  "log",
  "naga",
+ "once_cell",
  "parking_lot 0.12.1",
  "profiling",
  "raw-window-handle",
  "rustc-hash",
  "smallvec",
  "thiserror",
  "web-sys",
  "wgpu-hal",
  "wgpu-types",
 ]
 
 [[package]]
 name = "wgpu-hal"
-version = "0.18.1"
+version = "0.19.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b84ecc802da3eb67b4cf3dd9ea6fe45bbb47ef13e6c49c5c3240868a9cc6cdd9"
+checksum = "49f972c280505ab52ffe17e94a7413d9d54b58af0114ab226b9fc4999a47082e"
 dependencies = [
  "android_system_properties",
  "arrayvec",
  "ash",
  "bit-set",
  "bitflags 2.4.1",
  "block",
+ "cfg_aliases",
  "core-graphics-types",
  "d3d12",
  "glow",
  "glutin_wgl_sys",
  "gpu-alloc",
  "gpu-allocator",
  "gpu-descriptor",
@@ -7485,14 +7646,15 @@
  "js-sys",
  "khronos-egl",
  "libc",
  "libloading 0.8.1",
  "log",
  "metal",
  "naga",
+ "ndk-sys",
  "objc",
  "once_cell",
  "parking_lot 0.12.1",
  "profiling",
  "range-alloc",
  "raw-window-handle",
  "renderdoc-sys",
@@ -7503,17 +7665,17 @@
  "web-sys",
  "wgpu-types",
  "winapi",
 ]
 
 [[package]]
 name = "wgpu-types"
-version = "0.18.0"
+version = "0.19.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d5ed5f0edf0de351fe311c53304986315ce866f394a2e6df0c4b3c70774bcdd"
+checksum = "b671ff9fb03f78b46ff176494ee1ebe7d603393f42664be55b64dc8d53969805"
 dependencies = [
  "bitflags 2.4.1",
  "js-sys",
  "web-sys",
 ]
 
 [[package]]
@@ -7790,45 +7952,58 @@
 name = "windows_x86_64_msvc"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dff9641d1cd4be8d1a070daf9e3773c5f67e78b4d9d42263020c057706765c04"
 
 [[package]]
 name = "winit"
-version = "0.28.7"
+version = "0.29.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9596d90b45384f5281384ab204224876e8e8bf7d58366d9b795ad99aa9894b94"
+checksum = "0d59ad965a635657faf09c8f062badd885748428933dad8e8bdd64064d92e5ca"
 dependencies = [
+ "ahash",
  "android-activity",
- "bitflags 1.3.2",
+ "atomic-waker",
+ "bitflags 2.4.1",
+ "bytemuck",
+ "calloop",
  "cfg_aliases",
  "core-foundation",
  "core-graphics",
- "dispatch",
- "instant",
+ "cursor-icon",
+ "icrate",
+ "js-sys",
  "libc",
  "log",
- "mio",
+ "memmap2 0.9.4",
  "ndk",
+ "ndk-sys",
  "objc2",
  "once_cell",
  "orbclient",
  "percent-encoding",
  "raw-window-handle",
  "redox_syscall 0.3.5",
+ "rustix",
  "sctk-adwaita",
  "smithay-client-toolkit",
+ "smol_str",
+ "unicode-segmentation",
  "wasm-bindgen",
+ "wasm-bindgen-futures",
+ "wayland-backend",
  "wayland-client",
- "wayland-commons",
  "wayland-protocols",
- "wayland-scanner",
+ "wayland-protocols-plasma",
  "web-sys",
- "windows-sys 0.45.0",
+ "web-time",
+ "windows-sys 0.48.0",
  "x11-dl",
+ "x11rb",
+ "xkbcommon-dl",
 ]
 
 [[package]]
 name = "winnow"
 version = "0.5.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b5c3db89721d50d0e2a673f5043fc4722f76dcc352d7b1ab8b8288bed4ed2c5"
@@ -7863,14 +8038,35 @@
 dependencies = [
  "libc",
  "once_cell",
  "pkg-config",
 ]
 
 [[package]]
+name = "x11rb"
+version = "0.13.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f8f25ead8c7e4cba123243a6367da5d3990e0d3affa708ea19dce96356bd9f1a"
+dependencies = [
+ "as-raw-xcb-connection",
+ "gethostname",
+ "libc",
+ "libloading 0.8.1",
+ "once_cell",
+ "rustix",
+ "x11rb-protocol",
+]
+
+[[package]]
+name = "x11rb-protocol"
+version = "0.13.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e63e71c4b8bd9ffec2c963173a4dc4cbde9ee96961d4fcb4429db9929b606c34"
+
+[[package]]
 name = "x25519-dalek"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb66477291e7e8d2b0ff1bcb900bf29489a9692816d79874bea351e7a8b6de96"
 dependencies = [
  "curve25519-dalek",
  "rand_core",
@@ -7898,14 +8094,33 @@
 [[package]]
 name = "xcursor"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a0ccd7b4a5345edfcd0c3535718a4e9ff7798ffc536bb5b5a0e26ff84732911"
 
 [[package]]
+name = "xkbcommon-dl"
+version = "0.4.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d039de8032a9a8856a6be89cea3e5d12fdd82306ab7c94d74e6deab2460651c5"
+dependencies = [
+ "bitflags 2.4.1",
+ "dlib",
+ "log",
+ "once_cell",
+ "xkeysym",
+]
+
+[[package]]
+name = "xkeysym"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "054a8e68b76250b253f671d1268cb7f1ae089ec35e195b2efb2a4e9a836d0621"
+
+[[package]]
 name = "xml-rs"
 version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fcb9cbac069e033553e8bb871be2fbdffcab578eb25bd0f7c508cedc6dcd75a"
 
 [[package]]
 name = "xmlparser"
```

### Comparing `avenger-0.0.3/README.md` & `avenger-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `avenger-0.0.3/LICENSE` & `avenger-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `avenger-0.0.3/PKG-INFO` & `avenger-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: avenger
-Version: 0.0.3
+Version: 0.0.4
 License-File: LICENSE
 Summary: A Visualization Engine and Renderer
 License: BSD-3-Clause
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # Avenger: A visualization engine and renderer
 Avenger is an early stage prototype of a new foundational rendering library for information visualization (InfoVis) systems. Avenger defines a 2D scenegraph representation tailored to the needs of InfoVis systems. To start with, the initial application of Avenger is to serve as an alternative, GPU accelerated, rendering backend for Vega visualizations.
```


# Comparing `tmp/xminigrid-0.7.0.tar.gz` & `tmp/xminigrid-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xminigrid-0.7.0.tar", last modified: Sun Mar 24 10:54:45 2024, max compression
+gzip compressed data, was "xminigrid-0.7.1.tar", last modified: Wed May  1 13:24:58 2024, max compression
```

## Comparing `xminigrid-0.7.0.tar` & `xminigrid-0.7.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 a.p.nikulin   (503) staff       (20)        0 2024-03-24 10:54:45.734533 xminigrid-0.7.0/
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)    11357 2024-02-01 08:42:11.000000 xminigrid-0.7.0/LICENSE
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)    31136 2024-03-24 10:54:45.734183 xminigrid-0.7.0/PKG-INFO
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)    16538 2024-03-24 10:53:49.000000 xminigrid-0.7.0/README.md
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     2346 2024-03-24 10:53:49.000000 xminigrid-0.7.0/pyproject.toml
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)       38 2024-03-24 10:54:45.734575 xminigrid-0.7.0/setup.cfg
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)      131 2023-12-01 17:14:46.000000 xminigrid-0.7.0/setup.py
-drwxr-xr-x   0 a.p.nikulin   (503) staff       (20)        0 2024-03-24 10:54:45.710731 xminigrid-0.7.0/src/
-drwxr-xr-x   0 a.p.nikulin   (503) staff       (20)        0 2024-03-24 10:54:45.718490 xminigrid-0.7.0/src/xminigrid/
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     7107 2024-03-24 10:53:49.000000 xminigrid-0.7.0/src/xminigrid/__init__.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     4447 2024-03-24 10:53:49.000000 xminigrid-0.7.0/src/xminigrid/benchmarks.py
-drwxr-xr-x   0 a.p.nikulin   (503) staff       (20)        0 2024-03-24 10:54:45.724229 xminigrid-0.7.0/src/xminigrid/core/
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     4638 2024-02-13 10:01:27.000000 xminigrid-0.7.0/src/xminigrid/core/actions.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     2597 2024-03-24 10:53:49.000000 xminigrid-0.7.0/src/xminigrid/core/constants.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)    13357 2024-01-22 07:21:10.000000 xminigrid-0.7.0/src/xminigrid/core/goals.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     7006 2024-03-24 10:53:49.000000 xminigrid-0.7.0/src/xminigrid/core/grid.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     5144 2024-03-24 10:53:49.000000 xminigrid-0.7.0/src/xminigrid/core/observation.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)    16607 2024-03-24 10:53:49.000000 xminigrid-0.7.0/src/xminigrid/core/rules.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     4233 2024-03-02 10:45:31.000000 xminigrid-0.7.0/src/xminigrid/environment.py
-drwxr-xr-x   0 a.p.nikulin   (503) staff       (20)        0 2024-03-24 10:54:45.725414 xminigrid-0.7.0/src/xminigrid/envs/
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)      641 2023-12-01 17:14:47.000000 xminigrid-0.7.0/src/xminigrid/envs/__init__.py
-drwxr-xr-x   0 a.p.nikulin   (503) staff       (20)        0 2024-03-24 10:54:45.729585 xminigrid-0.7.0/src/xminigrid/envs/minigrid/
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     3184 2024-02-13 10:01:27.000000 xminigrid-0.7.0/src/xminigrid/envs/minigrid/blockedunlockpickup.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     2443 2024-02-13 10:01:27.000000 xminigrid-0.7.0/src/xminigrid/envs/minigrid/doorkey.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     2593 2024-02-13 10:01:27.000000 xminigrid-0.7.0/src/xminigrid/envs/minigrid/empty.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     2303 2024-02-13 10:01:27.000000 xminigrid-0.7.0/src/xminigrid/envs/minigrid/fourrooms.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     4712 2024-02-13 10:01:27.000000 xminigrid-0.7.0/src/xminigrid/envs/minigrid/lockedroom.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     5340 2024-02-13 10:01:27.000000 xminigrid-0.7.0/src/xminigrid/envs/minigrid/memory.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     3209 2024-02-13 10:01:27.000000 xminigrid-0.7.0/src/xminigrid/envs/minigrid/playground.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     2433 2024-02-13 10:01:27.000000 xminigrid-0.7.0/src/xminigrid/envs/minigrid/unlock.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     2854 2024-02-13 10:01:27.000000 xminigrid-0.7.0/src/xminigrid/envs/minigrid/unlockpickup.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     7729 2024-03-24 10:53:49.000000 xminigrid-0.7.0/src/xminigrid/envs/xland.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     3757 2024-02-07 15:00:54.000000 xminigrid-0.7.0/src/xminigrid/envs/xland_tmp.py
-drwxr-xr-x   0 a.p.nikulin   (503) staff       (20)        0 2024-03-24 10:54:45.729955 xminigrid-0.7.0/src/xminigrid/experimental/
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     3701 2024-03-24 10:53:49.000000 xminigrid-0.7.0/src/xminigrid/experimental/img_obs.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     7075 2024-03-24 10:53:49.000000 xminigrid-0.7.0/src/xminigrid/manual_control.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     1785 2024-02-13 10:01:27.000000 xminigrid-0.7.0/src/xminigrid/registration.py
-drwxr-xr-x   0 a.p.nikulin   (503) staff       (20)        0 2024-03-24 10:54:45.731694 xminigrid-0.7.0/src/xminigrid/rendering/
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     9269 2024-03-24 10:53:49.000000 xminigrid-0.7.0/src/xminigrid/rendering/rgb_render.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     5206 2024-03-24 10:53:49.000000 xminigrid-0.7.0/src/xminigrid/rendering/text_render.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     3597 2024-02-13 10:01:27.000000 xminigrid-0.7.0/src/xminigrid/rendering/utils.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     1633 2024-02-13 10:01:27.000000 xminigrid-0.7.0/src/xminigrid/types.py
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     2677 2024-03-24 10:53:49.000000 xminigrid-0.7.0/src/xminigrid/wrappers.py
-drwxr-xr-x   0 a.p.nikulin   (503) staff       (20)        0 2024-03-24 10:54:45.732859 xminigrid-0.7.0/src/xminigrid.egg-info/
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)    31136 2024-03-24 10:54:45.000000 xminigrid-0.7.0/src/xminigrid.egg-info/PKG-INFO
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)     1209 2024-03-24 10:54:45.000000 xminigrid-0.7.0/src/xminigrid.egg-info/SOURCES.txt
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)        1 2024-03-24 10:54:45.000000 xminigrid-0.7.0/src/xminigrid.egg-info/dependency_links.txt
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)      260 2024-03-24 10:54:45.000000 xminigrid-0.7.0/src/xminigrid.egg-info/requires.txt
--rw-r--r--   0 a.p.nikulin   (503) staff       (20)       10 2024-03-24 10:54:45.000000 xminigrid-0.7.0/src/xminigrid.egg-info/top_level.txt
+drwxr-xr-x   0 a.p.nikulin   (503) staff       (20)        0 2024-05-01 13:24:58.813810 xminigrid-0.7.1/
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)    11357 2024-02-01 08:42:11.000000 xminigrid-0.7.1/LICENSE
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)    31136 2024-05-01 13:24:58.811986 xminigrid-0.7.1/PKG-INFO
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)    16538 2024-03-24 10:53:49.000000 xminigrid-0.7.1/README.md
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)     2346 2024-04-09 13:16:59.000000 xminigrid-0.7.1/pyproject.toml
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)       38 2024-05-01 13:24:58.813856 xminigrid-0.7.1/setup.cfg
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)      131 2023-12-01 17:14:46.000000 xminigrid-0.7.1/setup.py
+drwxr-xr-x   0 a.p.nikulin   (503) staff       (20)        0 2024-05-01 13:24:58.793691 xminigrid-0.7.1/src/
+drwxr-xr-x   0 a.p.nikulin   (503) staff       (20)        0 2024-05-01 13:24:58.799039 xminigrid-0.7.1/src/xminigrid/
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)     7107 2024-04-09 07:56:53.000000 xminigrid-0.7.1/src/xminigrid/__init__.py
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)     4447 2024-03-24 10:53:49.000000 xminigrid-0.7.1/src/xminigrid/benchmarks.py
+drwxr-xr-x   0 a.p.nikulin   (503) staff       (20)        0 2024-05-01 13:24:58.803382 xminigrid-0.7.1/src/xminigrid/core/
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)     4638 2024-02-13 10:01:27.000000 xminigrid-0.7.1/src/xminigrid/core/actions.py
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)     2597 2024-03-24 10:53:49.000000 xminigrid-0.7.1/src/xminigrid/core/constants.py
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)    13372 2024-04-15 15:41:50.000000 xminigrid-0.7.1/src/xminigrid/core/goals.py
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)     7006 2024-03-24 10:53:49.000000 xminigrid-0.7.1/src/xminigrid/core/grid.py
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)     5144 2024-03-24 10:53:49.000000 xminigrid-0.7.1/src/xminigrid/core/observation.py
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)    16622 2024-04-30 14:39:53.000000 xminigrid-0.7.1/src/xminigrid/core/rules.py
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)     4233 2024-03-02 10:45:31.000000 xminigrid-0.7.1/src/xminigrid/environment.py
+drwxr-xr-x   0 a.p.nikulin   (503) staff       (20)        0 2024-05-01 13:24:58.804715 xminigrid-0.7.1/src/xminigrid/envs/
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)      641 2023-12-01 17:14:47.000000 xminigrid-0.7.1/src/xminigrid/envs/__init__.py
+drwxr-xr-x   0 a.p.nikulin   (503) staff       (20)        0 2024-05-01 13:24:58.809209 xminigrid-0.7.1/src/xminigrid/envs/minigrid/
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)     3184 2024-02-13 10:01:27.000000 xminigrid-0.7.1/src/xminigrid/envs/minigrid/blockedunlockpickup.py
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)     2443 2024-02-13 10:01:27.000000 xminigrid-0.7.1/src/xminigrid/envs/minigrid/doorkey.py
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)     2593 2024-02-13 10:01:27.000000 xminigrid-0.7.1/src/xminigrid/envs/minigrid/empty.py
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)     2303 2024-02-13 10:01:27.000000 xminigrid-0.7.1/src/xminigrid/envs/minigrid/fourrooms.py
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)     4712 2024-02-13 10:01:27.000000 xminigrid-0.7.1/src/xminigrid/envs/minigrid/lockedroom.py
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)     5370 2024-04-30 14:39:53.000000 xminigrid-0.7.1/src/xminigrid/envs/minigrid/memory.py
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)     3209 2024-02-13 10:01:27.000000 xminigrid-0.7.1/src/xminigrid/envs/minigrid/playground.py
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)     2433 2024-02-13 10:01:27.000000 xminigrid-0.7.1/src/xminigrid/envs/minigrid/unlock.py
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)     2854 2024-02-13 10:01:27.000000 xminigrid-0.7.1/src/xminigrid/envs/minigrid/unlockpickup.py
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)     7729 2024-03-24 10:53:49.000000 xminigrid-0.7.1/src/xminigrid/envs/xland.py
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)     3757 2024-02-07 15:00:54.000000 xminigrid-0.7.1/src/xminigrid/envs/xland_tmp.py
+drwxr-xr-x   0 a.p.nikulin   (503) staff       (20)        0 2024-05-01 13:24:58.809530 xminigrid-0.7.1/src/xminigrid/experimental/
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)     3701 2024-03-24 10:53:49.000000 xminigrid-0.7.1/src/xminigrid/experimental/img_obs.py
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)     7130 2024-04-16 13:33:53.000000 xminigrid-0.7.1/src/xminigrid/manual_control.py
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)     1785 2024-02-13 10:01:27.000000 xminigrid-0.7.1/src/xminigrid/registration.py
+drwxr-xr-x   0 a.p.nikulin   (503) staff       (20)        0 2024-05-01 13:24:58.810554 xminigrid-0.7.1/src/xminigrid/rendering/
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)     9278 2024-03-28 10:48:43.000000 xminigrid-0.7.1/src/xminigrid/rendering/rgb_render.py
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)     5206 2024-03-24 10:53:49.000000 xminigrid-0.7.1/src/xminigrid/rendering/text_render.py
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)     3597 2024-02-13 10:01:27.000000 xminigrid-0.7.1/src/xminigrid/rendering/utils.py
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)     1633 2024-02-13 10:01:27.000000 xminigrid-0.7.1/src/xminigrid/types.py
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)     2677 2024-03-24 10:53:49.000000 xminigrid-0.7.1/src/xminigrid/wrappers.py
+drwxr-xr-x   0 a.p.nikulin   (503) staff       (20)        0 2024-05-01 13:24:58.810952 xminigrid-0.7.1/src/xminigrid.egg-info/
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)    31136 2024-05-01 13:24:58.000000 xminigrid-0.7.1/src/xminigrid.egg-info/PKG-INFO
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)     1209 2024-05-01 13:24:58.000000 xminigrid-0.7.1/src/xminigrid.egg-info/SOURCES.txt
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)        1 2024-05-01 13:24:58.000000 xminigrid-0.7.1/src/xminigrid.egg-info/dependency_links.txt
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)      260 2024-05-01 13:24:58.000000 xminigrid-0.7.1/src/xminigrid.egg-info/requires.txt
+-rw-r--r--   0 a.p.nikulin   (503) staff       (20)       10 2024-05-01 13:24:58.000000 xminigrid-0.7.1/src/xminigrid.egg-info/top_level.txt
```

### Comparing `xminigrid-0.7.0/LICENSE` & `xminigrid-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.0/PKG-INFO` & `xminigrid-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xminigrid
-Version: 0.7.0
+Version: 0.7.1
 Summary: JAX-accelerated meta-reinforcement learning environments inspired by XLand and MiniGrid
 Author-email: Alexander Nikulin <a.p.nikulin@tinkoff.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `xminigrid-0.7.0/README.md` & `xminigrid-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.0/pyproject.toml` & `xminigrid-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.0/src/xminigrid/__init__.py` & `xminigrid-0.7.1/src/xminigrid/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .benchmarks import load_benchmark, registered_benchmarks
 from .registration import make, register, registered_environments
 
 # TODO: add __all__
-__version__ = "0.7.0"
+__version__ = "0.7.1"
 
 # ---------- XLand-MiniGrid environments ----------
 
 # WARN: TMP, only for FPS measurements
 # register(
 #     id="MiniGrid-1Rules",
 #     entry_point="xminigrid.envs.xland_tmp:XLandMiniGrid",
```

### Comparing `xminigrid-0.7.0/src/xminigrid/benchmarks.py` & `xminigrid-0.7.1/src/xminigrid/benchmarks.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.0/src/xminigrid/core/actions.py` & `xminigrid-0.7.1/src/xminigrid/core/actions.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.0/src/xminigrid/core/constants.py` & `xminigrid-0.7.1/src/xminigrid/core/constants.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.0/src/xminigrid/core/goals.py` & `xminigrid-0.7.1/src/xminigrid/core/goals.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import jax.numpy as jnp
 from flax import struct
 
 from ..types import AgentState, GridState
 from .grid import equal, get_neighbouring_tiles, pad_along_axis
 
 MAX_GOAL_ENCODING_LEN = 4 + 1  # for idx
+NUM_GOALS = 15
 
 
 def check_goal(
     encoding: jax.Array, grid: GridState, agent: AgentState, action: int | jax.Array, position: jax.Array
 ) -> jax.Array:
     check = jax.lax.switch(
         encoding[0],
```

### Comparing `xminigrid-0.7.0/src/xminigrid/core/grid.py` & `xminigrid-0.7.1/src/xminigrid/core/grid.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.0/src/xminigrid/core/observation.py` & `xminigrid-0.7.1/src/xminigrid/core/observation.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.0/src/xminigrid/core/rules.py` & `xminigrid-0.7.1/src/xminigrid/core/rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from flax import struct
 
 from ..types import AgentState, GridState
 from .constants import TILES_REGISTRY, Colors, Tiles
 from .grid import equal, get_neighbouring_tiles, pad_along_axis
 
 MAX_RULE_ENCODING_LEN = 6 + 1  # +1 for idx
+NUM_RULES = 12
 
 
 # this is very costly, will evaluate all rules under vmap. Submit a PR if you know how to do it better!
 # In general, we need a way to select specific function/class based on ID number.
 # We can not just decode without evaluation, as then return type will be different between branches
 def check_rule(
     encodings: jax.Array, grid: GridState, agent: AgentState, action: int | jax.Array, position: jax.Array
```

### Comparing `xminigrid-0.7.0/src/xminigrid/environment.py` & `xminigrid-0.7.1/src/xminigrid/environment.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.0/src/xminigrid/envs/__init__.py` & `xminigrid-0.7.1/src/xminigrid/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.0/src/xminigrid/envs/minigrid/blockedunlockpickup.py` & `xminigrid-0.7.1/src/xminigrid/envs/minigrid/blockedunlockpickup.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.0/src/xminigrid/envs/minigrid/doorkey.py` & `xminigrid-0.7.1/src/xminigrid/envs/minigrid/doorkey.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.0/src/xminigrid/envs/minigrid/empty.py` & `xminigrid-0.7.1/src/xminigrid/envs/minigrid/empty.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.0/src/xminigrid/envs/minigrid/fourrooms.py` & `xminigrid-0.7.1/src/xminigrid/envs/minigrid/fourrooms.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.0/src/xminigrid/envs/minigrid/lockedroom.py` & `xminigrid-0.7.1/src/xminigrid/envs/minigrid/lockedroom.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.0/src/xminigrid/envs/minigrid/memory.py` & `xminigrid-0.7.1/src/xminigrid/envs/minigrid/memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         )
         return state
 
     def step(
         self, params: EnvParams, timestep: TimeStep[MemoryEnvCarry], action: IntOrArray
     ) -> TimeStep[MemoryEnvCarry]:
         # disabling pick_up action
-        action = jax.lax.select(jnp.equal(action, 3), 5, action)
+        action = jax.lax.select(jnp.equal(action, 3), jnp.asarray(5, dtype=jnp.uint8), action)
         new_grid, new_agent, _ = take_action(timestep.state.grid, timestep.state.agent, action)
 
         new_state = timestep.state.replace(grid=new_grid, agent=new_agent, step_num=timestep.state.step_num + 1)
         new_observation = transparent_field_of_view(new_state.grid, new_state.agent, params.view_size, params.view_size)
 
         truncated = new_state.step_num == self.time_limit(params)
         terminated = jnp.logical_or(
```

### Comparing `xminigrid-0.7.0/src/xminigrid/envs/minigrid/playground.py` & `xminigrid-0.7.1/src/xminigrid/envs/minigrid/playground.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.0/src/xminigrid/envs/minigrid/unlock.py` & `xminigrid-0.7.1/src/xminigrid/envs/minigrid/unlock.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.0/src/xminigrid/envs/minigrid/unlockpickup.py` & `xminigrid-0.7.1/src/xminigrid/envs/minigrid/unlockpickup.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.0/src/xminigrid/envs/xland.py` & `xminigrid-0.7.1/src/xminigrid/envs/xland.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.0/src/xminigrid/envs/xland_tmp.py` & `xminigrid-0.7.1/src/xminigrid/envs/xland_tmp.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.0/src/xminigrid/experimental/img_obs.py` & `xminigrid-0.7.1/src/xminigrid/experimental/img_obs.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.0/src/xminigrid/manual_control.py` & `xminigrid-0.7.1/src/xminigrid/manual_control.py`

 * *Files 9% similar despite different names*

```diff
@@ -112,39 +112,35 @@
                 if event.type == pygame.KEYDOWN:
                     event.key = pygame.key.name(int(event.key))
                     self.key_handler(event)
 
     def step(self, action: int) -> None:
         self.timestep = self._step(self.env_params, self.timestep, action)
         print(
-            "StepType: ",
-            self.timestep.step_type,
-            "Discount: ",
-            self.timestep.discount,
-            "Reward: ",
-            self.timestep.reward,
+            f"Step: {self.timestep.state.step_num} | ",
+            f"StepType: {self.timestep.step_type} | ",
+            f"Discount: {self.timestep.discount} | ",
+            f"Reward: {self.timestep.reward}",
         )
         self.render()
 
         if self.timestep.last():
             self.reset()
 
     def reset(self) -> None:
         print("Reset!")
         self._key, reset_key = jax.random.split(self._key)
 
         self.timestep = self._reset(self.env_params, reset_key)
         self.render()
         print(
-            "StepType: ",
-            self.timestep.step_type,
-            "Discount: ",
-            self.timestep.discount,
-            "Reward: ",
-            self.timestep.reward,
+            f"Step: {self.timestep.state.step_num} |",
+            f"StepType: {self.timestep.step_type} |",
+            f"Discount: {self.timestep.discount} |",
+            f"Reward: {self.timestep.reward}",
         )
 
     def key_handler(self, event: Event) -> None:
         key: str = event.key
         print("pressed", key)
 
         if key == "escape":
```

### Comparing `xminigrid-0.7.0/src/xminigrid/registration.py` & `xminigrid-0.7.1/src/xminigrid/registration.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.0/src/xminigrid/rendering/rgb_render.py` & `xminigrid-0.7.1/src/xminigrid/rendering/rgb_render.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,15 +246,15 @@
         for x in range(grid.shape[1]):
             if agent is not None and np.array_equal((y, x), agent.position):
                 agent_direction = int(agent.direction)
             else:
                 agent_direction = None
 
             tile_img = render_tile(
-                tile=tuple(grid[y, x]),
+                tile=tuple(grid[y, x].tolist()),
                 agent_direction=agent_direction,
                 highlight=highlight_mask[y, x],
                 tile_size=int(tile_size),
             )
 
             ymin = y * int(tile_size)
             ymax = (y + 1) * int(tile_size)
```

### Comparing `xminigrid-0.7.0/src/xminigrid/rendering/text_render.py` & `xminigrid-0.7.1/src/xminigrid/rendering/text_render.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.0/src/xminigrid/rendering/utils.py` & `xminigrid-0.7.1/src/xminigrid/rendering/utils.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.0/src/xminigrid/types.py` & `xminigrid-0.7.1/src/xminigrid/types.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.0/src/xminigrid/wrappers.py` & `xminigrid-0.7.1/src/xminigrid/wrappers.py`

 * *Files identical despite different names*

### Comparing `xminigrid-0.7.0/src/xminigrid.egg-info/PKG-INFO` & `xminigrid-0.7.1/src/xminigrid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xminigrid
-Version: 0.7.0
+Version: 0.7.1
 Summary: JAX-accelerated meta-reinforcement learning environments inspired by XLand and MiniGrid
 Author-email: Alexander Nikulin <a.p.nikulin@tinkoff.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `xminigrid-0.7.0/src/xminigrid.egg-info/SOURCES.txt` & `xminigrid-0.7.1/src/xminigrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*


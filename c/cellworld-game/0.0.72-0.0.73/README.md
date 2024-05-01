# Comparing `tmp/cellworld_game-0.0.72.tar.gz` & `tmp/cellworld_game-0.0.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellworld_game-0.0.72.tar", last modified: Wed May  1 01:42:08 2024, max compression
+gzip compressed data, was "cellworld_game-0.0.73.tar", last modified: Wed May  1 03:16:52 2024, max compression
```

## Comparing `cellworld_game-0.0.72.tar` & `cellworld_game-0.0.73.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 01:42:08.710399 cellworld_game-0.0.72/
--rw-rw-rw-   0        0        0       36 2024-05-01 01:42:07.000000 cellworld_game-0.0.72/MANIFEST.in
--rw-rw-rw-   0        0        0      474 2024-05-01 01:42:08.709385 cellworld_game-0.0.72/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-05-01 01:42:07.000000 cellworld_game-0.0.72/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 01:42:08.677309 cellworld_game-0.0.72/cellworld_game/
--rw-rw-rw-   0        0        0       32 2024-05-01 01:42:07.000000 cellworld_game-0.0.72/cellworld_game/README.md
--rw-rw-rw-   0        0        0      435 2024-04-30 14:54:26.000000 cellworld_game-0.0.72/cellworld_game/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 01:42:08.701208 cellworld_game-0.0.72/cellworld_game/__pycache__/
--rw-rw-rw-   0        0        0      592 2024-04-06 23:12:27.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      782 2024-04-30 15:03:00.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     4004 2024-04-09 15:04:25.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/agent.cpython-310.pyc
--rw-rw-rw-   0        0        0    10222 2024-04-30 15:03:01.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/agent.cpython-312.pyc
--rw-rw-rw-   0        0        0     2936 2024-04-09 15:05:01.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/cellworld_loader.cpython-310.pyc
--rw-rw-rw-   0        0        0     5043 2024-04-30 15:03:01.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/cellworld_loader.cpython-312.pyc
--rw-rw-rw-   0        0        0     2949 2024-04-09 15:04:26.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/environment.cpython-310.pyc
--rw-rw-rw-   0        0        0     8962 2024-04-15 19:38:53.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/environment.cpython-312.pyc
--rw-rw-rw-   0        0        0      778 2024-04-09 15:04:25.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/geometry.cpython-310.pyc
--rw-rw-rw-   0        0        0     1424 2024-04-06 23:24:51.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/geometry.cpython-312.pyc
--rw-rw-rw-   0        0        0     4416 2024-04-09 15:04:25.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/model.cpython-310.pyc
--rw-rw-rw-   0        0        0    12063 2024-04-30 19:57:46.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/model.cpython-312.pyc
--rw-rw-rw-   0        0        0     3674 2024-04-09 15:04:25.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/mouse.cpython-310.pyc
--rw-rw-rw-   0        0        0     2208 2024-04-30 15:03:01.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/mouse.cpython-312.pyc
--rw-rw-rw-   0        0        0     1752 2024-04-09 15:04:25.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/navigation.cpython-310.pyc
--rw-rw-rw-   0        0        0     2598 2024-04-30 15:03:01.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/navigation.cpython-312.pyc
--rw-rw-rw-   0        0        0     2273 2024-04-09 15:04:25.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/navigation_agent.cpython-310.pyc
--rw-rw-rw-   0        0        0     6038 2024-04-30 20:00:08.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/navigation_agent.cpython-312.pyc
--rw-rw-rw-   0        0        0     3756 2024-04-09 15:04:25.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/ray_tracing.cpython-310.pyc
--rw-rw-rw-   0        0        0     6071 2024-04-30 15:03:01.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/ray_tracing.cpython-312.pyc
--rw-rw-rw-   0        0        0      528 2024-04-09 15:04:25.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/resources.cpython-310.pyc
--rw-rw-rw-   0        0        0      870 2024-04-30 15:03:01.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/resources.cpython-312.pyc
--rw-rw-rw-   0        0        0     1245 2024-04-15 14:35:46.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/reward.cpython-312.pyc
--rw-rw-rw-   0        0        0     2029 2024-04-09 15:04:25.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/robot.cpython-310.pyc
--rw-rw-rw-   0        0        0     2743 2024-04-30 15:03:01.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/robot.cpython-312.pyc
--rw-rw-rw-   0        0        0     6229 2024-04-09 15:04:25.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/util.cpython-310.pyc
--rw-rw-rw-   0        0        0     9945 2024-04-30 15:03:01.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/util.cpython-312.pyc
--rw-rw-rw-   0        0        0     4717 2024-04-06 23:12:27.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/view.cpython-310.pyc
--rw-rw-rw-   0        0        0     9850 2024-04-30 15:03:00.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/view.cpython-312.pyc
--rw-rw-rw-   0        0        0     6299 2024-04-09 15:04:25.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/visibility.cpython-310.pyc
--rw-rw-rw-   0        0        0    10037 2024-04-15 14:35:44.000000 cellworld_game-0.0.72/cellworld_game/__pycache__/visibility.cpython-312.pyc
--rw-rw-rw-   0        0        0     6116 2024-04-30 14:54:26.000000 cellworld_game-0.0.72/cellworld_game/agent.py
--rw-rw-rw-   0        0        0     3652 2024-04-30 14:54:26.000000 cellworld_game-0.0.72/cellworld_game/cellworld_loader.py
-drwxrwxrwx   0        0        0        0 2024-05-01 01:42:08.702208 cellworld_game-0.0.72/cellworld_game/files/
--rw-rw-rw-   0        0        0     8477 2024-04-24 19:46:43.000000 cellworld_game-0.0.72/cellworld_game/files/agent.png
--rw-rw-rw-   0        0        0    41740 2024-04-24 19:46:43.000000 cellworld_game-0.0.72/cellworld_game/files/predator.png
--rw-rw-rw-   0        0        0    47356 2024-04-24 19:46:43.000000 cellworld_game-0.0.72/cellworld_game/files/prey.png
--rw-rw-rw-   0        0        0      431 2024-04-06 23:24:02.000000 cellworld_game-0.0.72/cellworld_game/geometry.py
--rw-rw-rw-   0        0        0     1636 2024-05-01 01:42:07.000000 cellworld_game-0.0.72/cellworld_game/license.txt
--rw-rw-rw-   0        0        0     8907 2024-04-30 19:57:44.000000 cellworld_game-0.0.72/cellworld_game/model.py
--rw-rw-rw-   0        0        0     1133 2024-04-24 19:46:43.000000 cellworld_game-0.0.72/cellworld_game/mouse.py
--rw-rw-rw-   0        0        0     1672 2024-04-24 19:46:43.000000 cellworld_game-0.0.72/cellworld_game/navigation.py
--rw-rw-rw-   0        0        0     4550 2024-04-30 20:00:00.000000 cellworld_game-0.0.72/cellworld_game/navigation_agent.py
--rw-rw-rw-   0        0        0     4876 2024-04-24 19:46:43.000000 cellworld_game-0.0.72/cellworld_game/ray_tracing.py
--rw-rw-rw-   0        0        0      211 2024-04-24 19:46:43.000000 cellworld_game-0.0.72/cellworld_game/resources.py
--rw-rw-rw-   0        0        0     1501 2024-04-30 14:54:26.000000 cellworld_game-0.0.72/cellworld_game/robot.py
--rw-rw-rw-   0        0        0      183 2024-05-01 01:42:07.000000 cellworld_game-0.0.72/cellworld_game/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-01 01:42:08.705869 cellworld_game-0.0.72/cellworld_game/tasks/
--rw-rw-rw-   0        0        0       89 2024-04-30 14:54:26.000000 cellworld_game-0.0.72/cellworld_game/tasks/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 01:42:08.708869 cellworld_game-0.0.72/cellworld_game/tasks/__pycache__/
--rw-rw-rw-   0        0        0      280 2024-04-30 15:03:03.000000 cellworld_game-0.0.72/cellworld_game/tasks/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     6974 2024-04-30 15:03:03.000000 cellworld_game-0.0.72/cellworld_game/tasks/__pycache__/botevade.cpython-312.pyc
--rw-rw-rw-   0        0        0    10654 2024-04-30 15:03:03.000000 cellworld_game-0.0.72/cellworld_game/tasks/__pycache__/dualevade.cpython-312.pyc
--rw-rw-rw-   0        0        0     9271 2024-04-30 15:03:03.000000 cellworld_game-0.0.72/cellworld_game/tasks/__pycache__/oasis.cpython-312.pyc
--rw-rw-rw-   0        0        0     5289 2024-05-01 01:15:50.000000 cellworld_game-0.0.72/cellworld_game/tasks/botevade.py
--rw-rw-rw-   0        0        0     7811 2024-04-30 14:54:26.000000 cellworld_game-0.0.72/cellworld_game/tasks/dualevade.py
--rw-rw-rw-   0        0        0     7256 2024-04-30 14:54:26.000000 cellworld_game-0.0.72/cellworld_game/tasks/oasis.py
--rw-rw-rw-   0        0        0     7672 2024-04-24 19:46:43.000000 cellworld_game-0.0.72/cellworld_game/util.py
--rw-rw-rw-   0        0        0     6495 2024-04-30 14:54:26.000000 cellworld_game-0.0.72/cellworld_game/view.py
--rw-rw-rw-   0        0        0     9289 2024-04-15 14:32:56.000000 cellworld_game-0.0.72/cellworld_game/visibility.py
-drwxrwxrwx   0        0        0        0 2024-05-01 01:42:08.709385 cellworld_game-0.0.72/cellworld_game.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-01 01:42:08.000000 cellworld_game-0.0.72/cellworld_game.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2794 2024-05-01 01:42:08.000000 cellworld_game-0.0.72/cellworld_game.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 01:42:08.000000 cellworld_game-0.0.72/cellworld_game.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-01 01:42:08.000000 cellworld_game-0.0.72/cellworld_game.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2024-05-01 01:42:08.000000 cellworld_game-0.0.72/cellworld_game.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-01 01:42:08.000000 cellworld_game-0.0.72/cellworld_game.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 01:42:08.710399 cellworld_game-0.0.72/setup.cfg
--rw-rw-rw-   0        0        0      667 2024-05-01 01:42:07.000000 cellworld_game-0.0.72/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 03:16:52.320936 cellworld_game-0.0.73/
+-rw-rw-rw-   0        0        0       36 2024-05-01 03:16:51.000000 cellworld_game-0.0.73/MANIFEST.in
+-rw-rw-rw-   0        0        0      474 2024-05-01 03:16:52.319937 cellworld_game-0.0.73/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2024-05-01 03:16:51.000000 cellworld_game-0.0.73/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 03:16:52.288738 cellworld_game-0.0.73/cellworld_game/
+-rw-rw-rw-   0        0        0       32 2024-05-01 03:16:51.000000 cellworld_game-0.0.73/cellworld_game/README.md
+-rw-rw-rw-   0        0        0      435 2024-04-30 14:54:26.000000 cellworld_game-0.0.73/cellworld_game/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 03:16:52.311929 cellworld_game-0.0.73/cellworld_game/__pycache__/
+-rw-rw-rw-   0        0        0      592 2024-04-06 23:12:27.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      782 2024-04-30 15:03:00.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4004 2024-04-09 15:04:25.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/agent.cpython-310.pyc
+-rw-rw-rw-   0        0        0    10222 2024-04-30 15:03:01.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/agent.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2936 2024-04-09 15:05:01.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/cellworld_loader.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5043 2024-04-30 15:03:01.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/cellworld_loader.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2949 2024-04-09 15:04:26.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/environment.cpython-310.pyc
+-rw-rw-rw-   0        0        0     8962 2024-04-15 19:38:53.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/environment.cpython-312.pyc
+-rw-rw-rw-   0        0        0      778 2024-04-09 15:04:25.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/geometry.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1424 2024-04-06 23:24:51.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/geometry.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4416 2024-04-09 15:04:25.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/model.cpython-310.pyc
+-rw-rw-rw-   0        0        0    12063 2024-04-30 19:57:46.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/model.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3674 2024-04-09 15:04:25.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/mouse.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2208 2024-04-30 15:03:01.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/mouse.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1752 2024-04-09 15:04:25.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/navigation.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2598 2024-04-30 15:03:01.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/navigation.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2273 2024-04-09 15:04:25.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/navigation_agent.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6038 2024-04-30 20:00:08.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/navigation_agent.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3756 2024-04-09 15:04:25.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/ray_tracing.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6071 2024-04-30 15:03:01.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/ray_tracing.cpython-312.pyc
+-rw-rw-rw-   0        0        0      528 2024-04-09 15:04:25.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/resources.cpython-310.pyc
+-rw-rw-rw-   0        0        0      870 2024-04-30 15:03:01.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/resources.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1245 2024-04-15 14:35:46.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/reward.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2029 2024-04-09 15:04:25.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/robot.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2743 2024-04-30 15:03:01.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/robot.cpython-312.pyc
+-rw-rw-rw-   0        0        0     6229 2024-04-09 15:04:25.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/util.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9945 2024-04-30 15:03:01.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/util.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4717 2024-04-06 23:12:27.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/view.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9850 2024-04-30 15:03:00.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/view.cpython-312.pyc
+-rw-rw-rw-   0        0        0     6299 2024-04-09 15:04:25.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/visibility.cpython-310.pyc
+-rw-rw-rw-   0        0        0    10037 2024-04-15 14:35:44.000000 cellworld_game-0.0.73/cellworld_game/__pycache__/visibility.cpython-312.pyc
+-rw-rw-rw-   0        0        0     6116 2024-04-30 14:54:26.000000 cellworld_game-0.0.73/cellworld_game/agent.py
+-rw-rw-rw-   0        0        0     3652 2024-04-30 14:54:26.000000 cellworld_game-0.0.73/cellworld_game/cellworld_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-01 03:16:52.313933 cellworld_game-0.0.73/cellworld_game/files/
+-rw-rw-rw-   0        0        0     8477 2024-04-24 19:46:43.000000 cellworld_game-0.0.73/cellworld_game/files/agent.png
+-rw-rw-rw-   0        0        0    41740 2024-04-24 19:46:43.000000 cellworld_game-0.0.73/cellworld_game/files/predator.png
+-rw-rw-rw-   0        0        0    47356 2024-04-24 19:46:43.000000 cellworld_game-0.0.73/cellworld_game/files/prey.png
+-rw-rw-rw-   0        0        0      431 2024-04-06 23:24:02.000000 cellworld_game-0.0.73/cellworld_game/geometry.py
+-rw-rw-rw-   0        0        0     1636 2024-05-01 03:16:51.000000 cellworld_game-0.0.73/cellworld_game/license.txt
+-rw-rw-rw-   0        0        0     8907 2024-04-30 19:57:44.000000 cellworld_game-0.0.73/cellworld_game/model.py
+-rw-rw-rw-   0        0        0     1133 2024-04-24 19:46:43.000000 cellworld_game-0.0.73/cellworld_game/mouse.py
+-rw-rw-rw-   0        0        0     1672 2024-04-24 19:46:43.000000 cellworld_game-0.0.73/cellworld_game/navigation.py
+-rw-rw-rw-   0        0        0     4550 2024-04-30 20:00:00.000000 cellworld_game-0.0.73/cellworld_game/navigation_agent.py
+-rw-rw-rw-   0        0        0     4876 2024-04-24 19:46:43.000000 cellworld_game-0.0.73/cellworld_game/ray_tracing.py
+-rw-rw-rw-   0        0        0      211 2024-04-24 19:46:43.000000 cellworld_game-0.0.73/cellworld_game/resources.py
+-rw-rw-rw-   0        0        0     1501 2024-04-30 14:54:26.000000 cellworld_game-0.0.73/cellworld_game/robot.py
+-rw-rw-rw-   0        0        0      183 2024-05-01 03:16:51.000000 cellworld_game-0.0.73/cellworld_game/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-01 03:16:52.316937 cellworld_game-0.0.73/cellworld_game/tasks/
+-rw-rw-rw-   0        0        0       89 2024-04-30 14:54:26.000000 cellworld_game-0.0.73/cellworld_game/tasks/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 03:16:52.318936 cellworld_game-0.0.73/cellworld_game/tasks/__pycache__/
+-rw-rw-rw-   0        0        0      280 2024-04-30 15:03:03.000000 cellworld_game-0.0.73/cellworld_game/tasks/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     6974 2024-04-30 15:03:03.000000 cellworld_game-0.0.73/cellworld_game/tasks/__pycache__/botevade.cpython-312.pyc
+-rw-rw-rw-   0        0        0    10654 2024-04-30 15:03:03.000000 cellworld_game-0.0.73/cellworld_game/tasks/__pycache__/dualevade.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9271 2024-04-30 15:03:03.000000 cellworld_game-0.0.73/cellworld_game/tasks/__pycache__/oasis.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5289 2024-05-01 01:15:50.000000 cellworld_game-0.0.73/cellworld_game/tasks/botevade.py
+-rw-rw-rw-   0        0        0     7815 2024-05-01 03:16:23.000000 cellworld_game-0.0.73/cellworld_game/tasks/dualevade.py
+-rw-rw-rw-   0        0        0     7256 2024-04-30 14:54:26.000000 cellworld_game-0.0.73/cellworld_game/tasks/oasis.py
+-rw-rw-rw-   0        0        0     7672 2024-04-24 19:46:43.000000 cellworld_game-0.0.73/cellworld_game/util.py
+-rw-rw-rw-   0        0        0     6495 2024-04-30 14:54:26.000000 cellworld_game-0.0.73/cellworld_game/view.py
+-rw-rw-rw-   0        0        0     9289 2024-04-15 14:32:56.000000 cellworld_game-0.0.73/cellworld_game/visibility.py
+drwxrwxrwx   0        0        0        0 2024-05-01 03:16:52.319937 cellworld_game-0.0.73/cellworld_game.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-01 03:16:52.000000 cellworld_game-0.0.73/cellworld_game.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2794 2024-05-01 03:16:52.000000 cellworld_game-0.0.73/cellworld_game.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 03:16:52.000000 cellworld_game-0.0.73/cellworld_game.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-01 03:16:52.000000 cellworld_game-0.0.73/cellworld_game.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2024-05-01 03:16:52.000000 cellworld_game-0.0.73/cellworld_game.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-01 03:16:52.000000 cellworld_game-0.0.73/cellworld_game.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 03:16:52.320936 cellworld_game-0.0.73/setup.cfg
+-rw-rw-rw-   0        0        0      667 2024-05-01 03:16:51.000000 cellworld_game-0.0.73/setup.py
```

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/__init__.cpython-310.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/__init__.cpython-312.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/agent.cpython-310.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/agent.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/agent.cpython-312.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/agent.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/cellworld_loader.cpython-310.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/cellworld_loader.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/cellworld_loader.cpython-312.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/cellworld_loader.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/environment.cpython-310.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/environment.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/environment.cpython-312.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/environment.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/geometry.cpython-310.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/geometry.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/geometry.cpython-312.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/geometry.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/model.cpython-310.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/model.cpython-312.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/model.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/mouse.cpython-310.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/mouse.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/mouse.cpython-312.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/mouse.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/navigation.cpython-310.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/navigation.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/navigation.cpython-312.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/navigation.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/navigation_agent.cpython-310.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/navigation_agent.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/navigation_agent.cpython-312.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/navigation_agent.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/ray_tracing.cpython-310.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/ray_tracing.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/ray_tracing.cpython-312.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/ray_tracing.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/resources.cpython-310.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/resources.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/resources.cpython-312.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/resources.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/reward.cpython-312.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/reward.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/robot.cpython-310.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/robot.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/robot.cpython-312.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/robot.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/util.cpython-310.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/util.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/util.cpython-312.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/util.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/view.cpython-310.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/view.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/view.cpython-312.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/view.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/visibility.cpython-310.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/visibility.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/__pycache__/visibility.cpython-312.pyc` & `cellworld_game-0.0.73/cellworld_game/__pycache__/visibility.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/agent.py` & `cellworld_game-0.0.73/cellworld_game/agent.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/cellworld_loader.py` & `cellworld_game-0.0.73/cellworld_game/cellworld_loader.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/files/agent.png` & `cellworld_game-0.0.73/cellworld_game/files/agent.png`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/files/predator.png` & `cellworld_game-0.0.73/cellworld_game/files/predator.png`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/files/prey.png` & `cellworld_game-0.0.73/cellworld_game/files/prey.png`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/license.txt` & `cellworld_game-0.0.73/cellworld_game/license.txt`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/model.py` & `cellworld_game-0.0.73/cellworld_game/model.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/mouse.py` & `cellworld_game-0.0.73/cellworld_game/mouse.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/navigation.py` & `cellworld_game-0.0.73/cellworld_game/navigation.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/navigation_agent.py` & `cellworld_game-0.0.73/cellworld_game/navigation_agent.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/ray_tracing.py` & `cellworld_game-0.0.73/cellworld_game/ray_tracing.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/robot.py` & `cellworld_game-0.0.73/cellworld_game/robot.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/tasks/__pycache__/botevade.cpython-312.pyc` & `cellworld_game-0.0.73/cellworld_game/tasks/__pycache__/botevade.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/tasks/__pycache__/dualevade.cpython-312.pyc` & `cellworld_game-0.0.73/cellworld_game/tasks/__pycache__/dualevade.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/tasks/__pycache__/oasis.cpython-312.pyc` & `cellworld_game-0.0.73/cellworld_game/tasks/__pycache__/oasis.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/tasks/botevade.py` & `cellworld_game-0.0.73/cellworld_game/tasks/botevade.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/tasks/dualevade.py` & `cellworld_game-0.0.73/cellworld_game/tasks/dualevade.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
                 if closest_visible_prey_location:
                     if self.prey_data_2.predator_prey_distance <= self.prey_data_1.predator_prey_distance:
                         closest_visible_prey_location = self.prey_2.state.location
                 else:
                     closest_visible_prey_location = self.prey_2.state.location
 
             if closest_visible_prey_location:
-                self.predator.set_destination(self.prey_2.state.location)
+                self.predator.set_destination(closest_visible_prey_location)
 
             if not self.predator.path:
                 self.predator.set_destination(random.choice(self.loader.open_locations))
 
         if delta_t < self.puff_cool_down:
             self.puff_cool_down -= delta_t
         else:
@@ -172,8 +172,8 @@
         self.__update_state__()
 
     def step(self) -> float:
         delta_t = Model.step(self)
         if self.render:
             self.view.draw()
         self.__update_state__(delta_t=delta_t)
-        return delta_t
+        return delta_t
```

### Comparing `cellworld_game-0.0.72/cellworld_game/tasks/oasis.py` & `cellworld_game-0.0.73/cellworld_game/tasks/oasis.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/util.py` & `cellworld_game-0.0.73/cellworld_game/util.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/view.py` & `cellworld_game-0.0.73/cellworld_game/view.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game/visibility.py` & `cellworld_game-0.0.73/cellworld_game/visibility.py`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/cellworld_game.egg-info/SOURCES.txt` & `cellworld_game-0.0.73/cellworld_game.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.72/setup.py` & `cellworld_game-0.0.73/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,9 +7,9 @@
       author_email='germanespinosa@gmail.com',
       long_description=open('./cellworld_game/README.md').read() + '\n---\n<small>Package created with Easy-pack</small>\n',
       long_description_content_type='text/markdown',
       packages=['cellworld_game'],
       install_requires=['cellworld', 'pygame', 'shapely'],
       license='MIT',
       include_package_data=True,
-      version='0.0.72',
+      version='0.0.73',
       zip_safe=False)
```


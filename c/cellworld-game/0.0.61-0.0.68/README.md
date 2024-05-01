# Comparing `tmp/cellworld_game-0.0.61.tar.gz` & `tmp/cellworld_game-0.0.68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellworld_game-0.0.61.tar", last modified: Mon Apr 29 16:23:50 2024, max compression
+gzip compressed data, was "cellworld_game-0.0.68.tar", last modified: Tue Apr 30 15:01:34 2024, max compression
```

## Comparing `cellworld_game-0.0.61.tar` & `cellworld_game-0.0.68.tar`

### file list

```diff
@@ -1,60 +1,72 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 16:23:50.730209 cellworld_game-0.0.61/
--rw-rw-rw-   0        0        0       36 2024-04-29 16:23:49.000000 cellworld_game-0.0.61/MANIFEST.in
--rw-rw-rw-   0        0        0      474 2024-04-29 16:23:50.729208 cellworld_game-0.0.61/PKG-INFO
--rw-rw-rw-   0        0        0       33 2024-04-29 16:23:49.000000 cellworld_game-0.0.61/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 16:23:50.690217 cellworld_game-0.0.61/cellworld_game/
--rw-rw-rw-   0        0        0       33 2024-04-29 16:23:49.000000 cellworld_game-0.0.61/cellworld_game/README.md
--rw-rw-rw-   0        0        0      447 2024-04-26 16:52:38.000000 cellworld_game-0.0.61/cellworld_game/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:23:50.713208 cellworld_game-0.0.61/cellworld_game/__pycache__/
--rw-rw-rw-   0        0        0      782 2024-04-26 16:52:40.000000 cellworld_game-0.0.61/cellworld_game/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0    10222 2024-04-26 17:03:42.000000 cellworld_game-0.0.61/cellworld_game/__pycache__/agent.cpython-312.pyc
--rw-rw-rw-   0        0        0     5043 2024-04-26 16:48:26.000000 cellworld_game-0.0.61/cellworld_game/__pycache__/cellworld_loader.cpython-312.pyc
--rw-rw-rw-   0        0        0     1424 2024-04-10 15:31:18.000000 cellworld_game-0.0.61/cellworld_game/__pycache__/geometry.cpython-312.pyc
--rw-rw-rw-   0        0        0     9662 2024-04-25 18:38:43.000000 cellworld_game-0.0.61/cellworld_game/__pycache__/model.cpython-312.pyc
--rw-rw-rw-   0        0        0     2208 2024-04-23 16:26:46.000000 cellworld_game-0.0.61/cellworld_game/__pycache__/mouse.cpython-312.pyc
--rw-rw-rw-   0        0        0     2598 2024-04-21 15:32:53.000000 cellworld_game-0.0.61/cellworld_game/__pycache__/navigation.cpython-312.pyc
--rw-rw-rw-   0        0        0     5807 2024-04-26 17:03:42.000000 cellworld_game-0.0.61/cellworld_game/__pycache__/navigation_agent.cpython-312.pyc
--rw-rw-rw-   0        0        0     6071 2024-04-21 15:32:53.000000 cellworld_game-0.0.61/cellworld_game/__pycache__/ray_tracing.cpython-312.pyc
--rw-rw-rw-   0        0        0      870 2024-04-21 15:16:32.000000 cellworld_game-0.0.61/cellworld_game/__pycache__/resources.cpython-312.pyc
--rw-rw-rw-   0        0        0     2743 2024-04-26 16:48:26.000000 cellworld_game-0.0.61/cellworld_game/__pycache__/robot.cpython-312.pyc
--rw-rw-rw-   0        0        0     9945 2024-04-23 16:16:30.000000 cellworld_game-0.0.61/cellworld_game/__pycache__/util.cpython-312.pyc
--rw-rw-rw-   0        0        0     9683 2024-04-26 17:03:42.000000 cellworld_game-0.0.61/cellworld_game/__pycache__/view.cpython-312.pyc
--rw-rw-rw-   0        0        0    10037 2024-04-11 19:37:36.000000 cellworld_game-0.0.61/cellworld_game/__pycache__/visibility.cpython-312.pyc
--rw-rw-rw-   0        0        0     6294 2024-04-26 17:03:41.000000 cellworld_game-0.0.61/cellworld_game/agent.py
--rw-rw-rw-   0        0        0     3712 2024-04-25 23:24:36.000000 cellworld_game-0.0.61/cellworld_game/cellworld_loader.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:23:50.717209 cellworld_game-0.0.61/cellworld_game/files/
--rw-rw-rw-   0        0        0     8477 2024-03-30 14:47:10.000000 cellworld_game-0.0.61/cellworld_game/files/agent.png
--rw-rw-rw-   0        0        0    41740 2024-04-02 20:09:30.000000 cellworld_game-0.0.61/cellworld_game/files/predator.png
--rw-rw-rw-   0        0        0    47356 2024-04-02 20:07:49.000000 cellworld_game-0.0.61/cellworld_game/files/prey.png
--rw-rw-rw-   0        0        0      431 2024-04-10 15:24:24.000000 cellworld_game-0.0.61/cellworld_game/geometry.py
--rw-rw-rw-   0        0        0     1636 2024-04-29 16:23:49.000000 cellworld_game-0.0.61/cellworld_game/license.txt
--rw-rw-rw-   0        0        0     8159 2024-04-29 16:23:49.000000 cellworld_game-0.0.61/cellworld_game/model.py
--rw-rw-rw-   0        0        0     1167 2024-04-23 16:26:41.000000 cellworld_game-0.0.61/cellworld_game/mouse.py
--rw-rw-rw-   0        0        0     1717 2024-04-21 15:19:56.000000 cellworld_game-0.0.61/cellworld_game/navigation.py
--rw-rw-rw-   0        0        0     4455 2024-04-26 17:03:41.000000 cellworld_game-0.0.61/cellworld_game/navigation_agent.py
--rw-rw-rw-   0        0        0     4973 2024-04-21 15:20:54.000000 cellworld_game-0.0.61/cellworld_game/ray_tracing.py
--rw-rw-rw-   0        0        0      220 2024-04-19 14:17:58.000000 cellworld_game-0.0.61/cellworld_game/resources.py
--rw-rw-rw-   0        0        0     1542 2024-04-26 16:24:32.000000 cellworld_game-0.0.61/cellworld_game/robot.py
--rw-rw-rw-   0        0        0      183 2024-04-29 16:23:49.000000 cellworld_game-0.0.61/cellworld_game/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-29 16:23:50.721208 cellworld_game-0.0.61/cellworld_game/tasks/
--rw-rw-rw-   0        0        0       92 2024-04-26 16:46:54.000000 cellworld_game-0.0.61/cellworld_game/tasks/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:23:50.726208 cellworld_game-0.0.61/cellworld_game/tasks/__pycache__/
--rw-rw-rw-   0        0        0      280 2024-04-26 16:48:27.000000 cellworld_game-0.0.61/cellworld_game/tasks/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     6831 2024-04-26 16:50:52.000000 cellworld_game-0.0.61/cellworld_game/tasks/__pycache__/botevade.cpython-312.pyc
--rw-rw-rw-   0        0        0     9943 2024-04-26 17:34:24.000000 cellworld_game-0.0.61/cellworld_game/tasks/__pycache__/dualevade.cpython-312.pyc
--rw-rw-rw-   0        0        0     9261 2024-04-26 16:51:24.000000 cellworld_game-0.0.61/cellworld_game/tasks/__pycache__/oasis.cpython-312.pyc
--rw-rw-rw-   0        0        0     5436 2024-04-26 17:38:02.000000 cellworld_game-0.0.61/cellworld_game/tasks/botevade.py
--rw-rw-rw-   0        0        0     8039 2024-04-29 15:41:10.000000 cellworld_game-0.0.61/cellworld_game/tasks/dualevade.py
--rw-rw-rw-   0        0        0     7476 2024-04-26 16:51:20.000000 cellworld_game-0.0.61/cellworld_game/tasks/oasis.py
--rw-rw-rw-   0        0        0     7912 2024-04-23 16:14:29.000000 cellworld_game-0.0.61/cellworld_game/util.py
--rw-rw-rw-   0        0        0     6637 2024-04-26 19:48:33.000000 cellworld_game-0.0.61/cellworld_game/view.py
--rw-rw-rw-   0        0        0     9497 2024-04-11 19:37:32.000000 cellworld_game-0.0.61/cellworld_game/visibility.py
-drwxrwxrwx   0        0        0        0 2024-04-29 16:23:50.728208 cellworld_game-0.0.61/cellworld_game.egg-info/
--rw-rw-rw-   0        0        0      474 2024-04-29 16:23:50.000000 cellworld_game-0.0.61/cellworld_game.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1902 2024-04-29 16:23:50.000000 cellworld_game-0.0.61/cellworld_game.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 16:23:50.000000 cellworld_game-0.0.61/cellworld_game.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-29 16:23:50.000000 cellworld_game-0.0.61/cellworld_game.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2024-04-29 16:23:50.000000 cellworld_game-0.0.61/cellworld_game.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-29 16:23:50.000000 cellworld_game-0.0.61/cellworld_game.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 16:23:50.730209 cellworld_game-0.0.61/setup.cfg
--rw-rw-rw-   0        0        0      667 2024-04-29 16:23:49.000000 cellworld_game-0.0.61/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 15:01:34.548412 cellworld_game-0.0.68/
+-rw-rw-rw-   0        0        0       36 2024-04-30 15:01:33.000000 cellworld_game-0.0.68/MANIFEST.in
+-rw-rw-rw-   0        0        0      474 2024-04-30 15:01:34.546957 cellworld_game-0.0.68/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2024-04-30 15:01:33.000000 cellworld_game-0.0.68/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 15:01:34.517938 cellworld_game-0.0.68/cellworld_game/
+-rw-rw-rw-   0        0        0       32 2024-04-30 15:01:33.000000 cellworld_game-0.0.68/cellworld_game/README.md
+-rw-rw-rw-   0        0        0      435 2024-04-30 14:54:26.000000 cellworld_game-0.0.68/cellworld_game/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 15:01:34.541956 cellworld_game-0.0.68/cellworld_game/__pycache__/
+-rw-rw-rw-   0        0        0      592 2024-04-06 23:12:27.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      645 2024-04-15 14:35:43.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4004 2024-04-09 15:04:25.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/agent.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5962 2024-04-07 18:05:49.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/agent.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2936 2024-04-09 15:05:01.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/cellworld_loader.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4974 2024-04-07 17:06:18.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/cellworld_loader.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2949 2024-04-09 15:04:26.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/environment.cpython-310.pyc
+-rw-rw-rw-   0        0        0     8962 2024-04-15 19:38:53.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/environment.cpython-312.pyc
+-rw-rw-rw-   0        0        0      778 2024-04-09 15:04:25.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/geometry.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1424 2024-04-06 23:24:51.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/geometry.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4416 2024-04-09 15:04:25.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/model.cpython-310.pyc
+-rw-rw-rw-   0        0        0     8490 2024-04-15 14:35:44.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/model.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3674 2024-04-09 15:04:25.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/mouse.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5862 2024-04-15 14:35:44.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/mouse.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1752 2024-04-09 15:04:25.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/navigation.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2666 2024-04-09 19:05:22.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/navigation.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2273 2024-04-09 15:04:25.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/navigation_agent.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3646 2024-04-09 19:00:04.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/navigation_agent.cpython-312.pyc
+-rw-rw-rw-   0        0        0     3756 2024-04-09 15:04:25.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/ray_tracing.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6071 2024-04-06 17:31:40.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/ray_tracing.cpython-312.pyc
+-rw-rw-rw-   0        0        0      528 2024-04-09 15:04:25.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/resources.cpython-310.pyc
+-rw-rw-rw-   0        0        0      650 2024-04-06 17:31:40.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/resources.cpython-312.pyc
+-rw-rw-rw-   0        0        0     1245 2024-04-15 14:35:46.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/reward.cpython-312.pyc
+-rw-rw-rw-   0        0        0     2029 2024-04-09 15:04:25.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/robot.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3312 2024-04-09 19:01:02.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/robot.cpython-312.pyc
+-rw-rw-rw-   0        0        0     6229 2024-04-09 15:04:25.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/util.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9945 2024-04-06 23:38:40.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/util.cpython-312.pyc
+-rw-rw-rw-   0        0        0     4717 2024-04-06 23:12:27.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/view.cpython-310.pyc
+-rw-rw-rw-   0        0        0    10660 2024-04-09 19:27:51.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/view.cpython-312.pyc
+-rw-rw-rw-   0        0        0     6299 2024-04-09 15:04:25.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/visibility.cpython-310.pyc
+-rw-rw-rw-   0        0        0    10037 2024-04-15 14:35:44.000000 cellworld_game-0.0.68/cellworld_game/__pycache__/visibility.cpython-312.pyc
+-rw-rw-rw-   0        0        0     6116 2024-04-30 14:54:26.000000 cellworld_game-0.0.68/cellworld_game/agent.py
+-rw-rw-rw-   0        0        0     3652 2024-04-30 14:54:26.000000 cellworld_game-0.0.68/cellworld_game/cellworld_loader.py
+drwxrwxrwx   0        0        0        0 2024-04-30 15:01:34.543956 cellworld_game-0.0.68/cellworld_game/files/
+-rw-rw-rw-   0        0        0     8477 2024-04-24 19:46:43.000000 cellworld_game-0.0.68/cellworld_game/files/agent.png
+-rw-rw-rw-   0        0        0    41740 2024-04-24 19:46:43.000000 cellworld_game-0.0.68/cellworld_game/files/predator.png
+-rw-rw-rw-   0        0        0    47356 2024-04-24 19:46:43.000000 cellworld_game-0.0.68/cellworld_game/files/prey.png
+-rw-rw-rw-   0        0        0      431 2024-04-06 23:24:02.000000 cellworld_game-0.0.68/cellworld_game/geometry.py
+-rw-rw-rw-   0        0        0     1636 2024-04-30 15:01:33.000000 cellworld_game-0.0.68/cellworld_game/license.txt
+-rw-rw-rw-   0        0        0     8334 2024-04-30 14:54:26.000000 cellworld_game-0.0.68/cellworld_game/model.py
+-rw-rw-rw-   0        0        0     1133 2024-04-24 19:46:43.000000 cellworld_game-0.0.68/cellworld_game/mouse.py
+-rw-rw-rw-   0        0        0     1672 2024-04-24 19:46:43.000000 cellworld_game-0.0.68/cellworld_game/navigation.py
+-rw-rw-rw-   0        0        0     4342 2024-04-30 14:54:26.000000 cellworld_game-0.0.68/cellworld_game/navigation_agent.py
+-rw-rw-rw-   0        0        0     4876 2024-04-24 19:46:43.000000 cellworld_game-0.0.68/cellworld_game/ray_tracing.py
+-rw-rw-rw-   0        0        0      211 2024-04-24 19:46:43.000000 cellworld_game-0.0.68/cellworld_game/resources.py
+-rw-rw-rw-   0        0        0     1501 2024-04-30 14:54:26.000000 cellworld_game-0.0.68/cellworld_game/robot.py
+-rw-rw-rw-   0        0        0      183 2024-04-30 15:01:33.000000 cellworld_game-0.0.68/cellworld_game/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-30 15:01:34.545956 cellworld_game-0.0.68/cellworld_game/tasks/
+-rw-rw-rw-   0        0        0       89 2024-04-30 14:54:26.000000 cellworld_game-0.0.68/cellworld_game/tasks/__init__.py
+-rw-rw-rw-   0        0        0     5298 2024-04-30 14:54:26.000000 cellworld_game-0.0.68/cellworld_game/tasks/botevade.py
+-rw-rw-rw-   0        0        0     7811 2024-04-30 14:54:26.000000 cellworld_game-0.0.68/cellworld_game/tasks/dualevade.py
+-rw-rw-rw-   0        0        0     7256 2024-04-30 14:54:26.000000 cellworld_game-0.0.68/cellworld_game/tasks/oasis.py
+-rw-rw-rw-   0        0        0     7672 2024-04-24 19:46:43.000000 cellworld_game-0.0.68/cellworld_game/util.py
+-rw-rw-rw-   0        0        0     6495 2024-04-30 14:54:26.000000 cellworld_game-0.0.68/cellworld_game/view.py
+-rw-rw-rw-   0        0        0     9289 2024-04-15 14:32:56.000000 cellworld_game-0.0.68/cellworld_game/visibility.py
+drwxrwxrwx   0        0        0        0 2024-04-30 15:01:34.546957 cellworld_game-0.0.68/cellworld_game.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-04-30 15:01:34.000000 cellworld_game-0.0.68/cellworld_game.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2564 2024-04-30 15:01:34.000000 cellworld_game-0.0.68/cellworld_game.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 15:01:34.000000 cellworld_game-0.0.68/cellworld_game.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-30 15:01:34.000000 cellworld_game-0.0.68/cellworld_game.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2024-04-30 15:01:34.000000 cellworld_game-0.0.68/cellworld_game.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-30 15:01:34.000000 cellworld_game-0.0.68/cellworld_game.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 15:01:34.548412 cellworld_game-0.0.68/setup.cfg
+-rw-rw-rw-   0        0        0      667 2024-04-30 15:01:33.000000 cellworld_game-0.0.68/setup.py
```

### Comparing `cellworld_game-0.0.61/cellworld_game/__pycache__/__init__.cpython-312.pyc` & `cellworld_game-0.0.68/cellworld_game/__pycache__/__init__.cpython-312.pyc`

 * *Files 23% similar despite different names*

#### Python bytecode

```diff
@@ -1,22 +1,21 @@
 magic:    0xcb0d0d0a
-moddate:  0xd6db2b66 (Fri Apr 26 16:52:38 2024 UTC)
-files sz: 447
+moddate:  0x983a1d66 (Mon Apr 15 14:32:56 2024 UTC)
+files sz: 351
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a030100640064
       036c046d055a056d065a066d075a070100640064046c086d095a09010064
       0064056c0a6d0b5a0b0100640064066c0c6d0d5a0d0100640064076c0e6d
-      0f5a0f0100640064086c106d115a110100640064096c126d135a136d145a
-      146d155a1501006400640a6c166d175a1701006400640b6c186d195a1901
-      006400640c6c1a6d1b5a1b6d1c5a1c6d1d5a1d0100a60d
+      0f5a0f0100640064086c106d115a110100640064096c126d135a13010064
+      00640a6c146d155a1501006400640b6c166d175a170100a60c
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (1)
                  4 LOAD_CONST               1 (('View',))
                  6 IMPORT_NAME              0 (view)
                  8 IMPORT_FROM              1 (View)
                 10 STORE_NAME               1 (View)
@@ -72,65 +71,49 @@
                 96 LOAD_CONST               8 (('Navigation',))
                 98 IMPORT_NAME             16 (navigation)
                100 IMPORT_FROM             17 (Navigation)
                102 STORE_NAME              17 (Navigation)
                104 POP_TOP
    
      9         106 LOAD_CONST               0 (1)
-               108 LOAD_CONST               9 (('create_hexagon', 'distance', 'direction'))
+               108 LOAD_CONST               9 (('create_hexagon',))
                110 IMPORT_NAME             18 (util)
                112 IMPORT_FROM             19 (create_hexagon)
                114 STORE_NAME              19 (create_hexagon)
-               116 IMPORT_FROM             20 (distance)
-               118 STORE_NAME              20 (distance)
-               120 IMPORT_FROM             21 (direction)
-               122 STORE_NAME              21 (direction)
-               124 POP_TOP
-   
-    10         126 LOAD_CONST               0 (1)
-               128 LOAD_CONST              10 (('CellWorldLoader',))
-               130 IMPORT_NAME             22 (cellworld_loader)
-               132 IMPORT_FROM             23 (CellWorldLoader)
-               134 STORE_NAME              23 (CellWorldLoader)
-               136 POP_TOP
-   
-    11         138 LOAD_CONST               0 (1)
-               140 LOAD_CONST              11 (('Visibility',))
-               142 IMPORT_NAME             24 (visibility)
-               144 IMPORT_FROM             25 (Visibility)
-               146 STORE_NAME              25 (Visibility)
-               148 POP_TOP
-   
-    12         150 LOAD_CONST               0 (1)
-               152 LOAD_CONST              12 (('BotEvade', 'Oasis', 'DualEvade'))
-               154 IMPORT_NAME             26 (tasks)
-               156 IMPORT_FROM             27 (BotEvade)
-               158 STORE_NAME              27 (BotEvade)
-               160 IMPORT_FROM             28 (Oasis)
-               162 STORE_NAME              28 (Oasis)
-               164 IMPORT_FROM             29 (DualEvade)
-               166 STORE_NAME              29 (DualEvade)
-               168 POP_TOP
-               170 PRECALL                 13
+               116 POP_TOP
+   
+    10         118 LOAD_CONST               0 (1)
+               120 LOAD_CONST              10 (('Environment',))
+               122 IMPORT_NAME             20 (environment)
+               124 IMPORT_FROM             21 (Environment)
+               126 STORE_NAME              21 (Environment)
+               128 POP_TOP
+   
+    11         130 LOAD_CONST               0 (1)
+               132 LOAD_CONST              11 (('Reward',))
+               134 IMPORT_NAME             22 (reward)
+               136 IMPORT_FROM             23 (Reward)
+               138 STORE_NAME              23 (Reward)
+               140 POP_TOP
+               142 PRECALL                 12
    consts
       1
       ('View',)
       ('Model',)
       ('Agent', 'AgentDynamics', 'AgentState')
       ('Resources',)
       ('Robot',)
       ('Mouse',)
       ('RayTracing',)
       ('Navigation',)
-      ('create_hexagon', 'distance', 'direction')
-      ('CellWorldLoader',)
-      ('Visibility',)
-      ('BotEvade', 'Oasis', 'DualEvade')
+      ('create_hexagon',)
+      ('Environment',)
+      ('Reward',)
       None
-   names      ('view', 'View', 'model', 'Model', 'agent', 'Agent', 'AgentDynamics', 'AgentState', 'resources', 'Resources', 'robot', 'Robot', 'mouse', 'Mouse', 'ray_tracing', 'RayTracing', 'navigation', 'Navigation', 'util', 'create_hexagon', 'distance', 'direction', 'cellworld_loader', 'CellWorldLoader', 'visibility', 'Visibility', 'tasks', 'BotEvade', 'Oasis', 'DualEvade')
+   names      ('view', 'View', 'model', 'Model', 'agent', 'Agent', 'AgentDynamics', 'AgentState', 'resources', 'Resources', 'robot', 'Robot', 'mouse', 'Mouse', 'ray_tracing', 'RayTracing', 'navigation', 'Navigation', 'util', 'create_hexagon', 'environment', 'Environment', 'reward', 'Reward')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   'C:\\Research\\cellworld_game\\cellworld_game\\__init__.py'
+   filename   'C:\\research\\cellworld_game\\cellworld_game\\__init__.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c010c0114010c010c010c010c010c0114010c010c01
+   lnotab 0x00ff02010c010c0114010c010c010c010c010c010c010c01
```

### Comparing `cellworld_game-0.0.61/cellworld_game/__pycache__/agent.cpython-312.pyc` & `cellworld_game-0.0.68/cellworld_game/__pycache__/view.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Fri Apr 26 17:03:41 2024 UTC, .py size: 6294 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 22% similar despite different names*

```diff
@@ -1,639 +1,667 @@
-00000000: cb0d 0d0a 0000 0000 6dde 2b66 9618 0000  ........m.+f....
+00000000: cb0d 0d0a 0000 0000 9796 1566 ce1f 0000  ...........f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
-00000020: 0000 0000 00f3 ac00 0000 9700 6400 6401  ............d.d.
-00000030: 6c00 5a00 6400 6401 6c01 5a01 6400 6401  l.Z.d.d.l.Z.d.d.
-00000040: 6c02 5a02 6400 6401 6c03 5a04 6402 6403  l.Z.d.d.l.Z.d.d.
-00000050: 6c05 6d06 5a06 0100 6402 6404 6c07 6d08  l.m.Z...d.d.l.m.
-00000060: 5a08 6d09 5a09 6d0a 5a0a 0100 6400 6405  Z.m.Z.m.Z...d.d.
-00000070: 6c0b 6d0c 5a0c 6d0d 5a0d 0100 0200 4700  l.m.Z.m.Z.....G.
-00000080: 6406 8400 6407 650e ab03 0000 0000 0000  d...d.e.........
-00000090: 5a0f 0200 4700 6408 8400 6409 650e ab03  Z...G.d...d.e...
-000000a0: 0000 0000 0000 5a10 0200 4700 640a 8400  ......Z...G.d...
-000000b0: 640b 650e ab03 0000 0000 0000 5a11 0200  d.e.........Z...
-000000c0: 4700 640c 8400 640d 650e ab03 0000 0000  G.d...d.e.......
-000000d0: 0000 5a12 7901 290e e900 0000 004e e901  ..Z.y.)......N..
-000000e0: 0000 0029 01da 0952 6573 6f75 7263 6573  ...)...Resources
-000000f0: 2903 da0e 6372 6561 7465 5f68 6578 6167  )...create_hexag
-00000100: 6f6e da0a 6d6f 7665 5f70 6f69 6e74 da08  on..move_point..
-00000110: 6469 7374 616e 6365 2902 da06 726f 7461  distance)...rota
-00000120: 7465 da09 7472 616e 736c 6174 6563 0000  te..translatec..
-00000130: 0000 0000 0000 0000 0000 0500 0000 0000  ................
-00000140: 0000 f392 0000 0097 0065 005a 0164 005a  .........e.Z.d.Z
-00000150: 0209 0064 0964 0165 036a 0800 0000 0000  ...d.d.e.j......
-00000160: 0000 0000 0000 0000 0000 0000 0065 0565  .............e.e
-00000170: 0566 0219 0000 0064 0265 0666 0464 0384  .f.....d.e.f.d..
-00000180: 055a 0764 0465 036a 1000 0000 0000 0000  .Z.d.e.j........
-00000190: 0000 0000 0000 0000 0000 0065 0965 0a66  ...........e.e.f
-000001a0: 0219 0000 0066 0264 0584 045a 0b64 0665  .....f.d...Z.d.e
-000001b0: 036a 1000 0000 0000 0000 0000 0000 0000  .j..............
-000001c0: 0000 0000 0065 0965 0a66 0219 0000 0066  .....e.e.f.....f
-000001d0: 0264 0784 045a 0c79 0829 0ada 1343 6f6f  .d...Z.y.)...Coo
-000001e0: 7264 696e 6174 6543 6f6e 7665 7274 6572  rdinateConverter
-000001f0: da0b 7363 7265 656e 5f73 697a 65da 0666  ..screen_size..f
-00000200: 6c69 705f 7963 0300 0000 0000 0000 0000  lip_yc..........
-00000210: 0000 0300 0000 0300 0000 f3ba 0000 0097  ................
-00000220: 007c 017c 005f 0000 0000 0000 0000 007c  .|.|._.........|
-00000230: 015c 0200 007c 005f 0100 0000 0000 0000  .\...|._........
-00000240: 007c 005f 0200 0000 0000 0000 007c 027c  .|._.........|.|
-00000250: 005f 0300 0000 0000 0000 007c 006a 0200  ._.........|.j..
-00000260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000270: 007c 006a 0400 0000 0000 0000 0000 0000  .|.j............
-00000280: 0000 0000 0000 007a 0a00 0064 017a 0b00  .......z...d.z..
-00000290: 007c 005f 0400 0000 0000 0000 0074 0b00  .|._.........t..
-000002a0: 0000 0000 0000 006a 0c00 0000 0000 0000  .......j........
-000002b0: 0000 0000 0000 0000 0000 0064 02ab 0100  ...........d....
-000002c0: 0000 0000 0064 017a 0b00 007c 005f 0700  .....d.z...|._..
-000002d0: 0000 0000 0000 0079 0029 034e e902 0000  .......y.).N....
-000002e0: 00e9 0300 0000 2908 720c 0000 00da 0c73  ......).r......s
-000002f0: 6372 6565 6e5f 7769 6474 68da 0d73 6372  creen_width..scr
-00000300: 6565 6e5f 6865 6967 6874 720d 0000 00da  een_heightr.....
-00000310: 0d73 6372 6565 6e5f 6f66 6673 6574 da04  .screen_offset..
-00000320: 6d61 7468 da04 7371 7274 da0a 6865 7861  math..sqrt..hexa
-00000330: 5f72 6174 696f 2903 da04 7365 6c66 720c  _ratio)...selfr.
-00000340: 0000 0072 0d00 0000 7303 0000 0020 2020  ...r....s....   
-00000350: fa32 433a 5c52 6573 6561 7263 685c 6365  .2C:\Research\ce
-00000360: 6c6c 776f 726c 645f 6761 6d65 5c63 656c  llworld_game\cel
-00000370: 6c77 6f72 6c64 5f67 616d 655c 6167 656e  lworld_game\agen
-00000380: 742e 7079 da08 5f5f 696e 6974 5f5f 7a1c  t.py..__init__z.
-00000390: 436f 6f72 6469 6e61 7465 436f 6e76 6572  CoordinateConver
-000003a0: 7465 722e 5f5f 696e 6974 5f5f 0b00 0000  ter.__init__....
-000003b0: 7355 0000 0080 00f0 0600 1c27 8804 d408  sU.........'....
-000003c0: 18d8 303b d108 2d88 04d4 0819 9834 d41b  ..0;..-......4..
-000003d0: 2dd8 161c 8804 8c0b d81e 22d7 1e2f d11e  -........."../..
-000003e0: 2fb0 24d7 3244 d132 44d1 1e44 c801 d11d  /.$.2D.2D..D....
-000003f0: 4988 04d4 081a dc1b 1f9f 3999 39a0 519b  I.........9.9.Q.
-00000400: 3ca8 21d1 1b2b 8804 8d0f f300 0000 00da  <.!..+..........
-00000410: 0963 616e 6f6e 6963 616c 6302 0000 0000  .canonicalc.....
-00000420: 0000 0000 0000 0004 0000 0003 0000 00f3  ................
-00000430: 0601 0000 9700 7401 0000 0000 0000 0000  ......t.........
-00000440: 7c01 7402 0000 0000 0000 0000 ab02 0000  |.t.............
-00000450: 0000 0000 720f 7c01 7c00 6a04 0000 0000  ....r.|.|.j.....
-00000460: 0000 0000 0000 0000 0000 0000 0000 7a05  ..............z.
-00000470: 0000 5300 7c01 5c02 0000 7d02 7d03 7c02  ..S.|.\...}.}.|.
-00000480: 7c00 6a04 0000 0000 0000 0000 0000 0000  |.j.............
-00000490: 0000 0000 0000 7a05 0000 7d04 7c00 6a06  ......z...}.|.j.
-000004a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004b0: 0000 7223 6401 7c03 7a0a 0000 7c00 6a04  ..r#d.|.z...|.j.
-000004c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004d0: 0000 7a05 0000 7c00 6a08 0000 0000 0000  ..z...|.j.......
-000004e0: 0000 0000 0000 0000 0000 0000 7a0a 0000  ............z...
-000004f0: 7d05 7c04 7c05 6602 5300 7c03 7c00 6a04  }.|.|.f.S.|.|.j.
-00000500: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000510: 0000 7a05 0000 7c00 6a08 0000 0000 0000  ..z...|.j.......
-00000520: 0000 0000 0000 0000 0000 0000 7a0a 0000  ............z...
-00000530: 7d05 7c04 7c05 6602 5300 2902 4e72 0300  }.|.|.f.S.).Nr..
-00000540: 0000 2905 da0a 6973 696e 7374 616e 6365  ..)...isinstance
-00000550: da05 666c 6f61 7472 1100 0000 720d 0000  ..floatr....r...
-00000560: 0072 1300 0000 2906 7217 0000 0072 1b00  .r....).r....r..
-00000570: 0000 da0b 6361 6e6f 6e69 6361 6c5f 78da  ....canonical_x.
-00000580: 0b63 616e 6f6e 6963 616c 5f79 da08 7363  .canonical_y..sc
-00000590: 7265 656e 5f78 da08 7363 7265 656e 5f79  reen_x..screen_y
-000005a0: 7306 0000 0020 2020 2020 2072 1800 0000  s....      r....
-000005b0: da0e 6672 6f6d 5f63 616e 6f6e 6963 616c  ..from_canonical
-000005c0: 7a22 436f 6f72 6469 6e61 7465 436f 6e76  z"CoordinateConv
-000005d0: 6572 7465 722e 6672 6f6d 5f63 616e 6f6e  erter.from_canon
-000005e0: 6963 616c 1400 0000 7392 0000 0080 00dc  ical....s.......
-000005f0: 0b15 9069 a415 d40b 27d8 131c 9874 d71f  ...i....'....t..
-00000600: 30d1 1f30 d113 30d0 0c30 e023 2cd1 0820  0..0..0..0.#,.. 
-00000610: 880b 905b d813 1ea0 14d7 2132 d121 32d1  ...[......!2.!2.
-00000620: 1332 8808 d80b 0f8f 3b8a 3bd8 1819 982b  .2......;.;....+
-00000630: 990d a814 d729 3ad1 293a d117 3ab8 54d7  .....):.):..:.T.
-00000640: 3d4f d13d 4fd1 174f 8848 f006 0010 1898  =O.=O..O.H......
-00000650: 18d0 0f21 d008 21f0 0300 1823 a054 d725  ...!..!....#.T.%
-00000660: 36d1 2536 d117 36b8 14d7 394b d139 4bd1  6.%6..6...9K.9K.
-00000670: 174b 8848 d80f 1798 18d0 0f21 d008 2172  .K.H.......!..!r
-00000680: 1a00 0000 da06 7363 7265 656e 6302 0000  ......screenc...
-00000690: 0000 0000 0000 0000 0004 0000 0003 0000  ................
-000006a0: 00f3 e000 0000 9700 7401 0000 0000 0000  ........t.......
-000006b0: 0000 7c01 7402 0000 0000 0000 0000 ab02  ..|.t...........
-000006c0: 0000 0000 0000 720f 7c01 7c00 6a04 0000  ......r.|.|.j...
-000006d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000006e0: 7a0b 0000 5300 7c01 5c02 0000 7d02 7d03  z...S.|.\...}.}.
-000006f0: 7c00 6a06 0000 0000 0000 0000 0000 0000  |.j.............
-00000700: 0000 0000 0000 7c03 7a0a 0000 7c00 6a08  ......|.z...|.j.
-00000710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000720: 0000 7a00 0000 7d04 7c04 7c00 6a06 0000  ..z...}.|.|.j...
-00000730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000740: 7a0b 0000 7c00 6a0a 0000 0000 0000 0000  z...|.j.........
-00000750: 0000 0000 0000 0000 0000 7a05 0000 7d05  ..........z...}.
-00000760: 7c02 7c00 6a04 0000 0000 0000 0000 0000  |.|.j...........
-00000770: 0000 0000 0000 0000 7a0b 0000 7d06 7c06  ........z...}.|.
-00000780: 7c05 6602 5300 a901 4e29 0672 1d00 0000  |.f.S...N).r....
-00000790: 721e 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
-000007a0: 1300 0000 7216 0000 0029 0772 1700 0000  ....r....).r....
-000007b0: 7224 0000 0072 2100 0000 7222 0000 00da  r$...r!...r"....
-000007c0: 0179 7220 0000 0072 1f00 0000 7307 0000  .yr ...r....s...
-000007d0: 0020 2020 2020 2020 7218 0000 00da 0c74  .       r......t
-000007e0: 6f5f 6361 6e6f 6e69 6361 6c7a 2043 6f6f  o_canonicalz Coo
-000007f0: 7264 696e 6174 6543 6f6e 7665 7274 6572  rdinateConverter
-00000800: 2e74 6f5f 6361 6e6f 6e69 6361 6c20 0000  .to_canonical ..
-00000810: 0073 7600 0000 8000 dc0b 1590 669c 65d4  .sv.........f.e.
-00000820: 0b24 d813 1998 44d7 1c2d d11c 2dd1 132d  .$....D..-..-..-
-00000830: d00c 2de0 1d23 d108 1a88 0890 28d8 0c10  ..-..#......(...
-00000840: d70c 1ed1 0c1e a018 d10c 29a8 44d7 2c3e  ..........).D.,>
-00000850: d12c 3ed1 0c3e 8801 d816 1798 24d7 1a2c  .,>..>......$..,
-00000860: d11a 2cd1 162c a874 af7f a97f d116 3e88  ..,..,.t......>.
-00000870: 0bd8 161e a014 d721 32d1 2132 d116 3288  .......!2.!2..2.
-00000880: 0bd8 0f1a 984b d00f 27d0 0827 721a 0000  .....K..'..'r...
-00000890: 004e 2901 4629 0dda 085f 5f6e 616d 655f  .N).F)...__name_
-000008a0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-000008b0: 5f71 7561 6c6e 616d 655f 5fda 0674 7970  _qualname__..typ
-000008c0: 696e 67da 0554 7570 6c65 da03 696e 74da  ing..Tuple..int.
-000008d0: 0462 6f6f 6c72 1900 0000 da05 556e 696f  .boolr......Unio
-000008e0: 6eda 0574 7570 6c65 721e 0000 0072 2300  n..tupler....r#.
-000008f0: 0000 7228 0000 00a9 0072 1a00 0000 7218  ..r(.....r....r.
-00000900: 0000 0072 0b00 0000 720b 0000 000a 0000  ...r....r.......
-00000910: 0073 5b00 0000 8400 f006 0021 26f1 0507  .s[........!&...
-00000920: 052d d81e 249f 6c99 6ca8 33b0 03a8 38d1  .-..$.l.l.3...8.
-00000930: 1e34 f003 0705 2de0 191d f305 0705 2df0  .4....-.......-.
-00000940: 120a 0522 a806 af0c a90c b055 b845 b05c  ...".......U.E.\
-00000950: d128 42f3 000a 0522 f018 0805 28a0 36a7  .(B...."....(.6.
-00000960: 3ca1 3cb0 05b0 75b0 0cd1 233d f400 0805  <.<...u...#=....
-00000970: 2872 1a00 0000 720b 0000 0063 0000 0000  (r....r....c....
-00000980: 0000 0000 0000 0000 0600 0000 0000 0000  ................
-00000990: f356 0000 0097 0065 005a 0164 005a 0264  .V.....e.Z.d.Z.d
-000009a0: 0a64 0165 036a 0800 0000 0000 0000 0000  .d.e.j..........
-000009b0: 0000 0000 0000 0000 0065 0565 0566 0219  .........e.e.f..
-000009c0: 0000 0064 0265 0566 0464 0384 055a 0664  ...d.e.f.d...Z.d
-000009d0: 0484 005a 0764 0565 0564 0665 0564 0764  ...Z.d.e.d.e.d.d
-000009e0: 0066 0664 0884 045a 0879 0929 0bda 0a41  .f.d...Z.y.)...A
-000009f0: 6765 6e74 5374 6174 65da 086c 6f63 6174  gentState..locat
-00000a00: 696f 6eda 0964 6972 6563 7469 6f6e 6303  ion..directionc.
-00000a10: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00000a20: 0000 00f3 2000 0000 9700 7c01 7c00 5f00  .... .....|.|._.
-00000a30: 0000 0000 0000 0000 7c02 7c00 5f01 0000  ........|.|._...
-00000a40: 0000 0000 0000 7900 7226 0000 00a9 0272  ......y.r&.....r
-00000a50: 3500 0000 7236 0000 0029 0372 1700 0000  5...r6...).r....
-00000a60: 7235 0000 0072 3600 0000 7303 0000 0020  r5...r6...s.... 
-00000a70: 2020 7218 0000 0072 1900 0000 7a13 4167    r....r....z.Ag
-00000a80: 656e 7453 7461 7465 2e5f 5f69 6e69 745f  entState.__init_
-00000a90: 5f2c 0000 0073 1000 0000 8000 d818 2088  _,...s........ .
-00000aa0: 048c 0dd8 1922 8804 8d0e 721a 0000 0063  ....."....r....c
-00000ab0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000ac0: 2300 0000 f344 0000 004b 0001 0097 007c  #....D...K.....|
-00000ad0: 006a 0000 0000 0000 0000 0000 0000 0000  .j..............
-00000ae0: 0000 0000 0096 0197 0101 007c 006a 0200  ...........|.j..
-00000af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b00: 0096 0197 0101 0079 00ad 0377 0172 2600  .......y...w.r&.
-00000b10: 0000 7238 0000 00a9 0172 1700 0000 7301  ..r8.....r....s.
-00000b20: 0000 0020 7218 0000 00da 085f 5f69 7465  ... r......__ite
-00000b30: 725f 5f7a 1341 6765 6e74 5374 6174 652e  r__z.AgentState.
-00000b40: 5f5f 6974 6572 5f5f 3000 0000 731a 0000  __iter__0...s...
-00000b50: 00e8 00f8 8000 d80e 128f 6d89 6dd2 081b  ..........m.m...
-00000b60: d80e 128f 6e89 6ed3 081c f9f3 0400 0000  ....n.n.........
-00000b70: 821e 2001 7207 0000 00da 0872 6f74 6174  .. .r......rotat
-00000b80: 696f 6eda 0672 6574 7572 6e63 0300 0000  ion..returnc....
-00000b90: 0000 0000 0000 0000 0700 0000 0300 0000  ................
-00000ba0: f366 0000 0097 007c 006a 0000 0000 0000  .f.....|.j......
-00000bb0: 0000 0000 0000 0000 0000 0000 007c 027a  .............|.z
-00000bc0: 0000 007d 0374 0300 0000 0000 0000 0074  ...}.t.........t
-00000bd0: 0500 0000 0000 0000 007c 006a 0600 0000  .........|.j....
-00000be0: 0000 0000 0000 0000 0000 0000 0000 007c  ...............|
-00000bf0: 037c 01ac 01ab 0300 0000 0000 007c 03ac  .|...........|..
-00000c00: 02ab 0200 0000 0000 0053 0029 034e 2903  .........S.).N).
-00000c10: da05 7374 6172 7472 3600 0000 7207 0000  ..startr6...r...
-00000c20: 0072 3800 0000 2904 7236 0000 0072 3400  .r8...).r6...r4.
-00000c30: 0000 7206 0000 0072 3500 0000 2904 7217  ..r....r5...).r.
-00000c40: 0000 0072 0700 0000 723d 0000 00da 0d6e  ...r....r=.....n
-00000c50: 6577 5f64 6972 6563 7469 6f6e 7304 0000  ew_directions...
-00000c60: 0020 2020 2072 1800 0000 da06 7570 6461  .    r......upda
-00000c70: 7465 7a11 4167 656e 7453 7461 7465 2e75  tez.AgentState.u
-00000c80: 7064 6174 6534 0000 0073 3800 0000 8000  pdate4...s8.....
-00000c90: f006 0019 1d9f 0e99 0ea8 18d1 1831 880d  .............1..
-00000ca0: dc0f 19a4 3ab0 44b7 4db1 4dd8 3845 d837  ....:.D.M.M.8E.7
-00000cb0: 3ff4 0502 2441 01f0 0600 2532 f407 0310  ?...$A....%2....
-00000cc0: 33f0 0003 0933 721a 0000 004e 2902 a902  3....3r....N)...
-00000cd0: 7202 0000 0072 0200 0000 7202 0000 0029  r....r....r....)
-00000ce0: 0972 2900 0000 722a 0000 0072 2b00 0000  .r)...r*...r+...
-00000cf0: 722c 0000 0072 2d00 0000 721e 0000 0072  r,...r-...r....r
-00000d00: 1900 0000 723b 0000 0072 4200 0000 7232  ....r;...rB...r2
-00000d10: 0000 0072 1a00 0000 7218 0000 0072 3400  ...r....r....r4.
-00000d20: 0000 7234 0000 002b 0000 0073 4500 0000  ..r4...+...sE...
-00000d30: 8400 f102 0205 23a0 16a7 1ca1 1ca8 65b0  ......#.......e.
-00000d40: 55a8 6cd1 213b f000 0205 23d0 5156 f300  U.l.!;....#.QV..
-00000d50: 0205 23f2 0802 051d f008 0705 33d8 191e  ..#.........3...
-00000d60: f003 0705 33e0 191e f005 0705 33e0 232f  ....3.......3.#/
-00000d70: f405 0705 3372 1a00 0000 7234 0000 0063  ....3r....r4...c
-00000d80: 0000 0000 0000 0000 0000 0000 0400 0000  ................
-00000d90: 0000 0000 f332 0000 0097 0065 005a 0164  .....2.....e.Z.d
-00000da0: 005a 0264 0165 0364 0265 0366 0464 0384  .Z.d.e.d.e.f.d..
-00000db0: 045a 0464 0484 005a 0564 0565 0364 0665  .Z.d...Z.d.e.d.e
-00000dc0: 0666 0464 0784 045a 0779 0829 09da 0d41  .f.d...Z.y.)...A
-00000dd0: 6765 6e74 4479 6e61 6d69 6373 da0d 666f  gentDynamics..fo
-00000de0: 7277 6172 645f 7370 6565 64da 0a74 7572  rward_speed..tur
-00000df0: 6e5f 7370 6565 6463 0300 0000 0000 0000  n_speedc........
-00000e00: 0000 0000 0200 0000 0300 0000 f320 0000  ............. ..
-00000e10: 0097 007c 017c 005f 0000 0000 0000 0000  ...|.|._........
-00000e20: 007c 027c 005f 0100 0000 0000 0000 0079  .|.|._.........y
-00000e30: 0072 2600 0000 a902 7246 0000 0072 4700  .r&.....rF...rG.
-00000e40: 0000 2903 7217 0000 0072 4600 0000 7247  ..).r....rF...rG
-00000e50: 0000 0073 0300 0000 2020 2072 1800 0000  ...s....   r....
-00000e60: 7219 0000 007a 1641 6765 6e74 4479 6e61  r....z.AgentDyna
-00000e70: 6d69 6373 2e5f 5f69 6e69 745f 5f3f 0000  mics.__init__?..
-00000e80: 0073 1100 0000 8000 d81d 2a88 04d4 081a  .s........*.....
-00000e90: d81a 2488 048d 0f72 1a00 0000 6301 0000  ..$....r....c...
-00000ea0: 0000 0000 0000 0000 0002 0000 0023 0000  .............#..
-00000eb0: 00f3 4400 0000 4b00 0100 9700 7c00 6a00  ..D...K.....|.j.
-00000ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000ed0: 0000 9601 9701 0100 7c00 6a02 0000 0000  ........|.j.....
-00000ee0: 0000 0000 0000 0000 0000 0000 0000 9601  ................
-00000ef0: 9701 0100 7900 ad03 7701 7226 0000 0072  ....y...w.r&...r
-00000f00: 4900 0000 723a 0000 0073 0100 0000 2072  I...r:...s.... r
-00000f10: 1800 0000 723b 0000 007a 1641 6765 6e74  ....r;...z.Agent
-00000f20: 4479 6e61 6d69 6373 2e5f 5f69 7465 725f  Dynamics.__iter_
-00000f30: 5f43 0000 0073 1c00 0000 e800 f880 00d8  _C...s..........
-00000f40: 0e12 d70e 20d1 0e20 d208 20d8 0e12 8f6f  .... .. .. ....o
-00000f50: 896f d308 1df9 723c 0000 00da 0764 656c  .o....r<.....del
-00000f60: 7461 5f74 723e 0000 0063 0200 0000 0000  ta_tr>...c......
-00000f70: 0000 0000 0000 0300 0000 0300 0000 f33e  ...............>
-00000f80: 0000 0097 007c 006a 0000 0000 0000 0000  .....|.j........
-00000f90: 0000 0000 0000 0000 0000 007c 017a 0500  ...........|.z..
-00000fa0: 007c 006a 0200 0000 0000 0000 0000 0000  .|.j............
-00000fb0: 0000 0000 0000 007c 017a 0500 0066 0253  .......|.z...f.S
-00000fc0: 0072 2600 0000 7249 0000 00a9 0272 1700  .r&...rI.....r..
-00000fd0: 0000 724b 0000 0073 0200 0000 2020 7218  ..rK...s....  r.
-00000fe0: 0000 00da 0663 6861 6e67 657a 1441 6765  .....changez.Age
-00000ff0: 6e74 4479 6e61 6d69 6373 2e63 6861 6e67  ntDynamics.chang
-00001000: 6547 0000 0073 2100 0000 8000 d80f 13d7  eG...s!.........
-00001010: 0f21 d10f 21a0 47d1 0f2b a864 af6f a96f  .!..!.G..+.d.o.o
-00001020: c007 d12e 47d0 0f47 d008 4772 1a00 0000  ....G..G..Gr....
-00001030: 4e29 0872 2900 0000 722a 0000 0072 2b00  N).r)...r*...r+.
-00001040: 0000 721e 0000 0072 1900 0000 723b 0000  ..r....r....r;..
-00001050: 0072 3100 0000 724e 0000 0072 3200 0000  .r1...rN...r2...
-00001060: 721a 0000 0072 1800 0000 7245 0000 0072  r....r....rE...r
-00001070: 4500 0000 3e00 0000 7330 0000 0084 00f0  E...>...s0......
-00001080: 0202 0525 a065 f000 0205 25b8 15f3 0002  ...%.e....%.....
-00001090: 0525 f208 0205 1ef0 0801 0548 0198 65f0  .%.........H..e.
-000010a0: 0001 0548 01a8 05f4 0001 0548 0172 1a00  ...H.......H.r..
-000010b0: 0000 7245 0000 0063 0000 0000 0000 0000  ..rE...c........
-000010c0: 0000 0000 0500 0000 0000 0000 f358 0100  .............X..
-000010d0: 0097 0065 005a 0164 005a 0209 0009 0064  ...e.Z.d.Z.....d
-000010e0: 1964 0165 0364 0265 0466 0464 0384 055a  .d.e.d.e.f.d...Z
-000010f0: 0564 0465 0666 0264 0584 045a 0764 0665  .d.e.f.d...Z.d.e
-00001100: 0864 0764 0866 0464 0984 045a 0965 0a64  .d.d.f.d...Z.e.d
-00001110: 0765 0866 0264 0a84 04ab 0000 0000 0000  .e.f.d..........
-00001120: 005a 0b64 1a64 0b84 045a 0c64 1a64 0c84  .Z.d.d...Z.d.d..
-00001130: 045a 0d64 0d65 0364 0764 0866 0464 0e84  .Z.d.e.d.d.f.d..
-00001140: 045a 0e65 0f64 0765 106a 2200 0000 0000  .Z.e.d.e.j".....
-00001150: 0000 0000 0000 0000 0000 0000 0066 0264  .............f.d
-00001160: 0f84 04ab 0000 0000 0000 005a 1265 0f64  ...........Z.e.d
-00001170: 0765 136a 2800 0000 0000 0000 0000 0000  .e.j(...........
-00001180: 0000 0000 0000 0066 0264 1084 04ab 0000  .......f.d......
-00001190: 0000 0000 005a 1509 0064 1b64 0665 0864  .....Z...d.d.e.d
-000011a0: 0765 136a 2800 0000 0000 0000 0000 0000  .e.j(...........
-000011b0: 0000 0000 0000 0066 0464 1184 055a 1664  .......f.d...Z.d
-000011c0: 0765 106a 2200 0000 0000 0000 0000 0000  .e.j"...........
-000011d0: 0000 0000 0000 0066 0264 1284 045a 1764  .......f.d...Z.d
-000011e0: 0765 1866 0264 1384 045a 1964 0765 1866  .e.f.d...Z.d.e.f
-000011f0: 0264 1484 045a 1a64 1565 106a 2200 0000  .d...Z.d.e.j"...
-00001200: 0000 0000 0000 0000 0000 0000 0000 0064  ...............d
-00001210: 1665 1b66 0464 1784 045a 1c64 1665 1b66  .e.f.d...Z.d.e.f
-00001220: 0264 1884 045a 1d79 0829 1cda 0541 6765  .d...Z.y.)...Age
-00001230: 6e74 da0a 7669 6577 5f66 6965 6c64 da09  nt..view_field..
-00001240: 636f 6c6c 6973 696f 6e63 0300 0000 0000  collisionc......
-00001250: 0000 0000 0000 0400 0000 0300 0000 f318  ................
-00001260: 0100 0097 0064 017c 005f 0000 0000 0000  .....d.|._......
-00001270: 0000 007c 017c 005f 0100 0000 0000 0000  ...|.|._........
-00001280: 0074 0500 0000 0000 0000 00ab 0000 0000  .t..............
-00001290: 0000 007c 005f 0300 0000 0000 0000 0074  ...|._.........t
-000012a0: 0900 0000 0000 0000 0064 0264 02ac 03ab  .........d.d....
-000012b0: 0200 0000 0000 007c 005f 0500 0000 0000  .......|._......
-000012c0: 0000 007c 006a 0d00 0000 0000 0000 0000  ...|.j..........
-000012d0: 0000 0000 0000 0000 00ab 0000 0000 0000  ................
-000012e0: 007c 005f 0700 0000 0000 0000 0064 007c  .|._.........d.|
-000012f0: 005f 0800 0000 0000 0000 007c 027c 005f  ._.........|.|._
-00001300: 0900 0000 0000 0000 0064 007c 005f 0a00  .........d.|._..
-00001310: 0000 0000 0000 0064 007c 005f 0b00 0000  .......d.|._....
-00001320: 0000 0000 0064 007c 005f 0c00 0000 0000  .....d.|._......
-00001330: 0000 0064 047c 005f 0d00 0000 0000 0000  ...d.|._........
-00001340: 0064 007c 005f 0e00 0000 0000 0000 0067  .d.|._.........g
-00001350: 007c 005f 0f00 0000 0000 0000 0064 007c  .|._.........d.|
-00001360: 005f 1000 0000 0000 0000 0064 057c 005f  ._.........d.|._
-00001370: 1100 0000 0000 0000 0079 0029 064e 5472  .........y.).NTr
-00001380: 0200 0000 7249 0000 00da 0046 2912 da07  ....rI.....F)...
-00001390: 7669 7369 626c 6572 5100 0000 7234 0000  visiblerQ...r4..
-000013a0: 00da 065f 7374 6174 6572 4500 0000 da08  ..._staterE.....
-000013b0: 6479 6e61 6d69 6373 da0e 6372 6561 7465  dynamics..create
-000013c0: 5f70 6f6c 7967 6f6e da07 706f 6c79 676f  _polygon..polygo
-000013d0: 6eda 0673 7072 6974 6572 5200 0000 da08  n..spriterR.....
-000013e0: 6f6e 5f72 6573 6574 da07 6f6e 5f73 7465  on_reset..on_ste
-000013f0: 70da 086f 6e5f 7374 6172 74da 046e 616d  p..on_start..nam
-00001400: 65da 056d 6f64 656c da0a 7472 616a 6563  e..model..trajec
-00001410: 746f 7279 da14 636f 6f72 6469 6e61 7465  tory..coordinate
-00001420: 5f63 6f6e 7665 7274 6572 da07 7275 6e6e  _converter..runn
-00001430: 696e 6729 0372 1700 0000 7251 0000 0072  ing).r....rQ...r
-00001440: 5200 0000 7303 0000 0020 2020 7218 0000  R...s....   r...
-00001450: 0072 1900 0000 7a0e 4167 656e 742e 5f5f  .r....z.Agent.__
-00001460: 696e 6974 5f5f 4d00 0000 7384 0000 0080  init__M...s.....
-00001470: 00f0 0600 181c 8804 8c0c d81a 2488 048c  ............$...
-00001480: 0fdc 222c a32c 8804 8c0b dc27 34c0 31d8  ..",.,.....'4.1.
-00001490: 4041 f403 0128 4301 8804 8c0d e017 1bd7  @A...(C.........
-000014a0: 172a d117 2ad3 172c 8804 8c0c d816 1a88  .*..*..,........
-000014b0: 048c 0bd8 1922 8804 8c0e d818 1c88 048c  ....."..........
-000014c0: 0dd8 171b 8804 8c0c d818 1c88 048c 0dd8  ................
-000014d0: 1416 8804 8c09 d815 1988 048c 0ad8 3335  ..............35
-000014e0: 8804 8c0f d84a 4e88 04d4 0821 d817 1c88  .....JN....!....
-000014f0: 048d 0c72 1a00 0000 da04 7369 7a65 6302  ...r......sizec.
-00001500: 0000 0000 0000 0000 0000 0004 0000 0003  ................
-00001510: 0000 00f3 6a00 0000 9700 7400 0000 0000  ....j.....t.....
-00001520: 0000 0000 6a02 0000 0000 0000 0000 0000  ....j...........
-00001530: 0000 0000 0000 0000 6a05 0000 0000 0000  ........j.......
-00001540: 0000 0000 0000 0000 0000 0000 7c00 6a07  ............|.j.
-00001550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001560: 0000 ab00 0000 0000 0000 7c01 ab02 0000  ..........|.....
-00001570: 0000 0000 7c00 5f04 0000 0000 0000 0000  ....|._.........
-00001580: 7900 7226 0000 0029 05da 0670 7967 616d  y.r&...)...pygam
-00001590: 65da 0974 7261 6e73 666f 726d da05 7363  e..transform..sc
-000015a0: 616c 65da 0d63 7265 6174 655f 7370 7269  ale..create_spri
-000015b0: 7465 725a 0000 0029 0272 1700 0000 7263  terZ...).r....rc
-000015c0: 0000 0073 0200 0000 2020 7218 0000 00da  ...s....  r.....
-000015d0: 0f73 6574 5f73 7072 6974 655f 7369 7a65  .set_sprite_size
-000015e0: 7a15 4167 656e 742e 7365 745f 7370 7269  z.Agent.set_spri
-000015f0: 7465 5f73 697a 6561 0000 0073 2500 0000  te_sizea...s%...
-00001600: 8000 dc16 1cd7 1626 d116 26d7 162c d116  .......&..&..,..
-00001610: 2ca8 54d7 2d3f d12d 3fd3 2d41 c034 d316  ,.T.-?.-?.-A.4..
-00001620: 4888 048d 0b72 1a00 0000 da05 7374 6174  H....r......stat
-00001630: 6572 3e00 0000 4e63 0200 0000 0000 0000  er>...Nc........
-00001640: 0000 0000 0300 0000 0300 0000 f348 0000  .............H..
-00001650: 0097 007c 006a 0000 0000 0000 0000 0000  ...|.j..........
-00001660: 0000 0000 0000 0000 006a 0300 0000 0000  .........j......
-00001670: 0000 0000 0000 0000 0000 0000 007c 01ab  .............|..
-00001680: 0100 0000 0000 0001 007c 017c 005f 0200  .........|.|._..
-00001690: 0000 0000 0000 0079 0072 2600 0000 2903  .......y.r&...).
-000016a0: 7260 0000 00da 0661 7070 656e 6472 5600  r`.....appendrV.
-000016b0: 0000 2902 7217 0000 0072 6a00 0000 7302  ..).r....rj...s.
-000016c0: 0000 0020 2072 1800 0000 da09 7365 745f  ...  r......set_
-000016d0: 7374 6174 657a 0f41 6765 6e74 2e73 6574  statez.Agent.set
-000016e0: 5f73 7461 7465 6400 0000 731b 0000 0080  _stated...s.....
-000016f0: 00d8 080c 8f0f 890f d708 1ed1 081e 9875  ...............u
-00001700: d408 25d8 161b 8804 8d0b 721a 0000 0063  ..%.......r....c
-00001710: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00001720: 0300 0000 f31a 0000 0097 007c 006a 0000  ...........|.j..
-00001730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001740: 0053 0072 2600 0000 2901 7256 0000 0072  .S.r&...).rV...r
-00001750: 3a00 0000 7301 0000 0020 7218 0000 0072  :...s.... r....r
-00001760: 6a00 0000 7a0b 4167 656e 742e 7374 6174  j...z.Agent.stat
-00001770: 6568 0000 0073 0c00 0000 8000 e00f 138f  eh...s..........
-00001780: 7b89 7bd0 081a 721a 0000 0063 0100 0000  {.{...r....c....
-00001790: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-000017a0: f37e 0000 0097 007c 006a 0000 0000 0000  .~.....|.j......
-000017b0: 0000 0000 0000 0000 0000 0000 006a 0300  .............j..
+00000020: 0000 0000 00f3 4e00 0000 9700 6400 6401  ......N.....d.d.
+00000030: 6c00 5a00 6402 6403 6c01 6d02 5a02 0100  l.Z.d.d.l.m.Z...
+00000040: 6402 6404 6c03 6d04 5a04 0100 6400 6401  d.d.l.m.Z...d.d.
+00000050: 6c05 5a05 6402 6405 6c06 6d07 5a07 0100  l.Z.d.d.l.m.Z...
+00000060: 0200 4700 6406 8400 6407 6508 ab03 0000  ..G.d...d.e.....
+00000070: 0000 0000 5a09 7901 2908 e900 0000 004e  ....Z.y.)......N
+00000080: e901 0000 0029 01da 054d 6f64 656c 2901  .....)...Model).
+00000090: da05 4167 656e 7429 01da 1867 656e 6572  ..Agent)...gener
+000000a0: 6174 655f 6469 7374 696e 6374 5f63 6f6c  ate_distinct_col
+000000b0: 6f72 7363 0000 0000 0000 0000 0000 0000  orsc............
+000000c0: 0700 0000 0000 0000 f36a 0000 0097 0065  .........j.....e
+000000d0: 005a 0164 005a 0209 0009 0064 1164 0165  .Z.d.Z.....d.d.e
+000000e0: 0364 0265 0464 0365 0566 0664 0484 055a  .d.e.d.e.f.d...Z
+000000f0: 0664 0565 0766 0264 0684 045a 0864 0765  .d.e.f.d...Z.d.e
+00000100: 0464 0865 0466 0464 0984 045a 0964 0a84  .d.e.f.d...Z.d..
+00000110: 005a 0a64 1264 0b84 015a 0b64 1264 0c84  .Z.d.d...Z.d.d..
+00000120: 015a 0c64 0d65 0d66 0264 0e84 045a 0e64  .Z.d.e.f.d...Z.d
+00000130: 0f84 005a 0f79 1029 13da 0456 6965 77da  ...Z.y.)...View.
+00000140: 056d 6f64 656c da0c 7363 7265 656e 5f77  .model..screen_w
+00000150: 6964 7468 da06 666c 6970 5f79 6304 0000  idth..flip_yc...
+00000160: 0000 0000 0000 0000 0008 0000 0003 0000  ................
+00000170: 00f3 3003 0000 9700 7401 0000 0000 0000  ..0.....t.......
+00000180: 0000 6a02 0000 0000 0000 0000 0000 0000  ..j.............
+00000190: 0000 0000 0000 ab00 0000 0000 0000 0100  ................
+000001a0: 7c01 7c00 5f02 0000 0000 0000 0000 7c01  |.|._.........|.
+000001b0: 6a06 0000 0000 0000 0000 0000 0000 0000  j...............
+000001c0: 0000 0000 7c00 5f03 0000 0000 0000 0000  ....|._.........
+000001d0: 7c02 7c00 5f04 0000 0000 0000 0000 740b  |.|._.........t.
+000001e0: 0000 0000 0000 0000 6a0c 0000 0000 0000  ........j.......
+000001f0: 0000 0000 0000 0000 0000 0000 6401 ab01  ............d...
+00000200: 0000 0000 0000 6402 7a0b 0000 7c00 5f07  ......d.z...|._.
+00000210: 0000 0000 0000 0000 7411 0000 0000 0000  ........t.......
+00000220: 0000 7c00 6a0e 0000 0000 0000 0000 0000  ..|.j...........
+00000230: 0000 0000 0000 0000 7c02 7a05 0000 ab01  ........|.z.....
+00000240: 0000 0000 0000 7c00 5f09 0000 0000 0000  ......|._.......
+00000250: 0000 7c03 7c00 5f0a 0000 0000 0000 0000  ..|.|._.........
+00000260: 7c00 6a08 0000 0000 0000 0000 0000 0000  |.j.............
+00000270: 0000 0000 0000 7c00 6a12 0000 0000 0000  ......|.j.......
+00000280: 0000 0000 0000 0000 0000 0000 7a0a 0000  ............z...
+00000290: 6402 7a0b 0000 7c00 5f0b 0000 0000 0000  d.z...|._.......
+000002a0: 0000 7c02 7c00 6a12 0000 0000 0000 0000  ..|.|.j.........
+000002b0: 0000 0000 0000 0000 0000 6602 7c00 5f0c  ..........f.|._.
+000002c0: 0000 0000 0000 0000 7400 0000 0000 0000  ........t.......
+000002d0: 0000 6a1a 0000 0000 0000 0000 0000 0000  ..j.............
+000002e0: 0000 0000 0000 6a1d 0000 0000 0000 0000  ......j.........
+000002f0: 0000 0000 0000 0000 0000 7c00 6a18 0000  ..........|.j...
+00000300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000310: ab01 0000 0000 0000 7c00 5f0f 0000 0000  ........|._.....
+00000320: 0000 0000 6403 7c00 5f10 0000 0000 0000  ....d.|._.......
+00000330: 0000 6404 7c00 5f11 0000 0000 0000 0000  ..d.|._.........
+00000340: 7425 0000 0000 0000 0000 7c00 6a04 0000  t%........|.j...
+00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000360: 6a26 0000 0000 0000 0000 0000 0000 0000  j&..............
+00000370: 0000 0000 6a29 0000 0000 0000 0000 0000  ....j)..........
+00000380: 0000 0000 0000 0000 ab00 0000 0000 0000  ................
+00000390: 742b 0000 0000 0000 0000 742d 0000 0000  t+........t-....
+000003a0: 0000 0000 7c00 6a04 0000 0000 0000 0000  ....|.j.........
+000003b0: 0000 0000 0000 0000 0000 6a26 0000 0000  ..........j&....
+000003c0: 0000 0000 0000 0000 0000 0000 0000 ab01  ................
+000003d0: 0000 0000 0000 ab01 0000 0000 0000 ab02  ................
+000003e0: 0000 0000 0000 4400 8f04 8f05 6303 6900  ......D.....c.i.
+000003f0: 6302 5d08 0000 5c02 0000 7d04 7d05 7c04  c.]...\...}.}.|.
+00000400: 7c05 9302 8c0a 0400 6303 7d05 7d04 7c00  |.......c.}.}.|.
+00000410: 5f17 0000 0000 0000 0000 7400 0000 0000  _.........t.....
+00000420: 0000 0000 6a30 0000 0000 0000 0000 0000  ....j0..........
+00000430: 0000 0000 0000 0000 6a33 0000 0000 0000  ........j3......
+00000440: 0000 0000 0000 0000 0000 0000 ab00 0000  ................
+00000450: 0000 0000 7c00 5f1a 0000 0000 0000 0000  ....|._.........
+00000460: 6405 7c00 5f1b 0000 0000 0000 0000 6406  d.|._.........d.
+00000470: 7c00 5f1c 0000 0000 0000 0000 6400 7c00  |._.........d.|.
+00000480: 5f1d 0000 0000 0000 0000 6400 7c00 5f1e  _.........d.|._.
+00000490: 0000 0000 0000 0000 7900 6302 0100 6303  ........y.c...c.
+000004a0: 7d05 7d04 7700 2907 4ee9 0300 0000 e902  }.}.w.).N.......
+000004b0: 0000 0029 03e9 ff00 0000 720f 0000 0072  ...)......r....r
+000004c0: 0f00 0000 2903 e932 0000 0072 1000 0000  ....)..2...r....
+000004d0: 7210 0000 00e9 ffff ffff 5429 1fda 0670  r.........T)...p
+000004e0: 7967 616d 65da 0469 6e69 7472 0900 0000  ygame..initr....
+000004f0: da0a 7669 7369 6269 6c69 7479 720a 0000  ..visibilityr...
+00000500: 00da 046d 6174 68da 0473 7172 74da 0a68  ...math..sqrt..h
+00000510: 6578 615f 7261 7469 6fda 0369 6e74 da0d  exa_ratio..int..
+00000520: 7363 7265 656e 5f68 6569 6768 7472 0b00  screen_heightr..
+00000530: 0000 da0d 7363 7265 656e 5f6f 6666 7365  ....screen_offse
+00000540: 74da 0b73 6372 6565 6e5f 7369 7a65 da07  t..screen_size..
+00000550: 6469 7370 6c61 79da 0873 6574 5f6d 6f64  display..set_mod
+00000560: 65da 0673 6372 6565 6eda 0b61 7265 6e61  e..screen..arena
+00000570: 5f63 6f6c 6f72 da0f 6f63 636c 7573 696f  _color..occlusio
+00000580: 6e5f 636f 6c6f 72da 037a 6970 da06 6167  n_color..zip..ag
+00000590: 656e 7473 da04 6b65 7973 7206 0000 00da  ents..keysr.....
+000005a0: 036c 656e da0c 6167 656e 745f 636f 6c6f  .len..agent_colo
+000005b0: 7273 da04 7469 6d65 da05 436c 6f63 6bda  rs..time..Clock.
+000005c0: 0563 6c6f 636b da11 6167 656e 745f 7065  .clock..agent_pe
+000005d0: 7273 7065 6374 6976 65da 0c73 686f 775f  rspective..show_
+000005e0: 7370 7269 7465 73da 0674 6172 6765 74da  sprites..target.
+000005f0: 0d73 6372 6565 6e5f 7461 7267 6574 2906  .screen_target).
+00000600: da04 7365 6c66 7209 0000 0072 0a00 0000  ..selfr....r....
+00000610: 720b 0000 00da 0a61 6765 6e74 5f6e 616d  r......agent_nam
+00000620: 65da 0563 6f6c 6f72 7306 0000 0020 2020  e..colors....   
+00000630: 2020 20fa 3143 3a5c 7265 7365 6172 6368     .1C:\research
+00000640: 5c63 656c 6c77 6f72 6c64 5f67 616d 655c  \cellworld_game\
+00000650: 6365 6c6c 776f 726c 645f 6761 6d65 5c76  cellworld_game\v
+00000660: 6965 772e 7079 da08 5f5f 696e 6974 5f5f  iew.py..__init__
+00000670: 7a0d 5669 6577 2e5f 5f69 6e69 745f 5f09  z.View.__init__.
+00000680: 0000 0073 4a01 0000 8000 f408 0009 0f8f  ...sJ...........
+00000690: 0b89 0b8c 0dd8 151a 8804 8c0a d81a 1fd7  ................
+000006a0: 1a2a d11a 2a88 048c 0fd8 1c28 8804 d408  .*..*......(....
+000006b0: 19dc 1b1f 9f39 9939 a051 9b3c a821 d11b  .....9.9.Q.<.!..
+000006c0: 2b88 048c 0fdc 1d20 a014 a71f a11f b03c  +...... .......<
+000006d0: d121 3fd3 1d40 8804 d408 1ad8 161c 8804  .!?..@..........
+000006e0: 8c0b d81e 22d7 1e2f d11e 2fb0 24d7 3244  ...."../../.$.2D
+000006f0: d132 44d1 1e44 c801 d11d 4988 04d4 081a  .2D..D....I.....
+00000700: d81c 28a8 24d7 2a3c d12a 3cd0 1b3d 8804  ..(.$.*<.*<..=..
+00000710: d408 18dc 161c 976e 916e d716 2dd1 162d  .......n.n..-..-
+00000720: a864 d72e 3ed1 2e3e d316 3f88 048c 0bd8  .d..>..>..?.....
+00000730: 1b2a 8804 d408 18d8 1f2b 8804 d408 1ce4  .*.......+......
+00000740: 3235 b064 b76a b16a d736 47d1 3647 d736  25.d.j.j.6G.6G.6
+00000750: 4cd1 364c d336 4edc 364e cc73 d053 57d7  L.6L.6N.6N.s.SW.
+00000760: 535d d153 5dd7 5364 d153 64d3 4f65 d336  S].S].Sd.Sd.Oe.6
+00000770: 66f3 0301 3368 01f7 0302 1d69 01d1 3344  f...3h.....i..3D
+00000780: b03a b875 985a a815 d11d 2ef3 0002 1d69  .:.u.Z.........i
+00000790: 0188 04d4 0819 f406 0016 1c97 5b91 5bd7  ............[.[.
+000007a0: 1526 d115 26d3 1528 8804 8c0a d821 2388  .&..&..(.....!#.
+000007b0: 04d4 081e d81c 2088 04d4 0819 d816 1a88  ...... .........
+000007c0: 048c 0bd8 1d21 8804 d508 1af9 f30f 021d  .....!..........
+000007d0: 6901 7306 0000 00c4 3c0d 4612 06da 0963  i.s.....<.F....c
+000007e0: 616e 6f6e 6963 616c 6302 0000 0000 0000  anonicalc.......
+000007f0: 0000 0000 0002 0000 0003 0000 00f3 c800  ................
+00000800: 0000 9700 7c01 5c02 0000 7d02 7d03 7c02  ....|.\...}.}.|.
+00000810: 7c00 6a00 0000 0000 0000 0000 0000 0000  |.j.............
+00000820: 0000 0000 0000 7a05 0000 7d04 7c00 6a02  ......z...}.|.j.
+00000830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000840: 0000 7223 6401 7c03 7a0a 0000 7c00 6a00  ..r#d.|.z...|.j.
+00000850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000860: 0000 7a05 0000 7c00 6a04 0000 0000 0000  ..z...|.j.......
+00000870: 0000 0000 0000 0000 0000 0000 7a0a 0000  ............z...
+00000880: 7d05 7c04 7c05 6602 5300 7c03 7c00 6a00  }.|.|.f.S.|.|.j.
+00000890: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000008a0: 0000 7a05 0000 7c00 6a04 0000 0000 0000  ..z...|.j.......
+000008b0: 0000 0000 0000 0000 0000 0000 7a0a 0000  ............z...
+000008c0: 7d05 7c04 7c05 6602 5300 2902 4e72 0300  }.|.|.f.S.).Nr..
+000008d0: 0000 2903 720a 0000 0072 0b00 0000 721a  ..).r....r....r.
+000008e0: 0000 0029 0672 2d00 0000 7232 0000 00da  ...).r-...r2....
+000008f0: 0b63 616e 6f6e 6963 616c 5f78 da0b 6361  .canonical_x..ca
+00000900: 6e6f 6e69 6361 6c5f 79da 0873 6372 6565  nonical_y..scree
+00000910: 6e5f 78da 0873 6372 6565 6e5f 7973 0600  n_x..screen_ys..
+00000920: 0000 2020 2020 2020 7230 0000 00da 0e66  ..      r0.....f
+00000930: 726f 6d5f 6361 6e6f 6e69 6361 6c7a 1356  rom_canonicalz.V
+00000940: 6965 772e 6672 6f6d 5f63 616e 6f6e 6963  iew.from_canonic
+00000950: 616c 2200 0000 7377 0000 0080 00d8 232c  al"...sw......#,
+00000960: d108 2088 0b90 5bd8 131e a014 d721 32d1  .. ...[......!2.
+00000970: 2132 d113 3288 08d8 0b0f 8f3b 8a3b d818  !2..2......;.;..
+00000980: 1998 2b99 0da8 14d7 293a d129 3ad1 173a  ..+.....):.):..:
+00000990: b854 d73d 4fd1 3d4f d117 4f88 48f0 0600  .T.=O.=O..O.H...
+000009a0: 1018 9818 d00f 21d0 0821 f003 0018 23a0  ......!..!....#.
+000009b0: 54d7 2536 d125 36d1 1736 b814 d739 4bd1  T.%6.%6..6...9K.
+000009c0: 394b d117 4b88 48d8 0f17 9818 d00f 21d0  9K..K.H.......!.
+000009d0: 0821 f300 0000 0072 3600 0000 7237 0000  .!.....r6...r7..
+000009e0: 0063 0300 0000 0000 0000 0000 0000 0200  .c..............
+000009f0: 0000 0300 0000 f398 0000 0097 007c 006a  .............|.j
+00000a00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000a10: 0000 007c 027a 0a00 007c 006a 0200 0000  ...|.z...|.j....
+00000a20: 0000 0000 0000 0000 0000 0000 0000 007a  ...............z
+00000a30: 0000 007d 037c 037c 006a 0000 0000 0000  ...}.|.|.j......
+00000a40: 0000 0000 0000 0000 0000 0000 007a 0b00  .............z..
+00000a50: 007c 006a 0400 0000 0000 0000 0000 0000  .|.j............
+00000a60: 0000 0000 0000 007a 0500 007d 047c 017c  .......z...}.|.|
+00000a70: 006a 0600 0000 0000 0000 0000 0000 0000  .j..............
+00000a80: 0000 0000 007a 0b00 007d 057c 057c 0466  .....z...}.|.|.f
+00000a90: 0253 0029 014e 2904 7219 0000 0072 1a00  .S.).N).r....r..
+00000aa0: 0000 7217 0000 0072 0a00 0000 2906 722d  ..r....r....).r-
+00000ab0: 0000 0072 3600 0000 7237 0000 00da 0179  ...r6...r7.....y
+00000ac0: 7235 0000 0072 3400 0000 7306 0000 0020  r5...r4...s.... 
+00000ad0: 2020 2020 2072 3000 0000 da0c 746f 5f63       r0.....to_c
+00000ae0: 616e 6f6e 6963 616c 7a11 5669 6577 2e74  anonicalz.View.t
+00000af0: 6f5f 6361 6e6f 6e69 6361 6c2b 0000 0073  o_canonical+...s
+00000b00: 5100 0000 8000 d80c 10d7 0c1e d10c 1ea0  Q...............
+00000b10: 18d1 0c29 a844 d72c 3ed1 2c3e d10c 3e88  ...).D.,>.,>..>.
+00000b20: 01d8 1617 9824 d71a 2cd1 1a2c d116 2ca8  .....$..,..,..,.
+00000b30: 74af 7fa9 7fd1 163e 880b d816 1ea0 14d7  t......>........
+00000b40: 2132 d121 32d1 1632 880b d80f 1a98 4bd0  !2.!2..2......K.
+00000b50: 0f27 d008 2772 3900 0000 6303 0000 0000  .'..'r9...c.....
+00000b60: 0000 0000 0000 000a 0000 0003 0000 00f3  ................
+00000b70: c600 0000 9700 7400 0000 0000 0000 0000  ......t.........
+00000b80: 6a02 0000 0000 0000 0000 0000 0000 0000  j...............
+00000b90: 0000 0000 6a05 0000 0000 0000 0000 0000  ....j...........
+00000ba0: 0000 0000 0000 0000 7c00 6a06 0000 0000  ........|.j.....
+00000bb0: 0000 0000 0000 0000 0000 0000 0000 7c02  ..............|.
+00000bc0: 7c01 6a08 0000 0000 0000 0000 0000 0000  |.j.............
+00000bd0: 0000 0000 0000 6a0a 0000 0000 0000 0000  ......j.........
+00000be0: 0000 0000 0000 0000 0000 4400 8f03 6302  ..........D...c.
+00000bf0: 6700 6302 5d13 0000 7d03 7c00 6a0d 0000  g.c.]...}.|.j...
+00000c00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000c10: 7c03 ab01 0000 0000 0000 9102 8c15 0400  |...............
+00000c20: 6302 7d03 ab03 0000 0000 0000 0100 7901  c.}...........y.
+00000c30: 6302 0100 6302 7d03 7700 2902 fa33 4472  c...c.}.w.)..3Dr
+00000c40: 6177 7320 6120 6865 7861 676f 6e20 6174  aws a hexagon at
+00000c50: 2074 6865 2073 7065 6369 6669 6564 2070   the specified p
+00000c60: 6f73 6974 696f 6e20 616e 6420 7369 7a65  osition and size
+00000c70: 2e4e 2907 7212 0000 00da 0464 7261 77da  .N).r......draw.
+00000c80: 0770 6f6c 7967 6f6e 721e 0000 00da 0865  .polygonr......e
+00000c90: 7874 6572 696f 72da 0663 6f6f 7264 7372  xterior..coordsr
+00000ca0: 3800 0000 2904 722d 0000 0072 4000 0000  8...).r-...r@...
+00000cb0: 722f 0000 00da 0570 6f69 6e74 7304 0000  r/.....points...
+00000cc0: 0020 2020 2072 3000 0000 da0c 6472 6177  .    r0.....draw
+00000cd0: 5f70 6f6c 7967 6f6e 7a11 5669 6577 2e64  _polygonz.View.d
+00000ce0: 7261 775f 706f 6c79 676f 6e31 0000 0073  raw_polygon1...s
+00000cf0: 4600 0000 8000 e408 0e8f 0b89 0bd7 081b  F...............
+00000d00: d108 1b98 449f 4b99 4bd8 1c21 d845 4cd7  ....D.K.K..!.EL.
+00000d10: 4555 d145 55d7 455c d145 5cd6 1c5d b845  EU.EU.E\.E\..].E
+00000d20: 9854 d71d 30d1 1d30 b015 d51d 37d2 1c5d  .T..0..0....7..]
+00000d30: f505 0209 5f01 f9e2 1c5d 7305 0000 00be  ...._....]s.....
+00000d40: 1841 1e0c 6304 0000 0000 0000 0000 0000  .A..c...........
+00000d50: 0008 0000 0003 0000 00f3 b400 0000 9700  ................
+00000d60: 7c01 6a00 0000 0000 0000 0000 0000 0000  |.j.............
+00000d70: 0000 0000 0000 6a02 0000 0000 0000 0000  ......j.........
+00000d80: 0000 0000 0000 0000 0000 4400 5d3f 0000  ..........D.]?..
+00000d90: 7d04 7404 0000 0000 0000 0000 6a06 0000  }.t.........j...
+00000da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000db0: 6a09 0000 0000 0000 0000 0000 0000 0000  j...............
+00000dc0: 0000 0000 7c00 6a0a 0000 0000 0000 0000  ....|.j.........
+00000dd0: 0000 0000 0000 0000 0000 7c02 7c00 6a0d  ..........|.|.j.
+00000de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000df0: 0000 7c04 ab01 0000 0000 0000 7c03 6401  ..|.........|.d.
+00000e00: ac02 ab05 0000 0000 0000 0100 8c41 0400  .............A..
+00000e10: 7903 a904 723e 0000 0072 0e00 0000 a905  y...r>...r......
+00000e20: da07 7375 7266 6163 6572 2f00 0000 da06  ..surfacer/.....
+00000e30: 6365 6e74 6572 da06 7261 6469 7573 da05  center..radius..
+00000e40: 7769 6474 684e 2907 7241 0000 0072 4200  widthN).rA...rB.
+00000e50: 0000 7212 0000 0072 3f00 0000 da06 6369  ..r....r?.....ci
+00000e60: 7263 6c65 721e 0000 0072 3800 0000 2905  rcler....r8...).
+00000e70: 722d 0000 0072 4000 0000 722f 0000 00da  r-...r@...r/....
+00000e80: 0473 697a 6572 4300 0000 7305 0000 0020  .sizerC...s.... 
+00000e90: 2020 2020 7230 0000 00da 1564 7261 775f      r0.....draw_
+00000ea0: 706f 6c79 676f 6e5f 7665 7274 6963 6573  polygon_vertices
+00000eb0: 7a1a 5669 6577 2e64 7261 775f 706f 6c79  z.View.draw_poly
+00000ec0: 676f 6e5f 7665 7274 6963 6573 3700 0000  gon_vertices7...
+00000ed0: 7351 0000 0080 00e0 151c d715 25d1 1525  sQ..........%..%
+00000ee0: d715 2cd1 152c f200 0509 2888 45dc 0c12  ..,..,....(.E...
+00000ef0: 8f4b 894b d70c 1ed1 0c1e a074 a77b a17b  .K.K.......t.{.{
+00000f00: d825 2ad8 262a d726 39d1 2639 b825 d326  .%*.&*.&9.&9.%.&
+00000f10: 40d8 262a d825 26f0 0900 0d1f f500 040d  @.&*.%&.........
+00000f20: 28f1 0305 0928 7239 0000 0063 0400 0000  (....(r9...c....
+00000f30: 0000 0000 0000 0000 0900 0000 0300 0000  ................
+00000f40: f3b8 0000 0097 007c 0144 005d 5500 007d  .......|.D.]U..}
+00000f50: 0474 0000 0000 0000 0000 006a 0200 0000  .t.........j....
+00000f60: 0000 0000 0000 0000 0000 0000 0000 006a  ...............j
+00000f70: 0500 0000 0000 0000 0000 0000 0000 0000  ................
+00000f80: 0000 007c 006a 0600 0000 0000 0000 0000  ...|.j..........
+00000f90: 0000 0000 0000 0000 007c 027c 006a 0900  .........|.|.j..
+00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000fb0: 007c 046a 0a00 0000 0000 0000 0000 0000  .|.j............
+00000fc0: 0000 0000 0000 007c 046a 0c00 0000 0000  .......|.j......
+00000fd0: 0000 0000 0000 0000 0000 0000 0066 02ab  .............f..
+00000fe0: 0100 0000 0000 007c 0364 01ac 02ab 0500  .......|.d......
+00000ff0: 0000 0000 0001 008c 5704 0079 0372 4600  ........W..y.rF.
+00001000: 0000 2907 7212 0000 0072 3f00 0000 724c  ..).r....r?...rL
+00001010: 0000 0072 1e00 0000 7238 0000 00da 0178  ...r....r8.....x
+00001020: 723b 0000 0029 0572 2d00 0000 da06 706f  r;...).r-.....po
+00001030: 696e 7473 722f 0000 0072 4d00 0000 7243  intsr/...rM...rC
+00001040: 0000 0073 0500 0000 2020 2020 2072 3000  ...s....     r0.
+00001050: 0000 da0b 6472 6177 5f70 6f69 6e74 737a  ....draw_pointsz
+00001060: 1056 6965 772e 6472 6177 5f70 6f69 6e74  .View.draw_point
+00001070: 7340 0000 0073 5200 0000 8000 e015 1bf2  s@...sR.........
+00001080: 0005 0928 8845 dc0c 128f 4b89 4bd7 0c1e  ...(.E....K.K...
+00001090: d10c 1ea0 74a7 7ba1 7bd8 252a d826 2ad7  ....t.{.{.%*.&*.
+000010a0: 2639 d126 39b8 35bf 37b9 37c0 45c7 47c1  &9.&9.5.7.7.E.G.
+000010b0: 47d0 3a4c d326 4dd8 262a d825 26f0 0900  G.:L.&M.&*.%&...
+000010c0: 0d1f f500 040d 28f1 0305 0928 7239 0000  ......(....(r9..
+000010d0: 00da 0561 6765 6e74 6302 0000 0000 0000  ...agentc.......
+000010e0: 0000 0000 0007 0000 0003 0000 00f3 ee00  ................
+000010f0: 0000 9700 7c01 6a01 0000 0000 0000 0000  ....|.j.........
+00001100: 0000 0000 0000 0000 0000 ab00 0000 0000  ................
+00001110: 0000 7d02 7c02 6a03 0000 0000 0000 0000  ..}.|.j.........
+00001120: 0000 0000 0000 0000 0000 ab00 0000 0000  ................
+00001130: 0000 5c02 0000 7d03 7d04 7c00 6a05 0000  ..\...}.}.|.j...
+00001140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001150: 7c01 6a06 0000 0000 0000 0000 0000 0000  |.j.............
+00001160: 0000 0000 0000 6a08 0000 0000 0000 0000  ......j.........
+00001170: 0000 0000 0000 0000 0000 ab01 0000 0000  ................
+00001180: 0000 5c02 0000 7d05 7d06 7c00 6a0a 0000  ..\...}.}.|.j...
+00001190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000011a0: 6a0d 0000 0000 0000 0000 0000 0000 0000  j...............
+000011b0: 0000 0000 7c02 7c05 7c03 6401 7a0b 0000  ....|.|.|.d.z...
+000011c0: 7a0a 0000 7c06 7c04 6401 7a0b 0000 7a0a  z...|.|.d.z...z.
+000011d0: 0000 6602 ab02 0000 0000 0000 0100 7900  ..f...........y.
+000011e0: 2902 4e72 0e00 0000 2907 da0a 6765 745f  ).Nr....)...get_
+000011f0: 7370 7269 7465 da08 6765 745f 7369 7a65  sprite..get_size
+00001200: 7238 0000 00da 0573 7461 7465 da08 6c6f  r8.....state..lo
+00001210: 6361 7469 6f6e 721e 0000 00da 0462 6c69  cationr......bli
+00001220: 7429 0772 2d00 0000 7253 0000 00da 0c61  t).r-...rS.....a
+00001230: 6765 6e74 5f73 7072 6974 6572 4b00 0000  gent_spriterK...
+00001240: da06 6865 6967 6874 7236 0000 0072 3700  ..heightr6...r7.
+00001250: 0000 7307 0000 0020 2020 2020 2020 7230  ..s....       r0
+00001260: 0000 00da 0a64 7261 775f 6167 656e 747a  .....draw_agentz
+00001270: 0f56 6965 772e 6472 6177 5f61 6765 6e74  .View.draw_agent
+00001280: 4900 0000 736d 0000 0080 00d8 272c d727  I...sm......',.'
+00001290: 37d1 2737 d327 3988 0cd8 1824 d718 2dd1  7.'7.'9....$..-.
+000012a0: 182d d318 2f89 0d88 0588 76d8 1d21 d71d  .-../.....v..!..
+000012b0: 30d1 1d30 b015 b71b b11b d731 45d1 3145  0..0.......1E.1E
+000012c0: d31d 46d1 081a 8808 9028 d808 0c8f 0b89  ..F......(......
+000012d0: 0bd7 0818 d108 1898 1ca8 08b0 35b8 31b1  ............5.1.
+000012e0: 39d1 283c b868 c816 d052 53c9 1ad1 3e53  9.(<.h...RS...>S
+000012f0: d027 54d5 0855 7239 0000 0063 0100 0000  .'T..Ur9...c....
+00001300: 0000 0000 0000 0000 0900 0000 0300 0000  ................
+00001310: f34e 0c00 0097 007c 006a 0000 0000 0000  .N.....|.j......
+00001320: 0000 0000 0000 0000 0000 0000 006a 0300  .............j..
+00001330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001340: 0064 01ab 0100 0000 0000 0001 007c 006a  .d...........|.j
+00001350: 0500 0000 0000 0000 0000 0000 0000 0000  ................
+00001360: 0000 007c 006a 0600 0000 0000 0000 0000  ...|.j..........
+00001370: 0000 0000 0000 0000 006a 0800 0000 0000  .........j......
+00001380: 0000 0000 0000 0000 0000 0000 007c 006a  .............|.j
+00001390: 0a00 0000 0000 0000 0000 0000 0000 0000  ................
+000013a0: 0000 00ab 0200 0000 0000 0001 007c 006a  .............|.j
+000013b0: 0c00 0000 0000 0000 0000 0000 0000 0000  ................
+000013c0: 0000 0064 026b 3700 0072 a474 0f00 0000  ...d.k7..r.t....
+000013d0: 0000 0000 007c 006a 0600 0000 0000 0000  .....|.j........
+000013e0: 0000 0000 0000 0000 0000 006a 1000 0000  ...........j....
+000013f0: 0000 0000 0000 0000 0000 0000 0000 006a  ...............j
+00001400: 1300 0000 0000 0000 0000 0000 0000 0000  ................
+00001410: 0000 00ab 0000 0000 0000 00ab 0100 0000  ................
+00001420: 0000 007c 006a 0c00 0000 0000 0000 0000  ...|.j..........
+00001430: 0000 0000 0000 0000 0019 0000 007d 017c  .............}.|
+00001440: 006a 0600 0000 0000 0000 0000 0000 0000  .j..............
+00001450: 0000 0000 006a 1000 0000 0000 0000 0000  .....j..........
+00001460: 0000 0000 0000 0000 007c 0119 0000 006a  .........|.....j
+00001470: 1400 0000 0000 0000 0000 0000 0000 0000  ................
+00001480: 0000 007d 027c 006a 1600 0000 0000 0000  ...}.|.j........
+00001490: 0000 0000 0000 0000 0000 006a 1900 0000  ...........j....
+000014a0: 0000 0000 0000 0000 0000 0000 0000 007c  ...............|
+000014b0: 026a 1a00 0000 0000 0000 0000 0000 0000  .j..............
+000014c0: 0000 0000 007c 026a 1c00 0000 0000 0000  .....|.j........
+000014d0: 0000 0000 0000 0000 0000 0064 03ac 04ab  ...........d....
+000014e0: 0300 0000 0000 005c 0200 007d 037d 047c  .......\...}.}.|
+000014f0: 006a 0500 0000 0000 0000 0000 0000 0000  .j..............
+00001500: 0000 0000 007c 0364 05ab 0200 0000 0000  .....|.d........
+00001510: 0001 007c 006a 0600 0000 0000 0000 0000  ...|.j..........
+00001520: 0000 0000 0000 0000 006a 1e00 0000 0000  .........j......
+00001530: 0000 0000 0000 0000 0000 0000 0044 005d  .............D.]
+00001540: 1e00 007d 057c 006a 0500 0000 0000 0000  ...}.|.j........
+00001550: 0000 0000 0000 0000 0000 007c 057c 006a  ...........|.|.j
+00001560: 2000 0000 0000 0000 0000 0000 0000 0000   ...............
+00001570: 0000 00ab 0200 0000 0000 0001 008c 2004  .............. .
+00001580: 0064 067c 006a 0600 0000 0000 0000 0000  .d.|.j..........
+00001590: 0000 0000 0000 0000 006a 1000 0000 0000  .........j......
+000015a0: 0000 0000 0000 0000 0000 0000 0076 0090  .............v..
+000015b0: 0272 5d7c 006a 0600 0000 0000 0000 0000  .r]|.j..........
+000015c0: 0000 0000 0000 0000 006a 1000 0000 0000  .........j......
+000015d0: 0000 0000 0000 0000 0000 0000 0064 0619  .............d..
+000015e0: 0000 006a 2200 0000 0000 0000 0000 0000  ...j"...........
+000015f0: 0000 0000 0000 0090 0272 397c 006a 0600  .........r9|.j..
+00001600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001610: 006a 1000 0000 0000 0000 0000 0000 0000  .j..............
+00001620: 0000 0000 0064 0619 0000 006a 1400 0000  .....d.....j....
+00001630: 0000 0000 0000 0000 0000 0000 0000 006a  ...............j
+00001640: 1a00 0000 0000 0000 0000 0000 0000 0000  ................
+00001650: 0000 007d 067c 006a 0600 0000 0000 0000  ...}.|.j........
+00001660: 0000 0000 0000 0000 0000 006a 1000 0000  ...........j....
+00001670: 0000 0000 0000 0000 0000 0000 0000 0064  ...............d
+00001680: 0619 0000 006a 2200 0000 0000 0000 0000  .....j".........
+00001690: 0000 0000 0000 0000 0044 005d 8c00 007d  .........D.]...}
+000016a0: 0774 2400 0000 0000 0000 006a 2600 0000  .t$........j&...
+000016b0: 0000 0000 0000 0000 0000 0000 0000 006a  ...............j
+000016c0: 2900 0000 0000 0000 0000 0000 0000 0000  )...............
+000016d0: 0000 007c 006a 0000 0000 0000 0000 0000  ...|.j..........
+000016e0: 0000 0000 0000 0000 0064 077c 006a 2b00  .........d.|.j+.
+000016f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001700: 007c 06ab 0100 0000 0000 007c 006a 2b00  .|.........|.j+.
+00001710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001720: 007c 07ab 0100 0000 0000 0064 08ab 0500  .|.........d....
+00001730: 0000 0000 0001 0074 2400 0000 0000 0000  .......t$.......
+00001740: 006a 2600 0000 0000 0000 0000 0000 0000  .j&.............
+00001750: 0000 0000 006a 2d00 0000 0000 0000 0000  .....j-.........
+00001760: 0000 0000 0000 0000 007c 006a 0000 0000  .........|.j....
+00001770: 0000 0000 0000 0000 0000 0000 0000 0064  ...............d
+00001780: 097c 006a 2b00 0000 0000 0000 0000 0000  .|.j+...........
+00001790: 0000 0000 0000 007c 07ab 0100 0000 0000  .......|........
+000017a0: 0064 0a64 08ac 0bab 0500 0000 0000 0001  .d.d............
+000017b0: 007c 077d 068c 8e04 0064 0c7c 006a 0600  .|.}.....d.|.j..
 000017c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000017d0: 00ab 0000 0000 0000 0001 007c 006a 0400  ...........|.j..
-000017e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000017f0: 0072 107c 006a 0500 0000 0000 0000 0000  .r.|.j..........
-00001800: 0000 0000 0000 0000 00ab 0000 0000 0000  ................
-00001810: 0001 0064 017c 005f 0300 0000 0000 0000  ...d.|._........
-00001820: 0079 0029 024e 5429 0472 6000 0000 da05  .y.).NT).r`.....
-00001830: 636c 6561 7272 5b00 0000 7262 0000 0072  clearr[...rb...r
-00001840: 3a00 0000 7301 0000 0020 7218 0000 00da  :...s.... r.....
-00001850: 0572 6573 6574 7a0b 4167 656e 742e 7265  .resetz.Agent.re
-00001860: 7365 746c 0000 0073 2900 0000 8000 d808  setl...s).......
-00001870: 0c8f 0f89 0fd7 081d d108 1dd4 081f d80b  ................
-00001880: 0f8f 3d8a 3dd8 0c10 8f4d 894d 8c4f d817  ..=.=....M.M.O..
-00001890: 1b88 048d 0c72 1a00 0000 6301 0000 0000  .....r....c.....
-000018a0: 0000 0000 0000 0002 0000 0003 0000 00f3  ................
-000018b0: 3e00 0000 9700 7c00 6a00 0000 0000 0000  >.....|.j.......
-000018c0: 0000 0000 0000 0000 0000 0000 7211 7c00  ............r.|.
-000018d0: 6a01 0000 0000 0000 0000 0000 0000 0000  j...............
-000018e0: 0000 0000 ab00 0000 0000 0000 0100 7900  ..............y.
-000018f0: 7900 7226 0000 0029 0172 5d00 0000 723a  y.r&...).r]...r:
-00001900: 0000 0073 0100 0000 2072 1800 0000 7240  ...s.... r....r@
-00001910: 0000 007a 0b41 6765 6e74 2e73 7461 7274  ...z.Agent.start
-00001920: 7200 0000 7317 0000 0080 00d8 0b0f 8f3d  r...s..........=
-00001930: 8a3d d80c 108f 4d89 4d8d 4ff0 0300 0c19  .=....M.M.O.....
-00001940: 721a 0000 0072 4b00 0000 6302 0000 0000  r....rK...c.....
-00001950: 0000 0000 0000 0003 0000 0003 0000 00f3  ................
-00001960: 4000 0000 9700 7c00 6a00 0000 0000 0000  @.....|.j.......
-00001970: 0000 0000 0000 0000 0000 0000 7212 7c00  ............r.|.
-00001980: 6a01 0000 0000 0000 0000 0000 0000 0000  j...............
-00001990: 0000 0000 7c01 ab01 0000 0000 0000 0100  ....|...........
-000019a0: 7900 7900 7226 0000 0029 0172 5c00 0000  y.y.r&...).r\...
-000019b0: 724d 0000 0073 0200 0000 2020 7218 0000  rM...s....  r...
-000019c0: 00da 0473 7465 707a 0a41 6765 6e74 2e73  ...stepz.Agent.s
-000019d0: 7465 7076 0000 0073 1a00 0000 8000 d80b  tepv...s........
-000019e0: 0f8f 3c8a 3cd8 0c10 8f4c 894c 9817 d50c  ..<.<....L.L....
-000019f0: 21f0 0300 0c18 721a 0000 0063 0000 0000  !.....r....c....
-00001a00: 0000 0000 0000 0000 0500 0000 0300 0000  ................
-00001a10: f3aa 0000 0097 0074 0000 0000 0000 0000  .......t........
-00001a20: 006a 0200 0000 0000 0000 0000 0000 0000  .j..............
-00001a30: 0000 0000 006a 0500 0000 0000 0000 0000  .....j..........
-00001a40: 0000 0000 0000 0000 0074 0700 0000 0000  .........t......
-00001a50: 0000 006a 0800 0000 0000 0000 0000 0000  ...j............
-00001a60: 0000 0000 0000 0064 01ab 0100 0000 0000  .......d........
-00001a70: 00ab 0100 0000 0000 007d 0074 0000 0000  .........}.t....
-00001a80: 0000 0000 006a 0a00 0000 0000 0000 0000  .....j..........
-00001a90: 0000 0000 0000 0000 006a 0d00 0000 0000  .........j......
-00001aa0: 0000 0000 0000 0000 0000 0000 007c 0064  .............|.d
-00001ab0: 02ab 0200 0000 0000 007d 017c 0153 0029  .........}.|.S.)
-00001ac0: 034e 7a09 6167 656e 742e 706e 67e9 5a00  .Nz.agent.png.Z.
-00001ad0: 0000 2907 7265 0000 00da 0569 6d61 6765  ..).re.....image
-00001ae0: da04 6c6f 6164 7204 0000 00da 0466 696c  ..loadr......fil
-00001af0: 6572 6600 0000 7208 0000 0029 0272 5a00  erf...r....).rZ.
-00001b00: 0000 da0e 726f 7461 7465 645f 7370 7269  ....rotated_spri
-00001b10: 7465 7302 0000 0020 2072 1800 0000 7268  tes....  r....rh
-00001b20: 0000 007a 1341 6765 6e74 2e63 7265 6174  ...z.Agent.creat
-00001b30: 655f 7370 7269 7465 7a00 0000 733d 0000  e_spritez...s=..
-00001b40: 0080 00e4 1117 971c 911c d711 22d1 1122  ............".."
-00001b50: a439 a73e a13e b02b d323 3ed3 113f 8806  .9.>.>.+.#>..?..
-00001b60: dc19 1fd7 1929 d119 29d7 1930 d119 30b0  .....)..)..0..0.
-00001b70: 16b8 12d3 193c 880e d80f 1dd0 081d 721a  .....<........r.
-00001b80: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00001b90: 0500 0000 0300 0000 f31c 0000 0097 0074  ...............t
-00001ba0: 0100 0000 0000 0000 0064 0164 0264 03ab  .........d.d.d..
-00001bb0: 0300 0000 0000 0053 0029 044e 7243 0000  .......S.).NrC..
-00001bc0: 0067 9a99 9999 9999 a93f e91e 0000 0029  .g.......?.....)
-00001bd0: 0172 0500 0000 7232 0000 0072 1a00 0000  .r....r2...r....
-00001be0: 7218 0000 0072 5800 0000 7a14 4167 656e  r....rX...z.Agen
-00001bf0: 742e 6372 6561 7465 5f70 6f6c 7967 6f6e  t.create_polygon
-00001c00: 8000 0000 7311 0000 0080 00e4 0f1d 9866  ....s..........f
-00001c10: a063 a832 d30f 2ed0 082e 721a 0000 0063  .c.2......r....c
-00001c20: 0200 0000 0000 0000 0000 0000 0600 0000  ................
-00001c30: 0300 0000 f3ec 0000 0097 007c 0172 1c7c  ...........|.r.|
-00001c40: 016a 0000 0000 0000 0000 0000 0000 0000  .j..............
-00001c50: 0000 0000 005c 0200 007d 027d 037c 016a  .....\...}.}.|.j
-00001c60: 0200 0000 0000 0000 0000 0000 0000 0000  ................
-00001c70: 0000 007d 046e 2f7c 006a 0400 0000 0000  ...}.n/|.j......
-00001c80: 0000 0000 0000 0000 0000 0000 006a 0000  .............j..
-00001c90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ca0: 005c 0200 007d 027d 037c 006a 0400 0000  .\...}.}.|.j....
-00001cb0: 0000 0000 0000 0000 0000 0000 0000 006a  ...............j
-00001cc0: 0200 0000 0000 0000 0000 0000 0000 0000  ................
-00001cd0: 0000 007d 0474 0700 0000 0000 0000 007c  ...}.t.........|
-00001ce0: 006a 0800 0000 0000 0000 0000 0000 0000  .j..............
-00001cf0: 0000 0000 007c 0464 0164 02ac 03ab 0400  .....|.d.d......
-00001d00: 0000 0000 007d 0574 0b00 0000 0000 0000  .....}.t........
-00001d10: 007c 057c 027c 03ab 0300 0000 0000 007d  .|.|.|.........}
-00001d20: 067c 0653 0029 044e 7243 0000 0046 2902  .|.S.).NrC...F).
-00001d30: da06 6f72 6967 696e da0b 7573 655f 7261  ..origin..use_ra
-00001d40: 6469 616e 7329 0672 3500 0000 7236 0000  dians).r5...r6..
-00001d50: 0072 5600 0000 7208 0000 0072 5900 0000  .rV...r....rY...
-00001d60: 7209 0000 0029 0772 1700 0000 726a 0000  r....).r....rj..
-00001d70: 00da 0178 7227 0000 0072 3600 0000 da0f  ...xr'...r6.....
-00001d80: 726f 7461 7465 645f 706f 6c79 676f 6eda  rotated_polygon.
-00001d90: 1274 7261 6e73 6c61 7465 645f 706f 6c79  .translated_poly
-00001da0: 676f 6e73 0700 0000 2020 2020 2020 2072  gons....       r
-00001db0: 1800 0000 da0b 6765 745f 706f 6c79 676f  ......get_polygo
-00001dc0: 6e7a 1141 6765 6e74 2e67 6574 5f70 6f6c  nz.Agent.get_pol
-00001dd0: 7967 6f6e 8400 0000 736f 0000 0080 00f1  ygon....so......
-00001de0: 0600 0c11 d813 1897 3e91 3e89 4488 4188  ........>.>.D.A.
-00001df0: 71d8 181d 9f0f 990f 8949 e013 1797 3b91  q........I....;.
-00001e00: 3bd7 1327 d113 2789 4488 4188 71d8 181c  ;..'..'.D.A.q...
-00001e10: 9f0b 990b d718 2dd1 182d 8849 dc1a 20a0  ......-..-.I.. .
-00001e20: 14a7 1ca1 1cd8 212a d828 2ed8 2d32 f407  ......!*.(..-2..
-00001e30: 031b 3488 0ff4 0800 1e27 a07f b801 b831  ..4......'.....1
-00001e40: d31d 3dd0 081a d80f 21d0 0821 721a 0000  ..=.....!..!r...
-00001e50: 0063 0100 0000 0000 0000 0000 0000 0400  .c..............
-00001e60: 0000 0300 0000 f382 0000 0097 0074 0000  .............t..
-00001e70: 0000 0000 0000 006a 0200 0000 0000 0000  .......j........
-00001e80: 0000 0000 0000 0000 0000 006a 0500 0000  ...........j....
-00001e90: 0000 0000 0000 0000 0000 0000 0000 007c  ...............|
-00001ea0: 006a 0600 0000 0000 0000 0000 0000 0000  .j..............
-00001eb0: 0000 0000 007c 006a 0800 0000 0000 0000  .....|.j........
-00001ec0: 0000 0000 0000 0000 0000 006a 0a00 0000  ...........j....
-00001ed0: 0000 0000 0000 0000 0000 0000 0000 00ab  ................
-00001ee0: 0200 0000 0000 007d 017c 0153 0072 2600  .......}.|.S.r&.
-00001ef0: 0000 2906 7265 0000 0072 6600 0000 7208  ..).re...rf...r.
-00001f00: 0000 0072 5a00 0000 7256 0000 0072 3600  ...rZ...rV...r6.
-00001f10: 0000 2902 7217 0000 0072 7a00 0000 7302  ..).r....rz...s.
-00001f20: 0000 0020 2072 1800 0000 da0a 6765 745f  ...  r......get_
-00001f30: 7370 7269 7465 7a10 4167 656e 742e 6765  spritez.Agent.ge
-00001f40: 745f 7370 7269 7465 9400 0000 732e 0000  t_sprite....s...
-00001f50: 0080 00dc 191f d719 29d1 1929 d719 30d1  ........)..)..0.
-00001f60: 1930 b014 b71b b11b b864 bf6b b96b d73e  .0.......d.k.k.>
-00001f70: 53d1 3e53 d319 5488 0ed8 0f1d d008 1d72  S.>S..T........r
-00001f80: 1a00 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00001f90: 0003 0000 0003 0000 00f3 6800 0000 9700  ..........h.....
-00001fa0: 7c00 6a00 0000 0000 0000 0000 0000 0000  |.j.............
-00001fb0: 0000 0000 0000 7226 7c00 6a00 0000 0000  ......r&|.j.....
-00001fc0: 0000 0000 0000 0000 0000 0000 0000 6a03  ..............j.
-00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001fe0: 0000 7c00 6a04 0000 0000 0000 0000 0000  ..|.j...........
-00001ff0: 0000 0000 0000 0000 ac01 ab01 0000 0000  ................
-00002000: 0000 5300 7900 2902 4e29 01da 0a61 6765  ..S.y.).N)...age
-00002010: 6e74 5f6e 616d 6529 0372 5f00 0000 da0f  nt_name).r_.....
-00002020: 6765 745f 6f62 7365 7276 6174 696f 6e72  get_observationr
-00002030: 5e00 0000 723a 0000 0073 0100 0000 2072  ^...r:...s.... r
-00002040: 1800 0000 7288 0000 007a 1541 6765 6e74  ....r....z.Agent
-00002050: 2e67 6574 5f6f 6273 6572 7661 7469 6f6e  .get_observation
-00002060: 9800 0000 7328 0000 0080 00d8 0b0f 8f3a  ....s(.........:
-00002070: 8a3a d813 1797 3a91 3ad7 132d d113 2db8  .:....:.:..-..-.
-00002080: 14bf 19b9 19d0 132d d313 43d0 0c43 e013  .......-..C..C..
-00002090: 1772 1a00 0000 6301 0000 0000 0000 0000  .r....c.........
-000020a0: 0000 0006 0000 0003 0000 00f3 a800 0000  ................
-000020b0: 9700 6900 7d01 6401 7d02 7c00 6a00 0000  ..i.}.d.}.|.j...
-000020c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000020d0: 6401 1900 0000 7d03 7c00 6a00 0000 0000  d.....}.|.j.....
-000020e0: 0000 0000 0000 0000 0000 0000 0000 6402  ..............d.
-000020f0: 6400 1a00 4400 5d27 0000 7d04 7c02 7403  d...D.]'..}.|.t.
-00002100: 0000 0000 0000 0000 7c03 6a04 0000 0000  ........|.j.....
-00002110: 0000 0000 0000 0000 0000 0000 0000 7c04  ..............|.
-00002120: 6a04 0000 0000 0000 0000 0000 0000 0000  j...............
-00002130: 0000 0000 ab02 0000 0000 0000 7a0d 0000  ............z...
-00002140: 7d02 7c04 7d03 8c29 0400 7c02 7c01 6403  }.|.}..)..|.|.d.
-00002150: 3c00 0000 7c01 5300 2904 4e72 0200 0000  <...|.S.).Nr....
-00002160: 7203 0000 0072 0700 0000 2903 7260 0000  r....r....).r`..
-00002170: 0072 0700 0000 7235 0000 0029 0572 1700  .r....r5...).r..
-00002180: 0000 da05 7374 6174 73da 0464 6973 74da  ....stats..dist.
-00002190: 0a70 7265 765f 7374 6174 6572 6a00 0000  .prev_staterj...
-000021a0: 7305 0000 0020 2020 2020 7218 0000 00da  s....     r.....
-000021b0: 0967 6574 5f73 7461 7473 7a0f 4167 656e  .get_statsz.Agen
-000021c0: 742e 6765 745f 7374 6174 739e 0000 0073  t.get_stats....s
-000021d0: 6500 0000 8000 d810 1288 05d8 0f10 8804  e...............
-000021e0: d815 1997 5f91 5fa0 51d1 1527 880a d815  ...._._.Q..'....
-000021f0: 1997 5f91 5fa0 51a0 52d0 1528 f200 0209  .._._.Q.R..(....
-00002200: 1f88 45d8 0c10 9448 985a d71d 30d1 1d30  ..E....H.Z..0..0
-00002210: b025 b72e b12e d314 41d1 0c41 8844 d819  .%......A..A.D..
-00002220: 1e89 4af0 0502 091f f006 001d 2188 0588  ..J.........!...
-00002230: 6ad1 0819 d80f 1488 0c72 1a00 0000 da07  j........r......
-00002240: 7375 7266 6163 6572 6100 0000 6303 0000  surfacera...c...
-00002250: 0000 0000 0000 0000 0007 0000 0003 0000  ................
-00002260: 00f3 da00 0000 9700 7c00 6a01 0000 0000  ........|.j.....
-00002270: 0000 0000 0000 0000 0000 0000 0000 ab00  ................
-00002280: 0000 0000 0000 7d03 7c03 6a03 0000 0000  ......}.|.j.....
-00002290: 0000 0000 0000 0000 0000 0000 0000 ab00  ................
-000022a0: 0000 0000 0000 5c02 0000 7d04 7d05 7c02  ......\...}.}.|.
-000022b0: 6a05 0000 0000 0000 0000 0000 0000 0000  j...............
-000022c0: 0000 0000 7c00 6a06 0000 0000 0000 0000  ....|.j.........
-000022d0: 0000 0000 0000 0000 0000 6a08 0000 0000  ..........j.....
-000022e0: 0000 0000 0000 0000 0000 0000 0000 ab01  ................
-000022f0: 0000 0000 0000 5c02 0000 7d06 7d07 7c01  ......\...}.}.|.
-00002300: 6a0b 0000 0000 0000 0000 0000 0000 0000  j...............
-00002310: 0000 0000 7c03 7c06 7c04 6401 7a0b 0000  ....|.|.|.d.z...
-00002320: 7a0a 0000 7c07 7c05 6401 7a0b 0000 7a0a  z...|.|.d.z...z.
-00002330: 0000 6602 ab02 0000 0000 0000 0100 7900  ..f...........y.
-00002340: 2902 4e72 0f00 0000 2906 7285 0000 00da  ).Nr....).r.....
-00002350: 0867 6574 5f73 697a 6572 2300 0000 726a  .get_sizer#...rj
-00002360: 0000 0072 3500 0000 da04 626c 6974 2908  ...r5.....blit).
-00002370: 7217 0000 0072 8e00 0000 7261 0000 00da  r....r....ra....
-00002380: 0c61 6765 6e74 5f73 7072 6974 65da 0577  .agent_sprite..w
-00002390: 6964 7468 da06 6865 6967 6874 7221 0000  idth..heightr!..
-000023a0: 0072 2200 0000 7308 0000 0020 2020 2020  .r"...s....     
-000023b0: 2020 2072 1800 0000 da04 6472 6177 7a0a     r......drawz.
-000023c0: 4167 656e 742e 6472 6177 a800 0000 7366  Agent.draw....sf
-000023d0: 0000 0080 00f0 0600 282c a77f a17f d327  ........(,.....'
-000023e0: 3888 0cd8 1824 d718 2dd1 182d d318 2f89  8....$..-..-../.
-000023f0: 0d88 0588 76d8 1d31 d71d 40d1 1d40 c014  ....v..1..@..@..
-00002400: c71a c11a d741 54d1 4154 d31d 55d1 081a  .....AT.AT..U...
-00002410: 8808 9028 d808 0f8f 0c89 0c90 5ca0 48a8  ...(........\.H.
-00002420: 75b0 71a9 79d1 2438 b828 c056 c861 c15a  u.q.y.$8.(.V.a.Z
-00002430: d13a 4fd0 2350 d508 5172 1a00 0000 6302  .:O.#P..Qr....c.
-00002440: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00002450: 0000 00f3 1200 0000 9700 7c01 7c00 5f00  ..........|.|._.
-00002460: 0000 0000 0000 0000 7900 7226 0000 0029  ........y.r&...)
-00002470: 0172 6100 0000 2902 7217 0000 0072 6100  .ra...).r....ra.
-00002480: 0000 7302 0000 0020 2072 1800 0000 da18  ..s....  r......
-00002490: 7365 745f 636f 6f72 6469 6e61 7465 5f63  set_coordinate_c
-000024a0: 6f6e 7665 7274 6572 7a1e 4167 656e 742e  onverterz.Agent.
-000024b0: 7365 745f 636f 6f72 6469 6e61 7465 5f63  set_coordinate_c
-000024c0: 6f6e 7665 7274 6572 b000 0000 730a 0000  onverter....s...
-000024d0: 0080 00e0 2438 8804 d508 2172 1a00 0000  ....$8....!r....
-000024e0: 2902 e9b4 0000 0054 2902 723e 0000 004e  )......T).r>...N
-000024f0: 7226 0000 0029 1e72 2900 0000 722a 0000  r&...).r)...r*..
-00002500: 0072 2b00 0000 721e 0000 0072 2f00 0000  .r+...r....r/...
-00002510: 7219 0000 0072 3100 0000 7269 0000 0072  r....r1...ri...r
-00002520: 3400 0000 726d 0000 00da 0870 726f 7065  4...rm.....prope
-00002530: 7274 7972 6a00 0000 7271 0000 0072 4000  rtyrj...rq...r@.
-00002540: 0000 7274 0000 00da 0c73 7461 7469 636d  ..rt.....staticm
-00002550: 6574 686f 6472 6500 0000 da07 5375 7266  ethodre.....Surf
-00002560: 6163 6572 6800 0000 da02 7370 da07 506f  acerh.....sp..Po
-00002570: 6c79 676f 6e72 5800 0000 7283 0000 0072  lygonrX...r....r
-00002580: 8500 0000 da04 6469 6374 7288 0000 0072  ......dictr....r
-00002590: 8d00 0000 720b 0000 0072 9500 0000 7297  ....r....r....r.
-000025a0: 0000 0072 3200 0000 721a 0000 0072 1800  ...r2...r....r..
-000025b0: 0000 7250 0000 0072 5000 0000 4b00 0000  ..rP...rP...K...
-000025c0: 7325 0100 0084 00f0 0600 2629 d823 27f1  s%........&).#'.
-000025d0: 0512 051d d81d 22f0 0312 051d e01c 20f3  ......"....... .
-000025e0: 0512 051d f028 0105 4901 a045 f300 0105  .....(..I..E....
-000025f0: 4901 f006 0205 1c98 7af0 0002 051c a864  I.......z......d
-00002600: f300 0205 1cf0 0800 060e f002 0105 1b90  ................
-00002610: 7af2 0001 051b f303 0006 0ef0 0201 051b  z...............
-00002620: f306 0405 1cf3 0c02 051c f008 0205 2298  ..............".
-00002630: 45f0 0002 0522 a064 f300 0205 22f0 0800  E....".d...."...
-00002640: 0612 f002 0305 1e98 369f 3e99 3ef2 0003  ........6.>.>...
-00002650: 051e f303 0006 12f0 0203 051e f00a 0006  ................
-00002660: 12f0 0201 052f 9842 9f4a 994a f200 0105  ...../.B.J.J....
-00002670: 2ff3 0300 0612 f002 0105 2ff0 0800 292d  /........./...)-
-00002680: f103 0e05 22d8 1b25 f003 0e05 22d8 3133  ...."..%....".13
-00002690: b71a b11a f303 0e05 22f0 2002 051e 9846  ........". ....F
-000026a0: 9f4e 994e f300 0205 1ef0 0804 0518 a014  .N.N............
-000026b0: f300 0405 18f0 0c08 0515 9834 f300 0805  ...........4....
-000026c0: 15f0 1406 0552 01d8 161c 976e 916e f003  .....R.....n.n..
-000026d0: 0605 5201 e023 36f3 0506 0552 01f0 1002  ..R..#6....R....
-000026e0: 0539 d837 4af4 0302 0539 721a 0000 0072  .9.7J....9r....r
-000026f0: 5000 0000 2913 7214 0000 0072 2c00 0000  P...).r....r,...
-00002700: 7265 0000 00da 0773 6861 7065 6c79 729c  re.....shapelyr.
-00002710: 0000 00da 0972 6573 6f75 7263 6573 7204  .....resourcesr.
-00002720: 0000 00da 0475 7469 6c72 0500 0000 7206  .....utilr....r.
-00002730: 0000 0072 0700 0000 da10 7368 6170 656c  ...r......shapel
-00002740: 792e 6166 6669 6e69 7479 7208 0000 0072  y.affinityr....r
-00002750: 0900 0000 da06 6f62 6a65 6374 720b 0000  ......objectr...
-00002760: 0072 3400 0000 7245 0000 0072 5000 0000  .r4...rE...rP...
-00002770: 7232 0000 0072 1a00 0000 7218 0000 00fa  r2...r....r.....
-00002780: 083c 6d6f 6475 6c65 3e72 a400 0000 0100  .<module>r......
-00002790: 0000 7352 0000 00f0 0301 0101 db00 0bdb  ..sR............
-000027a0: 000d db00 0ddb 0014 dd00 20df 0036 d100  .......... ..6..
-000027b0: 36df 002e f406 1e01 2898 26f4 001e 0128  6.......(.&....(
-000027c0: f442 0110 0133 9016 f400 1001 33f4 260a  .B...3......3.&.
-000027d0: 0148 0190 46f4 000a 0148 01f4 1a67 0101  .H..F....H...g..
-000027e0: 3988 46f5 0067 0101 3972 1a00 0000       9.F..g..9r....
+000017d0: 006a 1000 0000 0000 0000 0000 0000 0000  .j..............
+000017e0: 0000 0000 0076 0090 0172 417c 006a 2b00  .....v...rA|.j+.
+000017f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001800: 007c 006a 0600 0000 0000 0000 0000 0000  .|.j............
+00001810: 0000 0000 0000 006a 1000 0000 0000 0000  .......j........
+00001820: 0000 0000 0000 0000 0000 0064 0619 0000  ...........d....
+00001830: 006a 1400 0000 0000 0000 0000 0000 0000  .j..............
+00001840: 0000 0000 006a 1a00 0000 0000 0000 0000  .....j..........
+00001850: 0000 0000 0000 0000 00ab 0100 0000 0000  ................
+00001860: 007d 087c 006a 0600 0000 0000 0000 0000  .}.|.j..........
+00001870: 0000 0000 0000 0000 006a 1000 0000 0000  .........j......
+00001880: 0000 0000 0000 0000 0000 0000 0064 0c19  .............d..
+00001890: 0000 006a 2e00 0000 0000 0000 0000 0000  ...j............
+000018a0: 0000 0000 0000 007c 006a 3000 0000 0000  .......|.j0.....
+000018b0: 0000 0000 0000 0000 0000 0000 007a 0500  .............z..
+000018c0: 007d 097c 0864 0d19 0000 007c 097a 0a00  .}.|.d.....|.z..
+000018d0: 007c 0864 0e19 0000 007c 097a 0a00 0066  .|.d.....|.z...f
+000018e0: 027d 0a74 2500 0000 0000 0000 006a 3200  .}.t%........j2.
+000018f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001900: 007c 0964 087a 0500 007c 0964 087a 0500  .|.d.z...|.d.z..
+00001910: 0066 0274 2400 0000 0000 0000 006a 3400  .f.t$........j4.
+00001920: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001930: 00ab 0200 0000 0000 007d 0b7c 006a 0600  .........}.|.j..
+00001940: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001950: 006a 1000 0000 0000 0000 0000 0000 0000  .j..............
+00001960: 0000 0000 0064 0c19 0000 006a 3600 0000  .....d.....j6...
+00001970: 0000 0000 0000 0000 0000 0000 0000 0064  ...............d
+00001980: 0d6b 4400 0072 0264 0f6e 0164 107d 0c74  .kD..r.d.n.d.}.t
+00001990: 2400 0000 0000 0000 006a 2600 0000 0000  $........j&.....
+000019a0: 0000 0000 0000 0000 0000 0000 006a 2d00  .............j-.
+000019b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000019c0: 007c 0b7c 0c7c 097c 0966 027c 09ac 11ab  .|.|.|.|.f.|....
+000019d0: 0400 0000 0000 0001 007c 006a 0000 0000  .........|.j....
+000019e0: 0000 0000 0000 0000 0000 0000 0000 006a  ...............j
+000019f0: 3900 0000 0000 0000 0000 0000 0000 0000  9...............
+00001a00: 0000 007c 0b7c 0aab 0200 0000 0000 0001  ...|.|..........
+00001a10: 0074 2400 0000 0000 0000 006a 2600 0000  .t$........j&...
+00001a20: 0000 0000 0000 0000 0000 0000 0000 006a  ...............j
+00001a30: 2d00 0000 0000 0000 0000 0000 0000 0000  -...............
+00001a40: 0000 007c 006a 0000 0000 0000 0000 0000  ...|.j..........
+00001a50: 0000 0000 0000 0000 0064 097c 087c 0964  .........d.|.|.d
+00001a60: 08ac 0bab 0500 0000 0000 0001 0074 3b00  .............t;.
+00001a70: 0000 0000 0000 007c 006a 0600 0000 0000  .......|.j......
+00001a80: 0000 0000 0000 0000 0000 0000 006a 1000  .............j..
+00001a90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001aa0: 006a 3d00 0000 0000 0000 0000 0000 0000  .j=.............
+00001ab0: 0000 0000 00ab 0000 0000 0000 007c 006a  .............|.j
+00001ac0: 3e00 0000 0000 0000 0000 0000 0000 0000  >...............
+00001ad0: 0000 00ab 0200 0000 0000 0044 005d 6c00  ...........D.]l.
+00001ae0: 005c 0200 005c 0200 007d 0d7d 0e7d 0f7c  .\...\...}.}.}.|
+00001af0: 006a 4000 0000 0000 0000 0000 0000 0000  .j@.............
+00001b00: 0000 0000 0072 137c 006a 4300 0000 0000  .....r.|.jC.....
+00001b10: 0000 0000 0000 0000 0000 0000 007c 0eac  .............|..
+00001b20: 12ab 0100 0000 0000 0001 008c 287c 006a  ............(|.j
+00001b30: 0500 0000 0000 0000 0000 0000 0000 0000  ................
+00001b40: 0000 007c 006a 0600 0000 0000 0000 0000  ...|.j..........
+00001b50: 0000 0000 0000 0000 006a 1000 0000 0000  .........j......
+00001b60: 0000 0000 0000 0000 0000 0000 007c 0d19  .............|..
+00001b70: 0000 006a 4500 0000 0000 0000 0000 0000  ...jE...........
+00001b80: 0000 0000 0000 00ab 0000 0000 0000 007c  ...............|
+00001b90: 006a 3e00 0000 0000 0000 0000 0000 0000  .j>.............
+00001ba0: 0000 0000 007c 0d19 0000 00ac 13ab 0200  .....|..........
+00001bb0: 0000 0000 0001 008c 6e04 007c 006a 4600  ........n..|.jF.
+00001bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001bd0: 0072 3874 2400 0000 0000 0000 006a 2600  .r8t$........j&.
+00001be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001bf0: 006a 2d00 0000 0000 0000 0000 0000 0000  .j-.............
+00001c00: 0000 0000 007c 006a 0000 0000 0000 0000  .....|.j........
+00001c10: 0000 0000 0000 0000 0000 0064 147c 006a  ...........d.|.j
+00001c20: 4600 0000 0000 0000 0000 0000 0000 0000  F...............
+00001c30: 0000 0064 1564 08ac 0bab 0500 0000 0000  ...d.d..........
+00001c40: 0001 0074 2400 0000 0000 0000 006a 4800  ...t$........jH.
+00001c50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c60: 006a 4b00 0000 0000 0000 0000 0000 0000  .jK.............
+00001c70: 0000 0000 00ab 0000 0000 0000 0044 005d  .............D.]
+00001c80: b000 007d 107c 106a 4c00 0000 0000 0000  ...}.|.jL.......
+00001c90: 0000 0000 0000 0000 0000 0074 2400 0000  ...........t$...
+00001ca0: 0000 0000 006a 4e00 0000 0000 0000 0000  .....jN.........
+00001cb0: 0000 0000 0000 0000 006b 2800 0072 0264  .........k(..r.d
+00001cc0: 167d 117c 106a 4c00 0000 0000 0000 0000  .}.|.jL.........
+00001cd0: 0000 0000 0000 0000 0074 2400 0000 0000  .........t$.....
+00001ce0: 0000 006a 5000 0000 0000 0000 0000 0000  ...jP...........
+00001cf0: 0000 0000 0000 006b 2800 0073 018c 407c  .......k(..s..@|
+00001d00: 106a 5200 0000 0000 0000 0000 0000 0000  .jR.............
+00001d10: 0000 0000 0064 0e6b 2800 0073 018c 507c  .....d.k(..s..P|
+00001d20: 106a 5400 0000 0000 0000 0000 0000 0000  .jT.............
+00001d30: 0000 0000 005c 0200 007d 127d 137c 006a  .....\...}.}.|.j
+00001d40: 5700 0000 0000 0000 0000 0000 0000 0000  W...............
+00001d50: 0000 007c 127c 13ab 0200 0000 0000 007c  ...|.|.........|
+00001d60: 005f 2c00 0000 0000 0000 007c 127c 1366  ._,........|.|.f
+00001d70: 027c 005f 2300 0000 0000 0000 007c 006a  .|._#........|.j
+00001d80: 0600 0000 0000 0000 0000 0000 0000 0000  ................
+00001d90: 0000 006a 1000 0000 0000 0000 0000 0000  ...j............
+00001da0: 0000 0000 0000 0064 0619 0000 006a 5b00  .......d.....j[.
+00001db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001dc0: 007c 006a 5800 0000 0000 0000 0000 0000  .|.jX...........
+00001dd0: 0000 0000 0000 00ab 0100 0000 0000 0001  ................
+00001de0: 008c b204 0074 2400 0000 0000 0000 006a  .....t$........j
+00001df0: 5c00 0000 0000 0000 0000 0000 0000 0000  \...............
+00001e00: 0000 006a 5f00 0000 0000 0000 0000 0000  ...j_...........
+00001e10: 0000 0000 0000 00ab 0000 0000 0000 007d  ...............}
+00001e20: 147c 1474 2400 0000 0000 0000 006a 6000  .|.t$........j`.
+00001e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e40: 0019 0000 0072 0764 027c 005f 0600 0000  .....r.d.|._....
+00001e50: 0000 0000 007c 1474 2400 0000 0000 0000  .....|.t$.......
+00001e60: 006a 6200 0000 0000 0000 0000 0000 0000  .jb.............
+00001e70: 0000 0000 0019 0000 0072 0764 0d7c 005f  .........r.d.|._
+00001e80: 0600 0000 0000 0000 007c 1474 2400 0000  .........|.t$...
+00001e90: 0000 0000 006a 6400 0000 0000 0000 0000  .....jd.........
+00001ea0: 0000 0000 0000 0000 0019 0000 0072 0764  .............r.d
+00001eb0: 0e7c 005f 0600 0000 0000 0000 007c 1474  .|._.........|.t
+00001ec0: 2400 0000 0000 0000 006a 6600 0000 0000  $........jf.....
+00001ed0: 0000 0000 0000 0000 0000 0000 0019 0000  ................
+00001ee0: 0072 0764 167c 005f 2000 0000 0000 0000  .r.d.|._ .......
+00001ef0: 007c 1474 2400 0000 0000 0000 006a 6800  .|.t$........jh.
+00001f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f10: 0019 0000 0072 0764 177c 005f 2000 0000  .....r.d.|._ ...
+00001f20: 0000 0000 0074 2400 0000 0000 0000 006a  .....t$........j
+00001f30: 6a00 0000 0000 0000 0000 0000 0000 0000  j...............
+00001f40: 0000 006a 6d00 0000 0000 0000 0000 0000  ...jm...........
+00001f50: 0000 0000 0000 00ab 0000 0000 0000 0001  ................
+00001f60: 0079 0029 184e 2903 7202 0000 0072 0200  .y.).N).r....r..
+00001f70: 0000 7202 0000 0072 1100 0000 6968 0100  ..r....r....ih..
+00001f80: 0029 0372 5800 0000 da09 6469 7265 6374  .).rX.....direct
+00001f90: 696f 6eda 0a76 6965 775f 6669 656c 6429  ion..view_field)
+00001fa0: 03e9 b400 0000 7260 0000 0072 6000 0000  ......r`...r`...
+00001fb0: da08 7072 6564 6174 6f72 2903 720f 0000  ..predator).r...
+00001fc0: 0072 0200 0000 7202 0000 0072 0e00 0000  .r....r....r....
+00001fd0: 2903 7202 0000 0072 0200 0000 720f 0000  ).r....r....r...
+00001fe0: 00e9 0500 0000 7247 0000 00da 0470 7265  ......rG.....pre
+00001ff0: 7972 0200 0000 7203 0000 0029 0472 0f00  yr....r....).r..
+00002000: 0000 7202 0000 0072 0200 0000 e93c 0000  ..r....r.....<..
+00002010: 0029 0472 0200 0000 7202 0000 0072 0f00  .).r....r....r..
+00002020: 0000 7264 0000 0029 0372 2f00 0000 7249  ..rd...).r/...rI
+00002030: 0000 0072 4a00 0000 2901 7253 0000 0029  ...rJ...).rS...)
+00002040: 0172 2f00 0000 2903 720f 0000 0072 0200  .r/...).r....r..
+00002050: 0000 720f 0000 0072 0d00 0000 4654 2937  ..r....r....FT)7
+00002060: 721e 0000 00da 0466 696c 6c72 4400 0000  r......fillrD...
+00002070: 7209 0000 00da 0561 7265 6e61 721f 0000  r......arenar...
+00002080: 0072 2900 0000 da04 6c69 7374 7222 0000  .r).....listr"..
+00002090: 0072 2300 0000 7257 0000 0072 1400 0000  .r#...rW...r....
+000020a0: da16 6765 745f 7669 7369 6269 6c69 7479  ..get_visibility
+000020b0: 5f70 6f6c 7967 6f6e 7258 0000 0072 5e00  _polygonrX...r^.
+000020c0: 0000 da0a 6f63 636c 7573 696f 6e73 7220  ....occlusionsr 
+000020d0: 0000 00da 0470 6174 6872 1200 0000 723f  .....pathr....r?
+000020e0: 0000 00da 046c 696e 6572 3800 0000 724c  .....liner8...rL
+000020f0: 0000 00da 0e70 7566 665f 7468 7265 7368  .....puff_thresh
+00002100: 6f6c 6472 0a00 0000 da07 5375 7266 6163  oldr......Surfac
+00002110: 65da 0853 5243 414c 5048 41da 0e70 7566  e..SRCALPHA..puf
+00002120: 665f 636f 6f6c 5f64 6f77 6e72 5900 0000  f_cool_downrY...
+00002130: 7221 0000 00da 0569 7465 6d73 7225 0000  r!.....itemsr%..
+00002140: 0072 2a00 0000 725c 0000 00da 0b67 6574  .r*...r\.....get
+00002150: 5f70 6f6c 7967 6f6e 722c 0000 00da 0565  _polygonr,.....e
+00002160: 7665 6e74 da03 6765 74da 0474 7970 65da  vent..get..type.
+00002170: 0451 5549 54da 0f4d 4f55 5345 4255 5454  .QUIT..MOUSEBUTT
+00002180: 4f4e 444f 574e da06 6275 7474 6f6e da03  ONDOWN..button..
+00002190: 706f 7372 3c00 0000 722b 0000 00da 0f73  posr<...r+.....s
+000021a0: 6574 5f64 6573 7469 6e61 7469 6f6e da03  et_destination..
+000021b0: 6b65 79da 0b67 6574 5f70 7265 7373 6564  key..get_pressed
+000021c0: da03 4b5f 30da 034b 5f31 da03 4b5f 32da  ..K_0..K_1..K_2.
+000021d0: 034b 5f33 da03 4b5f 3472 1c00 0000 da04  .K_3..K_4r......
+000021e0: 666c 6970 2915 722d 0000 0072 2e00 0000  flip).r-...r....
+000021f0: da16 7669 7369 6269 6c69 7479 5f70 6572  ..visibility_per
+00002200: 7370 6563 7469 7665 da12 7669 7369 6269  spective..visibi
+00002210: 6c69 7479 5f70 6f6c 7967 6f6e da01 61da  lity_polygon..a.
+00002220: 096f 6363 6c75 7369 6f6e da0d 6375 7272  .occlusion..curr
+00002230: 656e 745f 706f 696e 74da 0473 7465 70da  ent_point..step.
+00002240: 1170 7265 6461 746f 725f 6c6f 6361 7469  .predator_locati
+00002250: 6f6e da0e 7075 6666 5f61 7265 615f 7369  on..puff_area_si
+00002260: 7a65 da0d 7075 6666 5f6c 6f63 6174 696f  ze..puff_locatio
+00002270: 6eda 1170 7566 665f 6172 6561 5f73 7572  n..puff_area_sur
+00002280: 6661 6365 da0f 7075 6666 5f61 7265 615f  face..puff_area_
+00002290: 636f 6c6f 72da 046e 616d 6572 5300 0000  color..namerS...
+000022a0: 722f 0000 0072 7200 0000 da07 7275 6e6e  r/...rr.....runn
+000022b0: 696e 6772 5000 0000 723b 0000 0072 2300  ingrP...r;...r#.
+000022c0: 0000 7315 0000 0020 2020 2020 2020 2020  ..s....         
+000022d0: 2020 2020 2020 2020 2020 2020 7230 0000              r0..
+000022e0: 0072 3f00 0000 7a09 5669 6577 2e64 7261  .r?...z.View.dra
+000022f0: 774f 0000 0073 1005 0000 8000 d808 0c8f  wO...s..........
+00002300: 0b89 0bd7 0818 d108 1898 19d4 0823 d808  .............#..
+00002310: 0cd7 0819 d108 1998 249f 2a99 2ad7 1a2a  ........$.*.*..*
+00002320: d11a 2aa8 44d7 2c3c d12c 3cd4 083d e00b  ..*.D.,<.,<..=..
+00002330: 0fd7 0b21 d10b 21a0 52d2 0b27 dc19 1d98  ...!..!.R..'....
+00002340: 649f 6a99 6ad7 1e2f d11e 2fd7 1e34 d11e  d.j.j../../..4..
+00002350: 34d3 1e36 d319 37b8 04d7 384e d138 4ed1  4..6..7...8N.8N.
+00002360: 194f 884a d825 29a7 5aa1 5ad7 2536 d125  .O.J.%).Z.Z.%6.%
+00002370: 36b0 7ad1 2542 d725 48d1 2548 d00c 22d8  6.z.%B.%H.%H..".
+00002380: 2428 a74f a14f d724 4ad1 244a d054 6ad7  $(.O.O.$J.$J.Tj.
+00002390: 5473 d154 73d8 556b d755 75d1 5575 d856  Ts.Ts.Uk.Uu.Uu.V
+000023a0: 59f0 0500 254b 01f3 0002 255b 01d1 0c21  Y...%K....%[...!
+000023b0: d00c 1ea0 01f0 0600 0d11 d70c 1dd1 0c1d  ................
+000023c0: d01e 30b0 2fd4 0c42 e019 1d9f 1a99 1ad7  ..0./..B........
+000023d0: 192e d119 2ef2 0001 093f 8849 d80c 10d7  .........?.I....
+000023e0: 0c1d d10c 1d98 69a8 14d7 293d d129 3dd5  ......i...)=.)=.
+000023f0: 0c3e f003 0109 3ff0 0600 0c16 9814 9f1a  .>....?.........
+00002400: 991a d719 2ad1 192a d20b 2aa8 74af 7aa9  ....*..*..*.t.z.
+00002410: 7ad7 2f40 d12f 40c0 1ad1 2f4c d72f 51d3  z./@./@.../L./Q.
+00002420: 2f51 d81c 209f 4a99 4ad7 1c2d d11c 2da8  /Q.. .J.J..-..-.
+00002430: 6ad1 1c39 d71c 3fd1 1c3f d71c 48d1 1c48  j..9..?..?..H..H
+00002440: 884d d818 1c9f 0a99 0ad7 1829 d118 29a8  .M.........)..).
+00002450: 2ad1 1835 d718 3ad1 183a f200 0b0d 2590  *..5..:..:....%.
+00002460: 04dc 1016 970b 910b d710 20d1 1020 a014  .......... .. ..
+00002470: a71b a11b d821 2cd8 2125 d721 34d1 2134  .....!,.!%.!4.!4
+00002480: b05d d321 43d8 2125 d721 34d1 2134 b054  .].!C.!%.!4.!4.T
+00002490: d321 3ad8 2122 f409 0411 24f4 0a00 1117  .!:.!"....$.....
+000024a0: 970b 910b d710 22d1 1022 a834 af3b a93b  ......"..".4.;.;
+000024b0: d829 34d8 2a2e d72a 3dd1 2a3d b864 d32a  .)4.*..*=.*=.d.*
+000024c0: 43d8 2a2b d829 2af0 0900 1123 f400 0411  C.*+.)*....#....
+000024d0: 2cf0 0a00 2125 910d f017 0b0d 25f0 1800  ,...!%......%...
+000024e0: 1016 9814 9f1a 991a d719 2ad1 192a d20f  ..........*..*..
+000024f0: 2ad8 2428 d724 37d1 2437 b804 bf0a b90a  *.$(.$7.$7......
+00002500: d738 49d1 3849 c82a d138 55d7 385b d138  .8I.8I.*.8U.8[.8
+00002510: 5bd7 3864 d138 64d3 2465 d010 21d8 2125  [.8d.8d.$e..!.!%
+00002520: a71a a11a d721 32d1 2132 b036 d121 3ad7  .....!2.!2.6.!:.
+00002530: 2149 d121 49c8 44d7 4c5d d14c 5dd1 215d  !I.!I.D.L].L].!]
+00002540: 900e d820 31b0 21d1 2034 b07e d120 45d0  ... 1.!. 4.~. E.
+00002550: 4859 d05a 5bd1 485c d05f 6dd1 486d d020  HY.Z[.H\._m.Hm. 
+00002560: 6d90 0ddc 242a a74e a14e b04e c051 d134  m...$*.N.N.N.Q.4
+00002570: 46c8 0ed0 595a d148 5ad0 335b d45d 63d7  F...YZ.HZ.3[.]c.
+00002580: 5d6c d15d 6cd3 246d d010 21d8 3539 b75a  ]l.]l.$m..!.59.Z
+00002590: b15a d735 46d1 3546 c076 d135 4ed7 355d  .Z.5F.5F.v.5N.5]
+000025a0: d135 5dd0 6061 d235 61a1 2fd0 6776 900f  .5].`a.5a./.gv..
+000025b0: dc10 1697 0b91 0bd7 1022 d110 22d0 2334  ........."..".#4
+000025c0: d829 38d8 2b39 b83e d02a 4ad8 2a38 f007  .)8.+9.>.*J.*8..
+000025d0: 0011 23f4 0003 113a f008 0011 1597 0b91  ..#....:........
+000025e0: 0bd7 1020 d110 20d0 2132 d821 2ef4 0301  ... .. .!2.!....
+000025f0: 1130 e410 1697 0b91 0bd7 1022 d110 22a8  .0........."..".
+00002600: 34af 3ba9 3bd8 2934 d82a 3bd8 2a38 d829  4.;.;.)4.*;.*8.)
+00002610: 2af0 0900 1123 f400 0411 2cf4 0e00 2528  *....#....,...%(
+00002620: a804 af0a a90a d728 39d1 2839 d728 3fd1  .......(9.(9.(?.
+00002630: 283f d328 41c0 34d7 4354 d143 54d3 2455  (?.(A.4.CT.CT.$U
+00002640: f200 0409 6801 d10c 2089 4d88 5490 3598  ....h... .M.T.5.
+00002650: 35d8 0f13 d70f 20d2 0f20 d810 1497 0f91  5..... .. ......
+00002660: 0fa0 6590 0fd5 102c e010 14d7 1021 d110  ..e....,.....!..
+00002670: 21a0 24a7 2aa1 2ad7 2233 d122 33b0 44d1  !.$.*.*."3."3.D.
+00002680: 2239 d722 45d1 2245 d322 47c8 74d7 4f60  "9."E."E."G.t.O`
+00002690: d14f 60d0 6165 d14f 66d0 1021 d510 67f0  .O`.ae.Of..!..g.
+000026a0: 0904 0968 01f0 0c00 0c10 d70b 1dd2 0b1d  ...h............
+000026b0: dc0c 128f 4b89 4bd7 0c1e d10c 1ea0 74a7  ....K.K.......t.
+000026c0: 7ba1 7bd8 2532 d826 2ad7 2638 d126 38d8  {.{.%2.&*.&8.&8.
+000026d0: 2627 d825 26f0 0900 0d1f f400 040d 28f4  &'.%&.........(.
+000026e0: 0c00 161c 975c 915c d715 25d1 1525 d315  .....\.\..%..%..
+000026f0: 27f2 0009 094f 0188 45d8 0f14 8f7a 897a  '....O..E....z.z
+00002700: 9c56 9f5b 995b d20f 28d8 1a1f 9007 e00f  .V.[.[..(.......
+00002710: 148f 7a89 7a9c 56d7 1d33 d11d 33d3 0f33  ..z.z.V..3..3..3
+00002720: d813 1897 3c91 3ca0 31d3 1324 d81b 209f  ....<.<.1..$.. .
+00002730: 3999 3991 4490 4190 71d8 2226 d722 33d1  9.9.D.A.q."&."3.
+00002740: 2233 b041 b071 d322 3990 4494 4bd8 2a2b  "3.A.q."9.D.K.*+
+00002750: a851 a816 9044 d414 26d8 1418 974a 914a  .Q...D..&....J.J
+00002760: d714 25d1 1425 a06a d114 31d7 1441 d114  ..%..%.j..1..A..
+00002770: 41c0 24c7 2bc1 2bd5 144e f013 0909 4f01  A.$.+.+..N....O.
+00002780: f418 0010 168f 7a89 7ad7 0f25 d10f 25d3  ......z.z..%..%.
+00002790: 0f27 8804 d80b 0f94 0697 0a91 0ad2 0b1b  .'..............
+000027a0: d825 2788 44d4 0c22 d80b 0f94 0697 0a91  .%'.D.."........
+000027b0: 0ad2 0b1b d825 2688 44d4 0c22 d80b 0f94  .....%&.D.."....
+000027c0: 0697 0a91 0ad2 0b1b d825 2688 44d4 0c22  .........%&.D.."
+000027d0: d80b 0f94 0697 0a91 0ad2 0b1b d820 2588  ............. %.
+000027e0: 44d4 0c1d d80b 0f94 0697 0a91 0ad2 0b1b  D...............
+000027f0: d820 2488 44d4 0c1d f41a 0009 0f8f 0e89  . $.D...........
+00002800: 0ed7 081b d108 1bd5 081d 7239 0000 004e  ..........r9...N
+00002810: 2902 6920 0300 0054 2901 720e 0000 0029  ).i ...T).r....)
+00002820: 10da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00002830: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00002840: 616d 655f 5f72 0400 0000 7218 0000 00da  ame__r....r.....
+00002850: 0462 6f6f 6c72 3100 0000 da05 7475 706c  .boolr1.....tupl
+00002860: 6572 3800 0000 723c 0000 0072 4400 0000  er8...r<...rD...
+00002870: 724e 0000 0072 5200 0000 7205 0000 0072  rN...rR...r....r
+00002880: 5c00 0000 723f 0000 00a9 0072 3900 0000  \...r?.....r9...
+00002890: 7230 0000 0072 0800 0000 7208 0000 0008  r0...r....r.....
+000028a0: 0000 0073 6c00 0000 8400 f006 0026 29d8  ...sl........&).
+000028b0: 2024 f107 1705 22d8 181d f003 1705 22e0   $....".......".
+000028c0: 1f22 f005 1705 22f0 0600 1a1e f307 1705  ."....".........
+000028d0: 22f0 3207 0522 a805 f300 0705 22f0 1204  ".2.."......"...
+000028e0: 0528 a053 f000 0405 28b0 43f3 0004 0528  .(.S....(.C....(
+000028f0: f20c 0405 5f01 f30c 0705 28f3 1207 0528  ...._.....(....(
+00002900: f012 0405 5601 a005 f300 0405 5601 f30c  ....V.......V...
+00002910: 6001 051e 7239 0000 0072 0800 0000 290a  `...r9...r....).
+00002920: 7212 0000 0072 0900 0000 7204 0000 0072  r....r....r....r
+00002930: 5300 0000 7205 0000 0072 1500 0000 da04  S...r....r......
+00002940: 7574 696c 7206 0000 00da 066f 626a 6563  utilr......objec
+00002950: 7472 0800 0000 7294 0000 0072 3900 0000  tr....r....r9...
+00002960: 7230 0000 00fa 083c 6d6f 6475 6c65 3e72  r0.....<module>r
+00002970: 9700 0000 0100 0000 7322 0000 00f0 0301  ........s"......
+00002980: 0101 db00 0ddd 0018 dd00 18db 000b dd00  ................
+00002990: 2af4 0667 0201 1e88 36f5 0067 0201 1e72  *..g....6..g...r
+000029a0: 3900 0000                                9...
```

### Comparing `cellworld_game-0.0.61/cellworld_game/__pycache__/cellworld_loader.cpython-312.pyc` & `cellworld_game-0.0.68/cellworld_game/__pycache__/cellworld_loader.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Thu Apr 25 23:24:36 2024 UTC, .py size: 3712 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-00000000: cb0d 0d0a 0000 0000 34e6 2a66 800e 0000  ........4.*f....
+00000000: cb0d 0d0a 0000 0000 85d2 1266 eb0d 0000  ...........f....
 00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
 00000020: 0000 0000 00f3 4000 0000 9700 6400 6401  ......@.....d.d.
 00000030: 6c00 5a00 6400 6401 6c01 5a02 6402 6403  l.Z.d.d.l.Z.d.d.
 00000040: 6c03 6d04 5a04 0100 6402 6404 6c05 6d06  l.m.Z...d.d.l.m.
 00000050: 5a06 0100 0200 4700 6405 8400 6406 ab02  Z.....G.d...d...
 00000060: 0000 0000 0000 5a07 7901 2907 e900 0000  ......Z.y.).....
 00000070: 004e e901 0000 0029 01da 0e63 7265 6174  .N.....)...creat
 00000080: 655f 6865 7861 676f 6e29 01da 0a4e 6176  e_hexagon)...Nav
 00000090: 6967 6174 696f 6e63 0000 0000 0000 0000  igationc........
 000000a0: 0000 0000 0200 0000 0000 0000 f318 0000  ................
 000000b0: 0097 0065 005a 0164 005a 0264 0165 0366  ...e.Z.d.Z.d.e.f
 000000c0: 0264 0284 045a 0479 0329 04da 0f43 656c  .d...Z.y.)...Cel
 000000d0: 6c57 6f72 6c64 4c6f 6164 6572 da0a 776f  lWorldLoader..wo
 000000e0: 726c 645f 6e61 6d65 6302 0000 0000 0000  rld_namec.......
-000000f0: 0000 0000 0009 0000 0003 0000 00f3 6c09  ..............l.
+000000f0: 0000 0000 0009 0000 0003 0000 00f3 4e09  ..............N.
 00000100: 0000 9700 7400 0000 0000 0000 0000 6a02  ....t.........j.
 00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000120: 0000 6a05 0000 0000 0000 0000 0000 0000  ..j.............
 00000130: 0000 0000 0000 6401 6402 7c01 ac03 ab03  ......d.d.|.....
 00000140: 0000 0000 0000 7c00 5f03 0000 0000 0000  ......|._.......
 00000150: 0000 7400 0000 0000 0000 0000 6a08 0000  ..t.........j...
 00000160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000170: 6a0b 0000 0000 0000 0000 0000 0000 0000  j...............
-00000180: 0000 0000 6401 7c01 ac04 ab02 0000 0000  ....d.|.........
+00000180: 0000 0000 6401 6404 ac05 ab02 0000 0000  ....d.d.........
 00000190: 0000 7d02 7401 0000 0000 0000 0000 6a0c  ..}.t.........j.
 000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001b0: 0000 7c02 7c00 6a06 0000 0000 0000 0000  ..|.|.j.........
-000001c0: 0000 0000 0000 0000 0000 ac05 ab02 0000  ................
+000001c0: 0000 0000 0000 0000 0000 ac06 ab02 0000  ................
 000001d0: 0000 0000 7d03 7401 0000 0000 0000 0000  ....}.t.........
 000001e0: 6a0e 0000 0000 0000 0000 0000 0000 0000  j...............
 000001f0: 0000 0000 7c00 6a06 0000 0000 0000 0000  ....|.j.........
 00000200: 0000 0000 0000 0000 0000 6a10 0000 0000  ..........j.....
 00000210: 0000 0000 0000 0000 0000 0000 0000 6a12  ..............j.
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000230: 0000 ab01 0000 0000 0000 7d04 7c00 6a06  ..........}.|.j.
@@ -61,15 +61,15 @@
 000003c0: 6a06 0000 0000 0000 0000 0000 0000 0000  j...............
 000003d0: 0000 0000 6a14 0000 0000 0000 0000 0000  ....j...........
 000003e0: 0000 0000 0000 0000 4400 5d5e 0000 7d08  ........D.]^..}.
 000003f0: 7c00 6a06 0000 0000 0000 0000 0000 0000  |.j.............
 00000400: 0000 0000 0000 6a14 0000 0000 0000 0000  ......j.........
 00000410: 0000 0000 0000 0000 0000 4400 5d43 0000  ..........D.]C..
 00000420: 7d09 7c03 6a25 0000 0000 0000 0000 0000  }.|.j%..........
-00000430: 0000 0000 0000 0000 7c08 7c09 ac06 ab02  ........|.|.....
+00000430: 0000 0000 0000 0000 7c08 7c09 ac07 ab02  ........|.|.....
 00000440: 0000 0000 0000 7d0a 7c04 7c08 6a26 0000  ......}.|.|.j&..
 00000450: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000460: 7c0a 7a00 0000 1900 0000 7d0b 7c0b 7c07  |.z.......}.|.|.
 00000470: 7c08 6a28 0000 0000 0000 0000 0000 0000  |.j(............
 00000480: 0000 0000 0000 1900 0000 7c09 6a28 0000  ..........|.j(..
 00000490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000004a0: 3c00 0000 8c45 0400 8c60 0400 7c07 7c00  <....E...`..|.|.
@@ -120,197 +120,192 @@
 00000770: 0000 0000 0000 0000 7c0e 6a3e 0000 0000  ........|.j>....
 00000780: 0000 0000 0000 0000 0000 0000 0000 7a00  ..............z.
 00000790: 0000 ab03 0000 0000 0000 9102 8c4a 0400  .............J..
 000007a0: 6302 7d0f 7c00 5f22 0000 0000 0000 0000  c.}.|._"........
 000007b0: 7400 0000 0000 0000 0000 6a46 0000 0000  t.........jF....
 000007c0: 0000 0000 0000 0000 0000 0000 0000 6a0b  ..............j.
 000007d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000007e0: 0000 6401 7c01 6407 ab03 0000 0000 0000  ..d.|.d.........
+000007e0: 0000 6401 7c01 6408 ab03 0000 0000 0000  ..d.|.d.........
 000007f0: 7d10 7c10 4400 8f11 6302 6700 6302 5d3c  }.|.D...c.g.c.]<
 00000800: 0000 7d11 7419 0000 0000 0000 0000 7c00  ..}.t.........|.
 00000810: 6a06 0000 0000 0000 0000 0000 0000 0000  j...............
 00000820: 0000 0000 6a14 0000 0000 0000 0000 0000  ....j...........
 00000830: 0000 0000 0000 0000 7c11 1900 0000 6a1a  ........|.....j.
 00000840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000850: 0000 6a1d 0000 0000 0000 0000 0000 0000  ..j.............
 00000860: 0000 0000 0000 ab00 0000 0000 0000 ab01  ................
 00000870: 0000 0000 0000 9102 8c3e 0400 6302 7d11  .........>..c.}.
 00000880: 7c00 5f24 0000 0000 0000 0000 7c00 6a2e  |._$........|.j.
 00000890: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000008a0: 0000 7c00 5f25 0000 0000 0000 0000 0900  ..|._%..........
-000008b0: 7400 0000 0000 0000 0000 6a46 0000 0000  t.........jF....
-000008c0: 0000 0000 0000 0000 0000 0000 0000 6a0b  ..............j.
+000008a0: 0000 7c00 5f25 0000 0000 0000 0000 7400  ..|._%........t.
+000008b0: 0000 0000 0000 0000 6a46 0000 0000 0000  ........jF......
+000008c0: 0000 0000 0000 0000 0000 0000 6a0b 0000  ............j...
 000008d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000008e0: 0000 6401 7c01 6408 ab03 0000 0000 0000  ..d.|.d.........
-000008f0: 7d12 7c12 4400 8f11 6302 6700 6302 5d3c  }.|.D...c.g.c.]<
-00000900: 0000 7d11 7419 0000 0000 0000 0000 7c00  ..}.t.........|.
-00000910: 6a06 0000 0000 0000 0000 0000 0000 0000  j...............
-00000920: 0000 0000 6a14 0000 0000 0000 0000 0000  ....j...........
-00000930: 0000 0000 0000 0000 7c11 1900 0000 6a1a  ........|.....j.
+000008e0: 6401 7c01 6409 ab03 0000 0000 0000 7d12  d.|.d.........}.
+000008f0: 7c12 4400 8f11 6302 6700 6302 5d3c 0000  |.D...c.g.c.]<..
+00000900: 7d11 7419 0000 0000 0000 0000 7c00 6a06  }.t.........|.j.
+00000910: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000920: 0000 6a14 0000 0000 0000 0000 0000 0000  ..j.............
+00000930: 0000 0000 0000 7c11 1900 0000 6a1a 0000  ......|.....j...
 00000940: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000950: 0000 6a1d 0000 0000 0000 0000 0000 0000  ..j.............
-00000960: 0000 0000 0000 ab00 0000 0000 0000 ab01  ................
-00000970: 0000 0000 0000 9102 8c3e 0400 6302 7d11  .........>..c.}.
-00000980: 7c00 5f26 0000 0000 0000 0000 7401 0000  |._&........t...
-00000990: 0000 0000 0000 6a4e 0000 0000 0000 0000  ......jN........
-000009a0: 0000 0000 0000 0000 0000 6409 6401 7c01  ..........d.d.|.
-000009b0: 640a ab04 0000 0000 0000 7d13 7451 0000  d.........}.tQ..
-000009c0: 0000 0000 0000 7c00 6a1e 0000 0000 0000  ......|.j.......
-000009d0: 0000 0000 0000 0000 0000 0000 7c00 6a2a  ............|.j*
+00000950: 6a1d 0000 0000 0000 0000 0000 0000 0000  j...............
+00000960: 0000 0000 ab00 0000 0000 0000 ab01 0000  ................
+00000970: 0000 0000 9102 8c3e 0400 6302 7d11 7c00  .......>..c.}.|.
+00000980: 5f26 0000 0000 0000 0000 7401 0000 0000  _&........t.....
+00000990: 0000 0000 6a4e 0000 0000 0000 0000 0000  ....jN..........
+000009a0: 0000 0000 0000 0000 640a 6401 7c01 640b  ........d.d.|.d.
+000009b0: ab04 0000 0000 0000 7d13 7451 0000 0000  ........}.tQ....
+000009c0: 0000 0000 7c00 6a1e 0000 0000 0000 0000  ....|.j.........
+000009d0: 0000 0000 0000 0000 0000 7c00 6a2a 0000  ..........|.j*..
 000009e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000009f0: 0000 7c13 ac0b ab03 0000 0000 0000 7c00  ..|...........|.
-00000a00: 5f29 0000 0000 0000 0000 7900 6302 0100  _)........y.c...
-00000a10: 6302 7d05 7700 6302 0100 6302 7d06 7700  c.}.w.c...c.}.w.
-00000a20: 6302 0100 6302 7d06 7700 6302 0100 6302  c...c.}.w.c...c.
-00000a30: 7d05 7700 6302 0100 6302 7d0f 7700 6302  }.w.c...c.}.w.c.
-00000a40: 0100 6302 7d11 7700 6302 0100 6302 7d11  ..c.}.w.c...c.}.
-00000a50: 7700 2300 0100 6700 7c00 5f26 0000 0000  w.#...g.|._&....
-00000a60: 0000 0000 5900 8c6e 7803 5900 7701 290c  ....Y..nx.Y.w.).
-00000a70: 4eda 0968 6578 6167 6f6e 616c da09 6361  N..hexagonal..ca
-00000a80: 6e6f 6e69 6361 6c29 03da 1877 6f72 6c64  nonical)...world
-00000a90: 5f63 6f6e 6669 6775 7261 7469 6f6e 5f6e  _configuration_n
-00000aa0: 616d 65da 1977 6f72 6c64 5f69 6d70 6c65  ame..world_imple
-00000ab0: 6d65 6e74 6174 696f 6e5f 6e61 6d65 da0f  mentation_name..
-00000ac0: 6f63 636c 7573 696f 6e73 5f6e 616d 6529  occlusions_name)
-00000ad0: 0272 0c00 0000 720e 0000 0029 02da 0762  .r....r....)...b
-00000ae0: 7569 6c64 6572 da05 776f 726c 6429 02da  uilder..world)..
-00000af0: 0873 7263 5f63 656c 6cda 0864 7374 5f63  .src_cell..dst_c
-00000b00: 656c 6cda 0f73 7061 776e 5f6c 6f63 6174  ell..spawn_locat
-00000b10: 696f 6e73 da04 6c70 706f da05 6772 6170  ions..lppo..grap
-00000b20: 68da 0f63 656c 6c5f 7669 7369 6269 6c69  h..cell_visibili
-00000b30: 7479 2903 da09 6c6f 6361 7469 6f6e 73da  ty)...locations.
-00000b40: 0570 6174 6873 da0a 7669 7369 6269 6c69  .paths..visibili
-00000b50: 7479 292a da02 6377 da05 576f 726c 64da  ty)*..cw..World.
-00000b60: 1967 6574 5f66 726f 6d5f 7061 7261 6d65  .get_from_parame
-00000b70: 7465 7273 5f6e 616d 6573 7210 0000 00da  ters_namesr.....
-00000b80: 0d50 6174 6873 5f62 7569 6c64 6572 da0d  .Paths_builder..
-00000b90: 6765 745f 6672 6f6d 5f6e 616d 65da 0550  get_from_name..P
-00000ba0: 6174 6873 da08 4365 6c6c 5f6d 6170 da0d  aths..Cell_map..
-00000bb0: 636f 6e66 6967 7572 6174 696f 6eda 1063  configuration..c
-00000bc0: 656c 6c5f 636f 6f72 6469 6e61 7465 73da  ell_coordinates.
-00000bd0: 0563 656c 6c73 da08 6f63 636c 7564 6564  .cells..occluded
-00000be0: da05 7475 706c 65da 086c 6f63 6174 696f  ..tuple..locatio
-00000bf0: 6eda 0a67 6574 5f76 616c 7565 7372 1700  n..get_valuesr..
-00000c00: 0000 da05 7261 6e67 65da 036c 656e da08  ....range..len..
-00000c10: 6765 745f 6d6f 7665 da0b 636f 6f72 6469  get_move..coordi
-00000c20: 6e61 7465 73da 0269 6472 1800 0000 da0a  nates..idr......
-00000c30: 6672 6565 5f63 656c 6c73 da0e 6f70 656e  free_cells..open
-00000c40: 5f6c 6f63 6174 696f 6e73 da0e 696d 706c  _locations..impl
-00000c50: 656d 656e 7461 7469 6f6e da05 7370 6163  ementation..spac
-00000c60: 65da 0663 656e 7465 72da 0e74 7261 6e73  e..center..trans
-00000c70: 666f 726d 6174 696f 6eda 1363 656c 6c5f  formation..cell_
-00000c80: 7472 616e 7366 6f72 6d61 7469 6f6e 7204  transformationr.
-00000c90: 0000 00da 0473 697a 65da 0872 6f74 6174  .....size..rotat
-00000ca0: 696f 6eda 0561 7265 6e61 da0e 6f63 636c  ion..arena..occl
-00000cb0: 7564 6564 5f63 656c 6c73 da0a 6f63 636c  uded_cells..occl
-00000cc0: 7573 696f 6e73 da12 4365 6c6c 5f67 726f  usions..Cell_gro
-00000cd0: 7570 5f62 7569 6c64 6572 da15 726f 626f  up_builder..robo
-00000ce0: 745f 7374 6172 745f 6c6f 6361 7469 6f6e  t_start_location
-00000cf0: 73da 1066 756c 6c5f 6163 7469 6f6e 5f6c  s..full_action_l
-00000d00: 6973 74da 1174 6c70 706f 5f61 6374 696f  ist..tlppo_actio
-00000d10: 6e5f 6c69 7374 da0c 6765 745f 7265 736f  n_list..get_reso
-00000d20: 7572 6365 7205 0000 00da 0a6e 6176 6967  urcer......navig
-00000d30: 6174 696f 6e29 14da 0473 656c 6672 0800  ation)...selfr..
-00000d40: 0000 da0d 7061 7468 735f 6275 696c 6465  ....paths_builde
-00000d50: 7272 1800 0000 da07 6365 6c6c 6d61 70da  rr......cellmap.
-00000d60: 0163 da01 5fda 0f6c 6f63 6174 696f 6e73  .c.._..locations
-00000d70: 5f70 6174 6873 7211 0000 0072 1200 0000  _pathsr....r....
-00000d80: da04 6d6f 7665 da0c 6e65 7874 5f73 7465  ..move..next_ste
-00000d90: 705f 6964 da0c 6172 656e 615f 6365 6e74  p_id..arena_cent
-00000da0: 6572 da14 6172 656e 615f 7472 616e 7366  er..arena_transf
-00000db0: 6f72 6d61 7469 6f6e 7233 0000 00da 0463  ormationr3.....c
-00000dc0: 656c 6cda 0b73 7061 776e 5f63 656c 6c73  ell..spawn_cells
-00000dd0: da02 7363 da0a 6c70 706f 5f63 656c 6c73  ..sc..lppo_cells
-00000de0: 7216 0000 0073 1400 0000 2020 2020 2020  r....s....      
-00000df0: 2020 2020 2020 2020 2020 2020 2020 fa3d                .=
-00000e00: 433a 5c52 6573 6561 7263 685c 6365 6c6c  C:\Research\cell
-00000e10: 776f 726c 645f 6761 6d65 5c63 656c 6c77  world_game\cellw
-00000e20: 6f72 6c64 5f67 616d 655c 6365 6c6c 776f  orld_game\cellwo
-00000e30: 726c 645f 6c6f 6164 6572 2e70 79da 085f  rld_loader.py.._
-00000e40: 5f69 6e69 745f 5f7a 1843 656c 6c57 6f72  _init__z.CellWor
-00000e50: 6c64 4c6f 6164 6572 2e5f 5f69 6e69 745f  ldLoader.__init_
-00000e60: 5f08 0000 0073 0b04 0000 8000 e415 1797  _....s..........
-00000e70: 5891 58d7 1537 d115 37d0 515c d852 5dd8  X.X..7..7.Q\.R].
-00000e80: 4852 f005 0016 38f3 0002 1654 0188 048c  HR....8....T....
-00000e90: 0af4 0600 191b d718 28d1 1828 d718 36d1  ........(..(..6.
-00000ea0: 1836 d050 5bd8 4751 f003 0019 37f3 0001  .6.P[.GQ....7...
-00000eb0: 1953 0188 0de4 1012 9708 9108 a01d b064  .S.............d
-00000ec0: b76a b16a d410 4188 05dc 1214 972b 912b  .j.j..A......+.+
-00000ed0: 9864 9f6a 996a d71e 36d1 1e36 d71e 47d1  .d.j.j..6..6..G.
-00000ee0: 1e47 d312 4888 07f0 0a00 5e01 6201 d75d  .G..H.....^.b..]
-00000ef0: 67d1 5d67 d75d 6dd1 5d6d f607 0354 016f  g.]g.]m.]m...T.o
-00000f00: 01f0 0600 5901 5a01 f005 0058 0159 01d7  ....Y.Z....X.Y..
-00000f10: 5761 d257 61f1 0300 5501 5901 e459 5ed0  Wa.Wa...U.Y..Y^.
-00000f20: 5f60 d75f 69d1 5f69 d75f 74d1 5f74 d35f  _`._i._i._t._t._
-00000f30: 76d3 5977 f105 0255 0178 01f2 0003 5401  v.Yw...U.x....T.
-00000f40: 6f01 8804 8c0e f40c 0056 015b 01d4 5b5e  o........V.[..[^
-00000f50: d05f 63d7 5f69 d15f 69d7 5f6f d15f 6fd3  ._c._i._i._o._o.
-00000f60: 5b70 d355 71f6 0301 4b01 7301 d850 51f4  [p.Uq...K.s..PQ.
-00000f70: 0300 5b01 6001 d460 63d0 6468 d764 6ed1  ..[.`..`c.dh.dn.
-00000f80: 646e d764 74d1 6474 d360 75d3 5a76 d64b  dn.dt.dt.`u.Zv.K
-00000f90: 77d0 5556 ca44 d44b 77f0 0001 4b01 7301  w.UV.D.Kw...K.s.
-00000fa0: 880f f000 014b 0173 01e0 181c 9f0a 990a  .....K.s........
-00000fb0: d718 28d1 1828 f200 0409 4901 8848 d81c  ..(..(....I..H..
-00000fc0: 209f 4a99 4ad7 1c2c d11c 2cf2 0003 0d49   .J.J..,..,....I
-00000fd0: 0190 08d8 171c 977e 917e a878 c028 907e  .......~.~.x.(.~
-00000fe0: d317 4b90 04d8 1f26 a078 d727 3bd1 273b  ..K....&.x.';.';
-00000ff0: b864 d127 42d1 1f43 900c d83c 4890 0fa0  .d.'B..C...<H...
-00001000: 08a7 0ba1 0bd1 102c a858 af5b a95b d210  .......,.X.[.[..
-00001010: 39f1 0703 0d49 01f0 0304 0949 01f0 0a00  9....I.....I....
-00001020: 1625 8804 8c0a d847 4bc7 7ac1 7ad7 4757  .%.....GK.z.z.GW
-00001030: d147 57d7 4762 d147 62d3 4764 d61e 65c0  .GW.Gb.Gb.Gd..e.
-00001040: 219c 75a0 51a7 5aa1 5ad7 253a d125 3ad3  !.u.Q.Z.Z.%:.%:.
-00001050: 253c d51f 3dd2 1e65 8804 d408 1bd8 171b  %<..=..e........
-00001060: 977a 917a d717 30d1 1730 d717 36d1 1736  .z.z..0..0..6..6
-00001070: d717 3dd1 173d d717 48d1 1748 d317 4a88  ..=..=..H..H..J.
-00001080: 0cd8 3236 b72a b12a d732 4bd1 324b d732  ..26.*.*.2K.2K.2
-00001090: 51d1 3251 d732 60d1 3260 d008 1cd8 3135  Q.2Q.2`.2`....15
-000010a0: b71a b11a d731 4ad1 314a d731 5ed1 315e  .....1J.1J.1^.1^
-000010b0: d008 1bdc 1523 a04c d032 46d7 324b d132  .....#.L.2F.2K.2
-000010c0: 4bd0 4d61 d74d 6ad1 4d6a d315 6b88 048c  K.Ma.Mj.Mj..k...
-000010d0: 0af0 0a00 1f23 9f6a 996a d71e 2ed1 1e2e  .....#.j.j......
-000010e0: d71e 3dd1 1e3d d31e 3ff6 0904 1b41 01f0  ..=..=..?....A..
-000010f0: 0600 2024 f407 001c 2aa8 24af 2da9 2dd7  .. $....*.$.-.-.
-00001100: 2a42 d12a 42d3 2a44 d82a 3dd7 2a42 d12a  *B.*B.*D.*=.*B.*
-00001110: 42d8 2a3e d72a 47d1 2a47 d04a 5dd7 4a66  B.*>.*G.*G.J].Jf
-00001120: d14a 66d1 2a66 f505 021c 6801 f200 041b  .Jf.*f....h.....
-00001130: 4101 8804 8c0f f40a 0017 19d7 162b d116  A............+..
-00001140: 2bd7 1639 d116 39b8 2bd8 3a44 d83a 4bf3  +..9..9.+.:D.:K.
-00001150: 0502 174d 0188 0bf0 0600 6301 6e01 d625  ...M......c.n..%
-00001160: 6ed0 5c5e a465 a844 af4a a94a d72c 3cd1  n.\^.e.D.J.J.,<.
-00001170: 2c3c b852 d12c 40d7 2c49 d12c 49d7 2c54  ,<.R.,@.,I.,I.,T
-00001180: d12c 54d3 2c56 d526 57d2 256e 8804 d408  .,T.,V.&W.%n....
-00001190: 22d8 2024 d720 33d1 2033 8804 d408 1df0  ". $. 3. 3......
-000011a0: 0407 0928 dc19 1bd7 192e d119 2ed7 193c  ...(...........<
-000011b0: d119 3cb8 5bd8 3d47 d83d 43f3 0502 1a45  ..<.[.=G.=C....E
-000011c0: 0188 4af0 0800 6301 6d01 d625 6dd0 5c5e  ..J...c.m..%m.\^
-000011d0: a465 a844 af4a a94a d72c 3cd1 2c3c b852  .e.D.J.J.,<.,<.R
-000011e0: d12c 40d7 2c49 d12c 49d7 2c54 d12c 54d3  .,@.,I.,I.,T.,T.
-000011f0: 2c56 d526 57d2 256d 8844 d40c 22f4 0800  ,V.&W.%m.D.."...
-00001200: 1b1d 9f2f 992f a827 b03b c00a d04c 5dd3  ..././.'.;...L].
-00001210: 1a5e 880f e41a 24a8 74af 7ea9 7ed8 2b2f  .^....$.t.~.~.+/
-00001220: af3a a93a d830 3ff4 0502 1b41 0188 048d  .:.:.0?....A....
-00001230: 0ff9 f251 0103 5401 6f01 f9f2 0a00 4c01  ...Q..T.o.....L.
-00001240: 7801 f9f2 0001 4b01 7301 f9f2 1000 1f66  x.....K.s......f
-00001250: 01f9 f20a 041b 4101 f9f2 1000 266f 01f9  ......A.....&o..
-00001260: f210 0026 6e01 f8f0 0201 0928 d825 2788  ...&n......(.%'.
-00001270: 44d6 0c22 fa73 5100 0000 c235 3852 0504  D..".sQ....58R..
-00001280: c41f 2f52 0f04 c50e 0952 0a0a c517 0552  ../R.....R.....R
-00001290: 0f04 c802 2a52 1404 cc02 410d 5219 04cd  ....*R....A.R...
-000012a0: 3c41 0152 1e04 cf17 2552 2800 cf3c 4101  <A.R....%R(..<A.
-000012b0: 5223 04d0 3d08 5228 00d2 0a05 520f 04d2  R#..=.R(....R...
-000012c0: 2305 5228 00d2 2809 5233 034e 2905 da08  #.R(..(.R3.N)...
-000012d0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-000012e0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-000012f0: 5f5f da03 7374 7272 4e00 0000 a900 f300  __..strrN.......
-00001300: 0000 0072 4d00 0000 7207 0000 0072 0700  ...rM...r....r..
-00001310: 0000 0700 0000 7311 0000 0084 00f0 0234  ......s........4
-00001320: 0541 01d8 1d20 f403 3405 4101 7254 0000  .A... ..4.A.rT..
-00001330: 0072 0700 0000 2908 da06 7479 7069 6e67  .r....)...typing
-00001340: da09 6365 6c6c 776f 726c 6472 1a00 0000  ..cellworldr....
-00001350: da04 7574 696c 7204 0000 0072 3e00 0000  ..utilr....r>...
-00001360: 7205 0000 0072 0700 0000 7253 0000 0072  r....r....rS...r
-00001370: 5400 0000 724d 0000 00fa 083c 6d6f 6475  T...rM.....<modu
-00001380: 6c65 3e72 5800 0000 0100 0000 731d 0000  le>rX.......s...
-00001390: 00f0 0301 0101 db00 0ddb 0016 dd00 20dd  .............. .
-000013a0: 0022 f706 3501 4101 f200 3501 4101 7254  ."..5.A...5.A.rT
-000013b0: 0000 00                                  ...
+000009f0: 7c13 ac0c ab03 0000 0000 0000 7c00 5f29  |...........|._)
+00000a00: 0000 0000 0000 0000 7900 6302 0100 6302  ........y.c...c.
+00000a10: 7d05 7700 6302 0100 6302 7d06 7700 6302  }.w.c...c.}.w.c.
+00000a20: 0100 6302 7d06 7700 6302 0100 6302 7d05  ..c.}.w.c...c.}.
+00000a30: 7700 6302 0100 6302 7d0f 7700 6302 0100  w.c...c.}.w.c...
+00000a40: 6302 7d11 7700 6302 0100 6302 7d11 7700  c.}.w.c...c.}.w.
+00000a50: 290d 4eda 0968 6578 6167 6f6e 616c da09  ).N..hexagonal..
+00000a60: 6361 6e6f 6e69 6361 6c29 03da 1877 6f72  canonical)...wor
+00000a70: 6c64 5f63 6f6e 6669 6775 7261 7469 6f6e  ld_configuration
+00000a80: 5f6e 616d 65da 1977 6f72 6c64 5f69 6d70  _name..world_imp
+00000a90: 6c65 6d65 6e74 6174 696f 6e5f 6e61 6d65  lementation_name
+00000aa0: da0f 6f63 636c 7573 696f 6e73 5f6e 616d  ..occlusions_nam
+00000ab0: 65da 0532 315f 3035 2902 720c 0000 0072  e..21_05).r....r
+00000ac0: 0e00 0000 2902 da07 6275 696c 6465 72da  ....)...builder.
+00000ad0: 0577 6f72 6c64 2902 da08 7372 635f 6365  .world)...src_ce
+00000ae0: 6c6c da08 6473 745f 6365 6c6c da0f 7370  ll..dst_cell..sp
+00000af0: 6177 6e5f 6c6f 6361 7469 6f6e 73da 046c  awn_locations..l
+00000b00: 7070 6fda 0567 7261 7068 da0f 6365 6c6c  ppo..graph..cell
+00000b10: 5f76 6973 6962 696c 6974 7929 03da 096c  _visibility)...l
+00000b20: 6f63 6174 696f 6e73 da05 7061 7468 73da  ocations..paths.
+00000b30: 0a76 6973 6962 696c 6974 7929 2ada 0263  .visibility)*..c
+00000b40: 77da 0557 6f72 6c64 da19 6765 745f 6672  w..World..get_fr
+00000b50: 6f6d 5f70 6172 616d 6574 6572 735f 6e61  om_parameters_na
+00000b60: 6d65 7372 1100 0000 da0d 5061 7468 735f  mesr......Paths_
+00000b70: 6275 696c 6465 72da 0d67 6574 5f66 726f  builder..get_fro
+00000b80: 6d5f 6e61 6d65 da05 5061 7468 73da 0843  m_name..Paths..C
+00000b90: 656c 6c5f 6d61 70da 0d63 6f6e 6669 6775  ell_map..configu
+00000ba0: 7261 7469 6f6e da10 6365 6c6c 5f63 6f6f  ration..cell_coo
+00000bb0: 7264 696e 6174 6573 da05 6365 6c6c 73da  rdinates..cells.
+00000bc0: 086f 6363 6c75 6465 64da 0574 7570 6c65  .occluded..tuple
+00000bd0: da08 6c6f 6361 7469 6f6e da0a 6765 745f  ..location..get_
+00000be0: 7661 6c75 6573 7218 0000 00da 0572 616e  valuesr......ran
+00000bf0: 6765 da03 6c65 6eda 0867 6574 5f6d 6f76  ge..len..get_mov
+00000c00: 65da 0b63 6f6f 7264 696e 6174 6573 da02  e..coordinates..
+00000c10: 6964 7219 0000 00da 0a66 7265 655f 6365  idr......free_ce
+00000c20: 6c6c 73da 0e6f 7065 6e5f 6c6f 6361 7469  lls..open_locati
+00000c30: 6f6e 73da 0e69 6d70 6c65 6d65 6e74 6174  ons..implementat
+00000c40: 696f 6eda 0573 7061 6365 da06 6365 6e74  ion..space..cent
+00000c50: 6572 da0e 7472 616e 7366 6f72 6d61 7469  er..transformati
+00000c60: 6f6e da13 6365 6c6c 5f74 7261 6e73 666f  on..cell_transfo
+00000c70: 726d 6174 696f 6e72 0400 0000 da04 7369  rmationr......si
+00000c80: 7a65 da08 726f 7461 7469 6f6e da05 6172  ze..rotation..ar
+00000c90: 656e 61da 0e6f 6363 6c75 6465 645f 6365  ena..occluded_ce
+00000ca0: 6c6c 73da 0a6f 6363 6c75 7369 6f6e 73da  lls..occlusions.
+00000cb0: 1243 656c 6c5f 6772 6f75 705f 6275 696c  .Cell_group_buil
+00000cc0: 6465 72da 1572 6f62 6f74 5f73 7461 7274  der..robot_start
+00000cd0: 5f6c 6f63 6174 696f 6e73 da10 6675 6c6c  _locations..full
+00000ce0: 5f61 6374 696f 6e5f 6c69 7374 da11 746c  _action_list..tl
+00000cf0: 7070 6f5f 6163 7469 6f6e 5f6c 6973 74da  ppo_action_list.
+00000d00: 0c67 6574 5f72 6573 6f75 7263 6572 0500  .get_resourcer..
+00000d10: 0000 da0a 6e61 7669 6761 7469 6f6e 2914  ....navigation).
+00000d20: da04 7365 6c66 7208 0000 00da 0d70 6174  ..selfr......pat
+00000d30: 6873 5f62 7569 6c64 6572 7219 0000 00da  hs_builderr.....
+00000d40: 0763 656c 6c6d 6170 da01 63da 015f da0f  .cellmap..c.._..
+00000d50: 6c6f 6361 7469 6f6e 735f 7061 7468 7372  locations_pathsr
+00000d60: 1200 0000 7213 0000 00da 046d 6f76 65da  ....r......move.
+00000d70: 0c6e 6578 745f 7374 6570 5f69 64da 0c61  .next_step_id..a
+00000d80: 7265 6e61 5f63 656e 7465 72da 1461 7265  rena_center..are
+00000d90: 6e61 5f74 7261 6e73 666f 726d 6174 696f  na_transformatio
+00000da0: 6e72 3400 0000 da04 6365 6c6c da0b 7370  nr4.....cell..sp
+00000db0: 6177 6e5f 6365 6c6c 73da 0273 63da 0a6c  awn_cells..sc..l
+00000dc0: 7070 6f5f 6365 6c6c 7372 1700 0000 7314  ppo_cellsr....s.
+00000dd0: 0000 0020 2020 2020 2020 2020 2020 2020  ...             
+00000de0: 2020 2020 2020 20fa 3d43 3a5c 7265 7365         .=C:\rese
+00000df0: 6172 6368 5c63 656c 6c77 6f72 6c64 5f67  arch\cellworld_g
+00000e00: 616d 655c 6365 6c6c 776f 726c 645f 6761  ame\cellworld_ga
+00000e10: 6d65 5c63 656c 6c77 6f72 6c64 5f6c 6f61  me\cellworld_loa
+00000e20: 6465 722e 7079 da08 5f5f 696e 6974 5f5f  der.py..__init__
+00000e30: 7a18 4365 6c6c 576f 726c 644c 6f61 6465  z.CellWorldLoade
+00000e40: 722e 5f5f 696e 6974 5f5f 0800 0000 73f5  r.__init__....s.
+00000e50: 0300 0080 00e4 1517 9758 9158 d715 37d1  .........X.X..7.
+00000e60: 1537 d051 5cd8 525d d848 52f0 0500 1638  .7.Q\.R].HR....8
+00000e70: f300 0216 5401 8804 8c0a f406 0019 1bd7  ....T...........
+00000e80: 1828 d118 28d7 1836 d118 36d0 505b d847  .(..(..6..6.P[.G
+00000e90: 4ef0 0300 1937 f300 0119 5001 880d e410  N....7....P.....
+00000ea0: 1297 0891 08a0 1db0 64b7 6ab1 6ad4 1041  ........d.j.j..A
+00000eb0: 8805 dc12 1497 2b91 2b98 649f 6a99 6ad7  ......+.+.d.j.j.
+00000ec0: 1e36 d11e 36d7 1e47 d11e 47d3 1248 8807  .6..6..G..G..H..
+00000ed0: f00a 005e 0162 01d7 5d67 d15d 67d7 5d6d  ...^.b..]g.]g.]m
+00000ee0: d15d 6df6 0703 5401 6f01 f006 0059 015a  .]m...T.o....Y.Z
+00000ef0: 01f0 0500 5801 5901 d757 61d2 5761 f103  ....X.Y..Wa.Wa..
+00000f00: 0055 0159 01e4 595e d05f 60d7 5f69 d15f  .U.Y..Y^._`._i._
+00000f10: 69d7 5f74 d15f 74d3 5f76 d359 77f1 0502  i._t._t._v.Yw...
+00000f20: 5501 7801 f200 0354 016f 0188 048c 0ef4  U.x....T.o......
+00000f30: 0c00 5601 5b01 d45b 5ed0 5f63 d75f 69d1  ..V.[..[^._c._i.
+00000f40: 5f69 d75f 6fd1 5f6f d35b 70d3 5571 f603  _i._o._o.[p.Uq..
+00000f50: 014b 0173 01d8 5051 f403 005b 0160 01d4  .K.s..PQ...[.`..
+00000f60: 6063 d064 68d7 646e d164 6ed7 6474 d164  `c.dh.dn.dn.dt.d
+00000f70: 74d3 6075 d35a 76d6 4b77 d055 56ca 44d4  t.`u.Zv.Kw.UV.D.
+00000f80: 4b77 f000 014b 0173 0188 0ff0 0001 4b01  Kw...K.s......K.
+00000f90: 7301 e018 1c9f 0a99 0ad7 1828 d118 28f2  s..........(..(.
+00000fa0: 0004 0949 0188 48d8 1c20 9f4a 994a d71c  ...I..H.. .J.J..
+00000fb0: 2cd1 1c2c f200 030d 4901 9008 d817 1c97  ,..,....I.......
+00000fc0: 7e91 7ea8 78c0 2890 7ed3 174b 9004 d81f  ~.~.x.(.~..K....
+00000fd0: 26a0 78d7 273b d127 3bb8 64d1 2742 d11f  &.x.';.';.d.'B..
+00000fe0: 4390 0cd8 3c48 900f a008 a70b a10b d110  C...<H..........
+00000ff0: 2ca8 58af 5ba9 5bd2 1039 f107 030d 4901  ,.X.[.[..9....I.
+00001000: f003 0409 4901 f00a 0016 2588 048c 0ad8  ....I.....%.....
+00001010: 474b c77a c17a d747 57d1 4757 d747 62d1  GK.z.z.GW.GW.Gb.
+00001020: 4762 d347 64d6 1e65 c021 9c75 a051 a75a  Gb.Gd..e.!.u.Q.Z
+00001030: a15a d725 3ad1 253a d325 3cd5 1f3d d21e  .Z.%:.%:.%<..=..
+00001040: 6588 04d4 081b d817 1b97 7a91 7ad7 1730  e.........z.z..0
+00001050: d117 30d7 1736 d117 36d7 173d d117 3dd7  ..0..6..6..=..=.
+00001060: 1748 d117 48d3 174a 880c d832 36b7 2ab1  .H..H..J...26.*.
+00001070: 2ad7 324b d132 4bd7 3251 d132 51d7 3260  *.2K.2K.2Q.2Q.2`
+00001080: d132 60d0 081c d831 35b7 1ab1 1ad7 314a  .2`....15.....1J
+00001090: d131 4ad7 315e d131 5ed0 081b dc15 23a0  .1J.1^.1^.....#.
+000010a0: 4cd0 3246 d732 4bd1 324b d04d 61d7 4d6a  L.2F.2K.2K.Ma.Mj
+000010b0: d14d 6ad3 156b 8804 8c0a f00a 001f 239f  .Mj..k........#.
+000010c0: 6a99 6ad7 1e2e d11e 2ed7 1e3d d11e 3dd3  j.j........=..=.
+000010d0: 1e3f f609 041b 4101 f006 0020 24f4 0700  .?....A.... $...
+000010e0: 1c2a a824 af2d a92d d72a 42d1 2a42 d32a  .*.$.-.-.*B.*B.*
+000010f0: 44d8 2a3d d72a 42d1 2a42 d82a 3ed7 2a47  D.*=.*B.*B.*>.*G
+00001100: d12a 47d0 4a5d d74a 66d1 4a66 d12a 66f5  .*G.J].Jf.Jf.*f.
+00001110: 0502 1c68 01f2 0004 1b41 0188 048c 0ff4  ...h.....A......
+00001120: 0a00 1719 d716 2bd1 162b d716 39d1 1639  ......+..+..9..9
+00001130: b82b d83a 44d8 3a4b f305 0217 4d01 880b  .+.:D.:K....M...
+00001140: f006 0063 016e 01d6 256e d05c 5ea4 65a8  ...c.n..%n.\^.e.
+00001150: 44af 4aa9 4ad7 2c3c d12c 3cb8 52d1 2c40  D.J.J.,<.,<.R.,@
+00001160: d72c 49d1 2c49 d72c 54d1 2c54 d32c 56d5  .,I.,I.,T.,T.,V.
+00001170: 2657 d225 6e88 04d4 0822 d820 24d7 2033  &W.%n....". $. 3
+00001180: d120 3388 04d4 081d e415 17d7 152a d115  . 3..........*..
+00001190: 2ad7 1538 d115 38b8 1bd8 3943 d839 3ff3  *..8..8...9C.9?.
+000011a0: 0502 1641 0188 0af0 0800 5f01 6901 d621  ...A......_.i..!
+000011b0: 69d0 585a a425 a804 af0a a90a d728 38d1  i.XZ.%.......(8.
+000011c0: 2838 b812 d128 3cd7 2845 d128 45d7 2850  (8...(<.(E.(E.(P
+000011d0: d128 50d3 2852 d522 53d2 2169 8804 d408  .(P.(R."S.!i....
+000011e0: 1ee4 1a1c 9f2f 992f a827 b03b c00a d04c  ....././.'.;...L
+000011f0: 5dd3 1a5e 880f e41a 24a8 74af 7ea9 7ed8  ]..^....$.t.~.~.
+00001200: 2b2f af3a a93a d830 3ff4 0502 1b41 0188  +/.:.:.0?....A..
+00001210: 048d 0ff9 f24b 0103 5401 6f01 f9f2 0a00  .....K..T.o.....
+00001220: 4c01 7801 f9f2 0001 4b01 7301 f9f2 1000  L.x.....K.s.....
+00001230: 1f66 01f9 f20a 041b 4101 f9f2 1000 266f  .f......A.....&o
+00001240: 01f9 f20e 0022 6a01 7339 0000 00c2 3538  ....."j.s9....58
+00001250: 5204 04c4 1f2f 520e 04c5 0e09 5209 0ac5  R..../R.....R...
+00001260: 1705 520e 04c8 022a 5213 04cc 0241 0d52  ..R....*R....A.R
+00001270: 1804 cd3c 4101 521d 04cf 3b41 0152 2204  ...<A.R...;A.R".
+00001280: d209 0552 0e04 4e29 05da 085f 5f6e 616d  ...R..N)...__nam
+00001290: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+000012a0: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0373  .__qualname__..s
+000012b0: 7472 724f 0000 00a9 00f3 0000 0000 724e  trrO..........rN
+000012c0: 0000 0072 0700 0000 7207 0000 0007 0000  ...r....r.......
+000012d0: 0073 1100 0000 8400 f002 3105 4101 d81d  .s........1.A...
+000012e0: 20f4 0331 0541 0172 5500 0000 7207 0000   ..1.A.rU...r...
+000012f0: 0029 08da 0674 7970 696e 67da 0963 656c  .)...typing..cel
+00001300: 6c77 6f72 6c64 721b 0000 00da 0475 7469  lworldr......uti
+00001310: 6c72 0400 0000 723f 0000 0072 0500 0000  lr....r?...r....
+00001320: 7207 0000 0072 5400 0000 7255 0000 0072  r....rT...rU...r
+00001330: 4e00 0000 fa08 3c6d 6f64 756c 653e 7259  N.....<module>rY
+00001340: 0000 0001 0000 0073 1d00 0000 f003 0101  .......s........
+00001350: 01db 000d db00 16dd 0020 dd00 22f7 0632  ......... .."..2
+00001360: 0141 01f2 0032 0141 0172 5500 0000       .A...2.A.rU...
```

### Comparing `cellworld_game-0.0.61/cellworld_game/__pycache__/geometry.cpython-312.pyc` & `cellworld_game-0.0.68/cellworld_game/__pycache__/geometry.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Wed Apr 10 15:24:24 2024 UTC, .py size: 431 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 28af 1666 af01 0000  ........(..f....
+00000000: cb0d 0d0a 0000 0000 92d9 1166 af01 0000  ...........f....
 00000010: e300 0000 0000 0000 0000 0000 0006 0000  ................
 00000020: 0000 0000 00f3 ac00 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 5a00 6400 6401 6c01 5a02 6402 6502  l.Z.d.d.l.Z.d.e.
 00000040: 6a06 0000 0000 0000 0000 0000 0000 0000  j...............
 00000050: 0000 0000 6403 6502 6a06 0000 0000 0000  ....d.e.j.......
 00000060: 0000 0000 0000 0000 0000 0000 6604 6404  ............f.d.
 00000070: 8404 5a04 6405 6502 6a06 0000 0000 0000  ..Z.d.e.j.......
@@ -20,15 +20,15 @@
 00000130: 0000 0000 0000 7a0a 0000 6401 7a08 0000  ......z...d.z...
 00000140: 7c01 6a02 0000 0000 0000 0000 0000 0000  |.j.............
 00000150: 0000 0000 0000 7c00 6a02 0000 0000 0000  ......|.j.......
 00000160: 0000 0000 0000 0000 0000 0000 7a0a 0000  ............z...
 00000170: 6401 7a08 0000 7a00 0000 5300 2902 4ee9  d.z...z...S.).N.
 00000180: 0200 0000 2902 da01 78da 0179 2902 7203  ....)...x..y).r.
 00000190: 0000 0072 0400 0000 7302 0000 0020 20fa  ...r....s....  .
-000001a0: 3543 3a5c 5265 7365 6172 6368 5c63 656c  5C:\Research\cel
+000001a0: 3543 3a5c 7265 7365 6172 6368 5c63 656c  5C:\research\cel
 000001b0: 6c77 6f72 6c64 5f67 616d 655c 6365 6c6c  lworld_game\cell
 000001c0: 776f 726c 645f 6761 6d65 5c67 656f 6d65  world_game\geome
 000001d0: 7472 792e 7079 da09 6469 7374 616e 6365  try.py..distance
 000001e0: 3272 0a00 0000 0500 0000 7331 0000 0080  2r........s1....
 000001f0: 00d8 0c12 8f48 8948 9076 9778 9178 d10c  .....H.H.v.x.x..
 00000200: 1fa0 41d1 0b25 a816 af18 a918 b046 b748  ..A..%.......F.H
 00000210: b148 d129 3cc0 11d1 2842 d10b 42d0 0442  .H.)<...(B..B..B
```

### Comparing `cellworld_game-0.0.61/cellworld_game/__pycache__/model.cpython-312.pyc` & `cellworld_game-0.0.68/cellworld_game/__pycache__/model.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Wed Apr 24 14:48:26 2024 UTC, .py size: 7506 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 11% similar despite different names*

```diff
@@ -1,604 +1,531 @@
-00000000: cb0d 0d0a 0000 0000 ba1b 2966 521d 0000  ..........)fR...
+00000000: cb0d 0d0a 0000 0000 983a 1d66 f919 0000  .........:.f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
-00000020: 0000 0000 00f3 6200 0000 9700 6400 6401  ......b.....d.d.
+00000020: 0000 0000 00f3 5e00 0000 9700 6400 6401  ......^.....d.d.
 00000030: 6c00 5a00 6400 6401 6c01 5a01 6400 6401  l.Z.d.d.l.Z.d.d.
 00000040: 6c02 5a02 6400 6401 6c03 5a04 6402 6403  l.Z.d.d.l.Z.d.d.
-00000050: 6c05 6d06 5a06 6d07 5a07 0100 6402 6404  l.m.Z.m.Z...d.d.
-00000060: 6c08 6d09 5a09 0100 6402 6405 6c0a 6d0b  l.m.Z...d.d.l.m.
-00000070: 5a0b 0100 0200 4700 6406 8400 6407 650c  Z.....G.d...d.e.
-00000080: ab03 0000 0000 0000 5a0d 7901 2908 e900  ........Z.y.)...
-00000090: 0000 004e e901 0000 0029 02da 0541 6765  ...N.....)...Age
-000000a0: 6e74 da0a 4167 656e 7453 7461 7465 2901  nt..AgentState).
-000000b0: da0a 5669 7369 6269 6c69 7479 2901 da05  ..Visibility)...
-000000c0: 6174 616e 3263 0000 0000 0000 0000 0000  atan2c..........
-000000d0: 0000 0700 0000 0000 0000 f3fa 0000 0097  ................
-000000e0: 0065 005a 0164 005a 0209 0009 0064 1964  .e.Z.d.Z.....d.d
-000000f0: 0165 0364 0265 0466 0464 0384 055a 0509  .e.d.e.f.d...Z..
-00000100: 0064 1a64 0465 066a 0e00 0000 0000 0000  .d.d.e.j........
-00000110: 0000 0000 0000 0000 0000 0065 0865 0966  ...........e.e.f
-00000120: 0219 0000 0064 0565 0466 0464 0684 055a  .....d.e.f.d...Z
-00000130: 0a09 0064 1a64 0565 0466 0264 0784 055a  ...d.d.e.f.d...Z
-00000140: 0b64 0865 0864 0965 0c66 0464 0a84 045a  .d.e.d.e.f.d...Z
-00000150: 0d64 0b84 005a 0e64 0c65 0f6a 2000 0000  .d...Z.d.e.j ...
-00000160: 0000 0000 0000 0000 0000 0000 0000 0064  ...............d
-00000170: 0d65 0364 0e65 0366 0664 0f84 045a 1164  .e.d.e.f.d...Z.d
-00000180: 1065 066a 2400 0000 0000 0000 0000 0000  .e.j$...........
-00000190: 0000 0000 0000 0065 0465 0466 0219 0000  .......e.e.f....
-000001a0: 0064 1165 1366 0464 1284 045a 1464 1384  .d.e.f.d...Z.d..
-000001b0: 005a 1509 0064 1b64 1465 0864 1565 0364  .Z...d.d.e.d.e.d
-000001c0: 0e65 1666 0664 1684 055a 1764 0e65 0466  .e.f.d...Z.d.e.f
-000001d0: 0264 1784 045a 1879 1829 1cda 054d 6f64  .d...Z.y.)...Mod
-000001e0: 656c da09 7265 616c 5f74 696d 65da 0974  el..real_time..t
-000001f0: 696d 655f 7374 6570 6305 0000 0000 0000  ime_stepc.......
-00000200: 0000 0000 0004 0000 0003 0000 00f3 ce00  ................
-00000210: 0000 9700 7c01 7c00 5f00 0000 0000 0000  ....|.|._.......
-00000220: 0000 7c02 7c00 5f01 0000 0000 0000 0000  ..|.|._.........
-00000230: 7c03 7c00 5f02 0000 0000 0000 0000 7c04  |.|._.........|.
-00000240: 7c00 5f03 0000 0000 0000 0000 6900 7c00  |._.........i.|.
-00000250: 5f04 0000 0000 0000 0000 740b 0000 0000  _.........t.....
-00000260: 0000 0000 7c00 6a00 0000 0000 0000 0000  ....|.j.........
-00000270: 0000 0000 0000 0000 0000 7c00 6a02 0000  ..........|.j...
-00000280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000290: ac01 ab02 0000 0000 0000 7c00 5f06 0000  ..........|._...
-000002a0: 0000 0000 0000 6400 7c00 5f07 0000 0000  ......d.|._.....
-000002b0: 0000 0000 6402 7c00 5f08 0000 0000 0000  ....d.|._.......
-000002c0: 0000 6403 7c00 5f09 0000 0000 0000 0000  ..d.|._.........
-000002d0: 6402 7c00 5f0a 0000 0000 0000 0000 7900  d.|._.........y.
-000002e0: 2904 4e29 02da 0561 7265 6e61 da0a 6f63  ).N)...arena..oc
-000002f0: 636c 7573 696f 6e73 7202 0000 0046 290b  clusionsr....F).
-00000300: 720d 0000 0072 0e00 0000 720a 0000 0072  r....r....r....r
-00000310: 0b00 0000 da06 6167 656e 7473 7206 0000  ......agentsr...
-00000320: 00da 0a76 6973 6962 696c 6974 79da 096c  ...visibility..l
-00000330: 6173 745f 7374 6570 da04 7469 6d65 da07  ast_step..time..
-00000340: 7275 6e6e 696e 67da 0a73 7465 705f 636f  running..step_co
-00000350: 756e 7429 05da 0473 656c 6672 0d00 0000  unt)...selfr....
-00000360: 720e 0000 0072 0a00 0000 720b 0000 0073  r....r....r....s
-00000370: 0500 0000 2020 2020 20fa 3243 3a5c 5265  ....     .2C:\Re
-00000380: 7365 6172 6368 5c63 656c 6c77 6f72 6c64  search\cellworld
-00000390: 5f67 616d 655c 6365 6c6c 776f 726c 645f  _game\cellworld_
-000003a0: 6761 6d65 5c6d 6f64 656c 2e70 79da 085f  game\model.py.._
-000003b0: 5f69 6e69 745f 5f7a 0e4d 6f64 656c 2e5f  _init__z.Model._
-000003c0: 5f69 6e69 745f 5f0c 0000 0073 5900 0000  _init__....sY...
-000003d0: 8000 f00a 0016 1b88 048c 0ad8 1a24 8804  .............$..
-000003e0: 8c0f d819 2288 048c 0ed8 1922 8804 8c0e  ...."......"....
-000003f0: d82f 3188 048c 0bdc 1a24 a834 af3a a93a  ./1......$.4.:.:
-00000400: c024 c72f c12f d41a 5288 048c 0fd8 191d  .$././..R.......
-00000410: 8804 8c0e d814 1588 048c 09d8 171c 8804  ................
-00000420: 8c0c d81a 1b88 048d 0ff3 0000 0000 da0c  ................
-00000430: 6167 656e 7473 5f73 7461 7465 da07 6465  agents_state..de
-00000440: 6c74 615f 7463 0300 0000 0000 0000 0000  lta_tc..........
-00000450: 0000 0400 0000 0300 0000 f3b0 0000 0097  ................
-00000460: 007c 016a 0100 0000 0000 0000 0000 0000  .|.j............
-00000470: 0000 0000 0000 00ab 0000 0000 0000 0044  ...............D
-00000480: 005d 3200 005c 0200 007d 037d 047c 037c  .]2..\...}.}.|.|
-00000490: 006a 0200 0000 0000 0000 0000 0000 0000  .j..............
-000004a0: 0000 0000 0076 0073 018c 157c 006a 0200  .....v.s...|.j..
-000004b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004c0: 007c 0319 0000 006a 0500 0000 0000 0000  .|.....j........
-000004d0: 0000 0000 0000 0000 0000 007c 04ab 0100  ...........|....
-000004e0: 0000 0000 0001 008c 3404 007c 006a 0700  ........4..|.j..
-000004f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000500: 007c 02ab 0100 0000 0000 0001 0079 00a9  .|...........y..
-00000510: 014e 2904 da05 6974 656d 7372 0f00 0000  .N)...itemsr....
-00000520: da09 7365 745f 7374 6174 65da 105f 5f75  ..set_state..__u
-00000530: 7064 6174 655f 7374 6174 655f 5f29 0572  pdate_state__).r
-00000540: 1500 0000 7219 0000 0072 1a00 0000 da0a  ....r....r......
-00000550: 6167 656e 745f 6e61 6d65 da0b 6167 656e  agent_name..agen
-00000560: 745f 7374 6174 6573 0500 0000 2020 2020  t_states....    
-00000570: 2072 1600 0000 da10 7365 745f 6167 656e   r......set_agen
-00000580: 7473 5f73 7461 7465 7a16 4d6f 6465 6c2e  ts_statez.Model.
-00000590: 7365 745f 6167 656e 7473 5f73 7461 7465  set_agents_state
-000005a0: 1c00 0000 7352 0000 0080 00e0 2733 d727  ....sR......'3.'
-000005b0: 39d1 2739 d327 3bf2 0002 093f d10c 2388  9.'9.';....?..#.
-000005c0: 4a98 0bd8 0f19 9854 9f5b 995b d20f 28d8  J......T.[.[..(.
-000005d0: 1014 970b 910b 984a d110 27d7 1031 d110  .......J..'..1..
-000005e0: 31b0 2bd5 103e f005 0209 3ff0 0600 090d  1.+..>....?.....
-000005f0: d708 1dd1 081d 9867 d508 2672 1800 0000  .......g..&r....
-00000600: 6302 0000 0000 0000 0000 0000 0000 0000  c...............
-00000610: 0003 0000 00f3 0400 0000 9700 7900 721c  ............y.r.
-00000620: 0000 00a9 0029 0272 1500 0000 721a 0000  .....).r....r...
-00000630: 0073 0200 0000 2020 7216 0000 0072 1f00  .s....  r....r..
-00000640: 0000 7a16 4d6f 6465 6c2e 5f5f 7570 6461  ..z.Model.__upda
-00000650: 7465 5f73 7461 7465 5f5f 2300 0000 7305  te_state__#...s.
-00000660: 0000 0080 00e0 080c 7218 0000 00da 046e  ........r......n
-00000670: 616d 65da 0561 6765 6e74 6303 0000 0000  ame..agentc.....
-00000680: 0000 0000 0000 0003 0000 0003 0000 00f3  ................
-00000690: 3e00 0000 9700 7c02 7c00 6a00 0000 0000  >.....|.|.j.....
-000006a0: 0000 0000 0000 0000 0000 0000 0000 7c01  ..............|.
-000006b0: 3c00 0000 7c01 7c02 5f01 0000 0000 0000  <...|.|._.......
-000006c0: 0000 7c00 7c02 5f02 0000 0000 0000 0000  ..|.|._.........
-000006d0: 7900 721c 0000 0029 0372 0f00 0000 7225  y.r....).r....r%
-000006e0: 0000 00da 056d 6f64 656c 2903 7215 0000  .....model).r...
-000006f0: 0072 2500 0000 7226 0000 0073 0300 0000  .r%...r&...s....
-00000700: 2020 2072 1600 0000 da09 6164 645f 6167     r......add_ag
-00000710: 656e 747a 0f4d 6f64 656c 2e61 6464 5f61  entz.Model.add_a
-00000720: 6765 6e74 2700 0000 731e 0000 0080 00d8  gent'...s.......
-00000730: 1c21 8804 8f0b 890b 9044 d108 19d8 1519  .!.......D......
-00000740: 8805 8c0a d816 1a88 058d 0b72 1800 0000  ...........r....
-00000750: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-00000760: 0003 0000 00f3 3a01 0000 9700 6401 7c00  ......:.....d.|.
-00000770: 5f00 0000 0000 0000 0000 7c00 6a02 0000  _.........|.j...
-00000780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000790: 6a05 0000 0000 0000 0000 0000 0000 0000  j...............
-000007a0: 0000 0000 ab00 0000 0000 0000 4400 5d15  ............D.].
-000007b0: 0000 5c02 0000 7d01 7d02 7c02 6a07 0000  ..\...}.}.|.j...
-000007c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000007d0: ab00 0000 0000 0000 0100 8c17 0400 7c00  ..............|.
-000007e0: 6a09 0000 0000 0000 0000 0000 0000 0000  j...............
-000007f0: 0000 0000 ab00 0000 0000 0000 7d03 7c00  ............}.|.
-00000800: 6a02 0000 0000 0000 0000 0000 0000 0000  j...............
-00000810: 0000 0000 6a05 0000 0000 0000 0000 0000  ....j...........
-00000820: 0000 0000 0000 0000 ab00 0000 0000 0000  ................
-00000830: 4400 5d15 0000 5c02 0000 7d01 7d02 7c02  D.]...\...}.}.|.
-00000840: 6a0b 0000 0000 0000 0000 0000 0000 0000  j...............
-00000850: 0000 0000 ab00 0000 0000 0000 0100 8c17  ................
-00000860: 0400 740d 0000 0000 0000 0000 6a0c 0000  ..t.........j...
-00000870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000880: ab00 0000 0000 0000 7c00 5f07 0000 0000  ........|._.....
-00000890: 0000 0000 6402 7c00 5f08 0000 0000 0000  ....d.|._.......
-000008a0: 0000 7900 2903 4e54 7202 0000 0029 0972  ..y.).NTr....).r
-000008b0: 1300 0000 720f 0000 0072 1d00 0000 da05  ....r....r......
-000008c0: 7265 7365 74da 1067 6574 5f6f 6273 6572  reset..get_obser
-000008d0: 7661 7469 6f6e 73da 0573 7461 7274 7212  vations..startr.
-000008e0: 0000 0072 1100 0000 7214 0000 0029 0472  ...r....r....).r
-000008f0: 1500 0000 7225 0000 0072 2600 0000 da0c  ....r%...r&.....
-00000900: 6f62 7365 7276 6174 696f 6e73 7304 0000  observationss...
-00000910: 0020 2020 2072 1600 0000 722b 0000 007a  .    r....r+...z
-00000920: 0b4d 6f64 656c 2e72 6573 6574 2c00 0000  .Model.reset,...
-00000930: 737d 0000 0080 00d8 171b 8804 8c0c d81b  s}..............
-00000940: 1f9f 3b99 3bd7 1b2c d11b 2cd3 1b2e f200  ..;.;..,..,.....
-00000950: 0109 1a89 4b88 4490 25d8 0c11 8f4b 894b  ....K.D.%....K.K
-00000960: 8d4d f003 0109 1ae0 171b d717 2cd1 172c  .M..........,..,
-00000970: d317 2e88 0cd8 1b1f 9f3b 993b d71b 2cd1  .........;.;..,.
-00000980: 1b2c d31b 2ef2 0001 091a 894b 8844 9025  .,.........K.D.%
-00000990: d80c 118f 4b89 4b8d 4df0 0301 091a e419  ....K.K.M.......
-000009a0: 1d9f 1999 199b 1b88 048c 0ed8 1a1b 8804  ................
-000009b0: 8d0f 7218 0000 00da 0d61 6765 6e74 5f70  ..r......agent_p
-000009c0: 6f6c 7967 6f6e da0a 636f 6c6c 6973 696f  olygon..collisio
-000009d0: 6e73 da06 7265 7475 726e 6303 0000 0000  ns..returnc.....
-000009e0: 0000 0000 0000 0004 0000 0003 0000 00f3  ................
-000009f0: 8800 0000 9700 7c00 6a00 0000 0000 0000  ......|.j.......
-00000a00: 0000 0000 0000 0000 0000 0000 6a03 0000  ............j...
-00000a10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000a20: 7c01 ab01 0000 0000 0000 7301 7901 7c02  |.........s.y.|.
-00000a30: 7224 7c00 6a04 0000 0000 0000 0000 0000  r$|.j...........
-00000a40: 0000 0000 0000 0000 4400 5d15 0000 7d03  ........D.]...}.
-00000a50: 7c01 6a07 0000 0000 0000 0000 0000 0000  |.j.............
-00000a60: 0000 0000 0000 7c03 ab01 0000 0000 0000  ......|.........
-00000a70: 7301 8c15 0100 7901 0400 7902 2903 4e46  s.....y...y.).NF
-00000a80: 5429 0472 0d00 0000 da08 636f 6e74 6169  T).r......contai
-00000a90: 6e73 720e 0000 00da 0a69 6e74 6572 7365  nsr......interse
-00000aa0: 6374 7329 0472 1500 0000 722f 0000 0072  cts).r....r/...r
-00000ab0: 3000 0000 da09 6f63 636c 7573 696f 6e73  0.....occlusions
-00000ac0: 0400 0000 2020 2020 7216 0000 00da 0e69  ....    r......i
-00000ad0: 735f 7661 6c69 645f 7374 6174 657a 144d  s_valid_statez.M
-00000ae0: 6f64 656c 2e69 735f 7661 6c69 645f 7374  odel.is_valid_st
-00000af0: 6174 6536 0000 0073 4300 0000 8000 d80f  ate6...sC.......
-00000b00: 138f 7a89 7ad7 0f22 d10f 22a0 3dd4 0f31  ..z.z.."..".=..1
-00000b10: d813 18d9 0b15 d81d 219f 5f99 5ff2 0002  ........!._._...
-00000b20: 0d21 9009 d813 20d7 132b d113 2ba8 49d5  .!.... ..+..+.I.
-00000b30: 1336 d91b 20f0 0502 0d21 f006 0010 1472  .6.. ....!.....r
-00000b40: 1800 0000 da03 7372 63da 0b77 616c 6c5f  ......src..wall_
-00000b50: 6e75 6d62 6572 6303 0000 0000 0000 0000  numberc.........
-00000b60: 0000 0007 0000 0003 0000 00f3 9400 0000  ................
-00000b70: 9700 7401 0000 0000 0000 0000 6a02 0000  ..t.........j...
+00000050: 6c05 6d06 5a06 0100 6402 6404 6c07 6d08  l.m.Z...d.d.l.m.
+00000060: 5a08 0100 6402 6405 6c09 6d0a 5a0a 0100  Z...d.d.l.m.Z...
+00000070: 0200 4700 6406 8400 6407 650b ab03 0000  ..G.d...d.e.....
+00000080: 0000 0000 5a0c 7901 2908 e900 0000 004e  ....Z.y.)......N
+00000090: e901 0000 0029 01da 0541 6765 6e74 2901  .....)...Agent).
+000000a0: da0a 5669 7369 6269 6c69 7479 2901 da05  ..Visibility)...
+000000b0: 6174 616e 3263 0000 0000 0000 0000 0000  atan2c..........
+000000c0: 0000 0700 0000 0000 0000 f3b2 0000 0097  ................
+000000d0: 0065 005a 0164 005a 0209 0009 0064 1564  .e.Z.d.Z.....d.d
+000000e0: 0165 0364 0265 0466 0464 0384 055a 0564  .e.d.e.f.d...Z.d
+000000f0: 0465 0664 0565 0766 0464 0684 045a 0864  .e.d.e.f.d...Z.d
+00000100: 0784 005a 0964 0865 0a6a 1600 0000 0000  ...Z.d.e.j......
+00000110: 0000 0000 0000 0000 0000 0000 0064 0965  .............d.e
+00000120: 0364 0a65 0366 0664 0b84 045a 0c64 0c65  .d.e.f.d...Z.d.e
+00000130: 0d6a 1c00 0000 0000 0000 0000 0000 0000  .j..............
+00000140: 0000 0000 0065 0465 0466 0219 0000 0064  .....e.e.f.....d
+00000150: 0d65 0f66 0464 0e84 045a 1064 0f84 005a  .e.f.d...Z.d...Z
+00000160: 1109 0064 1664 1065 0664 1165 0364 0a65  ...d.d.e.d.e.d.e
+00000170: 1266 0664 1284 055a 1364 1384 005a 1479  .f.d...Z.d...Z.y
+00000180: 1429 17da 054d 6f64 656c da09 7265 616c  .)...Model..real
+00000190: 5f74 696d 65da 0974 696d 655f 7374 6570  _time..time_step
+000001a0: 6305 0000 0000 0000 0000 0000 0004 0000  c...............
+000001b0: 0003 0000 00f3 a400 0000 9700 7c01 7c00  ............|.|.
+000001c0: 5f00 0000 0000 0000 0000 7c02 7c00 5f01  _.........|.|._.
+000001d0: 0000 0000 0000 0000 7c03 7c00 5f02 0000  ........|.|._...
+000001e0: 0000 0000 0000 7c04 7c00 5f03 0000 0000  ......|.|._.....
+000001f0: 0000 0000 6900 7c00 5f04 0000 0000 0000  ....i.|._.......
+00000200: 0000 740b 0000 0000 0000 0000 7c00 6a00  ..t.........|.j.
+00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000220: 0000 7c00 6a02 0000 0000 0000 0000 0000  ..|.j...........
+00000230: 0000 0000 0000 0000 ac01 ab02 0000 0000  ................
+00000240: 0000 7c00 5f06 0000 0000 0000 0000 6400  ..|._.........d.
+00000250: 7c00 5f07 0000 0000 0000 0000 7900 2902  |._.........y.).
+00000260: 4e29 02da 0561 7265 6e61 da0a 6f63 636c  N)...arena..occl
+00000270: 7573 696f 6e73 2908 720c 0000 0072 0d00  usions).r....r..
+00000280: 0000 7209 0000 0072 0a00 0000 da06 6167  ..r....r......ag
+00000290: 656e 7473 7205 0000 00da 0a76 6973 6962  entsr......visib
+000002a0: 696c 6974 79da 096c 6173 745f 7374 6570  ility..last_step
+000002b0: 2905 da04 7365 6c66 720c 0000 0072 0d00  )...selfr....r..
+000002c0: 0000 7209 0000 0072 0a00 0000 7305 0000  ..r....r....s...
+000002d0: 0020 2020 2020 fa32 433a 5c72 6573 6561  .     .2C:\resea
+000002e0: 7263 685c 6365 6c6c 776f 726c 645f 6761  rch\cellworld_ga
+000002f0: 6d65 5c63 656c 6c77 6f72 6c64 5f67 616d  me\cellworld_gam
+00000300: 655c 6d6f 6465 6c2e 7079 da08 5f5f 696e  e\model.py..__in
+00000310: 6974 5f5f 7a0e 4d6f 6465 6c2e 5f5f 696e  it__z.Model.__in
+00000320: 6974 5f5f 0c00 0000 7344 0000 0080 00f0  it__....sD......
+00000330: 0a00 161b 8804 8c0a d81a 2488 048c 0fd8  ..........$.....
+00000340: 1922 8804 8c0e d819 2288 048c 0ed8 2f31  ."......"...../1
+00000350: 8804 8c0b dc1a 24a8 34af 3aa9 3ac0 24c7  ......$.4.:.:.$.
+00000360: 2fc1 2fd4 1a52 8804 8c0f d819 1d88 048d  /./..R..........
+00000370: 0ef3 0000 0000 da04 6e61 6d65 da05 6167  ........name..ag
+00000380: 656e 7463 0300 0000 0000 0000 0000 0000  entc............
+00000390: 0300 0000 0300 0000 f33e 0000 0097 007c  .........>.....|
+000003a0: 027c 006a 0000 0000 0000 0000 0000 0000  .|.j............
+000003b0: 0000 0000 0000 007c 013c 0000 007c 017c  .......|.<...|.|
+000003c0: 025f 0100 0000 0000 0000 007c 007c 025f  ._.........|.|._
+000003d0: 0200 0000 0000 0000 0079 00a9 014e 2903  .........y...N).
+000003e0: 720e 0000 0072 1500 0000 da05 6d6f 6465  r....r......mode
+000003f0: 6c29 0372 1100 0000 7215 0000 0072 1600  l).r....r....r..
+00000400: 0000 7303 0000 0020 2020 7212 0000 00da  ..s....   r.....
+00000410: 0961 6464 5f61 6765 6e74 7a0f 4d6f 6465  .add_agentz.Mode
+00000420: 6c2e 6164 645f 6167 656e 7419 0000 0073  l.add_agent....s
+00000430: 1e00 0000 8000 d81c 2188 048f 0b89 0b90  ........!.......
+00000440: 44d1 0819 d815 1988 058c 0ad8 161a 8805  D...............
+00000450: 8d0b 7214 0000 0063 0100 0000 0000 0000  ..r....c........
+00000460: 0000 0000 0300 0000 0300 0000 f31e 0100  ................
+00000470: 0097 007c 006a 0000 0000 0000 0000 0000  ...|.j..........
+00000480: 0000 0000 0000 0000 006a 0300 0000 0000  .........j......
+00000490: 0000 0000 0000 0000 0000 0000 00ab 0000  ................
+000004a0: 0000 0000 0044 005d 1500 005c 0200 007d  .....D.]...\...}
+000004b0: 017d 027c 026a 0500 0000 0000 0000 0000  .}.|.j..........
+000004c0: 0000 0000 0000 0000 00ab 0000 0000 0000  ................
+000004d0: 0001 008c 1704 007c 006a 0700 0000 0000  .......|.j......
+000004e0: 0000 0000 0000 0000 0000 0000 00ab 0000  ................
+000004f0: 0000 0000 007d 037c 006a 0000 0000 0000  .....}.|.j......
+00000500: 0000 0000 0000 0000 0000 0000 006a 0300  .............j..
+00000510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000520: 00ab 0000 0000 0000 0044 005d 1500 005c  .........D.]...\
+00000530: 0200 007d 017d 027c 026a 0900 0000 0000  ...}.}.|.j......
+00000540: 0000 0000 0000 0000 0000 0000 00ab 0000  ................
+00000550: 0000 0000 0001 008c 1704 0074 0b00 0000  ...........t....
+00000560: 0000 0000 006a 0a00 0000 0000 0000 0000  .....j..........
+00000570: 0000 0000 0000 0000 00ab 0000 0000 0000  ................
+00000580: 007c 005f 0600 0000 0000 0000 0079 0072  .|._.........y.r
+00000590: 1800 0000 2907 720e 0000 00da 0569 7465  ....).r......ite
+000005a0: 6d73 da05 7265 7365 74da 1067 6574 5f6f  ms..reset..get_o
+000005b0: 6273 6572 7661 7469 6f6e 73da 0573 7461  bservations..sta
+000005c0: 7274 da04 7469 6d65 7210 0000 0029 0472  rt..timer....).r
+000005d0: 1100 0000 7215 0000 0072 1600 0000 da0c  ....r....r......
+000005e0: 6f62 7365 7276 6174 696f 6e73 7304 0000  observationss...
+000005f0: 0020 2020 2072 1200 0000 721d 0000 007a  .    r....r....z
+00000600: 0b4d 6f64 656c 2e72 6573 6574 1e00 0000  .Model.reset....
+00000610: 736f 0000 0080 00d8 1b1f 9f3b 993b d71b  so.........;.;..
+00000620: 2cd1 1b2c d31b 2ef2 0001 091a 894b 8844  ,..,.........K.D
+00000630: 9025 d80c 118f 4b89 4b8d 4df0 0301 091a  .%....K.K.M.....
+00000640: e017 1bd7 172c d117 2cd3 172e 880c d81b  .....,..,.......
+00000650: 1f9f 3b99 3bd7 1b2c d11b 2cd3 1b2e f200  ..;.;..,..,.....
+00000660: 0109 1a89 4b88 4490 25d8 0c11 8f4b 894b  ....K.D.%....K.K
+00000670: 8d4d f003 0109 1ae4 191d 9f19 9919 9b1b  .M..............
+00000680: 8804 8d0e 7214 0000 00da 0d61 6765 6e74  ....r......agent
+00000690: 5f70 6f6c 7967 6f6e da0a 636f 6c6c 6973  _polygon..collis
+000006a0: 696f 6e73 da06 7265 7475 726e 6303 0000  ions..returnc...
+000006b0: 0000 0000 0000 0000 0004 0000 0003 0000  ................
+000006c0: 00f3 8800 0000 9700 7c00 6a00 0000 0000  ........|.j.....
+000006d0: 0000 0000 0000 0000 0000 0000 0000 6a03  ..............j.
+000006e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000006f0: 0000 7c01 ab01 0000 0000 0000 7301 7901  ..|.........s.y.
+00000700: 7c02 7224 7c00 6a04 0000 0000 0000 0000  |.r$|.j.........
+00000710: 0000 0000 0000 0000 0000 4400 5d15 0000  ..........D.]...
+00000720: 7d03 7c01 6a07 0000 0000 0000 0000 0000  }.|.j...........
+00000730: 0000 0000 0000 0000 7c03 ab01 0000 0000  ........|.......
+00000740: 0000 7301 8c15 0100 7901 0400 7902 2903  ..s.....y...y.).
+00000750: 4e46 5429 0472 0c00 0000 da08 636f 6e74  NFT).r......cont
+00000760: 6169 6e73 720d 0000 00da 0a69 6e74 6572  ainsr......inter
+00000770: 7365 6374 7329 0472 1100 0000 7222 0000  sects).r....r"..
+00000780: 0072 2300 0000 da09 6f63 636c 7573 696f  .r#.....occlusio
+00000790: 6e73 0400 0000 2020 2020 7212 0000 00da  ns....    r.....
+000007a0: 0e69 735f 7661 6c69 645f 7374 6174 657a  .is_valid_statez
+000007b0: 144d 6f64 656c 2e69 735f 7661 6c69 645f  .Model.is_valid_
+000007c0: 7374 6174 6526 0000 0073 4300 0000 8000  state&...sC.....
+000007d0: d80f 138f 7a89 7ad7 0f22 d10f 22a0 3dd4  ....z.z.."..".=.
+000007e0: 0f31 d813 18d9 0b15 d81d 219f 5f99 5ff2  .1........!._._.
+000007f0: 0002 0d21 9009 d813 20d7 132b d113 2ba8  ...!.... ..+..+.
+00000800: 49d5 1336 d91b 20f0 0502 0d21 f006 0010  I..6.. ....!....
+00000810: 1472 1400 0000 da03 7372 63da 0b77 616c  .r......src..wal
+00000820: 6c5f 6e75 6d62 6572 6303 0000 0000 0000  l_numberc.......
+00000830: 0000 0000 0007 0000 0003 0000 00f3 9400  ................
+00000840: 0000 9700 7401 0000 0000 0000 0000 6a02  ....t.........j.
+00000850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000860: 0000 7405 0000 0000 0000 0000 7407 0000  ..t.........t...
+00000870: 0000 0000 0000 6a08 0000 0000 0000 0000  ......j.........
+00000880: 0000 0000 0000 0000 0000 7c01 ab01 0000  ..........|.....
+00000890: 0000 0000 7c00 6a0a 0000 0000 0000 0000  ....|.j.........
+000008a0: 0000 0000 0000 0000 0000 6a0c 0000 0000  ..........j.....
+000008b0: 0000 0000 0000 0000 0000 0000 0000 7c02  ..............|.
+000008c0: 1900 0000 ab02 0000 0000 0000 ab01 0000  ................
+000008d0: 0000 0000 5300 7218 0000 0029 07da 046d  ....S.r....)...m
+000008e0: 6174 68da 0764 6567 7265 6573 7206 0000  ath..degreesr...
+000008f0: 00da 0273 70da 0550 6f69 6e74 720f 0000  ...sp..Pointr...
+00000900: 00da 0f77 616c 6c73 5f63 656e 7472 6f69  ...walls_centroi
+00000910: 6473 2903 7211 0000 0072 2a00 0000 722b  ds).r....r*...r+
+00000920: 0000 0073 0300 0000 2020 2072 1200 0000  ...s....   r....
+00000930: da0e 7761 6c6c 5f64 6972 6563 7469 6f6e  ..wall_direction
+00000940: 7a14 4d6f 6465 6c2e 7761 6c6c 5f64 6972  z.Model.wall_dir
+00000950: 6563 7469 6f6e 2f00 0000 7330 0000 0080  ection/...s0....
+00000960: 00dc 0f13 8f7c 897c 9c45 a422 a728 a128  .....|.|.E.".(.(
+00000970: a833 a32d b014 b71f b11f d731 50d1 3150  .3.-.......1P.1P
+00000980: d051 5cd1 315d d31c 5ed3 0f5f d008 5f72  .Q\.1]..^.._.._r
+00000990: 1400 0000 6301 0000 0000 0000 0000 0000  ....c...........
+000009a0: 000a 0000 0003 0000 00f3 e603 0000 9700  ................
+000009b0: 7c00 6a00 0000 0000 0000 0000 0000 0000  |.j.............
+000009c0: 0000 0000 0000 4400 8f01 8f02 6303 6900  ......D.....c.i.
+000009d0: 6302 5d1e 0000 7d01 7c01 7c00 6a00 0000  c.]...}.|.|.j...
+000009e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000009f0: 4400 8f02 6302 6900 6302 5d05 0000 7d02  D...c.i.c.]...}.
+00000a00: 7c02 6400 9302 8c07 0400 6302 7d02 9302  |.d.......c.}...
+00000a10: 8c20 0400 7d03 7d01 7d02 6900 7d04 7c00  . ..}.}.}.i.}.|.
+00000a20: 6a00 0000 0000 0000 0000 0000 0000 0000  j...............
+00000a30: 0000 0000 6a03 0000 0000 0000 0000 0000  ....j...........
+00000a40: 0000 0000 0000 0000 ab00 0000 0000 0000  ................
+00000a50: 4400 9001 5d90 0000 5c02 0000 7d01 7d05  D...]...\...}.}.
+00000a60: 6900 7c04 7c01 3c00 0000 7405 0000 0000  i.|.|.<...t.....
+00000a70: 0000 0000 6a06 0000 0000 0000 0000 0000  ....j...........
+00000a80: 0000 0000 0000 0000 7c05 6a08 0000 0000  ........|.j.....
+00000a90: 0000 0000 0000 0000 0000 0000 0000 6a0a  ..............j.
+00000aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000ab0: 0000 ab01 0000 0000 0000 7d06 7c00 6a0c  ..........}.|.j.
+00000ac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000ad0: 0000 6a0f 0000 0000 0000 0000 0000 0000  ..j.............
+00000ae0: 0000 0000 0000 7c06 ac01 ab01 0000 0000  ......|.........
+00000af0: 0000 7d07 6700 7d08 7c07 4400 5d2a 0000  ..}.g.}.|.D.]*..
+00000b00: 5c03 0000 7d09 7d0a 7d0b 7c08 6a11 0000  \...}.}.}.|.j...
+00000b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000b20: 7c0b 7c00 6a13 0000 0000 0000 0000 0000  |.|.j...........
+00000b30: 0000 0000 0000 0000 7c06 7c09 ac02 ab02  ........|.|.....
+00000b40: 0000 0000 0000 6602 ab01 0000 0000 0000  ......f.........
+00000b50: 0100 8c2c 0400 7c08 7c04 7c01 1900 0000  ...,..|.|.|.....
+00000b60: 6403 3c00 0000 7c00 6a00 0000 0000 0000  d.<...|.j.......
+00000b70: 0000 0000 0000 0000 0000 0000 6a03 0000  ............j...
 00000b80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b90: 7405 0000 0000 0000 0000 7407 0000 0000  t.........t.....
-00000ba0: 0000 0000 6a08 0000 0000 0000 0000 0000  ....j...........
-00000bb0: 0000 0000 0000 0000 7c01 ab01 0000 0000  ........|.......
-00000bc0: 0000 7c00 6a0a 0000 0000 0000 0000 0000  ..|.j...........
-00000bd0: 0000 0000 0000 0000 6a0c 0000 0000 0000  ........j.......
-00000be0: 0000 0000 0000 0000 0000 0000 7c02 1900  ............|...
-00000bf0: 0000 ab02 0000 0000 0000 ab01 0000 0000  ................
-00000c00: 0000 5300 721c 0000 0029 07da 046d 6174  ..S.r....)...mat
-00000c10: 68da 0764 6567 7265 6573 7207 0000 00da  h..degreesr.....
-00000c20: 0273 70da 0550 6f69 6e74 7210 0000 00da  .sp..Pointr.....
-00000c30: 0f77 616c 6c73 5f63 656e 7472 6f69 6473  .walls_centroids
-00000c40: 2903 7215 0000 0072 3700 0000 7238 0000  ).r....r7...r8..
-00000c50: 0073 0300 0000 2020 2072 1600 0000 da0e  .s....   r......
-00000c60: 7761 6c6c 5f64 6972 6563 7469 6f6e 7a14  wall_directionz.
-00000c70: 4d6f 6465 6c2e 7761 6c6c 5f64 6972 6563  Model.wall_direc
-00000c80: 7469 6f6e 3f00 0000 7330 0000 0080 00dc  tion?...s0......
-00000c90: 0f13 8f7c 897c 9c45 a422 a728 a128 a833  ...|.|.E.".(.(.3
-00000ca0: a32d b014 b71f b11f d731 50d1 3150 d051  .-.......1P.1P.Q
-00000cb0: 5cd1 315d d31c 5ed3 0f5f d008 5f72 1800  \.1]..^.._.._r..
-00000cc0: 0000 6301 0000 0000 0000 0000 0000 000a  ..c.............
-00000cd0: 0000 0003 0000 00f3 e603 0000 9700 7c00  ..............|.
-00000ce0: 6a00 0000 0000 0000 0000 0000 0000 0000  j...............
-00000cf0: 0000 0000 4400 8f01 8f02 6303 6900 6302  ....D.....c.i.c.
-00000d00: 5d1e 0000 7d01 7c01 7c00 6a00 0000 0000  ]...}.|.|.j.....
-00000d10: 0000 0000 0000 0000 0000 0000 0000 4400  ..............D.
-00000d20: 8f02 6302 6900 6302 5d05 0000 7d02 7c02  ..c.i.c.]...}.|.
-00000d30: 6400 9302 8c07 0400 6302 7d02 9302 8c20  d.......c.}.... 
-00000d40: 0400 7d03 7d01 7d02 6900 7d04 7c00 6a00  ..}.}.}.i.}.|.j.
-00000d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000d60: 0000 6a03 0000 0000 0000 0000 0000 0000  ..j.............
-00000d70: 0000 0000 0000 ab00 0000 0000 0000 4400  ..............D.
-00000d80: 9001 5d90 0000 5c02 0000 7d01 7d05 6900  ..]...\...}.}.i.
-00000d90: 7c04 7c01 3c00 0000 7405 0000 0000 0000  |.|.<...t.......
-00000da0: 0000 6a06 0000 0000 0000 0000 0000 0000  ..j.............
-00000db0: 0000 0000 0000 7c05 6a08 0000 0000 0000  ......|.j.......
-00000dc0: 0000 0000 0000 0000 0000 0000 6a0a 0000  ............j...
-00000dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000de0: ab01 0000 0000 0000 7d06 7c00 6a0c 0000  ........}.|.j...
-00000df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000e00: 6a0f 0000 0000 0000 0000 0000 0000 0000  j...............
-00000e10: 0000 0000 7c06 ac01 ab01 0000 0000 0000  ....|...........
-00000e20: 7d07 6700 7d08 7c07 4400 5d2a 0000 5c03  }.g.}.|.D.]*..\.
-00000e30: 0000 7d09 7d0a 7d0b 7c08 6a11 0000 0000  ..}.}.}.|.j.....
-00000e40: 0000 0000 0000 0000 0000 0000 0000 7c0b  ..............|.
-00000e50: 7c00 6a13 0000 0000 0000 0000 0000 0000  |.j.............
-00000e60: 0000 0000 0000 7c06 7c09 ac02 ab02 0000  ......|.|.......
-00000e70: 0000 0000 6602 ab01 0000 0000 0000 0100  ....f...........
-00000e80: 8c2c 0400 7c08 7c04 7c01 1900 0000 6403  .,..|.|.|.....d.
-00000e90: 3c00 0000 7c00 6a00 0000 0000 0000 0000  <...|.j.........
-00000ea0: 0000 0000 0000 0000 0000 6a03 0000 0000  ..........j.....
-00000eb0: 0000 0000 0000 0000 0000 0000 0000 ab00  ................
-00000ec0: 0000 0000 0000 4400 5d6d 0000 5c02 0000  ......D.]m..\...
-00000ed0: 7d02 7d0c 7c03 7c01 1900 0000 7c02 1900  }.}.|.|.....|...
-00000ee0: 0000 8101 8c0f 7c01 7c02 6b28 0000 7203  ......|.|.k(..r.
-00000ef0: 6404 7d0d 6e47 7405 0000 0000 0000 0000  d.}.nGt.........
-00000f00: 6a06 0000 0000 0000 0000 0000 0000 0000  j...............
-00000f10: 0000 0000 7c0c 6a08 0000 0000 0000 0000  ....|.j.........
-00000f20: 0000 0000 0000 0000 0000 6a0a 0000 0000  ..........j.....
-00000f30: 0000 0000 0000 0000 0000 0000 0000 ab01  ................
-00000f40: 0000 0000 0000 7d0e 7c00 6a0c 0000 0000  ......}.|.j.....
-00000f50: 0000 0000 0000 0000 0000 0000 0000 6a15  ..............j.
-00000f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000f70: 0000 7c06 7c0e 7c07 ac05 ab03 0000 0000  ..|.|.|.........
-00000f80: 0000 7d0d 7c0d 7c03 7c01 1900 0000 7c02  ..}.|.|.|.....|.
-00000f90: 3c00 0000 7c0d 7c03 7c02 1900 0000 7c01  <...|.|.|.....|.
-00000fa0: 3c00 0000 8c6f 0400 6900 7c04 7c01 1900  <....o..i.|.|...
-00000fb0: 0000 6406 3c00 0000 7c03 6a03 0000 0000  ..d.<...|.j.....
-00000fc0: 0000 0000 0000 0000 0000 0000 0000 ab00  ................
-00000fd0: 0000 0000 0000 4400 5d62 0000 5c02 0000  ......D.]b..\...
-00000fe0: 7d02 7d0d 7c0d 7250 7c00 6a00 0000 0000  }.}.|.rP|.j.....
-00000ff0: 0000 0000 0000 0000 0000 0000 0000 7c02  ..............|.
-00001000: 1900 0000 6a08 0000 0000 0000 0000 0000  ....j...........
-00001010: 0000 0000 0000 0000 6a0a 0000 0000 0000  ........j.......
-00001020: 0000 0000 0000 0000 0000 0000 7c00 6a00  ............|.j.
-00001030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001040: 0000 7c02 1900 0000 6a08 0000 0000 0000  ..|.....j.......
-00001050: 0000 0000 0000 0000 0000 0000 6a16 0000  ............j...
-00001060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001070: 6602 7c04 7c01 1900 0000 6406 1900 0000  f.|.|.....d.....
-00001080: 7c02 3c00 0000 8c58 6400 7c04 7c01 1900  |.<....Xd.|.|...
-00001090: 0000 6406 1900 0000 7c02 3c00 0000 8c64  ..d.....|.<....d
-000010a0: 0400 9001 8c93 0400 7c04 5300 6302 0100  ........|.S.c...
-000010b0: 6302 7d02 7700 6302 0100 6303 7d02 7d01  c.}.w.c...c.}.}.
-000010c0: 7700 2907 4ea9 0172 3700 0000 a902 7237  w.).N..r7.....r7
-000010d0: 0000 0072 3800 0000 da05 7761 6c6c 7354  ...r8.....wallsT
-000010e0: a903 7237 0000 00da 0364 7374 da11 7761  ..r7.....dst..wa
-000010f0: 6c6c 735f 6279 5f64 6973 7461 6e63 65da  lls_by_distance.
-00001100: 0c61 6765 6e74 5f73 7461 7465 7329 0c72  .agent_states).r
-00001110: 0f00 0000 721d 0000 0072 3c00 0000 723d  ....r....r<...r=
-00001120: 0000 00da 0573 7461 7465 da08 6c6f 6361  .....state..loca
-00001130: 7469 6f6e 7210 0000 0072 4600 0000 da06  tionr....rF.....
-00001140: 6170 7065 6e64 723f 0000 00da 0d6c 696e  appendr?.....lin
-00001150: 655f 6f66 5f73 6967 6874 da09 6469 7265  e_of_sight..dire
-00001160: 6374 696f 6e29 0f72 1500 0000 da08 7372  ction).r......sr
-00001170: 635f 6e61 6d65 da08 6473 745f 6e61 6d65  c_name..dst_name
-00001180: da10 6167 656e 745f 7669 7369 6269 6c69  ..agent_visibili
-00001190: 7479 722e 0000 00da 0973 7263 5f61 6765  tyr......src_age
-000011a0: 6e74 da09 7372 635f 706f 696e 7472 4600  nt..src_pointrF.
-000011b0: 0000 da0c 7061 7273 6564 5f77 616c 6c73  ....parsed_walls
-000011c0: 7238 0000 00da 0876 6572 7469 6365 73da  r8.....vertices.
-000011d0: 0864 6973 7461 6e63 65da 0964 7374 5f61  .distance..dst_a
-000011e0: 6765 6e74 da0a 6973 5f76 6973 6962 6c65  gent..is_visible
-000011f0: da09 6473 745f 706f 696e 7473 0f00 0000  ..dst_points....
-00001200: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00001210: 1600 0000 722c 0000 007a 164d 6f64 656c  ....r,...z.Model
-00001220: 2e67 6574 5f6f 6273 6572 7661 7469 6f6e  .get_observation
-00001230: 7342 0000 0073 4102 0000 8000 d863 67d7  sB...sA......cg.
-00001240: 636e d163 6ed7 1b6f d057 5f98 48c0 64c7  cn.cn..o.W_.H.d.
-00001250: 6bc1 6bd6 2652 b828 a078 b014 a17e d226  k.k.&R.(.x...~.&
-00001260: 52d1 1c52 d01b 6fd0 0818 d11b 6fd8 1719  R..R..o.....o...
-00001270: 880c d823 27a7 3ba1 3bd7 2334 d123 34d3  ...#'.;.;.#4.#4.
-00001280: 2336 f300 1809 4c01 d10c 1f88 4890 69d8  #6....L.....H.i.
-00001290: 2527 884c 9818 d10c 22dc 181a 9f08 9908  %'.L....".......
-000012a0: a019 a71f a11f d721 39d1 2139 d318 3a88  .......!9.!9..:.
-000012b0: 49d8 2024 a70f a10f d720 41d1 2041 c069  I. $..... A. A.i
-000012c0: d020 41d3 2050 d00c 1dd8 1b1d 884c d833  . A. P.......L.3
-000012d0: 44f2 0001 0d6d 01d1 102f 900b 9858 a078  D....m.../...X.x
-000012e0: d810 1cd7 1023 d110 23a0 58a8 74d7 2f42  .....#..#.X.t./B
-000012f0: d12f 42c0 79d0 5e69 d02f 42d3 2f6a d024  ./B.y.^i./B./j.$
-00001300: 6bd5 106c f003 010d 6d01 e02e 3a88 4c98  k..l....m...:.L.
-00001310: 18d1 0c22 a037 d10c 2bd8 272b a77b a17b  ...".7..+.'+.{.{
-00001320: d727 38d1 2738 d327 3af2 000a 0d46 01d1  .'8.'8.':....F..
-00001330: 1023 9008 9829 d813 23a0 48d1 132d a868  .#...)..#.H..-.h
-00001340: d113 37d1 133f d817 1fa0 38d2 172b d825  ..7..?....8..+.%
-00001350: 2999 0ae4 2426 a748 a148 a859 af5f a95f  )...$&.H.H.Y._._
-00001360: d72d 45d1 2d45 d324 4698 09d8 2529 a75f  .-E.-E.$F...%)._
-00001370: a15f d725 42d1 2542 c079 d847 50d8 5566  ._.%B.%B.y.GP.Uf
-00001380: f005 0026 4301 f300 0226 6801 980a f006  ...&C....&h.....
-00001390: 003c 4601 d014 24a0 58d1 142e a878 d114  .<F...$.X....x..
-000013a0: 38d8 3b45 d014 24a0 58d1 142e a878 d214  8.;E..$.X....x..
-000013b0: 38f0 150a 0d46 01f0 1600 3638 884c 9818  8....F....68.L..
-000013c0: d10c 22a0 3ed1 0c32 d828 38d7 283e d128  ..".>..2.(8.(>.(
-000013d0: 3ed3 2840 f200 040d 4c01 d110 2490 0898  >.(@....L...$...
-000013e0: 2ad9 131d d847 4bc7 7bc1 7bd0 535b d147  *....GK.{.{.S[.G
-000013f0: 5cd7 4762 d147 62d7 476b d147 6bd0 6d71  \.Gb.Gb.Gk.Gk.mq
-00001400: d76d 78d1 6d78 f000 007a 0142 02f1 0000  .mx.mx...z.B....
-00001410: 6e01 4302 f700 006e 0149 02f1 0000 6e01  n.C....n.I....n.
-00001420: 4902 f700 006e 0153 02f1 0000 6e01 5302  I....n.S....n.S.
-00001430: f000 0048 0153 0290 4ca0 18d1 142a a83e  ...H.S..L....*.>
-00001440: d114 3ab8 38d2 1444 e047 4b90 4ca0 18d1  ..:.8..D.GK.L...
-00001450: 142a a83e d114 3ab8 38d2 1444 f209 040d  .*.>..:.8..D....
-00001460: 4c01 f029 1809 4c01 f032 0010 1cd0 081b  L..)..L..2......
-00001470: f9f2 3700 2753 01f9 d31b 6f73 1500 0000  ..7.'S....os....
-00001480: 9014 472d 06a4 0a47 280e ae05 472d 06c7  ..G-...G(...G-..
-00001490: 2805 472d 0672 2000 0000 da09 706f 6c79  (.G-.r .....poly
-000014a0: 676f 6e61 6c63 0300 0000 0000 0000 0000  gonalc..........
-000014b0: 0000 0800 0000 0300 0000 f38a 0300 0097  ................
-000014c0: 0069 007d 0374 0100 0000 0000 0000 006a  .i.}.t.........j
-000014d0: 0200 0000 0000 0000 0000 0000 0000 0000  ................
-000014e0: 0000 007c 006a 0400 0000 0000 0000 0000  ...|.j..........
-000014f0: 0000 0000 0000 0000 007c 0119 0000 006a  .........|.....j
-00001500: 0600 0000 0000 0000 0000 0000 0000 0000  ................
-00001510: 0000 006a 0800 0000 0000 0000 0000 0000  ...j............
-00001520: 0000 0000 0000 00ab 0100 0000 0000 007d  ...............}
-00001530: 047c 0272 457c 006a 0a00 0000 0000 0000  .|.rE|.j........
-00001540: 0000 0000 0000 0000 0000 006a 0d00 0000  ...........j....
-00001550: 0000 0000 0000 0000 0000 0000 0000 007c  ...............|
-00001560: 046a 0600 0000 0000 0000 0000 0000 0000  .j..............
-00001570: 0000 0000 006a 0800 0000 0000 0000 0000  .....j..........
-00001580: 0000 0000 0000 0000 007c 046a 0600 0000  .........|.j....
-00001590: 0000 0000 0000 0000 0000 0000 0000 006a  ...............j
-000015a0: 0e00 0000 0000 0000 0000 0000 0000 0000  ................
-000015b0: 0000 00ab 0200 0000 0000 007d 056e 1c7c  ...........}.n.|
-000015c0: 006a 0a00 0000 0000 0000 0000 0000 0000  .j..............
-000015d0: 0000 0000 006a 1100 0000 0000 0000 0000  .....j..........
-000015e0: 0000 0000 0000 0000 007c 04ac 01ab 0100  .........|......
-000015f0: 0000 0000 007d 0667 007d 077f 0644 005d  .....}.g.}...D.]
-00001600: 2a00 005c 0300 007d 087d 097d 0a7c 076a  *..\...}.}.}.|.j
-00001610: 1300 0000 0000 0000 0000 0000 0000 0000  ................
-00001620: 0000 007c 0a7c 006a 1500 0000 0000 0000  ...|.|.j........
-00001630: 0000 0000 0000 0000 0000 007c 047c 08ac  ...........|.|..
-00001640: 02ab 0200 0000 0000 0066 02ab 0100 0000  .........f......
-00001650: 0000 0001 008c 2c04 007c 077c 0364 033c  ......,..|.|.d.<
-00001660: 0000 0069 007c 0364 043c 0000 007c 006a  ...i.|.d.<...|.j
-00001670: 0400 0000 0000 0000 0000 0000 0000 0000  ................
-00001680: 0000 006a 1700 0000 0000 0000 0000 0000  ...j............
-00001690: 0000 0000 0000 00ab 0000 0000 0000 0044  ...............D
-000016a0: 005d cf00 005c 0200 007d 0b7d 0c7c 017c  .]...\...}.}.|.|
-000016b0: 0b6b 2800 0072 0364 057d 0d6e 6b74 0100  .k(..r.d.}.nkt..
-000016c0: 0000 0000 0000 006a 0200 0000 0000 0000  .......j........
-000016d0: 0000 0000 0000 0000 0000 007c 0c6a 0600  ...........|.j..
-000016e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000016f0: 006a 0800 0000 0000 0000 0000 0000 0000  .j..............
-00001700: 0000 0000 00ab 0100 0000 0000 007d 0e7c  .............}.|
-00001710: 0272 227c 0c6a 1900 0000 0000 0000 0000  .r"|.j..........
-00001720: 0000 0000 0000 0000 00ab 0000 0000 0000  ................
-00001730: 007d 0f7c 0f6a 1b00 0000 0000 0000 0000  .}.|.j..........
-00001740: 0000 0000 0000 0000 007f 05ab 0100 0000  ................
-00001750: 0000 007d 0d6e 1e7c 006a 0a00 0000 0000  ...}.n.|.j......
-00001760: 0000 0000 0000 0000 0000 0000 006a 1d00  .............j..
-00001770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001780: 007c 047c 0e7c 06ac 06ab 0300 0000 0000  .|.|.|..........
-00001790: 007d 0d7c 0d72 4d7c 006a 0400 0000 0000  .}.|.rM|.j......
-000017a0: 0000 0000 0000 0000 0000 0000 007c 0b19  .............|..
-000017b0: 0000 006a 0600 0000 0000 0000 0000 0000  ...j............
-000017c0: 0000 0000 0000 006a 0800 0000 0000 0000  .......j........
-000017d0: 0000 0000 0000 0000 0000 007c 006a 0400  ...........|.j..
-000017e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000017f0: 007c 0b19 0000 006a 0600 0000 0000 0000  .|.....j........
-00001800: 0000 0000 0000 0000 0000 006a 0e00 0000  ...........j....
-00001810: 0000 0000 0000 0000 0000 0000 0000 0066  ...............f
-00001820: 027c 0364 0419 0000 007c 0b3c 0000 008c  .|.d.....|.<....
-00001830: c864 007c 0364 0419 0000 007c 0b3c 0000  .d.|.d.....|.<..
-00001840: 008c d104 007c 0353 0029 074e 7241 0000  .....|.S.).NrA..
-00001850: 0072 4200 0000 7243 0000 0072 4700 0000  .rB...rC...rG...
-00001860: 5472 4400 0000 290f 723c 0000 0072 3d00  TrD...).r<...r=.
-00001870: 0000 720f 0000 0072 4800 0000 7249 0000  ..r....rH...rI..
-00001880: 0072 1000 0000 da16 6765 745f 7669 7369  .r......get_visi
-00001890: 6269 6c69 7479 5f70 6f6c 7967 6f6e 724c  bility_polygonrL
-000018a0: 0000 0072 4600 0000 724a 0000 0072 3f00  ...rF...rJ...r?.
-000018b0: 0000 721d 0000 00da 0b67 6574 5f70 6f6c  ..r......get_pol
-000018c0: 7967 6f6e 7234 0000 0072 4b00 0000 2910  ygonr4...rK...).
-000018d0: 7215 0000 0072 2000 0000 7258 0000 00da  r....r ...rX....
-000018e0: 0b6f 6273 6572 7661 7469 6f6e 7251 0000  .observationrQ..
-000018f0: 00da 1276 6973 6962 696c 6974 795f 706f  ...visibility_po
-00001900: 6c79 676f 6e72 4600 0000 7252 0000 0072  lygonrF...rR...r
-00001910: 3800 0000 7253 0000 0072 5400 0000 724e  8...rS...rT...rN
-00001920: 0000 0072 5500 0000 7256 0000 0072 5700  ...rU...rV...rW.
-00001930: 0000 da0b 6473 745f 706f 6c79 676f 6e73  ....dst_polygons
-00001940: 1000 0000 2020 2020 2020 2020 2020 2020  ....            
-00001950: 2020 2020 7216 0000 00da 0f67 6574 5f6f      r......get_o
-00001960: 6273 6572 7661 7469 6f6e 7a15 4d6f 6465  bservationz.Mode
-00001970: 6c2e 6765 745f 6f62 7365 7276 6174 696f  l.get_observatio
-00001980: 6e60 0000 0073 bd01 0000 8000 f006 0017  n`...s..........
-00001990: 1988 0bdc 1416 9748 9148 9854 9f5b 995b  .......H.H.T.[.[
-000019a0: a81a d11d 34d7 1d3a d11d 3ad7 1d43 d11d  ....4..:..:..C..
-000019b0: 43d3 1444 8809 d90b 14d8 2125 a71f a11f  C..D......!%....
-000019c0: d721 47d1 2147 c809 cf0f c90f d748 60d1  .!G.!G.......H`.
-000019d0: 4860 d062 6bd7 6271 d162 71d7 627b d162  H`.bk.bq.bq.b{.b
-000019e0: 7bd3 217c d10c 1ee0 2024 a70f a10f d720  {.!|.... $..... 
-000019f0: 41d1 2041 c069 d020 41d3 2050 d00c 1dd8  A. A.i. A. P....
-00001a00: 1719 880c d82f 40f2 0001 0969 01d1 0c2b  ...../@....i...+
-00001a10: 884b 9818 a038 d80c 18d7 0c1f d10c 1fa0  .K...8..........
-00001a20: 18a8 34d7 2b3e d12b 3ec0 39d0 5a65 d02b  ..4.+>.+>.9.Ze.+
-00001a30: 3ed3 2b66 d020 67d5 0c68 f003 0109 6901  >.+f. g..h....i.
-00001a40: e01f 2b88 0b90 47d1 081c d826 2888 0b90  ..+...G....&(...
-00001a50: 4ed1 0823 d823 27a7 3ba1 3bd7 2334 d123  N..#.#'.;.;.#4.#
-00001a60: 34d3 2336 f200 0f09 3dd1 0c1f 8848 9069  4.#6....=....H.i
-00001a70: d80f 1998 58d2 0f25 d81d 2191 0ae4 1c1e  ....X..%..!.....
-00001a80: 9f48 9948 a059 a75f a15f d725 3dd1 253d  .H.H.Y._._.%=.%=
-00001a90: d31c 3e90 09d9 131c d822 2bd7 2237 d122  ..>......"+."7."
-00001aa0: 37d3 2239 904b d821 2cd7 2137 d121 37d0  7."9.K.!,.!7.!7.
-00001ab0: 384a d321 4b91 4ae0 2125 a71f a11f d721  8J.!K.J.!%.....!
-00001ac0: 3ed1 213e c039 d843 4cd8 5162 f005 0022  >.!>.9.CL.Qb..."
-00001ad0: 3ff3 0002 2264 0190 4af1 0600 101a d838  ?..."d..J......8
-00001ae0: 3cbf 0bb9 0bc0 48d1 384d d738 53d1 3853  <.....H.8M.8S.8S
-00001af0: d738 5cd1 385c d05e 62d7 5e69 d15e 69d0  .8\.8\.^b.^i.^i.
-00001b00: 6a72 d15e 73d7 5e79 d15e 79f7 0000 5f01  jr.^s.^y.^y..._.
-00001b10: 4402 f100 005f 0144 02f0 0000 3944 0290  D...._.D....9D..
-00001b20: 0b98 4ed1 102b a848 d210 35e0 383c 900b  ..N..+.H..5.8<..
-00001b30: 984e d110 2ba8 48d2 1035 f01f 0f09 3df0  .N..+.H..5....=.
-00001b40: 2000 101b d008 1a72 1800 0000 6301 0000   ......r....c...
-00001b50: 0000 0000 0000 0000 0005 0000 0003 0000  ................
-00001b60: 00f3 de04 0000 9700 7c00 6a00 0000 0000  ........|.j.....
-00001b70: 0000 0000 0000 0000 0000 0000 0000 725e  ..............r^
-00001b80: 7c00 6a02 0000 0000 0000 0000 0000 0000  |.j.............
-00001b90: 0000 0000 0000 7c00 6a04 0000 0000 0000  ......|.j.......
-00001ba0: 0000 0000 0000 0000 0000 0000 7a00 0000  ............z...
-00001bb0: 7407 0000 0000 0000 0000 6a06 0000 0000  t.........j.....
-00001bc0: 0000 0000 0000 0000 0000 0000 0000 ab00  ................
-00001bd0: 0000 0000 0000 6b44 0000 7230 0900 7c00  ......kD..r0..|.
-00001be0: 6a02 0000 0000 0000 0000 0000 0000 0000  j...............
-00001bf0: 0000 0000 7c00 6a04 0000 0000 0000 0000  ....|.j.........
-00001c00: 0000 0000 0000 0000 0000 7a00 0000 7407  ..........z...t.
-00001c10: 0000 0000 0000 0000 6a06 0000 0000 0000  ........j.......
-00001c20: 0000 0000 0000 0000 0000 0000 ab00 0000  ................
-00001c30: 0000 0000 6b44 0000 7201 8c30 7407 0000  ....kD..r..0t...
-00001c40: 0000 0000 0000 6a06 0000 0000 0000 0000  ......j.........
-00001c50: 0000 0000 0000 0000 0000 ab00 0000 0000  ................
-00001c60: 0000 7c00 5f01 0000 0000 0000 0000 7c00  ..|._.........|.
-00001c70: 6a08 0000 0000 0000 0000 0000 0000 0000  j...............
-00001c80: 0000 0000 6a0b 0000 0000 0000 0000 0000  ....j...........
-00001c90: 0000 0000 0000 0000 ab00 0000 0000 0000  ................
-00001ca0: 4400 9001 5d4f 0000 5c02 0000 7d01 7d02  D...]O..\...}.}.
-00001cb0: 7c02 6a0c 0000 0000 0000 0000 0000 0000  |.j.............
-00001cc0: 0000 0000 0000 7d03 7c03 6a0f 0000 0000  ......}.|.j.....
-00001cd0: 0000 0000 0000 0000 0000 0000 0000 7c00  ..............|.
-00001ce0: 6a04 0000 0000 0000 0000 0000 0000 0000  j...............
-00001cf0: 0000 0000 ac01 ab01 0000 0000 0000 5c02  ..............\.
-00001d00: 0000 7d04 7d05 7c02 6a10 0000 0000 0000  ..}.}.|.j.......
-00001d10: 0000 0000 0000 0000 0000 0000 6a13 0000  ............j...
-00001d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d30: 7c05 7c04 ac02 ab02 0000 0000 0000 7d06  |.|...........}.
-00001d40: 7c02 6a15 0000 0000 0000 0000 0000 0000  |.j.............
-00001d50: 0000 0000 0000 7c06 ac03 ab01 0000 0000  ......|.........
-00001d60: 0000 7d07 7c00 6a17 0000 0000 0000 0000  ..}.|.j.........
-00001d70: 0000 0000 0000 0000 0000 7c07 7c02 6a18  ..........|.|.j.
-00001d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d90: 0000 ac04 ab02 0000 0000 0000 7213 7c02  ............r.|.
-00001da0: 6a1b 0000 0000 0000 0000 0000 0000 0000  j...............
-00001db0: 0000 0000 7c06 ac03 ab01 0000 0000 0000  ....|...........
-00001dc0: 0100 8c91 7c02 6a10 0000 0000 0000 0000  ....|.j.........
-00001dd0: 0000 0000 0000 0000 0000 6a13 0000 0000  ..........j.....
-00001de0: 0000 0000 0000 0000 0000 0000 0000 7c05  ..............|.
-00001df0: 6405 ac02 ab02 0000 0000 0000 7d06 7c02  d...........}.|.
-00001e00: 6a15 0000 0000 0000 0000 0000 0000 0000  j...............
-00001e10: 0000 0000 7c06 ac03 ab01 0000 0000 0000  ....|...........
-00001e20: 7d07 7c00 6a17 0000 0000 0000 0000 0000  }.|.j...........
-00001e30: 0000 0000 0000 0000 7c07 7c02 6a18 0000  ........|.|.j...
-00001e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e50: ac04 ab02 0000 0000 0000 7213 7c02 6a1b  ..........r.|.j.
-00001e60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001e70: 0000 7c06 ac03 ab01 0000 0000 0000 0100  ..|.............
-00001e80: 8cf0 7c02 6a10 0000 0000 0000 0000 0000  ..|.j...........
-00001e90: 0000 0000 0000 0000 6a13 0000 0000 0000  ........j.......
-00001ea0: 0000 0000 0000 0000 0000 0000 6405 7c04  ............d.|.
-00001eb0: ac02 ab02 0000 0000 0000 7d06 7c02 6a15  ..........}.|.j.
-00001ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ed0: 0000 7c06 ac03 ab01 0000 0000 0000 7d07  ..|...........}.
-00001ee0: 7c00 6a17 0000 0000 0000 0000 0000 0000  |.j.............
-00001ef0: 0000 0000 0000 7c07 7c02 6a18 0000 0000  ......|.|.j.....
-00001f00: 0000 0000 0000 0000 0000 0000 0000 ac04  ................
-00001f10: ab02 0000 0000 0000 7302 9001 8c3e 7c02  ........s....>|.
-00001f20: 6a1b 0000 0000 0000 0000 0000 0000 0000  j...............
-00001f30: 0000 0000 7c06 ac03 ab01 0000 0000 0000  ....|...........
-00001f40: 0100 9001 8c52 0400 7c00 6a08 0000 0000  .....R..|.j.....
-00001f50: 0000 0000 0000 0000 0000 0000 0000 6a0b  ..............j.
-00001f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f70: 0000 ab00 0000 0000 0000 4400 5d21 0000  ..........D.]!..
-00001f80: 5c02 0000 7d01 7d02 7c02 6a1d 0000 0000  \...}.}.|.j.....
-00001f90: 0000 0000 0000 0000 0000 0000 0000 7c00  ..............|.
-00001fa0: 6a04 0000 0000 0000 0000 0000 0000 0000  j...............
-00001fb0: 0000 0000 ac01 ab01 0000 0000 0000 0100  ................
-00001fc0: 8c23 0400 7c00 7801 6a06 0000 0000 0000  .#..|.x.j.......
-00001fd0: 0000 0000 0000 0000 0000 0000 7c00 6a04  ............|.j.
-00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001ff0: 0000 7a0d 0000 6302 5f03 0000 0000 0000  ..z...c._.......
-00002000: 0000 7c00 7801 6a1e 0000 0000 0000 0000  ..|.x.j.........
-00002010: 0000 0000 0000 0000 0000 6406 7a0d 0000  ..........d.z...
-00002020: 6302 5f0f 0000 0000 0000 0000 7c00 6a04  c._.........|.j.
-00002030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002040: 0000 5300 2907 4e29 0172 1a00 0000 2902  ..S.).N).r....).
-00002050: da08 726f 7461 7469 6f6e 7254 0000 0029  ..rotationrT...)
-00002060: 0172 4800 0000 2902 722f 0000 0072 3000  .rH...).r/...r0.
-00002070: 0000 7202 0000 0072 0300 0000 2910 720a  ..r....r....).r.
-00002080: 0000 0072 1100 0000 720b 0000 0072 1200  ...r....r....r..
-00002090: 0000 720f 0000 0072 1d00 0000 da08 6479  ..r....r......dy
-000020a0: 6e61 6d69 6373 da06 6368 616e 6765 7248  namics..changerH
-000020b0: 0000 00da 0675 7064 6174 6572 5b00 0000  .....updater[...
-000020c0: 7236 0000 00da 0963 6f6c 6c69 7369 6f6e  r6.....collision
-000020d0: 721e 0000 00da 0473 7465 7072 1400 0000  r......stepr....
-000020e0: 2908 7215 0000 0072 2500 0000 7226 0000  ).r....r%...r&..
-000020f0: 0072 6200 0000 7254 0000 0072 6100 0000  .rb...rT...ra...
-00002100: da09 6e65 775f 7374 6174 6572 2f00 0000  ..new_stater/...
-00002110: 7308 0000 0020 2020 2020 2020 2072 1600  s....        r..
-00002120: 0000 7266 0000 007a 0a4d 6f64 656c 2e73  ..rf...z.Model.s
-00002130: 7465 7080 0000 0073 0702 0000 8000 d80b  tep....s........
-00002140: 0f8f 3e8a 3ed8 1216 972e 912e a034 a73e  ..>.>........4.>
-00002150: a13e d112 31b4 44b7 49b1 49b3 4bd2 123f  .>..1.D.I.I.K..?
-00002160: d810 14f0 0300 1317 972e 912e a034 a73e  .............4.>
-00002170: a13e d112 31b4 44b7 49b1 49b3 4bd3 123f  .>..1.D.I.I.K..?
-00002180: f406 001a 1e9f 1999 199b 1b88 048c 0ed8  ................
-00002190: 1b1f 9f3b 993b d71b 2cd1 1b2c d31b 2ef3  ...;.;..,..,....
-000021a0: 0016 0939 894b 8844 9025 d817 1c97 7e91  ...9.K.D.%....~.
-000021b0: 7e88 48d8 2129 a71f a11f b814 bf1e b91e  ~.H.!)..........
-000021c0: a01f d321 48d1 0c1e 8848 9068 d818 1d9f  ...!H....H.h....
-000021d0: 0b99 0bd7 182a d118 2ab0 48d8 343c f003  .....*..*.H.4<..
-000021e0: 0019 2bf3 0001 193e 8849 e01c 21d7 1c2d  ..+....>.I..!..-
-000021f0: d11c 2db0 49d0 1c2d d31c 3e88 4dd8 0f13  ..-.I..-..>.M...
-00002200: d70f 22d1 0f22 b01d d82e 33af 6fa9 6ff0  ..".."....3.o.o.
-00002210: 0300 1023 f400 0110 3fe0 1015 970f 910f  ...#....?.......
-00002220: a069 900f d510 30e0 1c21 9f4b 994b d71c  .i....0..!.K.K..
-00002230: 2ed1 1c2e b808 d838 39f0 0300 1d2f f300  .......89..../..
-00002240: 011d 3b90 09e0 2025 d720 31d1 2031 b809  ..;... %. 1. 1..
-00002250: d020 31d3 2042 900d d813 17d7 1326 d113  . 1. B.......&..
-00002260: 26b0 5dd8 3237 b72f b12f f003 0014 27f4  &.].27././....'.
-00002270: 0001 1443 01e0 1419 974f 914f a829 904f  ...C.....O.O.).O
-00002280: d514 34e0 2025 a70b a10b d720 32d1 2032  ..4. %..... 2. 2
-00002290: b841 d83c 44f0 0300 2133 f300 0121 4601  .A.<D...!3...!F.
-000022a0: 9049 e024 29d7 2435 d124 35b8 49d0 2435  .I.$).$5.$5.I.$5
-000022b0: d324 4690 4dd8 171b d717 2ad1 172a b81d  .$F.M.....*..*..
-000022c0: d836 3bb7 6fb1 6ff0 0300 182b f600 0118  .6;.o.o....+....
-000022d0: 4701 e018 1d9f 0f99 0fa8 6998 0fd6 1838  G.........i....8
-000022e0: f02d 1609 39f0 2e00 1c20 9f3b 993b d71b  .-..9.... .;.;..
-000022f0: 2cd1 1b2c d31b 2ef2 0001 092f 894b 8844  ,..,......./.K.D
-00002300: 9025 d80c 118f 4a89 4a98 749f 7e99 7e88  .%....J.J.t.~.~.
-00002310: 4ad5 0c2e f003 0109 2fe0 080c 8f09 8a09  J......./.......
-00002320: 9054 975e 915e d108 238d 09d8 080c 8f0f  .T.^.^..#.......
-00002330: 8a0f 9831 d108 1c8d 0fd8 0f13 8f7e 897e  ...1.........~.~
-00002340: d008 1d72 1800 0000 4e29 0246 679a 9999  ...r....N).Fg...
-00002350: 9999 99b9 3f29 0172 0200 0000 2901 4629  ....?).r....).F)
-00002360: 19da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00002370: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00002380: 616d 655f 5fda 0462 6f6f 6cda 0566 6c6f  ame__..bool..flo
-00002390: 6174 7217 0000 00da 0674 7970 696e 67da  atr......typing.
-000023a0: 0444 6963 74da 0373 7472 7205 0000 0072  .Dict..strr....r
-000023b0: 2200 0000 721f 0000 0072 0400 0000 7229  "...r....r....r)
-000023c0: 0000 0072 2b00 0000 723c 0000 00da 0750  ...r+...r<.....P
-000023d0: 6f6c 7967 6f6e 7236 0000 00da 0554 7570  olygonr6.....Tup
-000023e0: 6c65 da03 696e 7472 3f00 0000 722c 0000  le..intr?...r,..
-000023f0: 00da 0464 6963 7472 5f00 0000 7266 0000  ...dictr_...rf..
-00002400: 0072 2400 0000 7218 0000 0072 1600 0000  .r$...r....r....
-00002410: 7209 0000 0072 0900 0000 0a00 0000 73e9  r....r........s.
-00002420: 0000 0084 00f0 0a00 2429 d824 27f1 090e  ........$).$'...
-00002430: 051c f006 001d 21f0 070e 051c f008 001d  ......!.........
-00002440: 22f3 090e 051c f022 002b 2cf1 0305 0527  "......".+,....'
-00002450: a856 af5b a95b b813 b86a b81f d12d 49f0  .V.[.[...j...-I.
-00002460: 0005 0527 d822 27f3 0305 0527 f010 002b  ...'."'....'...+
-00002470: 2cf1 0302 050d d822 27f3 0302 050d f008  ,......"'.......
-00002480: 0305 1b98 63f0 0003 051b a825 f300 0305  ....c......%....
-00002490: 1bf2 0a08 051c f014 0705 14a8 42af 4aa9  ............B.J.
-000024a0: 4af0 0007 0514 c044 f000 0705 14c8 54f3  J......D......T.
-000024b0: 0007 0514 f012 0105 6001 a026 a72c a12c  ........`..&.,.,
-000024c0: a875 b065 a87c d122 3cf0 0001 0560 01c8  .u.e.|."<....`..
-000024d0: 33f3 0001 0560 01f2 061c 051c f040 0100  3....`.......@..
-000024e0: 2b30 f105 1e05 1bd8 2427 f003 1e05 1be0  +0......$'......
-000024f0: 2327 f005 1e05 1be0 3438 f305 1e05 1bf0  #'......48......
-00002500: 4001 2105 1e90 65f4 0021 051e 7218 0000  @.!...e..!..r...
-00002510: 0072 0900 0000 290e 723a 0000 0072 1200  .r....).r:...r..
-00002520: 0000 726d 0000 00da 0773 6861 7065 6c79  ..rm.....shapely
-00002530: 723c 0000 0072 2600 0000 7204 0000 0072  r<...r&...r....r
-00002540: 0500 0000 7210 0000 0072 0600 0000 da08  ....r....r......
-00002550: 6765 6f6d 6574 7279 7207 0000 00da 066f  geometryr......o
-00002560: 626a 6563 7472 0900 0000 7224 0000 0072  bjectr....r$...r
-00002570: 1800 0000 7216 0000 00fa 083c 6d6f 6475  ....r......<modu
-00002580: 6c65 3e72 7700 0000 0100 0000 7328 0000  le>rw.......s(..
-00002590: 00f0 0301 0101 db00 0bdb 000b db00 0ddb  ................
-000025a0: 0014 df00 24dd 0022 dd00 1bf4 0657 0201  ....$..".....W..
-000025b0: 1e88 46f5 0057 0201 1e72 1800 0000       ..F..W...r....
+00000b90: ab00 0000 0000 0000 4400 5d6d 0000 5c02  ........D.]m..\.
+00000ba0: 0000 7d02 7d0c 7c03 7c01 1900 0000 7c02  ..}.}.|.|.....|.
+00000bb0: 1900 0000 8101 8c0f 7c01 7c02 6b28 0000  ........|.|.k(..
+00000bc0: 7203 6404 7d0d 6e47 7405 0000 0000 0000  r.d.}.nGt.......
+00000bd0: 0000 6a06 0000 0000 0000 0000 0000 0000  ..j.............
+00000be0: 0000 0000 0000 7c0c 6a08 0000 0000 0000  ......|.j.......
+00000bf0: 0000 0000 0000 0000 0000 0000 6a0a 0000  ............j...
+00000c00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000c10: ab01 0000 0000 0000 7d0e 7c00 6a0c 0000  ........}.|.j...
+00000c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000c30: 6a15 0000 0000 0000 0000 0000 0000 0000  j...............
+00000c40: 0000 0000 7c06 7c0e 7c07 ac05 ab03 0000  ....|.|.|.......
+00000c50: 0000 0000 7d0d 7c0d 7c03 7c01 1900 0000  ....}.|.|.|.....
+00000c60: 7c02 3c00 0000 7c0d 7c03 7c02 1900 0000  |.<...|.|.|.....
+00000c70: 7c01 3c00 0000 8c6f 0400 6900 7c04 7c01  |.<....o..i.|.|.
+00000c80: 1900 0000 6406 3c00 0000 7c03 6a03 0000  ....d.<...|.j...
+00000c90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000ca0: ab00 0000 0000 0000 4400 5d62 0000 5c02  ........D.]b..\.
+00000cb0: 0000 7d02 7d0d 7c0d 7250 7c00 6a00 0000  ..}.}.|.rP|.j...
+00000cc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000cd0: 7c02 1900 0000 6a08 0000 0000 0000 0000  |.....j.........
+00000ce0: 0000 0000 0000 0000 0000 6a0a 0000 0000  ..........j.....
+00000cf0: 0000 0000 0000 0000 0000 0000 0000 7c00  ..............|.
+00000d00: 6a00 0000 0000 0000 0000 0000 0000 0000  j...............
+00000d10: 0000 0000 7c02 1900 0000 6a08 0000 0000  ....|.....j.....
+00000d20: 0000 0000 0000 0000 0000 0000 0000 6a16  ..............j.
+00000d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000d40: 0000 6602 7c04 7c01 1900 0000 6406 1900  ..f.|.|.....d...
+00000d50: 0000 7c02 3c00 0000 8c58 6400 7c04 7c01  ..|.<....Xd.|.|.
+00000d60: 1900 0000 6406 1900 0000 7c02 3c00 0000  ....d.....|.<...
+00000d70: 8c64 0400 9001 8c93 0400 7c04 5300 6302  .d........|.S.c.
+00000d80: 0100 6302 7d02 7700 6302 0100 6303 7d02  ..c.}.w.c...c.}.
+00000d90: 7d01 7700 2907 4ea9 0172 2a00 0000 a902  }.w.).N..r*.....
+00000da0: 722a 0000 0072 2b00 0000 da05 7761 6c6c  r*...r+.....wall
+00000db0: 7354 a903 722a 0000 00da 0364 7374 da11  sT..r*.....dst..
+00000dc0: 7761 6c6c 735f 6279 5f64 6973 7461 6e63  walls_by_distanc
+00000dd0: 65da 0c61 6765 6e74 5f73 7461 7465 7329  e..agent_states)
+00000de0: 0c72 0e00 0000 721c 0000 0072 2f00 0000  .r....r....r/...
+00000df0: 7230 0000 00da 0573 7461 7465 da08 6c6f  r0.....state..lo
+00000e00: 6361 7469 6f6e 720f 0000 0072 3900 0000  cationr....r9...
+00000e10: da06 6170 7065 6e64 7232 0000 00da 0d6c  ..appendr2.....l
+00000e20: 696e 655f 6f66 5f73 6967 6874 da09 6469  ine_of_sight..di
+00000e30: 7265 6374 696f 6e29 0f72 1100 0000 da08  rection).r......
+00000e40: 7372 635f 6e61 6d65 da08 6473 745f 6e61  src_name..dst_na
+00000e50: 6d65 da10 6167 656e 745f 7669 7369 6269  me..agent_visibi
+00000e60: 6c69 7479 7221 0000 00da 0973 7263 5f61  lityr!.....src_a
+00000e70: 6765 6e74 da09 7372 635f 706f 696e 7472  gent..src_pointr
+00000e80: 3900 0000 da0c 7061 7273 6564 5f77 616c  9.....parsed_wal
+00000e90: 6c73 722b 0000 00da 0876 6572 7469 6365  lsr+.....vertice
+00000ea0: 73da 0864 6973 7461 6e63 65da 0964 7374  s..distance..dst
+00000eb0: 5f61 6765 6e74 da0a 6973 5f76 6973 6962  _agent..is_visib
+00000ec0: 6c65 da09 6473 745f 706f 696e 7473 0f00  le..dst_points..
+00000ed0: 0000 2020 2020 2020 2020 2020 2020 2020  ..              
+00000ee0: 2072 1200 0000 721e 0000 007a 164d 6f64   r....r....z.Mod
+00000ef0: 656c 2e67 6574 5f6f 6273 6572 7661 7469  el.get_observati
+00000f00: 6f6e 7332 0000 0073 4102 0000 8000 d863  ons2...sA......c
+00000f10: 67d7 636e d163 6ed7 1b6f d057 5f98 48c0  g.cn.cn..o.W_.H.
+00000f20: 64c7 6bc1 6bd6 2652 b828 a078 b014 a17e  d.k.k.&R.(.x...~
+00000f30: d226 52d1 1c52 d01b 6fd0 0818 d11b 6fd8  .&R..R..o.....o.
+00000f40: 1719 880c d823 27a7 3ba1 3bd7 2334 d123  .....#'.;.;.#4.#
+00000f50: 34d3 2336 f300 1809 4c01 d10c 1f88 4890  4.#6....L.....H.
+00000f60: 69d8 2527 884c 9818 d10c 22dc 181a 9f08  i.%'.L....".....
+00000f70: 9908 a019 a71f a11f d721 39d1 2139 d318  .........!9.!9..
+00000f80: 3a88 49d8 2024 a70f a10f d720 41d1 2041  :.I. $..... A. A
+00000f90: c069 d020 41d3 2050 d00c 1dd8 1b1d 884c  .i. A. P.......L
+00000fa0: d833 44f2 0001 0d6d 01d1 102f 900b 9858  .3D....m.../...X
+00000fb0: a078 d810 1cd7 1023 d110 23a0 58a8 74d7  .x.....#..#.X.t.
+00000fc0: 2f42 d12f 42c0 79d0 5e69 d02f 42d3 2f6a  /B./B.y.^i./B./j
+00000fd0: d024 6bd5 106c f003 010d 6d01 e02e 3a88  .$k..l....m...:.
+00000fe0: 4c98 18d1 0c22 a037 d10c 2bd8 272b a77b  L....".7..+.'+.{
+00000ff0: a17b d727 38d1 2738 d327 3af2 000a 0d46  .{.'8.'8.':....F
+00001000: 01d1 1023 9008 9829 d813 23a0 48d1 132d  ...#...)..#.H..-
+00001010: a868 d113 37d1 133f d817 1fa0 38d2 172b  .h..7..?....8..+
+00001020: d825 2999 0ae4 2426 a748 a148 a859 af5f  .%)...$&.H.H.Y._
+00001030: a95f d72d 45d1 2d45 d324 4698 09d8 2529  ._.-E.-E.$F...%)
+00001040: a75f a15f d725 42d1 2542 c079 d847 50d8  ._._.%B.%B.y.GP.
+00001050: 5566 f005 0026 4301 f300 0226 6801 980a  Uf...&C....&h...
+00001060: f006 003c 4601 d014 24a0 58d1 142e a878  ...<F...$.X....x
+00001070: d114 38d8 3b45 d014 24a0 58d1 142e a878  ..8.;E..$.X....x
+00001080: d214 38f0 150a 0d46 01f0 1600 3638 884c  ..8....F....68.L
+00001090: 9818 d10c 22a0 3ed1 0c32 d828 38d7 283e  ....".>..2.(8.(>
+000010a0: d128 3ed3 2840 f200 040d 4c01 d110 2490  .(>.(@....L...$.
+000010b0: 0898 2ad9 131d d847 4bc7 7bc1 7bd0 535b  ..*....GK.{.{.S[
+000010c0: d147 5cd7 4762 d147 62d7 476b d147 6bd0  .G\.Gb.Gb.Gk.Gk.
+000010d0: 6d71 d76d 78d1 6d78 f000 007a 0142 02f1  mq.mx.mx...z.B..
+000010e0: 0000 6e01 4302 f700 006e 0149 02f1 0000  ..n.C....n.I....
+000010f0: 6e01 4902 f700 006e 0153 02f1 0000 6e01  n.I....n.S....n.
+00001100: 5302 f000 0048 0153 0290 4ca0 18d1 142a  S....H.S..L....*
+00001110: a83e d114 3ab8 38d2 1444 e047 4b90 4ca0  .>..:.8..D.GK.L.
+00001120: 18d1 142a a83e d114 3ab8 38d2 1444 f209  ...*.>..:.8..D..
+00001130: 040d 4c01 f029 1809 4c01 f032 0010 1cd0  ..L..)..L..2....
+00001140: 081b f9f2 3700 2753 01f9 d31b 6f73 1500  ....7.'S....os..
+00001150: 0000 9014 472d 06a4 0a47 280e ae05 472d  ....G-...G(...G-
+00001160: 06c7 2805 472d 06da 0a61 6765 6e74 5f6e  ..(.G-...agent_n
+00001170: 616d 65da 0970 6f6c 7967 6f6e 616c 6303  ame..polygonalc.
+00001180: 0000 0000 0000 0000 0000 0008 0000 0003  ................
+00001190: 0000 00f3 8a03 0000 9700 6900 7d03 7401  ..........i.}.t.
+000011a0: 0000 0000 0000 0000 6a02 0000 0000 0000  ........j.......
+000011b0: 0000 0000 0000 0000 0000 0000 7c00 6a04  ............|.j.
+000011c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000011d0: 0000 7c01 1900 0000 6a06 0000 0000 0000  ..|.....j.......
+000011e0: 0000 0000 0000 0000 0000 0000 6a08 0000  ............j...
+000011f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001200: ab01 0000 0000 0000 7d04 7c02 7245 7c00  ........}.|.rE|.
+00001210: 6a0a 0000 0000 0000 0000 0000 0000 0000  j...............
+00001220: 0000 0000 6a0d 0000 0000 0000 0000 0000  ....j...........
+00001230: 0000 0000 0000 0000 7c04 6a06 0000 0000  ........|.j.....
+00001240: 0000 0000 0000 0000 0000 0000 0000 6a08  ..............j.
+00001250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001260: 0000 7c04 6a06 0000 0000 0000 0000 0000  ..|.j...........
+00001270: 0000 0000 0000 0000 6a0e 0000 0000 0000  ........j.......
+00001280: 0000 0000 0000 0000 0000 0000 ab02 0000  ................
+00001290: 0000 0000 7d05 6e1c 7c00 6a0a 0000 0000  ....}.n.|.j.....
+000012a0: 0000 0000 0000 0000 0000 0000 0000 6a11  ..............j.
+000012b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000012c0: 0000 7c04 ac01 ab01 0000 0000 0000 7d06  ..|...........}.
+000012d0: 6700 7d07 7f06 4400 5d2a 0000 5c03 0000  g.}...D.]*..\...
+000012e0: 7d08 7d09 7d0a 7c07 6a13 0000 0000 0000  }.}.}.|.j.......
+000012f0: 0000 0000 0000 0000 0000 0000 7c0a 7c00  ............|.|.
+00001300: 6a15 0000 0000 0000 0000 0000 0000 0000  j...............
+00001310: 0000 0000 7c04 7c08 ac02 ab02 0000 0000  ....|.|.........
+00001320: 0000 6602 ab01 0000 0000 0000 0100 8c2c  ..f............,
+00001330: 0400 7c07 7c03 6403 3c00 0000 6900 7c03  ..|.|.d.<...i.|.
+00001340: 6404 3c00 0000 7c00 6a04 0000 0000 0000  d.<...|.j.......
+00001350: 0000 0000 0000 0000 0000 0000 6a17 0000  ............j...
+00001360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001370: ab00 0000 0000 0000 4400 5dcf 0000 5c02  ........D.]...\.
+00001380: 0000 7d0b 7d0c 7c01 7c0b 6b28 0000 7203  ..}.}.|.|.k(..r.
+00001390: 6405 7d0d 6e6b 7401 0000 0000 0000 0000  d.}.nkt.........
+000013a0: 6a02 0000 0000 0000 0000 0000 0000 0000  j...............
+000013b0: 0000 0000 7c0c 6a06 0000 0000 0000 0000  ....|.j.........
+000013c0: 0000 0000 0000 0000 0000 6a08 0000 0000  ..........j.....
+000013d0: 0000 0000 0000 0000 0000 0000 0000 ab01  ................
+000013e0: 0000 0000 0000 7d0e 7c02 7222 7c0c 6a19  ......}.|.r"|.j.
+000013f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001400: 0000 ab00 0000 0000 0000 7d0f 7c0f 6a1b  ..........}.|.j.
+00001410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001420: 0000 7f05 ab01 0000 0000 0000 7d0d 6e1e  ............}.n.
+00001430: 7c00 6a0a 0000 0000 0000 0000 0000 0000  |.j.............
+00001440: 0000 0000 0000 6a1d 0000 0000 0000 0000  ......j.........
+00001450: 0000 0000 0000 0000 0000 7c04 7c0e 7c06  ..........|.|.|.
+00001460: ac06 ab03 0000 0000 0000 7d0d 7c0d 724d  ..........}.|.rM
+00001470: 7c00 6a04 0000 0000 0000 0000 0000 0000  |.j.............
+00001480: 0000 0000 0000 7c0b 1900 0000 6a06 0000  ......|.....j...
+00001490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000014a0: 6a08 0000 0000 0000 0000 0000 0000 0000  j...............
+000014b0: 0000 0000 7c00 6a04 0000 0000 0000 0000  ....|.j.........
+000014c0: 0000 0000 0000 0000 0000 7c0b 1900 0000  ..........|.....
+000014d0: 6a06 0000 0000 0000 0000 0000 0000 0000  j...............
+000014e0: 0000 0000 6a0e 0000 0000 0000 0000 0000  ....j...........
+000014f0: 0000 0000 0000 0000 6602 7c03 6404 1900  ........f.|.d...
+00001500: 0000 7c0b 3c00 0000 8cc8 6400 7c03 6404  ..|.<.....d.|.d.
+00001510: 1900 0000 7c0b 3c00 0000 8cd1 0400 7c03  ....|.<.......|.
+00001520: 5300 2907 4e72 3400 0000 7235 0000 0072  S.).Nr4...r5...r
+00001530: 3600 0000 723a 0000 0054 7237 0000 0029  6...r:...Tr7...)
+00001540: 0f72 2f00 0000 7230 0000 0072 0e00 0000  .r/...r0...r....
+00001550: 723b 0000 0072 3c00 0000 720f 0000 00da  r;...r<...r.....
+00001560: 1667 6574 5f76 6973 6962 696c 6974 795f  .get_visibility_
+00001570: 706f 6c79 676f 6e72 3f00 0000 7239 0000  polygonr?...r9..
+00001580: 0072 3d00 0000 7232 0000 0072 1c00 0000  .r=...r2...r....
+00001590: da0b 6765 745f 706f 6c79 676f 6e72 2700  ..get_polygonr'.
+000015a0: 0000 723e 0000 0029 1072 1100 0000 724b  ..r>...).r....rK
+000015b0: 0000 0072 4c00 0000 da0b 6f62 7365 7276  ...rL.....observ
+000015c0: 6174 696f 6e72 4400 0000 da12 7669 7369  ationrD.....visi
+000015d0: 6269 6c69 7479 5f70 6f6c 7967 6f6e 7239  bility_polygonr9
+000015e0: 0000 0072 4500 0000 722b 0000 0072 4600  ...rE...r+...rF.
+000015f0: 0000 7247 0000 0072 4100 0000 7248 0000  ..rG...rA...rH..
+00001600: 0072 4900 0000 724a 0000 00da 0b64 7374  .rI...rJ.....dst
+00001610: 5f70 6f6c 7967 6f6e 7310 0000 0020 2020  _polygons....   
+00001620: 2020 2020 2020 2020 2020 2020 2072 1200               r..
+00001630: 0000 da0f 6765 745f 6f62 7365 7276 6174  ....get_observat
+00001640: 696f 6e7a 154d 6f64 656c 2e67 6574 5f6f  ionz.Model.get_o
+00001650: 6273 6572 7661 7469 6f6e 5000 0000 73bd  bservationP...s.
+00001660: 0100 0080 00f0 0600 1719 880b dc14 1697  ................
+00001670: 4891 4898 549f 5b99 5ba8 1ad1 1d34 d71d  H.H.T.[.[....4..
+00001680: 3ad1 1d3a d71d 43d1 1d43 d314 4488 09d9  :..:..C..C..D...
+00001690: 0b14 d821 25a7 1fa1 1fd7 2147 d121 47c8  ...!%.....!G.!G.
+000016a0: 09cf 0fc9 0fd7 4860 d148 60d0 626b d762  ......H`.H`.bk.b
+000016b0: 71d1 6271 d762 7bd1 627b d321 7cd1 0c1e  q.bq.b{.b{.!|...
+000016c0: e020 24a7 0fa1 0fd7 2041 d120 41c0 69d0  . $..... A. A.i.
+000016d0: 2041 d320 50d0 0c1d d817 1988 0cd8 2f40   A. P........./@
+000016e0: f200 0109 6901 d10c 2b88 4b98 18a0 38d8  ....i...+.K...8.
+000016f0: 0c18 d70c 1fd1 0c1f a018 a834 d72b 3ed1  ...........4.+>.
+00001700: 2b3e c039 d05a 65d0 2b3e d32b 66d0 2067  +>.9.Ze.+>.+f. g
+00001710: d50c 68f0 0301 0969 01e0 1f2b 880b 9047  ..h....i...+...G
+00001720: d108 1cd8 2628 880b 904e d108 23d8 2327  ....&(...N..#.#'
+00001730: a73b a13b d723 34d1 2334 d323 36f2 000f  .;.;.#4.#4.#6...
+00001740: 093d d10c 1f88 4890 69d8 0f19 9858 d20f  .=....H.i....X..
+00001750: 25d8 1d21 910a e41c 1e9f 4899 48a0 59a7  %..!......H.H.Y.
+00001760: 5fa1 5fd7 253d d125 3dd3 1c3e 9009 d913  _._.%=.%=..>....
+00001770: 1cd8 222b d722 37d1 2237 d322 3990 4bd8  .."+."7."7."9.K.
+00001780: 212c d721 37d1 2137 d038 4ad3 214b 914a  !,.!7.!7.8J.!K.J
+00001790: e021 25a7 1fa1 1fd7 213e d121 3ec0 39d8  .!%.....!>.!>.9.
+000017a0: 434c d851 62f0 0500 223f f300 0222 6401  CL.Qb..."?..."d.
+000017b0: 904a f106 0010 1ad8 383c bf0b b90b c048  .J......8<.....H
+000017c0: d138 4dd7 3853 d138 53d7 385c d138 5cd0  .8M.8S.8S.8\.8\.
+000017d0: 5e62 d75e 69d1 5e69 d06a 72d1 5e73 d75e  ^b.^i.^i.jr.^s.^
+000017e0: 79d1 5e79 f700 005f 0144 02f1 0000 5f01  y.^y..._.D...._.
+000017f0: 4402 f000 0039 4402 900b 984e d110 2ba8  D....9D....N..+.
+00001800: 48d2 1035 e038 3c90 0b98 4ed1 102b a848  H..5.8<...N..+.H
+00001810: d210 35f0 1f0f 093d f020 0010 1bd0 081a  ..5....=. ......
+00001820: 7214 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00001830: 0000 0500 0000 0300 0000 f31e 0400 0097  ................
+00001840: 007c 006a 0000 0000 0000 0000 0000 0000  .|.j............
+00001850: 0000 0000 0000 0072 5e7c 006a 0200 0000  .......r^|.j....
+00001860: 0000 0000 0000 0000 0000 0000 0000 007c  ...............|
+00001870: 006a 0400 0000 0000 0000 0000 0000 0000  .j..............
+00001880: 0000 0000 007a 0000 0074 0700 0000 0000  .....z...t......
+00001890: 0000 006a 0600 0000 0000 0000 0000 0000  ...j............
+000018a0: 0000 0000 0000 00ab 0000 0000 0000 006b  ...............k
+000018b0: 4400 0072 3009 007c 006a 0200 0000 0000  D..r0..|.j......
+000018c0: 0000 0000 0000 0000 0000 0000 007c 006a  .............|.j
+000018d0: 0400 0000 0000 0000 0000 0000 0000 0000  ................
+000018e0: 0000 007a 0000 0074 0700 0000 0000 0000  ...z...t........
+000018f0: 006a 0600 0000 0000 0000 0000 0000 0000  .j..............
+00001900: 0000 0000 00ab 0000 0000 0000 006b 4400  .............kD.
+00001910: 0072 018c 3074 0700 0000 0000 0000 006a  .r..0t.........j
+00001920: 0600 0000 0000 0000 0000 0000 0000 0000  ................
+00001930: 0000 00ab 0000 0000 0000 007c 005f 0100  ...........|._..
+00001940: 0000 0000 0000 007c 006a 0800 0000 0000  .......|.j......
+00001950: 0000 0000 0000 0000 0000 0000 006a 0b00  .............j..
+00001960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001970: 00ab 0000 0000 0000 0044 0090 015d 2e00  .........D...]..
+00001980: 005c 0200 007d 017d 027c 026a 0c00 0000  .\...}.}.|.j....
+00001990: 0000 0000 0000 0000 0000 0000 0000 007d  ...............}
+000019a0: 037c 036a 0f00 0000 0000 0000 0000 0000  .|.j............
+000019b0: 0000 0000 0000 007c 006a 0400 0000 0000  .......|.j......
+000019c0: 0000 0000 0000 0000 0000 0000 00ac 01ab  ................
+000019d0: 0100 0000 0000 005c 0200 007d 047d 057c  .......\...}.}.|
+000019e0: 026a 1000 0000 0000 0000 0000 0000 0000  .j..............
+000019f0: 0000 0000 006a 1300 0000 0000 0000 0000  .....j..........
+00001a00: 0000 0000 0000 0000 007c 057c 04ac 02ab  .........|.|....
+00001a10: 0200 0000 0000 007d 067c 026a 1500 0000  .......}.|.j....
+00001a20: 0000 0000 0000 0000 0000 0000 0000 007c  ...............|
+00001a30: 06ac 03ab 0100 0000 0000 007d 077c 006a  ...........}.|.j
+00001a40: 1700 0000 0000 0000 0000 0000 0000 0000  ................
+00001a50: 0000 007c 077c 026a 1800 0000 0000 0000  ...|.|.j........
+00001a60: 0000 0000 0000 0000 0000 00ac 04ab 0200  ................
+00001a70: 0000 0000 0072 087c 067c 025f 0800 0000  .....r.|.|._....
+00001a80: 0000 0000 008c 867c 026a 1000 0000 0000  .......|.j......
+00001a90: 0000 0000 0000 0000 0000 0000 006a 1300  .............j..
+00001aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ab0: 007c 0564 05ac 02ab 0200 0000 0000 007d  .|.d...........}
+00001ac0: 067c 026a 1500 0000 0000 0000 0000 0000  .|.j............
+00001ad0: 0000 0000 0000 007c 06ac 03ab 0100 0000  .......|........
+00001ae0: 0000 007d 077c 006a 1700 0000 0000 0000  ...}.|.j........
+00001af0: 0000 0000 0000 0000 0000 007c 077c 026a  ...........|.|.j
+00001b00: 1800 0000 0000 0000 0000 0000 0000 0000  ................
+00001b10: 0000 00ac 04ab 0200 0000 0000 0072 087c  .............r.|
+00001b20: 067c 025f 0800 0000 0000 0000 008c da7c  .|._...........|
+00001b30: 026a 1000 0000 0000 0000 0000 0000 0000  .j..............
+00001b40: 0000 0000 006a 1300 0000 0000 0000 0000  .....j..........
+00001b50: 0000 0000 0000 0000 0064 057c 04ac 02ab  .........d.|....
+00001b60: 0200 0000 0000 007d 067c 026a 1500 0000  .......}.|.j....
+00001b70: 0000 0000 0000 0000 0000 0000 0000 007c  ...............|
+00001b80: 06ac 03ab 0100 0000 0000 007d 077c 006a  ...........}.|.j
+00001b90: 1700 0000 0000 0000 0000 0000 0000 0000  ................
+00001ba0: 0000 007c 077c 026a 1800 0000 0000 0000  ...|.|.j........
+00001bb0: 0000 0000 0000 0000 0000 00ac 04ab 0200  ................
+00001bc0: 0000 0000 0073 0290 018c 287c 067c 025f  .....s....(|.|._
+00001bd0: 0800 0000 0000 0000 0090 018c 3104 007c  ............1..|
+00001be0: 006a 0800 0000 0000 0000 0000 0000 0000  .j..............
+00001bf0: 0000 0000 006a 0b00 0000 0000 0000 0000  .....j..........
+00001c00: 0000 0000 0000 0000 00ab 0000 0000 0000  ................
+00001c10: 0044 005d 2100 005c 0200 007d 017d 027c  .D.]!..\...}.}.|
+00001c20: 026a 1b00 0000 0000 0000 0000 0000 0000  .j..............
+00001c30: 0000 0000 007c 006a 0400 0000 0000 0000  .....|.j........
+00001c40: 0000 0000 0000 0000 0000 00ac 01ab 0100  ................
+00001c50: 0000 0000 0001 008c 2304 0079 0029 064e  ........#..y.).N
+00001c60: 2901 da07 6465 6c74 615f 7429 02da 0872  )...delta_t)...r
+00001c70: 6f74 6174 696f 6e72 4700 0000 2901 723b  otationrG...).r;
+00001c80: 0000 0029 0272 2200 0000 7223 0000 0072  ...).r"...r#...r
+00001c90: 0200 0000 290e 7209 0000 0072 1000 0000  ....).r....r....
+00001ca0: 720a 0000 0072 2000 0000 720e 0000 0072  r....r ...r....r
+00001cb0: 1c00 0000 da08 6479 6e61 6d69 6373 da06  ......dynamics..
+00001cc0: 6368 616e 6765 723b 0000 00da 0675 7064  changer;.....upd
+00001cd0: 6174 6572 4f00 0000 7229 0000 00da 0963  aterO...r).....c
+00001ce0: 6f6c 6c69 7369 6f6e da04 7374 6570 2908  ollision..step).
+00001cf0: 7211 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
+00001d00: 5700 0000 7247 0000 0072 5600 0000 da09  W...rG...rV.....
+00001d10: 6e65 775f 7374 6174 6572 2200 0000 7308  new_stater"...s.
+00001d20: 0000 0020 2020 2020 2020 2072 1200 0000  ...        r....
+00001d30: 725b 0000 007a 0a4d 6f64 656c 2e73 7465  r[...z.Model.ste
+00001d40: 7070 0000 0073 c801 0000 8000 d80b 0f8f  pp...s..........
+00001d50: 3e8a 3ed8 1216 972e 912e a034 a73e a13e  >.>........4.>.>
+00001d60: d112 31b4 44b7 49b1 49b3 4bd2 123f d810  ..1.D.I.I.K..?..
+00001d70: 14f0 0300 1317 972e 912e a034 a73e a13e  ...........4.>.>
+00001d80: d112 31b4 44b7 49b1 49b3 4bd3 123f f406  ..1.D.I.I.K..?..
+00001d90: 001a 1e9f 1999 199b 1b88 048c 0ed8 1b1f  ................
+00001da0: 9f3b 993b d71b 2cd1 1b2c d31b 2ef3 0016  .;.;..,..,......
+00001db0: 0930 894b 8844 9025 d817 1c97 7e91 7e88  .0.K.D.%....~.~.
+00001dc0: 48d8 2129 a71f a11f b814 bf1e b91e a01f  H.!)............
+00001dd0: d321 48d1 0c1e 8848 9068 d818 1d9f 0b99  .!H....H.h......
+00001de0: 0bd7 182a d118 2ab0 48d8 343c f003 0019  ...*..*.H.4<....
+00001df0: 2bf3 0001 193e 8849 e01c 21d7 1c2d d11c  +....>.I..!..-..
+00001e00: 2db0 49d0 1c2d d31c 3e88 4dd8 0f13 d70f  -.I..-..>.M.....
+00001e10: 22d1 0f22 b01d d82e 33af 6fa9 6ff0 0300  ".."....3.o.o...
+00001e20: 1023 f400 0110 3fe0 1e27 9005 950b e01c  .#....?..'......
+00001e30: 219f 4b99 4bd7 1c2e d11c 2eb8 08d8 3839  !.K.K.........89
+00001e40: f003 001d 2ff3 0001 1d3b 9009 e020 25d7  ..../....;... %.
+00001e50: 2031 d120 31b8 09d0 2031 d320 4290 0dd8   1. 1... 1. B...
+00001e60: 1317 d713 26d1 1326 b05d d832 37b7 2fb1  ....&..&.].27./.
+00001e70: 2ff0 0300 1427 f400 0114 4301 e022 2b90  /....'....C.."+.
+00001e80: 4595 4be0 2025 a70b a10b d720 32d1 2032  E.K. %..... 2. 2
+00001e90: b841 d83c 44f0 0300 2133 f300 0121 4601  .A.<D...!3...!F.
+00001ea0: 9049 e024 29d7 2435 d124 35b8 49d0 2435  .I.$).$5.$5.I.$5
+00001eb0: d324 4690 4dd8 171b d717 2ad1 172a b81d  .$F.M.....*..*..
+00001ec0: d836 3bb7 6fb1 6ff0 0300 182b f600 0118  .6;.o.o....+....
+00001ed0: 4701 e026 2f98 059e 0bf0 2d16 0930 f02e  G..&/.....-..0..
+00001ee0: 001c 209f 3b99 3bd7 1b2c d11b 2cd3 1b2e  .. .;.;..,..,...
+00001ef0: f200 0109 2f89 4b88 4490 25d8 0c11 8f4a  ..../.K.D.%....J
+00001f00: 894a 9874 9f7e 997e 884a d50c 2ef1 0301  .J.t.~.~.J......
+00001f10: 092f 7214 0000 004e 2902 4667 9a99 9999  ./r....N).Fg....
+00001f20: 9999 b93f 2901 4629 15da 085f 5f6e 616d  ...?).F)...__nam
+00001f30: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00001f40: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0462  .__qualname__..b
+00001f50: 6f6f 6cda 0566 6c6f 6174 7213 0000 00da  ool..floatr.....
+00001f60: 0373 7472 7204 0000 0072 1a00 0000 721d  .strr....r....r.
+00001f70: 0000 0072 2f00 0000 da07 506f 6c79 676f  ...r/.....Polygo
+00001f80: 6e72 2900 0000 da06 7479 7069 6e67 da05  nr).....typing..
+00001f90: 5475 706c 65da 0369 6e74 7232 0000 0072  Tuple..intr2...r
+00001fa0: 1e00 0000 da04 6469 6374 7253 0000 0072  ......dictrS...r
+00001fb0: 5b00 0000 a900 7214 0000 0072 1200 0000  [.....r....r....
+00001fc0: 7208 0000 0072 0800 0000 0a00 0000 73aa  r....r........s.
+00001fd0: 0000 0084 00f0 0a00 2429 d824 27f1 090b  ........$).$'...
+00001fe0: 051e f006 001d 21f0 070b 051e f008 001d  ......!.........
+00001ff0: 22f3 090b 051e f01a 0305 1b98 63f0 0003  "...........c...
+00002000: 051b a825 f300 0305 1bf2 0a06 0525 f010  ...%.........%..
+00002010: 0705 14a8 42af 4aa9 4af0 0007 0514 c044  ....B.J.J......D
+00002020: f000 0705 14c8 54f3 0007 0514 f012 0105  ......T.........
+00002030: 6001 a026 a72c a12c a875 b065 a87c d122  `..&.,.,.u.e.|."
+00002040: 3cf0 0001 0560 01c8 33f3 0001 0560 01f2  <....`..3....`..
+00002050: 061c 051c f040 0100 2b30 f105 1e05 1bd8  .....@..+0......
+00002060: 2427 f003 1e05 1be0 2327 f005 1e05 1be0  $'......#'......
+00002070: 3438 f305 1e05 1bf3 4001 1e05 2f72 1400  48......@.../r..
+00002080: 0000 7208 0000 0029 0d72 2d00 0000 7220  ..r....).r-...r 
+00002090: 0000 0072 6400 0000 da07 7368 6170 656c  ...rd.....shapel
+000020a0: 7972 2f00 0000 7216 0000 0072 0400 0000  yr/...r....r....
+000020b0: 720f 0000 0072 0500 0000 da08 6765 6f6d  r....r......geom
+000020c0: 6574 7279 7206 0000 00da 066f 626a 6563  etryr......objec
+000020d0: 7472 0800 0000 7268 0000 0072 1400 0000  tr....rh...r....
+000020e0: 7212 0000 00fa 083c 6d6f 6475 6c65 3e72  r......<module>r
+000020f0: 6c00 0000 0100 0000 7328 0000 00f0 0301  l.......s(......
+00002100: 0101 db00 0bdb 000b db00 0ddb 0014 dd00  ................
+00002110: 18dd 0022 dd00 1bf4 0644 0201 2f88 46f5  ...".....D../.F.
+00002120: 0044 0201 2f72 1400 0000                 .D../r....
```

### Comparing `cellworld_game-0.0.61/cellworld_game/__pycache__/navigation.cpython-312.pyc` & `cellworld_game-0.0.68/cellworld_game/__pycache__/navigation.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Apr 21 15:19:56 2024 UTC, .py size: 1717 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 7% similar despite different names*

```diff
@@ -1,163 +1,167 @@
-00000000: cb0d 0d0a 0000 0000 9c2e 2566 b506 0000  ..........%f....
+00000000: cb0d 0d0a 0000 0000 6f91 1566 c006 0000  ........o..f....
 00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
-00000020: 0000 0000 00f3 2800 0000 9700 6400 6401  ......(.....d.d.
-00000030: 6c00 5a00 6400 6401 6c01 5a01 0200 4700  l.Z.d.d.l.Z...G.
-00000040: 6402 8400 6403 ab02 0000 0000 0000 5a02  d...d.........Z.
-00000050: 7901 2904 e900 0000 004e 6300 0000 0000  y.)......Nc.....
-00000060: 0000 0000 0000 0009 0000 0000 0000 00f3  ................
-00000070: aa01 0000 9700 6500 5a01 6400 5a02 6401  ......e.Z.d.Z.d.
-00000080: 6503 6a08 0000 0000 0000 0000 0000 0000  e.j.............
-00000090: 0000 0000 0000 6503 6a0a 0000 0000 0000  ......e.j.......
-000000a0: 0000 0000 0000 0000 0000 0000 6503 6a0c  ............e.j.
-000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000000c0: 0000 6507 6507 6602 1900 0000 1900 0000  ..e.e.f.........
-000000d0: 1900 0000 6402 6503 6a08 0000 0000 0000  ....d.e.j.......
-000000e0: 0000 0000 0000 0000 0000 0000 6503 6a08  ............e.j.
-000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000100: 0000 6508 1900 0000 1900 0000 6403 6503  ..e.........d.e.
-00000110: 6a08 0000 0000 0000 0000 0000 0000 0000  j...............
-00000120: 0000 0000 6503 6a08 0000 0000 0000 0000  ....e.j.........
-00000130: 0000 0000 0000 0000 0000 6503 6a08 0000  ..........e.j...
-00000140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000150: 6508 1900 0000 1900 0000 1900 0000 6606  e.............f.
-00000160: 6404 8404 5a09 6405 6503 6a0c 0000 0000  d...Z.d.e.j.....
-00000170: 0000 0000 0000 0000 0000 0000 0000 6507  ..............e.
-00000180: 6507 6602 1900 0000 6406 6508 6604 6407  e.f.....d.e.f.d.
-00000190: 8404 5a0a 6408 6503 6a0c 0000 0000 0000  ..Z.d.e.j.......
-000001a0: 0000 0000 0000 0000 0000 0000 6507 6507  ............e.e.
-000001b0: 6602 1900 0000 6409 6503 6a0c 0000 0000  f.....d.e.j.....
-000001c0: 0000 0000 0000 0000 0000 0000 0000 6507  ..............e.
-000001d0: 6507 6602 1900 0000 6406 6503 6a08 0000  e.f.....d.e.j...
-000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001f0: 6503 6a0c 0000 0000 0000 0000 0000 0000  e.j.............
-00000200: 0000 0000 0000 6507 6507 6602 1900 0000  ......e.e.f.....
-00000210: 1900 0000 6606 640a 8404 5a0b 790b 290c  ....f.d...Z.y.).
-00000220: da0a 4e61 7669 6761 7469 6f6e da09 6c6f  ..Navigation..lo
-00000230: 6361 7469 6f6e 73da 0570 6174 6873 da0a  cations..paths..
-00000240: 7669 7369 6269 6c69 7479 6304 0000 0000  visibilityc.....
-00000250: 0000 0000 0000 0002 0000 0003 0000 00f3  ................
-00000260: 2e00 0000 9700 7c01 7c00 5f00 0000 0000  ......|.|._.....
-00000270: 0000 0000 7c02 7c00 5f01 0000 0000 0000  ....|.|._.......
-00000280: 0000 7c03 7c00 5f02 0000 0000 0000 0000  ..|.|._.........
-00000290: 7900 2901 4e29 0372 0500 0000 7206 0000  y.).N).r....r...
-000002a0: 0072 0700 0000 2904 da04 7365 6c66 7205  .r....)...selfr.
-000002b0: 0000 0072 0600 0000 7207 0000 0073 0400  ...r....r....s..
-000002c0: 0000 2020 2020 fa37 433a 5c52 6573 6561  ..    .7C:\Resea
-000002d0: 7263 685c 6365 6c6c 776f 726c 645f 6761  rch\cellworld_ga
-000002e0: 6d65 5c63 656c 6c77 6f72 6c64 5f67 616d  me\cellworld_gam
-000002f0: 655c 6e61 7669 6761 7469 6f6e 2e70 79da  e\navigation.py.
-00000300: 085f 5f69 6e69 745f 5f7a 134e 6176 6967  .__init__z.Navig
-00000310: 6174 696f 6e2e 5f5f 696e 6974 5f5f 0600  ation.__init__..
-00000320: 0000 7319 0000 0080 00f0 0800 1a23 8804  ..s..........#..
-00000330: 8c0e d815 1a88 048c 0ad8 1a24 8804 8d0f  ...........$....
-00000340: f300 0000 00da 086c 6f63 6174 696f 6eda  .......location.
-00000350: 0672 6574 7572 6e63 0200 0000 0000 0000  .returnc........
-00000360: 0000 0000 0500 0000 0300 0000 f3b8 0000  ................
-00000370: 0097 0074 0000 0000 0000 0000 006a 0200  ...t.........j..
-00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000390: 007d 0264 007d 0374 0500 0000 0000 0000  .}.d.}.t........
-000003a0: 007c 006a 0600 0000 0000 0000 0000 0000  .|.j............
-000003b0: 0000 0000 0000 00ab 0100 0000 0000 0044  ...............D
-000003c0: 005d 2f00 005c 0200 007d 047d 057c 0580  .]/..\...}.}.|..
-000003d0: 018c 097c 0564 0119 0000 007c 0164 0119  ...|.d.....|.d..
-000003e0: 0000 007a 0a00 0064 027a 0800 007c 0564  ...z...d.z...|.d
-000003f0: 0319 0000 007c 0164 0319 0000 007a 0a00  .....|.d.....z..
-00000400: 0064 027a 0800 007a 0000 007d 067c 067c  .d.z...z...}.|.|
-00000410: 026b 0200 0073 018c 2c7c 047d 037c 067d  .k...s..,|.}.|.}
-00000420: 028c 3104 007c 0353 0029 044e 7202 0000  ..1..|.S.).Nr...
-00000430: 00e9 0200 0000 e901 0000 0029 04da 046d  ...........)...m
-00000440: 6174 68da 0369 6e66 da09 656e 756d 6572  ath..inf..enumer
-00000450: 6174 6572 0500 0000 2907 7209 0000 0072  ater....).r....r
-00000460: 0d00 0000 da09 6d69 6e5f 6469 7374 32da  ......min_dist2.
-00000470: 0763 6c6f 7365 7374 da01 69da 016c da05  .closest..i..l..
-00000480: 6469 7374 3273 0700 0000 2020 2020 2020  dist2s....      
-00000490: 2072 0a00 0000 da10 636c 6f73 6573 745f   r......closest_
-000004a0: 6c6f 6361 7469 6f6e 7a1b 4e61 7669 6761  locationz.Naviga
-000004b0: 7469 6f6e 2e63 6c6f 7365 7374 5f6c 6f63  tion.closest_loc
-000004c0: 6174 696f 6e0e 0000 0073 7b00 0000 8000  ation....s{.....
-000004d0: e414 1897 4891 4888 09d8 1216 8807 dc14  ....H.H.........
-000004e0: 1d98 649f 6e99 6ed3 142d f200 0609 2289  ..d.n.n..-....".
-000004f0: 4488 4188 71d8 0f10 8879 d810 18d8 1516  D.A.q....y......
-00000500: 9071 9154 9848 a051 994b d115 27a8 41d1  .q.T.H.Q.K..'.A.
-00000510: 142d b011 b031 b114 b808 c011 b90b d131  .-...1.........1
-00000520: 43c8 01d1 3049 d114 4988 45d8 0f14 9079  C...0I..I.E....y
-00000530: d30f 20d8 1a1b 9007 d81c 2191 09f0 0d06  .. .......!.....
-00000540: 0922 f00e 0010 1788 0e72 0c00 0000 da03  .".......r......
-00000550: 7372 63da 0364 7374 6303 0000 0000 0000  src..dstc.......
-00000560: 0000 0000 0005 0000 0003 0000 00f3 5a01  ..............Z.
-00000570: 0000 9700 7c00 6a01 0000 0000 0000 0000  ....|.j.........
-00000580: 0000 0000 0000 0000 0000 7c01 ac01 ab01  ..........|.....
-00000590: 0000 0000 0000 7d03 7c00 6a01 0000 0000  ......}.|.j.....
-000005a0: 0000 0000 0000 0000 0000 0000 0000 7c02  ..............|.
-000005b0: ac01 ab01 0000 0000 0000 7d04 7c03 7d05  ..........}.|.}.
-000005c0: 7c03 7d06 6700 7d07 7c05 814d 7c05 7c04  |.}.g.}.|..M|.|.
-000005d0: 6b37 0000 7248 7c00 6a02 0000 0000 0000  k7..rH|.j.......
-000005e0: 0000 0000 0000 0000 0000 0000 7c05 1900  ............|...
-000005f0: 0000 7c04 1900 0000 7d08 7c08 7c05 6b28  ..|.....}.|.|.k(
-00000600: 0000 7201 6e30 7c08 7c00 6a04 0000 0000  ..r.n0|.|.j.....
-00000610: 0000 0000 0000 0000 0000 0000 0000 7c06  ..............|.
-00000620: 1900 0000 7600 7d09 7c09 7313 7c07 6a07  ....v.}.|.s.|.j.
-00000630: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000640: 0000 7c05 ab01 0000 0000 0000 0100 7c05  ..|...........|.
-00000650: 7d06 7c08 7d05 7c05 8106 7c05 7c04 6b37  }.|.}.|...|.|.k7
-00000660: 0000 7201 8c48 7c07 6a07 0000 0000 0000  ..r..H|.j.......
-00000670: 0000 0000 0000 0000 0000 0000 7c04 ab01  ............|...
-00000680: 0000 0000 0000 0100 7c07 4400 8f0a 6302  ........|.D...c.
-00000690: 6700 6302 5d11 0000 7d0a 7c00 6a08 0000  g.c.]...}.|.j...
-000006a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000006b0: 7c0a 1900 0000 9102 8c13 0400 6302 7d0a  |...........c.}.
-000006c0: 5300 6302 0100 6302 7d0a 7700 2902 4e29  S.c...c.}.w.).N)
-000006d0: 0172 0d00 0000 2905 721a 0000 0072 0600  .r....).r....r..
-000006e0: 0000 7207 0000 00da 0661 7070 656e 6472  ..r......appendr
-000006f0: 0500 0000 290b 7209 0000 0072 1b00 0000  ....).r....r....
-00000700: 721c 0000 00da 0973 7263 5f69 6e64 6578  r......src_index
-00000710: da09 6473 745f 696e 6465 78da 0763 7572  ..dst_index..cur
-00000720: 7265 6e74 da09 6c61 7374 5f73 7465 70da  rent..last_step.
-00000730: 0c70 6174 685f 696e 6465 7865 73da 096e  .path_indexes..n
-00000740: 6578 745f 7374 6570 da0a 6973 5f76 6973  ext_step..is_vis
-00000750: 6962 6c65 da01 7373 0b00 0000 2020 2020  ible..ss....    
-00000760: 2020 2020 2020 2072 0a00 0000 da08 6765         r......ge
-00000770: 745f 7061 7468 7a13 4e61 7669 6761 7469  t_pathz.Navigati
-00000780: 6f6e 2e67 6574 5f70 6174 681b 0000 0073  on.get_path....s
-00000790: ce00 0000 8000 f006 0015 19d7 1429 d114  .............)..
-000007a0: 29b0 33d0 1429 d314 3788 09d8 1418 d714  ).3..)..7.......
-000007b0: 29d1 1429 b033 d014 29d3 1437 8809 d812  )..).3..)..7....
-000007c0: 1b88 07d8 141d 8809 d817 1988 0cd8 0e15  ................
-000007d0: d00e 21a0 67b0 19d2 263a d818 1c9f 0a99  ..!.g...&:......
-000007e0: 0aa0 37d1 182b a849 d118 3688 49d8 0f18  ..7..+.I..6.I...
-000007f0: 9847 d20f 23d8 1015 d819 22a0 64a7 6fa1  .G..#.....".d.o.
-00000800: 6fb0 69d1 2640 d019 4088 4ad9 131d d810  o.i.&@..@.J.....
-00000810: 1cd7 1023 d110 23a0 47d4 102c d81c 2390  ...#..#.G..,..#.
-00000820: 09d8 161f 8847 f011 000f 16d0 0e21 a067  .....G.......!.g
-00000830: b019 d326 3af0 1200 0915 d708 1bd1 081b  ...&:...........
-00000840: 9849 d408 26d8 2b37 d60f 38a0 6190 0497  .I..&.+7..8.a...
-00000850: 0e91 0e98 71d3 1021 d20f 38d0 0838 f9d2  ....q..!..8..8..
-00000860: 0f38 7306 0000 00c2 0f16 4228 044e 290c  .8s.......B(.N).
-00000870: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00000880: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00000890: 6d65 5f5f da06 7479 7069 6e67 da04 4c69  me__..typing..Li
-000008a0: 7374 da08 4f70 7469 6f6e 616c da05 5475  st..Optional..Tu
-000008b0: 706c 65da 0566 6c6f 6174 da03 696e 7472  ple..float..intr
-000008c0: 0b00 0000 721a 0000 0072 2700 0000 a900  ....r....r'.....
-000008d0: 720c 0000 0072 0a00 0000 7204 0000 0072  r....r....r....r
-000008e0: 0400 0000 0500 0000 73dd 0000 0084 00f0  ........s.......
-000008f0: 0206 0525 d81c 229f 4b99 4ba8 06af 0fa9  ...%..".K.K.....
-00000900: 0fb8 06bf 0cb9 0cc0 55c8 45c0 5cd1 3852  ........U.E.\.8R
-00000910: d128 53d1 1c54 f003 0605 25e0 181e 9f0b  .(S..T....%.....
-00000920: 990b a046 a74b a14b b003 d124 34d1 1835  ...F.K.K...$4..5
-00000930: f005 0605 25f0 0600 1e24 9f5b 995b a816  ....%....$.[.[..
-00000940: af1b a91b b056 b75b b15b c013 d135 45d1  .....V.[.[...5E.
-00000950: 2946 d11d 47f3 0706 0525 f010 0b05 17d8  )F..G....%......
-00000960: 2329 a73c a13c b005 b075 b00c d123 3df0  #).<.<...u...#=.
-00000970: 030b 0517 d842 45f3 030b 0517 f01a 1205  .....BE.........
-00000980: 39d8 161c 976c 916c a035 a825 a03c d116  9....l.l.5.%.<..
-00000990: 30f0 0312 0539 e016 1c97 6c91 6ca0 35a8  0....9....l.l.5.
-000009a0: 25a0 3cd1 1630 f005 1205 39e0 353b b75b  %.<..0....9.5;.[
-000009b0: b15b c016 c71c c11c c865 d055 5ac8 6cd1  .[.......e.UZ.l.
-000009c0: 415b d135 5cf4 0512 0539 720c 0000 0072  A[.5\....9r....r
-000009d0: 0400 0000 2903 7212 0000 0072 2b00 0000  ....).r....r+...
-000009e0: 7204 0000 0072 3100 0000 720c 0000 0072  r....r1...r....r
-000009f0: 0a00 0000 fa08 3c6d 6f64 756c 653e 7232  ......<module>r2
-00000a00: 0000 0001 0000 0073 1500 0000 f003 0101  .......s........
-00000a10: 01db 000b db00 0df7 0628 0139 f200 2801  .........(.9..(.
-00000a20: 3972 0c00 0000                           9r....
+00000020: 0000 0000 00f3 3c00 0000 9700 6400 6401  ......<.....d.d.
+00000030: 6c00 5a00 6400 6401 6c01 5a01 6402 6403  l.Z.d.d.l.Z.d.d.
+00000040: 6c02 6d03 5a03 0100 6400 6401 6c04 5a05  l.m.Z...d.d.l.Z.
+00000050: 0200 4700 6404 8400 6405 ab02 0000 0000  ..G.d...d.......
+00000060: 0000 5a06 7901 2906 e900 0000 004e e901  ..Z.y.)......N..
+00000070: 0000 0029 01da 0a56 6973 6962 696c 6974  ...)...Visibilit
+00000080: 7963 0000 0000 0000 0000 0000 0000 0900  yc..............
+00000090: 0000 0000 0000 f3aa 0100 0097 0065 005a  .............e.Z
+000000a0: 0164 005a 0264 0165 036a 0800 0000 0000  .d.Z.d.e.j......
+000000b0: 0000 0000 0000 0000 0000 0000 0065 036a  .............e.j
+000000c0: 0a00 0000 0000 0000 0000 0000 0000 0000  ................
+000000d0: 0000 0065 036a 0c00 0000 0000 0000 0000  ...e.j..........
+000000e0: 0000 0000 0000 0000 0065 0765 0766 0219  .........e.e.f..
+000000f0: 0000 0019 0000 0019 0000 0064 0265 036a  ...........d.e.j
+00000100: 0800 0000 0000 0000 0000 0000 0000 0000  ................
+00000110: 0000 0065 036a 0800 0000 0000 0000 0000  ...e.j..........
+00000120: 0000 0000 0000 0000 0065 0819 0000 0019  .........e......
+00000130: 0000 0064 0365 036a 0800 0000 0000 0000  ...d.e.j........
+00000140: 0000 0000 0000 0000 0000 0065 036a 0800  ...........e.j..
+00000150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000160: 0065 036a 0800 0000 0000 0000 0000 0000  .e.j............
+00000170: 0000 0000 0000 0065 0819 0000 0019 0000  .......e........
+00000180: 0019 0000 0066 0664 0484 045a 0964 0565  .....f.d...Z.d.e
+00000190: 036a 0c00 0000 0000 0000 0000 0000 0000  .j..............
+000001a0: 0000 0000 0065 0765 0766 0219 0000 0064  .....e.e.f.....d
+000001b0: 0665 0866 0464 0784 045a 0a64 0865 036a  .e.f.d...Z.d.e.j
+000001c0: 0c00 0000 0000 0000 0000 0000 0000 0000  ................
+000001d0: 0000 0065 0765 0766 0219 0000 0064 0965  ...e.e.f.....d.e
+000001e0: 036a 0c00 0000 0000 0000 0000 0000 0000  .j..............
+000001f0: 0000 0000 0065 0765 0766 0219 0000 0064  .....e.e.f.....d
+00000200: 0665 036a 0800 0000 0000 0000 0000 0000  .e.j............
+00000210: 0000 0000 0000 0065 036a 0c00 0000 0000  .......e.j......
+00000220: 0000 0000 0000 0000 0000 0000 0065 0765  .............e.e
+00000230: 0766 0219 0000 0019 0000 0066 0664 0a84  .f.........f.d..
+00000240: 045a 0b79 0b29 0cda 0a4e 6176 6967 6174  .Z.y.)...Navigat
+00000250: 696f 6eda 096c 6f63 6174 696f 6e73 da05  ion..locations..
+00000260: 7061 7468 73da 0a76 6973 6962 696c 6974  paths..visibilit
+00000270: 7963 0400 0000 0000 0000 0000 0000 0200  yc..............
+00000280: 0000 0300 0000 f32e 0000 0097 007c 017c  .............|.|
+00000290: 005f 0000 0000 0000 0000 007c 027c 005f  ._.........|.|._
+000002a0: 0100 0000 0000 0000 007c 037c 005f 0200  .........|.|._..
+000002b0: 0000 0000 0000 0079 0029 014e 2903 7207  .......y.).N).r.
+000002c0: 0000 0072 0800 0000 7209 0000 0029 04da  ...r....r....)..
+000002d0: 0473 656c 6672 0700 0000 7208 0000 0072  .selfr....r....r
+000002e0: 0900 0000 7304 0000 0020 2020 20fa 3743  ....s....    .7C
+000002f0: 3a5c 7265 7365 6172 6368 5c63 656c 6c77  :\research\cellw
+00000300: 6f72 6c64 5f67 616d 655c 6365 6c6c 776f  orld_game\cellwo
+00000310: 726c 645f 6761 6d65 5c6e 6176 6967 6174  rld_game\navigat
+00000320: 696f 6e2e 7079 da08 5f5f 696e 6974 5f5f  ion.py..__init__
+00000330: 7a13 4e61 7669 6761 7469 6f6e 2e5f 5f69  z.Navigation.__i
+00000340: 6e69 745f 5f08 0000 0073 1900 0000 8000  nit__....s......
+00000350: f008 001a 2388 048c 0ed8 151a 8804 8c0a  ....#...........
+00000360: d81a 2488 048d 0ff3 0000 0000 da08 6c6f  ..$...........lo
+00000370: 6361 7469 6f6e da06 7265 7475 726e 6302  cation..returnc.
+00000380: 0000 0000 0000 0000 0000 0005 0000 0003  ................
+00000390: 0000 00f3 b800 0000 9700 7400 0000 0000  ..........t.....
+000003a0: 0000 0000 6a02 0000 0000 0000 0000 0000  ....j...........
+000003b0: 0000 0000 0000 0000 7d02 6400 7d03 7405  ........}.d.}.t.
+000003c0: 0000 0000 0000 0000 7c00 6a06 0000 0000  ........|.j.....
+000003d0: 0000 0000 0000 0000 0000 0000 0000 ab01  ................
+000003e0: 0000 0000 0000 4400 5d2f 0000 5c02 0000  ......D.]/..\...
+000003f0: 7d04 7d05 7c05 8001 8c09 7c05 6401 1900  }.}.|.....|.d...
+00000400: 0000 7c01 6401 1900 0000 7a0a 0000 6402  ..|.d.....z...d.
+00000410: 7a08 0000 7c05 6403 1900 0000 7c01 6403  z...|.d.....|.d.
+00000420: 1900 0000 7a0a 0000 6402 7a08 0000 7a00  ....z...d.z...z.
+00000430: 0000 7d06 7c06 7c02 6b02 0000 7301 8c2c  ..}.|.|.k...s..,
+00000440: 7c04 7d03 7c06 7d02 8c31 0400 7c03 5300  |.}.|.}..1..|.S.
+00000450: 2904 4e72 0200 0000 e902 0000 0072 0300  ).Nr.........r..
+00000460: 0000 2904 da04 6d61 7468 da03 696e 66da  ..)...math..inf.
+00000470: 0965 6e75 6d65 7261 7465 7207 0000 0029  .enumerater....)
+00000480: 0772 0b00 0000 720f 0000 00da 096d 696e  .r....r......min
+00000490: 5f64 6973 7432 da07 636c 6f73 6573 74da  _dist2..closest.
+000004a0: 0169 da01 6cda 0564 6973 7432 7307 0000  .i..l..dist2s...
+000004b0: 0020 2020 2020 2020 720c 0000 00da 1063  .       r......c
+000004c0: 6c6f 7365 7374 5f6c 6f63 6174 696f 6e7a  losest_locationz
+000004d0: 1b4e 6176 6967 6174 696f 6e2e 636c 6f73  .Navigation.clos
+000004e0: 6573 745f 6c6f 6361 7469 6f6e 1000 0000  est_location....
+000004f0: 737b 0000 0080 00e4 1418 9748 9148 8809  s{.........H.H..
+00000500: d812 1688 07dc 141d 9864 9f6e 996e d314  .........d.n.n..
+00000510: 2df2 0006 0922 8944 8841 8871 d80f 1088  -....".D.A.q....
+00000520: 79d8 1018 d815 1690 7191 5498 48a0 5199  y.......q.T.H.Q.
+00000530: 4bd1 1527 a841 d114 2db0 11b0 31b1 14b8  K..'.A..-...1...
+00000540: 08c0 11b9 0bd1 3143 c801 d130 49d1 1449  ......1C...0I..I
+00000550: 8845 d80f 1490 79d3 0f20 d81a 1b90 07d8  .E....y.. ......
+00000560: 1c21 9109 f00d 0609 22f0 0e00 1017 880e  .!......".......
+00000570: 720e 0000 00da 0373 7263 da03 6473 7463  r......src..dstc
+00000580: 0300 0000 0000 0000 0000 0000 0500 0000  ................
+00000590: 0300 0000 f35a 0100 0097 007c 006a 0100  .....Z.....|.j..
+000005a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005b0: 007c 01ac 01ab 0100 0000 0000 007d 037c  .|...........}.|
+000005c0: 006a 0100 0000 0000 0000 0000 0000 0000  .j..............
+000005d0: 0000 0000 007c 02ac 01ab 0100 0000 0000  .....|..........
+000005e0: 007d 047c 037d 057c 037d 0667 007d 077c  .}.|.}.|.}.g.}.|
+000005f0: 0581 4d7c 057c 046b 3700 0072 487c 006a  ..M|.|.k7..rH|.j
+00000600: 0200 0000 0000 0000 0000 0000 0000 0000  ................
+00000610: 0000 007c 0519 0000 007c 0419 0000 007d  ...|.....|.....}
+00000620: 087c 087c 056b 2800 0072 016e 307c 087c  .|.|.k(..r.n0|.|
+00000630: 006a 0400 0000 0000 0000 0000 0000 0000  .j..............
+00000640: 0000 0000 007c 0619 0000 0076 007d 097c  .....|.....v.}.|
+00000650: 0973 137c 076a 0700 0000 0000 0000 0000  .s.|.j..........
+00000660: 0000 0000 0000 0000 007c 05ab 0100 0000  .........|......
+00000670: 0000 0001 007c 057d 067c 087d 057c 0581  .....|.}.|.}.|..
+00000680: 067c 057c 046b 3700 0072 018c 487c 076a  .|.|.k7..r..H|.j
+00000690: 0700 0000 0000 0000 0000 0000 0000 0000  ................
+000006a0: 0000 007c 04ab 0100 0000 0000 0001 007c  ...|...........|
+000006b0: 0744 008f 0a63 0267 0063 025d 1100 007d  .D...c.g.c.]...}
+000006c0: 0a7c 006a 0800 0000 0000 0000 0000 0000  .|.j............
+000006d0: 0000 0000 0000 007c 0a19 0000 0091 028c  .......|........
+000006e0: 1304 0063 027d 0a53 0063 0201 0063 027d  ...c.}.S.c...c.}
+000006f0: 0a77 0029 024e 2901 720f 0000 0029 0572  .w.).N).r....).r
+00000700: 1b00 0000 7208 0000 0072 0900 0000 da06  ....r....r......
+00000710: 6170 7065 6e64 7207 0000 0029 0b72 0b00  appendr....).r..
+00000720: 0000 721c 0000 0072 1d00 0000 da09 7372  ..r....r......sr
+00000730: 635f 696e 6465 78da 0964 7374 5f69 6e64  c_index..dst_ind
+00000740: 6578 da07 6375 7272 656e 74da 096c 6173  ex..current..las
+00000750: 745f 7374 6570 da0c 7061 7468 5f69 6e64  t_step..path_ind
+00000760: 6578 6573 da09 6e65 7874 5f73 7465 70da  exes..next_step.
+00000770: 0a69 735f 7669 7369 626c 65da 0173 730b  .is_visible..ss.
+00000780: 0000 0020 2020 2020 2020 2020 2020 720c  ...           r.
+00000790: 0000 00da 0867 6574 5f70 6174 687a 134e  .....get_pathz.N
+000007a0: 6176 6967 6174 696f 6e2e 6765 745f 7061  avigation.get_pa
+000007b0: 7468 1d00 0000 73ce 0000 0080 00f0 0600  th....s.........
+000007c0: 1519 d714 29d1 1429 b033 d014 29d3 1437  ....)..).3..)..7
+000007d0: 8809 d814 18d7 1429 d114 29b0 33d0 1429  .......)..).3..)
+000007e0: d314 3788 09d8 121b 8807 d814 1d88 09d8  ..7.............
+000007f0: 1719 880c d80e 15d0 0e21 a067 b019 d226  .........!.g...&
+00000800: 3ad8 181c 9f0a 990a a037 d118 2ba8 49d1  :........7..+.I.
+00000810: 1836 8849 d80f 1898 47d2 0f23 d810 15d8  .6.I....G..#....
+00000820: 1922 a064 a76f a16f b069 d126 40d0 1940  .".d.o.o.i.&@..@
+00000830: 884a d913 1dd8 101c d710 23d1 1023 a047  .J........#..#.G
+00000840: d410 2cd8 1c23 9009 d816 1f88 47f0 1100  ..,..#......G...
+00000850: 0f16 d00e 21a0 67b0 19d3 263a f012 0009  ....!.g...&:....
+00000860: 15d7 081b d108 1b98 49d4 0826 d82b 37d6  ........I..&.+7.
+00000870: 0f38 a061 9004 970e 910e 9871 d310 21d2  .8.a.......q..!.
+00000880: 0f38 d008 38f9 d20f 3873 0600 0000 c20f  .8..8...8s......
+00000890: 1642 2804 4e29 0cda 085f 5f6e 616d 655f  .B(.N)...__name_
+000008a0: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
+000008b0: 5f71 7561 6c6e 616d 655f 5fda 0674 7970  _qualname__..typ
+000008c0: 696e 67da 044c 6973 74da 084f 7074 696f  ing..List..Optio
+000008d0: 6e61 6cda 0554 7570 6c65 da05 666c 6f61  nal..Tuple..floa
+000008e0: 74da 0369 6e74 720d 0000 0072 1b00 0000  t..intr....r....
+000008f0: 7228 0000 00a9 0072 0e00 0000 720c 0000  r(.....r....r...
+00000900: 0072 0600 0000 7206 0000 0007 0000 0073  .r....r........s
+00000910: dd00 0000 8400 f002 0605 25d8 1c22 9f4b  ..........%..".K
+00000920: 994b a806 af0f a90f b806 bf0c b90c c055  .K.............U
+00000930: c845 c05c d138 52d1 2853 d11c 54f0 0306  .E.\.8R.(S..T...
+00000940: 0525 e018 1e9f 0b99 0ba0 46a7 4ba1 4bb0  .%........F.K.K.
+00000950: 03d1 2434 d118 35f0 0506 0525 f006 001e  ..$4..5....%....
+00000960: 249f 5b99 5ba8 16af 1ba9 1bb0 56b7 5bb1  $.[.[.......V.[.
+00000970: 5bc0 13d1 3545 d129 46d1 1d47 f307 0605  [...5E.)F..G....
+00000980: 25f0 100b 0517 d823 29a7 3ca1 3cb0 05b0  %......#).<.<...
+00000990: 75b0 0cd1 233d f003 0b05 17d8 4245 f303  u...#=......BE..
+000009a0: 0b05 17f0 1a12 0539 d816 1c97 6c91 6ca0  .......9....l.l.
+000009b0: 35a8 25a0 3cd1 1630 f003 1205 39e0 161c  5.%.<..0....9...
+000009c0: 976c 916c a035 a825 a03c d116 30f0 0512  .l.l.5.%.<..0...
+000009d0: 0539 e035 3bb7 5bb1 5bc0 16c7 1cc1 1cc8  .9.5;.[.[.......
+000009e0: 65d0 555a c86c d141 5bd1 355c f405 1205  e.UZ.l.A[.5\....
+000009f0: 3972 0e00 0000 7206 0000 0029 0772 1300  9r....r....).r..
+00000a00: 0000 722c 0000 0072 0900 0000 7204 0000  ..r,...r....r...
+00000a10: 00da 0773 6861 7065 6c79 da02 7370 7206  ...shapely..spr.
+00000a20: 0000 0072 3200 0000 720e 0000 0072 0c00  ...r2...r....r..
+00000a30: 0000 fa08 3c6d 6f64 756c 653e 7235 0000  ....<module>r5..
+00000a40: 0001 0000 0073 1b00 0000 f003 0101 01db  .....s..........
+00000a50: 000b db00 0ddd 0022 db00 14f7 0628 0139  .......".....(.9
+00000a60: f200 2801 3972 0e00 0000                 ..(.9r....
```

### Comparing `cellworld_game-0.0.61/cellworld_game/__pycache__/navigation_agent.cpython-312.pyc` & `cellworld_game-0.0.68/cellworld_game/__pycache__/mouse.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Fri Apr 26 17:03:41 2024 UTC, .py size: 4455 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 24% similar despite different names*

```diff
@@ -1,363 +1,367 @@
-00000000: cb0d 0d0a 0000 0000 6dde 2b66 6711 0000  ........m.+fg...
-00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
-00000020: 0000 0000 00f3 5600 0000 9700 6400 6401  ......V.....d.d.
-00000030: 6c00 5a00 6402 6403 6c01 6d02 5a02 6d03  l.Z.d.d.l.m.Z.m.
-00000040: 5a03 6d04 5a04 6d05 5a05 0100 6402 6404  Z.m.Z.m.Z...d.d.
-00000050: 6c06 6d07 5a07 6d08 5a08 0100 6402 6405  l.m.Z.m.Z...d.d.
-00000060: 6c09 6d0a 5a0a 0100 0200 4700 6406 8400  l.m.Z.....G.d...
-00000070: 6407 6507 ab03 0000 0000 0000 5a0b 7901  d.e.........Z.y.
-00000080: 2908 e900 0000 004e e901 0000 0029 04da  )......N.....)..
-00000090: 0864 6973 7461 6e63 65da 0964 6972 6563  .distance..direc
-000000a0: 7469 6f6e da14 6469 7265 6374 696f 6e5f  tion..direction_
-000000b0: 6469 6666 6572 656e 6365 da1d 6469 7265  difference..dire
-000000c0: 6374 696f 6e5f 6572 726f 725f 6e6f 726d  ction_error_norm
-000000d0: 616c 697a 6174 696f 6e29 02da 0541 6765  alization)...Age
-000000e0: 6e74 da13 436f 6f72 6469 6e61 7465 436f  nt..CoordinateCo
-000000f0: 6e76 6572 7465 7229 01da 0a4e 6176 6967  nverter)...Navig
-00000100: 6174 696f 6e63 0000 0000 0000 0000 0000  ationc..........
-00000110: 0000 0b00 0000 0000 0000 f37c 0000 0097  ...........|....
-00000120: 0065 005a 0164 005a 0209 0009 0064 1264  .e.Z.d.Z.....d.d
-00000130: 0165 0364 0265 0464 0365 0464 0465 0464  .e.d.e.d.e.d.e.d
-00000140: 0565 0566 0a64 0684 055a 0664 0784 005a  .e.f.d...Z.d...Z
-00000150: 0764 0884 005a 0864 0984 005a 0964 0a84  .d...Z.d...Z.d..
-00000160: 005a 0a64 0b65 0466 0264 0c84 045a 0b64  .Z.d.e.f.d...Z.d
-00000170: 0d65 0c6a 1a00 0000 0000 0000 0000 0000  .e.j............
-00000180: 0000 0000 0000 0064 0e65 0e66 0464 0f84  .......d.e.f.d..
-00000190: 045a 0f64 1084 005a 1079 1129 13da 0f4e  .Z.d...Z.y.)...N
-000001a0: 6176 6967 6174 696f 6e41 6765 6e74 da0a  avigationAgent..
-000001b0: 6e61 7669 6761 7469 6f6e da11 6d61 785f  navigation..max_
-000001c0: 666f 7277 6172 645f 7370 6565 64da 116d  forward_speed..m
-000001d0: 6178 5f74 7572 6e69 6e67 5f73 7065 6564  ax_turning_speed
-000001e0: da09 7468 7265 7368 6f6c 64da 1764 6573  ..threshold..des
-000001f0: 7469 6e61 7469 6f6e 5f75 7064 6174 655f  tination_update_
-00000200: 7261 7465 6306 0000 0000 0000 0000 0000  ratec...........
-00000210: 0003 0000 0003 0000 00f3 c800 0000 9700  ................
-00000220: 7c02 7c00 5f00 0000 0000 0000 0000 7c03  |.|._.........|.
-00000230: 7c00 5f01 0000 0000 0000 0000 7c04 7c00  |._.........|.|.
-00000240: 5f02 0000 0000 0000 0000 7c05 7c00 5f03  _.........|.|._.
-00000250: 0000 0000 0000 0000 7c01 7c00 5f04 0000  ........|.|._...
-00000260: 0000 0000 0000 6400 7c00 5f05 0000 0000  ......d.|._.....
-00000270: 0000 0000 6400 7c00 5f06 0000 0000 0000  ....d.|._.......
-00000280: 0000 6401 7c00 5f07 0000 0000 0000 0000  ..d.|._.........
-00000290: 6401 7c00 5f08 0000 0000 0000 0000 6700  d.|._.........g.
-000002a0: 7c00 5f09 0000 0000 0000 0000 7415 0000  |._.........t...
-000002b0: 0000 0000 0000 6a16 0000 0000 0000 0000  ......j.........
-000002c0: 0000 0000 0000 0000 0000 7c00 ab01 0000  ..........|.....
-000002d0: 0000 0000 0100 6402 7c00 5f0c 0000 0000  ......d.|._.....
-000002e0: 0000 0000 7900 2903 4e72 0200 0000 4629  ....y.).Nr....F)
-000002f0: 0d72 0e00 0000 720f 0000 0072 1000 0000  .r....r....r....
-00000300: 7211 0000 0072 0d00 0000 da0f 6e65 775f  r....r......new_
-00000310: 6465 7374 696e 6174 696f 6eda 0b64 6573  destination..des
-00000320: 7469 6e61 7469 6f6e da1b 6e61 7669 6761  tination..naviga
-00000330: 7469 6f6e 5f70 6c61 6e5f 7570 6461 7465  tion_plan_update
-00000340: 5f77 6169 74da 1064 6573 7469 6e61 7469  _wait..destinati
-00000350: 6f6e 5f77 6169 74da 0470 6174 6872 0800  on_wait..pathr..
-00000360: 0000 da08 5f5f 696e 6974 5f5f da09 636f  ....__init__..co
-00000370: 6c6c 6973 696f 6e29 06da 0473 656c 6672  llision)...selfr
-00000380: 0d00 0000 720e 0000 0072 0f00 0000 7210  ....r....r....r.
-00000390: 0000 0072 1100 0000 7306 0000 0020 2020  ...r....s....   
-000003a0: 2020 20fa 3d43 3a5c 5265 7365 6172 6368     .=C:\Research
-000003b0: 5c63 656c 6c77 6f72 6c64 5f67 616d 655c  \cellworld_game\
-000003c0: 6365 6c6c 776f 726c 645f 6761 6d65 5c6e  cellworld_game\n
-000003d0: 6176 6967 6174 696f 6e5f 6167 656e 742e  avigation_agent.
-000003e0: 7079 7218 0000 007a 184e 6176 6967 6174  pyr....z.Navigat
-000003f0: 696f 6e41 6765 6e74 2e5f 5f69 6e69 745f  ionAgent.__init_
-00000400: 5f09 0000 0073 6400 0000 8000 f00c 0022  _....sd........"
-00000410: 3388 04d4 081e d821 3288 04d4 081e d819  3......!2.......
-00000420: 2288 048c 0ed8 273e 8804 d408 24d8 1a24  ".....'>....$..$
-00000430: 8804 8c0f d81f 2388 04d4 081c d81b 1f88  ......#.........
-00000440: 04d4 0818 d82b 2c88 04d4 0828 d820 2188  .....+,....(. !.
-00000450: 04d4 081d d814 1688 048c 09dc 080d 8f0e  ................
-00000460: 890e 9074 d408 1cd8 191e 8804 8d0e f300  ...t............
-00000470: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00000480: 0200 0000 0300 0000 f33a 0000 0097 007c  .........:.....|
-00000490: 006a 0000 0000 0000 0000 0000 0000 0000  .j..............
-000004a0: 0000 0000 0072 0f7c 006a 0000 0000 0000  .....r.|.j......
-000004b0: 0000 0000 0000 0000 0000 0000 0064 0119  .............d..
-000004c0: 0000 0053 0079 00a9 024e 7202 0000 0029  ...S.y...Nr....)
-000004d0: 0172 1700 0000 a901 721a 0000 0073 0100  .r......r....s..
-000004e0: 0000 2072 1b00 0000 da09 6e65 7874 5f73  .. r......next_s
-000004f0: 7465 707a 194e 6176 6967 6174 696f 6e41  tepz.NavigationA
-00000500: 6765 6e74 2e6e 6578 745f 7374 6570 1c00  gent.next_step..
-00000510: 0000 731a 0000 0080 00d8 0b0f 8f39 8a39  ..s..........9.9
-00000520: d813 1797 3991 3998 5191 3cd0 0c1f d80f  ....9.9.Q.<.....
-00000530: 1372 1c00 0000 6302 0000 0000 0000 0000  .r....c.........
-00000540: 0000 0002 0000 0003 0000 00f3 1200 0000  ................
-00000550: 9700 7c01 7c00 5f00 0000 0000 0000 0000  ..|.|._.........
-00000560: 7900 a901 4e29 0172 1300 0000 2902 721a  y...N).r....).r.
-00000570: 0000 0072 1400 0000 7302 0000 0020 2072  ...r....s....  r
-00000580: 1b00 0000 da0f 7365 745f 6465 7374 696e  ......set_destin
-00000590: 6174 696f 6e7a 1f4e 6176 6967 6174 696f  ationz.Navigatio
-000005a0: 6e41 6765 6e74 2e73 6574 5f64 6573 7469  nAgent.set_desti
-000005b0: 6e61 7469 6f6e 2100 0000 730a 0000 0080  nation!...s.....
-000005c0: 00d8 1f2a 8804 d508 1c72 1c00 0000 6301  ...*.....r....c.
-000005d0: 0000 0000 0000 0000 0000 0003 0000 0003  ................
-000005e0: 0000 00f3 4a00 0000 9700 6400 7c00 5f00  ....J.....d.|._.
-000005f0: 0000 0000 0000 0000 6700 7c00 5f01 0000  ........g.|._...
-00000600: 0000 0000 0000 7405 0000 0000 0000 0000  ......t.........
-00000610: 6a06 0000 0000 0000 0000 0000 0000 0000  j...............
-00000620: 0000 0000 7c00 ab01 0000 0000 0000 0100  ....|...........
-00000630: 7900 7222 0000 0029 0472 1400 0000 7217  y.r"...).r....r.
-00000640: 0000 0072 0800 0000 da05 7265 7365 7472  ...r......resetr
-00000650: 1f00 0000 7301 0000 0020 721b 0000 0072  ....s.... r....r
-00000660: 2500 0000 7a15 4e61 7669 6761 7469 6f6e  %...z.Navigation
-00000670: 4167 656e 742e 7265 7365 7424 0000 0073  Agent.reset$...s
-00000680: 1d00 0000 8000 d81b 1f88 04d4 0818 d814  ................
-00000690: 1688 048c 09dc 080d 8f0b 890b 9044 d508  .............D..
-000006a0: 1972 1c00 0000 6301 0000 0000 0000 0000  .r....c.........
-000006b0: 0000 0003 0000 0003 0000 00f3 2e00 0000  ................
-000006c0: 9700 7401 0000 0000 0000 0000 6a02 0000  ..t.........j...
-000006d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000006e0: 7c00 ab01 0000 0000 0000 0100 7900 7222  |...........y.r"
-000006f0: 0000 0029 0272 0800 0000 da05 7374 6172  ...).r......star
-00000700: 7472 1f00 0000 7301 0000 0020 721b 0000  tr....s.... r...
-00000710: 0072 2700 0000 7a15 4e61 7669 6761 7469  .r'...z.Navigati
-00000720: 6f6e 4167 656e 742e 7374 6172 7429 0000  onAgent.start)..
-00000730: 0073 0e00 0000 8000 dc08 0d8f 0b89 0b90  .s..............
-00000740: 44d5 0819 721c 0000 00da 0764 656c 7461  D...r......delta
-00000750: 5f74 6302 0000 0000 0000 0000 0000 0005  _tc.............
-00000760: 0000 0003 0000 00f3 8c05 0000 9700 7c00  ..............|.
-00000770: 6a00 0000 0000 0000 0000 0000 0000 0000  j...............
-00000780: 0000 0000 7311 7c00 6a03 0000 0000 0000  ....s.|.j.......
-00000790: 0000 0000 0000 0000 0000 0000 ab00 0000  ................
-000007a0: 0000 0000 0100 7900 7c00 6a04 0000 0000  ......y.|.j.....
-000007b0: 0000 0000 0000 0000 0000 0000 0000 7289  ..............r.
-000007c0: 7c00 6a06 0000 0000 0000 0000 0000 0000  |.j.............
-000007d0: 0000 0000 0000 6401 6b28 0000 727a 7c00  ......d.k(..rz|.
-000007e0: 6a04 0000 0000 0000 0000 0000 0000 0000  j...............
-000007f0: 0000 0000 7c00 5f04 0000 0000 0000 0000  ....|._.........
-00000800: 6400 7c00 5f02 0000 0000 0000 0000 7c00  d.|._.........|.
-00000810: 6a0a 0000 0000 0000 0000 0000 0000 0000  j...............
-00000820: 0000 0000 7c00 5f03 0000 0000 0000 0000  ....|._.........
-00000830: 7c00 6a0a 0000 0000 0000 0000 0000 0000  |.j.............
-00000840: 0000 0000 0000 7c00 5f06 0000 0000 0000  ......|._.......
-00000850: 0000 7c00 6a0e 0000 0000 0000 0000 0000  ..|.j...........
-00000860: 0000 0000 0000 0000 6a11 0000 0000 0000  ........j.......
-00000870: 0000 0000 0000 0000 0000 0000 7c00 6a12  ............|.j.
-00000880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000890: 0000 6a14 0000 0000 0000 0000 0000 0000  ..j.............
-000008a0: 0000 0000 0000 7c00 6a08 0000 0000 0000  ......|.j.......
-000008b0: 0000 0000 0000 0000 0000 0000 ac02 ab02  ................
-000008c0: 0000 0000 0000 7c00 5f0b 0000 0000 0000  ......|._.......
-000008d0: 0000 7c00 6a08 0000 0000 0000 0000 0000  ..|.j...........
-000008e0: 0000 0000 0000 0000 724f 7c00 6a0c 0000  ........rO|.j...
-000008f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000900: 6401 6b28 0000 7240 7c00 6a0e 0000 0000  d.k(..r@|.j.....
-00000910: 0000 0000 0000 0000 0000 0000 0000 6a11  ..............j.
-00000920: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000930: 0000 7c00 6a12 0000 0000 0000 0000 0000  ..|.j...........
-00000940: 0000 0000 0000 0000 6a14 0000 0000 0000  ........j.......
-00000950: 0000 0000 0000 0000 0000 0000 7c00 6a08  ............|.j.
-00000960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000970: 0000 ac02 ab02 0000 0000 0000 7c00 5f0b  ............|._.
-00000980: 0000 0000 0000 0000 7c00 6a06 0000 0000  ........|.j.....
-00000990: 0000 0000 0000 0000 0000 0000 0000 7215  ..............r.
-000009a0: 7c00 7801 6a06 0000 0000 0000 0000 0000  |.x.j...........
-000009b0: 0000 0000 0000 0000 6403 7a17 0000 6302  ........d.z...c.
-000009c0: 5f03 0000 0000 0000 0000 7c00 6a0c 0000  _.........|.j...
-000009d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000009e0: 7215 7c00 7801 6a0c 0000 0000 0000 0000  r.|.x.j.........
-000009f0: 0000 0000 0000 0000 0000 6403 7a17 0000  ..........d.z...
-00000a00: 6302 5f06 0000 0000 0000 0000 7c00 6a19  c._.........|.j.
-00000a10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000a20: 0000 ab00 0000 0000 0000 8159 741b 0000  ...........Yt...
-00000a30: 0000 0000 0000 7c00 6a12 0000 0000 0000  ......|.j.......
-00000a40: 0000 0000 0000 0000 0000 0000 6a14 0000  ............j...
-00000a50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000a60: 7c00 6a19 0000 0000 0000 0000 0000 0000  |.j.............
-00000a70: 0000 0000 0000 ab00 0000 0000 0000 ac02  ................
-00000a80: ab02 0000 0000 0000 7d02 7c02 7c00 6a1c  ........}.|.|.j.
-00000a90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000aa0: 0000 6b02 0000 721b 7c00 6a16 0000 0000  ..k...r.|.j.....
-00000ab0: 0000 0000 0000 0000 0000 0000 0000 6a1f  ..............j.
-00000ac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000ad0: 0000 6401 ab01 0000 0000 0000 0100 7c00  ..d...........|.
-00000ae0: 6a19 0000 0000 0000 0000 0000 0000 0000  j...............
-00000af0: 0000 0000 ab00 0000 0000 0000 72da 741b  ............r.t.
-00000b00: 0000 0000 0000 0000 7c00 6a12 0000 0000  ........|.j.....
-00000b10: 0000 0000 0000 0000 0000 0000 0000 6a14  ..............j.
-00000b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b30: 0000 7c00 6a19 0000 0000 0000 0000 0000  ..|.j...........
-00000b40: 0000 0000 0000 0000 ab00 0000 0000 0000  ................
-00000b50: ac02 ab02 0000 0000 0000 7d02 7421 0000  ..........}.t!..
-00000b60: 0000 0000 0000 7c02 6404 7a0b 0000 6403  ......|.d.z...d.
-00000b70: ab02 0000 0000 0000 7d03 7423 0000 0000  ........}.t#....
-00000b80: 0000 0000 7c00 6a12 0000 0000 0000 0000  ....|.j.........
-00000b90: 0000 0000 0000 0000 0000 6a14 0000 0000  ..........j.....
-00000ba0: 0000 0000 0000 0000 0000 0000 0000 7c00  ..............|.
-00000bb0: 6a19 0000 0000 0000 0000 0000 0000 0000  j...............
-00000bc0: 0000 0000 ab00 0000 0000 0000 ac02 ab02  ................
-00000bd0: 0000 0000 0000 7d04 7425 0000 0000 0000  ......}.t%......
-00000be0: 0000 7c00 6a12 0000 0000 0000 0000 0000  ..|.j...........
-00000bf0: 0000 0000 0000 0000 6a22 0000 0000 0000  ........j"......
-00000c00: 0000 0000 0000 0000 0000 0000 7c04 ac05  ............|...
-00000c10: ab02 0000 0000 0000 7d05 7427 0000 0000  ........}.t'....
-00000c20: 0000 0000 7c05 ac06 ab01 0000 0000 0000  ....|...........
-00000c30: 7d06 7c00 6a28 0000 0000 0000 0000 0000  }.|.j(..........
-00000c40: 0000 0000 0000 0000 7c06 7a05 0000 7c03  ........|.z...|.
-00000c50: 7a05 0000 7c00 6a2a 0000 0000 0000 0000  z...|.j*........
-00000c60: 0000 0000 0000 0000 0000 5f16 0000 0000  .........._.....
-00000c70: 0000 0000 7c00 6a2e 0000 0000 0000 0000  ....|.j.........
-00000c80: 0000 0000 0000 0000 0000 7c05 7a05 0000  ..........|.z...
-00000c90: 7c00 6a2a 0000 0000 0000 0000 0000 0000  |.j*............
-00000ca0: 0000 0000 0000 5f18 0000 0000 0000 0000  ......_.........
-00000cb0: 7900 6401 7c00 6a2a 0000 0000 0000 0000  y.d.|.j*........
-00000cc0: 0000 0000 0000 0000 0000 5f16 0000 0000  .........._.....
-00000cd0: 0000 0000 6401 7c00 6a2a 0000 0000 0000  ....d.|.j*......
-00000ce0: 0000 0000 0000 0000 0000 0000 5f18 0000  ............_...
-00000cf0: 0000 0000 0000 7900 2907 4e72 0200 0000  ......y.).Nr....
-00000d00: 2902 da03 7372 63da 0364 7374 7203 0000  )...src..dstr...
-00000d10: 0067 9a99 9999 9999 c93f 2902 da0a 6469  .g.......?)...di
-00000d20: 7265 6374 696f 6e31 da0a 6469 7265 6374  rection1..direct
-00000d30: 696f 6e32 2901 da0f 6469 7265 6374 696f  ion2)...directio
-00000d40: 6e5f 6572 726f 7229 19da 0772 756e 6e69  n_error)...runni
-00000d50: 6e67 da0f 7374 6f70 5f6e 6176 6967 6174  ng..stop_navigat
-00000d60: 696f 6e72 1300 0000 7216 0000 0072 1400  ionr....r....r..
-00000d70: 0000 7211 0000 0072 1500 0000 720d 0000  ..r....r....r...
-00000d80: 00da 0867 6574 5f70 6174 68da 0573 7461  ...get_path..sta
-00000d90: 7465 da08 6c6f 6361 7469 6f6e 7217 0000  te..locationr...
-00000da0: 0072 2000 0000 7204 0000 0072 1000 0000  .r ...r....r....
-00000db0: da03 706f 70da 036d 6178 7205 0000 0072  ..pop..maxr....r
-00000dc0: 0600 0000 7207 0000 0072 0e00 0000 da08  ....r....r......
-00000dd0: 6479 6e61 6d69 6373 da0d 666f 7277 6172  dynamics..forwar
-00000de0: 645f 7370 6565 6472 0f00 0000 da0a 7475  d_speedr......tu
-00000df0: 726e 5f73 7065 6564 2907 721a 0000 0072  rn_speed).r....r
-00000e00: 2800 0000 da0e 6469 7374 616e 6365 5f65  (.....distance_e
-00000e10: 7272 6f72 da19 6e6f 726d 616c 697a 6564  rror..normalized
-00000e20: 5f64 6973 7461 6e63 655f 6572 726f 72da  _distance_error.
-00000e30: 1564 6573 7469 6e61 7469 6f6e 5f64 6972  .destination_dir
-00000e40: 6563 7469 6f6e 722e 0000 00da 1a6e 6f72  ectionr......nor
-00000e50: 6d61 6c69 7a65 645f 6469 7265 6374 696f  malized_directio
-00000e60: 6e5f 6572 726f 7273 0700 0000 2020 2020  n_errors....    
-00000e70: 2020 2072 1b00 0000 da04 7374 6570 7a14     r......stepz.
-00000e80: 4e61 7669 6761 7469 6f6e 4167 656e 742e  NavigationAgent.
-00000e90: 7374 6570 2c00 0000 731c 0200 0080 00d8  step,...s.......
-00000ea0: 0f13 8f7c 8a7c d80c 10d7 0c20 d10c 20d4  ...|.|..... .. .
-00000eb0: 0c22 d80c 12e0 0b0f d70b 1fd2 0b1f a044  .".............D
-00000ec0: d724 39d1 2439 b851 d224 3ed8 1f23 d71f  .$9.$9.Q.$>..#..
-00000ed0: 33d1 1f33 8844 d40c 1cd8 2327 8844 d40c  3..3.D....#'.D..
-00000ee0: 20d8 2428 d724 40d1 2440 8844 d40c 21d8   .$(.$@.$@.D..!.
-00000ef0: 2f33 d72f 4bd1 2f4b 8844 d40c 2cd8 181c  /3./K./K.D..,...
-00000f00: 9f0f 990f d718 30d1 1830 b054 b75a b15a  ......0..0.T.Z.Z
-00000f10: d735 48d1 3548 c864 d74e 5ed1 4e5e d018  .5H.5H.d.N^.N^..
-00000f20: 30d3 185f 8844 8c49 e00b 0fd7 0b1b d20b  0.._.D.I........
-00000f30: 1ba0 04d7 2040 d120 40c0 41d2 2045 d818  .... @. @.A. E..
-00000f40: 1c9f 0f99 0fd7 1830 d118 30b0 54b7 5ab1  .......0..0.T.Z.
-00000f50: 5ad7 3548 d135 48c8 64d7 4e5e d14e 5ed0  Z.5H.5H.d.N^.N^.
-00000f60: 1830 d318 5f88 448c 49e0 0b0f d70b 20d2  .0.._.D.I..... .
-00000f70: 0b20 d80c 10d7 0c21 d20c 21a0 51d1 0c26  . .....!..!.Q..&
-00000f80: d50c 21e0 0b0f d70b 2bd2 0b2b d80c 10d7  ..!.....+..+....
-00000f90: 0c2c d20c 2cb0 01d1 0c31 d50c 2ce0 0b0f  .,..,....1..,...
-00000fa0: 8f3e 893e d30b 1bd0 0b27 dc1d 25a8 24af  .>.>.....'..%.$.
-00000fb0: 2aa9 2ad7 2a3d d12a 3dd8 2a2e af2e a92e  *.*.*=.*=.*.....
-00000fc0: d32a 3af4 0301 1e3c 884e e00f 1da0 04a7  .*:....<.N......
-00000fd0: 0ea1 0ed2 0f2e d810 1497 0991 0997 0d91  ................
-00000fe0: 0d98 61d4 1020 e00b 0f8f 3e89 3ed4 0b1b  ..a.. ....>.>...
-00000ff0: dc1d 25a8 24af 2aa9 2ad7 2a3d d12a 3dd8  ..%.$.*.*.*=.*=.
-00001000: 2a2e af2e a92e d32a 3af4 0301 1e3c 884e  *......*:....<.N
-00001010: f406 0029 2ca8 4eb8 32d1 2c3d b871 d328  ...),.N.2.,=.q.(
-00001020: 41d0 0c25 e424 2db0 24b7 2ab1 2ad7 3245  A..%.$-.$.*.*.2E
-00001030: d132 45d8 3236 b72e b12e d332 42f4 0301  .2E.26.....2B...
-00001040: 2544 01d0 0c21 e41e 32b8 64bf 6ab9 6ad7  %D...!..2.d.j.j.
-00001050: 3e52 d13e 52d8 3e53 f403 011f 5501 884f  >R.>R.>S....U..O
-00001060: e429 46d0 5766 d429 67d0 0c26 e02a 2ed7  .)F.Wf.)g..&.*..
-00001070: 2a40 d12a 40d0 435d d12a 5dd0 6079 d12a  *@.*@.C].*].`y.*
-00001080: 7988 448f 4d89 4dd4 0c27 d827 2bd7 273d  y.D.M.M..'.'+.'=
-00001090: d127 3dc0 0fd1 274f 8844 8f4d 894d d50c  .'=...'O.D.M.M..
-000010a0: 24e0 2a2b 8844 8f4d 894d d40c 27d8 2728  $.*+.D.M.M..'.'(
-000010b0: 8844 8f4d 894d d50c 2472 1c00 0000 da07  .D.M.M..$r......
-000010c0: 7375 7266 6163 65da 1463 6f6f 7264 696e  surface..coordin
-000010d0: 6174 655f 636f 6e76 6572 7465 7263 0300  ate_converterc..
-000010e0: 0000 0000 0000 0000 0000 0900 0000 0300  ................
-000010f0: 0000 f374 0100 0097 007c 006a 0000 0000  ...t.....|.j....
-00001100: 0000 0000 0000 0000 0000 0000 0000 006a  ...............j
-00001110: 0200 0000 0000 0000 0000 0000 0000 0000  ................
-00001120: 0000 007d 037c 006a 0400 0000 0000 0000  ...}.|.j........
-00001130: 0000 0000 0000 0000 0000 0044 005d 7b00  ...........D.]{.
-00001140: 007d 047c 0480 018c 0674 0600 0000 0000  .}.|.....t......
-00001150: 0000 006a 0800 0000 0000 0000 0000 0000  ...j............
-00001160: 0000 0000 0000 006a 0b00 0000 0000 0000  .......j........
-00001170: 0000 0000 0000 0000 0000 007c 0164 017c  ...........|.d.|
-00001180: 026a 0d00 0000 0000 0000 0000 0000 0000  .j..............
-00001190: 0000 0000 007c 03ab 0100 0000 0000 007c  .....|.........|
-000011a0: 026a 0d00 0000 0000 0000 0000 0000 0000  .j..............
-000011b0: 0000 0000 007c 04ab 0100 0000 0000 0064  .....|.........d
-000011c0: 02ab 0500 0000 0000 0001 0074 0600 0000  ...........t....
-000011d0: 0000 0000 006a 0800 0000 0000 0000 0000  .....j..........
-000011e0: 0000 0000 0000 0000 006a 0f00 0000 0000  .........j......
-000011f0: 0000 0000 0000 0000 0000 0000 007c 0164  .............|.d
-00001200: 037c 026a 0d00 0000 0000 0000 0000 0000  .|.j............
-00001210: 0000 0000 0000 007c 04ab 0100 0000 0000  .......|........
-00001220: 0064 0464 02ac 05ab 0500 0000 0000 0001  .d.d............
-00001230: 007c 047d 038c 7d04 0074 1100 0000 0000  .|.}..}..t......
-00001240: 0000 006a 0800 0000 0000 0000 0000 0000  ...j............
-00001250: 0000 0000 0000 007c 007c 017c 02ac 06ab  .......|.|.|....
-00001260: 0300 0000 0000 0001 0079 0029 074e 2903  .........y.).N).
-00001270: e9ff 0000 0072 0200 0000 7202 0000 00e9  .....r....r.....
-00001280: 0200 0000 2903 7202 0000 0072 0200 0000  ....).r....r....
-00001290: 7241 0000 00e9 0500 0000 2905 723e 0000  rA........).r>..
-000012a0: 00da 0563 6f6c 6f72 da06 6365 6e74 6572  ...color..center
-000012b0: da06 7261 6469 7573 da05 7769 6474 6829  ..radius..width)
-000012c0: 0372 1a00 0000 723e 0000 0072 3f00 0000  .r....r>...r?...
-000012d0: 2909 7232 0000 0072 3300 0000 7217 0000  ).r2...r3...r...
-000012e0: 00da 0670 7967 616d 65da 0464 7261 77da  ...pygame..draw.
-000012f0: 046c 696e 65da 0e66 726f 6d5f 6361 6e6f  .line..from_cano
-00001300: 6e69 6361 6cda 0663 6972 636c 6572 0800  nical..circler..
-00001310: 0000 2905 721a 0000 0072 3e00 0000 723f  ..).r....r>...r?
-00001320: 0000 00da 0d63 7572 7265 6e74 5f70 6f69  .....current_poi
-00001330: 6e74 723d 0000 0073 0500 0000 2020 2020  ntr=...s....    
-00001340: 2072 1b00 0000 7249 0000 007a 144e 6176   r....rI...z.Nav
-00001350: 6967 6174 696f 6e41 6765 6e74 2e64 7261  igationAgent.dra
-00001360: 7759 0000 0073 b300 0000 8000 f006 0019  wY...s..........
-00001370: 1d9f 0a99 0ad7 182b d118 2b88 0dd8 1418  .......+..+.....
-00001380: 9749 9149 f200 0d09 2188 44d8 0f13 887c  .I.I....!.D....|
-00001390: d810 18dc 0c12 8f4b 894b d70c 1cd1 0c1c  .......K.K......
-000013a0: 9857 d81d 28d8 1d31 d71d 40d1 1d40 c01d  .W..(..1..@..@..
-000013b0: d31d 4fd8 1d31 d71d 40d1 1d40 c014 d31d  ..O..1..@..@....
-000013c0: 46d8 1d1e f409 040d 20f4 0a00 0d13 8f4b  F....... ......K
-000013d0: 894b d70c 1ed1 0c1e a077 d825 30d8 263a  .K.......w.%0.&:
-000013e0: d726 49d1 2649 c824 d326 4fd8 2627 d825  .&I.&I.$.&O.&'.%
-000013f0: 26f0 0900 0d1f f400 040d 28f0 0a00 1d21  &.........(....!
-00001400: 894d f01b 0d09 21f4 1c00 090e 8f0a 890a  .M....!.........
-00001410: 9804 d81b 22d8 283c f605 0209 3e72 1c00  ....".(<....>r..
-00001420: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
-00001430: 0000 0003 0000 00f3 4800 0000 9700 6401  ........H.....d.
-00001440: 7c00 6a00 0000 0000 0000 0000 0000 0000  |.j.............
-00001450: 0000 0000 0000 5f01 0000 0000 0000 0000  ......_.........
-00001460: 6401 7c00 6a00 0000 0000 0000 0000 0000  d.|.j...........
-00001470: 0000 0000 0000 0000 5f02 0000 0000 0000  ........_.......
-00001480: 0000 7900 721e 0000 0029 0372 3600 0000  ..y.r....).r6...
-00001490: 7237 0000 0072 3800 0000 721f 0000 0073  r7...r8...r....s
-000014a0: 0100 0000 2072 1b00 0000 7230 0000 007a  .... r....r0...z
-000014b0: 1f4e 6176 6967 6174 696f 6e41 6765 6e74  .NavigationAgent
-000014c0: 2e73 746f 705f 6e61 7669 6761 7469 6f6e  .stop_navigation
-000014d0: 6f00 0000 731a 0000 0080 00d8 2627 8804  o...s.......&'..
-000014e0: 8f0d 890d d408 23d8 2324 8804 8f0d 890d  ......#.#$......
-000014f0: d508 2072 1c00 0000 4e29 0267 7b14 ae47  .. r....N).g{..G
-00001500: e17a 843f e90a 0000 0029 11da 085f 5f6e  .z.?.....)...__n
-00001510: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00001520: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
-00001530: 0a00 0000 da05 666c 6f61 74da 0369 6e74  ......float..int
-00001540: 7218 0000 0072 2000 0000 7223 0000 0072  r....r ...r#...r
-00001550: 2500 0000 7227 0000 0072 3d00 0000 7248  %...r'...r=...rH
-00001560: 0000 00da 0753 7572 6661 6365 7209 0000  .....Surfacer...
-00001570: 0072 4900 0000 7230 0000 00a9 0072 1c00  .rI...r0.....r..
-00001580: 0000 721b 0000 0072 0c00 0000 720c 0000  ..r....r....r...
-00001590: 0007 0000 0073 7c00 0000 8400 f00c 0025  .....s|........%
-000015a0: 29d8 3032 f10b 1105 1fd8 1d27 f003 1105  ).02.......'....
-000015b0: 1fe0 2429 f005 1105 1ff0 0600 252a f007  ..$)........%*..
-000015c0: 1105 1ff0 0800 1d22 f009 1105 1ff0 0a00  ......."........
-000015d0: 2b2e f30b 1105 1ff2 2603 0514 f20a 0105  +.......&.......
-000015e0: 2bf2 0603 051a f20a 0105 1af0 062b 0529  +............+.)
-000015f0: 9845 f300 2b05 29f0 5a01 1405 3ed8 161c  .E..+.).Z...>...
-00001600: 976e 916e f003 1405 3ee0 2336 f305 1405  .n.n....>.#6....
-00001610: 3ef3 2c02 0525 721c 0000 0072 0c00 0000  >.,..%r....r....
-00001620: 290c 7248 0000 00da 0475 7469 6c72 0400  ).rH.....utilr..
-00001630: 0000 7205 0000 0072 0600 0000 7207 0000  ..r....r....r...
-00001640: 00da 0561 6765 6e74 7208 0000 0072 0900  ...agentr....r..
-00001650: 0000 720d 0000 0072 0a00 0000 720c 0000  ..r....r....r...
-00001660: 0072 5600 0000 721c 0000 0072 1b00 0000  .rV...r....r....
-00001670: fa08 3c6d 6f64 756c 653e 7259 0000 0001  ..<module>rY....
-00001680: 0000 0073 2200 0000 f003 0101 01db 000d  ...s"...........
-00001690: df00 5ad3 005a df00 2ddd 0022 f406 6a01  ..Z..Z..-.."..j.
-000016a0: 0125 9065 f500 6a01 0125 721c 0000 00    .%.e..j..%r....
+00000000: cb0d 0d0a 0000 0000 983a 1d66 2d0d 0000  .........:.f-...
+00000010: e300 0000 0000 0000 0000 0000 0006 0000  ................
+00000020: 0000 0000 00f3 b600 0000 9700 6400 6401  ............d.d.
+00000030: 6c00 5a00 6400 6401 6c01 5a01 6400 6401  l.Z.d.d.l.Z.d.d.
+00000040: 6c02 5a02 6402 6403 6c03 6d04 5a04 6d05  l.Z.d.d.l.m.Z.m.
+00000050: 5a05 0100 6402 6404 6c06 6d07 5a07 0100  Z...d.d.l.m.Z...
+00000060: 6402 6405 6c08 6d09 5a09 0100 6402 6406  d.d.l.m.Z...d.d.
+00000070: 6c0a 6d0b 5a0b 0100 6400 6401 6c0c 5a0d  l.m.Z...d.d.l.Z.
+00000080: 6400 6407 6c0e 6d0f 5a0f 0100 6402 6408  d.d.l.m.Z...d.d.
+00000090: 6c10 6d11 5a11 0100 0200 4700 6409 8400  l.m.Z.....G.d...
+000000a0: 640a 6501 6a24 0000 0000 0000 0000 0000  d.e.j$..........
+000000b0: 0000 0000 0000 0000 6513 1900 0000 ab03  ........e.......
+000000c0: 0000 0000 0000 5a14 0200 4700 640b 8400  ......Z...G.d...
+000000d0: 640c 6509 ab03 0000 0000 0000 5a15 7901  d.e.........Z.y.
+000000e0: 290d e900 0000 004e e901 0000 0029 02da  )......N.....)..
+000000f0: 0a41 6765 6e74 5374 6174 65da 0541 6765  .AgentState..Age
+00000100: 6e74 2901 da0a 4e61 7669 6761 7469 6f6e  nt)...Navigation
+00000110: 2901 da0f 4e61 7669 6761 7469 6f6e 4167  )...NavigationAg
+00000120: 656e 7429 01da 0952 6573 6f75 7263 6573  ent)...Resources
+00000130: 2901 da04 456e 756d 2901 da08 6469 7374  )...Enum)...dist
+00000140: 616e 6365 6300 0000 0000 0000 0000 0000  ancec...........
+00000150: 0005 0000 0000 0000 00f3 4000 0000 8700  ..........@.....
+00000160: 9700 6500 5a01 6400 5a02 0200 4700 6401  ..e.Z.d.Z...G.d.
+00000170: 8400 6402 6503 ab03 0000 0000 0000 5a04  ..d.e.........Z.
+00000180: 8800 6601 6403 8408 5a05 6404 6504 6602  ..f.d...Z.d.e.f.
+00000190: 6405 8404 5a06 8800 7801 5a07 5300 2906  d...Z...x.Z.S.).
+000001a0: da10 4d6f 7573 654f 6273 6572 7661 7469  ..MouseObservati
+000001b0: 6f6e 6300 0000 0000 0000 0000 0000 0001  onc.............
+000001c0: 0000 0000 0000 00f3 3800 0000 9700 6500  ........8.....e.
+000001d0: 5a01 6400 5a02 6401 5a03 6402 5a04 6403  Z.d.Z.d.Z.d.Z.d.
+000001e0: 5a05 6404 5a06 6405 5a07 6406 5a08 6407  Z.d.Z.d.Z.d.Z.d.
+000001f0: 5a09 6408 5a0a 6409 5a0b 640a 5a0c 640b  Z.d.Z.d.Z.d.Z.d.
+00000200: 5a0d 790c 290d fa16 4d6f 7573 654f 6273  Z.y.)...MouseObs
+00000210: 6572 7661 7469 6f6e 2e46 6965 6c64 7202  ervation.Fieldr.
+00000220: 0000 0072 0300 0000 e902 0000 00e9 0300  ...r............
+00000230: 0000 e904 0000 00e9 0500 0000 e906 0000  ................
+00000240: 00e9 0700 0000 e908 0000 00e9 0900 0000  ................
+00000250: e90a 0000 004e 290e da08 5f5f 6e61 6d65  .....N)...__name
+00000260: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
+00000270: 5f5f 7175 616c 6e61 6d65 5f5f da06 7072  __qualname__..pr
+00000280: 6579 5f78 da06 7072 6579 5f79 da0e 7072  ey_x..prey_y..pr
+00000290: 6579 5f64 6972 6563 7469 6f6e da0a 7072  ey_direction..pr
+000002a0: 6564 6174 6f72 5f78 da0a 7072 6564 6174  edator_x..predat
+000002b0: 6f72 5f79 da12 7072 6564 6174 6f72 5f64  or_y..predator_d
+000002c0: 6972 6563 7469 6f6e da0d 676f 616c 5f64  irection..goal_d
+000002d0: 6973 7461 6e63 65da 1170 7265 6461 746f  istance..predato
+000002e0: 725f 6469 7374 616e 6365 da06 7075 6666  r_distance..puff
+000002f0: 6564 da10 7075 6666 5f63 6f6f 6c65 645f  ed..puff_cooled_
+00000300: 646f 776e da08 6669 6e69 7368 6564 a900  down..finished..
+00000310: f300 0000 00fa 3243 3a5c 7265 7365 6172  ......2C:\resear
+00000320: 6368 5c63 656c 6c77 6f72 6c64 5f67 616d  ch\cellworld_gam
+00000330: 655c 6365 6c6c 776f 726c 645f 6761 6d65  e\cellworld_game
+00000340: 5c6d 6f75 7365 2e70 79da 0546 6965 6c64  \mouse.py..Field
+00000350: 720e 0000 000f 0000 0073 3c00 0000 8400  r........s<.....
+00000360: d811 1288 06d8 1112 8806 d819 1a88 0ed8  ................
+00000370: 1516 880a d815 1688 0ad8 1d1e d008 1ad8  ................
+00000380: 1819 880d d81c 1dd0 0819 d811 1288 06d8  ................
+00000390: 1b1c d008 18d8 1315 8908 7227 0000 0072  ..........r'...r
+000003a0: 2900 0000 6301 0000 0000 0000 0000 0000  )...c...........
+000003b0: 0004 0000 0003 0000 00f3 6e00 0000 9501  ..........n.....
+000003c0: 9700 7400 0000 0000 0000 0000 8902 7c00  ..t...........|.
+000003d0: 8d05 0000 ab00 0000 0000 0000 0100 7404  ..............t.
+000003e0: 0000 0000 0000 0000 6a06 0000 0000 0000  ........j.......
+000003f0: 0000 0000 0000 0000 0000 0000 4400 5d13  ............D.].
+00000400: 0000 7d01 7c00 6a09 0000 0000 0000 0000  ..}.|.j.........
+00000410: 0000 0000 0000 0000 0000 6401 ab01 0000  ..........d.....
+00000420: 0000 0000 0100 8c15 0400 7900 2902 4e67  ..........y.).Ng
+00000430: 0000 0000 0000 0000 2905 da05 7375 7065  ........)...supe
+00000440: 72da 085f 5f69 6e69 745f 5f72 0c00 0000  r..__init__r....
+00000450: 7229 0000 00da 0661 7070 656e 6429 03da  r).....append)..
+00000460: 0473 656c 66da 0169 da09 5f5f 636c 6173  .self..i..__clas
+00000470: 735f 5f73 0300 0000 2020 8072 2800 0000  s__s....  .r(...
+00000480: 722c 0000 007a 194d 6f75 7365 4f62 7365  r,...z.MouseObse
+00000490: 7276 6174 696f 6e2e 5f5f 696e 6974 5f5f  rvation.__init__
+000004a0: 1c00 0000 732f 0000 00f8 8000 dc08 0d89  ....s/..........
+000004b0: 07d1 0818 d408 1adc 1121 d711 27d1 1127  .........!..'..'
+000004c0: f200 0109 1d88 41d8 0c10 8f4b 894b 9803  ......A....K.K..
+000004d0: d50c 1cf1 0301 091d 7227 0000 00da 0566  ........r'.....f
+000004e0: 6965 6c64 6303 0000 0000 0000 0000 0000  ieldc...........
+000004f0: 0005 0000 0003 0000 00f3 4600 0000 9700  ..........F.....
+00000500: 7400 0000 0000 0000 0000 6a03 0000 0000  t.........j.....
+00000510: 0000 0000 0000 0000 0000 0000 0000 7c00  ..............|.
+00000520: 7c01 6a04 0000 0000 0000 0000 0000 0000  |.j.............
+00000530: 0000 0000 0000 7c02 ab03 0000 0000 0000  ......|.........
+00000540: 0100 7900 a901 4e29 03da 046c 6973 74da  ..y...N)...list.
+00000550: 0b5f 5f73 6574 6974 656d 5f5f da05 7661  .__setitem__..va
+00000560: 6c75 6529 0372 2e00 0000 7231 0000 0072  lue).r....r1...r
+00000570: 3600 0000 7303 0000 0020 2020 7228 0000  6...s....   r(..
+00000580: 0072 3500 0000 7a1c 4d6f 7573 654f 6273  .r5...z.MouseObs
+00000590: 6572 7661 7469 6f6e 2e5f 5f73 6574 6974  ervation.__setit
+000005a0: 656d 5f5f 2100 0000 7318 0000 0080 00dc  em__!...s.......
+000005b0: 080c d708 18d1 0818 9814 9875 9f7b 997b  ...........u.{.{
+000005c0: a845 d508 3272 2700 0000 2908 7218 0000  .E..2r'...).r...
+000005d0: 0072 1900 0000 721a 0000 0072 0900 0000  .r....r....r....
+000005e0: 7229 0000 0072 2c00 0000 7235 0000 00da  r)...r,...r5....
+000005f0: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 2901  .__classcell__).
+00000600: 7230 0000 0073 0100 0000 4072 2800 0000  r0...s....@r(...
+00000610: 720c 0000 0072 0c00 0000 0e00 0000 7320  r....r........s 
+00000620: 0000 00f8 8400 f402 0b05 1690 04f4 000b  ................
+00000630: 0516 f41a 0305 1df0 0a01 0533 a015 f700  ...........3....
+00000640: 0105 3372 2700 0000 720c 0000 0063 0000  ..3r'...r....c..
+00000650: 0000 0000 0000 0000 0000 1000 0000 0000  ................
+00000660: 0000 f302 0100 0097 0065 005a 0164 005a  .........e.Z.d.Z
+00000670: 0264 0165 0364 0265 046a 0a00 0000 0000  .d.e.d.e.j......
+00000680: 0000 0000 0000 0000 0000 0000 0065 046a  .............e.j
+00000690: 0c00 0000 0000 0000 0000 0000 0000 0000  ................
+000006a0: 0000 0065 0765 0766 0219 0000 0019 0000  ...e.e.f........
+000006b0: 0064 0365 046a 0c00 0000 0000 0000 0000  .d.e.j..........
+000006c0: 0000 0000 0000 0000 0065 0765 0766 0219  .........e.e.f..
+000006d0: 0000 0064 0465 0764 0565 0764 0665 0764  ...d.e.d.e.d.e.d
+000006e0: 0765 0864 0865 0966 1064 0984 045a 0a64  .e.d.e.f.d...Z.d
+000006f0: 0a84 005a 0b64 0b84 005a 0c64 0c65 0766  ...Z.d...Z.d.e.f
+00000700: 0264 0d84 045a 0d65 0e64 0e65 0f6a 2000  .d...Z.e.d.e.j .
+00000710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000720: 0066 0264 0f84 04ab 0000 0000 0000 005a  .f.d...........Z
+00000730: 1165 0e64 0e65 126a 2600 0000 0000 0000  .e.d.e.j&.......
+00000740: 0000 0000 0000 0000 0000 0066 0264 1084  ...........f.d..
+00000750: 04ab 0000 0000 0000 005a 1464 1165 1566  .........Z.d.e.f
+00000760: 0264 1284 045a 1679 1329 14da 054d 6f75  .d...Z.y.)...Mou
+00000770: 7365 da0b 7374 6172 745f 7374 6174 65da  se..start_state.
+00000780: 0761 6374 696f 6e73 da0d 676f 616c 5f6c  .actions..goal_l
+00000790: 6f63 6174 696f 6eda 0e67 6f61 6c5f 7468  ocation..goal_th
+000007a0: 7265 7368 6f6c 64da 0e70 7566 665f 7468  reshold..puff_th
+000007b0: 7265 7368 6f6c 64da 1370 7566 665f 636f  reshold..puff_co
+000007c0: 6f6c 5f64 6f77 6e5f 7469 6d65 da0a 6e61  ol_down_time..na
+000007d0: 7669 6761 7469 6f6e da08 7072 6564 6174  vigation..predat
+000007e0: 6f72 6309 0000 0000 0000 0000 0000 0006  orc.............
+000007f0: 0000 0003 0000 00f3 c200 0000 9700 7401  ..............t.
+00000800: 0000 0000 0000 0000 6a02 0000 0000 0000  ........j.......
+00000810: 0000 0000 0000 0000 0000 0000 7c00 7c07  ............|.|.
+00000820: 6401 6402 ac03 ab04 0000 0000 0000 0100  d.d.............
+00000830: 7c01 7c00 5f02 0000 0000 0000 0000 7c02  |.|._.........|.
+00000840: 7c00 5f03 0000 0000 0000 0000 7c03 7c00  |._.........|.|.
+00000850: 5f04 0000 0000 0000 0000 7c04 7c00 5f05  _.........|.|._.
+00000860: 0000 0000 0000 0000 7c05 7c00 5f06 0000  ........|.|._...
+00000870: 0000 0000 0000 6404 7c00 5f07 0000 0000  ......d.|._.....
+00000880: 0000 0000 7c06 7c00 5f08 0000 0000 0000  ....|.|._.......
+00000890: 0000 7c08 7c00 5f09 0000 0000 0000 0000  ..|.|._.........
+000008a0: 6405 7c00 5f0a 0000 0000 0000 0000 6405  d.|._.........d.
+000008b0: 7c00 5f0b 0000 0000 0000 0000 7900 2906  |._.........y.).
+000008c0: 4e67 0000 0000 0000 e03f 6700 0000 0000  Ng.......?g.....
+000008d0: 0034 4029 0372 4000 0000 da11 6d61 785f  .4@).r@.....max_
+000008e0: 666f 7277 6172 645f 7370 6565 64da 116d  forward_speed..m
+000008f0: 6178 5f74 7572 6e69 6e67 5f73 7065 6564  ax_turning_speed
+00000900: 7202 0000 0046 290c 7207 0000 0072 2c00  r....F).r....r,.
+00000910: 0000 723a 0000 0072 3b00 0000 723c 0000  ..r:...r;...r<..
+00000920: 0072 3d00 0000 723e 0000 00da 0e70 7566  .r=...r>.....puf
+00000930: 665f 636f 6f6c 5f64 6f77 6e72 3f00 0000  f_cool_downr?...
+00000940: 7241 0000 0072 2500 0000 7223 0000 0029  rA...r%...r#...)
+00000950: 0972 2e00 0000 723a 0000 0072 3b00 0000  .r....r:...r;...
+00000960: 723c 0000 0072 3d00 0000 723e 0000 0072  r<...r=...r>...r
+00000970: 3f00 0000 7240 0000 0072 4100 0000 7309  ?...r@...rA...s.
+00000980: 0000 0020 2020 2020 2020 2020 7228 0000  ...         r(..
+00000990: 0072 2c00 0000 7a0e 4d6f 7573 652e 5f5f  .r,...z.Mouse.__
+000009a0: 696e 6974 5f5f 2600 0000 736b 0000 0080  init__&...sk....
+000009b0: 00f4 1200 0918 d708 20d1 0820 a014 d82c  ........ .. ...,
+000009c0: 36d8 3336 d833 37f5 0703 0939 f008 001c  6.36.37....9....
+000009d0: 2788 04d4 0818 d817 1e88 048c 0cd8 1d2a  '..............*
+000009e0: 8804 d408 1ad8 1e2c 8804 d408 1bd8 1e2c  .......,.......,
+000009f0: 8804 d408 1bd8 1e1f 8804 d408 1bd8 2336  ..............#6
+00000a00: 8804 d408 20d8 1820 8804 8c0d d818 1d88  .... .. ........
+00000a10: 048c 0dd8 161b 8804 8d0b 7227 0000 0063  ..........r'...c
+00000a20: 0100 0000 0000 0000 0000 0000 0300 0000  ................
+00000a30: 0300 0000 f3de 0000 0097 0064 017c 005f  ...........d.|._
+00000a40: 0000 0000 0000 0000 0064 027c 005f 0100  .........d.|._..
+00000a50: 0000 0000 0000 007c 006a 0400 0000 0000  .......|.j......
+00000a60: 0000 0000 0000 0000 0000 0000 006a 0600  .............j..
+00000a70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000a80: 007c 006a 0800 0000 0000 0000 0000 0000  .|.j............
+00000a90: 0000 0000 0000 005f 0300 0000 0000 0000  ......._........
+00000aa0: 007c 006a 0400 0000 0000 0000 0000 0000  .|.j............
+00000ab0: 0000 0000 0000 006a 0a00 0000 0000 0000  .......j........
+00000ac0: 0000 0000 0000 0000 0000 007c 006a 0800  ...........|.j..
+00000ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000ae0: 005f 0500 0000 0000 0000 0074 0d00 0000  ._.........t....
+00000af0: 0000 0000 006a 0e00 0000 0000 0000 0000  .....j..........
+00000b00: 0000 0000 0000 0000 007c 00ab 0100 0000  .........|......
+00000b10: 0000 0001 0079 0029 034e 4672 0200 0000  .....y.).NFr....
+00000b20: 2908 7225 0000 0072 4500 0000 723a 0000  ).r%...rE...r:..
+00000b30: 00da 086c 6f63 6174 696f 6eda 0573 7461  ...location..sta
+00000b40: 7465 da09 6469 7265 6374 696f 6e72 0700  te..directionr..
+00000b50: 0000 da05 7265 7365 74a9 0172 2e00 0000  ....reset..r....
+00000b60: 7301 0000 0020 7228 0000 0072 4a00 0000  s.... r(...rJ...
+00000b70: 7a0b 4d6f 7573 652e 7265 7365 743e 0000  z.Mouse.reset>..
+00000b80: 0073 4f00 0000 8000 d818 1d88 048c 0dd8  .sO.............
+00000b90: 1e1f 8804 d408 1bd8 1e22 d71e 2ed1 1e2e  ........."......
+00000ba0: d71e 37d1 1e37 8804 8f0a 890a d408 1bd8  ..7..7..........
+00000bb0: 1f23 d71f 2fd1 1f2f d71f 39d1 1f39 8804  .#../../..9..9..
+00000bc0: 8f0a 890a d408 1cdc 0817 d708 1dd1 081d  ................
+00000bd0: 9864 d508 2372 2700 0000 6301 0000 0000  .d..#r'...c.....
+00000be0: 0000 0000 0000 0003 0000 0003 0000 00f3  ................
+00000bf0: 2e00 0000 9700 7401 0000 0000 0000 0000  ......t.........
+00000c00: 6a02 0000 0000 0000 0000 0000 0000 0000  j...............
+00000c10: 0000 0000 7c00 ab01 0000 0000 0000 0100  ....|...........
+00000c20: 7900 7233 0000 0029 0272 0700 0000 da05  y.r3...).r......
+00000c30: 7374 6172 7472 4b00 0000 7301 0000 0020  startrK...s.... 
+00000c40: 7228 0000 0072 4d00 0000 7a0b 4d6f 7573  r(...rM...z.Mous
+00000c50: 652e 7374 6172 7445 0000 0073 1000 0000  e.startE...s....
+00000c60: 8000 dc08 17d7 081d d108 1d98 64d5 0823  ............d..#
+00000c70: 7227 0000 00da 0764 656c 7461 5f74 6302  r'.....delta_tc.
+00000c80: 0000 0000 0000 0000 0000 0004 0000 0003  ................
+00000c90: 0000 00f3 9402 0000 9700 7c00 6a00 0000  ..........|.j...
+00000ca0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000cb0: 6401 6b1a 0000 72bd 7403 0000 0000 0000  d.k...r.t.......
+00000cc0: 0000 7c00 6a04 0000 0000 0000 0000 0000  ..|.j...........
+00000cd0: 0000 0000 0000 0000 6a06 0000 0000 0000  ........j.......
+00000ce0: 0000 0000 0000 0000 0000 0000 7c00 6a08  ............|.j.
+00000cf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000d00: 0000 6a04 0000 0000 0000 0000 0000 0000  ..j.............
+00000d10: 0000 0000 0000 6a06 0000 0000 0000 0000  ......j.........
+00000d20: 0000 0000 0000 0000 0000 ab02 0000 0000  ................
+00000d30: 0000 7d02 7c02 7c00 6a0a 0000 0000 0000  ..}.|.|.j.......
+00000d40: 0000 0000 0000 0000 0000 0000 6b1a 0000  ............k...
+00000d50: 7270 7c00 6a0c 0000 0000 0000 0000 0000  rp|.j...........
+00000d60: 0000 0000 0000 0000 6a0e 0000 0000 0000  ........j.......
+00000d70: 0000 0000 0000 0000 0000 0000 6a11 0000  ............j...
+00000d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000d90: 7c00 6a04 0000 0000 0000 0000 0000 0000  |.j.............
+00000da0: 0000 0000 0000 6a06 0000 0000 0000 0000  ......j.........
+00000db0: 0000 0000 0000 0000 0000 7c00 6a08 0000  ..........|.j...
+00000dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000dd0: 6a04 0000 0000 0000 0000 0000 0000 0000  j...............
+00000de0: 0000 0000 6a06 0000 0000 0000 0000 0000  ....j...........
+00000df0: 0000 0000 0000 0000 ab02 0000 0000 0000  ................
+00000e00: 7218 6402 7c00 5f09 0000 0000 0000 0000  r.d.|._.........
+00000e10: 7c00 6a14 0000 0000 0000 0000 0000 0000  |.j.............
+00000e20: 0000 0000 0000 7c00 5f00 0000 0000 0000  ......|._.......
+00000e30: 0000 7c01 7c00 6a00 0000 0000 0000 0000  ..|.|.j.........
+00000e40: 0000 0000 0000 0000 0000 6b02 0000 7216  ..........k...r.
+00000e50: 7c00 7801 6a00 0000 0000 0000 0000 0000  |.x.j...........
+00000e60: 0000 0000 0000 0000 7c01 7a17 0000 6302  ........|.z...c.
+00000e70: 5f00 0000 0000 0000 0000 6e07 6401 7c00  _.........n.d.|.
+00000e80: 5f00 0000 0000 0000 0000 7403 0000 0000  _.........t.....
+00000e90: 0000 0000 7c00 6a16 0000 0000 0000 0000  ....|.j.........
+00000ea0: 0000 0000 0000 0000 0000 7c00 6a04 0000  ..........|.j...
+00000eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000ec0: 6a06 0000 0000 0000 0000 0000 0000 0000  j...............
+00000ed0: 0000 0000 ab02 0000 0000 0000 7d03 7c03  ............}.|.
+00000ee0: 7c00 6a18 0000 0000 0000 0000 0000 0000  |.j.............
+00000ef0: 0000 0000 0000 6b1a 0000 7c00 5f0d 0000  ......k...|._...
+00000f00: 0000 0000 0000 7c00 6a1d 0000 0000 0000  ......|.j.......
+00000f10: 0000 0000 0000 0000 0000 0000 7c01 ac03  ............|...
+00000f20: ab01 0000 0000 0000 0100 7900 2904 4e72  ..........y.).Nr
+00000f30: 0200 0000 5429 0172 4e00 0000 290f 7245  ....T).rN...).rE
+00000f40: 0000 0072 0a00 0000 7248 0000 0072 4700  ...r....rH...rG.
+00000f50: 0000 7241 0000 0072 3e00 0000 da05 6d6f  ..rA...r>.....mo
+00000f60: 6465 6cda 0a76 6973 6962 696c 6974 79da  del..visibility.
+00000f70: 0d6c 696e 655f 6f66 5f73 6967 6874 7223  .line_of_sightr#
+00000f80: 0000 0072 3f00 0000 723c 0000 0072 3d00  ...r?...r<...r=.
+00000f90: 0000 7225 0000 00da 086e 6176 6967 6174  ..r%.....navigat
+00000fa0: 6529 0472 2e00 0000 724e 0000 0072 2200  e).r....rN...r".
+00000fb0: 0000 7221 0000 0073 0400 0000 2020 2020  ..r!...s....    
+00000fc0: 7228 0000 00da 0473 7465 707a 0a4d 6f75  r(.....stepz.Mou
+00000fd0: 7365 2e73 7465 7048 0000 0073 f500 0000  se.stepH...s....
+00000fe0: 8000 d80b 0fd7 0b1e d10b 1ea0 21d2 0b23  ............!..#
+00000ff0: dc20 28a8 14af 1aa9 1ad7 293c d129 3cd8  . (.......)<.)<.
+00001000: 292d af1d a91d d729 3cd1 293c d729 45d1  )-.....)<.)<.)E.
+00001010: 2945 f303 0121 4701 d00c 1de0 0f20 a044  )E...!G...... .D
+00001020: d724 37d1 2437 d20f 37d8 1317 973a 913a  .$7.$7..7....:.:
+00001030: d713 28d1 1328 d713 36d1 1336 b074 b77a  ..(..(..6..6.t.z
+00001040: b17a d737 4ad1 374a c844 cf4d c94d d74c  .z.7J.7J.D.M.M.L
+00001050: 5fd1 4c5f d74c 68d1 4c68 d413 69d8 2226  _.L_.Lh.Lh..i."&
+00001060: 9044 944b d82a 2ed7 2a42 d12a 4290 44d4  .D.K.*..*B.*B.D.
+00001070: 1427 e00b 1290 54d7 1528 d115 28d2 0b28  .'....T..(..(..(
+00001080: d80c 10d7 0c1f d20c 1fa0 37d1 0c2a d60c  ..........7..*..
+00001090: 1fe0 2223 8844 d40c 1fe4 1820 a014 d721  .."#.D..... ...!
+000010a0: 33d1 2133 b054 b75a b15a d735 48d1 3548  3.!3.T.Z.Z.5H.5H
+000010b0: d318 4988 0dd8 1825 a814 d729 3cd1 293c  ..I....%...)<.)<
+000010c0: d118 3c88 048c 0dd8 080c 8f0d 890d 9867  ..<............g
+000010d0: 880d d508 2672 2700 0000 da06 7265 7475  ....&r'.....retu
+000010e0: 726e 6300 0000 0000 0000 0000 0000 0005  rnc.............
+000010f0: 0000 0003 0000 00f3 aa00 0000 9700 7400  ..............t.
+00001100: 0000 0000 0000 0000 6a02 0000 0000 0000  ........j.......
+00001110: 0000 0000 0000 0000 0000 0000 6a05 0000  ............j...
+00001120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001130: 7407 0000 0000 0000 0000 6a08 0000 0000  t.........j.....
+00001140: 0000 0000 0000 0000 0000 0000 0000 6401  ..............d.
+00001150: ab01 0000 0000 0000 ab01 0000 0000 0000  ................
+00001160: 7d00 7400 0000 0000 0000 0000 6a0a 0000  }.t.........j...
+00001170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001180: 6a0d 0000 0000 0000 0000 0000 0000 0000  j...............
+00001190: 0000 0000 7c00 6402 ab02 0000 0000 0000  ....|.d.........
+000011a0: 7d01 7c01 5300 2903 4e7a 0870 7265 792e  }.|.S.).Nz.prey.
+000011b0: 706e 6769 0e01 0000 2907 da06 7079 6761  pngi....)...pyga
+000011c0: 6d65 da05 696d 6167 65da 046c 6f61 6472  me..image..loadr
+000011d0: 0800 0000 da04 6669 6c65 da09 7472 616e  ......file..tran
+000011e0: 7366 6f72 6dda 0672 6f74 6174 6529 02da  sform..rotate)..
+000011f0: 0673 7072 6974 65da 0e72 6f74 6174 6564  .sprite..rotated
+00001200: 5f73 7072 6974 6573 0200 0000 2020 7228  _sprites....  r(
+00001210: 0000 00da 0d63 7265 6174 655f 7370 7269  .....create_spri
+00001220: 7465 7a13 4d6f 7573 652e 6372 6561 7465  tez.Mouse.create
+00001230: 5f73 7072 6974 655a 0000 0073 3d00 0000  _spriteZ...s=...
+00001240: 8000 e411 1797 1c91 1cd7 1122 d111 22a4  ..........."..".
+00001250: 39a7 3ea1 3eb0 2ad3 233d d311 3e88 06dc  9.>.>.*.#=..>...
+00001260: 191f d719 29d1 1929 d719 30d1 1930 b016  ....)..)..0..0..
+00001270: b813 d319 3d88 0ed8 0f1d d008 1d72 2700  ....=........r'.
+00001280: 0000 6300 0000 0000 0000 0000 0000 0004  ..c.............
+00001290: 0000 0003 0000 00f3 3000 0000 9700 7401  ........0.....t.
+000012a0: 0000 0000 0000 0000 6a02 0000 0000 0000  ........j.......
+000012b0: 0000 0000 0000 0000 0000 0000 6700 6401  ............g.d.
+000012c0: a201 ab01 0000 0000 0000 5300 2902 4e29  ..........S.).N)
+000012d0: 0429 0267 b81e 85eb 51b8 8e3f 7202 0000  .).g....Q..?r...
+000012e0: 0029 0272 0200 0000 677b 14ae 47e1 7a74  .).r....g{..G.zt
+000012f0: 3f29 0267 b81e 85eb 51b8 8ebf 7202 0000  ?).g....Q...r...
+00001300: 0029 0272 0200 0000 677b 14ae 47e1 7a74  .).r....g{..G.zt
+00001310: bf29 02da 0273 70da 0750 6f6c 7967 6f6e  .)...sp..Polygon
+00001320: 7226 0000 0072 2700 0000 7228 0000 00da  r&...r'...r(....
+00001330: 0e63 7265 6174 655f 706f 6c79 676f 6e7a  .create_polygonz
+00001340: 144d 6f75 7365 2e63 7265 6174 655f 706f  .Mouse.create_po
+00001350: 6c79 676f 6e60 0000 0073 1200 0000 8000  lygon`...s......
+00001360: e40f 118f 7a89 7ad2 1a4a d30f 4bd0 084b  ....z.z..J..K..K
+00001370: 7227 0000 00da 0d61 6374 696f 6e5f 6e75  r'.....action_nu
+00001380: 6d62 6572 6302 0000 0000 0000 0000 0000  mberc...........
+00001390: 0004 0000 0003 0000 00f3 4000 0000 9700  ..........@.....
+000013a0: 7c00 6a01 0000 0000 0000 0000 0000 0000  |.j.............
+000013b0: 0000 0000 0000 7c00 6a02 0000 0000 0000  ......|.j.......
+000013c0: 0000 0000 0000 0000 0000 0000 7c01 1900  ............|...
+000013d0: 0000 ab01 0000 0000 0000 0100 7900 7233  ............y.r3
+000013e0: 0000 0029 02da 0f73 6574 5f64 6573 7469  ...)...set_desti
+000013f0: 6e61 7469 6f6e 723b 0000 0029 0272 2e00  nationr;...).r..
+00001400: 0000 7264 0000 0073 0200 0000 2020 7228  ..rd...s....  r(
+00001410: 0000 00da 0a73 6574 5f61 6374 696f 6e7a  .....set_actionz
+00001420: 104d 6f75 7365 2e73 6574 5f61 6374 696f  .Mouse.set_actio
+00001430: 6e64 0000 0073 1900 0000 8000 d808 0cd7  nd...s..........
+00001440: 081c d108 1c98 549f 5c99 5ca8 2dd1 1d38  ......T.\.\.-..8
+00001450: d508 3972 2700 0000 4e29 1772 1800 0000  ..9r'...N).r....
+00001460: 7219 0000 0072 1a00 0000 7204 0000 00da  r....r....r.....
+00001470: 0674 7970 696e 67da 044c 6973 74da 0554  .typing..List..T
+00001480: 7570 6c65 da05 666c 6f61 7472 0600 0000  uple..floatr....
+00001490: 7205 0000 0072 2c00 0000 724a 0000 0072  r....r,...rJ...r
+000014a0: 4d00 0000 7254 0000 00da 0c73 7461 7469  M...rT.....stati
+000014b0: 636d 6574 686f 6472 5700 0000 da07 5375  cmethodrW.....Su
+000014c0: 7266 6163 6572 5f00 0000 7261 0000 0072  rfacer_...ra...r
+000014d0: 6200 0000 7263 0000 00da 0369 6e74 7267  b...rc.....intrg
+000014e0: 0000 0072 2600 0000 7227 0000 0072 2800  ...r&...r'...r(.
+000014f0: 0000 7239 0000 0072 3900 0000 2500 0000  ..r9...r9...%...
+00001500: 73d9 0000 0084 00f0 0216 051c d81e 28f0  s.............(.
+00001510: 0316 051c e01a 209f 2b99 2ba0 66a7 6ca1  ...... .+.+.f.l.
+00001520: 6cb0 35b8 25b0 3cd1 2640 d11a 41f0 0516  l.5.%.<.&@..A...
+00001530: 051c f006 0021 27a7 0ca1 0ca8 55b0 45a8  .....!'.....U.E.
+00001540: 5cd1 203a f007 1605 1cf0 0800 2227 f009  \. :........"'..
+00001550: 1605 1cf0 0a00 2227 f00b 1605 1cf0 0c00  ......"'........
+00001560: 272c f00d 1605 1cf0 0e00 1e28 f00f 1605  ',.........(....
+00001570: 1cf0 1000 1c21 f311 1605 1cf2 3005 0524  .....!......0..$
+00001580: f20e 0105 24f0 0610 0527 9845 f300 1005  ....$....'.E....
+00001590: 27f0 2400 0612 f002 0305 1e98 369f 3e99  '.$.........6.>.
+000015a0: 3ef2 0003 051e f303 0006 12f0 0203 051e  >...............
+000015b0: f00a 0006 12f0 0201 054c 0198 429f 4a99  .........L..B.J.
+000015c0: 4af2 0001 054c 01f3 0300 0612 f002 0105  J....L..........
+000015d0: 4c01 f006 0105 3aa8 03f4 0001 053a 7227  L.....:......:r'
+000015e0: 0000 0072 3900 0000 2916 da04 6d61 7468  ...r9...)...math
+000015f0: 7268 0000 0072 5700 0000 da05 6167 656e  rh...rW.....agen
+00001600: 7472 0400 0000 7205 0000 0072 4000 0000  tr....r....r@...
+00001610: 7206 0000 00da 106e 6176 6967 6174 696f  r......navigatio
+00001620: 6e5f 6167 656e 7472 0700 0000 da09 7265  n_agentr......re
+00001630: 736f 7572 6365 7372 0800 0000 da07 7368  sourcesr......sh
+00001640: 6170 656c 7972 6100 0000 da04 656e 756d  apelyra.....enum
+00001650: 7209 0000 00da 0475 7469 6c72 0a00 0000  r......utilr....
+00001660: 7269 0000 0072 6b00 0000 720c 0000 0072  ri...rk...r....r
+00001670: 3900 0000 7226 0000 0072 2700 0000 7228  9...r&...r'...r(
+00001680: 0000 00fa 083c 6d6f 6475 6c65 3e72 7600  .....<module>rv.
+00001690: 0000 0100 0000 7346 0000 00f0 0301 0101  ......sF........
+000016a0: db00 0bdb 000d e300 0ddf 0024 dd00 22dd  ...........$..".
+000016b0: 002d dd00 20db 0014 dd00 15dd 001a f406  .-.. ...........
+000016c0: 1401 3390 7697 7b91 7ba0 35d1 1729 f400  ..3.v.{.{.5..)..
+000016d0: 1401 33f4 2e40 0101 3a88 4ff5 0040 0101  ..3..@..:.O..@..
+000016e0: 3a72 2700 0000                           :r'...
```

### Comparing `cellworld_game-0.0.61/cellworld_game/__pycache__/ray_tracing.cpython-312.pyc` & `cellworld_game-0.0.68/cellworld_game/__pycache__/ray_tracing.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Sun Apr 21 15:20:54 2024 UTC, .py size: 4973 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-00000000: cb0d 0d0a 0000 0000 d62e 2566 6d13 0000  ..........%fm...
+00000000: cb0d 0d0a 0000 0000 4482 1166 0c13 0000  ........D..f....
 00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
 00000020: 0000 0000 00f3 5c00 0000 9700 6400 6401  ......\.....d.d.
-00000030: 6c00 5a00 6400 6401 6c01 5a01 6400 6401  l.Z.d.d.l.Z.d.d.
-00000040: 6c02 5a02 6400 6401 6c03 5a04 6402 6403  l.Z.d.d.l.Z.d.d.
-00000050: 6c05 6d06 5a06 0100 6402 6404 6c07 6d08  l.m.Z...d.d.l.m.
-00000060: 5a08 0100 6402 6405 6c09 6d0a 5a0a 0100  Z...d.d.l.m.Z...
+00000030: 6c00 5a00 6400 6401 6c01 5a02 6402 6403  l.Z.d.d.l.Z.d.d.
+00000040: 6c03 6d04 5a04 0100 6402 6404 6c05 6d06  l.m.Z...d.d.l.m.
+00000050: 5a06 0100 6402 6405 6c07 6d08 5a08 0100  Z...d.d.l.m.Z...
+00000060: 6400 6401 6c09 5a09 6400 6401 6c0a 5a0a  d.d.l.Z.d.d.l.Z.
 00000070: 0200 4700 6406 8400 6407 ab02 0000 0000  ..G.d...d.......
 00000080: 0000 5a0b 7901 2908 e900 0000 004e e901  ..Z.y.)......N..
 00000090: 0000 0029 01da 054d 6f64 656c 2901 da0a  ...)...Model)...
 000000a0: 4167 656e 7453 7461 7465 2901 da12 6372  AgentState)...cr
 000000b0: 6561 7465 5f6c 696e 655f 7374 7269 6e67  eate_line_string
 000000c0: 6300 0000 0000 0000 0000 0000 000b 0000  c...............
 000000d0: 0000 0000 00f3 9c00 0000 9700 6500 5a01  ............e.Z.
@@ -68,15 +68,15 @@
 00000430: 636c 7573 696f 6e5f 636f 6c6f 72da 106f  clusion_color..o
 00000440: 6363 6c75 7369 6f6e 5f68 6569 6768 74da  cclusion_height.
 00000450: 0a77 616c 6c5f 636f 6c6f 72da 0b77 616c  .wall_color..wal
 00000460: 6c5f 6865 6967 6874 2907 da04 7365 6c66  l_height)...self
 00000470: 7209 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
 00000480: 0c00 0000 720d 0000 00da 096f 6363 6c75  ....r......occlu
 00000490: 7369 6f6e 7307 0000 0020 2020 2020 2020  sions....       
-000004a0: fa38 433a 5c52 6573 6561 7263 685c 6365  .8C:\Research\ce
+000004a0: fa38 433a 5c72 6573 6561 7263 685c 6365  .8C:\research\ce
 000004b0: 6c6c 776f 726c 645f 6761 6d65 5c63 656c  llworld_game\cel
 000004c0: 6c77 6f72 6c64 5f67 616d 655c 7261 795f  lworld_game\ray_
 000004d0: 7472 6163 696e 672e 7079 da08 5f5f 696e  tracing.py..__in
 000004e0: 6974 5f5f 7a13 5261 7954 7261 6369 6e67  it__z.RayTracing
 000004f0: 2e5f 5f69 6e69 745f 5f0b 0000 0073 a300  .__init__....s..
 00000500: 0000 8000 f00a 0016 1b88 048c 0ad8 2336  ..............#6
 00000510: 8804 d408 20d8 253a 8804 d408 22d8 2234  .... .%:...."."4
@@ -364,17 +364,17 @@
 000016b0: f007 1005 26f0 0800 1e21 f309 1005 26f0  ....&....!....&.
 000016c0: 2401 053e a805 f000 0105 3eb0 25f3 0001  $..>......>.%...
 000016d0: 053e f006 0305 5d01 d065 6bd7 6571 d165  .>....]..ek.eq.e
 000016e0: 71d0 7277 d079 7ed0 727e d165 7ff3 0003  q.rw.y~.r~.e....
 000016f0: 055d 01f0 0a0f 0530 c815 f300 0f05 30f0  .].....0......0.
 00001700: 222b 051e a02a f000 2b05 1eb0 66b7 6eb1  "+...*..+...f.n.
 00001710: 6ef4 002b 051e 7226 0000 0072 0800 0000  n..+..r&...r....
-00001720: 290c 7240 0000 0072 2900 0000 7271 0000  ).r@...r)...rq..
-00001730: 00da 0773 6861 7065 6c79 7211 0000 0072  ...shapelyr....r
-00001740: 0900 0000 7204 0000 00da 0561 6765 6e74  ....r......agent
-00001750: 7205 0000 00da 0475 7469 6c72 0600 0000  r......utilr....
+00001720: 290c 7271 0000 00da 0773 6861 7065 6c79  ).rq.....shapely
+00001730: 7211 0000 0072 0900 0000 7204 0000 00da  r....r....r.....
+00001740: 0561 6765 6e74 7205 0000 00da 0475 7469  .agentr......uti
+00001750: 6c72 0600 0000 7240 0000 0072 2900 0000  lr....r@...r)...
 00001760: 7208 0000 0072 3500 0000 7226 0000 0072  r....r5...r&...r
 00001770: 1f00 0000 fa08 3c6d 6f64 756c 653e 7277  ......<module>rw
 00001780: 0000 0001 0000 0073 2600 0000 f003 0101  .......s&.......
-00001790: 01db 000d db00 0bdb 000d db00 14dd 0018  ................
-000017a0: dd00 1ddd 0024 f706 5701 011e f200 5701  .....$..W.....W.
+00001790: 01db 000d db00 14dd 0018 dd00 1ddd 0024  ...............$
+000017a0: db00 0ddb 000b f706 5701 011e f200 5701  ........W.....W.
 000017b0: 011e 7226 0000 00                        ..r&...
```

### Comparing `cellworld_game-0.0.61/cellworld_game/__pycache__/robot.cpython-312.pyc` & `cellworld_game-0.0.68/cellworld_game/__pycache__/robot.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Fri Apr 26 16:24:32 2024 UTC, .py size: 1542 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 23% similar despite different names*

```diff
@@ -1,172 +1,207 @@
-00000000: cb0d 0d0a 0000 0000 40d5 2b66 0606 0000  ........@.+f....
+00000000: cb0d 0d0a 0000 0000 4a90 1566 2a07 0000  ........J..f*...
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
-00000020: 0000 0000 00f3 6a00 0000 9700 6400 6401  ......j.....d.d.
-00000030: 6c00 5a01 6400 6401 6c02 5a02 6400 6401  l.Z.d.d.l.Z.d.d.
-00000040: 6c03 5a03 6400 6401 6c04 5a04 6402 6403  l.Z.d.d.l.Z.d.d.
-00000050: 6c05 6d06 5a06 0100 6402 6404 6c07 6d08  l.m.Z...d.d.l.m.
-00000060: 5a08 0100 6402 6405 6c09 6d0a 5a0a 0100  Z...d.d.l.m.Z...
-00000070: 6402 6406 6c0b 6d0c 5a0c 0100 0200 4700  d.d.l.m.Z.....G.
-00000080: 6407 8400 6408 650a ab03 0000 0000 0000  d...d.e.........
-00000090: 5a0d 7901 2909 e900 0000 004e e901 0000  Z.y.)......N....
-000000a0: 0029 01da 0a41 6765 6e74 5374 6174 6529  .)...AgentState)
-000000b0: 01da 0a4e 6176 6967 6174 696f 6e29 01da  ...Navigation)..
-000000c0: 0f4e 6176 6967 6174 696f 6e41 6765 6e74  .NavigationAgent
-000000d0: 2901 da09 5265 736f 7572 6365 7363 0000  )...Resourcesc..
-000000e0: 0000 0000 0000 0000 0000 0700 0000 0000  ................
-000000f0: 0000 f3f6 0000 0097 0065 005a 0164 005a  .........e.Z.d.Z
-00000100: 0264 0165 036a 0800 0000 0000 0000 0000  .d.e.j..........
-00000110: 0000 0000 0000 0000 0065 036a 0a00 0000  .........e.j....
-00000120: 0000 0000 0000 0000 0000 0000 0000 0065  ...............e
-00000130: 0665 0666 0219 0000 0019 0000 0064 0265  .e.f.........d.e
-00000140: 036a 0800 0000 0000 0000 0000 0000 0000  .j..............
-00000150: 0000 0000 0065 036a 0a00 0000 0000 0000  .....e.j........
-00000160: 0000 0000 0000 0000 0000 0065 0665 0666  ...........e.e.f
-00000170: 0219 0000 0019 0000 0064 0365 0766 0664  .........d.e.f.d
-00000180: 0484 045a 0864 0584 005a 0965 0a64 0665  ...Z.d...Z.e.d.e
-00000190: 0b6a 1800 0000 0000 0000 0000 0000 0000  .j..............
-000001a0: 0000 0000 0066 0264 0784 04ab 0000 0000  .....f.d........
-000001b0: 0000 005a 0d65 0a64 0665 0e6a 1e00 0000  ...Z.e.d.e.j....
-000001c0: 0000 0000 0000 0000 0000 0000 0000 0066  ...............f
-000001d0: 0264 0884 04ab 0000 0000 0000 005a 1064  .d...........Z.d
-000001e0: 0965 0666 0264 0a84 045a 1179 0b29 0cda  .e.f.d...Z.y.)..
-000001f0: 0552 6f62 6f74 da0f 7374 6172 745f 6c6f  .Robot..start_lo
-00000200: 6361 7469 6f6e 73da 0e6f 7065 6e5f 6c6f  cations..open_lo
-00000210: 6361 7469 6f6e 73da 0a6e 6176 6967 6174  cations..navigat
-00000220: 696f 6e63 0400 0000 0000 0000 0000 0000  ionc............
-00000230: 0600 0000 0300 0000 f360 0000 0097 0074  .........`.....t
-00000240: 0100 0000 0000 0000 006a 0200 0000 0000  .........j......
-00000250: 0000 0000 0000 0000 0000 0000 007c 007c  .............|.|
-00000260: 0364 0164 02ac 03ab 0400 0000 0000 0001  .d.d............
-00000270: 007c 017c 005f 0200 0000 0000 0000 007c  .|.|._.........|
-00000280: 027c 005f 0300 0000 0000 0000 0064 047c  .|._.........d.|
-00000290: 005f 0400 0000 0000 0000 0079 0029 054e  ._.........y.).N
-000002a0: 6733 3333 3333 33b3 3f67 0000 0000 0000  g333333.?g......
-000002b0: 0c40 2903 720c 0000 00da 116d 6178 5f66  .@).r......max_f
-000002c0: 6f72 7761 7264 5f73 7065 6564 da11 6d61  orward_speed..ma
-000002d0: 785f 7475 726e 696e 675f 7370 6565 6472  x_turning_speedr
-000002e0: 0200 0000 2905 7206 0000 00da 085f 5f69  ....).r......__i
-000002f0: 6e69 745f 5f72 0a00 0000 720b 0000 00da  nit__r....r.....
-00000300: 156c 6173 745f 6465 7374 696e 6174 696f  .last_destinatio
-00000310: 6e5f 7469 6d65 2904 da04 7365 6c66 720a  n_time)...selfr.
-00000320: 0000 0072 0b00 0000 720c 0000 0073 0400  ...r....r....s..
-00000330: 0000 2020 2020 fa32 433a 5c52 6573 6561  ..    .2C:\Resea
-00000340: 7263 685c 6365 6c6c 776f 726c 645f 6761  rch\cellworld_ga
-00000350: 6d65 5c63 656c 6c77 6f72 6c64 5f67 616d  me\cellworld_gam
-00000360: 655c 726f 626f 742e 7079 7210 0000 007a  e\robot.pyr....z
-00000370: 0e52 6f62 6f74 2e5f 5f69 6e69 745f 5f0c  .Robot.__init__.
-00000380: 0000 0073 3700 0000 8000 f408 0009 18d7  ...s7...........
-00000390: 0820 d108 20a0 14d8 2c36 d833 38d8 3336  . .. ...,6.38.36
-000003a0: f507 0309 38f0 0800 202f 8804 d408 1cd8  ....8... /......
-000003b0: 1e2c 8804 d408 1bd8 2526 8804 d508 22f3  .,......%&....".
-000003c0: 0000 0000 6301 0000 0000 0000 0000 0000  ....c...........
-000003d0: 0007 0000 0003 0000 00f3 a000 0000 9700  ................
-000003e0: 7401 0000 0000 0000 0000 6a02 0000 0000  t.........j.....
-000003f0: 0000 0000 0000 0000 0000 0000 0000 7c00  ..............|.
-00000400: ab01 0000 0000 0000 0100 7c00 6a05 0000  ..........|.j...
-00000410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000420: 7407 0000 0000 0000 0000 7409 0000 0000  t.........t.....
-00000430: 0000 0000 6a0a 0000 0000 0000 0000 0000  ....j...........
-00000440: 0000 0000 0000 0000 7c00 6a0c 0000 0000  ........|.j.....
-00000450: 0000 0000 0000 0000 0000 0000 0000 ab01  ................
-00000460: 0000 0000 0000 6401 ac02 ab02 0000 0000  ......d.........
-00000470: 0000 ab01 0000 0000 0000 0100 7900 2903  ............y.).
-00000480: 4ee9 b400 0000 2902 da08 6c6f 6361 7469  N.....)...locati
-00000490: 6f6e da09 6469 7265 6374 696f 6e29 0772  on..direction).r
-000004a0: 0600 0000 da05 7265 7365 74da 0973 6574  ......reset..set
-000004b0: 5f73 7461 7465 7204 0000 00da 0672 616e  _stater......ran
-000004c0: 646f 6dda 0663 686f 6963 6572 0a00 0000  dom..choicer....
-000004d0: 2901 7212 0000 0073 0100 0000 2072 1300  ).r....s.... r..
-000004e0: 0000 7219 0000 007a 0b52 6f62 6f74 2e72  ..r....z.Robot.r
-000004f0: 6573 6574 1800 0000 7337 0000 0080 00dc  eset....s7......
-00000500: 0817 d708 1dd1 081d 9864 d408 23d8 080c  .........d..#...
-00000510: 8f0e 890e 947a ac36 af3d a93d b814 d739  .....z.6.=.=...9
-00000520: 4dd1 394d d32b 4ed8 2c2f f403 0118 31f5  M.9M.+N.,/....1.
-00000530: 0001 0932 7214 0000 00da 0672 6574 7572  ...2r......retur
-00000540: 6e63 0000 0000 0000 0000 0000 0000 0500  nc..............
-00000550: 0000 0300 0000 f3aa 0000 0097 0074 0000  .............t..
-00000560: 0000 0000 0000 006a 0200 0000 0000 0000  .......j........
-00000570: 0000 0000 0000 0000 0000 006a 0500 0000  ...........j....
-00000580: 0000 0000 0000 0000 0000 0000 0000 0074  ...............t
-00000590: 0700 0000 0000 0000 006a 0800 0000 0000  .........j......
-000005a0: 0000 0000 0000 0000 0000 0000 0064 01ab  .............d..
-000005b0: 0100 0000 0000 00ab 0100 0000 0000 007d  ...............}
-000005c0: 0074 0000 0000 0000 0000 006a 0a00 0000  .t.........j....
-000005d0: 0000 0000 0000 0000 0000 0000 0000 006a  ...............j
-000005e0: 0d00 0000 0000 0000 0000 0000 0000 0000  ................
-000005f0: 0000 007c 0064 02ab 0200 0000 0000 007d  ...|.d.........}
-00000600: 017c 0153 0029 034e 7a0c 7072 6564 6174  .|.S.).Nz.predat
-00000610: 6f72 2e70 6e67 690e 0100 0029 07da 0670  or.pngi....)...p
-00000620: 7967 616d 65da 0569 6d61 6765 da04 6c6f  ygame..image..lo
-00000630: 6164 7207 0000 00da 0466 696c 65da 0974  adr......file..t
-00000640: 7261 6e73 666f 726d da06 726f 7461 7465  ransform..rotate
-00000650: 2902 da06 7370 7269 7465 da0e 726f 7461  )...sprite..rota
-00000660: 7465 645f 7370 7269 7465 7302 0000 0020  ted_sprites.... 
-00000670: 2072 1300 0000 da0d 6372 6561 7465 5f73   r......create_s
-00000680: 7072 6974 657a 1352 6f62 6f74 2e63 7265  pritez.Robot.cre
-00000690: 6174 655f 7370 7269 7465 1d00 0000 733d  ate_sprite....s=
-000006a0: 0000 0080 00e4 1117 971c 911c d711 22d1  ..............".
-000006b0: 1122 a439 a73e a13e b02e d323 41d3 1142  .".9.>.>...#A..B
-000006c0: 8806 dc19 1fd7 1929 d119 29d7 1930 d119  .......)..)..0..
-000006d0: 30b0 16b8 13d3 193d 880e d80f 1dd0 081d  0......=........
-000006e0: 7214 0000 0063 0000 0000 0000 0000 0000  r....c..........
-000006f0: 0000 0400 0000 0300 0000 f330 0000 0097  ...........0....
-00000700: 0074 0100 0000 0000 0000 006a 0200 0000  .t.........j....
-00000710: 0000 0000 0000 0000 0000 0000 0000 0067  ...............g
-00000720: 0064 01a2 01ab 0100 0000 0000 0053 0029  .d...........S.)
-00000730: 024e 2906 2902 e77b 14ae 47e1 7a94 3fe7  .N).)..{..G.z.?.
-00000740: 39b4 c876 be9f 8a3f 2902 e77b 14ae 47e1  9..v...?)..{..G.
-00000750: 7a94 bf72 2a00 0000 2902 722b 0000 00e7  z..r*...).r+....
-00000760: 39b4 c876 be9f 8abf 2902 7229 0000 0072  9..v....).r)...r
-00000770: 2c00 0000 2902 e79a 9999 9999 9999 3f67  ,...).........?g
-00000780: 7b14 ae47 e17a 84bf 2902 722d 0000 0067  {..G.z..).r-...g
-00000790: 7b14 ae47 e17a 843f 2902 da02 7370 da07  {..G.z.?)...sp..
-000007a0: 506f 6c79 676f 6ea9 0072 1400 0000 7213  Polygon..r....r.
-000007b0: 0000 00da 0e63 7265 6174 655f 706f 6c79  .....create_poly
-000007c0: 676f 6e7a 1452 6f62 6f74 2e63 7265 6174  gonz.Robot.creat
-000007d0: 655f 706f 6c79 676f 6e23 0000 0073 1200  e_polygon#...s..
-000007e0: 0000 8000 e40f 118f 7a89 7ad2 1a73 d30f  ........z.z..s..
-000007f0: 74d0 0874 7214 0000 00da 0764 656c 7461  t..tr......delta
-00000800: 5f74 6302 0000 0000 0000 0000 0000 0004  _tc.............
-00000810: 0000 0003 0000 00f3 3200 0000 9700 7401  ........2.....t.
-00000820: 0000 0000 0000 0000 6a02 0000 0000 0000  ........j.......
-00000830: 0000 0000 0000 0000 0000 0000 7c00 7c01  ............|.|.
-00000840: ac01 ab02 0000 0000 0000 0100 7900 2902  ............y.).
-00000850: 4ea9 0272 1200 0000 7232 0000 0029 0272  N..r....r2...).r
-00000860: 0600 0000 da04 7374 6570 7234 0000 0073  ......stepr4...s
-00000870: 0200 0000 2020 7213 0000 0072 3500 0000  ....  r....r5...
-00000880: 7a0a 526f 626f 742e 7374 6570 2700 0000  z.Robot.step'...
-00000890: 7315 0000 0080 00dc 0817 d708 1cd1 081c  s...............
-000008a0: a024 d825 2cf6 0301 092e 7214 0000 004e  .$.%,.....r....N
-000008b0: 2912 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-000008c0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-000008d0: 6e61 6d65 5f5f da06 7479 7069 6e67 da04  name__..typing..
-000008e0: 4c69 7374 da05 5475 706c 65da 0566 6c6f  List..Tuple..flo
-000008f0: 6174 7205 0000 0072 1000 0000 7219 0000  atr....r....r...
-00000900: 00da 0c73 7461 7469 636d 6574 686f 6472  ...staticmethodr
-00000910: 1f00 0000 da07 5375 7266 6163 6572 2700  ......Surfacer'.
-00000920: 0000 722e 0000 0072 2f00 0000 7231 0000  ..r....r/...r1..
-00000930: 0072 3500 0000 7230 0000 0072 1400 0000  .r5...r0...r....
-00000940: 7213 0000 0072 0900 0000 7209 0000 000b  r....r....r.....
-00000950: 0000 0073 9f00 0000 8400 f002 0a05 27d8  ...s..........'.
-00000960: 2228 a72b a12b a866 af6c a96c b835 c025  "(.+.+.f.l.l.5.%
-00000970: b83c d12e 48d1 2249 f003 0a05 27e0 2127  .<..H."I....'.!'
-00000980: a71b a11b a856 af5c a95c b825 c015 b82c  .....V.\.\.%...,
-00000990: d12d 47d1 2148 f005 0a05 27f0 0600 1e28  .-G.!H....'....(
-000009a0: f307 0a05 27f2 1803 0532 f00a 0006 12f0  ....'....2......
-000009b0: 0203 051e 9836 9f3e 993e f200 0305 1ef3  .....6.>.>......
-000009c0: 0300 0612 f002 0305 1ef0 0a00 0612 f002  ................
-000009d0: 0105 7501 9842 9f4a 994a f200 0105 7501  ..u..B.J.J....u.
-000009e0: f303 0006 12f0 0201 0575 01f0 0602 052e  .........u......
-000009f0: 9845 f400 0205 2e72 1400 0000 7209 0000  .E.....r....r...
-00000a00: 0029 0eda 0773 6861 7065 6c79 722e 0000  .)...shapelyr...
-00000a10: 0072 1b00 0000 7239 0000 0072 1f00 0000  .r....r9...r....
-00000a20: da05 6167 656e 7472 0400 0000 720c 0000  ..agentr....r...
-00000a30: 0072 0500 0000 da10 6e61 7669 6761 7469  .r......navigati
-00000a40: 6f6e 5f61 6765 6e74 7206 0000 00da 0972  on_agentr......r
-00000a50: 6573 6f75 7263 6573 7207 0000 0072 0900  esourcesr....r..
-00000a60: 0000 7230 0000 0072 1400 0000 7213 0000  ..r0...r....r...
-00000a70: 00fa 083c 6d6f 6475 6c65 3e72 4300 0000  ...<module>rC...
-00000a80: 0100 0000 7329 0000 00f0 0301 0101 db00  ....s)..........
-00000a90: 14db 000d db00 0ddb 000d dd00 1ddd 0022  ..............."
-00000aa0: dd00 2ddd 0020 f406 1e01 2e88 4ff5 001e  ..-.. ......O...
-00000ab0: 012e 7214 0000 00                        ..r....
+00000020: 0000 0000 00f3 6600 0000 9700 6400 6401  ......f.....d.d.
+00000030: 6c00 5a00 6400 6401 6c01 5a01 6400 6401  l.Z.d.d.l.Z.d.d.
+00000040: 6c02 5a02 6402 6403 6c03 6d04 5a04 0100  l.Z.d.d.l.m.Z...
+00000050: 6402 6404 6c05 6d06 5a06 0100 6402 6405  d.d.l.m.Z...d.d.
+00000060: 6c07 6d08 5a08 0100 6400 6401 6c09 5a0a  l.m.Z...d.d.l.Z.
+00000070: 6400 6401 6c0b 5a0b 0200 4700 6406 8400  d.d.l.Z...G.d...
+00000080: 6407 6506 ab03 0000 0000 0000 5a0c 7901  d.e.........Z.y.
+00000090: 2908 e900 0000 004e e901 0000 0029 01da  )......N.....)..
+000000a0: 0a4e 6176 6967 6174 696f 6e29 01da 0f4e  .Navigation)...N
+000000b0: 6176 6967 6174 696f 6e41 6765 6e74 2901  avigationAgent).
+000000c0: da09 5265 736f 7572 6365 7363 0000 0000  ..Resourcesc....
+000000d0: 0000 0000 0000 0000 0700 0000 0000 0000  ................
+000000e0: f3f6 0000 0097 0065 005a 0164 005a 0264  .......e.Z.d.Z.d
+000000f0: 0165 036a 0800 0000 0000 0000 0000 0000  .e.j............
+00000100: 0000 0000 0000 0065 036a 0a00 0000 0000  .......e.j......
+00000110: 0000 0000 0000 0000 0000 0000 0065 0665  .............e.e
+00000120: 0666 0219 0000 0019 0000 0064 0265 036a  .f.........d.e.j
+00000130: 0800 0000 0000 0000 0000 0000 0000 0000  ................
+00000140: 0000 0065 036a 0a00 0000 0000 0000 0000  ...e.j..........
+00000150: 0000 0000 0000 0000 0065 0665 0666 0219  .........e.e.f..
+00000160: 0000 0019 0000 0064 0365 0766 0664 0484  .......d.e.f.d..
+00000170: 045a 0864 0584 005a 0965 0a64 0665 0b6a  .Z.d...Z.e.d.e.j
+00000180: 1800 0000 0000 0000 0000 0000 0000 0000  ................
+00000190: 0000 0066 0264 0784 04ab 0000 0000 0000  ...f.d..........
+000001a0: 005a 0d65 0a64 0665 0e6a 1e00 0000 0000  .Z.e.d.e.j......
+000001b0: 0000 0000 0000 0000 0000 0000 0066 0264  .............f.d
+000001c0: 0884 04ab 0000 0000 0000 005a 1064 0965  ...........Z.d.e
+000001d0: 0666 0264 0a84 045a 1179 0b29 0cda 0552  .f.d...Z.y.)...R
+000001e0: 6f62 6f74 da0f 7374 6172 745f 6c6f 6361  obot..start_loca
+000001f0: 7469 6f6e 73da 0e6f 7065 6e5f 6c6f 6361  tions..open_loca
+00000200: 7469 6f6e 73da 0a6e 6176 6967 6174 696f  tions..navigatio
+00000210: 6e63 0400 0000 0000 0000 0000 0000 0600  nc..............
+00000220: 0000 0300 0000 f360 0000 0097 0074 0100  .......`.....t..
+00000230: 0000 0000 0000 006a 0200 0000 0000 0000  .......j........
+00000240: 0000 0000 0000 0000 0000 007c 007c 0364  ...........|.|.d
+00000250: 0164 02ac 03ab 0400 0000 0000 0001 007c  .d.............|
+00000260: 017c 005f 0200 0000 0000 0000 007c 027c  .|._.........|.|
+00000270: 005f 0300 0000 0000 0000 0064 047c 005f  ._.........d.|._
+00000280: 0400 0000 0000 0000 0079 0029 054e 6733  .........y.).Ng3
+00000290: 3333 3333 33b3 3f67 0000 0000 0000 0c40  33333.?g.......@
+000002a0: 2903 720b 0000 00da 116d 6178 5f66 6f72  ).r......max_for
+000002b0: 7761 7264 5f73 7065 6564 da11 6d61 785f  ward_speed..max_
+000002c0: 7475 726e 696e 675f 7370 6565 6472 0200  turning_speedr..
+000002d0: 0000 2905 7205 0000 00da 085f 5f69 6e69  ..).r......__ini
+000002e0: 745f 5f72 0900 0000 720a 0000 00da 156c  t__r....r......l
+000002f0: 6173 745f 6465 7374 696e 6174 696f 6e5f  ast_destination_
+00000300: 7469 6d65 2904 da04 7365 6c66 7209 0000  time)...selfr...
+00000310: 0072 0a00 0000 720b 0000 0073 0400 0000  .r....r....s....
+00000320: 2020 2020 fa32 433a 5c72 6573 6561 7263      .2C:\researc
+00000330: 685c 6365 6c6c 776f 726c 645f 6761 6d65  h\cellworld_game
+00000340: 5c63 656c 6c77 6f72 6c64 5f67 616d 655c  \cellworld_game\
+00000350: 726f 626f 742e 7079 720f 0000 007a 0e52  robot.pyr....z.R
+00000360: 6f62 6f74 2e5f 5f69 6e69 745f 5f0c 0000  obot.__init__...
+00000370: 0073 3700 0000 8000 f408 0009 18d7 0820  .s7............ 
+00000380: d108 20a0 14d8 2c36 d833 38d8 3336 f507  .. ...,6.38.36..
+00000390: 0309 38f0 0800 202f 8804 d408 1cd8 1e2c  ..8... /.......,
+000003a0: 8804 d408 1bd8 2526 8804 d508 22f3 0000  ......%&...."...
+000003b0: 0000 6301 0000 0000 0000 0000 0000 0003  ..c.............
+000003c0: 0000 0003 0000 00f3 ac00 0000 9700 7401  ..............t.
+000003d0: 0000 0000 0000 0000 6a02 0000 0000 0000  ........j.......
+000003e0: 0000 0000 0000 0000 0000 0000 7c00 ab01  ............|...
+000003f0: 0000 0000 0000 0100 7405 0000 0000 0000  ........t.......
+00000400: 0000 6a06 0000 0000 0000 0000 0000 0000  ..j.............
+00000410: 0000 0000 0000 7c00 6a08 0000 0000 0000  ......|.j.......
+00000420: 0000 0000 0000 0000 0000 0000 ab01 0000  ................
+00000430: 0000 0000 7c00 6a0a 0000 0000 0000 0000  ....|.j.........
+00000440: 0000 0000 0000 0000 0000 5f06 0000 0000  .........._.....
+00000450: 0000 0000 6401 7c00 6a0a 0000 0000 0000  ....d.|.j.......
+00000460: 0000 0000 0000 0000 0000 0000 5f07 0000  ............_...
+00000470: 0000 0000 0000 7900 2902 4ee9 b400 0000  ......y.).N.....
+00000480: 2908 7205 0000 00da 0572 6573 6574 da06  ).r......reset..
+00000490: 7261 6e64 6f6d da06 6368 6f69 6365 7209  random..choicer.
+000004a0: 0000 00da 0573 7461 7465 da08 6c6f 6361  .....state..loca
+000004b0: 7469 6f6e da09 6469 7265 6374 696f 6e29  tion..direction)
+000004c0: 0172 1100 0000 7301 0000 0020 7212 0000  .r....s.... r...
+000004d0: 0072 1600 0000 7a0b 526f 626f 742e 7265  .r....z.Robot.re
+000004e0: 7365 7418 0000 0073 3700 0000 8000 dc08  set....s7.......
+000004f0: 17d7 081d d108 1d98 64d4 0823 dc1e 249f  ........d..#..$.
+00000500: 6d99 6da8 44d7 2c40 d12c 40d3 1e41 8804  m.m.D.,@.,@..A..
+00000510: 8f0a 890a d408 1bd8 1f22 8804 8f0a 890a  ........."......
+00000520: d508 1c72 1300 0000 da06 7265 7475 726e  ...r......return
+00000530: 6300 0000 0000 0000 0000 0000 0005 0000  c...............
+00000540: 0003 0000 00f3 aa00 0000 9700 7400 0000  ............t...
+00000550: 0000 0000 0000 6a02 0000 0000 0000 0000  ......j.........
+00000560: 0000 0000 0000 0000 0000 6a05 0000 0000  ..........j.....
+00000570: 0000 0000 0000 0000 0000 0000 0000 7407  ..............t.
+00000580: 0000 0000 0000 0000 6a08 0000 0000 0000  ........j.......
+00000590: 0000 0000 0000 0000 0000 0000 6401 ab01  ............d...
+000005a0: 0000 0000 0000 ab01 0000 0000 0000 7d00  ..............}.
+000005b0: 7400 0000 0000 0000 0000 6a0a 0000 0000  t.........j.....
+000005c0: 0000 0000 0000 0000 0000 0000 0000 6a0d  ..............j.
+000005d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005e0: 0000 7c00 6402 ab02 0000 0000 0000 7d01  ..|.d.........}.
+000005f0: 7c01 5300 2903 4e7a 0c70 7265 6461 746f  |.S.).Nz.predato
+00000600: 722e 706e 6769 0e01 0000 2907 da06 7079  r.pngi....)...py
+00000610: 6761 6d65 da05 696d 6167 65da 046c 6f61  game..image..loa
+00000620: 6472 0600 0000 da04 6669 6c65 da09 7472  dr......file..tr
+00000630: 616e 7366 6f72 6dda 0672 6f74 6174 6529  ansform..rotate)
+00000640: 02da 0673 7072 6974 65da 0e72 6f74 6174  ...sprite..rotat
+00000650: 6564 5f73 7072 6974 6573 0200 0000 2020  ed_sprites....  
+00000660: 7212 0000 00da 0d63 7265 6174 655f 7370  r......create_sp
+00000670: 7269 7465 7a13 526f 626f 742e 6372 6561  ritez.Robot.crea
+00000680: 7465 5f73 7072 6974 651d 0000 0073 3d00  te_sprite....s=.
+00000690: 0000 8000 e411 1797 1c91 1cd7 1122 d111  ............."..
+000006a0: 22a4 39a7 3ea1 3eb0 2ed3 2341 d311 4288  ".9.>.>...#A..B.
+000006b0: 06dc 191f d719 29d1 1929 d719 30d1 1930  ......)..)..0..0
+000006c0: b016 b813 d319 3d88 0ed8 0f1d d008 1d72  ......=........r
+000006d0: 1300 0000 6300 0000 0000 0000 0000 0000  ....c...........
+000006e0: 0004 0000 0003 0000 00f3 3000 0000 9700  ..........0.....
+000006f0: 7401 0000 0000 0000 0000 6a02 0000 0000  t.........j.....
+00000700: 0000 0000 0000 0000 0000 0000 0000 6700  ..............g.
+00000710: 6401 a201 ab01 0000 0000 0000 5300 2902  d...........S.).
+00000720: 4e29 0629 02e7 7b14 ae47 e17a 943f e739  N).)..{..G.z.?.9
+00000730: b4c8 76be 9f8a 3f29 02e7 7b14 ae47 e17a  ..v...?)..{..G.z
+00000740: 94bf 7229 0000 0029 0272 2a00 0000 e739  ..r)...).r*....9
+00000750: b4c8 76be 9f8a bf29 0272 2800 0000 722b  ..v....).r(...r+
+00000760: 0000 0029 02e7 9a99 9999 9999 993f 677b  ...).........?g{
+00000770: 14ae 47e1 7a84 bf29 0272 2c00 0000 677b  ..G.z..).r,...g{
+00000780: 14ae 47e1 7a84 3f29 02da 0273 70da 0750  ..G.z.?)...sp..P
+00000790: 6f6c 7967 6f6e a900 7213 0000 0072 1200  olygon..r....r..
+000007a0: 0000 da0e 6372 6561 7465 5f70 6f6c 7967  ....create_polyg
+000007b0: 6f6e 7a14 526f 626f 742e 6372 6561 7465  onz.Robot.create
+000007c0: 5f70 6f6c 7967 6f6e 2300 0000 7312 0000  _polygon#...s...
+000007d0: 0080 00e4 0f11 8f7a 897a d21a 73d3 0f74  .......z.z..s..t
+000007e0: d008 7472 1300 0000 da07 6465 6c74 615f  ..tr......delta_
+000007f0: 7463 0200 0000 0000 0000 0000 0000 0500  tc..............
+00000800: 0000 0300 0000 f388 0100 0097 007c 006a  .............|.j
+00000810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000820: 0000 0064 017a 0000 0074 0300 0000 0000  ...d.z...t......
+00000830: 0000 006a 0200 0000 0000 0000 0000 0000  ...j............
+00000840: 0000 0000 0000 00ab 0000 0000 0000 006b  ...............k
+00000850: 0200 0072 527c 006a 0500 0000 0000 0000  ...rR|.j........
+00000860: 0000 0000 0000 0000 0000 00ab 0000 0000  ................
+00000870: 0000 007d 0274 0300 0000 0000 0000 006a  ...}.t.........j
+00000880: 0200 0000 0000 0000 0000 0000 0000 0000  ................
+00000890: 0000 00ab 0000 0000 0000 007c 005f 0000  ...........|._..
+000008a0: 0000 0000 0000 0064 027c 0264 0319 0000  .......d.|.d....
+000008b0: 0076 0072 227c 0264 0319 0000 0064 0219  .v.r"|.d.....d..
+000008c0: 0000 0072 1a7c 006a 0700 0000 0000 0000  ...r.|.j........
+000008d0: 0000 0000 0000 0000 0000 007c 0264 0319  ...........|.d..
+000008e0: 0000 0064 0219 0000 0064 0419 0000 00ab  ...d.....d......
+000008f0: 0100 0000 0000 0001 007c 006a 0800 0000  .........|.j....
+00000900: 0000 0000 0000 0000 0000 0000 0000 0073  ...............s
+00000910: 2e7c 006a 0700 0000 0000 0000 0000 0000  .|.j............
+00000920: 0000 0000 0000 0074 0b00 0000 0000 0000  .......t........
+00000930: 006a 0c00 0000 0000 0000 0000 0000 0000  .j..............
+00000940: 0000 0000 007c 006a 0e00 0000 0000 0000  .....|.j........
+00000950: 0000 0000 0000 0000 0000 00ab 0100 0000  ................
+00000960: 0000 00ab 0100 0000 0000 0001 007c 006a  .............|.j
+00000970: 1100 0000 0000 0000 0000 0000 0000 0000  ................
+00000980: 0000 007c 01ac 05ab 0100 0000 0000 0001  ...|............
+00000990: 0079 0029 064e 7203 0000 00da 0470 7265  .y.).Nr......pre
+000009a0: 79da 0c61 6765 6e74 5f73 7461 7465 7372  y..agent_statesr
+000009b0: 0200 0000 2901 7231 0000 0029 0972 1000  ....).r1...).r..
+000009c0: 0000 da04 7469 6d65 da0f 6765 745f 6f62  ....time..get_ob
+000009d0: 7365 7276 6174 696f 6eda 0f73 6574 5f64  servation..set_d
+000009e0: 6573 7469 6e61 7469 6f6e da04 7061 7468  estination..path
+000009f0: 7217 0000 0072 1800 0000 720a 0000 00da  r....r....r.....
+00000a00: 086e 6176 6967 6174 6529 0372 1100 0000  .navigate).r....
+00000a10: 7231 0000 00da 0b6f 6273 6572 7661 7469  r1.....observati
+00000a20: 6f6e 7303 0000 0020 2020 7212 0000 00da  ons....   r.....
+00000a30: 0473 7465 707a 0a52 6f62 6f74 2e73 7465  .stepz.Robot.ste
+00000a40: 7027 0000 0073 a000 0000 8000 d80b 0fd7  p'...s..........
+00000a50: 0b25 d10b 25a8 01d1 0b29 ac44 af49 a949  .%..%....).D.I.I
+00000a60: ab4b d20b 37d8 1a1e d71a 2ed1 1a2e d31a  .K..7...........
+00000a70: 3088 4bdc 292d af19 a919 ab1b 8844 d40c  0.K.)-.......D..
+00000a80: 26d8 0f15 981b a05e d119 34d1 0f34 b81b  &......^..4..4..
+00000a90: c05e d139 54d0 555b d239 5cd8 1014 d710  .^.9T.U[.9\.....
+00000aa0: 24d1 1024 a05b b01e d125 40c0 16d1 2548  $..$.[...%@...%H
+00000ab0: c811 d125 4bd4 104c e00f 138f 798a 79d8  ...%K..L....y.y.
+00000ac0: 0c10 d70c 20d1 0c20 a416 a71d a11d a874  .... .. .......t
+00000ad0: d72f 42d1 2f42 d321 43d4 0c44 e008 0c8f  ./B./B.!C..D....
+00000ae0: 0d89 0d98 6788 0dd5 0826 7213 0000 004e  ....g....&r....N
+00000af0: 2912 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+00000b00: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+00000b10: 6e61 6d65 5f5f da06 7479 7069 6e67 da04  name__..typing..
+00000b20: 4c69 7374 da05 5475 706c 65da 0566 6c6f  List..Tuple..flo
+00000b30: 6174 7204 0000 0072 0f00 0000 7216 0000  atr....r....r...
+00000b40: 00da 0c73 7461 7469 636d 6574 686f 6472  ...staticmethodr
+00000b50: 1e00 0000 da07 5375 7266 6163 6572 2600  ......Surfacer&.
+00000b60: 0000 722d 0000 0072 2e00 0000 7230 0000  ..r-...r....r0..
+00000b70: 0072 3b00 0000 722f 0000 0072 1300 0000  .r;...r/...r....
+00000b80: 7212 0000 0072 0800 0000 7208 0000 000b  r....r....r.....
+00000b90: 0000 0073 9f00 0000 8400 f002 0a05 27d8  ...s..........'.
+00000ba0: 2228 a72b a12b a866 af6c a96c b835 c025  "(.+.+.f.l.l.5.%
+00000bb0: b83c d12e 48d1 2249 f003 0a05 27e0 2127  .<..H."I....'.!'
+00000bc0: a71b a11b a856 af5c a95c b825 c015 b82c  .....V.\.\.%...,
+00000bd0: d12d 47d1 2148 f005 0a05 27f0 0600 1e28  .-G.!H....'....(
+00000be0: f307 0a05 27f2 1803 0523 f00a 0006 12f0  ....'....#......
+00000bf0: 0203 051e 9836 9f3e 993e f200 0305 1ef3  .....6.>.>......
+00000c00: 0300 0612 f002 0305 1ef0 0a00 0612 f002  ................
+00000c10: 0105 7501 9842 9f4a 994a f200 0105 7501  ..u..B.J.J....u.
+00000c20: f303 0006 12f0 0201 0575 01f0 060a 0527  .........u.....'
+00000c30: 9845 f400 0a05 2772 1300 0000 7208 0000  .E....'r....r...
+00000c40: 0029 0d72 1700 0000 723f 0000 0072 1e00  .).r....r?...r..
+00000c50: 0000 720b 0000 0072 0400 0000 da10 6e61  ..r....r......na
+00000c60: 7669 6761 7469 6f6e 5f61 6765 6e74 7205  vigation_agentr.
+00000c70: 0000 00da 0972 6573 6f75 7263 6573 7206  .....resourcesr.
+00000c80: 0000 00da 0773 6861 7065 6c79 722d 0000  .....shapelyr-..
+00000c90: 0072 3500 0000 7208 0000 0072 2f00 0000  .r5...r....r/...
+00000ca0: 7213 0000 0072 1200 0000 fa08 3c6d 6f64  r....r......<mod
+00000cb0: 756c 653e 7248 0000 0001 0000 0073 2900  ule>rH.......s).
+00000cc0: 0000 f003 0101 01db 000d db00 0ddb 000d  ................
+00000cd0: dd00 22dd 002d dd00 20db 0014 db00 0bf4  .."..-.. .......
+00000ce0: 0626 0127 884f f500 2601 2772 1300 0000  .&.'.O..&.'r....
```

### Comparing `cellworld_game-0.0.61/cellworld_game/__pycache__/util.cpython-312.pyc` & `cellworld_game-0.0.68/cellworld_game/__pycache__/util.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Tue Apr 23 16:14:29 2024 UTC, .py size: 7912 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 65de 2766 e81e 0000  ........e.'f....
+00000000: cb0d 0d0a 0000 0000 cdda 1166 f61d 0000  ...........f....
 00000010: e300 0000 0000 0000 0000 0000 000d 0000  ................
 00000020: 0000 0000 00f3 8601 0000 9700 6400 6401  ............d.d.
 00000030: 6c00 5a00 6400 6401 6c01 5a01 6400 6401  l.Z.d.d.l.Z.d.d.
 00000040: 6c02 5a03 6400 6401 6c04 5a04 6402 6501  l.Z.d.d.l.Z.d.e.
 00000050: 6a0a 0000 0000 0000 0000 0000 0000 0000  j...............
 00000060: 0000 0000 6506 6506 6602 1900 0000 6403  ....e.e.f.....d.
 00000070: 6501 6a0a 0000 0000 0000 0000 0000 0000  e.j.............
@@ -30,15 +30,15 @@
 000001d0: 0000 0000 0004 0000 0003 0000 00f3 3c00  ..............<.
 000001e0: 0000 9700 7c01 6401 1900 0000 7c00 6401  ....|.d.....|.d.
 000001f0: 1900 0000 7a0a 0000 6402 7a08 0000 7c01  ....z...d.z...|.
 00000200: 6403 1900 0000 7c00 6403 1900 0000 7a0a  d.....|.d.....z.
 00000210: 0000 6402 7a08 0000 7a00 0000 5300 a904  ..d.z...z...S...
 00000220: 4e72 0200 0000 e902 0000 00e9 0100 0000  Nr..............
 00000230: a900 2902 7203 0000 0072 0400 0000 7302  ..).r....r....s.
-00000240: 0000 0020 20fa 3143 3a5c 5265 7365 6172  ...  .1C:\Resear
+00000240: 0000 0020 20fa 3143 3a5c 7265 7365 6172  ...  .1C:\resear
 00000250: 6368 5c63 656c 6c77 6f72 6c64 5f67 616d  ch\cellworld_gam
 00000260: 655c 6365 6c6c 776f 726c 645f 6761 6d65  e\cellworld_game
 00000270: 5c75 7469 6c2e 7079 da09 6469 7374 616e  \util.py..distan
 00000280: 6365 3272 0b00 0000 0700 0000 7331 0000  ce2r........s1..
 00000290: 0080 00e0 0c12 9031 8949 9806 9871 9909  .......1.I...q..
 000002a0: d10c 21a0 61d1 0b27 a836 b021 a939 b076  ..!.a..'.6.!.9.v
 000002b0: b861 b179 d12b 40c0 51d1 2a46 d10b 46d0  .a.y.+@.Q.*F..F.
@@ -564,44 +564,44 @@
 00002330: 0000 7d02 7c02 6403 6b02 0000 7205 7c02  ..}.|.d.k...r.|.
 00002340: 6402 7a0d 0000 7d02 7c02 5300 2904 4e72  d.z...}.|.S.).Nr
 00002350: 8300 0000 7282 0000 0072 8100 0000 2901  ....r....r....).
 00002360: 7284 0000 0029 0372 8500 0000 7286 0000  r....).r....r...
 00002370: 00da 0a64 6966 6665 7265 6e63 6573 0300  ...differences..
 00002380: 0000 2020 2072 0a00 0000 da14 6469 7265  ..   r......dire
 00002390: 6374 696f 6e5f 6469 6666 6572 656e 6365  ction_difference
-000023a0: 7289 0000 00e3 0000 0073 4a00 0000 8000  r........sJ.....
+000023a0: 7289 0000 00e1 0000 0073 4a00 0000 8000  r........sJ.....
 000023b0: dc11 24a0 5ad3 1130 804a dc11 24a0 5ad3  ..$.Z..0.J..$.Z.
 000023c0: 1130 804a d811 1b98 6ad1 1128 804a d807  .0.J....j..(.J..
 000023d0: 1190 43d2 0717 d808 1290 63d1 0819 880a  ..C.......c.....
 000023e0: d807 1190 44d2 0718 d808 1290 63d1 0819  ....D.......c...
 000023f0: 880a d80b 15d0 0415 720c 0000 00da 0f64  ........r......d
 00002400: 6972 6563 7469 6f6e 5f65 7272 6f72 6301  irection_errorc.
 00002410: 0000 0000 0000 0000 0000 0003 0000 0003  ................
 00002420: 0000 00f3 2200 0000 9700 7c00 6401 7a0b  ....".....|.d.z.
 00002430: 0000 7d01 6402 7c01 7c01 7a05 0000 6402  ..}.d.|.|.z...d.
-00002440: 7a00 0000 7a0b 0000 5300 2903 4ee9 0800  z...z...S.).N...
+00002440: 7a00 0000 7a0b 0000 5300 2903 4e72 0700  z...z...S.).Nr..
 00002450: 0000 7208 0000 0072 0900 0000 2902 728a  ..r....r....).r.
 00002460: 0000 00da 0670 695f 6572 7273 0200 0000  .....pi_errs....
 00002470: 2020 720a 0000 00da 1d64 6972 6563 7469    r......directi
 00002480: 6f6e 5f65 7272 6f72 5f6e 6f72 6d61 6c69  on_error_normali
-00002490: 7a61 7469 6f6e 728e 0000 00ee 0000 0073  zationr........s
+00002490: 7a61 7469 6f6e 728d 0000 00ec 0000 0073  zationr........s
 000024a0: 2000 0000 8000 d80d 1c98 71d1 0d20 8046   .........q.. .F
 000024b0: d80b 0c90 0698 1691 0fa0 21d1 1023 d10b  ..........!..#..
 000024c0: 24d0 0424 720c 0000 0029 024e 4e29 1972  $..$r....).NN).r
 000024d0: 2900 0000 da06 7479 7069 6e67 da07 7368  ).....typing..sh
 000024e0: 6170 656c 7972 2d00 0000 7215 0000 00da  apelyr-...r.....
 000024f0: 0554 7570 6c65 da05 666c 6f61 7472 0b00  .Tuple..floatr..
 00002500: 0000 7220 0000 0072 1700 0000 722f 0000  ..r ...r....r/..
 00002510: 0072 3900 0000 7244 0000 0072 4800 0000  .r9...rD...rH...
 00002520: 7252 0000 0072 6f00 0000 da09 6974 6572  rR...ro.....iter
 00002530: 746f 6f6c 7372 7000 0000 7273 0000 0072  toolsrp...rs...r
 00002540: 7700 0000 723b 0000 0072 3c00 0000 7284  w...r;...r<...r.
-00002550: 0000 0072 8900 0000 728e 0000 0072 0900  ...r....r....r..
+00002550: 0000 0072 8900 0000 728d 0000 0072 0900  ...r....r....r..
 00002560: 0000 720c 0000 0072 0a00 0000 fa08 3c6d  ..r....r......<m
-00002570: 6f64 756c 653e 7294 0000 0001 0000 0073  odule>r........s
+00002570: 6f64 756c 653e 7293 0000 0001 0000 0073  odule>r........s
 00002580: 5001 0000 f003 0101 01db 000b db00 0ddb  P...............
 00002590: 0014 db00 0ff0 0602 0147 0190 6697 6c91  .........G..f.l.
 000025a0: 6ca0 35a8 25a0 3cd1 1630 f000 0201 4701  l.5.%.<..0....G.
 000025b0: d816 1c97 6c91 6ca0 35a8 25a0 3cd1 1630  ....l.l.5.%.<..0
 000025c0: f303 0201 4701 f20a 1401 12f0 2e1a 0113  ....G...........
 000025d0: 9835 f000 1a01 13a8 45f0 001a 0113 b825  .5......E......%
 000025e0: f000 1a01 13c0 42c7 4ac1 4af3 001a 0113  ......B.J.J.....
@@ -613,10 +613,10 @@
 00002640: 5a02 f000 004e 025a 02f1 0000 4102 5b02  Z....N.Z....A.[.
 00002650: f300 0601 30f0 1203 0141 0198 669f 6c99  ....0....A..f.l.
 00002660: 6ca8 35b0 25a8 3cd1 1e38 f000 0301 4101  l.5.%.<..8....A.
 00002670: c055 f000 0301 4101 d056 5bf3 0003 0141  .U....A..V[....A
 00002680: 01f2 0c11 0117 f228 4801 0145 01f5 5602  .......(H..E..V.
 00002690: 0001 23f2 0619 0118 f238 0301 28f2 0c01  ..#......8..(...
 000026a0: 0142 01f2 0801 0146 01f0 0805 0115 a035  .B.....F.......5
-000026b0: f300 0501 15f0 1008 0116 a055 f000 0801  ...........U....
+000026b0: f300 0501 15f0 0c08 0116 a055 f000 0801  ...........U....
 000026c0: 16b8 05f3 0008 0116 f016 0201 25b0 35f4  ............%.5.
 000026d0: 0002 0125 720c 0000 00                   ...%r....
```

### Comparing `cellworld_game-0.0.61/cellworld_game/__pycache__/visibility.cpython-312.pyc` & `cellworld_game-0.0.68/cellworld_game/__pycache__/visibility.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Thu Apr 11 19:37:32 2024 UTC, .py size: 9497 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 fc3b 1866 1925 0000  .........;.f.%..
+00000000: cb0d 0d0a 0000 0000 983a 1d66 4924 0000  .........:.fI$..
 00000010: e300 0000 0000 0000 0000 0000 0004 0000  ................
 00000020: 0000 0000 00f3 5c00 0000 9700 6400 6401  ......\.....d.d.
 00000030: 6c00 5a00 6400 6401 6c01 5a01 6400 6401  l.Z.d.d.l.Z.d.d.
 00000040: 6c02 5a02 6400 6401 6c03 5a04 6402 6403  l.Z.d.d.l.Z.d.d.
 00000050: 6c05 6d06 5a06 6d07 5a07 0100 6402 6404  l.m.Z.m.Z...d.d.
 00000060: 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b 0100  l.m.Z.m.Z.m.Z...
 00000070: 0200 4700 6405 8400 6406 ab02 0000 0000  ..G.d...d.......
@@ -69,15 +69,15 @@
 00000440: 7274 6963 6573 da08 6578 7465 7269 6f72  rtices..exterior
 00000450: da06 636f 6f72 6473 da02 7370 da05 506f  ..coords..sp..Po
 00000460: 696e 74da 036d 6178 da08 6469 7374 616e  int..max..distan
 00000470: 6365 da0c 6d61 785f 6469 7374 616e 6365  ce..max_distance
 00000480: 2907 da04 7365 6c66 720b 0000 0072 0c00  )...selfr....r..
 00000490: 0000 da01 63da 0e61 7265 6e61 5f76 6572  ....c..arena_ver
 000004a0: 7469 6365 73da 0276 31da 0276 3273 0700  tices..v1..v2s..
-000004b0: 0000 2020 2020 2020 20fa 3743 3a5c 5265  ..       .7C:\Re
+000004b0: 0000 2020 2020 2020 20fa 3743 3a5c 7265  ..       .7C:\re
 000004c0: 7365 6172 6368 5c63 656c 6c77 6f72 6c64  search\cellworld
 000004d0: 5f67 616d 655c 6365 6c6c 776f 726c 645f  _game\cellworld_
 000004e0: 6761 6d65 5c76 6973 6962 696c 6974 792e  game\visibility.
 000004f0: 7079 da08 5f5f 696e 6974 5f5f 7a13 5669  py..__init__z.Vi
 00000500: 7369 6269 6c69 7479 2e5f 5f69 6e69 745f  sibility.__init_
 00000510: 5f0a 0000 0073 8b00 0000 8000 dc4f 60d0  _....s.......O`.
 00000520: 616b d06f 74d0 6e75 d161 75d3 4f76 d108  ak.ot.nu.au.Ov..
```

### Comparing `cellworld_game-0.0.61/cellworld_game/agent.py` & `cellworld_game-0.0.68/cellworld_game/agent.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,178 +1,178 @@
-import math
-import typing
-import pygame
-import shapely as sp
-from .resources import Resources
-from .util import create_hexagon, move_point, distance
-from shapely.affinity import rotate, translate
-
-
-class CoordinateConverter(object):
-    def __init__(self,
-                 screen_size: typing.Tuple[int, int],
-                 flip_y: bool = False):
-        self.screen_size = screen_size
-        self.screen_width, self.screen_height = screen_size
-        self.flip_y = flip_y
-        self.screen_offset = (self.screen_width - self.screen_height) / 2
-        self.hexa_ratio = (math.sqrt(3) / 2)
-
-    def from_canonical(self, canonical: typing.Union[tuple, float]):
-        if isinstance(canonical, float):
-            return canonical * self.screen_width
-
-        canonical_x, canonical_y = canonical
-        screen_x = canonical_x * self.screen_width
-        if self.flip_y:
-            screen_y = (1-canonical_y) * self.screen_width - self.screen_offset
-        else:
-            screen_y = canonical_y * self.screen_width - self.screen_offset
-        return screen_x, screen_y
-
-    def to_canonical(self, screen: typing.Union[tuple, float]):
-        if isinstance(screen, float):
-            return screen / self.screen_width
-
-        screen_x, screen_y = screen
-        y = self.screen_height - screen_y + self.screen_offset
-        canonical_y = y / self.screen_height * self.hexa_ratio
-        canonical_x = screen_x / self.screen_width
-        return canonical_x, canonical_y
-
-
-class AgentState(object):
-    def __init__(self, location: typing.Tuple[float, float] = (0, 0), direction: float = 0):
-        self.location = location
-        self.direction = direction
-
-    def __iter__(self):
-        yield self.location
-        yield self.direction
-
-    def update(self,
-               distance: float,
-               rotation: float) -> "AgentState":
-        new_direction = self.direction + rotation
-        return AgentState(location=move_point(start=self.location,
-                                              direction=new_direction,
-                                              distance=distance),
-                          direction=new_direction)
-
-
-class AgentDynamics(object):
-    def __init__(self, forward_speed: float, turn_speed: float):
-        self.forward_speed = forward_speed
-        self.turn_speed = turn_speed
-
-    def __iter__(self):
-        yield self.forward_speed
-        yield self.turn_speed
-
-    def change(self, delta_t: float) -> tuple:
-        return self.forward_speed * delta_t,  self.turn_speed * delta_t
-
-
-class Agent(object):
-
-    def __init__(self,
-                 view_field: float = 180,
-                 collision: bool = True):
-        self.visible = True
-        self.view_field = view_field
-        self._state: AgentState = AgentState()
-        self.dynamics: AgentDynamics = AgentDynamics(forward_speed=0,
-                                                     turn_speed=0)
-        self.polygon = self.create_polygon()
-        self.sprite = None
-        self.collision = collision
-        self.on_reset = None
-        self.on_step = None
-        self.on_start = None
-        self.name = ""
-        self.model = None
-        self.trajectory: typing.List[AgentState] = []
-        self.coordinate_converter: typing.Optional[CoordinateConverter] = None
-        self.running = False
-
-    def set_sprite_size(self, size: tuple):
-        self.sprite = pygame.transform.scale(self.create_sprite(), size)
-
-    def set_state(self, state: AgentState) -> None:
-        self.trajectory.append(state)
-        self._state = state
-
-    @property
-    def state(self) -> AgentState:
-        return self._state
-
-    def reset(self) -> None:
-        self.trajectory.clear()
-        if self.on_reset:
-            self.on_reset()
-        self.running = True
-
-    def start(self) -> None:
-        if self.on_start:
-            self.on_start()
-
-    def step(self, delta_t: float) -> None:
-        if self.on_step:
-            self.on_step(delta_t)
-
-    @staticmethod
-    def create_sprite() -> pygame.Surface:
-        sprite = pygame.image.load(Resources.file("agent.png"))
-        rotated_sprite = pygame.transform.rotate(sprite, 90)
-        return rotated_sprite
-
-    @staticmethod
-    def create_polygon() -> sp.Polygon:
-        return create_hexagon((0, 0), .05, 30)
-
-    def get_polygon(self,
-                    state: AgentState = None) -> sp.Polygon:
-        # Rotate and then translate the arrow polygon
-        if state:
-            x, y = state.location
-            direction = state.direction
-        else:
-            x, y = self._state.location
-            direction = self._state.direction
-        rotated_polygon = rotate(self.polygon,
-                                 direction,
-                                 origin=(0, 0),
-                                 use_radians=False)
-        translated_polygon = translate(rotated_polygon, x, y)
-        return translated_polygon
-
-    def get_sprite(self) -> pygame.Surface:
-        rotated_sprite = pygame.transform.rotate(self.sprite, self._state.direction)
-        return rotated_sprite
-
-    def get_observation(self) -> dict:
-        if self.model:
-            return self.model.get_observation(agent_name=self.name)
-        else:
-            return None
-
-    def get_stats(self) -> dict:
-        stats = {}
-        dist = 0
-        prev_state = self.trajectory[0]
-        for state in self.trajectory[1:]:
-            dist += distance(prev_state.location, state.location)
-            prev_state = state
-        stats["distance"] = dist
-        return stats
-
-    def draw(self,
-             surface: pygame.Surface,
-             coordinate_converter: CoordinateConverter):
-        agent_sprite: pygame.Surface = self.get_sprite()
-        width, height = agent_sprite.get_size()
-        screen_x, screen_y = coordinate_converter.from_canonical(self.state.location)
-        surface.blit(agent_sprite, (screen_x - width / 2, screen_y - height / 2))
-
-    def set_coordinate_converter(self,
-                                 coordinate_converter: CoordinateConverter):
-        self.coordinate_converter = coordinate_converter
+import math
+import typing
+import pygame
+import shapely as sp
+from .resources import Resources
+from .util import create_hexagon, move_point, distance
+from shapely.affinity import rotate, translate
+
+
+class CoordinateConverter(object):
+    def __init__(self,
+                 screen_size: typing.Tuple[int, int],
+                 flip_y: bool = False):
+        self.screen_size = screen_size
+        self.screen_width, self.screen_height = screen_size
+        self.flip_y = flip_y
+        self.screen_offset = (self.screen_width - self.screen_height) / 2
+        self.hexa_ratio = (math.sqrt(3) / 2)
+
+    def from_canonical(self, canonical: typing.Union[tuple, float]):
+        if isinstance(canonical, float):
+            return canonical * self.screen_width
+
+        canonical_x, canonical_y = canonical
+        screen_x = canonical_x * self.screen_width
+        if self.flip_y:
+            screen_y = (1-canonical_y) * self.screen_width - self.screen_offset
+        else:
+            screen_y = canonical_y * self.screen_width - self.screen_offset
+        return screen_x, screen_y
+
+    def to_canonical(self, screen: typing.Union[tuple, float]):
+        if isinstance(screen, float):
+            return screen / self.screen_width
+
+        screen_x, screen_y = screen
+        y = self.screen_height - screen_y + self.screen_offset
+        canonical_y = y / self.screen_height * self.hexa_ratio
+        canonical_x = screen_x / self.screen_width
+        return canonical_x, canonical_y
+
+
+class AgentState(object):
+    def __init__(self, location: typing.Tuple[float, float] = (0, 0), direction: float = 0):
+        self.location = location
+        self.direction = direction
+
+    def __iter__(self):
+        yield self.location
+        yield self.direction
+
+    def update(self,
+               distance: float,
+               rotation: float) -> "AgentState":
+        new_direction = self.direction + rotation
+        return AgentState(location=move_point(start=self.location,
+                                              direction=new_direction,
+                                              distance=distance),
+                          direction=new_direction)
+
+
+class AgentDynamics(object):
+    def __init__(self, forward_speed: float, turn_speed: float):
+        self.forward_speed = forward_speed
+        self.turn_speed = turn_speed
+
+    def __iter__(self):
+        yield self.forward_speed
+        yield self.turn_speed
+
+    def change(self, delta_t: float) -> tuple:
+        return self.forward_speed * delta_t,  self.turn_speed * delta_t
+
+
+class Agent(object):
+
+    def __init__(self,
+                 view_field: float = 180,
+                 collision: bool = True):
+        self.visible = True
+        self.view_field = view_field
+        self._state: AgentState = AgentState()
+        self.dynamics: AgentDynamics = AgentDynamics(forward_speed=0,
+                                                     turn_speed=0)
+        self.polygon = self.create_polygon()
+        self.sprite = None
+        self.collision = collision
+        self.on_reset = None
+        self.on_step = None
+        self.on_start = None
+        self.name = ""
+        self.model = None
+        self.trajectory: typing.List[AgentState] = []
+        self.coordinate_converter: typing.Optional[CoordinateConverter] = None
+        self.running = False
+
+    def set_sprite_size(self, size: tuple):
+        self.sprite = pygame.transform.scale(self.create_sprite(), size)
+
+    def set_state(self, state: AgentState) -> None:
+        self.trajectory.append(state)
+        self._state = state
+
+    @property
+    def state(self) -> AgentState:
+        return self._state
+
+    def reset(self) -> None:
+        self.trajectory.clear()
+        if self.on_reset:
+            self.on_reset()
+        self.running = True
+
+    def start(self) -> None:
+        if self.on_start:
+            self.on_start()
+
+    def step(self, delta_t: float) -> None:
+        if self.on_step:
+            self.on_step(delta_t)
+
+    @staticmethod
+    def create_sprite() -> pygame.Surface:
+        sprite = pygame.image.load(Resources.file("agent.png"))
+        rotated_sprite = pygame.transform.rotate(sprite, 90)
+        return rotated_sprite
+
+    @staticmethod
+    def create_polygon() -> sp.Polygon:
+        return create_hexagon((0, 0), .05, 30)
+
+    def get_polygon(self,
+                    state: AgentState = None) -> sp.Polygon:
+        # Rotate and then translate the arrow polygon
+        if state:
+            x, y = state.location
+            direction = state.direction
+        else:
+            x, y = self._state.location
+            direction = self._state.direction
+        rotated_polygon = rotate(self.polygon,
+                                 direction,
+                                 origin=(0, 0),
+                                 use_radians=False)
+        translated_polygon = translate(rotated_polygon, x, y)
+        return translated_polygon
+
+    def get_sprite(self) -> pygame.Surface:
+        rotated_sprite = pygame.transform.rotate(self.sprite, self._state.direction)
+        return rotated_sprite
+
+    def get_observation(self) -> dict:
+        if self.model:
+            return self.model.get_observation(agent_name=self.name)
+        else:
+            return None
+
+    def get_stats(self) -> dict:
+        stats = {}
+        dist = 0
+        prev_state = self.trajectory[0]
+        for state in self.trajectory[1:]:
+            dist += distance(prev_state.location, state.location)
+            prev_state = state
+        stats["distance"] = dist
+        return stats
+
+    def draw(self,
+             surface: pygame.Surface,
+             coordinate_converter: CoordinateConverter):
+        agent_sprite: pygame.Surface = self.get_sprite()
+        width, height = agent_sprite.get_size()
+        screen_x, screen_y = coordinate_converter.from_canonical(self.state.location)
+        surface.blit(agent_sprite, (screen_x - width / 2, screen_y - height / 2))
+
+    def set_coordinate_converter(self,
+                                 coordinate_converter: CoordinateConverter):
+        self.coordinate_converter = coordinate_converter
```

### Comparing `cellworld_game-0.0.61/cellworld_game/cellworld_loader.py` & `cellworld_game-0.0.68/cellworld_game/cellworld_loader.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-import typing
-import cellworld as cw
-from .util import create_hexagon
-from .navigation import Navigation
-
-
-class CellWorldLoader:
-    def __init__(self,
-                 world_name: str):
-        self.world = cw.World.get_from_parameters_names(world_configuration_name="hexagonal",
-                                                        world_implementation_name="canonical",
-                                                        occlusions_name=world_name)
-        paths_builder = cw.Paths_builder.get_from_name(world_configuration_name="hexagonal",
-                                                       occlusions_name=world_name)
-        paths = cw.Paths(builder=paths_builder, world=self.world)
-        cellmap = cw.Cell_map(self.world.configuration.cell_coordinates)
-
-        self.locations: typing.List[typing.Optional[typing.Tuple[float, float]]] = [None
-                                                                                    if c.occluded
-                                                                                    else tuple(c.location.get_values())
-                                                                                    for c in self.world.cells]
-
-        locations_paths: typing.List[typing.List[typing.Optional[int]]] = [[None for _ in range(len(self.world.cells))]
-                                                                            for _ in range(len(self.world.cells))]
-        for src_cell in self.world.cells:
-            for dst_cell in self.world.cells:
-                move = paths.get_move(src_cell=src_cell, dst_cell=dst_cell)
-                next_step_id = cellmap[src_cell.coordinates + move]
-                locations_paths[src_cell.id][dst_cell.id] = next_step_id
-        self.paths = locations_paths
-        self.open_locations = [tuple(c.location.get_values()) for c in self.world.cells.free_cells()]
-        arena_center = self.world.implementation.space.center.get_values()
-        arena_transformation: cw.Transformation = self.world.implementation.space.transformation
-        cell_transformation: cw.Transformation = self.world.implementation.cell_transformation
-        self.arena = create_hexagon(arena_center, arena_transformation.size, arena_transformation.rotation)
-        self.occlusions = [create_hexagon(cell.location.get_values(),
-                                          cell_transformation.size,
-                                          arena_transformation.rotation + cell_transformation.rotation)
-                           for cell
-                           in self.world.cells.occluded_cells()]
-        spawn_cells = cw.Cell_group_builder.get_from_name("hexagonal",
-                                                          world_name,
-                                                          "spawn_locations")
-        self.robot_start_locations = [tuple(self.world.cells[sc].location.get_values()) for sc in spawn_cells]
-        self.full_action_list = self.open_locations
-
-        try:
-            lppo_cells = cw.Cell_group_builder.get_from_name("hexagonal",
-                                                             world_name,
-                                                             "lppo")
-
-            self.tlppo_action_list = [tuple(self.world.cells[sc].location.get_values()) for sc in lppo_cells]
-        except :
-            self.tlppo_action_list = []
-
-        cell_visibility = cw.get_resource("graph", "hexagonal", world_name, "cell_visibility")
-
-        self.navigation = Navigation(locations=self.locations,
-                                     paths=self.paths,
-                                     visibility=cell_visibility)
+import typing
+import cellworld as cw
+from .util import create_hexagon
+from .navigation import Navigation
+
+
+class CellWorldLoader:
+    def __init__(self,
+                 world_name: str):
+        self.world = cw.World.get_from_parameters_names(world_configuration_name="hexagonal",
+                                                        world_implementation_name="canonical",
+                                                        occlusions_name=world_name)
+        paths_builder = cw.Paths_builder.get_from_name(world_configuration_name="hexagonal",
+                                                       occlusions_name=world_name)
+        paths = cw.Paths(builder=paths_builder, world=self.world)
+        cellmap = cw.Cell_map(self.world.configuration.cell_coordinates)
+
+        self.locations: typing.List[typing.Optional[typing.Tuple[float, float]]] = [None
+                                                                                    if c.occluded
+                                                                                    else tuple(c.location.get_values())
+                                                                                    for c in self.world.cells]
+
+        locations_paths: typing.List[typing.List[typing.Optional[int]]] = [[None for _ in range(len(self.world.cells))]
+                                                                            for _ in range(len(self.world.cells))]
+        for src_cell in self.world.cells:
+            for dst_cell in self.world.cells:
+                move = paths.get_move(src_cell=src_cell, dst_cell=dst_cell)
+                next_step_id = cellmap[src_cell.coordinates + move]
+                locations_paths[src_cell.id][dst_cell.id] = next_step_id
+        self.paths = locations_paths
+        self.open_locations = [tuple(c.location.get_values()) for c in self.world.cells.free_cells()]
+        arena_center = self.world.implementation.space.center.get_values()
+        arena_transformation: cw.Transformation = self.world.implementation.space.transformation
+        cell_transformation: cw.Transformation = self.world.implementation.cell_transformation
+        self.arena = create_hexagon(arena_center, arena_transformation.size, arena_transformation.rotation)
+        self.occlusions = [create_hexagon(cell.location.get_values(),
+                                          cell_transformation.size,
+                                          arena_transformation.rotation + cell_transformation.rotation)
+                           for cell
+                           in self.world.cells.occluded_cells()]
+        spawn_cells = cw.Cell_group_builder.get_from_name("hexagonal",
+                                                          world_name,
+                                                          "spawn_locations")
+        self.robot_start_locations = [tuple(self.world.cells[sc].location.get_values()) for sc in spawn_cells]
+        self.full_action_list = self.open_locations
+
+        try:
+            lppo_cells = cw.Cell_group_builder.get_from_name("hexagonal",
+                                                             world_name,
+                                                             "lppo")
+
+            self.tlppo_action_list = [tuple(self.world.cells[sc].location.get_values()) for sc in lppo_cells]
+        except :
+            self.tlppo_action_list = []
+
+        cell_visibility = cw.get_resource("graph", "hexagonal", world_name, "cell_visibility")
+
+        self.navigation = Navigation(locations=self.locations,
+                                     paths=self.paths,
+                                     visibility=cell_visibility)
```

### Comparing `cellworld_game-0.0.61/cellworld_game/files/agent.png` & `cellworld_game-0.0.68/cellworld_game/files/agent.png`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.61/cellworld_game/files/predator.png` & `cellworld_game-0.0.68/cellworld_game/files/predator.png`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.61/cellworld_game/files/prey.png` & `cellworld_game-0.0.68/cellworld_game/files/prey.png`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.61/cellworld_game/license.txt` & `cellworld_game-0.0.68/cellworld_game/license.txt`

 * *Files identical despite different names*

### Comparing `cellworld_game-0.0.61/cellworld_game/model.py` & `cellworld_game-0.0.68/cellworld_game/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,182 +1,197 @@
-import math
-import time
-import typing
-import shapely as sp
-from .agent import Agent, AgentState
-from .visibility import Visibility
-from .geometry import atan2
-
-
-class Model(object):
-
-    def __init__(self,
-                 arena,
-                 occlusions,
-                 real_time: bool = False,
-                 time_step: float = 0.1):
-        self.arena = arena
-        self.occlusions = occlusions
-        self.real_time = real_time
-        self.time_step = time_step
-        self.agents: typing.Dict[str, Agent] = {}
-        self.visibility = Visibility(arena=self.arena, occlusions=self.occlusions)
-        self.last_step = None
-        self.time = 0
-        self.running = False
-        self.step_count = 0
-        self.before_step = None
-        self.after_step = None
-        self.before_reset = None
-        self.after_reset = None
-        self.before_close = None
-        self.after_close = None
-
-    def set_agents_state(self, agents_state: typing.Dict[str, AgentState],
-                         delta_t: float = 0):
-        for agent_name, agent_state in agents_state.items():
-            if agent_name in self.agents:
-                self.agents[agent_name].set_state(agent_state)
-        self.__update_state__(delta_t)
-
-    def __update_state__(self,
-                         delta_t: float = 0):
-        pass
-
-    def add_agent(self, name: str, agent: Agent):
-        self.agents[name] = agent
-        agent.name = name
-        agent.model = self
-
-    def reset(self):
-        if self.before_reset is not None:
-            self.before_reset.reset()
-        self.running = True
-        for name, agent in self.agents.items():
-            agent.reset()
-        observations = self.get_observations()
-        for name, agent in self.agents.items():
-            agent.start()
-        self.last_step = time.time()
-        self.step_count = 0
-        if self.after_reset is not None:
-            self.after_reset()
-
-    def is_valid_state(self, agent_polygon: sp.Polygon, collisions: bool) -> bool:
-        if not self.arena.contains(agent_polygon):
-            return False
-        if collisions:
-            for occlusion in self.occlusions:
-                if agent_polygon.intersects(occlusion):
-                    return False
-        return True
-
-    def wall_direction(self, src: typing.Tuple[float, float], wall_number: int):
-        return math.degrees(atan2(sp.Point(src), self.visibility.walls_centroids[wall_number]))
-
-    def get_observations(self):
-        agent_visibility = {src_name: {dst_name: None for dst_name in self.agents} for src_name in self.agents}
-        observations = {}
-        for src_name, src_agent in self.agents.items():
-            observations[src_name] = {}
-            src_point = sp.Point(src_agent.state.location)
-            walls_by_distance = self.visibility.walls_by_distance(src=src_point)
-            parsed_walls = []
-            for wall_number, vertices, distance in walls_by_distance:
-                parsed_walls.append((distance, self.wall_direction(src=src_point, wall_number=wall_number)))
-            observations[src_name]["walls"] = parsed_walls
-            for dst_name, dst_agent in self.agents.items():
-                if agent_visibility[src_name][dst_name] is None:
-                    if src_name == dst_name:
-                        is_visible = True
-                    else:
-                        dst_point = sp.Point(dst_agent.state.location)
-                        is_visible = self.visibility.line_of_sight(src=src_point,
-                                                                   dst=dst_point,
-                                                                   walls_by_distance=walls_by_distance)
-                    agent_visibility[src_name][dst_name] = is_visible
-                    agent_visibility[dst_name][src_name] = is_visible
-            observations[src_name]["agent_states"] = {}
-            for dst_name, is_visible in agent_visibility.items():
-                if is_visible:
-                    observations[src_name]["agent_states"][dst_name] = self.agents[dst_name].state.location, self.agents[dst_name].state.direction
-                else:
-                    observations[src_name]["agent_states"][dst_name] = None
-        return observations
-
-    def get_observation(self,
-                        agent_name: str,
-                        polygonal: bool = False) -> dict:
-        observation = {}
-        src_point = sp.Point(self.agents[agent_name].state.location)
-        if polygonal:
-            visibility_polygon = self.visibility.get_visibility_polygon(src_point.state.location, src_point.state.direction)
-        else:
-            walls_by_distance = self.visibility.walls_by_distance(src=src_point)
-        parsed_walls = []
-        for wall_number, vertices, distance in walls_by_distance:
-            parsed_walls.append((distance, self.wall_direction(src=src_point, wall_number=wall_number)))
-        observation["walls"] = parsed_walls
-        observation["agent_states"] = {}
-        for dst_name, dst_agent in self.agents.items():
-            if agent_name == dst_name:
-                is_visible = True
-            else:
-                dst_point = sp.Point(dst_agent.state.location)
-                if polygonal:
-                    dst_polygon = dst_agent.get_polygon()
-                    is_visible = dst_polygon.intersects(visibility_polygon)
-                else:
-                    is_visible = self.visibility.line_of_sight(src=src_point,
-                                                               dst=dst_point,
-                                                               walls_by_distance=walls_by_distance)
-            if is_visible:
-                observation["agent_states"][dst_name] = self.agents[dst_name].state.location, self.agents[dst_name].state.direction
-            else:
-                observation["agent_states"][dst_name] = None
-        return observation
-
-    def step(self) -> float:
-        if self.before_step is not None:
-            self.before_step()
-
-        if self.real_time:
-            while self.last_step + self.time_step > time.time():
-                pass
-
-        self.last_step = time.time()
-        for name, agent in self.agents.items():
-            dynamics = agent.dynamics
-            distance, rotation = dynamics.change(delta_t=self.time_step)
-            new_state = agent.state.update(rotation=rotation,
-                                           distance=distance)
-            agent_polygon = agent.get_polygon(state=new_state)
-            if self.is_valid_state(agent_polygon=agent_polygon,
-                                   collisions=agent.collision):
-                agent.set_state(state=new_state)
-            else: #try only rotation
-                new_state = agent.state.update(rotation=rotation,
-                                               distance=0)
-                agent_polygon = agent.get_polygon(state=new_state)
-                if self.is_valid_state(agent_polygon=agent_polygon,
-                                       collisions=agent.collision):
-                    agent.set_state(state=new_state)
-                else: #try only translation
-                    new_state = agent.state.update(rotation=0,
-                                                   distance=distance)
-                    agent_polygon = agent.get_polygon(state=new_state)
-                    if self.is_valid_state(agent_polygon=agent_polygon,
-                                           collisions=agent.collision):
-                        agent.set_state(state=new_state)
-        for name, agent in self.agents.items():
-            agent.step(delta_t=self.time_step)
-        self.time += self.time_step
-        self.step_count += 1
-        if self.after_step is not None:
-            self.after_step()
-        return self.time_step
-
-    def close(self):
-        if self.before_close:
-            self.before_close()
-        if self.after_close:
-            self.after_close()
+import math
+import time
+import typing
+import shapely as sp
+from .agent import Agent, AgentState
+from .visibility import Visibility
+from .geometry import atan2
+
+
+class Model(object):
+
+    def __init__(self,
+                 arena,
+                 occlusions,
+                 real_time: bool = False,
+                 time_step: float = 0.1):
+        self.arena = arena
+        self.occlusions = occlusions
+        self.real_time = real_time
+        self.time_step = time_step
+        self.agents: typing.Dict[str, Agent] = {}
+        self.visibility = Visibility(arena=self.arena, occlusions=self.occlusions)
+        self.last_step = None
+        self.time = 0
+        self.running = False
+        self.episode_count = 0
+        self.step_count = 0
+        self.before_step = None
+        self.after_step = None
+        self.before_stop = None
+        self.after_stop = None
+        self.before_reset = None
+        self.after_reset = None
+        self.on_close = None
+
+    def set_agents_state(self, agents_state: typing.Dict[str, AgentState],
+                         delta_t: float = 0):
+        for agent_name, agent_state in agents_state.items():
+            if agent_name in self.agents:
+                self.agents[agent_name].set_state(agent_state)
+        self.__update_state__(delta_t)
+
+    def __update_state__(self,
+                         delta_t: float = 0):
+        pass
+
+    def add_agent(self, name: str, agent: Agent):
+        self.agents[name] = agent
+        agent.name = name
+        agent.model = self
+
+    def reset(self):
+        if self.running:
+            self.stop()
+        if self.before_reset is not None:
+            self.before_reset()
+        self.running = True
+        self.episode_count += 1
+        for name, agent in self.agents.items():
+            agent.reset()
+        observations = self.get_observations()
+        for name, agent in self.agents.items():
+            agent.start()
+        self.last_step = time.time()
+        self.step_count = 0
+        if self.after_reset is not None:
+            self.after_reset()
+
+    def stop(self):
+        if self.before_stop is not None:
+            self.before_stop()
+        self.running = False
+        if self.after_stop is not None:
+            self.after_stop()
+
+    def is_valid_state(self, agent_polygon: sp.Polygon, collisions: bool) -> bool:
+        if not self.arena.contains(agent_polygon):
+            return False
+        if collisions:
+            for occlusion in self.occlusions:
+                if agent_polygon.intersects(occlusion):
+                    return False
+        return True
+
+    def wall_direction(self, src: typing.Tuple[float, float], wall_number: int):
+        return math.degrees(atan2(sp.Point(src), self.visibility.walls_centroids[wall_number]))
+
+    def get_observations(self):
+        agent_visibility = {src_name: {dst_name: None for dst_name in self.agents} for src_name in self.agents}
+        observations = {}
+        for src_name, src_agent in self.agents.items():
+            observations[src_name] = {}
+            src_point = sp.Point(src_agent.state.location)
+            walls_by_distance = self.visibility.walls_by_distance(src=src_point)
+            parsed_walls = []
+            for wall_number, vertices, distance in walls_by_distance:
+                parsed_walls.append((distance, self.wall_direction(src=src_point, wall_number=wall_number)))
+            observations[src_name]["walls"] = parsed_walls
+            for dst_name, dst_agent in self.agents.items():
+                if agent_visibility[src_name][dst_name] is None:
+                    if src_name == dst_name:
+                        is_visible = True
+                    else:
+                        dst_point = sp.Point(dst_agent.state.location)
+                        is_visible = self.visibility.line_of_sight(src=src_point,
+                                                                   dst=dst_point,
+                                                                   walls_by_distance=walls_by_distance)
+                    agent_visibility[src_name][dst_name] = is_visible
+                    agent_visibility[dst_name][src_name] = is_visible
+            observations[src_name]["agent_states"] = {}
+            for dst_name, is_visible in agent_visibility.items():
+                if is_visible:
+                    observations[src_name]["agent_states"][dst_name] = self.agents[dst_name].state.location, self.agents[dst_name].state.direction
+                else:
+                    observations[src_name]["agent_states"][dst_name] = None
+        return observations
+
+    def get_observation(self,
+                        agent_name: str,
+                        polygonal: bool = False) -> dict:
+        observation = {}
+        src_point = sp.Point(self.agents[agent_name].state.location)
+        if polygonal:
+            visibility_polygon = self.visibility.get_visibility_polygon(src_point.state.location, src_point.state.direction)
+        else:
+            walls_by_distance = self.visibility.walls_by_distance(src=src_point)
+        parsed_walls = []
+        for wall_number, vertices, distance in walls_by_distance:
+            parsed_walls.append((distance, self.wall_direction(src=src_point, wall_number=wall_number)))
+        observation["walls"] = parsed_walls
+        observation["agent_states"] = {}
+        for dst_name, dst_agent in self.agents.items():
+            if agent_name == dst_name:
+                is_visible = True
+            else:
+                dst_point = sp.Point(dst_agent.state.location)
+                if polygonal:
+                    dst_polygon = dst_agent.get_polygon()
+                    is_visible = dst_polygon.intersects(visibility_polygon)
+                else:
+                    is_visible = self.visibility.line_of_sight(src=src_point,
+                                                               dst=dst_point,
+                                                               walls_by_distance=walls_by_distance)
+            if is_visible:
+                observation["agent_states"][dst_name] = self.agents[dst_name].state.location, self.agents[dst_name].state.direction
+            else:
+                observation["agent_states"][dst_name] = None
+        return observation
+
+    def step(self) -> float:
+        if not self.running:
+            return 0
+
+        if self.before_step is not None:
+            self.before_step()
+
+        if self.real_time:
+            while self.last_step + self.time_step > time.time():
+                pass
+
+        self.last_step = time.time()
+        for name, agent in self.agents.items():
+            dynamics = agent.dynamics
+            distance, rotation = dynamics.change(delta_t=self.time_step)
+            new_state = agent.state.update(rotation=rotation,
+                                           distance=distance)
+            agent_polygon = agent.get_polygon(state=new_state)
+            if self.is_valid_state(agent_polygon=agent_polygon,
+                                   collisions=agent.collision):
+                agent.set_state(state=new_state)
+            else: #try only rotation
+                new_state = agent.state.update(rotation=rotation,
+                                               distance=0)
+                agent_polygon = agent.get_polygon(state=new_state)
+                if self.is_valid_state(agent_polygon=agent_polygon,
+                                       collisions=agent.collision):
+                    agent.set_state(state=new_state)
+                else: #try only translation
+                    new_state = agent.state.update(rotation=0,
+                                                   distance=distance)
+                    agent_polygon = agent.get_polygon(state=new_state)
+                    if self.is_valid_state(agent_polygon=agent_polygon,
+                                           collisions=agent.collision):
+                        agent.set_state(state=new_state)
+        for name, agent in self.agents.items():
+            agent.step(delta_t=self.time_step)
+        self.time += self.time_step
+        self.step_count += 1
+        if self.after_step is not None:
+            self.after_step()
+        return self.time_step
+
+    def close(self):
+        if self.running:
+            self.stop()
+        if self.on_close:
+            self.on_close()
```

### Comparing `cellworld_game-0.0.61/cellworld_game/mouse.py` & `cellworld_game-0.0.68/cellworld_game/mouse.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-import typing
-import pygame
-from .agent import AgentState
-from .navigation import Navigation
-from .navigation_agent import NavigationAgent
-from .resources import Resources
-import shapely as sp
-
-
-class Mouse(NavigationAgent):
-    def __init__(self,
-                 start_state: AgentState,
-                 navigation: Navigation):
-        NavigationAgent.__init__(self,
-                                 navigation=navigation,
-                                 max_forward_speed=0.5,
-                                 max_turning_speed=20.0)
-        self.start_state = start_state
-
-    def reset(self):
-        NavigationAgent.reset(self)
-        self.set_state(AgentState(location=self.start_state.location,
-                                  direction=self.start_state.direction))
-
-    @staticmethod
-    def create_sprite() -> pygame.Surface:
-        sprite = pygame.image.load(Resources.file("prey.png"))
-        rotated_sprite = pygame.transform.rotate(sprite, 270)
-        return rotated_sprite
-
-    @staticmethod
-    def create_polygon() -> sp.Polygon:
-        return sp.Polygon([(.015, 0), (0, 0.005), (-.015, 0), (0, -0.005)])
-
+import typing
+import pygame
+from .agent import AgentState
+from .navigation import Navigation
+from .navigation_agent import NavigationAgent
+from .resources import Resources
+import shapely as sp
+
+
+class Mouse(NavigationAgent):
+    def __init__(self,
+                 start_state: AgentState,
+                 navigation: Navigation):
+        NavigationAgent.__init__(self,
+                                 navigation=navigation,
+                                 max_forward_speed=0.5,
+                                 max_turning_speed=20.0)
+        self.start_state = start_state
+
+    def reset(self):
+        NavigationAgent.reset(self)
+        self.set_state(AgentState(location=self.start_state.location,
+                                  direction=self.start_state.direction))
+
+    @staticmethod
+    def create_sprite() -> pygame.Surface:
+        sprite = pygame.image.load(Resources.file("prey.png"))
+        rotated_sprite = pygame.transform.rotate(sprite, 270)
+        return rotated_sprite
+
+    @staticmethod
+    def create_polygon() -> sp.Polygon:
+        return sp.Polygon([(.015, 0), (0, 0.005), (-.015, 0), (0, -0.005)])
+
```

### Comparing `cellworld_game-0.0.61/cellworld_game/navigation.py` & `cellworld_game-0.0.68/cellworld_game/navigation.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-import math
-import typing
-
-
-class Navigation:
-    def __init__(self,
-                 locations: typing.List[typing.Optional[typing.Tuple[float, float]]],
-                 paths: typing.List[typing.List[int]],
-                 visibility: typing.List[typing.List[typing.List[int]]]):
-        self.locations = locations
-        self.paths = paths
-        self.visibility = visibility
-
-    def closest_location(self,
-                         location: typing.Tuple[float, float]) -> int:
-        min_dist2 = math.inf
-        closest = None
-        for i, l in enumerate(self.locations):
-            if l is None:
-                continue
-            dist2 = (l[0] - location[0]) ** 2 + (l[1] - location[1]) ** 2
-            if dist2 < min_dist2:
-                closest = i
-                min_dist2 = dist2
-        return closest
-
-    def get_path(self,
-                 src: typing.Tuple[float, float],
-                 dst: typing.Tuple[float, float]) -> typing.List[typing.Tuple[float, float]]:
-        src_index = self.closest_location(location=src)
-        dst_index = self.closest_location(location=dst)
-        current = src_index
-        last_step = src_index
-        path_indexes = []
-        while current is not None and current != dst_index:
-            next_step = self.paths[current][dst_index]
-            if next_step == current:
-                break
-            is_visible = next_step in self.visibility[last_step]
-            if not is_visible:
-                path_indexes.append(current)
-                last_step = current
-            current = next_step
-        path_indexes.append(dst_index)
-        return [self.locations[s] for s in path_indexes]
+import math
+import typing
+
+
+class Navigation:
+    def __init__(self,
+                 locations: typing.List[typing.Optional[typing.Tuple[float, float]]],
+                 paths: typing.List[typing.List[int]],
+                 visibility: typing.List[typing.List[typing.List[int]]]):
+        self.locations = locations
+        self.paths = paths
+        self.visibility = visibility
+
+    def closest_location(self,
+                         location: typing.Tuple[float, float]) -> int:
+        min_dist2 = math.inf
+        closest = None
+        for i, l in enumerate(self.locations):
+            if l is None:
+                continue
+            dist2 = (l[0] - location[0]) ** 2 + (l[1] - location[1]) ** 2
+            if dist2 < min_dist2:
+                closest = i
+                min_dist2 = dist2
+        return closest
+
+    def get_path(self,
+                 src: typing.Tuple[float, float],
+                 dst: typing.Tuple[float, float]) -> typing.List[typing.Tuple[float, float]]:
+        src_index = self.closest_location(location=src)
+        dst_index = self.closest_location(location=dst)
+        current = src_index
+        last_step = src_index
+        path_indexes = []
+        while current is not None and current != dst_index:
+            next_step = self.paths[current][dst_index]
+            if next_step == current:
+                break
+            is_visible = next_step in self.visibility[last_step]
+            if not is_visible:
+                path_indexes.append(current)
+                last_step = current
+            current = next_step
+        path_indexes.append(dst_index)
+        return [self.locations[s] for s in path_indexes]
```

### Comparing `cellworld_game-0.0.61/cellworld_game/navigation_agent.py` & `cellworld_game-0.0.68/cellworld_game/navigation_agent.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-import pygame
-from .util import distance, direction, direction_difference, direction_error_normalization
-from .agent import Agent, CoordinateConverter
-from .navigation import Navigation
-
-
-class NavigationAgent(Agent):
-
-    def __init__(self,
-                 navigation: Navigation,
-                 max_forward_speed: float,
-                 max_turning_speed: float,
-                 threshold: float = 0.01,
-                 destination_update_rate: int = 10):
-        self.max_forward_speed = max_forward_speed
-        self.max_turning_speed = max_turning_speed
-        self.threshold = threshold
-        self.destination_update_rate = destination_update_rate
-        self.navigation = navigation
-        self.new_destination = None
-        self.destination = None
-        self.navigation_plan_update_wait = 0
-        self.destination_wait = 0
-        self.path = []
-        Agent.__init__(self)
-        self.collision = False
-
-    def next_step(self):
-        if self.path:
-            return self.path[0]
-        return None
-
-    def set_destination(self, destination):
-        self.new_destination = destination
-
-    def reset(self):
-        self.destination = None
-        self.path = []
-        Agent.reset(self)
-
-    def start(self):
-        Agent.start(self)
-
-    def step(self, delta_t: float):
-        if not self.running:
-            self.stop_navigation()
-            return
-
-        if self.new_destination and self.destination_wait == 0:
-            self.destination = self.new_destination
-            self.new_destination = None
-            self.destination_wait = self.destination_update_rate
-            self.navigation_plan_update_wait = self.destination_update_rate
-            self.path = self.navigation.get_path(src=self.state.location, dst=self.destination)
-
-        if self.destination and self.navigation_plan_update_wait == 0:
-            self.path = self.navigation.get_path(src=self.state.location, dst=self.destination)
-
-        if self.destination_wait:
-            self.destination_wait -= 1
-
-        if self.navigation_plan_update_wait:
-            self.navigation_plan_update_wait -= 1
-
-        if self.next_step() is not None:
-            distance_error = distance(src=self.state.location,
-                                      dst=self.next_step())
-            if distance_error < self.threshold:
-                self.path.pop(0)
-
-        if self.next_step():
-            distance_error = distance(src=self.state.location,
-                                      dst=self.next_step())
-
-            normalized_distance_error = max(distance_error/.2, 1)
-
-            destination_direction = direction(src=self.state.location,
-                                              dst=self.next_step())
-            direction_error = direction_difference(direction1=self.state.direction,
-                                                   direction2=destination_direction)
-            normalized_direction_error = direction_error_normalization(direction_error=direction_error)
-
-            self.dynamics.forward_speed = self.max_forward_speed * normalized_direction_error * normalized_distance_error
-            self.dynamics.turn_speed = self.max_turning_speed * direction_error
-        else:
-            self.dynamics.forward_speed = 0
-            self.dynamics.turn_speed = 0
-
-    def draw(self,
-             surface: pygame.Surface,
-             coordinate_converter: CoordinateConverter):
-        current_point = self.state.location
-        for step in self.path:
-            if step is None:
-                continue
-            pygame.draw.line(surface,
-                             (255, 0, 0),
-                             coordinate_converter.from_canonical(current_point),
-                             coordinate_converter.from_canonical(step),
-                             2)
-            pygame.draw.circle(surface=surface,
-                               color=(0, 0, 255),
-                               center=coordinate_converter.from_canonical(step),
-                               radius=5,
-                               width=2)
-            current_point = step
-        Agent.draw(self=self,
-                   surface=surface,
-                   coordinate_converter=coordinate_converter)
-
-    def stop_navigation(self):
-        self.dynamics.forward_speed = 0
-        self.dynamics.turn_speed = 0
+import pygame
+from .util import distance, direction, direction_difference, direction_error_normalization
+from .agent import Agent, CoordinateConverter
+from .navigation import Navigation
+
+
+class NavigationAgent(Agent):
+
+    def __init__(self,
+                 navigation: Navigation,
+                 max_forward_speed: float,
+                 max_turning_speed: float,
+                 threshold: float = 0.01,
+                 destination_update_rate: int = 10):
+        self.max_forward_speed = max_forward_speed
+        self.max_turning_speed = max_turning_speed
+        self.threshold = threshold
+        self.destination_update_rate = destination_update_rate
+        self.navigation = navigation
+        self.new_destination = None
+        self.destination = None
+        self.navigation_plan_update_wait = 0
+        self.destination_wait = 0
+        self.path = []
+        Agent.__init__(self)
+        self.collision = False
+
+    def next_step(self):
+        if self.path:
+            return self.path[0]
+        return None
+
+    def set_destination(self, destination):
+        self.new_destination = destination
+
+    def reset(self):
+        self.destination = None
+        self.path = []
+        Agent.reset(self)
+
+    def start(self):
+        Agent.start(self)
+
+    def step(self, delta_t: float):
+        if not self.running:
+            self.stop_navigation()
+            return
+
+        if self.new_destination and self.destination_wait == 0:
+            self.destination = self.new_destination
+            self.new_destination = None
+            self.destination_wait = self.destination_update_rate
+            self.navigation_plan_update_wait = self.destination_update_rate
+            self.path = self.navigation.get_path(src=self.state.location, dst=self.destination)
+
+        if self.destination and self.navigation_plan_update_wait == 0:
+            self.path = self.navigation.get_path(src=self.state.location, dst=self.destination)
+
+        if self.destination_wait:
+            self.destination_wait -= 1
+
+        if self.navigation_plan_update_wait:
+            self.navigation_plan_update_wait -= 1
+
+        if self.next_step() is not None:
+            distance_error = distance(src=self.state.location,
+                                      dst=self.next_step())
+            if distance_error < self.threshold:
+                self.path.pop(0)
+
+        if self.next_step():
+            distance_error = distance(src=self.state.location,
+                                      dst=self.next_step())
+
+            normalized_distance_error = max(distance_error/.2, 1)
+
+            destination_direction = direction(src=self.state.location,
+                                              dst=self.next_step())
+            direction_error = direction_difference(direction1=self.state.direction,
+                                                   direction2=destination_direction)
+            normalized_direction_error = direction_error_normalization(direction_error=direction_error)
+
+            self.dynamics.forward_speed = self.max_forward_speed * normalized_direction_error * normalized_distance_error
+            self.dynamics.turn_speed = self.max_turning_speed * direction_error
+        else:
+            self.dynamics.forward_speed = 0
+            self.dynamics.turn_speed = 0
+
+    def draw(self,
+             surface: pygame.Surface,
+             coordinate_converter: CoordinateConverter):
+        current_point = self.state.location
+        for step in self.path:
+            if step is None:
+                continue
+            pygame.draw.line(surface,
+                             (255, 0, 0),
+                             coordinate_converter.from_canonical(current_point),
+                             coordinate_converter.from_canonical(step),
+                             2)
+            pygame.draw.circle(surface=surface,
+                               color=(0, 0, 255),
+                               center=coordinate_converter.from_canonical(step),
+                               radius=5,
+                               width=2)
+            current_point = step
+        Agent.draw(self=self,
+                   surface=surface,
+                   coordinate_converter=coordinate_converter)
+
+    def stop_navigation(self):
+        self.dynamics.forward_speed = 0
+        self.dynamics.turn_speed = 0
```

### Comparing `cellworld_game-0.0.61/cellworld_game/ray_tracing.py` & `cellworld_game-0.0.68/cellworld_game/ray_tracing.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-import pygame
-import math
-import typing
-import shapely as sp
-from .model import Model
-from .agent import AgentState
-from .util import create_line_string
-
-
-class RayTracing:
-    def __init__(self, model: Model,
-                 horizontal_view_field: float = 270.0,
-                 vertical_view_field: float = 90,
-                 perspective_height: float = .025,
-                 resolution: int = 1):
-        self.model = model
-        self.vertical_view_field = vertical_view_field
-        self.horizontal_view_field = horizontal_view_field
-        self.perspective_height = perspective_height
-        self.resolution = resolution
-        self.walls = sp.geometry.LineString(model.arena.exterior)
-        self.occlusions = [sp.geometry.LineString(occlusion.exterior) for occlusion in model.occlusions]
-        self.ray_length = 1.0
-        self.occlusion_color: typing.Tuple[int, int, int] = (255, 255, 255)
-        self.occlusion_height: float = 0.1
-        self.wall_color: typing.Tuple[int, int, int] = (255, 200, 200)
-        self.wall_height: float = 0.5
-
-    def distance_factor(self, distance: float) -> float:
-        return (self.ray_length - distance) / self.ray_length
-
-    def line_limits(self, perspective_height, line_bottom, line_top, distance, view_field_offset) -> typing.Tuple[float, float]:
-        bottom_angle = self.vertical_view_field / 2 + math.degrees(math.atan2(perspective_height, distance))
-        top_angle = self.vertical_view_field / 2 - math.degrees(math.atan2(line_top-perspective_height, distance))
-        return bottom_angle / self.vertical_view_field, top_angle / self.vertical_view_field
-
-    def render_line(self, screen, screen_x, distance, view_field_offset: float, color, height):
-        screen_width, screen_height = screen.get_size()
-        distance_factor = self.distance_factor(distance=distance)
-        line_color = tuple(channel * distance_factor for channel in color)
-        line_start, line_end = self.line_limits(self.perspective_height,
-                                                0,
-                                                height,
-                                                distance,
-                                                view_field_offset)
-        y_start = screen_height * line_start
-        y_ends = screen_height * line_end
-        pygame.draw.line(surface=screen,
-                         color=line_color,
-                         start_pos=(screen_x, y_start),
-                         end_pos=(screen_x, y_ends),
-                         width=self.resolution)
-
-    def render(self, perspective: AgentState, screen: pygame.Surface):
-        screen_width, screen_height = screen.get_size()
-        start_angle = perspective.direction - self.horizontal_view_field / 2
-        step_angle = self.horizontal_view_field / screen_width
-        start = sp.Point(perspective.location)
-        screen.fill((0, 0, 0))
-        sorted_occlusions = sorted(self.occlusions, key=lambda line: line.distance(start))
-        for x in range(0, screen_width, self.resolution):
-            view_angle = step_angle * x
-            view_field_offset = view_angle - self.horizontal_view_field / 2
-            ray_direction = start_angle + view_angle
-            screen_x = screen_width - x - 1
-            ray = create_line_string(start=perspective.location,
-                                     direction=ray_direction,
-                                     distance=self.ray_length)
-            wall_intersection = ray.intersection(self.walls)
-            wall_distance = wall_intersection.distance(start)
-            self.render_line(screen=screen,
-                             screen_x=screen_x,
-                             color=self.wall_color,
-                             height=self.wall_height,
-                             distance=wall_distance,
-                             view_field_offset=view_field_offset)
-            closest_distance = wall_distance
-            occluded = False
-            for occlusion in sorted_occlusions:
-                intersection = ray.intersection(occlusion)
-                if intersection:
-                    for intersection_point in intersection.geoms:
-                        distance = intersection_point.distance(start)
-                        if distance < closest_distance:
-                            closest_distance = distance
-                            occluded = True
-                    if occluded:
-                        break
-            if occluded:
-                self.render_line(screen=screen,
-                                 screen_x=screen_x,
-                                 color=self.occlusion_color,
-                                 height=self.occlusion_height,
-                                 distance=closest_distance,
-                                 view_field_offset=view_field_offset)
-
-        pygame.display.flip()
+import pygame
+import math
+import typing
+import shapely as sp
+from .model import Model
+from .agent import AgentState
+from .util import create_line_string
+
+
+class RayTracing:
+    def __init__(self, model: Model,
+                 horizontal_view_field: float = 270.0,
+                 vertical_view_field: float = 90,
+                 perspective_height: float = .025,
+                 resolution: int = 1):
+        self.model = model
+        self.vertical_view_field = vertical_view_field
+        self.horizontal_view_field = horizontal_view_field
+        self.perspective_height = perspective_height
+        self.resolution = resolution
+        self.walls = sp.geometry.LineString(model.arena.exterior)
+        self.occlusions = [sp.geometry.LineString(occlusion.exterior) for occlusion in model.occlusions]
+        self.ray_length = 1.0
+        self.occlusion_color: typing.Tuple[int, int, int] = (255, 255, 255)
+        self.occlusion_height: float = 0.1
+        self.wall_color: typing.Tuple[int, int, int] = (255, 200, 200)
+        self.wall_height: float = 0.5
+
+    def distance_factor(self, distance: float) -> float:
+        return (self.ray_length - distance) / self.ray_length
+
+    def line_limits(self, perspective_height, line_bottom, line_top, distance, view_field_offset) -> typing.Tuple[float, float]:
+        bottom_angle = self.vertical_view_field / 2 + math.degrees(math.atan2(perspective_height, distance))
+        top_angle = self.vertical_view_field / 2 - math.degrees(math.atan2(line_top-perspective_height, distance))
+        return bottom_angle / self.vertical_view_field, top_angle / self.vertical_view_field
+
+    def render_line(self, screen, screen_x, distance, view_field_offset: float, color, height):
+        screen_width, screen_height = screen.get_size()
+        distance_factor = self.distance_factor(distance=distance)
+        line_color = tuple(channel * distance_factor for channel in color)
+        line_start, line_end = self.line_limits(self.perspective_height,
+                                                0,
+                                                height,
+                                                distance,
+                                                view_field_offset)
+        y_start = screen_height * line_start
+        y_ends = screen_height * line_end
+        pygame.draw.line(surface=screen,
+                         color=line_color,
+                         start_pos=(screen_x, y_start),
+                         end_pos=(screen_x, y_ends),
+                         width=self.resolution)
+
+    def render(self, perspective: AgentState, screen: pygame.Surface):
+        screen_width, screen_height = screen.get_size()
+        start_angle = perspective.direction - self.horizontal_view_field / 2
+        step_angle = self.horizontal_view_field / screen_width
+        start = sp.Point(perspective.location)
+        screen.fill((0, 0, 0))
+        sorted_occlusions = sorted(self.occlusions, key=lambda line: line.distance(start))
+        for x in range(0, screen_width, self.resolution):
+            view_angle = step_angle * x
+            view_field_offset = view_angle - self.horizontal_view_field / 2
+            ray_direction = start_angle + view_angle
+            screen_x = screen_width - x - 1
+            ray = create_line_string(start=perspective.location,
+                                     direction=ray_direction,
+                                     distance=self.ray_length)
+            wall_intersection = ray.intersection(self.walls)
+            wall_distance = wall_intersection.distance(start)
+            self.render_line(screen=screen,
+                             screen_x=screen_x,
+                             color=self.wall_color,
+                             height=self.wall_height,
+                             distance=wall_distance,
+                             view_field_offset=view_field_offset)
+            closest_distance = wall_distance
+            occluded = False
+            for occlusion in sorted_occlusions:
+                intersection = ray.intersection(occlusion)
+                if intersection:
+                    for intersection_point in intersection.geoms:
+                        distance = intersection_point.distance(start)
+                        if distance < closest_distance:
+                            closest_distance = distance
+                            occluded = True
+                    if occluded:
+                        break
+            if occluded:
+                self.render_line(screen=screen,
+                                 screen_x=screen_x,
+                                 color=self.occlusion_color,
+                                 height=self.occlusion_height,
+                                 distance=closest_distance,
+                                 view_field_offset=view_field_offset)
+
+        pygame.display.flip()
```

### Comparing `cellworld_game-0.0.61/cellworld_game/robot.py` & `cellworld_game-0.0.68/cellworld_game/robot.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-import shapely as sp
-import random
-import typing
-import pygame
-from .agent import AgentState
-from .navigation import Navigation
-from .navigation_agent import NavigationAgent
-from .resources import Resources
-
-
-class Robot(NavigationAgent):
-    def __init__(self,
-                 start_locations: typing.List[typing.Tuple[float, float]],
-                 open_locations: typing.List[typing.Tuple[float, float]],
-                 navigation: Navigation):
-        NavigationAgent.__init__(self,
-                                 navigation=navigation,
-                                 max_forward_speed=0.075,
-                                 max_turning_speed=3.5)
-        self.start_locations = start_locations
-        self.open_locations = open_locations
-        self.last_destination_time = 0
-
-    def reset(self):
-        NavigationAgent.reset(self)
-        self.set_state(AgentState(location=random.choice(self.start_locations),
-                                  direction=180))
-
-    @staticmethod
-    def create_sprite() -> pygame.Surface:
-        sprite = pygame.image.load(Resources.file("predator.png"))
-        rotated_sprite = pygame.transform.rotate(sprite, 270)
-        return rotated_sprite
-
-    @staticmethod
-    def create_polygon() -> sp.Polygon:
-        return sp.Polygon([(.02, 0.013), (-.02, 0.013), (-.02, -0.013), (.02, -0.013), (.025, -0.01), (.025, 0.01)])
-
-    def step(self, delta_t: float):
-        NavigationAgent.step(self=self,
-                             delta_t=delta_t)
+import shapely as sp
+import random
+import typing
+import pygame
+from .agent import AgentState
+from .navigation import Navigation
+from .navigation_agent import NavigationAgent
+from .resources import Resources
+
+
+class Robot(NavigationAgent):
+    def __init__(self,
+                 start_locations: typing.List[typing.Tuple[float, float]],
+                 open_locations: typing.List[typing.Tuple[float, float]],
+                 navigation: Navigation):
+        NavigationAgent.__init__(self,
+                                 navigation=navigation,
+                                 max_forward_speed=0.075,
+                                 max_turning_speed=3.5)
+        self.start_locations = start_locations
+        self.open_locations = open_locations
+        self.last_destination_time = 0
+
+    def reset(self):
+        NavigationAgent.reset(self)
+        self.set_state(AgentState(location=random.choice(self.start_locations),
+                                  direction=180))
+
+    @staticmethod
+    def create_sprite() -> pygame.Surface:
+        sprite = pygame.image.load(Resources.file("predator.png"))
+        rotated_sprite = pygame.transform.rotate(sprite, 270)
+        return rotated_sprite
+
+    @staticmethod
+    def create_polygon() -> sp.Polygon:
+        return sp.Polygon([(.02, 0.013), (-.02, 0.013), (-.02, -0.013), (.02, -0.013), (.025, -0.01), (.025, 0.01)])
+
+    def step(self, delta_t: float):
+        NavigationAgent.step(self=self,
+                             delta_t=delta_t)
```

### Comparing `cellworld_game-0.0.61/cellworld_game/tasks/__pycache__/botevade.cpython-312.pyc` & `cellworld_game-0.0.68/cellworld_game/__pycache__/environment.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Fri Apr 26 16:50:49 2024 UTC, .py size: 5299 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 25% similar despite different names*

```diff
@@ -1,427 +1,561 @@
-00000000: cb0d 0d0a 0000 0000 69db 2b66 b314 0000  ........i.+f....
+00000000: cb0d 0d0a 0000 0000 4482 1d66 ca14 0000  ........D..f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
-00000020: 0000 0000 00f3 6e00 0000 9700 6400 6401  ......n.....d.d.
-00000030: 6c00 5a00 6402 6403 6c01 6d02 5a02 0100  l.Z.d.d.l.m.Z...
-00000040: 6402 6404 6c03 6d04 5a04 0100 6402 6405  d.d.l.m.Z...d.d.
-00000050: 6c05 6d06 5a06 6d07 5a07 0100 6402 6406  l.m.Z.m.Z...d.d.
-00000060: 6c08 6d09 5a09 0100 6402 6407 6c0a 6d0b  l.m.Z...d.d.l.m.
-00000070: 5a0b 0100 6402 6408 6c0c 6d0d 5a0d 0100  Z...d.d.l.m.Z...
-00000080: 0200 4700 6409 8400 640a 6504 ab03 0000  ..G.d...d.e.....
-00000090: 0000 0000 5a0e 7901 290b e900 0000 004e  ....Z.y.)......N
-000000a0: e902 0000 0029 01da 0864 6973 7461 6e63  .....)...distanc
-000000b0: 6529 01da 054d 6f64 656c 2902 da0a 4167  e)...Model)...Ag
-000000c0: 656e 7453 7461 7465 da13 436f 6f72 6469  entState..Coordi
-000000d0: 6e61 7465 436f 6e76 6572 7465 7229 01da  nateConverter)..
-000000e0: 054d 6f75 7365 2901 da05 526f 626f 7429  .Mouse)...Robot)
-000000f0: 01da 0f43 656c 6c57 6f72 6c64 4c6f 6164  ...CellWorldLoad
-00000100: 6572 6300 0000 0000 0000 0000 0000 0011  erc.............
-00000110: 0000 0000 0000 00f3 7000 0000 9700 6500  ........p.....e.
-00000120: 5a01 6400 5a02 0900 0900 0900 0900 0900  Z.d.Z...........
-00000130: 0900 0900 0900 0900 6411 6401 6503 6402  ........d.d.e.d.
-00000140: 6504 6403 6505 6404 6505 6405 6505 6406  e.d.e.d.e.d.e.d.
-00000150: 6505 6407 6504 6408 6504 6610 6409 8405  e.d.e.d.e.f.d...
-00000160: 5a06 0900 6412 640a 6505 6602 640b 8405  Z...d.d.e.f.d...
-00000170: 5a07 640c 8400 5a08 640d 8400 5a09 640e  Z.d...Z.d...Z.d.
-00000180: 6505 6602 640f 8404 5a0a 7910 2913 da08  e.f.d...Z.y.)...
-00000190: 426f 7445 7661 6465 da0a 776f 726c 645f  BotEvade..world_
-000001a0: 6e61 6d65 da0c 7573 655f 7072 6564 6174  name..use_predat
-000001b0: 6f72 da13 7075 6666 5f63 6f6f 6c5f 646f  or..puff_cool_do
-000001c0: 776e 5f74 696d 65da 0e70 7566 665f 7468  wn_time..puff_th
-000001d0: 7265 7368 6f6c 64da 0e67 6f61 6c5f 7468  reshold..goal_th
-000001e0: 7265 7368 6f6c 64da 0974 696d 655f 7374  reshold..time_st
-000001f0: 6570 da09 7265 616c 5f74 696d 65da 0672  ep..real_time..r
-00000200: 656e 6465 7263 0a00 0000 0000 0000 0000  enderc..........
-00000210: 0000 0700 0000 0300 0000 f3c2 0300 0087  ................
-00000220: 0087 0c97 007c 0289 005f 0000 0000 0000  .....|..._......
-00000230: 0000 007c 0389 005f 0100 0000 0000 0000  ...|..._........
-00000240: 007c 0489 005f 0200 0000 0000 0000 007c  .|..._.........|
-00000250: 0589 005f 0300 0000 0000 0000 007c 0689  ..._.........|..
-00000260: 005f 0400 0000 0000 0000 007c 0989 005f  ._.........|..._
-00000270: 0500 0000 0000 0000 0074 0d00 0000 0000  .........t......
-00000280: 0000 007c 01ac 01ab 0100 0000 0000 0089  ...|............
-00000290: 005f 0700 0000 0000 0000 0074 1100 0000  ._.........t....
-000002a0: 0000 0000 006a 1200 0000 0000 0000 0000  .....j..........
-000002b0: 0000 0000 0000 0000 0089 0089 006a 0e00  .............j..
-000002c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002d0: 006a 1400 0000 0000 0000 0000 0000 0000  .j..............
-000002e0: 0000 0000 0089 006a 0e00 0000 0000 0000  .......j........
-000002f0: 0000 0000 0000 0000 0000 006a 1600 0000  ...........j....
-00000300: 0000 0000 0000 0000 0000 0000 0000 007c  ...............|
-00000310: 077c 08ac 02ab 0500 0000 0000 0001 007c  .|.............|
-00000320: 0272 6b74 1900 0000 0000 0000 0089 006a  .rkt...........j
-00000330: 0e00 0000 0000 0000 0000 0000 0000 0000  ................
-00000340: 0000 006a 1a00 0000 0000 0000 0000 0000  ...j............
-00000350: 0000 0000 0000 0089 006a 0e00 0000 0000  .........j......
-00000360: 0000 0000 0000 0000 0000 0000 006a 1c00  .............j..
-00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000380: 0089 006a 0e00 0000 0000 0000 0000 0000  ...j............
-00000390: 0000 0000 0000 006a 1e00 0000 0000 0000  .......j........
-000003a0: 0000 0000 0000 0000 0000 00ac 03ab 0300  ................
-000003b0: 0000 0000 0089 005f 1000 0000 0000 0000  ......._........
-000003c0: 0089 006a 2300 0000 0000 0000 0000 0000  ...j#...........
-000003d0: 0000 0000 0000 0064 0489 006a 2000 0000  .......d...j ...
-000003e0: 0000 0000 0000 0000 0000 0000 0000 00ab  ................
-000003f0: 0200 0000 0000 0001 0074 2500 0000 0000  .........t%.....
-00000400: 0000 0074 2700 0000 0000 0000 0064 0564  ...t'........d.d
-00000410: 06ac 07ab 0200 0000 0000 0089 006a 0e00  .............j..
-00000420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000430: 006a 1e00 0000 0000 0000 0000 0000 0000  .j..............
-00000440: 0000 0000 00ac 08ab 0200 0000 0000 0089  ................
-00000450: 005f 1400 0000 0000 0000 0089 006a 2300  ._...........j#.
-00000460: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000470: 0064 0989 006a 2800 0000 0000 0000 0000  .d...j(.........
-00000480: 0000 0000 0000 0000 00ab 0200 0000 0000  ................
-00000490: 0001 0064 0a89 005f 1500 0000 0000 0000  ...d..._........
-000004a0: 0089 006a 0a00 0000 0000 0000 0000 0000  ...j............
-000004b0: 0000 0000 0000 0072 6964 0b64 0c6c 166d  .......rid.d.l.m
-000004c0: 177d 0a01 0002 007c 0a89 00ac 0dab 0100  .}.....|........
-000004d0: 0000 0000 0089 005f 1600 0000 0000 0000  ......._........
-000004e0: 0089 006a 3000 0000 0000 0000 0000 0000  ...j0...........
-000004f0: 0000 0000 0000 0089 006a 2c00 0000 0000  .........j,.....
-00000500: 0000 0000 0000 0000 0000 0000 005f 1900  ............._..
-00000510: 0000 0000 0000 007c 0272 3864 0664 006c  .......|.r8d.d.l
-00000520: 1a8a 0c64 0e89 0c6a 3600 0000 0000 0000  ...d...j6.......
-00000530: 0000 0000 0000 0000 0000 0064 0f74 3800  ...........d.t8.
-00000540: 0000 0000 0000 0066 0488 0c88 0066 0264  .......f.....f.d
-00000550: 1084 0c7d 0b89 006a 2c00 0000 0000 0000  ...}...j,.......
-00000560: 0000 0000 0000 0000 0000 006a 3b00 0000  ...........j;...
-00000570: 0000 0000 0000 0000 0000 0000 0000 007c  ...............|
-00000580: 0bab 0100 0000 0000 0001 0064 0a89 005f  ...........d..._
-00000590: 1e00 0000 0000 0000 0064 0689 005f 1f00  .........d..._..
-000005a0: 0000 0000 0000 0064 0a89 005f 2000 0000  .......d..._ ...
-000005b0: 0000 0000 0064 1189 005f 2100 0000 0000  .....d..._!.....
-000005c0: 0000 0064 0689 005f 2200 0000 0000 0000  ...d..._".......
-000005d0: 0064 0689 005f 2300 0000 0000 0000 0079  .d..._#........y
-000005e0: 0029 124e 2901 720d 0000 0029 04da 0561  .).N).r....)...a
-000005f0: 7265 6e61 da0a 6f63 636c 7573 696f 6e73  rena..occlusions
-00000600: 7212 0000 0072 1300 0000 2903 da0f 7374  r....r....)...st
-00000610: 6172 745f 6c6f 6361 7469 6f6e 73da 0e6f  art_locations..o
-00000620: 7065 6e5f 6c6f 6361 7469 6f6e 73da 0a6e  pen_locations..n
-00000630: 6176 6967 6174 696f 6eda 0870 7265 6461  avigation..preda
-00000640: 746f 7229 0267 9a99 9999 9999 a93f e700  tor).g.......?..
-00000650: 0000 0000 00e0 3f72 0200 0000 2902 da08  ......?r....)...
-00000660: 6c6f 6361 7469 6f6e da09 6469 7265 6374  location..direct
-00000670: 696f 6e29 02da 0b73 7461 7274 5f73 7461  ion)...start_sta
-00000680: 7465 721a 0000 00da 0470 7265 7946 7203  ter......preyFr.
-00000690: 0000 0029 01da 0456 6965 7729 01da 056d  ...)...View)...m
-000006a0: 6f64 656c da07 7375 7266 6163 65da 1463  odel..surface..c
-000006b0: 6f6f 7264 696e 6174 655f 636f 6e76 6572  oordinate_conver
-000006c0: 7465 7263 0200 0000 0000 0000 0000 0000  terc............
-000006d0: 0700 0000 1300 0000 f3ca 0100 0095 0297  ................
-000006e0: 007c 016a 0100 0000 0000 0000 0000 0000  .|.j............
-000006f0: 0000 0000 0000 0089 086a 0200 0000 0000  .........j......
-00000700: 0000 0000 0000 0000 0000 0000 006a 0400  .............j..
+00000020: 0000 0000 00f3 9a00 0000 9700 6400 6401  ............d.d.
+00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
+00000040: 5a03 0100 6400 6403 6c04 6d05 5a05 6d06  Z...d.d.l.m.Z.m.
+00000050: 5a06 0100 6400 6404 6c07 6d08 5a08 0100  Z...d.d.l.m.Z...
+00000060: 6400 6405 6c09 6d0a 5a0a 0100 6406 6407  d.d.l.m.Z...d.d.
+00000070: 6c0b 6d0c 5a0c 0100 6406 6408 6c0b 6d0d  l.m.Z...d.d.l.m.
+00000080: 5a0d 0100 6400 6409 6c0e 6d0f 5a0f 0100  Z...d.d.l.m.Z...
+00000090: 6406 640a 6c10 5a11 6400 640b 6c12 6d13  d.d.l.Z.d.d.l.m.
+000000a0: 5a13 0100 6406 640a 6c14 5a14 0200 4700  Z...d.d.l.Z...G.
+000000b0: 640c 8400 640d 650c ab03 0000 0000 0000  d...d.e.........
+000000c0: 5a15 790a 290e e901 0000 0029 01da 054d  Z.y.)......)...M
+000000d0: 6f64 656c 2901 da05 526f 626f 7429 02da  odel)...Robot)..
+000000e0: 054d 6f75 7365 da10 4d6f 7573 654f 6273  .Mouse..MouseObs
+000000f0: 6572 7661 7469 6f6e 2901 da0a 4167 656e  ervation)...Agen
+00000100: 7453 7461 7465 2901 da04 5669 6577 e900  tState)...View..
+00000110: 0000 0029 01da 0345 6e76 2901 da06 7370  ...)...Env)...sp
+00000120: 6163 6573 2901 da0f 4365 6c6c 576f 726c  aces)...CellWorl
+00000130: 644c 6f61 6465 724e 2901 da08 6469 7374  dLoaderN)...dist
+00000140: 616e 6365 6300 0000 0000 0000 0000 0000  ancec...........
+00000150: 000b 0000 0000 0000 00f3 5e00 0000 9700  ..........^.....
+00000160: 6500 5a01 6400 5a02 6401 6402 8400 6403  e.Z.d.Z.d.d...d.
+00000170: 6603 6404 6503 6405 6504 6406 6504 6407  f.d.e.d.e.d.e.d.
+00000180: 6505 6408 6505 660a 6409 8405 5a06 640a  e.d.e.f.d...Z.d.
+00000190: 8400 5a07 640b 6505 6602 640c 8404 5a08  ..Z.d.e.f.d...Z.
+000001a0: 640b 6505 6602 640d 8404 5a09 6411 640f  d.e.f.d...Z.d.d.
+000001b0: 8401 5a0a 6410 8400 5a0b 790e 2912 da0b  ..Z.d...Z.y.)...
+000001c0: 456e 7669 726f 6e6d 656e 74e9 c800 0000  Environment.....
+000001d0: 6301 0000 0000 0000 0000 0000 0000 0000  c...............
+000001e0: 0003 0000 00f3 0400 0000 9700 7901 a902  ............y...
+000001f0: 4e72 0900 0000 a900 2901 da01 7873 0100  Nr......)...xs..
+00000200: 0000 20fa 3843 3a5c 7265 7365 6172 6368  .. .8C:\research
+00000210: 5c63 656c 6c77 6f72 6c64 5f67 616d 655c  \cellworld_game\
+00000220: 6365 6c6c 776f 726c 645f 6761 6d65 5c65  cellworld_game\e
+00000230: 6e76 6972 6f6e 6d65 6e74 2e70 79fa 083c  nvironment.py..<
+00000240: 6c61 6d62 6461 3e7a 1445 6e76 6972 6f6e  lambda>z.Environ
+00000250: 6d65 6e74 2e3c 6c61 6d62 6461 3e14 0000  ment.<lambda>...
+00000260: 0073 0200 0000 8100 f300 0000 00e9 0500  .s..............
+00000270: 0000 da0a 776f 726c 645f 6e61 6d65 da09  ....world_name..
+00000280: 7573 655f 6c70 706f 73da 0c75 7365 5f70  use_lppos..use_p
+00000290: 7265 6461 746f 72da 086d 6178 5f73 7465  redator..max_ste
+000002a0: 70da 0973 7465 705f 7761 6974 6307 0000  p..step_waitc...
+000002b0: 0000 0000 0000 0000 000a 0000 0003 0000  ................
+000002c0: 00f3 ca04 0000 9700 7c04 7c00 5f00 0000  ........|.|._...
+000002d0: 0000 0000 0000 7c05 7c00 5f01 0000 0000  ......|.|._.....
+000002e0: 0000 0000 7c06 7c00 5f02 0000 0000 0000  ....|.|._.......
+000002f0: 0000 7407 0000 0000 0000 0000 7c01 ac01  ..t.........|...
+00000300: ab01 0000 0000 0000 7c00 5f04 0000 0000  ........|._.....
+00000310: 0000 0000 740b 0000 0000 0000 0000 ab00  ....t...........
+00000320: 0000 0000 0000 7c00 5f06 0000 0000 0000  ......|._.......
+00000330: 0000 740f 0000 0000 0000 0000 6a10 0000  ..t.........j...
+00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000350: 7412 0000 0000 0000 0000 6a14 0000 0000  t.........j.....
+00000360: 0000 0000 0000 0000 0000 0000 0000 0b00  ................
+00000370: 7412 0000 0000 0000 0000 6a14 0000 0000  t.........j.....
+00000380: 0000 0000 0000 0000 0000 0000 0000 7417  ..............t.
+00000390: 0000 0000 0000 0000 7c00 6a0c 0000 0000  ........|.j.....
+000003a0: 0000 0000 0000 0000 0000 0000 0000 ab01  ................
+000003b0: 0000 0000 0000 6601 7412 0000 0000 0000  ......f.t.......
+000003c0: 0000 6a18 0000 0000 0000 0000 0000 0000  ..j.............
+000003d0: 0000 0000 0000 ac02 ab04 0000 0000 0000  ................
+000003e0: 7c00 5f0d 0000 0000 0000 0000 740f 0000  |._.........t...
+000003f0: 0000 0000 0000 6a1c 0000 0000 0000 0000  ......j.........
+00000400: 0000 0000 0000 0000 0000 7c02 721f 7417  ..........|.r.t.
+00000410: 0000 0000 0000 0000 7c00 6a08 0000 0000  ........|.j.....
+00000420: 0000 0000 0000 0000 0000 0000 0000 6a1e  ..............j.
+00000430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000440: 0000 ab01 0000 0000 0000 6e1e 7417 0000  ..........n.t...
+00000450: 0000 0000 0000 7c00 6a08 0000 0000 0000  ......|.j.......
+00000460: 0000 0000 0000 0000 0000 0000 6a20 0000  ............j ..
+00000470: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000480: ab01 0000 0000 0000 ab01 0000 0000 0000  ................
+00000490: 7c00 5f11 0000 0000 0000 0000 7c02 721c  |._.........|.r.
+000004a0: 7c00 6a08 0000 0000 0000 0000 0000 0000  |.j.............
+000004b0: 0000 0000 0000 6a1e 0000 0000 0000 0000  ......j.........
+000004c0: 0000 0000 0000 0000 0000 7c00 5f12 0000  ..........|._...
+000004d0: 0000 0000 0000 6e1b 7c00 6a08 0000 0000  ......n.|.j.....
+000004e0: 0000 0000 0000 0000 0000 0000 0000 6a26  ..............j&
+000004f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000500: 0000 7c00 5f12 0000 0000 0000 0000 7429  ..|._.........t)
+00000510: 0000 0000 0000 0000 7c00 6a08 0000 0000  ........|.j.....
+00000520: 0000 0000 0000 0000 0000 0000 0000 6a2a  ..............j*
+00000530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000540: 0000 7c00 6a08 0000 0000 0000 0000 0000  ..|.j...........
+00000550: 0000 0000 0000 0000 6a2c 0000 0000 0000  ........j,......
+00000560: 0000 0000 0000 0000 0000 0000 6403 6404  ............d.d.
+00000570: ac05 ab04 0000 0000 0000 7c00 5f17 0000  ..........|._...
+00000580: 0000 0000 0000 7c03 7275 7431 0000 0000  ......|.rut1....
+00000590: 0000 0000 7c00 6a08 0000 0000 0000 0000  ....|.j.........
+000005a0: 0000 0000 0000 0000 0000 6a32 0000 0000  ..........j2....
+000005b0: 0000 0000 0000 0000 0000 0000 0000 7c00  ..............|.
+000005c0: 6a08 0000 0000 0000 0000 0000 0000 0000  j...............
+000005d0: 0000 0000 6a20 0000 0000 0000 0000 0000  ....j ..........
+000005e0: 0000 0000 0000 0000 7c00 6a08 0000 0000  ........|.j.....
+000005f0: 0000 0000 0000 0000 0000 0000 0000 6a34  ..............j4
+00000600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000610: 0000 ac06 ab03 0000 0000 0000 7c00 5f1b  ............|._.
+00000620: 0000 0000 0000 0000 7c00 6a2e 0000 0000  ........|.j.....
+00000630: 0000 0000 0000 0000 0000 0000 0000 6a39  ..............j9
+00000640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000650: 0000 6407 7c00 6a36 0000 0000 0000 0000  ..d.|.j6........
+00000660: 0000 0000 0000 0000 0000 ab02 0000 0000  ................
+00000670: 0000 0100 743b 0000 0000 0000 0000 743d  ....t;........t=
+00000680: 0000 0000 0000 0000 6408 6409 ac0a ab02  ........d.d.....
+00000690: 0000 0000 0000 640b 640c 640c 640d 7c00  ......d.d.d.d.|.
+000006a0: 6a08 0000 0000 0000 0000 0000 0000 0000  j...............
+000006b0: 0000 0000 6a34 0000 0000 0000 0000 0000  ....j4..........
+000006c0: 0000 0000 0000 0000 7c00 6a24 0000 0000  ........|.j$....
+000006d0: 0000 0000 0000 0000 0000 0000 0000 7c00  ..............|.
+000006e0: 6a36 0000 0000 0000 0000 0000 0000 0000  j6..............
+000006f0: 0000 0000 ac0e ab08 0000 0000 0000 7c00  ..............|.
+00000700: 5f1f 0000 0000 0000 0000 7c00 6a2e 0000  _.........|.j...
 00000710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000720: 006a 0600 0000 0000 0000 0000 0000 0000  .j..............
-00000730: 0000 0000 00ab 0100 0000 0000 007d 0289  .............}..
-00000740: 086a 0800 0000 0000 0000 0000 0000 0000  .j..............
-00000750: 0000 0000 007c 016a 0a00 0000 0000 0000  .....|.j........
-00000760: 0000 0000 0000 0000 0000 007a 0500 007d  ...........z...}
-00000770: 037c 0264 0119 0000 007c 037a 0a00 007c  .|.d.....|.z...|
-00000780: 0264 0219 0000 007c 037a 0a00 0066 027d  .d.....|.z...f.}
-00000790: 0489 076a 0d00 0000 0000 0000 0000 0000  ...j............
-000007a0: 0000 0000 0000 007c 0364 037a 0500 007c  .......|.d.z...|
-000007b0: 0364 037a 0500 0066 0289 076a 0e00 0000  .d.z...f...j....
-000007c0: 0000 0000 0000 0000 0000 0000 0000 00ab  ................
-000007d0: 0200 0000 0000 007d 0589 086a 1000 0000  .......}...j....
-000007e0: 0000 0000 0000 0000 0000 0000 0000 0064  ...............d
-000007f0: 016b 4400 0072 0264 046e 0164 057d 0689  .kD..r.d.n.d.}..
-00000800: 076a 1200 0000 0000 0000 0000 0000 0000  .j..............
-00000810: 0000 0000 006a 1500 0000 0000 0000 0000  .....j..........
-00000820: 0000 0000 0000 0000 007c 057c 067c 037c  .........|.|.|.|
-00000830: 0366 027c 03ac 06ab 0400 0000 0000 0001  .f.|............
-00000840: 007c 006a 1700 0000 0000 0000 0000 0000  .|.j............
-00000850: 0000 0000 0000 007c 057c 04ab 0200 0000  .......|.|......
-00000860: 0000 0001 0089 076a 1200 0000 0000 0000  .......j........
-00000870: 0000 0000 0000 0000 0000 006a 1500 0000  ...........j....
-00000880: 0000 0000 0000 0000 0000 0000 0000 007c  ...............|
-00000890: 0064 077c 027c 0364 03ac 08ab 0500 0000  .d.|.|.d........
-000008a0: 0000 0001 0079 0029 094e 7202 0000 00e9  .....y.).Nr.....
-000008b0: 0100 0000 7203 0000 0029 04e9 ff00 0000  ....r....)......
-000008c0: 7202 0000 0072 0200 0000 e93c 0000 0029  r....r.....<...)
-000008d0: 0472 0200 0000 7202 0000 0072 2700 0000  .r....r....r'...
-000008e0: 7228 0000 0029 03da 0563 6f6c 6f72 da06  r(...)...color..
-000008f0: 6365 6e74 6572 da06 7261 6469 7573 2903  center..radius).
-00000900: 7202 0000 0072 0200 0000 7227 0000 0029  r....r....r'...)
-00000910: 0572 2300 0000 7229 0000 0072 2a00 0000  .r#...r)...r*...
-00000920: 722b 0000 00da 0577 6964 7468 290c da0e  r+.....width)...
-00000930: 6672 6f6d 5f63 616e 6f6e 6963 616c 721b  from_canonicalr.
-00000940: 0000 00da 0573 7461 7465 721d 0000 0072  .....stater....r
-00000950: 1000 0000 da0c 7363 7265 656e 5f77 6964  ......screen_wid
-00000960: 7468 da07 5375 7266 6163 65da 0853 5243  th..Surface..SRC
-00000970: 414c 5048 41da 0e70 7566 665f 636f 6f6c  ALPHA..puff_cool
-00000980: 5f64 6f77 6eda 0464 7261 77da 0663 6972  _down..draw..cir
-00000990: 636c 65da 0462 6c69 7429 0972 2300 0000  cle..blit).r#...
-000009a0: 7224 0000 00da 1170 7265 6461 746f 725f  r$.....predator_
-000009b0: 6c6f 6361 7469 6f6e da0e 7075 6666 5f61  location..puff_a
-000009c0: 7265 615f 7369 7a65 da0d 7075 6666 5f6c  rea_size..puff_l
-000009d0: 6f63 6174 696f 6eda 1170 7566 665f 6172  ocation..puff_ar
-000009e0: 6561 5f73 7572 6661 6365 da0f 7075 6666  ea_surface..puff
-000009f0: 5f61 7265 615f 636f 6c6f 72da 0670 7967  _area_color..pyg
-00000a00: 616d 65da 0473 656c 6673 0900 0000 2020  ame..selfs....  
-00000a10: 2020 2020 2080 80fa 3b43 3a5c 5265 7365       ...;C:\Rese
-00000a20: 6172 6368 5c63 656c 6c77 6f72 6c64 5f67  arch\cellworld_g
-00000a30: 616d 655c 6365 6c6c 776f 726c 645f 6761  ame\cellworld_ga
-00000a40: 6d65 5c74 6173 6b73 5c62 6f74 6576 6164  me\tasks\botevad
-00000a50: 652e 7079 da10 7265 6e64 6572 5f70 7566  e.py..render_puf
-00000a60: 665f 6172 6561 7a2b 426f 7445 7661 6465  f_areaz+BotEvade
-00000a70: 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63 616c  .__init__.<local
-00000a80: 733e 2e72 656e 6465 725f 7075 6666 5f61  s>.render_puff_a
-00000a90: 7265 613a 0000 0073 fa00 0000 f880 00e0  rea:...s........
-00000aa0: 283c d728 4bd1 284b c844 cf4d c94d d74c  (<.(K.(K.D.M.M.L
-00000ab0: 5fd1 4c5f d74c 68d1 4c68 d328 69d0 1425  _.L_.Lh.Lh.(i..%
-00000ac0: d825 29d7 2538 d125 38d0 3b4f d73b 5cd1  .%).%8.%8.;O.;\.
-00000ad0: 3b5c d125 5c90 4ed8 2435 b061 d124 38b8  ;\.%\.N.$5.a.$8.
-00000ae0: 3ed1 2449 d04b 5cd0 5d5e d14b 5fd0 6270  >.$I.K\.]^.K_.bp
-00000af0: d14b 70d0 2470 904d d828 2eaf 0ea9 0eb8  .Kp.$p.M.(......
-00000b00: 0ec8 11d1 384a c84e d05d 5ed1 4c5e d037  ....8J.N.]^.L^.7
-00000b10: 5fd0 6167 d761 70d1 6170 d328 71d0 1425  _.ag.ap.ap.(q..%
-00000b20: d839 3dd7 394c d139 4cc8 71d2 3950 a16f  .9=.9L.9L.q.9P.o
-00000b30: d056 6590 4fd8 141a 974b 914b d714 26d1  .Ve.O....K.K..&.
-00000b40: 1426 d027 38d8 2d3c d82f 3db8 7ed0 2e4e  .&.'8.-<./=.~..N
-00000b50: d82e 3cf0 0700 1527 f400 0315 3ef0 0800  ..<....'....>...
-00000b60: 151c 974c 914c d021 32d8 212e f403 0115  ...L.L.!2.!.....
-00000b70: 30e0 141a 974b 914b d714 26d1 1426 a877  0....K.K..&..&.w
-00000b80: d82d 38d8 2e3f d82e 3cd8 2d2e f009 0015  .-8..?..<.-.....
-00000b90: 27f5 0004 1530 f300 0000 0072 2600 0000  '....0.....r&...
-00000ba0: 2924 720e 0000 0072 0f00 0000 7210 0000  )$r....r....r...
-00000bb0: 00da 0d67 6f61 6c5f 6c6f 6361 7469 6f6e  ...goal_location
-00000bc0: 7211 0000 0072 1400 0000 720a 0000 00da  r....r....r.....
-00000bd0: 066c 6f61 6465 7272 0500 0000 da08 5f5f  .loaderr......__
-00000be0: 696e 6974 5f5f 7216 0000 0072 1700 0000  init__r....r....
-00000bf0: 7209 0000 00da 1572 6f62 6f74 5f73 7461  r......robot_sta
-00000c00: 7274 5f6c 6f63 6174 696f 6e73 7219 0000  rt_locationsr...
-00000c10: 0072 1a00 0000 721b 0000 00da 0961 6464  .r....r......add
-00000c20: 5f61 6765 6e74 7208 0000 0072 0600 0000  _agentr....r....
-00000c30: 7220 0000 00da 0772 756e 6e69 6e67 da04  r .....running..
-00000c40: 7669 6577 7221 0000 00da 0b5f 5f6f 6e5f  viewr!.....__on_
-00000c50: 7175 6974 5f5f da07 6f6e 5f71 7569 7472  quit__..on_quitr
-00000c60: 3b00 0000 7230 0000 0072 0700 0000 da0f  ;...r0...r......
-00000c70: 6164 645f 7265 6e64 6572 5f73 7465 70da  add_render_step.
-00000c80: 0670 7566 6665 6472 3200 0000 da0d 676f  .puffedr2.....go
-00000c90: 616c 5f61 6368 6965 7665 64da 1670 7265  al_achieved..pre
-00000ca0: 6461 746f 725f 7072 6579 5f64 6973 7461  dator_prey_dista
-00000cb0: 6e63 65da 1270 7265 795f 676f 616c 5f64  nce..prey_goal_d
-00000cc0: 6973 7461 6e63 65da 0a70 7566 665f 636f  istance..puff_co
-00000cd0: 756e 7429 0d72 3c00 0000 720d 0000 0072  unt).r<...r....r
-00000ce0: 0e00 0000 720f 0000 0072 1000 0000 7240  ....r....r....r@
-00000cf0: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
-00000d00: 0000 7214 0000 0072 2100 0000 723e 0000  ..r....r!...r>..
-00000d10: 0072 3b00 0000 730d 0000 0060 2020 2020  .r;...s....`    
-00000d20: 2020 2020 2020 2040 723d 0000 0072 4200         @r=...rB.
-00000d30: 0000 7a11 426f 7445 7661 6465 2e5f 5f69  ..z.BotEvade.__i
-00000d40: 6e69 745f 5f0b 0000 0073 8301 0000 f980  nit__....s......
-00000d50: 00f0 1400 1d29 8804 d408 19d8 2336 8804  .....)......#6..
-00000d60: d408 20d8 1e2c 8804 d408 1bd8 1d2a 8804  .. ..,.......*..
-00000d70: d408 1ad8 1e2c 8804 d408 1bd8 161c 8804  .....,..........
-00000d80: 8c0b dc16 25b0 1ad4 163c 8804 8c0b e408  ....%....<......
-00000d90: 0d8f 0e89 0e90 74d8 1d21 9f5b 995b d71d  ......t..!.[.[..
-00000da0: 2ed1 1d2e d822 26a7 2ba1 2bd7 2238 d122  ....."&.+.+."8."
-00000db0: 38d8 212a d821 2af5 0904 092c f10c 000c  8.!*.!*....,....
-00000dc0: 18dc 1c21 b024 b72b b12b d732 53d1 3253  ...!.$.+.+.2S.2S
-00000dd0: d831 35b7 1bb1 1bd7 314b d131 4bd8 2d31  .15.....1K.1K.-1
-00000de0: af5b a95b d72d 43d1 2d43 f405 021d 4501  .[.[.-C.-C....E.
-00000df0: 8844 8c4d f008 000d 118f 4e89 4e98 3aa0  .D.M......N.N.:.
-00000e00: 74a7 7da1 7dd4 0c35 e414 19a4 6ab8 29d8  t.}.}..5....j.).
-00000e10: 3b3c f403 0127 3ee0 2529 a75b a15b d725  ;<...'>.%).[.[.%
-00000e20: 3bd1 253b f405 0215 3d88 048c 09f0 0800  ;.%;....=.......
-00000e30: 090d 8f0e 890e 9076 9874 9f79 9979 d408  .......v.t.y.y..
-00000e40: 29e0 171c 8804 8c0c e00b 0f8f 3b8a 3bdd  )...........;.;.
-00000e50: 0c23 d918 1ca0 34d4 1828 8844 8c49 d820  .#....4..(.D.I. 
-00000e60: 24d7 2030 d120 3088 448f 4989 49d4 0c1d  $. 0. 0.D.I.I...
-00000e70: e10f 1bdb 101d f004 1111 30a8 66af 6ea9  ..........0.f.n.
-00000e80: 6ef0 0011 1130 dc3b 4ef6 0311 1130 f026  n....0.;N....0.&
-00000e90: 0011 1597 0991 09d7 1029 d110 29d0 2a3a  .........)..).*:
-00000ea0: d410 3be0 1c21 8804 8c0b d825 2688 04d4  ..;..!.....%&...
-00000eb0: 081b d823 2888 04d4 081a d82d 2e88 04d4  ...#(......-....
-00000ec0: 0823 d829 2a88 04d4 081f d81a 1b88 048d  .#.)*...........
-00000ed0: 0f72 3f00 0000 da07 6465 6c74 615f 7463  .r?.....delta_tc
-00000ee0: 0200 0000 0000 0000 0000 0000 0500 0000  ................
-00000ef0: 0300 0000 f350 0400 0097 007c 006a 0000  .....P.....|.j..
-00000f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000f10: 0090 0172 8c7c 006a 0200 0000 0000 0000  ...r.|.j........
-00000f20: 0000 0000 0000 0000 0000 0064 016b 1a00  ...........d.k..
-00000f30: 0090 0172 7c74 0500 0000 0000 0000 007c  ...r|t.........|
-00000f40: 006a 0600 0000 0000 0000 0000 0000 0000  .j..............
-00000f50: 0000 0000 006a 0800 0000 0000 0000 0000  .....j..........
-00000f60: 0000 0000 0000 0000 006a 0a00 0000 0000  .........j......
-00000f70: 0000 0000 0000 0000 0000 0000 007c 006a  .............|.j
-00000f80: 0c00 0000 0000 0000 0000 0000 0000 0000  ................
-00000f90: 0000 006a 0800 0000 0000 0000 0000 0000  ...j............
-00000fa0: 0000 0000 0000 006a 0a00 0000 0000 0000  .......j........
-00000fb0: 0000 0000 0000 0000 0000 00ab 0200 0000  ................
-00000fc0: 0000 007c 005f 0700 0000 0000 0000 007c  ...|._.........|
-00000fd0: 006a 1000 0000 0000 0000 0000 0000 0000  .j..............
-00000fe0: 0000 0000 006a 1300 0000 0000 0000 0000  .....j..........
-00000ff0: 0000 0000 0000 0000 007c 006a 0600 0000  .........|.j....
-00001000: 0000 0000 0000 0000 0000 0000 0000 006a  ...............j
-00001010: 0800 0000 0000 0000 0000 0000 0000 0000  ................
-00001020: 0000 006a 0a00 0000 0000 0000 0000 0000  ...j............
-00001030: 0000 0000 0000 007c 006a 0c00 0000 0000  .......|.j......
-00001040: 0000 0000 0000 0000 0000 0000 006a 0800  .............j..
-00001050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001060: 006a 0a00 0000 0000 0000 0000 0000 0000  .j..............
-00001070: 0000 0000 00ab 0200 0000 0000 0072 7f7c  .............r.|
-00001080: 006a 0e00 0000 0000 0000 0000 0000 0000  .j..............
-00001090: 0000 0000 007c 006a 1400 0000 0000 0000  .....|.j........
-000010a0: 0000 0000 0000 0000 0000 006b 1a00 0072  ...........k...r
-000010b0: 2d64 027c 005f 0b00 0000 0000 0000 007c  -d.|._.........|
-000010c0: 0078 016a 1800 0000 0000 0000 0000 0000  .x.j............
-000010d0: 0000 0000 0000 0064 037a 0d00 0063 025f  .......d.z...c._
-000010e0: 0c00 0000 0000 0000 007c 006a 1a00 0000  .........|.j....
-000010f0: 0000 0000 0000 0000 0000 0000 0000 007c  ...............|
-00001100: 005f 0100 0000 0000 0000 007c 006a 0c00  ._.........|.j..
-00001110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001120: 006a 1d00 0000 0000 0000 0000 0000 0000  .j..............
-00001130: 0000 0000 007c 006a 0600 0000 0000 0000  .....|.j........
-00001140: 0000 0000 0000 0000 0000 006a 0800 0000  ...........j....
-00001150: 0000 0000 0000 0000 0000 0000 0000 006a  ...............j
-00001160: 0a00 0000 0000 0000 0000 0000 0000 0000  ................
-00001170: 0000 00ab 0100 0000 0000 0001 007c 006a  .............|.j
-00001180: 0c00 0000 0000 0000 0000 0000 0000 0000  ................
-00001190: 0000 006a 1e00 0000 0000 0000 0000 0000  ...j............
-000011a0: 0000 0000 0000 0073 427c 006a 0c00 0000  .......sB|.j....
-000011b0: 0000 0000 0000 0000 0000 0000 0000 006a  ...............j
-000011c0: 1d00 0000 0000 0000 0000 0000 0000 0000  ................
-000011d0: 0000 0074 2100 0000 0000 0000 006a 2200  ...t!........j".
-000011e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000011f0: 007c 006a 2400 0000 0000 0000 0000 0000  .|.j$...........
-00001200: 0000 0000 0000 006a 2600 0000 0000 0000  .......j&.......
-00001210: 0000 0000 0000 0000 0000 00ab 0100 0000  ................
-00001220: 0000 00ab 0100 0000 0000 0001 007c 017c  .............|.|
-00001230: 006a 0200 0000 0000 0000 0000 0000 0000  .j..............
-00001240: 0000 0000 006b 0200 0072 167c 0078 016a  .....k...r.|.x.j
-00001250: 0200 0000 0000 0000 0000 0000 0000 0000  ................
-00001260: 0000 007c 017a 1700 0063 025f 0100 0000  ...|.z...c._....
-00001270: 0000 0000 006e 0764 017c 005f 0100 0000  .....n.d.|._....
-00001280: 0000 0000 0074 0500 0000 0000 0000 007c  .....t.........|
-00001290: 006a 2800 0000 0000 0000 0000 0000 0000  .j(.............
-000012a0: 0000 0000 007c 006a 0600 0000 0000 0000  .....|.j........
-000012b0: 0000 0000 0000 0000 0000 006a 0800 0000  ...........j....
-000012c0: 0000 0000 0000 0000 0000 0000 0000 006a  ...............j
-000012d0: 0a00 0000 0000 0000 0000 0000 0000 0000  ................
-000012e0: 0000 00ab 0200 0000 0000 007c 005f 1500  ...........|._..
-000012f0: 0000 0000 0000 007c 006a 2a00 0000 0000  .......|.j*.....
-00001300: 0000 0000 0000 0000 0000 0000 007c 006a  .............|.j
-00001310: 2c00 0000 0000 0000 0000 0000 0000 0000  ,...............
-00001320: 0000 006b 1a00 0072 0f64 027c 005f 1700  ...k...r.d.|._..
-00001330: 0000 0000 0000 0064 047c 005f 1800 0000  .......d.|._....
-00001340: 0000 0000 0079 0079 0029 054e 7202 0000  .....y.y.).Nr...
-00001350: 0054 7226 0000 0046 2919 720e 0000 0072  .Tr&...F).r....r
-00001360: 3200 0000 7204 0000 0072 2000 0000 722e  2...r....r ...r.
-00001370: 0000 0072 1d00 0000 721b 0000 0072 4c00  ...r....r....rL.
-00001380: 0000 da0a 7669 7369 6269 6c69 7479 da0d  ....visibility..
-00001390: 6c69 6e65 5f6f 665f 7369 6768 7472 1000  line_of_sightr..
-000013a0: 0000 724a 0000 0072 4e00 0000 720f 0000  ..rJ...rN...r...
-000013b0: 00da 0f73 6574 5f64 6573 7469 6e61 7469  ...set_destinati
-000013c0: 6f6e da04 7061 7468 da06 7261 6e64 6f6d  on..path..random
-000013d0: da06 6368 6f69 6365 7241 0000 0072 1900  ..choicerA...r..
-000013e0: 0000 7240 0000 0072 4d00 0000 7211 0000  ..r@...rM...r...
-000013f0: 0072 4b00 0000 7245 0000 00a9 0272 3c00  .rK...rE.....r<.
-00001400: 0000 724f 0000 0073 0200 0000 2020 723d  ..rO...s....  r=
-00001410: 0000 00da 105f 5f75 7064 6174 655f 7374  .....__update_st
-00001420: 6174 655f 5f7a 1942 6f74 4576 6164 652e  ate__z.BotEvade.
-00001430: 5f5f 7570 6461 7465 5f73 7461 7465 5f5f  __update_state__
-00001440: 5600 0000 7376 0100 0080 00e0 0b0f d70b  V...sv..........
-00001450: 1cd3 0b1c a014 d721 34d1 2134 b801 d321  .......!4.!4...!
-00001460: 39dc 2a32 b034 b739 b139 b73f b13f d733  9.*2.4.9.9.?.?.3
-00001470: 4bd1 334b d833 37b7 3db1 3dd7 3346 d133  K.3K.37.=.=.3F.3
-00001480: 46d7 334f d133 4ff3 0301 2b51 0188 44d4  F.3O.3O...+Q..D.
-00001490: 0c27 e00f 138f 7f89 7fd7 0f2c d10f 2ca8  .'.........,..,.
-000014a0: 54af 59a9 59af 5fa9 5fd7 2d45 d12d 45c0  T.Y.Y._._.-E.-E.
-000014b0: 74c7 7dc1 7dd7 475a d147 5ad7 4763 d147  t.}.}.GZ.GZ.Gc.G
-000014c0: 63d4 0f64 d813 17d7 132e d113 2eb0 24d7  c..d..........$.
-000014d0: 3245 d132 45d2 1345 d822 2690 4494 4bd8  2E.2E..E."&.D.K.
-000014e0: 1418 974f 924f a071 d114 2895 4fd8 2a2e  ...O.O.q..(.O.*.
-000014f0: d72a 42d1 2a42 9044 d414 27e0 1014 970d  .*B.*B.D..'.....
-00001500: 910d d710 2dd1 102d a864 af69 a969 af6f  ....-..-.d.i.i.o
-00001510: a96f d72e 46d1 2e46 d410 47e0 1317 973d  .o..F..F..G....=
-00001520: 913d d713 25d2 1325 d810 1497 0d91 0dd7  .=..%..%........
-00001530: 102d d110 2dac 66af 6da9 6db8 44bf 4bb9  .-..-.f.m.m.D.K.
-00001540: 4bd7 3c56 d13c 56d3 2e57 d410 58e0 0b12  K.<V.<V..W..X...
-00001550: 9054 d715 28d1 1528 d20b 28d8 0c10 d70c  .T..(..(..(.....
-00001560: 1fd2 0c1f a037 d10c 2ad6 0c1f e022 2388  .....7..*...."#.
-00001570: 44d4 0c1f e422 2aa8 34d7 2b3d d12b 3db8  D...."*.4.+=.+=.
-00001580: 74bf 79b9 79bf 7fb9 7fd7 3f57 d13f 57d3  t.y.y.....?W.?W.
-00001590: 2258 8804 d408 1fe0 0b0f d70b 22d1 0b22  "X..........".."
-000015a0: a064 d726 39d1 2639 d20b 39d8 2125 8844  .d.&9.&9..9.!%.D
-000015b0: d40c 1ed8 1b20 8844 8d4c f005 000c 3a72  ..... .D.L....:r
-000015c0: 3f00 0000 6301 0000 0000 0000 0000 0000  ?...c...........
-000015d0: 0002 0000 0003 0000 00f3 1200 0000 9700  ................
-000015e0: 6401 7c00 5f00 0000 0000 0000 0000 7900  d.|._.........y.
-000015f0: 2902 4e46 2901 7245 0000 00a9 0172 3c00  ).NF).rE.....r<.
-00001600: 0000 7301 0000 0020 723d 0000 0072 4700  ..s.... r=...rG.
-00001610: 0000 7a14 426f 7445 7661 6465 2e5f 5f6f  ..z.BotEvade.__o
-00001620: 6e5f 7175 6974 5f5f 7100 0000 7309 0000  n_quit__q...s...
-00001630: 0080 00d8 171c 8804 8d0c 723f 0000 0063  ..........r?...c
-00001640: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-00001650: 0300 0000 f36a 0000 0097 0074 0100 0000  .....j.....t....
-00001660: 0000 0000 006a 0200 0000 0000 0000 0000  .....j..........
-00001670: 0000 0000 0000 0000 007c 00ab 0100 0000  .........|......
-00001680: 0000 0001 0064 017c 005f 0200 0000 0000  .....d.|._......
-00001690: 0000 0064 027c 005f 0300 0000 0000 0000  ...d.|._........
-000016a0: 007c 006a 0900 0000 0000 0000 0000 0000  .|.j............
-000016b0: 0000 0000 0000 00ab 0000 0000 0000 0001  ................
-000016c0: 0079 0029 034e 4672 0200 0000 2905 7205  .y.).NFr....).r.
-000016d0: 0000 00da 0572 6573 6574 724b 0000 0072  .....resetrK...r
-000016e0: 4e00 0000 7258 0000 0072 5a00 0000 7301  N...rX...rZ...s.
-000016f0: 0000 0020 723d 0000 0072 5c00 0000 7a0e  ... r=...r\...z.
-00001700: 426f 7445 7661 6465 2e72 6573 6574 7400  BotEvade.resett.
-00001710: 0000 7329 0000 0080 00dc 080d 8f0b 890b  ..s)............
-00001720: 9044 d408 19d8 1d22 8804 d408 1ad8 1a1b  .D....."........
-00001730: 8804 8c0f d808 0cd7 081d d108 1dd5 081f  ................
-00001740: 723f 0000 00da 0672 6574 7572 6e63 0100  r?.....returnc..
-00001750: 0000 0000 0000 0000 0000 0300 0000 0300  ................
-00001760: 0000 f3a0 0000 0097 0074 0100 0000 0000  .........t......
-00001770: 0000 006a 0200 0000 0000 0000 0000 0000  ...j............
-00001780: 0000 0000 0000 007c 00ab 0100 0000 0000  .......|........
-00001790: 007d 017c 006a 0400 0000 0000 0000 0000  .}.|.j..........
-000017a0: 0000 0000 0000 0000 0072 1a7c 006a 0600  .........r.|.j..
-000017b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000017c0: 006a 0900 0000 0000 0000 0000 0000 0000  .j..............
-000017d0: 0000 0000 00ab 0000 0000 0000 0001 007c  ...............|
-000017e0: 006a 0b00 0000 0000 0000 0000 0000 0000  .j..............
-000017f0: 0000 0000 007c 01ac 01ab 0100 0000 0000  .....|..........
-00001800: 0001 007c 0153 0029 024e 2901 724f 0000  ...|.S.).N).rO..
-00001810: 0029 0672 0500 0000 da04 7374 6570 7214  .).r......stepr.
-00001820: 0000 0072 4600 0000 7233 0000 0072 5800  ...rF...r3...rX.
-00001830: 0000 7257 0000 0073 0200 0000 2020 723d  ..rW...s....  r=
-00001840: 0000 0072 5f00 0000 7a0d 426f 7445 7661  ...r_...z.BotEva
-00001850: 6465 2e73 7465 707a 0000 0073 3b00 0000  de.stepz...s;...
-00001860: 8000 dc12 1797 2a91 2a98 54d3 1222 8807  ......*.*.T.."..
-00001870: d80b 0f8f 3b8a 3bd8 0c10 8f49 8949 8f4e  ....;.;....I.I.N
-00001880: 894e d40c 1cd8 080c d708 1dd1 081d a067  .N.............g
-00001890: d008 1dd4 082e d80f 1688 0e72 3f00 0000  ...........r?...
-000018a0: 4e29 09da 0532 315f 3035 5472 1c00 0000  N)...21_05Tr....
-000018b0: e79a 9999 9999 99b9 3f29 0267 0000 0000  ........?).g....
-000018c0: 0000 f03f 721c 0000 0072 6100 0000 679a  ...?r....ra...g.
-000018d0: 9999 9999 9999 3f46 4629 0172 0200 0000  ......?FF).r....
-000018e0: 290b da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-000018f0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-00001900: 6e61 6d65 5f5f da03 7374 72da 0462 6f6f  name__..str..boo
-00001910: 6cda 0566 6c6f 6174 7242 0000 0072 5800  l..floatrB...rX.
-00001920: 0000 7247 0000 0072 5c00 0000 725f 0000  ..rG...r\...r_..
-00001930: 00a9 0072 3f00 0000 723d 0000 0072 0c00  ...r?...r=...r..
-00001940: 0000 720c 0000 000a 0000 0073 a000 0000  ..r........s....
-00001950: 8400 e023 2ad8 262a d82e 30d8 292b d81f  ...#*.&*..0.)+..
-00001960: 29d8 292b d824 28d8 2328 d820 25f1 1349  ).)+.$(.#(. %..I
-00001970: 0105 1cd8 1d20 f003 4901 051c e01f 23f0  ..... ..I.....#.
-00001980: 0549 0105 1cf0 0600 272c f007 4901 051c  .I......',..I...
-00001990: f008 0022 27f0 0949 0105 1cf0 0c00 2227  ..."'..I......"'
-000019a0: f00d 4901 051c f00e 001d 22f0 0f49 0105  ..I......."..I..
-000019b0: 1cf0 1000 1d21 f011 4901 051c f012 001a  .....!..I.......
-000019c0: 1ef3 1349 0105 1cf0 5802 002b 2cf1 0319  ...I....X..+,...
-000019d0: 0521 d822 27f3 0319 0521 f236 0105 1df2  .!."'....!.6....
-000019e0: 0604 0520 f00c 0505 1790 65f4 0005 0517  ... ......e.....
-000019f0: 723f 0000 0072 0c00 0000 290f 7255 0000  r?...r....).rU..
-00001a00: 00da 0475 7469 6c72 0400 0000 7222 0000  ...utilr....r"..
-00001a10: 0072 0500 0000 da05 6167 656e 7472 0600  .r......agentr..
-00001a20: 0000 7207 0000 00da 056d 6f75 7365 7208  ..r......mouser.
-00001a30: 0000 00da 0572 6f62 6f74 7209 0000 00da  .....robotr.....
-00001a40: 1063 656c 6c77 6f72 6c64 5f6c 6f61 6465  .cellworld_loade
-00001a50: 7272 0a00 0000 720c 0000 0072 6800 0000  rr....r....rh...
-00001a60: 723f 0000 0072 3d00 0000 fa08 3c6d 6f64  r?...r=.....<mod
-00001a70: 756c 653e 726e 0000 0001 0000 0073 2800  ule>rn.......s(.
-00001a80: 0000 f003 0101 01db 000d dd00 1bdd 0019  ................
-00001a90: df00 33dd 0019 dd00 19dd 002e f406 7501  ..3...........u.
-00001aa0: 0117 8875 f500 7501 0117 723f 0000 00    ...u..u...r?...
+00000720: 6a39 0000 0000 0000 0000 0000 0000 0000  j9..............
+00000730: 0000 0000 640f 7c00 6a3e 0000 0000 0000  ....d.|.j>......
+00000740: 0000 0000 0000 0000 0000 0000 ab02 0000  ................
+00000750: 0000 0000 0100 6400 7c00 5f20 0000 0000  ......d.|._ ....
+00000760: 0000 0000 6404 7c00 5f21 0000 0000 0000  ....d.|._!......
+00000770: 0000 6409 7c00 5f22 0000 0000 0000 0000  ..d.|._"........
+00000780: 6409 7c00 5f23 0000 0000 0000 0000 7900  d.|._#........y.
+00000790: 2910 4e29 0172 1900 0000 2901 da05 6474  ).N).r....)...dt
+000007a0: 7970 6567 9a99 9999 9999 993f 4629 04da  ypeg.......?F)..
+000007b0: 0561 7265 6e61 da0a 6f63 636c 7573 696f  .arena..occlusio
+000007c0: 6e73 da09 7469 6d65 5f73 7465 70da 0972  ns..time_step..r
+000007d0: 6561 6c5f 7469 6d65 2903 da0f 7374 6172  eal_time)...star
+000007e0: 745f 6c6f 6361 7469 6f6e 73da 0e6f 7065  t_locations..ope
+000007f0: 6e5f 6c6f 6361 7469 6f6e 73da 0a6e 6176  n_locations..nav
+00000800: 6967 6174 696f 6eda 0870 7265 6461 746f  igation..predato
+00000810: 7229 0267 9a99 9999 9999 a93f e700 0000  r).g.......?....
+00000820: 0000 00e0 3f72 0900 0000 2902 da08 6c6f  ....?r....)...lo
+00000830: 6361 7469 6f6e da09 6469 7265 6374 696f  cation..directio
+00000840: 6e29 0272 0200 0000 7228 0000 0067 9a99  n).r....r(...g..
+00000850: 9999 9999 b93f 7228 0000 0029 08da 0b73  .....?r(...)...s
+00000860: 7461 7274 5f73 7461 7465 da0d 676f 616c  tart_state..goal
+00000870: 5f6c 6f63 6174 696f 6eda 0e67 6f61 6c5f  _location..goal_
+00000880: 7468 7265 7368 6f6c 64da 0e70 7566 665f  threshold..puff_
+00000890: 7468 7265 7368 6f6c 64da 1370 7566 665f  threshold..puff_
+000008a0: 636f 6f6c 5f64 6f77 6e5f 7469 6d65 7226  cool_down_timer&
+000008b0: 0000 00da 0761 6374 696f 6e73 7227 0000  .....actionsr'..
+000008c0: 00da 0470 7265 7929 2472 1c00 0000 da0f  ...prey)$r......
+000008d0: 7265 7761 7264 5f66 756e 6374 696f 6e72  reward_functionr
+000008e0: 1d00 0000 720c 0000 00da 066c 6f61 6465  ....r......loade
+000008f0: 7272 0600 0000 da0b 6f62 7365 7276 6174  rr......observat
+00000900: 696f 6e72 0b00 0000 da03 426f 78da 026e  ionr......Box..n
+00000910: 70da 0369 6e66 da03 6c65 6eda 0766 6c6f  p..inf..len..flo
+00000920: 6174 3332 da11 6f62 7365 7276 6174 696f  at32..observatio
+00000930: 6e5f 7370 6163 65da 0844 6973 6372 6574  n_space..Discret
+00000940: 65da 1174 6c70 706f 5f61 6374 696f 6e5f  e..tlppo_action_
+00000950: 6c69 7374 7225 0000 00da 0c61 6374 696f  listr%.....actio
+00000960: 6e5f 7370 6163 65da 0b61 6374 696f 6e5f  n_space..action_
+00000970: 6c69 7374 da10 6675 6c6c 5f61 6374 696f  list..full_actio
+00000980: 6e5f 6c69 7374 7203 0000 0072 2000 0000  n_listr....r ...
+00000990: 7221 0000 00da 056d 6f64 656c 7204 0000  r!.....modelr...
+000009a0: 00da 1572 6f62 6f74 5f73 7461 7274 5f6c  ...robot_start_l
+000009b0: 6f63 6174 696f 6e73 7226 0000 0072 2700  ocationsr&...r'.
+000009c0: 0000 da09 6164 645f 6167 656e 7472 0500  ....add_agentr..
+000009d0: 0000 7207 0000 0072 3100 0000 da04 7669  ..r....r1.....vi
+000009e0: 6577 da0c 7265 6e64 6572 5f73 7465 7073  ew..render_steps
+000009f0: da0a 7374 6570 5f63 6f75 6e74 da08 6361  ..step_count..ca
+00000a00: 7074 7572 6573 2907 da04 7365 6c66 7219  ptures)...selfr.
+00000a10: 0000 0072 1a00 0000 721b 0000 0072 1c00  ...r....r....r..
+00000a20: 0000 7232 0000 0072 1d00 0000 7307 0000  ..r2...r....s...
+00000a30: 0020 2020 2020 2020 7215 0000 00da 085f  .       r......_
+00000a40: 5f69 6e69 745f 5f7a 1445 6e76 6972 6f6e  _init__z.Environ
+00000a50: 6d65 6e74 2e5f 5f69 6e69 745f 5f0f 0000  ment.__init__...
+00000a60: 0073 c001 0000 8000 f00e 0019 2188 048c  .s..........!...
+00000a70: 0dd8 1f2e 8804 d408 1cd8 1922 8804 8c0e  ..........."....
+00000a80: dc16 25b0 1ad4 163c 8804 8c0b dc1b 2bd3  ..%....<......+.
+00000a90: 1b2d 8804 d408 18dc 2127 a71a a11a ac52  .-......!'.....R
+00000aa0: af56 a956 a847 b452 b756 b156 bc63 c024  .V.V.G.R.V.V.c.$
+00000ab0: d742 52d1 4252 d33e 53d0 3d55 d45d 5fd7  .BR.BR.>S.=U.]_.
+00000ac0: 5d67 d15d 67d4 2168 8804 d408 1edc 1c22  ]g.]g.!h......."
+00000ad0: 9f4f 994f d92f 38f4 0300 2d30 b004 b70b  .O.O./8...-0....
+00000ae0: b10b d730 4dd1 304d d42c 4ee4 3134 b054  ...0M.0M.,N.14.T
+00000af0: b75b b15b d735 4fd1 354f d331 50f3 0502  .[.[.5O.5O.1P...
+00000b00: 1d52 0188 04d4 0819 f106 000c 15d8 1f23  .R.............#
+00000b10: 9f7b 997b d71f 3cd1 1f3c 8844 d50c 1ce0  .{.{..<..<.D....
+00000b20: 1f23 9f7b 997b d71f 3bd1 1f3b 8844 d40c  .#.{.{..;..;.D..
+00000b30: 1ce4 151a a014 a71b a11b d721 32d1 2132  ...........!2.!2
+00000b40: d826 2aa7 6ba1 6bd7 263c d126 3cd8 2529  .&*.k.k.&<.&<.%)
+00000b50: d825 2af4 0703 162c 8804 8c0a f108 000c  .%*....,........
+00000b60: 18dc 1c21 b024 b72b b12b d732 53d1 3253  ...!.$.+.+.2S.2S
+00000b70: d831 35b7 1bb1 1bd7 314b d131 4bd8 2d31  .15.....1K.1K.-1
+00000b80: af5b a95b d72d 43d1 2d43 f405 021d 4501  .[.[.-C.-C....E.
+00000b90: 8844 8c4d f006 000d 118f 4a89 4ad7 0c20  .D.M......J.J.. 
+00000ba0: d10c 20a0 1aa8 54af 5da9 5dd4 0c3b e414  .. ...T.].]..;..
+00000bb0: 19a4 6ab8 29d8 3b3c f403 0127 3ee0 282f  ..j.).;<...'>.(/
+00000bc0: d829 2bd8 292b d82e 30d8 2529 a75b a15b  .)+.)+..0.%).[.[
+00000bd0: d725 3bd1 253b d822 26d7 2232 d122 32d8  .%;.%;."&."2."2.
+00000be0: 2327 a73d a13d f411 0815 3288 048c 09f0  #'.=.=....2.....
+00000bf0: 1200 090d 8f0a 890a d708 1cd1 081c 9856  ...............V
+00000c00: a054 a759 a159 d408 2fd8 1418 8804 8c09  .T.Y.Y../.......
+00000c10: d81c 2188 04d4 0819 d81a 1b88 048c 0fd8  ..!.............
+00000c20: 1819 8804 8d0d 7217 0000 0063 0100 0000  ......r....c....
+00000c30: 0000 0000 0000 0000 0400 0000 0300 0000  ................
+00000c40: f37a 0800 0097 007c 006a 0000 0000 0000  .z.....|.j......
+00000c50: 0000 0000 0000 0000 0000 0000 006a 0200  .............j..
+00000c60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000c70: 006a 0400 0000 0000 0000 0000 0000 0000  .j..............
+00000c80: 0000 0000 0064 0119 0000 007c 006a 0600  .....d.....|.j..
+00000c90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000ca0: 0074 0800 0000 0000 0000 006a 0a00 0000  .t.........j....
+00000cb0: 0000 0000 0000 0000 0000 0000 0000 006a  ...............j
+00000cc0: 0c00 0000 0000 0000 0000 0000 0000 0000  ................
+00000cd0: 0000 003c 0000 007c 006a 0000 0000 0000  ...<...|.j......
+00000ce0: 0000 0000 0000 0000 0000 0000 006a 0200  .............j..
+00000cf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000d00: 006a 0400 0000 0000 0000 0000 0000 0000  .j..............
+00000d10: 0000 0000 0064 0219 0000 007c 006a 0600  .....d.....|.j..
+00000d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000d30: 0074 0800 0000 0000 0000 006a 0a00 0000  .t.........j....
+00000d40: 0000 0000 0000 0000 0000 0000 0000 006a  ...............j
+00000d50: 0e00 0000 0000 0000 0000 0000 0000 0000  ................
+00000d60: 0000 003c 0000 0074 1100 0000 0000 0000  ...<...t........
+00000d70: 006a 1200 0000 0000 0000 0000 0000 0000  .j..............
+00000d80: 0000 0000 007c 006a 0000 0000 0000 0000  .....|.j........
+00000d90: 0000 0000 0000 0000 0000 006a 0200 0000  ...........j....
+00000da0: 0000 0000 0000 0000 0000 0000 0000 006a  ...............j
+00000db0: 1400 0000 0000 0000 0000 0000 0000 0000  ................
+00000dc0: 0000 00ab 0100 0000 0000 007c 006a 0600  ...........|.j..
+00000dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000de0: 0074 0800 0000 0000 0000 006a 0a00 0000  .t.........j....
+00000df0: 0000 0000 0000 0000 0000 0000 0000 006a  ...............j
+00000e00: 1600 0000 0000 0000 0000 0000 0000 0000  ................
+00000e10: 0000 003c 0000 007c 006a 1800 0000 0000  ...<...|.j......
+00000e20: 0000 0000 0000 0000 0000 0000 006a 1a00  .............j..
+00000e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000e40: 006a 1d00 0000 0000 0000 0000 0000 0000  .j..............
+00000e50: 0000 0000 007c 006a 0000 0000 0000 0000  .....|.j........
+00000e60: 0000 0000 0000 0000 0000 006a 0200 0000  ...........j....
+00000e70: 0000 0000 0000 0000 0000 0000 0000 006a  ...............j
+00000e80: 0400 0000 0000 0000 0000 0000 0000 0000  ................
+00000e90: 0000 007c 006a 1e00 0000 0000 0000 0000  ...|.j..........
+00000ea0: 0000 0000 0000 0000 006a 0200 0000 0000  .........j......
+00000eb0: 0000 0000 0000 0000 0000 0000 006a 0400  .............j..
+00000ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000ed0: 00ab 0200 0000 0000 0090 0172 317c 006a  ...........r1|.j
+00000ee0: 1e00 0000 0000 0000 0000 0000 0000 0000  ................
+00000ef0: 0000 006a 0200 0000 0000 0000 0000 0000  ...j............
+00000f00: 0000 0000 0000 006a 0400 0000 0000 0000  .......j........
+00000f10: 0000 0000 0000 0000 0000 0064 0119 0000  ...........d....
+00000f20: 007c 006a 0600 0000 0000 0000 0000 0000  .|.j............
+00000f30: 0000 0000 0000 0074 0800 0000 0000 0000  .......t........
+00000f40: 006a 0a00 0000 0000 0000 0000 0000 0000  .j..............
+00000f50: 0000 0000 006a 2000 0000 0000 0000 0000  .....j .........
+00000f60: 0000 0000 0000 0000 003c 0000 007c 006a  .........<...|.j
+00000f70: 1e00 0000 0000 0000 0000 0000 0000 0000  ................
+00000f80: 0000 006a 0200 0000 0000 0000 0000 0000  ...j............
+00000f90: 0000 0000 0000 006a 0400 0000 0000 0000  .......j........
+00000fa0: 0000 0000 0000 0000 0000 0064 0219 0000  ...........d....
+00000fb0: 007c 006a 0600 0000 0000 0000 0000 0000  .|.j............
+00000fc0: 0000 0000 0000 0074 0800 0000 0000 0000  .......t........
+00000fd0: 006a 0a00 0000 0000 0000 0000 0000 0000  .j..............
+00000fe0: 0000 0000 006a 2200 0000 0000 0000 0000  .....j".........
+00000ff0: 0000 0000 0000 0000 003c 0000 0074 1100  .........<...t..
+00001000: 0000 0000 0000 006a 1200 0000 0000 0000  .......j........
+00001010: 0000 0000 0000 0000 0000 007c 006a 1e00  ...........|.j..
+00001020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001030: 006a 0200 0000 0000 0000 0000 0000 0000  .j..............
+00001040: 0000 0000 006a 1400 0000 0000 0000 0000  .....j..........
+00001050: 0000 0000 0000 0000 00ab 0100 0000 0000  ................
+00001060: 007c 006a 0600 0000 0000 0000 0000 0000  .|.j............
+00001070: 0000 0000 0000 0074 0800 0000 0000 0000  .......t........
+00001080: 006a 0a00 0000 0000 0000 0000 0000 0000  .j..............
+00001090: 0000 0000 006a 2400 0000 0000 0000 0000  .....j$.........
+000010a0: 0000 0000 0000 0000 003c 0000 0074 2700  .........<...t'.
+000010b0: 0000 0000 0000 007c 006a 0000 0000 0000  .......|.j......
+000010c0: 0000 0000 0000 0000 0000 0000 006a 0200  .............j..
+000010d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000010e0: 006a 0400 0000 0000 0000 0000 0000 0000  .j..............
+000010f0: 0000 0000 007c 006a 1e00 0000 0000 0000  .....|.j........
+00001100: 0000 0000 0000 0000 0000 006a 0200 0000  ...........j....
+00001110: 0000 0000 0000 0000 0000 0000 0000 006a  ...............j
+00001120: 0400 0000 0000 0000 0000 0000 0000 0000  ................
+00001130: 0000 00ab 0200 0000 0000 007d 016e 7764  ...........}.nwd
+00001140: 017c 006a 0600 0000 0000 0000 0000 0000  .|.j............
+00001150: 0000 0000 0000 0074 0800 0000 0000 0000  .......t........
+00001160: 006a 0a00 0000 0000 0000 0000 0000 0000  .j..............
+00001170: 0000 0000 006a 2000 0000 0000 0000 0000  .....j .........
+00001180: 0000 0000 0000 0000 003c 0000 0064 017c  .........<...d.|
+00001190: 006a 0600 0000 0000 0000 0000 0000 0000  .j..............
+000011a0: 0000 0000 0074 0800 0000 0000 0000 006a  .....t.........j
+000011b0: 0a00 0000 0000 0000 0000 0000 0000 0000  ................
+000011c0: 0000 006a 2200 0000 0000 0000 0000 0000  ...j"...........
+000011d0: 0000 0000 0000 003c 0000 0064 017c 006a  .......<...d.|.j
+000011e0: 0600 0000 0000 0000 0000 0000 0000 0000  ................
+000011f0: 0000 0074 0800 0000 0000 0000 006a 0a00  ...t.........j..
+00001200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001210: 006a 2400 0000 0000 0000 0000 0000 0000  .j$.............
+00001220: 0000 0000 003c 0000 0064 027d 0174 2700  .....<...d.}.t'.
+00001230: 0000 0000 0000 007c 006a 0000 0000 0000  .......|.j......
+00001240: 0000 0000 0000 0000 0000 0000 006a 2800  .............j(.
+00001250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001260: 007c 006a 0000 0000 0000 0000 0000 0000  .|.j............
+00001270: 0000 0000 0000 006a 0200 0000 0000 0000  .......j........
+00001280: 0000 0000 0000 0000 0000 006a 0400 0000  ...........j....
+00001290: 0000 0000 0000 0000 0000 0000 0000 00ab  ................
+000012a0: 0200 0000 0000 007d 027c 027c 006a 0600  .......}.|.|.j..
+000012b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000012c0: 0074 0800 0000 0000 0000 006a 0a00 0000  .t.........j....
+000012d0: 0000 0000 0000 0000 0000 0000 0000 006a  ...............j
+000012e0: 2a00 0000 0000 0000 0000 0000 0000 0000  *...............
+000012f0: 0000 003c 0000 007c 017c 006a 0600 0000  ...<...|.|.j....
+00001300: 0000 0000 0000 0000 0000 0000 0000 0074  ...............t
+00001310: 0800 0000 0000 0000 006a 0a00 0000 0000  .........j......
+00001320: 0000 0000 0000 0000 0000 0000 006a 2c00  .............j,.
+00001330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001340: 003c 0000 007c 006a 0000 0000 0000 0000  .<...|.j........
+00001350: 0000 0000 0000 0000 0000 006a 2e00 0000  ...........j....
+00001360: 0000 0000 0000 0000 0000 0000 0000 007c  ...............|
+00001370: 006a 0600 0000 0000 0000 0000 0000 0000  .j..............
+00001380: 0000 0000 0074 0800 0000 0000 0000 006a  .....t.........j
+00001390: 0a00 0000 0000 0000 0000 0000 0000 0000  ................
+000013a0: 0000 006a 2e00 0000 0000 0000 0000 0000  ...j............
+000013b0: 0000 0000 0000 003c 0000 007c 006a 0000  .......<...|.j..
+000013c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000013d0: 006a 3000 0000 0000 0000 0000 0000 0000  .j0.............
+000013e0: 0000 0000 007c 006a 0600 0000 0000 0000  .....|.j........
+000013f0: 0000 0000 0000 0000 0000 0074 0800 0000  ...........t....
+00001400: 0000 0000 006a 0a00 0000 0000 0000 0000  .....j..........
+00001410: 0000 0000 0000 0000 006a 3200 0000 0000  .........j2.....
+00001420: 0000 0000 0000 0000 0000 0000 003c 0000  .............<..
+00001430: 007c 006a 0000 0000 0000 0000 0000 0000  .|.j............
+00001440: 0000 0000 0000 006a 3400 0000 0000 0000  .......j4.......
+00001450: 0000 0000 0000 0000 0000 007c 006a 0600  ...........|.j..
+00001460: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001470: 0074 0800 0000 0000 0000 006a 0a00 0000  .t.........j....
+00001480: 0000 0000 0000 0000 0000 0000 0000 006a  ...............j
+00001490: 3400 0000 0000 0000 0000 0000 0000 0000  4...............
+000014a0: 0000 003c 0000 007c 006a 0600 0000 0000  ...<...|.j......
+000014b0: 0000 0000 0000 0000 0000 0000 0053 0029  .............S.)
+000014c0: 034e 7209 0000 0072 0200 0000 291b 7231  .Nr....r....).r1
+000014d0: 0000 00da 0573 7461 7465 7229 0000 0072  .....stater)...r
+000014e0: 3400 0000 7206 0000 00da 0546 6965 6c64  4...r......Field
+000014f0: da06 7072 6579 5f78 da06 7072 6579 5f79  ..prey_x..prey_y
+00001500: da04 6d61 7468 da07 7261 6469 616e 7372  ..math..radiansr
+00001510: 2a00 0000 da0e 7072 6579 5f64 6972 6563  *.....prey_direc
+00001520: 7469 6f6e 7240 0000 00da 0a76 6973 6962  tionr@.....visib
+00001530: 696c 6974 79da 0d6c 696e 655f 6f66 5f73  ility..line_of_s
+00001540: 6967 6874 7227 0000 00da 0a70 7265 6461  ightr'.....preda
+00001550: 746f 725f 78da 0a70 7265 6461 746f 725f  tor_x..predator_
+00001560: 79da 1270 7265 6461 746f 725f 6469 7265  y..predator_dire
+00001570: 6374 696f 6e72 0d00 0000 722c 0000 00da  ctionr....r,....
+00001580: 0d67 6f61 6c5f 6469 7374 616e 6365 da11  .goal_distance..
+00001590: 7072 6564 6174 6f72 5f64 6973 7461 6e63  predator_distanc
+000015a0: 65da 0670 7566 6665 64da 0e70 7566 665f  e..puffed..puff_
+000015b0: 636f 6f6c 5f64 6f77 6eda 1070 7566 665f  cool_down..puff_
+000015c0: 636f 6f6c 6564 5f64 6f77 6eda 0866 696e  cooled_down..fin
+000015d0: 6973 6865 6429 0372 4700 0000 7257 0000  ished).rG...rW..
+000015e0: 0072 5600 0000 7303 0000 0020 2020 7215  .rV...s....   r.
+000015f0: 0000 00da 0f67 6574 5f6f 6273 6572 7661  .....get_observa
+00001600: 7469 6f6e 7a1b 456e 7669 726f 6e6d 656e  tionz.Environmen
+00001610: 742e 6765 745f 6f62 7365 7276 6174 696f  t.get_observatio
+00001620: 6e3d 0000 0073 d702 0000 8000 d83a 3ebf  n=...s.......:>.
+00001630: 29b9 29bf 2fb9 2fd7 3a52 d13a 52d0 5354  ).)././.:R.:R.ST
+00001640: d13a 5588 04d7 0818 d108 18d4 1929 d719  .:U..........)..
+00001650: 2fd1 192f d719 36d1 1936 d108 37d8 3a3e  /../..6..6..7.:>
+00001660: bf29 b929 bf2f b92f d73a 52d1 3a52 d053  .).)././.:R.:R.S
+00001670: 54d1 3a55 8804 d708 18d1 0818 d419 29d7  T.:U..........).
+00001680: 192f d119 2fd7 1936 d119 36d1 0837 dc42  ./../..6..6..7.B
+00001690: 46c7 2cc1 2cc8 74cf 79c9 79cf 7fc9 7fd7  F.,.,.t.y.y.....
+000016a0: 4f68 d14f 68d3 4269 8804 d708 18d1 0818  Oh.Oh.Bi........
+000016b0: d419 29d7 192f d119 2fd7 193e d119 3ed1  ..)../../..>..>.
+000016c0: 083f e00b 0f8f 3a89 3ad7 0b20 d10b 20d7  .?....:.:.. .. .
+000016d0: 0b2e d10b 2ea8 74af 79a9 79af 7fa9 7fd7  ......t.y.y.....
+000016e0: 2f47 d12f 47c8 14cf 1dc9 1dd7 495c d149  /G./G.......I\.I
+000016f0: 5cd7 4965 d149 65d5 0b66 d842 46c7 2dc1  \.Ie.Ie..f.BF.-.
+00001700: 2dd7 4255 d142 55d7 425e d142 5ed0 5f60  -.BU.BU.B^.B^._`
+00001710: d142 6188 44d7 0c1c d10c 1cd4 1d2d d71d  .Ba.D........-..
+00001720: 33d1 1d33 d71d 3ed1 1d3e d10c 3fd8 4246  3..3..>..>..?.BF
+00001730: c72d c12d d742 55d1 4255 d742 5ed1 425e  .-.-.BU.BU.B^.B^
+00001740: d05f 60d1 4261 8844 d70c 1cd1 0c1c d41d  ._`.Ba.D........
+00001750: 2dd7 1d33 d11d 33d7 1d3e d11d 3ed1 0c3f  -..3..3..>..>..?
+00001760: dc4a 4ecf 2cc9 2cd8 1014 970d 910d d710  .JN.,.,.........
+00001770: 23d1 1023 d710 2dd1 102d f303 014b 012f  #..#..-..-...K./
+00001780: 8844 d70c 1cd1 0c1c d41d 2dd7 1d33 d11d  .D........-..3..
+00001790: 33d7 1d46 d11d 46d1 0c47 e420 28a8 14af  3..F..F..G. (...
+000017a0: 19a9 19af 1fa9 1fd7 2941 d129 41c0 34c7  ........)A.)A.4.
+000017b0: 3dc1 3dd7 4356 d143 56d7 435f d143 5fd3  =.=.CV.CV.C_.C_.
+000017c0: 2060 d10c 1de0 4243 8844 d70c 1cd1 0c1c   `....BC.D......
+000017d0: d41d 2dd7 1d33 d11d 33d7 1d3e d11d 3ed1  ..-..3..3..>..>.
+000017e0: 0c3f d842 4388 44d7 0c1c d10c 1cd4 1d2d  .?.BC.D........-
+000017f0: d71d 33d1 1d33 d71d 3ed1 1d3e d10c 3fd8  ..3..3..>..>..?.
+00001800: 4a4b 8844 d70c 1cd1 0c1c d41d 2dd7 1d33  JK.D........-..3
+00001810: d11d 33d7 1d46 d11d 46d1 0c47 d820 21d0  ..3..F..F..G. !.
+00001820: 0c1d e418 20a0 14a7 19a1 19d7 2138 d121  .... .......!8.!
+00001830: 38b8 24bf 29b9 29bf 2fb9 2fd7 3a52 d13a  8.$.).)././.:R.:
+00001840: 52d3 1853 880d d841 4e88 04d7 0818 d108  R..S...AN.......
+00001850: 18d4 1929 d719 2fd1 192f d719 3dd1 193d  ...)../../..=..=
+00001860: d108 3ed8 4556 8804 d708 18d1 0818 d419  ..>.EV..........
+00001870: 29d7 192f d119 2fd7 1941 d119 41d1 0842  )../../..A..A..B
+00001880: d83a 3ebf 29b9 29d7 3a4a d13a 4a88 04d7  .:>.).).:J.:J...
+00001890: 0818 d108 18d4 1929 d719 2fd1 192f d719  .......)../../..
+000018a0: 36d1 1936 d108 37d8 4448 c749 c149 d744  6..6..7.DH.I.I.D
+000018b0: 5cd1 445c 8804 d708 18d1 0818 d419 29d7  \.D\..........).
+000018c0: 192f d119 2fd7 1940 d119 40d1 0841 d83c  ./../..@..@..A.<
+000018d0: 40bf 49b9 49d7 3c4e d13c 4e88 04d7 0818  @.I.I.<N.<N.....
+000018e0: d108 18d4 1929 d719 2fd1 192f d719 38d1  .....)../../..8.
+000018f0: 1938 d108 39d8 0f13 d70f 1fd1 0f1f d008  .8..9...........
+00001900: 1f72 1700 0000 da06 6163 7469 6f6e 6302  .r......actionc.
+00001910: 0000 0000 0000 0000 0000 0003 0000 0003  ................
+00001920: 0000 00f3 3a00 0000 9700 7c00 6a00 0000  ....:.....|.j...
+00001930: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001940: 6a03 0000 0000 0000 0000 0000 0000 0000  j...............
+00001950: 0000 0000 7c01 ab01 0000 0000 0000 0100  ....|...........
+00001960: 7900 a901 4e29 0272 3100 0000 da0a 7365  y...N).r1.....se
+00001970: 745f 6163 7469 6f6e 2902 7247 0000 0072  t_action).rG...r
+00001980: 5d00 0000 7302 0000 0020 2072 1500 0000  ]...s....  r....
+00001990: 7260 0000 007a 1645 6e76 6972 6f6e 6d65  r`...z.Environme
+000019a0: 6e74 2e73 6574 5f61 6374 696f 6e56 0000  nt.set_actionV..
+000019b0: 0073 1400 0000 8000 d808 0c8f 0989 09d7  .s..............
+000019c0: 081c d108 1c98 56d5 0824 7217 0000 0063  ......V..$r....c
+000019d0: 0200 0000 0000 0000 0000 0000 0800 0000  ................
+000019e0: 0300 0000 f3c8 0200 0097 007c 0078 016a  ...........|.x.j
+000019f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001a00: 0000 0064 017a 0d00 0063 025f 0000 0000  ...d.z...c._....
+00001a10: 0000 0000 007c 006a 0300 0000 0000 0000  .....|.j........
+00001a20: 0000 0000 0000 0000 0000 007c 01ac 02ab  ...........|....
+00001a30: 0100 0000 0000 0001 0074 0500 0000 0000  .........t......
+00001a40: 0000 007c 006a 0600 0000 0000 0000 0000  ...|.j..........
+00001a50: 0000 0000 0000 0000 00ab 0100 0000 0000  ................
+00001a60: 0044 005d 3900 007d 027c 006a 0800 0000  .D.]9..}.|.j....
+00001a70: 0000 0000 0000 0000 0000 0000 0000 006a  ...............j
+00001a80: 0b00 0000 0000 0000 0000 0000 0000 0000  ................
+00001a90: 0000 00ab 0000 0000 0000 0001 007c 006a  .............|.j
+00001aa0: 0c00 0000 0000 0000 0000 0000 0000 0000  ................
+00001ab0: 0000 0073 018c 2a7c 006a 0f00 0000 0000  ...s..*|.j......
+00001ac0: 0000 0000 0000 0000 0000 0000 00ab 0000  ................
+00001ad0: 0000 0000 0001 008c 3b04 007c 006a 0000  ........;..|.j..
+00001ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001af0: 007c 006a 1000 0000 0000 0000 0000 0000  .|.j............
+00001b00: 0000 0000 0000 006b 5c00 007d 037c 006a  .......k\..}.|.j
+00001b10: 1300 0000 0000 0000 0000 0000 0000 0000  ................
+00001b20: 0000 00ab 0000 0000 0000 007d 047c 006a  ...........}.|.j
+00001b30: 1500 0000 0000 0000 0000 0000 0000 0000  ................
+00001b40: 0000 007c 04ab 0100 0000 0000 007d 057c  ...|.........}.|
+00001b50: 006a 1600 0000 0000 0000 0000 0000 0000  .j..............
+00001b60: 0000 0000 006a 1800 0000 0000 0000 0000  .....j..........
+00001b70: 0000 0000 0000 0000 0072 2964 017d 067c  .........r)d.}.|
+00001b80: 0078 016a 1a00 0000 0000 0000 0000 0000  .x.j............
+00001b90: 0000 0000 0000 0064 017a 0d00 0063 025f  .......d.z...c._
+00001ba0: 0d00 0000 0000 0000 0064 037c 006a 1600  .........d.|.j..
+00001bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001bc0: 005f 0c00 0000 0000 0000 006e 0264 047d  ._.........n.d.}
+00001bd0: 067c 047c 057c 006a 1600 0000 0000 0000  .|.|.|.j........
+00001be0: 0000 0000 0000 0000 0000 006a 1c00 0000  ...........j....
+00001bf0: 0000 0000 0000 0000 0000 0000 0000 007c  ...............|
+00001c00: 037c 067c 006a 1600 0000 0000 0000 0000  .|.|.j..........
+00001c10: 0000 0000 0000 0000 006a 1c00 0000 0000  .........j......
+00001c20: 0000 0000 0000 0000 0000 0000 0072 117c  .............r.|
+00001c30: 006a 1a00 0000 0000 0000 0000 0000 0000  .j..............
+00001c40: 0000 0000 0064 046b 2800 0072 0264 016e  .....d.k(..r.d.n
+00001c50: 0164 047c 006a 1600 0000 0000 0000 0000  .d.|.j..........
+00001c60: 0000 0000 0000 0000 006a 1c00 0000 0000  .........j......
+00001c70: 0000 0000 0000 0000 0000 0000 0072 147c  .............r.|
+00001c80: 006a 1a00 0000 0000 0000 0000 0000 0000  .j..............
+00001c90: 0000 0000 0064 046b 2800 0072 0564 0164  .....d.k(..r.d.d
+00001ca0: 059c 0366 0553 0064 0464 059c 0366 0553  ...f.S.d.d...f.S
+00001cb0: 0029 064e 7202 0000 0029 0172 5d00 0000  .).Nr....).r]...
+00001cc0: 4672 0900 0000 2903 da07 6361 7074 7572  Fr....)...captur
+00001cd0: 65da 0a69 735f 7375 6363 6573 73da 0873  e..is_success..s
+00001ce0: 7572 7669 7665 6429 0f72 4500 0000 7260  urvived).rE...r`
+00001cf0: 0000 00da 0572 616e 6765 721d 0000 0072  .....ranger....r
+00001d00: 4000 0000 da04 7374 6570 7244 0000 00da  @.....steprD....
+00001d10: 0672 656e 6465 7272 1c00 0000 725c 0000  .renderr....r\..
+00001d20: 0072 3200 0000 7231 0000 0072 5800 0000  .r2...r1...rX...
+00001d30: 7246 0000 0072 5b00 0000 2907 7247 0000  rF...r[...).rG..
+00001d40: 0072 5d00 0000 da01 69da 0974 7275 6e63  .r].....i..trunc
+00001d50: 6174 6564 da03 6f62 73da 0672 6577 6172  ated..obs..rewar
+00001d60: 6472 6200 0000 7307 0000 0020 2020 2020  drb...s....     
+00001d70: 2020 7215 0000 0072 6600 0000 7a10 456e    r....rf...z.En
+00001d80: 7669 726f 6e6d 656e 742e 7374 6570 5900  vironment.stepY.
+00001d90: 0000 7334 0100 0080 00d8 080c 8f0f 8a0f  ..s4............
+00001da0: 9831 d108 1c8d 0fd8 080c 8f0f 890f 9876  .1.............v
+00001db0: 880f d408 26dc 1116 9074 977e 917e d311  ....&....t.~.~..
+00001dc0: 26f2 0003 091e 8841 d80c 108f 4a89 4a8f  &......A....J.J.
+00001dd0: 4f89 4fd4 0c1d d80f 13d7 0f20 d30f 20d8  O.O........ .. .
+00001de0: 1014 970b 910b 950d f007 0309 1ef0 0800  ................
+00001df0: 161a 975f 915f a804 af0d a90d d115 3588  ..._._........5.
+00001e00: 09d8 0e12 d70e 22d1 0e22 d30e 2488 03d8  ......".."..$...
+00001e10: 1115 d711 25d1 1125 a063 d311 2a88 06d8  ....%..%.c..*...
+00001e20: 0b0f 8f39 8939 d70b 1bd2 0b1b d816 1788  ...9.9..........
+00001e30: 47d8 0c10 8f4d 8a4d 9851 d10c 1e8d 4dd8  G....M.M.Q....M.
+00001e40: 1f24 8844 8f49 8949 d50c 1ce0 1617 8847  .$.D.I.I.......G
+00001e50: d80f 1290 4698 449f 4999 49d7 1c2e d11c  ....F.D.I.I.....
+00001e60: 2eb0 09c0 77d8 4f53 cf79 c979 d74f 61d2  ....w.OS.y.y.Oa.
+00001e70: 4f61 d066 6ad7 6673 d166 73d0 7778 d266  Oa.fj.fs.fs.wx.f
+00001e80: 78c9 21d0 7e7f d84d 51cf 59c9 59d7 4d5f  x.!.~..MQ.Y.Y.M_
+00001e90: d24d 5fd0 6468 d764 71d1 6471 d075 76d2  .M_.dh.dq.dq.uv.
+00001ea0: 6476 c801 f105 023c 7f01 f000 0210 7f01  dv.....<........
+00001eb0: f000 0209 7f01 e07c 7df1 0502 3c7f 01f0  .......|}...<...
+00001ec0: 0002 107f 01f0 0002 097f 0172 1700 0000  ...........r....
+00001ed0: 4e63 0200 0000 0000 0000 0000 0000 0200  Nc..............
+00001ee0: 0000 0300 0000 f37a 0000 0097 0064 017c  .......z.....d.|
+00001ef0: 005f 0000 0000 0000 0000 0064 017c 005f  ._.........d.|._
+00001f00: 0100 0000 0000 0000 007c 006a 0400 0000  .........|.j....
+00001f10: 0000 0000 0000 0000 0000 0000 0000 006a  ...............j
+00001f20: 0700 0000 0000 0000 0000 0000 0000 0000  ................
+00001f30: 0000 00ab 0000 0000 0000 0001 007c 006a  .............|.j
+00001f40: 0900 0000 0000 0000 0000 0000 0000 0000  ................
+00001f50: 0000 00ab 0000 0000 0000 007d 027c 0269  ...........}.|.i
+00001f60: 0066 0253 0072 1200 0000 2905 7246 0000  .f.S.r....).rF..
+00001f70: 0072 4500 0000 7240 0000 00da 0572 6573  .rE...r@.....res
+00001f80: 6574 725c 0000 0029 0372 4700 0000 da04  etr\...).rG.....
+00001f90: 7365 6564 726a 0000 0073 0300 0000 2020  seedrj...s....  
+00001fa0: 2072 1500 0000 726d 0000 007a 1145 6e76   r....rm...z.Env
+00001fb0: 6972 6f6e 6d65 6e74 2e72 6573 6574 6d00  ironment.resetm.
+00001fc0: 0000 7337 0000 0080 00d8 1819 8804 8c0d  ..s7............
+00001fd0: d81a 1b88 048c 0fd8 080c 8f0a 890a d708  ................
+00001fe0: 18d1 0818 d408 1ad8 0e12 d70e 22d1 0e22  ............".."
+00001ff0: d30e 2488 03d8 0f12 9042 8877 880e 7217  ..$......B.w..r.
+00002000: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00002010: 0300 0000 0300 0000 f386 0000 0097 007c  ...............|
+00002020: 006a 0000 0000 0000 0000 0000 0000 0000  .j..............
+00002030: 0000 0000 0080 1b74 0300 0000 0000 0000  .......t........
+00002040: 007c 006a 0400 0000 0000 0000 0000 0000  .|.j............
+00002050: 0000 0000 0000 00ac 01ab 0100 0000 0000  ................
+00002060: 007c 005f 0000 0000 0000 0000 007c 006a  .|._.........|.j
+00002070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002080: 0000 006a 0700 0000 0000 0000 0000 0000  ...j............
+00002090: 0000 0000 0000 00ab 0000 0000 0000 0001  ................
+000020a0: 0079 0029 024e 2901 7240 0000 0029 0472  .y.).N).r@...).r
+000020b0: 4300 0000 7208 0000 0072 4000 0000 da04  C...r....r@.....
+000020c0: 6472 6177 2901 7247 0000 0073 0100 0000  draw).rG...s....
+000020d0: 2072 1500 0000 7267 0000 007a 1245 6e76   r....rg...z.Env
+000020e0: 6972 6f6e 6d65 6e74 2e72 656e 6465 7274  ironment.rendert
+000020f0: 0000 0073 2a00 0000 8000 d80b 0f8f 3989  ...s*.........9.
+00002100: 39d0 0b1c dc18 1ca0 34a7 3aa1 3ad4 182e  9.......4.:.:...
+00002110: 8844 8c49 d808 0c8f 0989 098f 0e89 0ed5  .D.I............
+00002120: 0818 7217 0000 0072 5f00 0000 290c da08  ..r....r_...)...
+00002130: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00002140: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00002150: 5f5f da03 7374 72da 0462 6f6f 6cda 0369  __..str..bool..i
+00002160: 6e74 7248 0000 0072 5c00 0000 7260 0000  ntrH...r\...r`..
+00002170: 0072 6600 0000 726d 0000 0072 6700 0000  .rf...rm...rg...
+00002180: 7213 0000 0072 1700 0000 7215 0000 0072  r....r....r....r
+00002190: 0f00 0000 720f 0000 000e 0000 0073 6a00  ....r........sj.
+000021a0: 0000 8400 f00a 0022 25d9 212c d822 23f1  ......."%.!,."#.
+000021b0: 0d2c 051a d81d 20f0 032c 051a e01c 20f0  .,.... ..,.... .
+000021c0: 052c 051a f006 0020 24f0 072c 051a f008  .,..... $..,....
+000021d0: 001c 1ff0 092c 051a f00c 001d 20f3 0d2c  .....,...... ..,
+000021e0: 051a f25c 0117 0520 f032 0105 25a0 13f3  ...\... .2..%...
+000021f0: 0001 0525 f006 1205 7f01 9833 f300 1205  ...%.......3....
+00002200: 7f01 f328 0505 17f3 0e03 0519 7217 0000  ...(........r...
+00002210: 0072 0f00 0000 2916 7240 0000 0072 0300  .r....).r@...r..
+00002220: 0000 da05 726f 626f 7472 0400 0000 da05  ....robotr......
+00002230: 6d6f 7573 6572 0500 0000 7206 0000 00da  mouser....r.....
+00002240: 0561 6765 6e74 7207 0000 0072 4300 0000  .agentr....rC...
+00002250: 7208 0000 00da 0967 796d 6e61 7369 756d  r......gymnasium
+00002260: 720a 0000 0072 0b00 0000 da10 6365 6c6c  r....r......cell
+00002270: 776f 726c 645f 6c6f 6164 6572 720c 0000  world_loaderr...
+00002280: 00da 056e 756d 7079 7236 0000 00da 0475  ...numpyr6.....u
+00002290: 7469 6c72 0d00 0000 724e 0000 0072 0f00  tilr....rN...r..
+000022a0: 0000 7213 0000 0072 1700 0000 7215 0000  ..r....r....r...
+000022b0: 00fa 083c 6d6f 6475 6c65 3e72 7e00 0000  ...<module>r~...
+000022c0: 0100 0000 7334 0000 00f0 0301 0101 dd00  ....s4..........
+000022d0: 18dd 0018 df00 2add 001d dd00 16dd 0019  ......*.........
+000022e0: dd00 1cdd 002d db00 12dd 001a db00 0bf4  .....-..........
+000022f0: 0669 0101 1990 23f5 0069 0101 1972 1700  .i....#..i...r..
+00002300: 0000                                     ..
```

### Comparing `cellworld_game-0.0.61/cellworld_game/tasks/botevade.py` & `cellworld_game-0.0.68/cellworld_game/tasks/botevade.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-import random
-from ..util import distance
-from ..model import Model
-from ..agent import AgentState, CoordinateConverter
-from ..mouse import Mouse
-from ..robot import Robot
-from ..cellworld_loader import CellWorldLoader
-
-
-class BotEvade(Model):
-    def __init__(self,
-                 world_name: str = "21_05",
-                 use_predator: bool = True,
-                 puff_cool_down_time: float = .5,
-                 puff_threshold: float = .1,
-                 goal_location=(1.0, 0.5),
-                 goal_threshold: float = .1,
-                 time_step: float = .025,
-                 real_time: bool = False,
-                 render: bool = False):
-        self.use_predator = use_predator
-        self.puff_cool_down_time = puff_cool_down_time
-        self.puff_threshold = puff_threshold
-        self.goal_location = goal_location
-        self.goal_threshold = goal_threshold
-        self.render = render
-        self.loader = CellWorldLoader(world_name=world_name)
-
-        Model.__init__(self,
-                       arena=self.loader.arena,
-                       occlusions=self.loader.occlusions,
-                       time_step=time_step,
-                       real_time=real_time)
-
-        if use_predator:
-            self.predator = Robot(start_locations=self.loader.robot_start_locations,
-                                  open_locations=self.loader.open_locations,
-                                  navigation=self.loader.navigation)
-
-            self.add_agent("predator", self.predator)
-
-        self.prey = Mouse(start_state=AgentState(location=(.05, .5),
-                                                 direction=0),
-                          navigation=self.loader.navigation)
-
-        self.add_agent("prey", self.prey)
-
-        self.running = False
-
-        if self.render:
-            from ..view import View
-            self.view = View(model=self)
-            self.view.on_quit = self.__on_quit__
-
-            if use_predator:
-                import pygame
-
-                def render_puff_area(surface: pygame.Surface,
-                                     coordinate_converter: CoordinateConverter):
-                    predator_location = coordinate_converter.from_canonical(self.predator.state.location)
-                    puff_area_size = self.puff_threshold * coordinate_converter.screen_width
-                    puff_location = predator_location[0] - puff_area_size, predator_location[1] - puff_area_size
-                    puff_area_surface = pygame.Surface((puff_area_size * 2, puff_area_size * 2), pygame.SRCALPHA)
-                    puff_area_color = (255, 0, 0, 60) if self.puff_cool_down > 0 else (0, 0, 255, 60)
-                    pygame.draw.circle(puff_area_surface,
-                                       color=puff_area_color,
-                                       center=(puff_area_size, puff_area_size),
-                                       radius=puff_area_size)
-                    surface.blit(puff_area_surface,
-                                 puff_location)
-                    pygame.draw.circle(surface=surface,
-                                       color=(0, 0, 255),
-                                       center=predator_location,
-                                       radius=puff_area_size,
-                                       width=2)
-
-                self.view.add_render_step(render_puff_area)
-
-        self.puffed: bool = False
-        self.puff_cool_down: float = 0
-        self.goal_achieved: bool = False
-        self.predator_prey_distance: float = 1
-        self.prey_goal_distance: float = 0
-        self.puff_count = 0
-        self.predator_visible = False
-
-    def __update_state__(self,
-                         delta_t: float = 0):
-        if self.use_predator and self.puff_cool_down <= 0:
-            self.predator_prey_distance = distance(self.prey.state.location,
-                                                   self.predator.state.location)
-            self.predator_visible = self.visibility.line_of_sight(self.prey.state.location, self.predator.state.location)
-            if self.predator_visible:
-                if self.predator_prey_distance <= self.puff_threshold:
-                    self.puffed = True
-                    self.puff_count += 1
-                    self.puff_cool_down = self.puff_cool_down_time
-
-                self.predator.set_destination(self.prey.state.location)
-
-            if not self.predator.path:
-                self.predator.set_destination(random.choice(self.loader.open_locations))
-
-        if delta_t < self.puff_cool_down:
-            self.puff_cool_down -= delta_t
-        else:
-            self.puff_cool_down = 0
-
-        self.prey_goal_distance = distance(self.goal_location, self.prey.state.location)
-
-        if self.prey_goal_distance <= self.goal_threshold:
-            self.goal_achieved = True
-            self.running = False
-
-    def __on_quit__(self):
-        self.running = False
-
-    def reset(self):
-        Model.reset(self)
-        self.goal_achieved = False
-        self.predator_visible = False
-        self.puff_count = 0
-        self.__update_state__()
-
-    def step(self) -> float:
-        delta_t = Model.step(self)
-        if self.render:
-            self.view.draw()
-        self.__update_state__(delta_t=delta_t)
+import random
+from ..util import distance
+from ..model import Model
+from ..agent import AgentState, CoordinateConverter
+from ..mouse import Mouse
+from ..robot import Robot
+from ..cellworld_loader import CellWorldLoader
+
+
+class BotEvade(Model):
+    def __init__(self,
+                 world_name: str = "21_05",
+                 use_predator: bool = True,
+                 puff_cool_down_time: float = .5,
+                 puff_threshold: float = .1,
+                 goal_location=(1.0, 0.5),
+                 goal_threshold: float = .1,
+                 time_step: float = .025,
+                 real_time: bool = False,
+                 render: bool = False):
+        self.use_predator = use_predator
+        self.puff_cool_down_time = puff_cool_down_time
+        self.puff_threshold = puff_threshold
+        self.goal_location = goal_location
+        self.goal_threshold = goal_threshold
+        self.render = render
+        self.loader = CellWorldLoader(world_name=world_name)
+
+        Model.__init__(self,
+                       arena=self.loader.arena,
+                       occlusions=self.loader.occlusions,
+                       time_step=time_step,
+                       real_time=real_time)
+
+        if use_predator:
+            self.predator = Robot(start_locations=self.loader.robot_start_locations,
+                                  open_locations=self.loader.open_locations,
+                                  navigation=self.loader.navigation)
+
+            self.add_agent("predator", self.predator)
+
+        self.prey = Mouse(start_state=AgentState(location=(.05, .5),
+                                                 direction=0),
+                          navigation=self.loader.navigation)
+
+        self.add_agent("prey", self.prey)
+
+        self.running = False
+
+        if self.render:
+            from ..view import View
+            self.view = View(model=self)
+            self.view.on_quit = self.__on_quit__
+
+            if use_predator:
+                import pygame
+
+                def render_puff_area(surface: pygame.Surface,
+                                     coordinate_converter: CoordinateConverter):
+                    predator_location = coordinate_converter.from_canonical(self.predator.state.location)
+                    puff_area_size = self.puff_threshold * coordinate_converter.screen_width
+                    puff_location = predator_location[0] - puff_area_size, predator_location[1] - puff_area_size
+                    puff_area_surface = pygame.Surface((puff_area_size * 2, puff_area_size * 2), pygame.SRCALPHA)
+                    puff_area_color = (255, 0, 0, 60) if self.puff_cool_down > 0 else (0, 0, 255, 60)
+                    pygame.draw.circle(puff_area_surface,
+                                       color=puff_area_color,
+                                       center=(puff_area_size, puff_area_size),
+                                       radius=puff_area_size)
+                    surface.blit(puff_area_surface,
+                                 puff_location)
+                    pygame.draw.circle(surface=surface,
+                                       color=(0, 0, 255),
+                                       center=predator_location,
+                                       radius=puff_area_size,
+                                       width=2)
+
+                self.view.add_render_step(render_puff_area)
+
+        self.puffed: bool = False
+        self.puff_cool_down: float = 0
+        self.goal_achieved: bool = False
+        self.predator_prey_distance: float = 1
+        self.prey_goal_distance: float = 0
+        self.puff_count = 0
+        self.predator_visible = False
+
+    def __update_state__(self,
+                         delta_t: float = 0):
+        if self.use_predator and self.puff_cool_down <= 0:
+            self.predator_prey_distance = distance(self.prey.state.location,
+                                                   self.predator.state.location)
+            self.predator_visible = self.visibility.line_of_sight(self.prey.state.location, self.predator.state.location)
+            if self.predator_visible:
+                if self.predator_prey_distance <= self.puff_threshold:
+                    self.puffed = True
+                    self.puff_count += 1
+                    self.puff_cool_down = self.puff_cool_down_time
+
+                self.predator.set_destination(self.prey.state.location)
+
+            if not self.predator.path:
+                self.predator.set_destination(random.choice(self.loader.open_locations))
+
+        if delta_t < self.puff_cool_down:
+            self.puff_cool_down -= delta_t
+        else:
+            self.puff_cool_down = 0
+
+        self.prey_goal_distance = distance(self.goal_location, self.prey.state.location)
+
+        if self.prey_goal_distance <= self.goal_threshold:
+            self.goal_achieved = True
+            self.running = False
+
+    def __on_quit__(self):
+        self.stop()
+
+    def reset(self):
+        Model.reset(self)
+        self.goal_achieved = False
+        self.predator_visible = False
+        self.puff_count = 0
+        self.__update_state__()
+
+    def step(self) -> float:
+        delta_t = Model.step(self)
+        if self.render:
+            self.view.draw()
+        self.__update_state__(delta_t=delta_t)
         return delta_t
```

### Comparing `cellworld_game-0.0.61/cellworld_game/tasks/dualevade.py` & `cellworld_game-0.0.68/cellworld_game/tasks/dualevade.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,181 +1,179 @@
-import random
-from ..util import distance
-from ..model import Model
-from ..agent import AgentState, CoordinateConverter
-from ..mouse import Mouse
-from ..robot import Robot
-from ..cellworld_loader import CellWorldLoader
-
-
-class DualEvadePreyData:
-    def __init__(self):
-        self.puffed = False
-        self.goal_achieved = False
-        self.predator_visible = False
-        self.predator_prey_distance = 1
-        self.prey_goal_distance = 0
-        self.puff_count = 0
-
-    def reset(self):
-        self.puffed = False
-        self.goal_achieved = False
-        self.predator_visible = False
-        self.predator_prey_distance = 1
-        self.prey_goal_distance = 0
-        self.puff_count = 0
-
-
-class DualEvade(Model):
-    def __init__(self,
-                 world_name: str = "21_05",
-                 use_predator: bool = True,
-                 puff_cool_down_time: float = .5,
-                 puff_threshold: float = .1,
-                 goal_location=(1.0, 0.5),
-                 goal_threshold: float = .1,
-                 time_step: float = .025,
-                 real_time: bool = False,
-                 render: bool = False):
-        self.use_predator = use_predator
-        self.puff_cool_down_time = puff_cool_down_time
-        self.puff_threshold = puff_threshold
-        self.goal_location = goal_location
-        self.goal_threshold = goal_threshold
-        self.render = render
-        self.loader = CellWorldLoader(world_name=world_name)
-
-        Model.__init__(self,
-                       arena=self.loader.arena,
-                       occlusions=self.loader.occlusions,
-                       time_step=time_step,
-                       real_time=real_time)
-
-        if use_predator:
-            self.predator = Robot(start_locations=self.loader.robot_start_locations,
-                                  open_locations=self.loader.open_locations,
-                                  navigation=self.loader.navigation)
-
-            self.add_agent("predator", self.predator)
-
-        self.prey_1 = Mouse(start_state=AgentState(location=(.05, .5),
-                                                   direction=0),
-                            navigation=self.loader.navigation)
-
-        self.add_agent("prey_1", self.prey_1)
-
-        self.prey_2 = Mouse(start_state=AgentState(location=(.05, .5),
-                                                   direction=0),
-                            navigation=self.loader.navigation)
-
-        self.add_agent("prey_2", self.prey_2)
-
-        self.running = False
-
-        if self.render:
-            from ..view import View
-            self.view = View(model=self)
-            self.view.on_quit = self.__on_quit__
-
-            if use_predator:
-                import pygame
-
-                def render_puff_area(surface: pygame.Surface,
-                                     coordinate_converter: CoordinateConverter):
-                    predator_location = coordinate_converter.from_canonical(self.predator.state.location)
-                    puff_area_size = self.puff_threshold * coordinate_converter.screen_width
-                    puff_location = predator_location[0] - puff_area_size, predator_location[1] - puff_area_size
-                    puff_area_surface = pygame.Surface((puff_area_size * 2, puff_area_size * 2), pygame.SRCALPHA)
-                    puff_area_color = (255, 0, 0, 60) if self.puff_cool_down > 0 else (0, 0, 255, 60)
-                    pygame.draw.circle(puff_area_surface,
-                                       color=puff_area_color,
-                                       center=(puff_area_size, puff_area_size),
-                                       radius=puff_area_size)
-                    surface.blit(puff_area_surface,
-                                 puff_location)
-                    pygame.draw.circle(surface=surface,
-                                       color=(0, 0, 255),
-                                       center=predator_location,
-                                       radius=puff_area_size,
-                                       width=2)
-
-                self.view.add_render_step(render_puff_area)
-
-        self.puff_cool_down: float = 0
-        self.prey_data_1 = DualEvadePreyData()
-        self.prey_data_2 = DualEvadePreyData()
-
-    def __update_state__(self,
-                         delta_t: float = 0):
-        self.mouse_visible = self.visibility.line_of_sight(self.prey_1.state.location, self.prey_2.state.location)
-        if self.use_predator and self.puff_cool_down <= 0:
-            self.prey_data_1.predator_prey_distance = distance(self.prey_1.state.location,
-                                                               self.predator.state.location)
-            self.prey_data_1.predator_visible = self.prey_1.visible and self.visibility.line_of_sight(self.prey_1.state.location, self.predator.state.location)
-            if self.prey_data_1.predator_visible:
-                if self.prey_data_1.predator_prey_distance <= self.puff_threshold:
-                    self.prey_data_1.puffed = True
-                    self.prey_data_1.puff_count += 1
-                    self.puff_cool_down = self.puff_cool_down_time
-
-            self.prey_data_2.predator_prey_distance = distance(self.prey_2.state.location,
-                                                               self.predator.state.location)
-
-            self.prey_data_2.predator_visible = self.prey_2.visible and self.visibility.line_of_sight(self.prey_2.state.location, self.predator.state.location)
-            if self.prey_data_2.predator_visible:
-                if self.prey_data_2.predator_prey_distance <= self.puff_threshold:
-                    self.prey_data_2.puffed = True
-                    self.prey_data_2.puff_count += 1
-                    self.puff_cool_down = self.puff_cool_down_time
-
-            closest_visible_prey_location = None
-            if self.prey_data_1.predator_visible:
-                closest_visible_prey_location = self.prey_1.state.location
-
-            if self.prey_data_2.predator_visible:
-                if closest_visible_prey_location:
-                    if self.prey_data_2.predator_prey_distance <= self.prey_data_1.predator_prey_distance:
-                        closest_visible_prey_location = self.prey_2.state.location
-                else:
-                    closest_visible_prey_location = self.prey_2.state.location
-
-            if closest_visible_prey_location:
-                self.predator.set_destination(self.prey_2.state.location)
-
-            if not self.predator.path:
-                self.predator.set_destination(random.choice(self.loader.open_locations))
-
-        if delta_t < self.puff_cool_down:
-            self.puff_cool_down -= delta_t
-        else:
-            self.puff_cool_down = 0
-
-        self.prey_data_1.prey_goal_distance = distance(self.goal_location, self.prey_1.state.location)
-        if self.prey_data_1.prey_goal_distance <= self.goal_threshold:
-            self.prey_data_1.goal_achieved = True
-            self.prey_1.visible = False
-
-        self.prey_data_2.prey_goal_distance = distance(self.goal_location, self.prey_2.state.location)
-        if self.prey_data_2.prey_goal_distance <= self.goal_threshold:
-            self.prey_data_2.goal_achieved = True
-            self.prey_2.visible = False
-
-        if self.prey_data_1.goal_achieved and self.prey_data_2.goal_achieved:
-            self.running = False
-
-    def __on_quit__(self):
-        self.running = False
-
-    def reset(self):
-        self.prey_data_1.reset()
-        self.prey_data_2.reset()
-        self.prey_1.visible = True
-        self.prey_2.visible = True
-        Model.reset(self)
-        self.__update_state__()
-
-    def step(self) -> float:
-        delta_t = Model.step(self)
-        if self.render:
-            self.view.draw()
-        self.__update_state__(delta_t=delta_t)
+import random
+from ..util import distance
+from ..model import Model
+from ..agent import AgentState, CoordinateConverter
+from ..mouse import Mouse
+from ..robot import Robot
+from ..cellworld_loader import CellWorldLoader
+
+
+class DualEvadePreyData:
+    def __init__(self):
+        self.puffed = False
+        self.goal_achieved = False
+        self.predator_visible = False
+        self.predator_prey_distance = 1
+        self.prey_goal_distance = 0
+        self.puff_count = 0
+
+    def reset(self):
+        self.puffed = False
+        self.goal_achieved = False
+        self.predator_visible = False
+        self.predator_prey_distance = 1
+        self.prey_goal_distance = 0
+        self.puff_count = 0
+
+
+class DualEvade(Model):
+    def __init__(self,
+                 world_name: str = "21_05",
+                 use_predator: bool = True,
+                 puff_cool_down_time: float = .5,
+                 puff_threshold: float = .1,
+                 goal_location=(1.0, 0.5),
+                 goal_threshold: float = .1,
+                 time_step: float = .025,
+                 real_time: bool = False,
+                 render: bool = False):
+        self.use_predator = use_predator
+        self.puff_cool_down_time = puff_cool_down_time
+        self.puff_threshold = puff_threshold
+        self.goal_location = goal_location
+        self.goal_threshold = goal_threshold
+        self.render = render
+        self.loader = CellWorldLoader(world_name=world_name)
+
+        Model.__init__(self,
+                       arena=self.loader.arena,
+                       occlusions=self.loader.occlusions,
+                       time_step=time_step,
+                       real_time=real_time)
+
+        if use_predator:
+            self.predator = Robot(start_locations=self.loader.robot_start_locations,
+                                  open_locations=self.loader.open_locations,
+                                  navigation=self.loader.navigation)
+
+            self.add_agent("predator", self.predator)
+
+        self.prey_1 = Mouse(start_state=AgentState(location=(.05, .5),
+                                                   direction=0),
+                            navigation=self.loader.navigation)
+
+        self.add_agent("prey_1", self.prey_1)
+
+        self.prey_2 = Mouse(start_state=AgentState(location=(.05, .5),
+                                                   direction=0),
+                            navigation=self.loader.navigation)
+
+        self.add_agent("prey_2", self.prey_2)
+
+        if self.render:
+            from ..view import View
+            self.view = View(model=self)
+            self.view.on_quit = self.__on_quit__
+
+            if use_predator:
+                import pygame
+
+                def render_puff_area(surface: pygame.Surface,
+                                     coordinate_converter: CoordinateConverter):
+                    predator_location = coordinate_converter.from_canonical(self.predator.state.location)
+                    puff_area_size = self.puff_threshold * coordinate_converter.screen_width
+                    puff_location = predator_location[0] - puff_area_size, predator_location[1] - puff_area_size
+                    puff_area_surface = pygame.Surface((puff_area_size * 2, puff_area_size * 2), pygame.SRCALPHA)
+                    puff_area_color = (255, 0, 0, 60) if self.puff_cool_down > 0 else (0, 0, 255, 60)
+                    pygame.draw.circle(puff_area_surface,
+                                       color=puff_area_color,
+                                       center=(puff_area_size, puff_area_size),
+                                       radius=puff_area_size)
+                    surface.blit(puff_area_surface,
+                                 puff_location)
+                    pygame.draw.circle(surface=surface,
+                                       color=(0, 0, 255),
+                                       center=predator_location,
+                                       radius=puff_area_size,
+                                       width=2)
+
+                self.view.add_render_step(render_puff_area)
+
+        self.puff_cool_down: float = 0
+        self.prey_data_1 = DualEvadePreyData()
+        self.prey_data_2 = DualEvadePreyData()
+
+    def __update_state__(self,
+                         delta_t: float = 0):
+        self.mouse_visible = self.visibility.line_of_sight(self.prey_1.state.location, self.prey_2.state.location)
+        if self.use_predator and self.puff_cool_down <= 0:
+            self.prey_data_1.predator_prey_distance = distance(self.prey_1.state.location,
+                                                               self.predator.state.location)
+            self.prey_data_1.predator_visible = self.prey_1.visible and self.visibility.line_of_sight(self.prey_1.state.location, self.predator.state.location)
+            if self.prey_data_1.predator_visible:
+                if self.prey_data_1.predator_prey_distance <= self.puff_threshold:
+                    self.prey_data_1.puffed = True
+                    self.prey_data_1.puff_count += 1
+                    self.puff_cool_down = self.puff_cool_down_time
+
+            self.prey_data_2.predator_prey_distance = distance(self.prey_2.state.location,
+                                                               self.predator.state.location)
+
+            self.prey_data_2.predator_visible = self.prey_2.visible and self.visibility.line_of_sight(self.prey_2.state.location, self.predator.state.location)
+            if self.prey_data_2.predator_visible:
+                if self.prey_data_2.predator_prey_distance <= self.puff_threshold:
+                    self.prey_data_2.puffed = True
+                    self.prey_data_2.puff_count += 1
+                    self.puff_cool_down = self.puff_cool_down_time
+
+            closest_visible_prey_location = None
+            if self.prey_data_1.predator_visible:
+                closest_visible_prey_location = self.prey_1.state.location
+
+            if self.prey_data_2.predator_visible:
+                if closest_visible_prey_location:
+                    if self.prey_data_2.predator_prey_distance <= self.prey_data_1.predator_prey_distance:
+                        closest_visible_prey_location = self.prey_2.state.location
+                else:
+                    closest_visible_prey_location = self.prey_2.state.location
+
+            if closest_visible_prey_location:
+                self.predator.set_destination(self.prey_2.state.location)
+
+            if not self.predator.path:
+                self.predator.set_destination(random.choice(self.loader.open_locations))
+
+        if delta_t < self.puff_cool_down:
+            self.puff_cool_down -= delta_t
+        else:
+            self.puff_cool_down = 0
+
+        self.prey_data_1.prey_goal_distance = distance(self.goal_location, self.prey_1.state.location)
+        if self.prey_data_1.prey_goal_distance <= self.goal_threshold:
+            self.prey_data_1.goal_achieved = True
+            self.prey_1.visible = False
+
+        self.prey_data_2.prey_goal_distance = distance(self.goal_location, self.prey_2.state.location)
+        if self.prey_data_2.prey_goal_distance <= self.goal_threshold:
+            self.prey_data_2.goal_achieved = True
+            self.prey_2.visible = False
+
+        if self.prey_data_1.goal_achieved and self.prey_data_2.goal_achieved:
+            self.stop()
+
+    def __on_quit__(self):
+        self.stop()
+
+    def reset(self):
+        self.prey_data_1.reset()
+        self.prey_data_2.reset()
+        self.prey_1.visible = True
+        self.prey_2.visible = True
+        Model.reset(self)
+        self.__update_state__()
+
+    def step(self) -> float:
+        delta_t = Model.step(self)
+        if self.render:
+            self.view.draw()
+        self.__update_state__(delta_t=delta_t)
         return delta_t
```

### Comparing `cellworld_game-0.0.61/cellworld_game/tasks/oasis.py` & `cellworld_game-0.0.68/cellworld_game/tasks/oasis.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,173 +1,171 @@
-import random
-import typing
-
-from ..util import distance
-from ..model import Model
-from ..agent import AgentState, CoordinateConverter
-from ..mouse import Mouse
-from ..robot import Robot
-from ..cellworld_loader import CellWorldLoader
-
-
-class Oasis(Model):
-    def __init__(self,
-                 world_name: str,
-                 goal_locations: typing.List[typing.Tuple[float, float]],
-                 goal_sequence_generator: typing.Callable[[None], typing.List[int]] = None,
-                 use_predator: bool = True,
-                 puff_cool_down_time: float = .5,
-                 goal_time: float = 1,
-                 puff_threshold: float = .1,
-                 goal_threshold: float = .1,
-                 time_step: float = .025,
-                 real_time: bool = False,
-                 render: bool = False):
-
-        if goal_sequence_generator is None:
-            goal_sequence_generator = lambda: random.sample(range(0, len(goal_locations)), 3)
-
-        self.start_location = (.05, .5)
-        self.goal_locations = goal_locations
-        self.goal_time = goal_time
-        self.goal_sequence_generator = goal_sequence_generator
-        self.use_predator = use_predator
-        self.puff_cool_down_time = puff_cool_down_time
-        self.puff_threshold = puff_threshold
-        self.goal_threshold = goal_threshold
-        self.render = render
-        self.loader = CellWorldLoader(world_name=world_name)
-        self.goal_location = None
-        self.goal_sequence: typing.List[int] = []
-
-        Model.__init__(self,
-                       arena=self.loader.arena,
-                       occlusions=self.loader.occlusions,
-                       time_step=time_step,
-                       real_time=real_time)
-
-        if use_predator:
-            self.predator = Robot(start_locations=self.loader.robot_start_locations,
-                                  open_locations=self.loader.open_locations,
-                                  navigation=self.loader.navigation)
-
-            self.add_agent("predator", self.predator)
-
-        self.prey = Mouse(start_state=AgentState(location=self.start_location,
-                                                 direction=0),
-                          navigation=self.loader.navigation)
-
-        self.add_agent("prey", self.prey)
-
-        self.running = False
-
-        if self.render:
-            import pygame
-            from ..view import View
-            self.view = View(model=self)
-            self.view.on_quit = self.__on_quit__
-
-            def render_active_goal(surface: pygame.Surface,
-                                   coordinate_converter: CoordinateConverter):
-                if self.goal_location is None:
-                    return
-                for goal_location in self.goal_locations:
-                    screen_goal_location = coordinate_converter.from_canonical(goal_location)
-                    radius = coordinate_converter.from_canonical(.0125)
-                    goal_color = (0, 255, 0) if self.goal_location == goal_location else (255, 0, 0)
-                    pygame.draw.circle(surface,
-                                       color=goal_color,
-                                       center=screen_goal_location,
-                                       radius=radius)
-
-            self.view.add_render_step(render_active_goal)
-
-            if use_predator:
-                def render_puff_area(surface: pygame.Surface,
-                                     coordinate_converter: CoordinateConverter):
-                    predator_location = coordinate_converter.from_canonical(self.predator.state.location)
-                    puff_area_size = self.puff_threshold * coordinate_converter.screen_width
-                    puff_location = predator_location[0] - puff_area_size, predator_location[1] - puff_area_size
-                    puff_area_surface = pygame.Surface((puff_area_size * 2, puff_area_size * 2), pygame.SRCALPHA)
-                    puff_area_color = (255, 0, 0, 60) if self.puff_cool_down > 0 else (0, 0, 255, 60)
-                    pygame.draw.circle(puff_area_surface,
-                                       color=puff_area_color,
-                                       center=(puff_area_size, puff_area_size),
-                                       radius=puff_area_size)
-                    surface.blit(puff_area_surface,
-                                 puff_location)
-                    pygame.draw.circle(surface=surface,
-                                       color=(0, 0, 255),
-                                       center=predator_location,
-                                       radius=puff_area_size,
-                                       width=2)
-
-                self.view.add_render_step(render_puff_area)
-
-        self.puffed: bool = False
-        self.puff_cool_down: float = 0
-        self.goal_achieved: bool = True
-        self.goal_achieved_time: float = 0
-        self.predator_prey_distance: float = 1
-        self.prey_goal_distance: float = 0
-        self.puff_count = 0
-
-    def __update_state__(self,
-                         delta_t: float = 0):
-        if self.use_predator and self.puff_cool_down <= 0:
-            self.predator_prey_distance = distance(self.prey.state.location,
-                                                   self.predator.state.location)
-            if self.visibility.line_of_sight(self.prey.state.location, self.predator.state.location):
-                if self.predator_prey_distance <= self.puff_threshold:
-                    self.puffed = True
-                    self.puff_count += 1
-                    self.puff_cool_down = self.puff_cool_down_time
-
-                self.predator.set_destination(self.prey.state.location)
-
-            if not self.predator.path:
-                self.predator.set_destination(random.choice(self.loader.open_locations))
-
-        if delta_t < self.puff_cool_down:
-            self.puff_cool_down -= delta_t
-        else:
-            self.puff_cool_down = 0
-
-        self.prey_goal_distance = distance(self.goal_location, self.prey.state.location)
-
-        if self.prey_goal_distance <= self.goal_threshold:
-            self.goal_achieved_time += delta_t
-            if self.goal_achieved_time >= self.goal_time:
-                self.__update_goal__()
-                self.goal_achieved_time = 0
-                self.goal_achieved = False
-                if self.goal_location is None:
-                    self.running = False
-            else:
-                self.goal_achieved = True
-
-    def __on_quit__(self):
-        self.running = False
-
-    def __update_goal__(self):
-        if self.goal_sequence:
-            self.goal_location = self.goal_locations[self.goal_sequence.pop(0)]
-        else:
-            if self.goal_location == self.start_location:
-                self.goal_location = None
-            else:
-                self.goal_location = self.start_location
-
-    def reset(self):
-        Model.reset(self)
-        self.goal_achieved = False
-        self.puff_count = 0
-        self.goal_sequence = self.goal_sequence_generator()
-        self.__update_goal__()
-        self.__update_state__()
-
-    def step(self) -> float:
-        delta_t = Model.step(self)
-        if self.render:
-            self.view.draw()
-        self.__update_state__(delta_t=delta_t)
+import random
+import typing
+
+from ..util import distance
+from ..model import Model
+from ..agent import AgentState, CoordinateConverter
+from ..mouse import Mouse
+from ..robot import Robot
+from ..cellworld_loader import CellWorldLoader
+
+
+class Oasis(Model):
+    def __init__(self,
+                 world_name: str,
+                 goal_locations: typing.List[typing.Tuple[float, float]],
+                 goal_sequence_generator: typing.Callable[[None], typing.List[int]] = None,
+                 use_predator: bool = True,
+                 puff_cool_down_time: float = .5,
+                 goal_time: float = 1,
+                 puff_threshold: float = .1,
+                 goal_threshold: float = .1,
+                 time_step: float = .025,
+                 real_time: bool = False,
+                 render: bool = False):
+
+        if goal_sequence_generator is None:
+            goal_sequence_generator = lambda: random.sample(range(0, len(goal_locations)), 3)
+
+        self.start_location = (.05, .5)
+        self.goal_locations = goal_locations
+        self.goal_time = goal_time
+        self.goal_sequence_generator = goal_sequence_generator
+        self.use_predator = use_predator
+        self.puff_cool_down_time = puff_cool_down_time
+        self.puff_threshold = puff_threshold
+        self.goal_threshold = goal_threshold
+        self.render = render
+        self.loader = CellWorldLoader(world_name=world_name)
+        self.goal_location = None
+        self.goal_sequence: typing.List[int] = []
+
+        Model.__init__(self,
+                       arena=self.loader.arena,
+                       occlusions=self.loader.occlusions,
+                       time_step=time_step,
+                       real_time=real_time)
+
+        if use_predator:
+            self.predator = Robot(start_locations=self.loader.robot_start_locations,
+                                  open_locations=self.loader.open_locations,
+                                  navigation=self.loader.navigation)
+
+            self.add_agent("predator", self.predator)
+
+        self.prey = Mouse(start_state=AgentState(location=self.start_location,
+                                                 direction=0),
+                          navigation=self.loader.navigation)
+
+        self.add_agent("prey", self.prey)
+
+        if self.render:
+            import pygame
+            from ..view import View
+            self.view = View(model=self)
+            self.view.on_quit = self.__on_quit__
+
+            def render_active_goal(surface: pygame.Surface,
+                                   coordinate_converter: CoordinateConverter):
+                if self.goal_location is None:
+                    return
+                for goal_location in self.goal_locations:
+                    screen_goal_location = coordinate_converter.from_canonical(goal_location)
+                    radius = coordinate_converter.from_canonical(.0125)
+                    goal_color = (0, 255, 0) if self.goal_location == goal_location else (255, 0, 0)
+                    pygame.draw.circle(surface,
+                                       color=goal_color,
+                                       center=screen_goal_location,
+                                       radius=radius)
+
+            self.view.add_render_step(render_active_goal)
+
+            if use_predator:
+                def render_puff_area(surface: pygame.Surface,
+                                     coordinate_converter: CoordinateConverter):
+                    predator_location = coordinate_converter.from_canonical(self.predator.state.location)
+                    puff_area_size = self.puff_threshold * coordinate_converter.screen_width
+                    puff_location = predator_location[0] - puff_area_size, predator_location[1] - puff_area_size
+                    puff_area_surface = pygame.Surface((puff_area_size * 2, puff_area_size * 2), pygame.SRCALPHA)
+                    puff_area_color = (255, 0, 0, 60) if self.puff_cool_down > 0 else (0, 0, 255, 60)
+                    pygame.draw.circle(puff_area_surface,
+                                       color=puff_area_color,
+                                       center=(puff_area_size, puff_area_size),
+                                       radius=puff_area_size)
+                    surface.blit(puff_area_surface,
+                                 puff_location)
+                    pygame.draw.circle(surface=surface,
+                                       color=(0, 0, 255),
+                                       center=predator_location,
+                                       radius=puff_area_size,
+                                       width=2)
+
+                self.view.add_render_step(render_puff_area)
+
+        self.puffed: bool = False
+        self.puff_cool_down: float = 0
+        self.goal_achieved: bool = True
+        self.goal_achieved_time: float = 0
+        self.predator_prey_distance: float = 1
+        self.prey_goal_distance: float = 0
+        self.puff_count = 0
+
+    def __update_state__(self,
+                         delta_t: float = 0):
+        if self.use_predator and self.puff_cool_down <= 0:
+            self.predator_prey_distance = distance(self.prey.state.location,
+                                                   self.predator.state.location)
+            if self.visibility.line_of_sight(self.prey.state.location, self.predator.state.location):
+                if self.predator_prey_distance <= self.puff_threshold:
+                    self.puffed = True
+                    self.puff_count += 1
+                    self.puff_cool_down = self.puff_cool_down_time
+
+                self.predator.set_destination(self.prey.state.location)
+
+            if not self.predator.path:
+                self.predator.set_destination(random.choice(self.loader.open_locations))
+
+        if delta_t < self.puff_cool_down:
+            self.puff_cool_down -= delta_t
+        else:
+            self.puff_cool_down = 0
+
+        self.prey_goal_distance = distance(self.goal_location, self.prey.state.location)
+
+        if self.prey_goal_distance <= self.goal_threshold:
+            self.goal_achieved_time += delta_t
+            if self.goal_achieved_time >= self.goal_time:
+                self.__update_goal__()
+                self.goal_achieved_time = 0
+                self.goal_achieved = False
+                if self.goal_location is None:
+                    self.stop()
+            else:
+                self.goal_achieved = True
+
+    def __on_quit__(self):
+        self.stop()
+
+    def __update_goal__(self):
+        if self.goal_sequence:
+            self.goal_location = self.goal_locations[self.goal_sequence.pop(0)]
+        else:
+            if self.goal_location == self.start_location:
+                self.goal_location = None
+            else:
+                self.goal_location = self.start_location
+
+    def reset(self):
+        Model.reset(self)
+        self.goal_achieved = False
+        self.puff_count = 0
+        self.goal_sequence = self.goal_sequence_generator()
+        self.__update_goal__()
+        self.__update_state__()
+
+    def step(self) -> float:
+        delta_t = Model.step(self)
+        if self.render:
+            self.view.draw()
+        self.__update_state__(delta_t=delta_t)
         return delta_t
```

### Comparing `cellworld_game-0.0.61/cellworld_game/util.py` & `cellworld_game-0.0.68/cellworld_game/util.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,240 +1,240 @@
-import math
-import typing
-import shapely as sp
-import colorsys
-
-
-def distance2(point1: typing.Tuple[float, float],
-              point2: typing.Tuple[float, float]):
-    return (point2[0] - point1[0]) ** 2 + (point2[1] - point1[1]) ** 2
-
-
-def generate_distinct_colors(n):
-    """
-    Generate a list of n distinct RGB colors.
-
-    Parameters:
-    n (int): The number of distinct colors to generate.
-
-    Returns:
-    List[Tuple[int, int, int]]: A list of n RGB colors.
-    """
-    colors = []
-    for i in range(n):
-        hue = i / n  # Evenly distribute hues in the [0, 1) interval
-        saturation = 0.7  # Choose a saturation level that avoids white and grays
-        lightness = 0.5  # Choose a lightness level that avoids black and white
-        rgb = colorsys.hls_to_rgb(hue, lightness, saturation)
-        # Convert the RGB values from [0, 1] to [0, 255] and round them to integers
-        rgb = tuple(round(c * 255) for c in rgb)
-        colors.append(rgb)
-
-    return colors
-
-
-def create_hexagon(center: tuple, diameter: float, angle: float) -> sp.Polygon:
-    """
-    Create a hexagon centered at the origin, with a specified rotation angle (in degrees)
-    and diameter (distance between opposite vertices).
-
-    Parameters:
-    angle (float): Rotation angle in degrees.
-    diameter (float): Diameter of the hexagon (distance between opposite vertices).
-
-    Returns:
-    Polygon: A Shapely Polygon object representing the hexagon.
-    """
-    radius = diameter / 2
-    rotation = math.radians(angle + 90)
-    # Generate the points for the hexagon
-    points = []
-    center_x, center_y = center
-    for i in range(6):
-        angle_rad = math.radians(60 * i)  # 60 degrees between the points of a hexagon
-        x = center_x + radius * math.cos(angle_rad + rotation)
-        y = center_y + radius * math.sin(angle_rad + rotation)
-        points.append((x, y))
-
-    # Create the hexagon
-    hexagon = sp.geometry.Polygon(points)
-
-    return hexagon
-
-
-def move_point(start: typing.Tuple[float, float], distance: float, direction: float = None, direction_radians: float = None) -> typing.Tuple[float, float]:
-    if direction_radians is None:
-        direction_radians = math.radians(direction)
-    start_x, start_y = start
-    delta_x = distance * math.cos(direction_radians)
-    delta_y = distance * math.sin(direction_radians)
-    return start_x + delta_x, start_y + delta_y
-
-
-def create_line_string(start: typing.Tuple[float, float], direction: float, distance: float):
-    return sp.LineString([start, move_point(start=start,
-                                            direction=direction,
-                                            distance=distance)])
-
-
-def polygon_to_linestrings(polygon):
-    """
-    Break a Polygon into individual LineStrings representing its edges.
-
-    Parameters:
-    polygon (Polygon): The input Polygon object.
-    include_holes (bool): If True, include the interior boundaries (holes) as well.
-
-    Returns:
-    List[LineString]: A list of LineString objects representing the edges of the polygon.
-    """
-    linestrings = []
-
-    # Process the exterior ring
-    exterior_coords = list(polygon.exterior.coords)
-    for i in range(1, len(exterior_coords)):
-        linestrings.append(sp.LineString([exterior_coords[i - 1], exterior_coords[i]]))
-    return linestrings
-
-
-def polygons_to_sides(polygons):
-    """
-    Break a Polygon into individual LineStrings representing its edges.
-
-    Parameters:
-    polygon (Polygon): The input Polygon object.
-    include_holes (bool): If True, include the interior boundaries (holes) as well.
-
-    Returns:
-    List[LineString]: A list of LineString objects representing the edges of the polygon.
-    """
-    vertices = []
-    vertices_sides = []
-
-    def add_vertex(vertex):
-        i = 0
-        for i, v in enumerate(vertices):
-            if v.distance(vertex) <= .001:
-                break
-        else:
-            i = len(vertices)
-            vertices.append(vertex)
-            vertices_sides.append([])
-        return i
-
-    sides_vertices = []
-
-    def find_side(sv):
-        for i, (a, b) in enumerate(sides_vertices):
-            if (a, b) == sv or (b, a) == sv:
-                return i
-        return -1
-
-    internal_sides = []
-    # Process the exterior ring
-    for polygon in polygons:
-        exterior_coords = list(polygon.exterior.coords)
-        origin = add_vertex(sp.Point(exterior_coords[0]))
-        vertices_sides.append([])
-        point_a = origin
-        for i in range(1, len(exterior_coords) - 1):
-            point_b = add_vertex(sp.Point(exterior_coords[i]))
-            i = find_side((point_a, point_b))
-            if i == -1:
-                side_number = len(sides_vertices)
-                sides_vertices.append((point_a, point_b))
-                vertices_sides[point_a].append(side_number)
-                vertices_sides[point_b].append(side_number)
-            else:
-                internal_sides.append(i)
-            point_a = point_b
-        i = find_side((point_a, origin))
-        if i == -1:
-            side_number = len(sides_vertices)
-            sides_vertices.append((point_a, origin))
-            vertices_sides[point_a].append(side_number)
-            vertices_sides[origin].append(side_number)
-        else:
-            internal_sides.append(i)
-
-    filtered_sides_vertices = []
-    for i, side_vertices in enumerate(sides_vertices):
-        if i not in internal_sides:
-            filtered_sides_vertices.append(side_vertices)
-
-    sides = []
-    sides_centroids = []
-    for a, b in filtered_sides_vertices:
-        side = sp.LineString([vertices[a], vertices[b]])
-        sides.append(side)
-        sides_centroids.append(side.centroid)
-
-    return sides, sides_centroids, vertices, filtered_sides_vertices
-
-
-from itertools import combinations
-
-
-def max_distance_between_vertices(polygon):
-    """
-    Calculate the maximum distance between any two vertices of a polygon's exterior.
-
-    Parameters:
-    polygon (Polygon): The input Polygon object.
-
-    Returns:
-    float: The maximum distance between any two vertices of the polygon's exterior.
-    """
-    # Get the exterior coordinates of the polygon
-    exterior_coords = list(polygon.exterior.coords)
-
-    # Initialize the maximum distance to be the minimum possible value
-    max_distance = 0
-
-    # Iterate over all combinations of two points among the vertices
-    for point1, point2 in combinations(exterior_coords, 2):
-        # Calculate the distance between the two points
-        distance = sp.Point(point1).distance(point2)
-
-        # Update the maximum distance if the current distance is greater
-        if distance > max_distance:
-            max_distance = distance
-
-    return max_distance
-
-
-def theta_in_between(theta, start, end):
-    if end > start:
-        return start < theta < end
-    return theta > start or theta < end
-
-
-def distance(src, dst):
-    return math.sqrt((src[0]-dst[0]) ** 2 + (src[1]-dst[1]) ** 2)
-
-
-def direction(src, dst):
-    return math.degrees(math.atan2(dst[1] - src[1], dst[0] - src[0]))
-
-
-def normalize_direction(direction: float):
-    while direction < -180:
-        direction += 360
-    while direction > 180:
-        direction -= 360
-    return direction
-
-
-def direction_difference(direction1: float, direction2: float):
-    direction1 = normalize_direction(direction1)
-    direction2 = normalize_direction(direction2)
-    difference = direction2 - direction1
-    if difference > 180:
-        difference -= 360
-    if difference < -180:
-        difference += 360
-    return difference
-
-
-def direction_error_normalization(direction_error: float):
-    pi_err = direction_error / 8
-    return 1 / (pi_err * pi_err + 1)
+import math
+import typing
+import shapely as sp
+import colorsys
+
+
+def distance2(point1: typing.Tuple[float, float],
+              point2: typing.Tuple[float, float]):
+    return (point2[0] - point1[0]) ** 2 + (point2[1] - point1[1]) ** 2
+
+
+def generate_distinct_colors(n):
+    """
+    Generate a list of n distinct RGB colors.
+
+    Parameters:
+    n (int): The number of distinct colors to generate.
+
+    Returns:
+    List[Tuple[int, int, int]]: A list of n RGB colors.
+    """
+    colors = []
+    for i in range(n):
+        hue = i / n  # Evenly distribute hues in the [0, 1) interval
+        saturation = 0.7  # Choose a saturation level that avoids white and grays
+        lightness = 0.5  # Choose a lightness level that avoids black and white
+        rgb = colorsys.hls_to_rgb(hue, lightness, saturation)
+        # Convert the RGB values from [0, 1] to [0, 255] and round them to integers
+        rgb = tuple(round(c * 255) for c in rgb)
+        colors.append(rgb)
+
+    return colors
+
+
+def create_hexagon(center: tuple, diameter: float, angle: float) -> sp.Polygon:
+    """
+    Create a hexagon centered at the origin, with a specified rotation angle (in degrees)
+    and diameter (distance between opposite vertices).
+
+    Parameters:
+    angle (float): Rotation angle in degrees.
+    diameter (float): Diameter of the hexagon (distance between opposite vertices).
+
+    Returns:
+    Polygon: A Shapely Polygon object representing the hexagon.
+    """
+    radius = diameter / 2
+    rotation = math.radians(angle + 90)
+    # Generate the points for the hexagon
+    points = []
+    center_x, center_y = center
+    for i in range(6):
+        angle_rad = math.radians(60 * i)  # 60 degrees between the points of a hexagon
+        x = center_x + radius * math.cos(angle_rad + rotation)
+        y = center_y + radius * math.sin(angle_rad + rotation)
+        points.append((x, y))
+
+    # Create the hexagon
+    hexagon = sp.geometry.Polygon(points)
+
+    return hexagon
+
+
+def move_point(start: typing.Tuple[float, float], distance: float, direction: float = None, direction_radians: float = None) -> typing.Tuple[float, float]:
+    if direction_radians is None:
+        direction_radians = math.radians(direction)
+    start_x, start_y = start
+    delta_x = distance * math.cos(direction_radians)
+    delta_y = distance * math.sin(direction_radians)
+    return start_x + delta_x, start_y + delta_y
+
+
+def create_line_string(start: typing.Tuple[float, float], direction: float, distance: float):
+    return sp.LineString([start, move_point(start=start,
+                                            direction=direction,
+                                            distance=distance)])
+
+
+def polygon_to_linestrings(polygon):
+    """
+    Break a Polygon into individual LineStrings representing its edges.
+
+    Parameters:
+    polygon (Polygon): The input Polygon object.
+    include_holes (bool): If True, include the interior boundaries (holes) as well.
+
+    Returns:
+    List[LineString]: A list of LineString objects representing the edges of the polygon.
+    """
+    linestrings = []
+
+    # Process the exterior ring
+    exterior_coords = list(polygon.exterior.coords)
+    for i in range(1, len(exterior_coords)):
+        linestrings.append(sp.LineString([exterior_coords[i - 1], exterior_coords[i]]))
+    return linestrings
+
+
+def polygons_to_sides(polygons):
+    """
+    Break a Polygon into individual LineStrings representing its edges.
+
+    Parameters:
+    polygon (Polygon): The input Polygon object.
+    include_holes (bool): If True, include the interior boundaries (holes) as well.
+
+    Returns:
+    List[LineString]: A list of LineString objects representing the edges of the polygon.
+    """
+    vertices = []
+    vertices_sides = []
+
+    def add_vertex(vertex):
+        i = 0
+        for i, v in enumerate(vertices):
+            if v.distance(vertex) <= .001:
+                break
+        else:
+            i = len(vertices)
+            vertices.append(vertex)
+            vertices_sides.append([])
+        return i
+
+    sides_vertices = []
+
+    def find_side(sv):
+        for i, (a, b) in enumerate(sides_vertices):
+            if (a, b) == sv or (b, a) == sv:
+                return i
+        return -1
+
+    internal_sides = []
+    # Process the exterior ring
+    for polygon in polygons:
+        exterior_coords = list(polygon.exterior.coords)
+        origin = add_vertex(sp.Point(exterior_coords[0]))
+        vertices_sides.append([])
+        point_a = origin
+        for i in range(1, len(exterior_coords) - 1):
+            point_b = add_vertex(sp.Point(exterior_coords[i]))
+            i = find_side((point_a, point_b))
+            if i == -1:
+                side_number = len(sides_vertices)
+                sides_vertices.append((point_a, point_b))
+                vertices_sides[point_a].append(side_number)
+                vertices_sides[point_b].append(side_number)
+            else:
+                internal_sides.append(i)
+            point_a = point_b
+        i = find_side((point_a, origin))
+        if i == -1:
+            side_number = len(sides_vertices)
+            sides_vertices.append((point_a, origin))
+            vertices_sides[point_a].append(side_number)
+            vertices_sides[origin].append(side_number)
+        else:
+            internal_sides.append(i)
+
+    filtered_sides_vertices = []
+    for i, side_vertices in enumerate(sides_vertices):
+        if i not in internal_sides:
+            filtered_sides_vertices.append(side_vertices)
+
+    sides = []
+    sides_centroids = []
+    for a, b in filtered_sides_vertices:
+        side = sp.LineString([vertices[a], vertices[b]])
+        sides.append(side)
+        sides_centroids.append(side.centroid)
+
+    return sides, sides_centroids, vertices, filtered_sides_vertices
+
+
+from itertools import combinations
+
+
+def max_distance_between_vertices(polygon):
+    """
+    Calculate the maximum distance between any two vertices of a polygon's exterior.
+
+    Parameters:
+    polygon (Polygon): The input Polygon object.
+
+    Returns:
+    float: The maximum distance between any two vertices of the polygon's exterior.
+    """
+    # Get the exterior coordinates of the polygon
+    exterior_coords = list(polygon.exterior.coords)
+
+    # Initialize the maximum distance to be the minimum possible value
+    max_distance = 0
+
+    # Iterate over all combinations of two points among the vertices
+    for point1, point2 in combinations(exterior_coords, 2):
+        # Calculate the distance between the two points
+        distance = sp.Point(point1).distance(point2)
+
+        # Update the maximum distance if the current distance is greater
+        if distance > max_distance:
+            max_distance = distance
+
+    return max_distance
+
+
+def theta_in_between(theta, start, end):
+    if end > start:
+        return start < theta < end
+    return theta > start or theta < end
+
+
+def distance(src, dst):
+    return math.sqrt((src[0]-dst[0]) ** 2 + (src[1]-dst[1]) ** 2)
+
+
+def direction(src, dst):
+    return math.degrees(math.atan2(dst[1] - src[1], dst[0] - src[0]))
+
+
+def normalize_direction(direction: float):
+    while direction < -180:
+        direction += 360
+    while direction > 180:
+        direction -= 360
+    return direction
+
+
+def direction_difference(direction1: float, direction2: float):
+    direction1 = normalize_direction(direction1)
+    direction2 = normalize_direction(direction2)
+    difference = direction2 - direction1
+    if difference > 180:
+        difference -= 360
+    if difference < -180:
+        difference += 360
+    return difference
+
+
+def direction_error_normalization(direction_error: float):
+    pi_err = direction_error / 8
+    return 1 / (pi_err * pi_err + 1)
```

### Comparing `cellworld_game-0.0.61/cellworld_game/view.py` & `cellworld_game-0.0.68/cellworld_game/view.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,142 +1,142 @@
-import math
-import pygame
-import typing
-from .model import Model
-from .agent import CoordinateConverter
-from .util import generate_distinct_colors
-
-
-class View(object):
-    def __init__(self,
-                 model: Model,
-                 screen_width: int = 800,
-                 flip_y: bool = True):
-        pygame.init()
-        self.model = model
-        self.visibility = model.visibility
-        self.screen_width = screen_width
-        self.hexa_ratio = (math.sqrt(3) / 2)
-        self.coordinate_converter = CoordinateConverter(screen_size=(screen_width, int(self.hexa_ratio * screen_width)),
-                                                        flip_y=flip_y)
-        for agent_name, agent in model.agents.items():
-            agent.set_sprite_size((screen_width/10, screen_width/10))
-            agent.set_coordinate_converter(self.coordinate_converter)
-        self.screen = pygame.display.set_mode(self.coordinate_converter.screen_size)
-        self.arena_color = (255, 255, 255)
-        self.occlusion_color = (50, 50, 50)
-        self.agent_colors = {agent_name: color for agent_name, color
-                             in zip(self.model.agents.keys(),
-                                    generate_distinct_colors(len(self.model.agents)))}
-        self.clock = pygame.time.Clock()
-        self.agent_perspective = -1
-        self.show_sprites = True
-        self.target = None
-        self.on_mouse_button_down = None
-        self.on_mouse_button_up = None
-        self.on_mouse_move = None
-        self.on_mouse_wheel = None
-        self.on_key_up = None
-        self.on_quit = None
-        self.on_frame = None
-        self.pressed_keys = pygame.key.get_pressed()
-        self.render_steps: typing.List[typing.Callable[[pygame.Surface, CoordinateConverter], None]] = []
-
-    def add_render_step(self,
-                        render_step: typing.Callable[[pygame.Surface, CoordinateConverter], None]):
-        self.render_steps.append(render_step)
-
-    def draw_polygon(self, polygon, color):
-        """Draws a hexagon at the specified position and size."""
-        pygame.draw.polygon(self.screen,
-                            color,
-                            [self.coordinate_converter.from_canonical(point) for point in polygon.exterior.coords])
-
-    def draw_polygon_vertices(self, polygon, color, size=2):
-        """Draws a hexagon at the specified position and size."""
-        for point in polygon.exterior.coords:
-            pygame.draw.circle(surface=self.screen,
-                               color=color,
-                               center=self.coordinate_converter.from_canonical(point),
-                               radius=size,
-                               width=2)
-
-    def draw_points(self, points, color, size=2):
-        """Draws a hexagon at the specified position and size."""
-        for point in points:
-            pygame.draw.circle(surface=self.screen,
-                               color=color,
-                               center=self.coordinate_converter.from_canonical((point.x, point.y)),
-                               radius=size,
-                               width=2)
-
-    def draw(self):
-        self.screen.fill((0, 0, 0))
-        self.draw_polygon(self.model.arena, self.arena_color)
-
-        if self.agent_perspective != -1:
-            agent_name = list(self.model.agents.keys())[self.agent_perspective]
-            visibility_perspective = self.model.agents[agent_name].state
-            visibility_polygon, a = self.visibility.get_visibility_polygon(location=visibility_perspective.location,
-                                                                           direction=visibility_perspective.direction,
-                                                                           view_field=360)
-            self.draw_polygon(visibility_polygon, (180, 180, 180))
-
-        for occlusion in self.model.occlusions:
-            self.draw_polygon(occlusion, self.occlusion_color)
-
-        for (name, agent), color in zip(self.model.agents.items(), self.agent_colors):
-            if agent.visible:
-                if self.show_sprites:
-                    agent.draw(surface=self.screen,
-                               coordinate_converter=self.coordinate_converter)
-                else:
-                    self.draw_polygon(self.model.agents[name].get_polygon(), color=self.agent_colors[name])
-
-        for render_step in self.render_steps:
-            render_step(self.screen, self.coordinate_converter)
-
-        self.__process_events__()
-        if self.on_frame:
-            self.on_frame(self.screen, self.coordinate_converter)
-        pygame.display.flip()
-
-    def __process_events__(self):
-        for event in pygame.event.get():
-            if event.type == pygame.QUIT:
-                if self.on_quit:
-                    self.on_quit()
-            if event.type == pygame.MOUSEBUTTONDOWN:
-                canonical_x_y = self.coordinate_converter.to_canonical(event.pos)
-                if self.on_mouse_button_down:
-                    self.on_mouse_button_down(event.button, canonical_x_y)
-            elif event.type == pygame.MOUSEBUTTONUP:
-                canonical_x_y = self.coordinate_converter.to_canonical(event.pos)
-                if self.on_mouse_button_up:
-                    self.on_mouse_button_up(event.button, canonical_x_y)
-            elif event.type == pygame.MOUSEMOTION:
-                canonical_x_y = self.coordinate_converter.to_canonical(event.pos)
-                if self.on_mouse_move:
-                    self.on_mouse_move(canonical_x_y)
-            elif event.type == pygame.MOUSEWHEEL:
-                canonical_x_y = self.coordinate_converter.to_canonical(event.pos)
-                if self.on_mouse_wheel:
-                    self.on_mouse_wheel(event.button, canonical_x_y)
-            elif event.type == pygame.KEYDOWN:
-                if self.on_key_down:
-                    self.on_key_down(key=event.key)
-            elif event.type == pygame.KEYUP:
-                if self.on_key_up:
-                    self.on_key_up(event.key)
-        self.pressed_keys = pygame.key.get_pressed()
-
-    def on_key_down(self, key):
-        if key == pygame.K_0:
-            self.agent_perspective = -1
-        if key == pygame.K_1:
-            self.agent_perspective = 0
-        if key == pygame.K_2:
-            self.agent_perspective = 1
-        if key == pygame.K_3:
-            self.show_sprites = False
-        if key == pygame.K_4:
-            self.show_sprites = True
+import math
+import pygame
+import typing
+from .model import Model
+from .agent import CoordinateConverter
+from .util import generate_distinct_colors
+
+
+class View(object):
+    def __init__(self,
+                 model: Model,
+                 screen_width: int = 800,
+                 flip_y: bool = True):
+        pygame.init()
+        self.model = model
+        self.visibility = model.visibility
+        self.screen_width = screen_width
+        self.hexa_ratio = (math.sqrt(3) / 2)
+        self.coordinate_converter = CoordinateConverter(screen_size=(screen_width, int(self.hexa_ratio * screen_width)),
+                                                        flip_y=flip_y)
+        for agent_name, agent in model.agents.items():
+            agent.set_sprite_size((screen_width/10, screen_width/10))
+            agent.set_coordinate_converter(self.coordinate_converter)
+        self.screen = pygame.display.set_mode(self.coordinate_converter.screen_size)
+        self.arena_color = (255, 255, 255)
+        self.occlusion_color = (50, 50, 50)
+        self.agent_colors = {agent_name: color for agent_name, color
+                             in zip(self.model.agents.keys(),
+                                    generate_distinct_colors(len(self.model.agents)))}
+        self.clock = pygame.time.Clock()
+        self.agent_perspective = -1
+        self.show_sprites = True
+        self.target = None
+        self.on_mouse_button_down = None
+        self.on_mouse_button_up = None
+        self.on_mouse_move = None
+        self.on_mouse_wheel = None
+        self.on_key_up = None
+        self.on_quit = None
+        self.on_frame = None
+        self.pressed_keys = pygame.key.get_pressed()
+        self.render_steps: typing.List[typing.Callable[[pygame.Surface, CoordinateConverter], None]] = []
+
+    def add_render_step(self,
+                        render_step: typing.Callable[[pygame.Surface, CoordinateConverter], None]):
+        self.render_steps.append(render_step)
+
+    def draw_polygon(self, polygon, color):
+        """Draws a hexagon at the specified position and size."""
+        pygame.draw.polygon(self.screen,
+                            color,
+                            [self.coordinate_converter.from_canonical(point) for point in polygon.exterior.coords])
+
+    def draw_polygon_vertices(self, polygon, color, size=2):
+        """Draws a hexagon at the specified position and size."""
+        for point in polygon.exterior.coords:
+            pygame.draw.circle(surface=self.screen,
+                               color=color,
+                               center=self.coordinate_converter.from_canonical(point),
+                               radius=size,
+                               width=2)
+
+    def draw_points(self, points, color, size=2):
+        """Draws a hexagon at the specified position and size."""
+        for point in points:
+            pygame.draw.circle(surface=self.screen,
+                               color=color,
+                               center=self.coordinate_converter.from_canonical((point.x, point.y)),
+                               radius=size,
+                               width=2)
+
+    def draw(self):
+        self.screen.fill((0, 0, 0))
+        self.draw_polygon(self.model.arena, self.arena_color)
+
+        if self.agent_perspective != -1:
+            agent_name = list(self.model.agents.keys())[self.agent_perspective]
+            visibility_perspective = self.model.agents[agent_name].state
+            visibility_polygon, a = self.visibility.get_visibility_polygon(location=visibility_perspective.location,
+                                                                           direction=visibility_perspective.direction,
+                                                                           view_field=360)
+            self.draw_polygon(visibility_polygon, (180, 180, 180))
+
+        for occlusion in self.model.occlusions:
+            self.draw_polygon(occlusion, self.occlusion_color)
+
+        for (name, agent), color in zip(self.model.agents.items(), self.agent_colors):
+            if agent.visible:
+                if self.show_sprites:
+                    agent.draw(surface=self.screen,
+                               coordinate_converter=self.coordinate_converter)
+                else:
+                    self.draw_polygon(self.model.agents[name].get_polygon(), color=self.agent_colors[name])
+
+        for render_step in self.render_steps:
+            render_step(self.screen, self.coordinate_converter)
+
+        self.__process_events__()
+        if self.on_frame:
+            self.on_frame(self.screen, self.coordinate_converter)
+        pygame.display.flip()
+
+    def __process_events__(self):
+        for event in pygame.event.get():
+            if event.type == pygame.QUIT:
+                if self.on_quit:
+                    self.on_quit()
+            if event.type == pygame.MOUSEBUTTONDOWN:
+                canonical_x_y = self.coordinate_converter.to_canonical(event.pos)
+                if self.on_mouse_button_down:
+                    self.on_mouse_button_down(event.button, canonical_x_y)
+            elif event.type == pygame.MOUSEBUTTONUP:
+                canonical_x_y = self.coordinate_converter.to_canonical(event.pos)
+                if self.on_mouse_button_up:
+                    self.on_mouse_button_up(event.button, canonical_x_y)
+            elif event.type == pygame.MOUSEMOTION:
+                canonical_x_y = self.coordinate_converter.to_canonical(event.pos)
+                if self.on_mouse_move:
+                    self.on_mouse_move(canonical_x_y)
+            elif event.type == pygame.MOUSEWHEEL:
+                canonical_x_y = self.coordinate_converter.to_canonical(event.pos)
+                if self.on_mouse_wheel:
+                    self.on_mouse_wheel(event.button, canonical_x_y)
+            elif event.type == pygame.KEYDOWN:
+                if self.on_key_down:
+                    self.on_key_down(key=event.key)
+            elif event.type == pygame.KEYUP:
+                if self.on_key_up:
+                    self.on_key_up(event.key)
+        self.pressed_keys = pygame.key.get_pressed()
+
+    def on_key_down(self, key):
+        if key == pygame.K_0:
+            self.agent_perspective = -1
+        if key == pygame.K_1:
+            self.agent_perspective = 0
+        if key == pygame.K_2:
+            self.agent_perspective = 1
+        if key == pygame.K_3:
+            self.show_sprites = False
+        if key == pygame.K_4:
+            self.show_sprites = True
```

### Comparing `cellworld_game-0.0.61/cellworld_game.egg-info/SOURCES.txt` & `cellworld_game-0.0.68/cellworld_game.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -20,32 +20,45 @@
 cellworld_game/visibility.py
 cellworld_game.egg-info/PKG-INFO
 cellworld_game.egg-info/SOURCES.txt
 cellworld_game.egg-info/dependency_links.txt
 cellworld_game.egg-info/not-zip-safe
 cellworld_game.egg-info/requires.txt
 cellworld_game.egg-info/top_level.txt
+cellworld_game/__pycache__/__init__.cpython-310.pyc
 cellworld_game/__pycache__/__init__.cpython-312.pyc
+cellworld_game/__pycache__/agent.cpython-310.pyc
 cellworld_game/__pycache__/agent.cpython-312.pyc
+cellworld_game/__pycache__/cellworld_loader.cpython-310.pyc
 cellworld_game/__pycache__/cellworld_loader.cpython-312.pyc
+cellworld_game/__pycache__/environment.cpython-310.pyc
+cellworld_game/__pycache__/environment.cpython-312.pyc
+cellworld_game/__pycache__/geometry.cpython-310.pyc
 cellworld_game/__pycache__/geometry.cpython-312.pyc
+cellworld_game/__pycache__/model.cpython-310.pyc
 cellworld_game/__pycache__/model.cpython-312.pyc
+cellworld_game/__pycache__/mouse.cpython-310.pyc
 cellworld_game/__pycache__/mouse.cpython-312.pyc
+cellworld_game/__pycache__/navigation.cpython-310.pyc
 cellworld_game/__pycache__/navigation.cpython-312.pyc
+cellworld_game/__pycache__/navigation_agent.cpython-310.pyc
 cellworld_game/__pycache__/navigation_agent.cpython-312.pyc
+cellworld_game/__pycache__/ray_tracing.cpython-310.pyc
 cellworld_game/__pycache__/ray_tracing.cpython-312.pyc
+cellworld_game/__pycache__/resources.cpython-310.pyc
 cellworld_game/__pycache__/resources.cpython-312.pyc
+cellworld_game/__pycache__/reward.cpython-312.pyc
+cellworld_game/__pycache__/robot.cpython-310.pyc
 cellworld_game/__pycache__/robot.cpython-312.pyc
+cellworld_game/__pycache__/util.cpython-310.pyc
 cellworld_game/__pycache__/util.cpython-312.pyc
+cellworld_game/__pycache__/view.cpython-310.pyc
 cellworld_game/__pycache__/view.cpython-312.pyc
+cellworld_game/__pycache__/visibility.cpython-310.pyc
 cellworld_game/__pycache__/visibility.cpython-312.pyc
 cellworld_game/files/agent.png
 cellworld_game/files/predator.png
 cellworld_game/files/prey.png
 cellworld_game/tasks/__init__.py
 cellworld_game/tasks/botevade.py
 cellworld_game/tasks/dualevade.py
-cellworld_game/tasks/oasis.py
-cellworld_game/tasks/__pycache__/__init__.cpython-312.pyc
-cellworld_game/tasks/__pycache__/botevade.cpython-312.pyc
-cellworld_game/tasks/__pycache__/dualevade.cpython-312.pyc
-cellworld_game/tasks/__pycache__/oasis.cpython-312.pyc
+cellworld_game/tasks/oasis.py
```

### Comparing `cellworld_game-0.0.61/setup.py` & `cellworld_game-0.0.68/setup.py`

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
-      version='0.0.61',
+      version='0.0.68',
       zip_safe=False)
```


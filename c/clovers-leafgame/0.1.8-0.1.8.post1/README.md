# Comparing `tmp/clovers_leafgame-0.1.8.tar.gz` & `tmp/clovers_leafgame-0.1.8.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clovers_leafgame-0.1.8.tar", max compression
+gzip compressed data, was "clovers_leafgame-0.1.8.post1.tar", max compression
```

## Comparing `clovers_leafgame-0.1.8.tar` & `clovers_leafgame-0.1.8.post1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      300 2024-04-27 08:49:20.730233 clovers_leafgame-0.1.8/clovers_leafgame/__init__.py
--rw-r--r--   0        0        0      682 2024-04-27 08:49:20.730233 clovers_leafgame-0.1.8/clovers_leafgame/config.py
--rw-r--r--   0        0        0     4001 2024-05-01 06:15:17.412881 clovers_leafgame-0.1.8/clovers_leafgame/core/clovers.py
--rw-r--r--   0        0        0     5568 2024-04-27 09:13:40.955639 clovers_leafgame-0.1.8/clovers_leafgame/core/data.py
--rw-r--r--   0        0        0     1617 2024-04-27 08:49:20.731606 clovers_leafgame-0.1.8/clovers_leafgame/item.py
--rw-r--r--   0        0        0     1151 2024-04-27 08:49:20.731606 clovers_leafgame-0.1.8/clovers_leafgame/main.py
--rw-r--r--   0        0        0     6630 2024-05-01 02:31:44.190645 clovers_leafgame-0.1.8/clovers_leafgame/manager.py
--rw-r--r--   0        0        0    14551 2024-05-01 01:41:25.978756 clovers_leafgame-0.1.8/clovers_leafgame/modules/account/__init__.py
--rw-r--r--   0        0        0      347 2024-04-27 08:49:20.733113 clovers_leafgame-0.1.8/clovers_leafgame/modules/account/config.py
--rw-r--r--   0        0        0    44586 2024-05-01 02:45:31.478949 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/__init__.py
--rw-r--r--   0        0        0      153 2024-04-27 08:49:20.733802 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/config.py
--rw-r--r--   0        0        0     8755 2024-04-27 08:49:20.734312 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/core.py
--rw-r--r--   0        0        0    10104 2024-04-27 08:49:20.734812 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/fortress/core.py
--rw-r--r--   0        0        0    12802 2024-04-27 08:49:20.735312 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/__init__.py
--rw-r--r--   0        0        0      447 2024-04-27 08:49:20.735312 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/config.py
--rw-r--r--   0        0        0     5817 2024-04-27 08:49:20.735812 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/Stand.json
--rw-r--r--   0        0        0     5728 2024-04-27 08:49:20.736312 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/“日常，真的很日常”.json
--rw-r--r--   0        0        0     2174 2024-04-27 08:49:20.736811 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/克苏鲁.json
--rw-r--r--   0        0        0     1231 2024-04-27 08:49:20.736811 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/基础事件.json
--rw-r--r--   0        0        0     2742 2024-04-27 08:49:20.737312 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/复刻经典事件集合v1.json
--rw-r--r--   0        0        0     1606 2024-04-27 08:49:20.737312 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/崩坏集合v1.json
--rw-r--r--   0        0        0    25830 2024-04-27 08:49:20.737811 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/群友日常.json
--rw-r--r--   0        0        0     5180 2024-04-27 08:49:20.738314 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/芜湖事件合集.json
--rw-r--r--   0        0        0     1072 2024-04-27 08:49:20.738314 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/赫尔事件集v1.json
--rw-r--r--   0        0        0     2294 2024-04-27 08:49:20.738812 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/赫尔的赛马场事件簿.json
--rw-r--r--   0        0        0     7488 2024-04-27 08:49:20.738812 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/horse.py
--rw-r--r--   0        0        0      933 2024-04-27 08:49:20.739312 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/start.py
--rw-r--r--   0        0        0      754 2024-04-27 08:49:20.739812 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/tools.py
--rw-r--r--   0        0        0    18182 2024-04-27 08:49:20.740312 clovers_leafgame-0.1.8/clovers_leafgame/modules/market/__init__.py
--rw-r--r--   0        0        0      457 2024-04-27 08:49:20.740820 clovers_leafgame-0.1.8/clovers_leafgame/modules/market/config.py
--rw-r--r--   0        0        0    12681 2024-05-01 06:16:15.242569 clovers_leafgame-0.1.8/clovers_leafgame/modules/prop/__init__.py
--rw-r--r--   0        0        0      271 2024-04-27 08:49:20.741311 clovers_leafgame-0.1.8/clovers_leafgame/modules/prop/config.py
--rw-r--r--   0        0        0     2085 2024-04-27 08:49:20.741812 clovers_leafgame-0.1.8/clovers_leafgame/modules/prop/core.py
--rw-r--r--   0        0        0     2681 2024-04-27 08:49:20.741812 clovers_leafgame-0.1.8/clovers_leafgame/modules/prop/output.py
--rw-r--r--   0        0        0     4516 2024-04-27 08:49:20.742312 clovers_leafgame-0.1.8/clovers_leafgame/modules/prop/props_library.json
--rw-r--r--   0        0        0     3958 2024-04-27 08:49:20.742812 clovers_leafgame-0.1.8/clovers_leafgame/modules/ranklist/__init__.py
--rw-r--r--   0        0        0     1003 2024-04-27 08:49:20.742812 clovers_leafgame-0.1.8/clovers_leafgame/modules/ranklist/output.py
--rw-r--r--   0        0        0     3587 2024-04-27 09:15:30.718836 clovers_leafgame-0.1.8/clovers_leafgame/modules/task/__init__.py
--rw-r--r--   0        0        0     6592 2024-04-27 08:49:20.743811 clovers_leafgame-0.1.8/clovers_leafgame/output.py
--rw-r--r--   0        0        0     1806 2024-04-27 09:12:59.164148 clovers_leafgame-0.1.8/clovers_leafgame/props_library.json
--rw-r--r--   0        0        0     1086 2024-04-27 08:49:20.729233 clovers_leafgame-0.1.8/LICENSE
--rw-r--r--   0        0        0      428 2024-05-01 06:17:07.963060 clovers_leafgame-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    18943 2024-04-27 15:58:16.641831 clovers_leafgame-0.1.8/README.md
--rw-r--r--   0        0        0    18657 1970-01-01 00:00:00.000000 clovers_leafgame-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      300 2024-04-27 08:49:20.730233 clovers_leafgame-0.1.8.post1/clovers_leafgame/__init__.py
+-rw-r--r--   0        0        0      682 2024-04-27 08:49:20.730233 clovers_leafgame-0.1.8.post1/clovers_leafgame/config.py
+-rw-r--r--   0        0        0     4001 2024-05-01 06:15:17.412881 clovers_leafgame-0.1.8.post1/clovers_leafgame/core/clovers.py
+-rw-r--r--   0        0        0     5568 2024-04-27 09:13:40.955639 clovers_leafgame-0.1.8.post1/clovers_leafgame/core/data.py
+-rw-r--r--   0        0        0     1617 2024-04-27 08:49:20.731606 clovers_leafgame-0.1.8.post1/clovers_leafgame/item.py
+-rw-r--r--   0        0        0     1151 2024-04-27 08:49:20.731606 clovers_leafgame-0.1.8.post1/clovers_leafgame/main.py
+-rw-r--r--   0        0        0     6630 2024-05-01 02:31:44.190645 clovers_leafgame-0.1.8.post1/clovers_leafgame/manager.py
+-rw-r--r--   0        0        0    14551 2024-05-01 01:41:25.978756 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/account/__init__.py
+-rw-r--r--   0        0        0      347 2024-04-27 08:49:20.733113 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/account/config.py
+-rw-r--r--   0        0        0    44586 2024-05-01 02:45:31.478949 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/__init__.py
+-rw-r--r--   0        0        0      153 2024-04-27 08:49:20.733802 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/config.py
+-rw-r--r--   0        0        0     8755 2024-04-27 08:49:20.734312 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/core.py
+-rw-r--r--   0        0        0    10104 2024-04-27 08:49:20.734812 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/fortress/core.py
+-rw-r--r--   0        0        0    12802 2024-04-27 08:49:20.735312 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/__init__.py
+-rw-r--r--   0        0        0      447 2024-04-27 08:49:20.735312 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/config.py
+-rw-r--r--   0        0        0     5817 2024-04-27 08:49:20.735812 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/Stand.json
+-rw-r--r--   0        0        0     5728 2024-04-27 08:49:20.736312 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/“日常，真的很日常”.json
+-rw-r--r--   0        0        0     2174 2024-04-27 08:49:20.736811 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/克苏鲁.json
+-rw-r--r--   0        0        0     1231 2024-04-27 08:49:20.736811 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/基础事件.json
+-rw-r--r--   0        0        0     2742 2024-04-27 08:49:20.737312 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/复刻经典事件集合v1.json
+-rw-r--r--   0        0        0     1606 2024-04-27 08:49:20.737312 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/崩坏集合v1.json
+-rw-r--r--   0        0        0    25830 2024-04-27 08:49:20.737811 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/群友日常.json
+-rw-r--r--   0        0        0     5180 2024-04-27 08:49:20.738314 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/芜湖事件合集.json
+-rw-r--r--   0        0        0     1072 2024-04-27 08:49:20.738314 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/赫尔事件集v1.json
+-rw-r--r--   0        0        0     2294 2024-04-27 08:49:20.738812 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/赫尔的赛马场事件簿.json
+-rw-r--r--   0        0        0     7488 2024-04-27 08:49:20.738812 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/horse.py
+-rw-r--r--   0        0        0      933 2024-04-27 08:49:20.739312 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/start.py
+-rw-r--r--   0        0        0      754 2024-04-27 08:49:20.739812 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/tools.py
+-rw-r--r--   0        0        0    18182 2024-04-27 08:49:20.740312 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/market/__init__.py
+-rw-r--r--   0        0        0      457 2024-04-27 08:49:20.740820 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/market/config.py
+-rw-r--r--   0        0        0    12681 2024-05-01 06:16:15.242569 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/prop/__init__.py
+-rw-r--r--   0        0        0      271 2024-04-27 08:49:20.741311 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/prop/config.py
+-rw-r--r--   0        0        0     2085 2024-04-27 08:49:20.741812 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/prop/core.py
+-rw-r--r--   0        0        0     2681 2024-04-27 08:49:20.741812 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/prop/output.py
+-rw-r--r--   0        0        0     4514 2024-05-01 06:19:53.256256 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/prop/props_library.json
+-rw-r--r--   0        0        0     3958 2024-04-27 08:49:20.742812 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/ranklist/__init__.py
+-rw-r--r--   0        0        0     1003 2024-04-27 08:49:20.742812 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/ranklist/output.py
+-rw-r--r--   0        0        0     3587 2024-04-27 09:15:30.718836 clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/task/__init__.py
+-rw-r--r--   0        0        0     6592 2024-04-27 08:49:20.743811 clovers_leafgame-0.1.8.post1/clovers_leafgame/output.py
+-rw-r--r--   0        0        0     1806 2024-04-27 09:12:59.164148 clovers_leafgame-0.1.8.post1/clovers_leafgame/props_library.json
+-rw-r--r--   0        0        0     1086 2024-04-27 08:49:20.729233 clovers_leafgame-0.1.8.post1/LICENSE
+-rw-r--r--   0        0        0      430 2024-05-01 06:21:17.767326 clovers_leafgame-0.1.8.post1/pyproject.toml
+-rw-r--r--   0        0        0    18943 2024-04-27 15:58:16.641831 clovers_leafgame-0.1.8.post1/README.md
+-rw-r--r--   0        0        0    18663 1970-01-01 00:00:00.000000 clovers_leafgame-0.1.8.post1/PKG-INFO
```

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/config.py` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/config.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/core/clovers.py` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/core/clovers.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/core/data.py` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/core/data.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/item.py` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/item.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/main.py` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/main.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/manager.py` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/manager.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/modules/account/__init__.py` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/account/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/__init__.py` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/core.py` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/core.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/fortress/core.py` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/fortress/core.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/__init__.py` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/Stand.json` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/Stand.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/“日常，真的很日常”.json` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/“日常，真的很日常”.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/克苏鲁.json` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/克苏鲁.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/基础事件.json` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/基础事件.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/复刻经典事件集合v1.json` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/复刻经典事件集合v1.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/崩坏集合v1.json` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/崩坏集合v1.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/群友日常.json` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/群友日常.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/芜湖事件合集.json` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/芜湖事件合集.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/赫尔事件集v1.json` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/赫尔事件集v1.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/赫尔的赛马场事件簿.json` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/event_library/赫尔的赛马场事件簿.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/horse.py` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/horse.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/start.py` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/horse_race/start.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/tools.py` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/game/tools.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/modules/market/__init__.py` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/market/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/modules/prop/__init__.py` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/prop/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/modules/prop/core.py` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/prop/core.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/modules/prop/output.py` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/prop/output.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/modules/prop/props_library.json` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/prop/props_library.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970238095238095%*

 * *Differences: {"'0215'": "{'intro': '你可以对自己开一枪，如果你足够幸运躲过一劫，那么你的名下所有账户的金币与股票净值都将翻倍。\\n如果你不幸中弹,你将会在这个世界上消失。'}"}*

```diff
@@ -3,15 +3,15 @@
         "color": "#85200C",
         "intro": "\u628a\u4f60\u7684\u4e2a\u4eba\u6570\u636e\u56de\u6eaf\u5230\u5230\u4efb\u610f\u65f6\u95f4\u8282\u70b9\u3002\n\u53ef\u56de\u6eaf\u7684\u65f6\u95f4\u8282\u70b9\u6709\u591a\u5c11\u53d6\u51b3\u4e8e\u670d\u52a1\u5668\u5907\u4efd\u8bbe\u7f6e",
         "name": "\u7eef\u7ea2\u8ff7\u96fe\u4e4b\u4e66",
         "tip": "\u673a\u5668\u4ebabug\u7814\u7a76\u4e2d\u5fc3"
     },
     "0215": {
         "color": "#0C343D",
-        "intro": "\u4f60\u53ef\u4ee5\u5bf9\u81ea\u5df1\u5f00\u4e00\u67aa\uff0c\u5982\u679c\u4f60\u8db3\u591f\u5e78\u8fd0\u8eb2\u8fc7\u4e00\u52ab\uff0c\u90a3\u4e48\u4f60\u7684\u540d\u4e0b\u6240\u6709\u8d26\u6237\u7684\u91d1\u5e01\u4e0e\u80a1\u7968\u51c0\u503c\u90fd\u5c06\u7ffb10\u500d\u3002\n\u5982\u679c\u4f60\u4e0d\u5e78\u4e2d\u5f39,\u4f60\u5c06\u4f1a\u5728\u8fd9\u4e2a\u4e16\u754c\u4e0a\u6d88\u5931\u3002",
+        "intro": "\u4f60\u53ef\u4ee5\u5bf9\u81ea\u5df1\u5f00\u4e00\u67aa\uff0c\u5982\u679c\u4f60\u8db3\u591f\u5e78\u8fd0\u8eb2\u8fc7\u4e00\u52ab\uff0c\u90a3\u4e48\u4f60\u7684\u540d\u4e0b\u6240\u6709\u8d26\u6237\u7684\u91d1\u5e01\u4e0e\u80a1\u7968\u51c0\u503c\u90fd\u5c06\u7ffb\u500d\u3002\n\u5982\u679c\u4f60\u4e0d\u5e78\u4e2d\u5f39,\u4f60\u5c06\u4f1a\u5728\u8fd9\u4e2a\u4e16\u754c\u4e0a\u6d88\u5931\u3002",
         "name": "\u6076\u9b54\u8f6e\u76d8",
         "tip": "\u4e00\u628a\u7834\u65e7\u7684\u5de6\u8f6e\u67aa"
     },
     "1213": {
         "color": "#66CCFF",
         "intro": "\u6bcf\u79cd\u7a7a\u6c14\u5404\u83b7\u5f97\u4e00\u4e2a",
         "name": "\u7a7a\u6c14\u793c\u5305",
```

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/modules/ranklist/__init__.py` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/ranklist/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/modules/ranklist/output.py` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/ranklist/output.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/modules/task/__init__.py` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/modules/task/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/output.py` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/output.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/clovers_leafgame/props_library.json` & `clovers_leafgame-0.1.8.post1/clovers_leafgame/props_library.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/LICENSE` & `clovers_leafgame-0.1.8.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/README.md` & `clovers_leafgame-0.1.8.post1/README.md`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.8/PKG-INFO` & `clovers_leafgame-0.1.8.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: clovers-leafgame
-Version: 0.1.8
+Version: 0.1.8.post1
 Summary: 
 Author: KarisAya
 Author-email: 1048827424@qq.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: clovers-apscheduler (>=0.1.3,<0.2.0)
+Requires-Dist: clovers-apscheduler (>=0.1.4,<0.2.0)
 Requires-Dist: clovers[linecard,tools] (>=0.1.8,<0.2.0)
 Requires-Dist: mplfinance (>=0.12.10b0,<0.13.0)
 Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD031 MD033 MD036 MD041 -->
 <div align="center">
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: clovers-leafgame Version: 0.1.8 Summary: Author:
-KarisAya Author-email: 1048827424@qq.com Requires-Python: >=3.12,<4.0
+Metadata-Version: 2.1 Name: clovers-leafgame Version: 0.1.8.post1 Summary:
+Author: KarisAya Author-email: 1048827424@qq.com Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3 Requires-Dist: clovers-
-apscheduler (>=0.1.3,<0.2.0) Requires-Dist: clovers[linecard,tools]
+apscheduler (>=0.1.4,<0.2.0) Requires-Dist: clovers[linecard,tools]
 (>=0.1.8,<0.2.0) Requires-Dist: mplfinance (>=0.12.10b0,<0.13.0) Requires-Dist:
 pydantic (>=2.7.0,<3.0.0) Description-Content-Type: text/markdown
   # clovers-leafgame _â¨ æ¹èª [nonebot_plugin_russian](https://github.com/
    HibiKier/nonebot_plugin_russian) å [nonebot_plugin_horserace](https://
  github.com/shinianj/nonebot_plugin_horserace) çå°æ¸¸æåé â¨_[python]
                         _[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
 ## ð¿ å®è£ ```bash pip install clovers_leafgame ``` ## âï¸ éç½® å¨
```


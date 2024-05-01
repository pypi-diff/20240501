# Comparing `tmp/clovers_leafgame-0.1.7.tar.gz` & `tmp/clovers_leafgame-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clovers_leafgame-0.1.7.tar", max compression
+gzip compressed data, was "clovers_leafgame-0.1.8.tar", max compression
```

## Comparing `clovers_leafgame-0.1.7.tar` & `clovers_leafgame-0.1.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      300 2024-04-27 08:49:20.730233 clovers_leafgame-0.1.7/clovers_leafgame/__init__.py
--rw-r--r--   0        0        0      682 2024-04-27 08:49:20.730233 clovers_leafgame-0.1.7/clovers_leafgame/config.py
--rw-r--r--   0        0        0     4000 2024-04-27 08:49:20.730733 clovers_leafgame-0.1.7/clovers_leafgame/core/clovers.py
--rw-r--r--   0        0        0     5568 2024-04-27 09:13:40.955639 clovers_leafgame-0.1.7/clovers_leafgame/core/data.py
--rw-r--r--   0        0        0     1617 2024-04-27 08:49:20.731606 clovers_leafgame-0.1.7/clovers_leafgame/item.py
--rw-r--r--   0        0        0     1151 2024-04-27 08:49:20.731606 clovers_leafgame-0.1.7/clovers_leafgame/main.py
--rw-r--r--   0        0        0     6491 2024-04-27 08:49:20.732220 clovers_leafgame-0.1.7/clovers_leafgame/manager.py
--rw-r--r--   0        0        0    14551 2024-04-27 08:49:20.732603 clovers_leafgame-0.1.7/clovers_leafgame/modules/account/__init__.py
--rw-r--r--   0        0        0      347 2024-04-27 08:49:20.733113 clovers_leafgame-0.1.7/clovers_leafgame/modules/account/config.py
--rw-r--r--   0        0        0    44581 2024-04-27 09:44:32.582838 clovers_leafgame-0.1.7/clovers_leafgame/modules/game/__init__.py
--rw-r--r--   0        0        0      153 2024-04-27 08:49:20.733802 clovers_leafgame-0.1.7/clovers_leafgame/modules/game/config.py
--rw-r--r--   0        0        0     8755 2024-04-27 08:49:20.734312 clovers_leafgame-0.1.7/clovers_leafgame/modules/game/core.py
--rw-r--r--   0        0        0    10104 2024-04-27 08:49:20.734812 clovers_leafgame-0.1.7/clovers_leafgame/modules/game/fortress/core.py
--rw-r--r--   0        0        0    12802 2024-04-27 08:49:20.735312 clovers_leafgame-0.1.7/clovers_leafgame/modules/game/horse_race/__init__.py
--rw-r--r--   0        0        0      447 2024-04-27 08:49:20.735312 clovers_leafgame-0.1.7/clovers_leafgame/modules/game/horse_race/config.py
--rw-r--r--   0        0        0     5817 2024-04-27 08:49:20.735812 clovers_leafgame-0.1.7/clovers_leafgame/modules/game/horse_race/event_library/Stand.json
--rw-r--r--   0        0        0     5728 2024-04-27 08:49:20.736312 clovers_leafgame-0.1.7/clovers_leafgame/modules/game/horse_race/event_library/“日常，真的很日常”.json
--rw-r--r--   0        0        0     2174 2024-04-27 08:49:20.736811 clovers_leafgame-0.1.7/clovers_leafgame/modules/game/horse_race/event_library/克苏鲁.json
--rw-r--r--   0        0        0     1231 2024-04-27 08:49:20.736811 clovers_leafgame-0.1.7/clovers_leafgame/modules/game/horse_race/event_library/基础事件.json
--rw-r--r--   0        0        0     2742 2024-04-27 08:49:20.737312 clovers_leafgame-0.1.7/clovers_leafgame/modules/game/horse_race/event_library/复刻经典事件集合v1.json
--rw-r--r--   0        0        0     1606 2024-04-27 08:49:20.737312 clovers_leafgame-0.1.7/clovers_leafgame/modules/game/horse_race/event_library/崩坏集合v1.json
--rw-r--r--   0        0        0    25830 2024-04-27 08:49:20.737811 clovers_leafgame-0.1.7/clovers_leafgame/modules/game/horse_race/event_library/群友日常.json
--rw-r--r--   0        0        0     5180 2024-04-27 08:49:20.738314 clovers_leafgame-0.1.7/clovers_leafgame/modules/game/horse_race/event_library/芜湖事件合集.json
--rw-r--r--   0        0        0     1072 2024-04-27 08:49:20.738314 clovers_leafgame-0.1.7/clovers_leafgame/modules/game/horse_race/event_library/赫尔事件集v1.json
--rw-r--r--   0        0        0     2294 2024-04-27 08:49:20.738812 clovers_leafgame-0.1.7/clovers_leafgame/modules/game/horse_race/event_library/赫尔的赛马场事件簿.json
--rw-r--r--   0        0        0     7488 2024-04-27 08:49:20.738812 clovers_leafgame-0.1.7/clovers_leafgame/modules/game/horse_race/horse.py
--rw-r--r--   0        0        0      933 2024-04-27 08:49:20.739312 clovers_leafgame-0.1.7/clovers_leafgame/modules/game/horse_race/start.py
--rw-r--r--   0        0        0      754 2024-04-27 08:49:20.739812 clovers_leafgame-0.1.7/clovers_leafgame/modules/game/tools.py
--rw-r--r--   0        0        0    18182 2024-04-27 08:49:20.740312 clovers_leafgame-0.1.7/clovers_leafgame/modules/market/__init__.py
--rw-r--r--   0        0        0      457 2024-04-27 08:49:20.740820 clovers_leafgame-0.1.7/clovers_leafgame/modules/market/config.py
--rw-r--r--   0        0        0    12241 2024-04-27 08:49:20.740820 clovers_leafgame-0.1.7/clovers_leafgame/modules/prop/__init__.py
--rw-r--r--   0        0        0      271 2024-04-27 08:49:20.741311 clovers_leafgame-0.1.7/clovers_leafgame/modules/prop/config.py
--rw-r--r--   0        0        0     2085 2024-04-27 08:49:20.741812 clovers_leafgame-0.1.7/clovers_leafgame/modules/prop/core.py
--rw-r--r--   0        0        0     2681 2024-04-27 08:49:20.741812 clovers_leafgame-0.1.7/clovers_leafgame/modules/prop/output.py
--rw-r--r--   0        0        0     4516 2024-04-27 08:49:20.742312 clovers_leafgame-0.1.7/clovers_leafgame/modules/prop/props_library.json
--rw-r--r--   0        0        0     3958 2024-04-27 08:49:20.742812 clovers_leafgame-0.1.7/clovers_leafgame/modules/ranklist/__init__.py
--rw-r--r--   0        0        0     1003 2024-04-27 08:49:20.742812 clovers_leafgame-0.1.7/clovers_leafgame/modules/ranklist/output.py
--rw-r--r--   0        0        0     3587 2024-04-27 09:15:30.718836 clovers_leafgame-0.1.7/clovers_leafgame/modules/task/__init__.py
--rw-r--r--   0        0        0     6592 2024-04-27 08:49:20.743811 clovers_leafgame-0.1.7/clovers_leafgame/output.py
--rw-r--r--   0        0        0     1806 2024-04-27 09:12:59.164148 clovers_leafgame-0.1.7/clovers_leafgame/props_library.json
--rw-r--r--   0        0        0     1086 2024-04-27 08:49:20.729233 clovers_leafgame-0.1.7/LICENSE
--rw-r--r--   0        0        0      428 2024-04-27 14:31:41.539010 clovers_leafgame-0.1.7/pyproject.toml
--rw-r--r--   0        0        0    18955 2024-04-27 09:20:13.625406 clovers_leafgame-0.1.7/README.md
--rw-r--r--   0        0        0    18663 1970-01-01 00:00:00.000000 clovers_leafgame-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      300 2024-04-27 08:49:20.730233 clovers_leafgame-0.1.8/clovers_leafgame/__init__.py
+-rw-r--r--   0        0        0      682 2024-04-27 08:49:20.730233 clovers_leafgame-0.1.8/clovers_leafgame/config.py
+-rw-r--r--   0        0        0     4001 2024-05-01 06:15:17.412881 clovers_leafgame-0.1.8/clovers_leafgame/core/clovers.py
+-rw-r--r--   0        0        0     5568 2024-04-27 09:13:40.955639 clovers_leafgame-0.1.8/clovers_leafgame/core/data.py
+-rw-r--r--   0        0        0     1617 2024-04-27 08:49:20.731606 clovers_leafgame-0.1.8/clovers_leafgame/item.py
+-rw-r--r--   0        0        0     1151 2024-04-27 08:49:20.731606 clovers_leafgame-0.1.8/clovers_leafgame/main.py
+-rw-r--r--   0        0        0     6630 2024-05-01 02:31:44.190645 clovers_leafgame-0.1.8/clovers_leafgame/manager.py
+-rw-r--r--   0        0        0    14551 2024-05-01 01:41:25.978756 clovers_leafgame-0.1.8/clovers_leafgame/modules/account/__init__.py
+-rw-r--r--   0        0        0      347 2024-04-27 08:49:20.733113 clovers_leafgame-0.1.8/clovers_leafgame/modules/account/config.py
+-rw-r--r--   0        0        0    44586 2024-05-01 02:45:31.478949 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/__init__.py
+-rw-r--r--   0        0        0      153 2024-04-27 08:49:20.733802 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/config.py
+-rw-r--r--   0        0        0     8755 2024-04-27 08:49:20.734312 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/core.py
+-rw-r--r--   0        0        0    10104 2024-04-27 08:49:20.734812 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/fortress/core.py
+-rw-r--r--   0        0        0    12802 2024-04-27 08:49:20.735312 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/__init__.py
+-rw-r--r--   0        0        0      447 2024-04-27 08:49:20.735312 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/config.py
+-rw-r--r--   0        0        0     5817 2024-04-27 08:49:20.735812 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/Stand.json
+-rw-r--r--   0        0        0     5728 2024-04-27 08:49:20.736312 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/“日常，真的很日常”.json
+-rw-r--r--   0        0        0     2174 2024-04-27 08:49:20.736811 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/克苏鲁.json
+-rw-r--r--   0        0        0     1231 2024-04-27 08:49:20.736811 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/基础事件.json
+-rw-r--r--   0        0        0     2742 2024-04-27 08:49:20.737312 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/复刻经典事件集合v1.json
+-rw-r--r--   0        0        0     1606 2024-04-27 08:49:20.737312 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/崩坏集合v1.json
+-rw-r--r--   0        0        0    25830 2024-04-27 08:49:20.737811 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/群友日常.json
+-rw-r--r--   0        0        0     5180 2024-04-27 08:49:20.738314 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/芜湖事件合集.json
+-rw-r--r--   0        0        0     1072 2024-04-27 08:49:20.738314 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/赫尔事件集v1.json
+-rw-r--r--   0        0        0     2294 2024-04-27 08:49:20.738812 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/赫尔的赛马场事件簿.json
+-rw-r--r--   0        0        0     7488 2024-04-27 08:49:20.738812 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/horse.py
+-rw-r--r--   0        0        0      933 2024-04-27 08:49:20.739312 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/start.py
+-rw-r--r--   0        0        0      754 2024-04-27 08:49:20.739812 clovers_leafgame-0.1.8/clovers_leafgame/modules/game/tools.py
+-rw-r--r--   0        0        0    18182 2024-04-27 08:49:20.740312 clovers_leafgame-0.1.8/clovers_leafgame/modules/market/__init__.py
+-rw-r--r--   0        0        0      457 2024-04-27 08:49:20.740820 clovers_leafgame-0.1.8/clovers_leafgame/modules/market/config.py
+-rw-r--r--   0        0        0    12681 2024-05-01 06:16:15.242569 clovers_leafgame-0.1.8/clovers_leafgame/modules/prop/__init__.py
+-rw-r--r--   0        0        0      271 2024-04-27 08:49:20.741311 clovers_leafgame-0.1.8/clovers_leafgame/modules/prop/config.py
+-rw-r--r--   0        0        0     2085 2024-04-27 08:49:20.741812 clovers_leafgame-0.1.8/clovers_leafgame/modules/prop/core.py
+-rw-r--r--   0        0        0     2681 2024-04-27 08:49:20.741812 clovers_leafgame-0.1.8/clovers_leafgame/modules/prop/output.py
+-rw-r--r--   0        0        0     4516 2024-04-27 08:49:20.742312 clovers_leafgame-0.1.8/clovers_leafgame/modules/prop/props_library.json
+-rw-r--r--   0        0        0     3958 2024-04-27 08:49:20.742812 clovers_leafgame-0.1.8/clovers_leafgame/modules/ranklist/__init__.py
+-rw-r--r--   0        0        0     1003 2024-04-27 08:49:20.742812 clovers_leafgame-0.1.8/clovers_leafgame/modules/ranklist/output.py
+-rw-r--r--   0        0        0     3587 2024-04-27 09:15:30.718836 clovers_leafgame-0.1.8/clovers_leafgame/modules/task/__init__.py
+-rw-r--r--   0        0        0     6592 2024-04-27 08:49:20.743811 clovers_leafgame-0.1.8/clovers_leafgame/output.py
+-rw-r--r--   0        0        0     1806 2024-04-27 09:12:59.164148 clovers_leafgame-0.1.8/clovers_leafgame/props_library.json
+-rw-r--r--   0        0        0     1086 2024-04-27 08:49:20.729233 clovers_leafgame-0.1.8/LICENSE
+-rw-r--r--   0        0        0      428 2024-05-01 06:17:07.963060 clovers_leafgame-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0    18943 2024-04-27 15:58:16.641831 clovers_leafgame-0.1.8/README.md
+-rw-r--r--   0        0        0    18657 1970-01-01 00:00:00.000000 clovers_leafgame-0.1.8/PKG-INFO
```

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/config.py` & `clovers_leafgame-0.1.8/clovers_leafgame/config.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/core/clovers.py` & `clovers_leafgame-0.1.8/clovers_leafgame/core/clovers.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         return self
 
     def group_admin(self):
         self.checker.append(lambda event: event.permission > 0)
         return self
 
     def locate(self, user_id, group_id):
-        self.checker.append(lambda event: event.user_id == user_id or event.group_id == group_id)
+        self.checker.append(lambda event: event.user_id == user_id and event.group_id == group_id)
         return self
 
     def to_me(self):
         self.checker.append(lambda event: event.to_me)
         return self
 
     def at(self):
```

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/core/data.py` & `clovers_leafgame-0.1.8/clovers_leafgame/core/data.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/item.py` & `clovers_leafgame-0.1.8/clovers_leafgame/item.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/main.py` & `clovers_leafgame-0.1.8/clovers_leafgame/main.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/manager.py` & `clovers_leafgame-0.1.8/clovers_leafgame/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,22 +40,20 @@
         for group in self.data.group_dict.values():
             if (stock := group.stock) and (stock_name := stock.name):
                 self.group_library.set_item(group.id, {stock_name}, group)
             else:
                 self.group_library[group.id] = group
 
     def backup(self):
-        now = datetime.now().strftime("%Y-%m-%d %H-%M-%S")
-        date_today, now_time = now.split()
+        date_today, now_time = datetime.now().strftime("%Y-%m-%d %H-%M-%S").split()
         backup_today = self.backup_path / date_today
         if not backup_today.exists():
-            backup_today.mkdir()
-        self.save()
+            backup_today.mkdir(mode=755)
         file = backup_today / f"russian_data {now_time}.json"
-        file.write_text(self.data.model_dump_json(indent=4))
+        file.write_text(self.data.model_dump_json(indent=4), "utf8")
 
     def clean_backup(self, delta: int | float):
         folders = [f for f in self.backup_path.iterdir() if f.is_dir()]
         info = []
         for folder in folders:
             if datetime.now().timestamp() - folder.stat().st_birthtime > delta:
                 folder.unlink(True)
@@ -145,11 +143,17 @@
             if group and (stock := group.stock) and stock.name and stock.issuance > 0:
                 value += stock.value * n / stock.issuance
             else:
                 invest[group_id] = 0
         return int(value)
 
     def invest_data(self, bank: Counter[str]):
-        return [(stock, n) for group_id, n in bank.items() if n != 0 and (stock := self.group_library[group_id].stock)]
+        def get_stock(group_id: str):
+            group = self.group_library.get(group_id)
+            if not group:
+                return
+            return group.stock
+
+        return [(stock, n) for group_id, n in bank.items() if n != 0 and (stock := get_stock(group_id))]
 
     def props_data(self, bank: Counter[str]):
         return [(prop, n) for prop_id, n in bank.items() if n != 0 and (prop := self.props_library.get(prop_id))]
```

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/modules/account/__init__.py` & `clovers_leafgame-0.1.8/clovers_leafgame/modules/account/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/modules/game/__init__.py` & `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     elif user_id == session.p2_uid:
         session.win = session.p1_uid
     else:
         return
     return session.end()
 
 
-@plugin.handle({"游戏重置"}, {"user_id", "group_id", "permission"})
+@plugin.handle({"游戏重置", "清除对战"}, {"user_id", "group_id", "permission"})
 async def _(event: Event):
     group_id = event.group_id
     session = place.get(group_id)
     if not session:
         return
     if session.timeout() > 0 and event.permission < 1:
         return f"当前游戏未超时。"
@@ -124,15 +124,15 @@
     MAG = bullet[index:]
     count = event.args_to_int() or 1
     l_MAG = len(MAG)
     if count < 0 or count > l_MAG:
         count = l_MAG
     shot_tip = f"连开{count}枪！\n" if count > 1 else ""
     if any(MAG[:count]):
-        session.win = session.p2_uid if session.p2_uid == user_id else session.p1_uid
+        session.win = session.p1_uid if session.p2_uid == user_id else session.p2_uid
         random_tip = random.choice(["嘭！，你直接去世了", "眼前一黑，你直接穿越到了异世界...(死亡)", "终究还是你先走一步..."])
         result = f"{shot_tip}{random_tip}\n第 {index + MAG.index(1) + 1} 发子弹送走了你..."
         return session.end(result)
     else:
         session.nextround()
         session.data["index"] += count
         next_name = session.p1_nickname if session.next == session.p1_uid else session.p2_nickname
@@ -723,15 +723,15 @@
     session.data["MAG2"] = 1
     session.data["card"] = None
     if session.bet:
         prop, n = session.bet
         tip = f"\n本场下注：{n}{prop.name}/轮"
     else:
         tip = ""
-    return f"西部对战场地已创建。{tip}\n{session.create_info()}"
+    return f"【西部对战】游戏已创建。{tip}\n{session.create_info()}"
 
 
 def western_duel_action(event: Event, session: Session, card: str):
     if event.user_id == session.p1_uid:
         if not event.is_private():
             return "", "请私信发送指令。"
         session.data["card"] = card
@@ -923,15 +923,15 @@
     session.data["props2"] = []
     if session.bet:
         prop, n = session.bet
         tip = f"\n本场下注：{n}{prop.name}/轮"
     else:
         tip = ""
     session.start_tips = [buckshot_roulette_loading(session), buckshot_roulette_status(session)]
-    return f"【恶魔轮盘】场地已创建。{tip}\n{session.create_info()}"
+    return f"【恶魔轮盘】游戏已创建。{tip}\n{session.create_info()}"
 
 
 @plugin.handle(r"向(自己|对方)开枪$", {"user_id", "group_id"})
 @buckshot_roulette.action(place)
 async def _(event: Event, session: Session):
     user_id = event.user_id
     bullet = session.data["bullet"]
@@ -983,31 +983,32 @@
     return ["\n".join(result), buckshot_roulette_status(session)]
 
 
 @plugin.handle({"使用道具"}, {"user_id", "group_id"})
 @buckshot_roulette.action(place)
 async def _(event: Event, session: Session):
     prop_key = event.single_arg()
-    if not prop_key:
+    prop_tips = {
+        "手铐": "对方一回合无法行动",
+        "短锯": "本发子弹伤害翻倍",
+        "放大镜": "查看本发子弹",
+        "香烟": "增加1点血量",
+        "啤酒": "退一发子弹",
+        "逆转器": "转换当前枪膛里面的子弹真假",
+        "过期药品": "50%的概率回两滴血，剩下的概率扣一滴血",
+        "肾上腺素": "偷取对方的道具并立即使用",
+        "手机": "查看接下来第n发子弹真假",
+        "箱子": "每人抽取一件道具",
+    }
+    if not prop_key or prop_key not in prop_tips:
         return
     session.delay()
 
     def use(session: Session, prop_key: str):
-        prop_tips = {
-            "手铐": "对方一回合无法行动",
-            "短锯": "本发子弹伤害翻倍",
-            "放大镜": "查看本发子弹",
-            "香烟": "增加1点血量",
-            "啤酒": "退一发子弹",
-            "逆转器": "转换当前枪膛里面的子弹真假",
-            "过期药品": "50%的概率回两滴血，剩下的概率扣一滴血",
-            "肾上腺素": "偷取对方的道具并立即使用",
-            "手机": "查看接下来第n发子弹真假",
-            "箱子": "每人抽取一件道具",
-        }
+
         if session.next == session.p1_uid:
             self_key = "1"
             others_key = "2"
         else:
             self_key = "2"
             others_key = "1"
         props = f"props{self_key}"
```

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/modules/game/core.py` & `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/core.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/modules/game/fortress/core.py` & `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/fortress/core.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/modules/game/horse_race/__init__.py` & `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/modules/game/horse_race/event_library/Stand.json` & `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/Stand.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/modules/game/horse_race/event_library/“日常，真的很日常”.json` & `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/“日常，真的很日常”.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/modules/game/horse_race/event_library/克苏鲁.json` & `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/克苏鲁.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/modules/game/horse_race/event_library/基础事件.json` & `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/基础事件.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/modules/game/horse_race/event_library/复刻经典事件集合v1.json` & `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/复刻经典事件集合v1.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/modules/game/horse_race/event_library/崩坏集合v1.json` & `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/崩坏集合v1.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/modules/game/horse_race/event_library/群友日常.json` & `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/群友日常.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/modules/game/horse_race/event_library/芜湖事件合集.json` & `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/芜湖事件合集.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/modules/game/horse_race/event_library/赫尔事件集v1.json` & `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/赫尔事件集v1.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/modules/game/horse_race/event_library/赫尔的赛马场事件簿.json` & `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/event_library/赫尔的赛马场事件簿.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/modules/game/horse_race/horse.py` & `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/horse.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/modules/game/horse_race/start.py` & `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/horse_race/start.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/modules/game/tools.py` & `clovers_leafgame-0.1.8/clovers_leafgame/modules/game/tools.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/modules/market/__init__.py` & `clovers_leafgame-0.1.8/clovers_leafgame/modules/market/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/modules/prop/__init__.py` & `clovers_leafgame-0.1.8/clovers_leafgame/modules/prop/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,14 @@
         return f"使用失败，{prop.name}最小赌注为{luckey_min}金币"
     if count > luckey_max:
         return f"使用失败，{prop.name}最大赌注为{luckey_max}金币"
     bank = prop.locate_bank(user, account)
     if prop.deal(bank, -1):
         return f"使用失败，你没有足够的{prop.name}"
     GOLD.deal(account.bank, -count)
-
     if random.randint(0, 1) == 0:
         GOLD.deal(account.bank, count * 2)
         return f"你获得了{count}金币"
     else:
         RED_PACKET.deal(RED_PACKET.locate_bank(user, account), 1)
         return f"你失去了{count}金币。\n{event.event.kwargs['Bot_Nickname']}送你1个『随机红包』，祝你好运~"
 
@@ -196,15 +195,15 @@
     return f"你获得了{count}个【{target_prop.name}】！（使用金币：{gold}）"
 
 
 @usage("绯红迷雾之书", {"user_id", "group_id", "nickname"})
 async def _(prop: Prop, event: Event, count: int, extra: str):
     user_id = event.user_id
     bank = manager.data.user(user_id).bank
-    if prop.deal(bank, -1):
+    if bank[prop.id] < 1:
         return f"使用失败，你未持有{prop.name}"
     group_id = event.group_id
     folders = {f.name: f for f in manager.backup_path.iterdir() if f.is_dir()}
     tip = "请输入你要回档的日期:\n" + "\n".join(folders.keys())
     key = f"{user_id} {group_id}"
 
     @plugin.temp_handle(key, extra_args={"user_id", "group_id"})
@@ -224,14 +223,15 @@
             clock = event.raw_command
             file = files.get(clock)
             if not file:
                 return tip2
             manager.data.cancel_user(user_id)
             old_data = manager.data.load(file)
             user = manager.data.user_dict[user_id] = old_data.user(user_id)
+            user.bank[prop.id] = bank[prop.id] - 1
             for account_id in user.accounts_map.values():
                 manager.data.register(old_data.account_dict[account_id])
             finish()
             return f"你已经回档到{date} {clock}"
 
         return tip2
 
@@ -242,51 +242,61 @@
 async def _(prop: Prop, event: Event, count: int, extra: str):
     user_id = event.user_id
     group_id = event.group_id
     user = manager.data.user(user_id)
     if user.bank[prop.id] < 1:
         return f"使用失败，你没有足够的{prop.name}"
     group_id = event.group_id
+    rate = 1
 
-    def ten_times_bank(bank: Counter):
-        for k in bank.keys():
-            bank[k] *= 10
-
-    @plugin.temp_handle(f"{user_id} {group_id}", extra_args={"user_id", "group_id"})
-    async def _(event_1: Event, finish):
-        if event_1.user_id != user_id or event_1.group_id != group_id:
+    @plugin.temp_handle(f"{user_id} {group_id}", extra_args={"user_id", "group_id"}, timeout=120)
+    async def _(event: Event, finish):
+        if event.user_id != user_id or event.group_id != group_id:
             return
-        finish()
-        if event_1.raw_command == "取消":
-            return "恶魔轮盘已取消"
-        if event_1.raw_command != "开枪":
+        if event.raw_command == "取消":
+            finish()
+            if rate == 1:
+                return f"你取消了恶魔轮盘"
+
+            def rate_times_bank(bank: Counter, rate: int):
+                for k in bank.keys():
+                    bank[k] *= rate
+
+            counter = Counter()
+            rate_times_bank(user.bank, rate)
+            user.bank[prop.id] = 1
+            counter += user.bank
+            for account_id in user.accounts_map.values():
+                account = manager.data.account_dict[account_id]
+                rate_times_bank(account.bank, rate)
+                counter += account.bank
+            user.bank[STD_GOLD.id] += manager.stock_value(user.invest) * rate
+
+            return ["这是你获得的道具", manager.info_card([prop_card(manager.props_data(counter))], user_id)]
+
+        if event.raw_command != "开枪":
             return
 
         async def result():
             bullet_lst = [0, 0, 0, 0, 0, 0]
-            for i in random.sample([0, 1, 2, 3, 4, 5], random.randint(0, 6)):
+            for i in random.sample([0, 1, 2, 3, 4, 5], 3):
                 bullet_lst[i] = 1
             index = random.randint(0, 5)
             yield f"子弹列表{" ".join(str(x) for x in bullet_lst)}，你中了第{index+1}发子弹。"
-            await asyncio.sleep(1)
+            await asyncio.sleep(0.5)
+            nonlocal rate
             if bullet_lst[index] == 1:
-                manager.data.cancel_user(user_id)
-                yield "砰！一团火从枪口喷出，你从这个世界上消失了。"
-                return
-            counter = Counter()
-            ten_times_bank(user.bank)
-            user.bank[prop.id] = 1
-            counter += user.bank
-            for account_id in user.accounts_map.values():
-                account = manager.data.account_dict[account_id]
-                ten_times_bank(account.bank)
-                counter += account.bank
-            user.bank[STD_GOLD.id] += manager.stock_value(user.invest) * 10
-            yield "咔！你活了下来..."
-            yield [
-                "这是你获得的道具",
-                manager.info_card([prop_card(manager.props_data(counter))], user_id),
-            ]
+                if rate == 1:
+                    manager.data.cancel_user(user_id)
+                    finish()
+                    yield "砰！一团火从枪口喷出，你从这个世界上消失了。"
+                    return
+                rate //= 2
+                msg = "砰！一团火从枪口喷出...你被救活了..."
+            else:
+                rate *= 2
+                msg = "咔！你活了下来..."
+            yield msg + f"\n当前倍率：{rate}\n请继续开枪，或者取消。"
 
         return result()
 
     return "你手中的左轮枪已经装好了子弹，请开枪，或者取消。"
```

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/modules/prop/core.py` & `clovers_leafgame-0.1.8/clovers_leafgame/modules/prop/core.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/modules/prop/output.py` & `clovers_leafgame-0.1.8/clovers_leafgame/modules/prop/output.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/modules/prop/props_library.json` & `clovers_leafgame-0.1.8/clovers_leafgame/modules/prop/props_library.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/modules/ranklist/__init__.py` & `clovers_leafgame-0.1.8/clovers_leafgame/modules/ranklist/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/modules/ranklist/output.py` & `clovers_leafgame-0.1.8/clovers_leafgame/modules/ranklist/output.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/modules/task/__init__.py` & `clovers_leafgame-0.1.8/clovers_leafgame/modules/task/__init__.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/output.py` & `clovers_leafgame-0.1.8/clovers_leafgame/output.py`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/clovers_leafgame/props_library.json` & `clovers_leafgame-0.1.8/clovers_leafgame/props_library.json`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/LICENSE` & `clovers_leafgame-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `clovers_leafgame-0.1.7/README.md` & `clovers_leafgame-0.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,17 @@
 <div align="center">
 
 # clovers-leafgame
 
 _✨ 改自 [nonebot_plugin_russian](https://github.com/HibiKier/nonebot_plugin_russian) 和 [nonebot_plugin_horserace](https://github.com/shinianj/nonebot_plugin_horserace) 的小游戏合集 ✨_
 
 <img src="https://img.shields.io/badge/python-3.12+-blue.svg" alt="python">
-<a href="./LICENSE">
-<img src="https://img.shields.io/github/license/KarisAya/clovers_leafgame.svg" alt="license">
-</a>
-<a href="https://pypi.python.org/pypi/clovers_leafgame">
-<img src="https://img.shields.io/pypi/v/clovers_leafgame.svg" alt="pypi">
-</a>
-<a href="https://pypi.python.org/pypi/clovers_leafgame">
-<img src="https://img.shields.io/pypi/dm/clovers_leafgame" alt="pypi download">
-</a>
+<a href="./LICENSE"><img src="https://img.shields.io/github/license/KarisAya/clovers_leafgame.svg" alt="license"></a>
+<a href="https://pypi.python.org/pypi/clovers_leafgame"><img src="https://img.shields.io/pypi/v/clovers_leafgame.svg" alt="pypi"></a>
+<a href="https://pypi.python.org/pypi/clovers_leafgame"><img src="https://img.shields.io/pypi/dm/clovers_leafgame" alt="pypi download"></a>
 
 </div>
 
 ## 💿 安装
 
 ```bash
 pip install clovers_leafgame
```

### Comparing `clovers_leafgame-0.1.7/PKG-INFO` & `clovers_leafgame-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clovers-leafgame
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: KarisAya
 Author-email: 1048827424@qq.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: clovers-apscheduler (>=0.1.3,<0.2.0)
 Requires-Dist: clovers[linecard,tools] (>=0.1.8,<0.2.0)
@@ -16,23 +16,17 @@
 <div align="center">
 
 # clovers-leafgame
 
 _✨ 改自 [nonebot_plugin_russian](https://github.com/HibiKier/nonebot_plugin_russian) 和 [nonebot_plugin_horserace](https://github.com/shinianj/nonebot_plugin_horserace) 的小游戏合集 ✨_
 
 <img src="https://img.shields.io/badge/python-3.12+-blue.svg" alt="python">
-<a href="./LICENSE">
-<img src="https://img.shields.io/github/license/KarisAya/clovers_leafgame.svg" alt="license">
-</a>
-<a href="https://pypi.python.org/pypi/clovers_leafgame">
-<img src="https://img.shields.io/pypi/v/clovers_leafgame.svg" alt="pypi">
-</a>
-<a href="https://pypi.python.org/pypi/clovers_leafgame">
-<img src="https://img.shields.io/pypi/dm/clovers_leafgame" alt="pypi download">
-</a>
+<a href="./LICENSE"><img src="https://img.shields.io/github/license/KarisAya/clovers_leafgame.svg" alt="license"></a>
+<a href="https://pypi.python.org/pypi/clovers_leafgame"><img src="https://img.shields.io/pypi/v/clovers_leafgame.svg" alt="pypi"></a>
+<a href="https://pypi.python.org/pypi/clovers_leafgame"><img src="https://img.shields.io/pypi/dm/clovers_leafgame" alt="pypi download"></a>
 
 </div>
 
 ## 💿 安装
 
 ```bash
 pip install clovers_leafgame
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clovers-leafgame Version: 0.1.7 Summary: Author:
+Metadata-Version: 2.1 Name: clovers-leafgame Version: 0.1.8 Summary: Author:
 KarisAya Author-email: 1048827424@qq.com Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3 Requires-Dist: clovers-
 apscheduler (>=0.1.3,<0.2.0) Requires-Dist: clovers[linecard,tools]
 (>=0.1.8,<0.2.0) Requires-Dist: mplfinance (>=0.12.10b0,<0.13.0) Requires-Dist:
 pydantic (>=2.7.0,<3.0.0) Description-Content-Type: text/markdown
   # clovers-leafgame _â¨ æ¹èª [nonebot_plugin_russian](https://github.com/
    HibiKier/nonebot_plugin_russian) å [nonebot_plugin_horserace](https://
```


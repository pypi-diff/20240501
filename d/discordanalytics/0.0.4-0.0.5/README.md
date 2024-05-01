# Comparing `tmp/discordanalytics-0.0.4.tar.gz` & `tmp/discordanalytics-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discordanalytics-0.0.4.tar", last modified: Sun Apr  7 14:42:11 2024, max compression
+gzip compressed data, was "discordanalytics-0.0.5.tar", last modified: Wed May  1 16:39:43 2024, max compression
```

## Comparing `discordanalytics-0.0.4.tar` & `discordanalytics-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:42:11.865636 discordanalytics-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-07 14:42:07.000000 discordanalytics-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-07 14:42:11.861636 discordanalytics-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-07 14:42:07.000000 discordanalytics-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:42:11.861636 discordanalytics-0.0.4/discordanalytics/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-07 14:42:07.000000 discordanalytics-0.0.4/discordanalytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-07 14:42:07.000000 discordanalytics-0.0.4/discordanalytics/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:42:11.861636 discordanalytics-0.0.4/discordanalytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-07 14:42:11.000000 discordanalytics-0.0.4/discordanalytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-07 14:42:11.000000 discordanalytics-0.0.4/discordanalytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:42:11.000000 discordanalytics-0.0.4/discordanalytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-07 14:42:11.000000 discordanalytics-0.0.4/discordanalytics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-07 14:42:07.000000 discordanalytics-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 14:42:11.865636 discordanalytics-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:39:43.816266 discordanalytics-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-01 16:39:39.000000 discordanalytics-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-01 16:39:43.816266 discordanalytics-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-01 16:39:39.000000 discordanalytics-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:39:43.816266 discordanalytics-0.0.5/discordanalytics/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-01 16:39:39.000000 discordanalytics-0.0.5/discordanalytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-05-01 16:39:39.000000 discordanalytics-0.0.5/discordanalytics/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:39:43.816266 discordanalytics-0.0.5/discordanalytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-01 16:39:43.000000 discordanalytics-0.0.5/discordanalytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-01 16:39:43.000000 discordanalytics-0.0.5/discordanalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:39:43.000000 discordanalytics-0.0.5/discordanalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 16:39:43.000000 discordanalytics-0.0.5/discordanalytics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-01 16:39:39.000000 discordanalytics-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 16:39:43.816266 discordanalytics-0.0.5/setup.cfg
```

### Comparing `discordanalytics-0.0.4/LICENSE` & `discordanalytics-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `discordanalytics-0.0.4/PKG-INFO` & `discordanalytics-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discordanalytics
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python package for interacting with Discord Analytics API
 Author-email: ValDesign <valdesign.dev@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Discord Analytics
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `discordanalytics-0.0.4/README.md` & `discordanalytics-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `discordanalytics-0.0.4/discordanalytics/client.py` & `discordanalytics-0.0.5/discordanalytics/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 from datetime import datetime
+from typing import Literal
 import discord
 from discord.enums import InteractionType
 import requests
 import sys
 
 from .__init__ import __version__
 
@@ -40,27 +41,36 @@
       "locales": [], # {locale:str, number:int}[]
       "guildsLocales": [], # {locale:str, number:int}[]
       "guildMembers": {
         "little": 0,
         "medium": 0,
         "big": 0,
         "huge": 0
-      }
+      },
+      "guildsStats": [], # {guildId:str, name:str, icon:str, members:int, interactions: int}[]
+      "addedGuilds": 0,
+      "removedGuilds": 0,
     }
   
   def track_events(self):
     if not self.client.is_ready():
       @self.client.event
       async def on_ready():
         self.init()
     else:
       self.init()
     @self.client.event
-    async def on_interaction(interaction):
+    async def on_interaction(interaction: discord.Interaction):
       self.track_interactions(interaction)
+    @self.client.event
+    async def on_guild_join(guild: discord.Guild):
+      self.trackGuilds(guild, "create")
+    @self.client.event
+    async def on_guild_remove(guild: discord.Guild):
+      self.trackGuilds(guild, "delete")
   
   def init(self):
     if not isinstance(self.client, discord.Client):
       raise ValueError(ErrorCodes.INVALID_CLIENT_TYPE)
     if not self.client.is_ready():
       raise ValueError(ErrorCodes.CLIENT_NOT_READY)
     
@@ -122,15 +132,18 @@
         self.stats = {
           "date": datetime.today().strftime("%Y-%m-%d"),
           "guilds": guild_count,
           "users": user_count,
           "interactions": [],
           "locales": [],
           "guildsLocales": [],
-          "guildMembers": self.calculate_guild_members_repartition()
+          "guildMembers": self.calculate_guild_members_repartition(),
+          "guildsStats": [],
+          "addedGuilds": 0,
+          "removedGuilds": 0,
         }
       
       await asyncio.sleep(10 if "--dev" in sys.argv else 300)
 
   def calculate_guild_members_repartition(self):
     result = {
       "little": 0,
@@ -147,67 +160,79 @@
       elif 500 < guild.member_count <= 1500:
         result["big"] += 1
       else:
         result["huge"] += 1
 
     return result
   
-  def track_interactions(self, interaction):
+  def track_interactions(self, interaction: discord.Interaction):
     if self.debug:
       print("[DISCORDANALYTICS] Track interactions triggered")
     if not self.is_ready:
       raise ValueError(ErrorCodes.INSTANCE_NOT_INITIALIZED)
     
     guilds = []
     for guild in self.client.guilds:
       if guild.preferred_locale is not None:
-        found = False
-        for g in guilds:
-          if g["locale"] == guild.preferred_locale.value:
-            g["number"] += 1
-            found = True
-            break
-        if not found:
+        guild_locale = next((x for x in guilds if x["locale"] == guild.preferred_locale.value), None)
+        if guild_locale is not None:
+          guild_locale["number"] += 1
+        else:
           guilds.append({
             "locale": guild.preferred_locale.value,
             "number": 1
           })
     self.stats["guildsLocales"] = guilds
     
-    found = False
-    for data in self.stats["locales"]:
-      if data["locale"] == interaction.locale.value:
-        data["number"] += 1
-        found = True
-        break
-    if not found:
+    locale = next((x for x in self.stats["locales"] if x["locale"] == interaction.locale.value), None)
+    if locale is not None:
+      locale["number"] += 1
+    else:
       self.stats["locales"].append({
         "locale": interaction.locale.value,
         "number": 1
       })
 
     if interaction.type == InteractionType.application_command or interaction.type == InteractionType.autocomplete:
-      found = False
-      for data in self.stats["interactions"]:
-        if data["name"] == interaction.data["name"] and data["type"] == interaction.type.value:
-          data["number"] += 1
-          found = True
-          break
-      if not found:
+      interaction_data = next((x for x in self.stats["interactions"] if x["name"] == interaction.data["name"] and x["type"] == interaction.type.value), None)
+      if interaction_data is not None:
+        interaction_data["number"] += 1
+      else:
         self.stats["interactions"].append({
           "name": interaction.data["name"],
           "number": 1,
           "type": interaction.type.value
         })
     elif interaction.type == InteractionType.component or interaction.type == InteractionType.modal_submit:
-      found = False
-      for data in self.stats["interactions"]:
-        if data["name"] == interaction.data["custom_id"] and data["type"] == interaction.type.value:
-          data["number"] += 1
-          found = True
-          break
-      if not found:
+      interaction_data = next((x for x in self.stats["interactions"] if x["name"] == interaction.data["custom_id"] and x["type"] == interaction.type.value), None)
+      if interaction_data is not None:
+        interaction_data["number"] += 1
+      else:
         self.stats["interactions"].append({
           "name": interaction.data["custom_id"],
           "number": 1,
           "type": interaction.type.value
-        })
+        })
+
+    guild_data = next((x for x in self.stats["guildsStats"] if x["guildId"] == str(interaction.guild.id)), None)
+    if guild_data is not None:
+      guild_data["interactions"] += 1
+    else:
+      self.stats["guildsStats"].append({
+        "guildId": str(interaction.guild.id),
+        "name": interaction.guild.name,
+        "icon": interaction.guild.icon,
+        "members": interaction.guild.member_count,
+        "interactions": 1
+      })
+
+  # type = delete or create
+  def trackGuilds(self, guild: discord.Guild, type: Literal["create", "delete"]):
+    if self.debug:
+      print(f"[DISCORDANALYTICS] trackGuilds({type}) triggered")
+
+    if type == "create":
+      self.stats["addedGuilds"] += 1
+    elif type == "delete":
+      self.stats["removedGuilds"] += 1
+    else:
+      raise ValueError(ErrorCodes.INVALID_EVENTS_COUNT)
```

### Comparing `discordanalytics-0.0.4/discordanalytics.egg-info/PKG-INFO` & `discordanalytics-0.0.5/discordanalytics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discordanalytics
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python package for interacting with Discord Analytics API
 Author-email: ValDesign <valdesign.dev@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Discord Analytics
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```


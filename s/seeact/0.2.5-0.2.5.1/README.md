# Comparing `tmp/seeact-0.2.5.tar.gz` & `tmp/seeact-0.2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seeact-0.2.5.tar", last modified: Mon Apr 29 22:22:35 2024, max compression
+gzip compressed data, was "seeact-0.2.5.1.tar", last modified: Wed May  1 01:20:55 2024, max compression
```

## Comparing `seeact-0.2.5.tar` & `seeact-0.2.5.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 22:22:35.308222 seeact-0.2.5/
--rw-r--r--   0 geminigby   (501) staff       (20)    11495 2024-04-29 00:05:59.000000 seeact-0.2.5/LICENSE
--rw-r--r--   0 geminigby   (501) staff       (20)    13352 2024-04-29 22:22:35.305351 seeact-0.2.5/PKG-INFO
--rw-r--r--   0 geminigby   (501) staff       (20)     1123 2024-04-29 22:22:10.000000 seeact-0.2.5/pyproject.toml
-drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 22:22:35.296302 seeact-0.2.5/seeact/
--rw-r--r--   0 geminigby   (501) staff       (20)      607 2024-04-29 00:05:59.000000 seeact-0.2.5/seeact/__init__.py
--rw-r--r--   0 geminigby   (501) staff       (20)    32246 2024-04-29 22:21:29.000000 seeact-0.2.5/seeact/agent.py
-drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 22:22:35.300897 seeact-0.2.5/seeact/data_utils/
--rw-r--r--   0 geminigby   (501) staff       (20)      607 2024-04-29 00:05:59.000000 seeact-0.2.5/seeact/data_utils/__init__.py
--rw-r--r--   0 geminigby   (501) staff       (20)     4278 2024-04-29 00:05:59.000000 seeact-0.2.5/seeact/data_utils/format_prompt_utils.py
--rw-r--r--   0 geminigby   (501) staff       (20)     7487 2024-04-29 00:05:59.000000 seeact-0.2.5/seeact/data_utils/prompts.py
-drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 22:22:35.303202 seeact-0.2.5/seeact/demo_utils/
--rw-r--r--   0 geminigby   (501) staff       (20)        0 2024-04-29 00:05:59.000000 seeact-0.2.5/seeact/demo_utils/__init__.py
--rw-r--r--   0 geminigby   (501) staff       (20)    13193 2024-04-29 00:45:49.000000 seeact-0.2.5/seeact/demo_utils/browser_helper.py
--rw-r--r--   0 geminigby   (501) staff       (20)     7555 2024-04-29 00:05:59.000000 seeact-0.2.5/seeact/demo_utils/format_prompt.py
--rw-r--r--   0 geminigby   (501) staff       (20)     8411 2024-04-29 00:05:59.000000 seeact-0.2.5/seeact/demo_utils/inference_engine.py
-drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 22:22:35.304284 seeact-0.2.5/seeact.egg-info/
--rw-r--r--   0 geminigby   (501) staff       (20)    13352 2024-04-29 22:22:35.000000 seeact-0.2.5/seeact.egg-info/PKG-INFO
--rw-r--r--   0 geminigby   (501) staff       (20)      445 2024-04-29 22:22:35.000000 seeact-0.2.5/seeact.egg-info/SOURCES.txt
--rw-r--r--   0 geminigby   (501) staff       (20)        1 2024-04-29 22:22:35.000000 seeact-0.2.5/seeact.egg-info/dependency_links.txt
--rw-r--r--   0 geminigby   (501) staff       (20)       53 2024-04-29 22:22:35.000000 seeact-0.2.5/seeact.egg-info/requires.txt
--rw-r--r--   0 geminigby   (501) staff       (20)        7 2024-04-29 22:22:35.000000 seeact-0.2.5/seeact.egg-info/top_level.txt
--rw-r--r--   0 geminigby   (501) staff       (20)       38 2024-04-29 22:22:35.308475 seeact-0.2.5/setup.cfg
+drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-05-01 01:20:55.034831 seeact-0.2.5.1/
+-rw-r--r--   0 geminigby   (501) staff       (20)    11495 2024-04-29 00:05:59.000000 seeact-0.2.5.1/LICENSE
+-rw-r--r--   0 geminigby   (501) staff       (20)    13354 2024-05-01 01:20:55.034534 seeact-0.2.5.1/PKG-INFO
+-rw-r--r--   0 geminigby   (501) staff       (20)     1125 2024-05-01 01:20:06.000000 seeact-0.2.5.1/pyproject.toml
+drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-05-01 01:20:55.031171 seeact-0.2.5.1/seeact/
+-rw-r--r--   0 geminigby   (501) staff       (20)      607 2024-04-29 00:05:59.000000 seeact-0.2.5.1/seeact/__init__.py
+-rw-r--r--   0 geminigby   (501) staff       (20)    32246 2024-04-29 22:20:31.000000 seeact-0.2.5.1/seeact/agent.py
+drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-05-01 01:20:55.032922 seeact-0.2.5.1/seeact/data_utils/
+-rw-r--r--   0 geminigby   (501) staff       (20)      607 2024-04-29 00:05:59.000000 seeact-0.2.5.1/seeact/data_utils/__init__.py
+-rw-r--r--   0 geminigby   (501) staff       (20)     4278 2024-05-01 01:16:18.000000 seeact-0.2.5.1/seeact/data_utils/format_prompt_utils.py
+-rw-r--r--   0 geminigby   (501) staff       (20)     7487 2024-04-29 00:05:59.000000 seeact-0.2.5.1/seeact/data_utils/prompts.py
+drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-05-01 01:20:55.033893 seeact-0.2.5.1/seeact/demo_utils/
+-rw-r--r--   0 geminigby   (501) staff       (20)        0 2024-04-29 00:05:59.000000 seeact-0.2.5.1/seeact/demo_utils/__init__.py
+-rw-r--r--   0 geminigby   (501) staff       (20)    13193 2024-04-29 00:45:49.000000 seeact-0.2.5.1/seeact/demo_utils/browser_helper.py
+-rw-r--r--   0 geminigby   (501) staff       (20)     7554 2024-05-01 01:16:18.000000 seeact-0.2.5.1/seeact/demo_utils/format_prompt.py
+-rw-r--r--   0 geminigby   (501) staff       (20)     8411 2024-04-29 00:05:59.000000 seeact-0.2.5.1/seeact/demo_utils/inference_engine.py
+drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-05-01 01:20:55.034236 seeact-0.2.5.1/seeact.egg-info/
+-rw-r--r--   0 geminigby   (501) staff       (20)    13354 2024-05-01 01:20:55.000000 seeact-0.2.5.1/seeact.egg-info/PKG-INFO
+-rw-r--r--   0 geminigby   (501) staff       (20)      445 2024-05-01 01:20:55.000000 seeact-0.2.5.1/seeact.egg-info/SOURCES.txt
+-rw-r--r--   0 geminigby   (501) staff       (20)        1 2024-05-01 01:20:55.000000 seeact-0.2.5.1/seeact.egg-info/dependency_links.txt
+-rw-r--r--   0 geminigby   (501) staff       (20)       53 2024-05-01 01:20:55.000000 seeact-0.2.5.1/seeact.egg-info/requires.txt
+-rw-r--r--   0 geminigby   (501) staff       (20)        7 2024-05-01 01:20:55.000000 seeact-0.2.5.1/seeact.egg-info/top_level.txt
+-rw-r--r--   0 geminigby   (501) staff       (20)       38 2024-05-01 01:20:55.034879 seeact-0.2.5.1/setup.cfg
```

### Comparing `seeact-0.2.5/LICENSE` & `seeact-0.2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seeact-0.2.5/PKG-INFO` & `seeact-0.2.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeact
-Version: 0.2.5
+Version: 0.2.5.1
 Summary: SeeAct is a system for generalist web agents that autonomously carry out tasks on any given website, with a focus on large multimodal models (LMMs) such as GPT-4V(ision). It consists of two main components: (1) A robust codebase that supports running web agents on live websites, and (2) an innovative framework that utilizes LMMs as generalist web agents.
 Author-email: Boyu Gou <gou.43@buckeyemail.osu.edu>, Boyuan Zheng <zheng.2372@osu.edu>, Zheng Du <du.913@buckeyemail.osu.edu>
 License: AI PUBS OPEN RAIL-S LICENSE
         Version 0.1, March 2, 2023
         
         http://licenses.ai/
```

### Comparing `seeact-0.2.5/pyproject.toml` & `seeact-0.2.5.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "seeact"
-version = "0.2.5"
+version = "0.2.5.1"
 description = "SeeAct is a system for generalist web agents that autonomously carry out tasks on any given website, with a focus on large multimodal models (LMMs) such as GPT-4V(ision). It consists of two main components: (1) A robust codebase that supports running web agents on live websites, and (2) an innovative framework that utilizes LMMs as generalist web agents."
 authors = [
     {name = "Boyu Gou", email = "gou.43@buckeyemail.osu.edu"},
     {name = "Boyuan Zheng", email = "zheng.2372@osu.edu"},
     {name = "Zheng Du", email = "du.913@buckeyemail.osu.edu"}
 ]
 license = {file="LICENSE"}
```

### Comparing `seeact-0.2.5/seeact/__init__.py` & `seeact-0.2.5.1/seeact/__init__.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.5/seeact/agent.py` & `seeact-0.2.5.1/seeact/agent.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.5/seeact/data_utils/__init__.py` & `seeact-0.2.5.1/seeact/data_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.5/seeact/data_utils/format_prompt_utils.py` & `seeact-0.2.5.1/seeact/data_utils/format_prompt_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     multi_choice = ''
     for multichoice_idx, choice in enumerate(choices):
         multi_choice += f"{generate_option_name(multichoice_idx)}. {choice}\n"
         abcd += f"{generate_option_name(multichoice_idx)}, "
 
         non_abcd = generate_option_name(multichoice_idx + 1)
 
-    multi_choice += f"{non_abcd}. None of the other options match the correct element or the action doesn't invlove an element."
+    multi_choice += f"{non_abcd}. None of the other options match the correct element or the action doesn't involve an element."
     # option_text += abcd
     option_text += f"If none of these elements match your target element or your target action doesn't involve an element, please select {non_abcd}.\n"
     option_text += (multi_choice + '\n\n')
     return option_text
 
 
 def generate_option_name(index):
```

### Comparing `seeact-0.2.5/seeact/data_utils/prompts.py` & `seeact-0.2.5.1/seeact/data_utils/prompts.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.5/seeact/demo_utils/browser_helper.py` & `seeact-0.2.5.1/seeact/demo_utils/browser_helper.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.5/seeact/demo_utils/format_prompt.py` & `seeact-0.2.5.1/seeact/demo_utils/format_prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                     + (
                         element["description"]
                         if len(element["description"].split()) < 30
                         else " ".join(element["description"].split()[:30]) + "..."
                     )
                     + f"</{element['tag']}>"
 
-                    if element['tag']!="select" else f'{element["center_point"]} <{element["tag_with_role"]}">'
+                    if element['tag']!="select" else f'{element["center_point"]} <{element["tag_with_role"]}>'
                     + (
                         element["description"]
                     )
                     + f"</{element['tag']}>"
                     for i, element in enumerate(elements)
                 ]
```

### Comparing `seeact-0.2.5/seeact/demo_utils/inference_engine.py` & `seeact-0.2.5.1/seeact/demo_utils/inference_engine.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.5/seeact.egg-info/PKG-INFO` & `seeact-0.2.5.1/seeact.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeact
-Version: 0.2.5
+Version: 0.2.5.1
 Summary: SeeAct is a system for generalist web agents that autonomously carry out tasks on any given website, with a focus on large multimodal models (LMMs) such as GPT-4V(ision). It consists of two main components: (1) A robust codebase that supports running web agents on live websites, and (2) an innovative framework that utilizes LMMs as generalist web agents.
 Author-email: Boyu Gou <gou.43@buckeyemail.osu.edu>, Boyuan Zheng <zheng.2372@osu.edu>, Zheng Du <du.913@buckeyemail.osu.edu>
 License: AI PUBS OPEN RAIL-S LICENSE
         Version 0.1, March 2, 2023
         
         http://licenses.ai/
```


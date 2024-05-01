# Comparing `tmp/aocstat-0.2.2.tar.gz` & `tmp/aocstat-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aocstat-0.2.2.tar", max compression
+gzip compressed data, was "aocstat-0.2.3.tar", max compression
```

## Comparing `aocstat-0.2.2.tar` & `aocstat-0.2.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2024-04-30 23:54:12.504859 aocstat-0.2.2/LICENSE
--rw-r--r--   0        0        0       68 2024-04-30 23:58:10.851359 aocstat-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-06-29 22:54:27.632641 aocstat-0.2.2/aocstat/__init__.py
--rw-r--r--   0        0        0    13236 2024-04-30 23:58:10.851359 aocstat-0.2.2/aocstat/api.py
--rw-r--r--   0        0        0     2833 2024-04-30 23:58:10.851359 aocstat-0.2.2/aocstat/config.py
--rw-r--r--   0        0        0     7054 2024-05-01 00:06:55.741258 aocstat-0.2.2/aocstat/format.py
--rw-r--r--   0        0        0     7421 2024-05-01 00:13:49.321301 aocstat-0.2.2/aocstat/main.py
--rw-r--r--   0        0        0      538 2024-05-01 00:14:09.701305 aocstat-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      677 1970-01-01 00:00:00.000000 aocstat-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-30 23:54:12.504859 aocstat-0.2.3/LICENSE
+-rw-r--r--   0        0        0       68 2024-04-30 23:58:10.851359 aocstat-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-29 22:54:27.632641 aocstat-0.2.3/aocstat/__init__.py
+-rw-r--r--   0        0        0    13246 2024-05-01 00:34:02.457323 aocstat-0.2.3/aocstat/api.py
+-rw-r--r--   0        0        0     2833 2024-04-30 23:58:10.851359 aocstat-0.2.3/aocstat/config.py
+-rw-r--r--   0        0        0     7054 2024-05-01 00:06:55.741258 aocstat-0.2.3/aocstat/format.py
+-rw-r--r--   0        0        0     7692 2024-05-01 00:34:06.754006 aocstat-0.2.3/aocstat/main.py
+-rw-r--r--   0        0        0      538 2024-05-01 00:35:04.110880 aocstat-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      677 1970-01-01 00:00:00.000000 aocstat-0.2.3/PKG-INFO
```

### Comparing `aocstat-0.2.2/LICENSE` & `aocstat-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aocstat-0.2.2/aocstat/api.py` & `aocstat-0.2.3/aocstat/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
     total_score = entry_soup.find("span", {"class": "leaderboard-totalscore"})
     entry["total_score"] = (
         int(total_score.contents[0]) if total_score is not None else None
     )
 
     # first we check to see if they have a linked github
     name_link = entry_soup.find(
-        "a", {"href": re.compile(r"^https:\/\/github\.com\/.+$")}
+        "a", {"href": re.compile(r"^https:\/\/(github|twitter)\.com\/.+$")}
     )
     anon_name = entry_soup.find("span", {"class": "leaderboard-anon"})
     time = entry_soup.find("span", {"class": "leaderboard-time"})
     if name_link is not None:
         entry["name"] = name_link.contents[-1]
     else:
         # then to see if they are an anonomous user
```

### Comparing `aocstat-0.2.2/aocstat/config.py` & `aocstat-0.2.3/aocstat/config.py`

 * *Files identical despite different names*

### Comparing `aocstat-0.2.2/aocstat/format.py` & `aocstat-0.2.3/aocstat/format.py`

 * *Files identical despite different names*

### Comparing `aocstat-0.2.2/aocstat/main.py` & `aocstat-0.2.3/aocstat/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,16 @@
         )
     else:
         parser.add_argument(
             "-d",
             "--day",
             default=None,
             type=glob_lb_day_type,
-            help="A day number in the form ('[1..25]:[1,2]') where the number after the colon denotes which part to view.",
+            dest="global",
+            help="A day number in the form ('[1..25]:[1,2]') where the number after the colon denotes which part to view. Will default to the overall leaderboard if not provided.",
         )
 
     parser.add_argument(
         "-f",
         "--force",
         default=False,
         action="store_true",
@@ -124,26 +125,29 @@
         const=1,
         type=int,
         action="store",
         nargs="?",
         help="Print the leaderboard in multiple columns with the specified padding.",
     )
     args = vars(parser.parse_args(args))
+    if args["global"] is not None:
+        if int(args["global"].split(":")[0]) > api.get_most_recent_day(args["year"]):
+            parser.error("The day selected is in the future.")
     output = None
     if api.get_lb_ids():
         if args["global"] is False:
             _lb = api.get_priv_lb(
                 id=args["id"], yr=args["year"], force_update=args["force"]
             )
             output = fmt.format_priv_lb(*_lb, ansi_on=not args["no_colour"])
         else:
             _lb = api.get_glob_lb(yr=args["year"], day=args["global"])
             output = fmt.format_glob_lb(*_lb, ansi_on=not args["no_colour"])
     else:
-        _lb = api.get_glob_lb(yr=args["year"], day=args["day"])
+        _lb = api.get_glob_lb(yr=args["year"], day=args["global"])
         output = fmt.format_glob_lb(*_lb, ansi_on=not args["no_colour"])
     if args["columns"] is not None:
         output = fmt.columnize(output, args["columns"])
     print(output)
 
 
 def _purge(args=sys.argv[1:]):
```

### Comparing `aocstat-0.2.2/pyproject.toml` & `aocstat-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aocstat"
-version = "0.2.2"
+version = "0.2.3"
 description = "Command line tool for interacting with Advent of Code."
 authors = ["Hector Brown <hectorjbrown@protonmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 selenium = "^4.7.2"
```

### Comparing `aocstat-0.2.2/PKG-INFO` & `aocstat-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aocstat
-Version: 0.2.2
+Version: 0.2.3
 Summary: Command line tool for interacting with Advent of Code.
 Author: Hector Brown
 Author-email: hectorjbrown@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


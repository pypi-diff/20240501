# Comparing `tmp/dzira-0.2.tar.gz` & `tmp/dzira-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dzira-0.2.tar", last modified: Mon Feb  5 20:21:01 2024, max compression
+gzip compressed data, was "dzira-0.3.0.tar", last modified: Wed May  1 19:47:15 2024, max compression
```

## Comparing `dzira-0.2.tar` & `dzira-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,28 @@
-drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-02-05 20:21:01.341946 dzira-0.2/
--rw-r--r--   0 piotr     (1000) piotr     (1000)     1072 2023-05-08 16:48:33.000000 dzira-0.2/LICENSE
--rw-r--r--   0 piotr     (1000) piotr     (1000)     7535 2024-02-05 20:21:01.341946 dzira-0.2/PKG-INFO
--rw-r--r--   0 piotr     (1000) piotr     (1000)     6495 2024-02-05 20:04:39.000000 dzira-0.2/README.md
--rw-r--r--   0 piotr     (1000) piotr     (1000)     1101 2024-02-05 19:36:02.000000 dzira-0.2/pyproject.toml
--rw-r--r--   0 piotr     (1000) piotr     (1000)       38 2024-02-05 20:21:01.341946 dzira-0.2/setup.cfg
-drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-02-05 20:21:01.341946 dzira-0.2/src/
-drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-02-05 20:21:01.341946 dzira-0.2/src/dzira/
--rw-r--r--   0 piotr     (1000) piotr     (1000)        0 2023-12-03 20:45:36.000000 dzira-0.2/src/dzira/__init__.py
--rw-r--r--   0 piotr     (1000) piotr     (1000)    32161 2024-01-28 19:14:27.000000 dzira-0.2/src/dzira/dzira.py
-drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-02-05 20:21:01.341946 dzira-0.2/src/dzira.egg-info/
--rw-r--r--   0 piotr     (1000) piotr     (1000)     7535 2024-02-05 20:21:01.000000 dzira-0.2/src/dzira.egg-info/PKG-INFO
--rw-r--r--   0 piotr     (1000) piotr     (1000)      314 2024-02-05 20:21:01.000000 dzira-0.2/src/dzira.egg-info/SOURCES.txt
--rw-r--r--   0 piotr     (1000) piotr     (1000)        1 2024-02-05 20:21:01.000000 dzira-0.2/src/dzira.egg-info/dependency_links.txt
--rw-r--r--   0 piotr     (1000) piotr     (1000)       43 2024-02-05 20:21:01.000000 dzira-0.2/src/dzira.egg-info/entry_points.txt
--rw-r--r--   0 piotr     (1000) piotr     (1000)       39 2024-02-05 20:21:01.000000 dzira-0.2/src/dzira.egg-info/requires.txt
--rw-r--r--   0 piotr     (1000) piotr     (1000)        6 2024-02-05 20:21:01.000000 dzira-0.2/src/dzira.egg-info/top_level.txt
-drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-02-05 20:21:01.341946 dzira-0.2/tests/
--rw-r--r--   0 piotr     (1000) piotr     (1000)    64248 2024-01-28 19:14:27.000000 dzira-0.2/tests/test_dzira.py
--rw-r--r--   0 piotr     (1000) piotr     (1000)      934 2023-12-03 20:45:36.000000 dzira-0.2/tests/test_readme.py
+drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-01 19:47:15.611689 dzira-0.3.0/
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     1072 2023-05-08 16:48:33.000000 dzira-0.3.0/LICENSE
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     7574 2024-05-01 19:47:15.611689 dzira-0.3.0/PKG-INFO
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     6532 2024-05-01 19:20:29.000000 dzira-0.3.0/README.md
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     1110 2024-05-01 19:33:00.000000 dzira-0.3.0/pyproject.toml
+-rw-r--r--   0 piotr     (1000) piotr     (1000)       38 2024-05-01 19:47:15.611689 dzira-0.3.0/setup.cfg
+drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-01 19:47:15.608355 dzira-0.3.0/src/
+drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-01 19:47:15.608355 dzira-0.3.0/src/dzira/
+-rw-r--r--   0 piotr     (1000) piotr     (1000)        0 2024-02-11 20:24:51.000000 dzira-0.3.0/src/dzira/__init__.py
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     4204 2024-05-01 19:20:29.000000 dzira-0.3.0/src/dzira/api.py
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     1198 2024-05-01 19:20:29.000000 dzira-0.3.0/src/dzira/betterdict.py
+drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-01 19:47:15.611689 dzira-0.3.0/src/dzira/cli/
+-rw-r--r--   0 piotr     (1000) piotr     (1000)    25671 2024-05-01 19:20:29.000000 dzira-0.3.0/src/dzira/cli/commands.py
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     1538 2024-05-01 19:20:29.000000 dzira-0.3.0/src/dzira/cli/config.py
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     3544 2024-05-01 19:20:29.000000 dzira-0.3.0/src/dzira/cli/output.py
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     1072 2024-05-01 19:03:08.000000 dzira-0.3.0/src/dzira/data.py
+drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-01 19:47:15.611689 dzira-0.3.0/src/dzira.egg-info/
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     7574 2024-05-01 19:47:15.000000 dzira-0.3.0/src/dzira.egg-info/PKG-INFO
+-rw-r--r--   0 piotr     (1000) piotr     (1000)      470 2024-05-01 19:47:15.000000 dzira-0.3.0/src/dzira.egg-info/SOURCES.txt
+-rw-r--r--   0 piotr     (1000) piotr     (1000)        1 2024-05-01 19:47:15.000000 dzira-0.3.0/src/dzira.egg-info/dependency_links.txt
+-rw-r--r--   0 piotr     (1000) piotr     (1000)       50 2024-05-01 19:47:15.000000 dzira-0.3.0/src/dzira.egg-info/entry_points.txt
+-rw-r--r--   0 piotr     (1000) piotr     (1000)       39 2024-05-01 19:47:15.000000 dzira-0.3.0/src/dzira.egg-info/requires.txt
+-rw-r--r--   0 piotr     (1000) piotr     (1000)        6 2024-05-01 19:47:15.000000 dzira-0.3.0/src/dzira.egg-info/top_level.txt
+drwxr-xr-x   0 piotr     (1000) piotr     (1000)        0 2024-05-01 19:47:15.611689 dzira-0.3.0/tests/
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     9608 2024-05-01 19:20:29.000000 dzira-0.3.0/tests/test_api.py
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     2288 2024-05-01 19:20:29.000000 dzira-0.3.0/tests/test_betterdict.py
+-rw-r--r--   0 piotr     (1000) piotr     (1000)     1882 2024-02-17 22:14:30.000000 dzira-0.3.0/tests/test_data.py
+-rw-r--r--   0 piotr     (1000) piotr     (1000)      941 2024-05-01 19:20:29.000000 dzira-0.3.0/tests/test_readme.py
```

### Comparing `dzira-0.2/LICENSE` & `dzira-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dzira-0.2/PKG-INFO` & `dzira-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dzira
-Version: 0.2
+Version: 0.3.0
 Summary: A cli wrapper for jira API to track sprints and manage worklogs
 Author-email: Piotr Kaznowski <piotr@kazno.dev>
 Project-URL: Homepage, https://github.com/caseneuve/dzira
 Project-URL: Issues, https://github.com/caseneuve/dzira/issues
 Project-URL: Changelog, https://github.com/caseneuve/dzira/blob/master/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -137,15 +137,16 @@
           "spent": null,
           "estimated": 4h
         }
       ]
     }
 
 Options:
-  -s, --state [active|closed]  Sprint state used for filtering  [default:
+  -s, --state [active|closed|future]
+                               Sprint state used for filtering  [default:
                                active]
   -i, --sprint-id INTEGER      Sprint id to get unambiguous result, helpful
                                when multiple active sprints; has precedence
                                over --state
   -f, --format TEXT            Output format: supports TABULATE formats + CSV
                                and JSON  [default: simple_grid]
   -h, --help                   Show this message and exit.
```

### Comparing `dzira-0.2/README.md` & `dzira-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,16 @@
           "spent": null,
           "estimated": 4h
         }
       ]
     }
 
 Options:
-  -s, --state [active|closed]  Sprint state used for filtering  [default:
+  -s, --state [active|closed|future]
+                               Sprint state used for filtering  [default:
                                active]
   -i, --sprint-id INTEGER      Sprint id to get unambiguous result, helpful
                                when multiple active sprints; has precedence
                                over --state
   -f, --format TEXT            Output format: supports TABULATE formats + CSV
                                and JSON  [default: simple_grid]
   -h, --help                   Show this message and exit.
```

### Comparing `dzira-0.2/pyproject.toml` & `dzira-0.3.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dzira"
-version = "0.2"
+version = "0.3.0"
 dependencies = [
     "click >= 8.1",
     "jira",
     "python-dotenv",
     "tabulate",
 ]
 authors = [
@@ -27,13 +27,13 @@
     "Programming Language :: Python :: 3.8",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Topic :: Software Development",
 ]
 
 [project.scripts]
-dzira = "dzira.dzira:main"
+dzira = "dzira.cli.commands:main"
 
 [project.urls]
 Homepage = "https://github.com/caseneuve/dzira"
 Issues = "https://github.com/caseneuve/dzira/issues"
 Changelog = "https://github.com/caseneuve/dzira/blob/master/CHANGELOG.md"
```

### Comparing `dzira-0.2/src/dzira/dzira.py` & `dzira-0.3.0/src/dzira/cli/commands.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,335 +1,158 @@
 from __future__ import annotations
 
-import concurrent.futures
 import csv
 import json
-import os
 import re
 import subprocess
 import sys
-import time
-from dataclasses import dataclass, field
 from datetime import date, datetime, timedelta
-from functools import wraps
-from itertools import cycle
-from pathlib import Path
-from typing import Any, Iterable
 
 import click
-from dotenv import dotenv_values
 from jira import JIRA
-from jira.exceptions import JIRAError
-from jira.resources import Board, Sprint, User, Worklog
-from tabulate import tabulate, tabulate_formats
+from jira.resources import Board, Sprint, Worklog
+from tabulate import tabulate
 
+from dzira import api
+from dzira.betterdict import D
+from dzira.cli.output import (
+    Colors,
+    Result,
+    Spinner,
+    hide_cursor,
+    show_cursor,
+)
+from .config import (
+    DEFAULT_OUTPUT_FORMAT,
+    VALID_OUTPUT_FORMATS,
+    get_config,
+)
 
-CONFIG_DIR_NAME = "dzira"
-DOTFILE = f".{CONFIG_DIR_NAME}"
-REQUIRED_KEYS = "JIRA_SERVER", "JIRA_EMAIL", "JIRA_TOKEN", "JIRA_PROJECT_KEY"
-
-VALID_OUTPUT_FORMATS = sorted(tabulate_formats + ["json", "csv"])
-DEFAULT_OUTPUT_FORMAT = "simple_grid"
-
-use_spinner = True
-use_color = True
-
-
-def c(*args):
-    C = {k: f"\033[{v}m" for k, v in (("^reset", 0),
-                                      ("^bold", 1),
-                                      ("^red", 91),
-                                      ("^green", 92),
-                                      ("^yellow", 93),
-                                      ("^blue", 94),
-                                      ("^magenta", 95),
-                                      ("^cyan", 96))}
-    if use_color:
-        return "".join([C.get(a, a) for a in args]) + C["^reset"]
-    return "".join([a for a in args if a not in C])
-
-
-def hide_cursor():
-    print("\033[?25l", end="", flush=True, file=sys.stderr)
-
-
-def show_cursor():
-    print("\033[?25h", end="", flush=True, file=sys.stderr)
-
-
-class D(dict):
-    def __call__(self, *keys) -> Iterable:
-        if keys:
-            return [self.get(*k) if isinstance(k, tuple) else self.get(k) for k in keys]
-        else:
-            return self.values()
-
-    def __getattr__(self, key):
-        try:
-            return self[key]
-        except KeyError:
-            raise AttributeError(f"'D' object has no attribute {key!r}")
-
-    def _update(self, k, v):
-        self[k] = v(self.get(k)) if callable(v) else v
-
-    def update(self, *args, **kwargs):
-        if len(args) % 2 != 0:
-            raise Exception(
-                f"Provide even number of key-value args, need a value for key: {args[-1]!r}"
-            )
-        for i in range(0, len(args), 2):
-            self._update(args[i], args[i + 1])
-        for k, v in kwargs.items():
-            self._update(k, v)
-        return self
-
-    def has(self, k):
-        return self.get(k) is not None
-
-    def without(self, *args):
-        return D({k: v for k, v in self.items() if k not in args})
-
-    def __repr__(self):
-        return f"betterdict({dict(self)})"
-
-
-@dataclass
-class Result:
-    result: Any = None
-    stdout: str = ""
-    data: D = field(default_factory=D)
-
-
-def spin_it(msg="", done="✓", fail="✗"):
-    spinner = cycle("⠋⠙⠹⠸⠼⠴⠦⠧⠇⠏")
-    separator = "  "
-    connector = ":\t"
-
-    def decorator(func):
-        func.is_decorated_with_spin_it = True
-
-        @wraps(func)
-        def wrapper(*args, **kwargs):
-            if not use_spinner:
-                return func(*args, **kwargs)
-            try:
-                with concurrent.futures.ThreadPoolExecutor() as executor:
-                    future = executor.submit(func, *args, **kwargs)
-
-                    while future.running():
-                        print(
-                            c("\r", "^magenta", next(spinner), separator, msg),
-                            end="",
-                            flush=True,
-                            file=sys.stderr
-                        )
-                        time.sleep(0.1)
-
-                    r: Result = future.result()
-                    print(
-                        c("\r", "^green", done, separator, msg, "^reset", connector, r.stdout),
-                        flush=True,
-                        file=sys.stderr
-                    )
-                    return r
-            except Exception as exc:
-                if type(exc) == JIRAError:
-                    error_msg = exc.response.json()["errors"]
-                else:
-                    error_msg = exc
-                print(
-                    c("\r", "^red", fail, separator, msg),
-                    end=":\n",
-                    flush=True,
-                    file=sys.stderr
-                )
-                raise Exception(error_msg)
-        return wrapper
-    return decorator
-
-
-def get_config_from_file(config_file: str | Path | None = None) -> dict:
-    if config_file is None:
-        config_file_dir = os.environ.get("XDG_CONFIG_HOME", os.environ["HOME"])
-        for path in (
-                os.path.join(config_file_dir, CONFIG_DIR_NAME, "env"),
-                os.path.join(config_file_dir, DOTFILE),
-                os.path.join(os.environ["HOME"], ".config", CONFIG_DIR_NAME, "env"),
-                os.path.join(os.environ["HOME"], ".config", DOTFILE),
-        ):
-            if os.path.isfile(path):
-                config_file = path
-                break
-
-    return dotenv_values(config_file)
-
-
-def get_config(config: dict = {}) -> dict:
-    for cfg_fn in (
-        lambda: get_config_from_file(config.get("file")),
-        lambda: (_ for _ in ()).throw(
-            Exception(
-                "could not find required config values: "
-                f"{', '.join(sorted(set(REQUIRED_KEYS).difference(set(config))))}"
-            )
-        ),
-    ):
-        if set(REQUIRED_KEYS).issubset(config.keys()):
-            break
-        config = {**cfg_fn(), **config}
 
-    return config
+colors = Colors()
+c = colors.c
+spinner = Spinner(c)
 
 
 ##################################################
 #  JIRA wrapper
 ##################################################
 
 
-@spin_it("Getting client")
-def get_jira(config: dict) -> Result:
-    jira = JIRA(
-        server=f"https://{config['JIRA_SERVER']}",
-        basic_auth=(config["JIRA_EMAIL"], config["JIRA_TOKEN"]),
-    )
-    msg = f"connecting to {config['JIRA_SERVER']}"
+@spinner.run("Getting client")
+def get_jira(config: D) -> Result:
+    server, email, token = config("JIRA_SERVER", "JIRA_EMAIL", "JIRA_TOKEN")
+    msg = f"connecting to {server}"
+    jira: JIRA = api.connect_to_jira(server, email, token)
     return Result(stdout=msg, result=jira)
 
 
-@spin_it("Getting board")
+@spinner.run("Getting board")
 def get_board(jira: JIRA, key: str) -> Result:
-    try:
-        boards = jira.boards(projectKeyOrID=key)
-    except JIRAError as exc_info:
-        raise Exception(str(exc_info))
-    if len(boards) > 1:
-        raise Exception(
-            f"Found more than one board matching {key!r}:\n"
-            f"{', '.join(b.raw['location']['displayName'] for b in boards)}"
-        )
+    board: Board = api.get_board_by_key(jira, key)
     return Result(
-        result=boards[0],
-        stdout=f'{boards[0].raw["location"]["displayName"]}'
+        result=board,
+        stdout=f'{board.raw["location"]["displayName"]}'
     )
 
 
-def _get_sprints(jira: JIRA, board: Board, state: str) -> list:
-    if sprints := jira.sprints(board_id=board.id, state=state):
-        return sprints
-    raise Exception(f"could not find any sprints for board {board.name!r}")
-
-
-def _get_first_sprint_matching_state(jira: JIRA, board: Board, state: str = "active", **_) -> Sprint:
-    sprints = _get_sprints(jira, board, state)
-    if len(sprints) > 1:
-        info = "\n".join([f"\t - {s.name}, id: {s.id}" for s in sprints])
-        raise Exception(
-            f"Found more than one {state} sprint:\n{info}\n"
-            "Use sprint id to get unambiguous result"
-        )
-    return sprints[0]
-
-
-def _get_sprint_from_id(jira: JIRA, sprint_id: int, **_) -> Sprint:
-    try:
-        return jira.sprint(sprint_id)
-    except JIRAError as exc:
-        raise Exception(str(exc))
+# TODO: -> move to data
+def process_sprint_out(sprint: Sprint | D) -> str:
+    fmt = lambda d: datetime.strptime(d, "%Y-%m-%dT%H:%M:%S.%fZ").strftime("%a, %b %d")
+    return f"{sprint.name} • id: {sprint.id} • {fmt(sprint.startDate)} -> {fmt(sprint.endDate)}"
 
 
-@spin_it("Getting sprint")
+@spinner.run("Getting sprint")
 def get_sprint(jira: JIRA, payload: D) -> Result:
-    fn = _get_sprint_from_id if payload.has("sprint_id") else _get_first_sprint_matching_state
-    sprint = fn(jira, **payload)
+    sprint_id, board, state = payload("sprint_id", "board", "state")
+    try:
+        warning = ""
+        if sprint_id:
+            sprint = api.get_sprint_by_id(jira, sprint_id)
+        else:
+            sprints = api.get_sprints_by_board(jira, board, state)
+            if len(sprints) > 1:
+                warning = f" (showing most recent sprint matching {state!r})"
+            sprint = sprints[-1]
+    except:
+        raise Exception("Could not find sprint matching given criteria")
     out = process_sprint_out(sprint)
-    return Result(result=sprint, stdout=out)
-
-
-def _get_sprint_issues(jira: JIRA, sprint: Sprint) -> list:
-    if issues := jira.search_issues(jql_str=f"Sprint = {sprint.name!r}"):
-        return list(issues)
-    raise Exception(f"could not find any issues for sprint {sprint.name!r}")
-
+    return Result(result=sprint, stdout=f"{out}{warning}")
 
-@spin_it("Getting issues")
-def get_issues(jira: JIRA, sprint: Sprint) -> Result:
-    issues: list = _get_sprint_issues(jira, sprint)
-    return Result(result=issues)
 
-
-# TODO: catch errors and properly process them in Result (stderr?) // update tests for new param
-@spin_it("Adding worklog")
+@spinner.run("Adding worklog")
 def add_worklog(
         jira: JIRA,
         issue: str,
+        seconds: int,
         comment: str | None = None,
-        seconds: int | None = None,
         date: datetime | None = None,
         **_
 ) -> Result:
-    work_log = jira.add_worklog(
-        issue=issue, timeSpentSeconds=seconds, comment=comment, started=date
-    )
+    work_log: Worklog = api.log_work(jira, issue, seconds, comment, date)
     return Result(
         stdout=(
             f"spent {work_log.raw['timeSpent']} in {issue} "
             f"[worklog {work_log.id}] at {datetime.now():%H:%M:%S}"
         )
     )
 
 
-def get_worklog(jira: JIRA, issue: str, worklog_id: str | int, **_) -> Worklog:
-    if work_log := jira.worklog(issue=issue, id=str(worklog_id)):
-        return work_log
-    raise Exception(f"could not find worklog {worklog_id} for issue {issue!r}")
+@spinner.run("Getting worklog")
+def get_worklog(jira: JIRA, issue: str, worklog_id: str | int, **_) -> Result:
+    work_log: Worklog = api.get_worklog(jira, issue=issue, worklog_id=str(worklog_id))
+    created = datetime.strptime(
+        work_log.created, "%Y-%m-%dT%H:%M:%S.%f%z"
+    ).astimezone().strftime("%a, %b %d, %H:%M:%S")
+    author = work_log.author.displayName
+    return Result(result=work_log, stdout=f"{work_log.id}, created by {author} on {created}")
 
 
 def _update_worklog(
         worklog: Worklog, time: str | None, comment: str | None, date: datetime | None
-) -> None:
+) -> D:
     if not (time or comment):
         raise Exception(
             "at least one of <time> or <comment> fields needed to perform the update!"
         )
     fields = {
         k: v
-        for k, v in zip(["timeSpent", "comment", "started"], [time, comment, date])
+        for k, v in zip(["timeSpentSeconds", "comment", "started"], [time, comment, date])
         if v
     }
     worklog.update(fields=fields)
+    return D(fields)
 
 
 # TODO: we can't update worklog to change the issue
 # * add delete option to worklog !!!
-# * catch error when someone tries to update worklog in wrong ticket! => test it
-@spin_it("Updating worklog")
+@spinner.run("Updating worklog")
 def update_worklog(
         worklog: Worklog, time: str, comment: str, date: datetime | None = None, **_
 ) -> Result:
-    try:
-       _update_worklog(worklog, time, comment, date)
-    except JIRAError as exc:
-        raise Exception(str(exc))
-    return Result(stdout=f"{worklog.id} updated!")
+    info = _update_worklog(worklog, time, comment, date)
+    for k in info.copy():
+        if k == "timeSpentSeconds":
+            info.pop(k)
+            k = "timeSpent"
+        info.update(k, worklog.raw[k])
+    return Result(stdout=f"updated: {info}")
 
 
-def set_spinner_use(with_spinner: bool):
-    global use_spinner;
-    use_spinner = with_spinner and sys.stdin.isatty()
+##################################################
+#  CLI wrapper
+##################################################
 
 
-def set_color_use(with_color: bool):
-    global use_color
-    use_color = with_color and sys.stdin.isatty()
+def set_spinner_use(with_spinner: bool):
+    spinner.use = with_spinner and sys.stdin.isatty()
 
 
-##################################################
-#  CLI wrapper
-##################################################
+def set_color_use(with_color: bool):
+    colors.use = with_color and sys.stdin.isatty()
 
 
 @click.group()
 @click.option("-f", "--file", help=f"Config file path", type=click.Path())
 @click.option("-k", "--key", help="JIRA_PROJECT_KEY value", envvar="JIRA_PROJECT_KEY")
 @click.option("-t", "--token", help="JIRA_TOKEN value", envvar="JIRA_TOKEN")
 @click.option("-m", "--email", help="JIRA_EMAIL value", envvar="JIRA_EMAIL")
@@ -377,34 +200,40 @@
     ctx.obj.update(cfg)
 
 
 ##################################################
 #  LS command
 ##################################################
 
-
-def process_sprint_out(sprint: Sprint) -> str:
-    fmt = lambda d: datetime.strptime(d, "%Y-%m-%dT%H:%M:%S.%fZ").strftime("%a, %b %d")
-    return f"{sprint.name} • id: {sprint.id} • {fmt(sprint.startDate)} -> {fmt(sprint.endDate)}"
+# TODO:
+# add --sprints/--issues
+# return {sprints: [], issues: []} and process accordingly
+# jira.sprints(board_id) -> need board OR jira.sprint(id) or sprint_info(sprint_id=id)
 
 
-# TODO:
-# - we probably should check board always, as sprint_id may not be matching the team's board...
-# - catch errors
-def get_sprint_and_issues(jira: JIRA, payload: D) -> D:
-    if not payload.has("sprint_id"):
-        payload.update("board", get_board(jira, payload["JIRA_PROJECT_KEY"]).result)
-    sprint = get_sprint(jira, payload).result
-    issues = get_issues(jira, sprint).result
-    return D(sprint=sprint, issues=issues)
+@spinner.run("Getting issues")
+def get_issues(jira: JIRA, payload: D) -> Result:
+    project_key, sprint_id, state = payload("JIRA_PROJECT_KEY", "sprint_id", ("state", "active"))
+    issues: list = api.search_issues_with_sprint_info(
+        jira, project_key=project_key, sprint_id=sprint_id, state=state
+    )
+    if issues:
+        # TODO: should use func from dzira.data
+        sprint_info = D(issues[0].raw["fields"]["Sprint"][0])
+        out = process_sprint_out(sprint_info)
+    else:
+        out = "No issues found"
+        sprint_info = {}
+    return Result(result=D(sprint=sprint_info, issues=issues), stdout=out)
 
 
+# TODO: move data processing to data
 def show_issues(sprint_and_issues: D, format: str) -> None:
     if format in ("json", "csv"):
-        global use_color; use_color = False
+        colors.use = False
 
     fmt = lambda t: str(timedelta(seconds=t)) if t else None
     state_clr = {"To Do": "^magenta", "In Progress": "^yellow", "Done": "^green"}
     clr = lambda s: c(state_clr.get(s, "^reset"), "^bold", s)
 
     def _estimate(i):
         try:
@@ -463,15 +292,15 @@
     raise click.BadParameter(f"format should be one of: {', '.join(VALID_OUTPUT_FORMATS)}")
 
 
 @cli.command()
 @click.pass_context
 @click.option(
     "-s", "--state",
-    type=click.Choice(["active", "closed"]), default="active", show_default=True,
+    type=click.Choice(["active", "closed", "future"]), default="active", show_default=True,
     help="Sprint state used for filtering",
 )
 @click.option(
     "-i", "--sprint-id",
     type=int,
     help=(
         "Sprint id to get unambiguous result, helpful when multiple active sprints; "
@@ -519,20 +348,18 @@
             "state": "To Do",
             "spent": null,
             "estimated": 4h
           }
         ]
       }
     """
-    config = get_config(config=ctx.obj)
-    jira = get_jira(config).result
-    sprint_and_issues: D = get_sprint_and_issues(
-        jira, D(state=state, sprint_id=sprint_id, **config)
-    )
-    show_issues(sprint_and_issues, format=format)
+    config: D = get_config(config=ctx.obj)
+    jira: JIRA = get_jira(config).result
+    issues: D = get_issues(jira, D(state=state, sprint_id=sprint_id, **config)).result
+    show_issues(issues, format=format)
 
 
 ##################################################
 #  LOG command
 ##################################################
 
 ### Validators
@@ -650,39 +477,39 @@
     )
     t1 = unify(start)
 
     if t2 < t1:
         raise click.BadParameter("start time cannot be later than end time")
     else:
         delta_seconds = (t2 - t1).total_seconds()
-        return payload.update("seconds", str(int(delta_seconds)))
+        return payload.update("seconds", int(delta_seconds))
 
 
 def establish_issue(jira: JIRA, payload: D) -> D:
     key = payload["JIRA_PROJECT_KEY"]
     issue = payload.get("issue", "")
 
     if issue.isdigit():
         return payload.update("issue", f"{key}-{issue}")
 
-    sprint_issues = get_sprint_and_issues(jira, payload)
-    candidates = [i for i in sprint_issues if issue.lower() in i.fields.summary.lower()]
+    sprint_issues = get_issues(jira, payload).result
+    candidates = [i for i in sprint_issues.issues if issue.lower() in i.fields.summary.lower()]
 
     if not candidates:
         raise Exception("could not find any matching issues")
     if len(candidates) > 1:
         msg = "\n".join(f" * {i.key}: {i.fields.summary}" for i in candidates)
         raise Exception("found more than one matching issue:\n" + msg)
 
     return payload.update("issue", candidates[0].key)
 
 
 def perform_log_action(jira: JIRA, payload: D) -> None:
     if payload["worklog_id"] is not None:
-        worklog = get_worklog(jira, **payload)
+        worklog: Worklog = get_worklog(jira, **payload).result
         update_worklog(worklog, **payload)
     else:
         add_worklog(jira, **payload)
 
 
 @cli.command()
 @click.pass_context
@@ -762,74 +589,46 @@
 
 
 ##################################################
 #  REPORT command
 ##################################################
 
 
-@spin_it("Getting user")
-def get_user(jira: JIRA, config: dict) -> Result:
-    try:
-        users = jira.search_users(query=config["JIRA_EMAIL"])
-    except Exception as exc:
-        raise Exception(str(exc))
-    if len(users) > 1:
-        raise Exception(f"Found more than one user\n{', '.join(u.displayName for u in users)}")
-    if users == []:
-        raise Exception("Could not find users matching given email address")
+@spinner.run("Getting user id")
+def get_user_id(jira: JIRA) -> Result:
+    return Result(result=api.get_current_user_id(jira))
 
-    return Result(result=users[0], stdout=users[0].displayName)
 
-
-@spin_it("Getting issues")
+@spinner.run("Getting issues")
 def get_issues_with_work_logged_on_date(jira: JIRA, report_date: datetime | None) -> Result:
-    if report_date is not None:
-        query = f"worklogDate = {report_date:%Y-%m-%d}"
-    else:
-        query = f"worklogDate >= startOfDay()"
+    issues = api.get_issues_by_work_logged_on_date(jira, report_date)
+    if report_date is None:
         report_date = datetime.combine(date.today(), datetime.min.time())
-    try:
-        issues = jira.search_issues(query)
-    except JIRAError as exc:
-        raise Exception(str(exc))
-
     return Result(
         result=issues,
         data=D(report_date=report_date),
         stdout=(
             f"Found {len(issues)} issue{'s' if len(issues) != 1 else ''} "
             f"with work logged on {report_date:%a, %b %d}"
         )
     )
 
 
-@spin_it("Getting worklogs")
-def get_user_worklogs_from_date(jira: JIRA, user: User, issues: Result) -> Result:
+@spinner.run("Getting worklogs")
+def get_user_worklogs_from_date(jira: JIRA, user_email: str, issues: Result) -> Result:
     worklogs = D(counter=0)
-
     for issue in issues.result:
-        try:
-            issue_worklogs = jira.worklogs(issue.id)
-            matching = [
-                w for w in issue_worklogs
-                if (
-                        (w.author.accountId == user.accountId)
-                        and (
-                            issues.data.report_date
-                            <= datetime.strptime(w.started.split(".")[0], "%Y-%m-%dT%H:%M:%S")
-                            < (issues.data.report_date + timedelta(days=1))
-                        )
-                )
-            ]
-            if matching:
-                key = issue.raw["key"]
-                summary = issue.raw["fields"]["summary"]
-                worklogs.update((key, summary), matching, counter=lambda x: x + (len(matching)))
-        except Exception as exc:
-            raise Exception(str(exc))
+        report_date = issues.data.report_date
+        assert type(report_date) == datetime, f"Got unexpected report_date type {type(report_date)}"
+        matching: list = api.get_issue_worklogs_by_user_and_date(
+            jira, issue, user_email, report_date
+        )
+        if matching:
+            worklogs[issue.id] = D(key=issue.key, summary=issue.fields.summary, worklogs=matching)
+            worklogs.update(counter=lambda x: x + (len(matching)))
 
     return Result(
         result=worklogs.without("counter"),
         stdout=(
             f"Found {worklogs.counter} worklog{'s' if worklogs.counter != 1 else ''} "
             "matching author and date"
         )
@@ -838,24 +637,25 @@
 
 def _seconds_to_hour_minute_fmt(seconds):
     hours, remainder = divmod(seconds, 3600)
     minutes, _ = divmod(remainder, 60)
     return f"{hours}h {minutes:02}m"
 
 
-def show_report(worklogs: D, format: str | None) -> None:
+# -> `data`, so it's processing data, and show_func only shows
+def show_report(issues_to_worklogs: D, format: str | None) -> None:
     total_time = 0
     csv_rows = []
     json_dict = {"issues": [], "total_time": None, "total_seconds": None}
     tables = []
-    for issue in worklogs:
-        key, summary = issue
+    for issue_id in issues_to_worklogs:
+        key, summary, worklogs = issues_to_worklogs[issue_id]("key", "summary", "worklogs")
         issue_total_time = 0
         issue_worklogs = []
-        for w in worklogs[issue]:
+        for w in worklogs:
             started, time_spent, comment, time_spent_seconds = D(w.raw)(
                 "started", "timeSpent", "comment", "timeSpentSeconds"
             )
             total_time += time_spent_seconds
             issue_total_time += time_spent_seconds
             local_timestamp = datetime.strptime(started, '%Y-%m-%dT%H:%M:%S.%f%z').astimezone()
             formatted_time = local_timestamp.strftime('%H:%M:%S')
@@ -958,20 +758,20 @@
         ],
         "total_time": "1h 15m",
         "total_seconds": 4500
       }
     """
     config = get_config(config=ctx.obj)
     jira = get_jira(config).result
-    user = get_user(jira, config).result
     issues = get_issues_with_work_logged_on_date(jira, report_date)
     if issues.result:
-        worklogs = get_user_worklogs_from_date(jira, user, issues).result
+        worklogs = get_user_worklogs_from_date(jira, config["JIRA_EMAIL"], issues).result
     else:
         worklogs = D()
+
     show_report(worklogs, format=format)
 
 
 @cli.command(hidden=True)
 @click.pass_context
 def shell(ctx):
     config = get_config(config=ctx.obj)
@@ -988,14 +788,7 @@
         cli()
     except Exception as e:
         print(e, file=sys.stderr)
         sys.exit(1)
     finally:
         if sys.stdin.isatty():
             show_cursor()
-
-
-if __name__ == "__main__":
-    main()
-
-
-# -*- python-indent-offset: 4 -*-
```

### Comparing `dzira-0.2/src/dzira.egg-info/PKG-INFO` & `dzira-0.3.0/src/dzira.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dzira
-Version: 0.2
+Version: 0.3.0
 Summary: A cli wrapper for jira API to track sprints and manage worklogs
 Author-email: Piotr Kaznowski <piotr@kazno.dev>
 Project-URL: Homepage, https://github.com/caseneuve/dzira
 Project-URL: Issues, https://github.com/caseneuve/dzira/issues
 Project-URL: Changelog, https://github.com/caseneuve/dzira/blob/master/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -137,15 +137,16 @@
           "spent": null,
           "estimated": 4h
         }
       ]
     }
 
 Options:
-  -s, --state [active|closed]  Sprint state used for filtering  [default:
+  -s, --state [active|closed|future]
+                               Sprint state used for filtering  [default:
                                active]
   -i, --sprint-id INTEGER      Sprint id to get unambiguous result, helpful
                                when multiple active sprints; has precedence
                                over --state
   -f, --format TEXT            Output format: supports TABULATE formats + CSV
                                and JSON  [default: simple_grid]
   -h, --help                   Show this message and exit.
```

### Comparing `dzira-0.2/tests/test_readme.py` & `dzira-0.3.0/tests/test_readme.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 
 from click.testing import CliRunner
 
-from src.dzira.dzira import cli
+from src.dzira.cli.commands import cli
 
 
 runner = CliRunner()
 readme = Path("README.md").read_text()
 
 
 def assert_help_in_readme(help):
```


# Comparing `tmp/libop-30.tar.gz` & `tmp/libop-5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libop-30.tar", last modified: Wed May  1 15:08:12 2024, max compression
+gzip compressed data, was "libop-5.tar", last modified: Sun Dec 31 20:26:04 2023, max compression
```

## Comparing `libop-30.tar` & `libop-5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-01 15:08:12.761974 libop-30/
--rw-r--r--   0 bart      (1000) bart      (1001)     4047 2024-05-01 15:08:12.761974 libop-30/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)     3513 2024-05-01 12:50:10.000000 libop-30/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-01 15:08:12.757974 libop-30/bin/
--rwxr-xr-x   0 bart      (1000) bart      (1001)     3743 2024-05-01 13:46:25.000000 libop-30/bin/op
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-01 15:08:12.757974 libop-30/libop.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1001)     4047 2024-05-01 15:08:12.000000 libop-30/libop.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)      659 2024-05-01 15:08:12.000000 libop-30/libop.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        1 2024-05-01 15:08:12.000000 libop-30/libop.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        3 2024-05-01 15:08:12.000000 libop-30/libop.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        1 2024-05-01 15:08:12.000000 libop-30/libop.egg-info/zip-safe
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-01 15:08:12.757974 libop-30/op/
--rw-r--r--   0 bart      (1000) bart      (1001)       60 2024-05-01 03:45:44.000000 libop-30/op/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)      704 2024-05-01 03:45:44.000000 libop-30/op/broker.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4002 2024-05-01 03:45:44.000000 libop-30/op/client.py
--rw-r--r--   0 bart      (1000) bart      (1001)      581 2024-05-01 03:45:44.000000 libop-30/op/command.py
--rw-r--r--   0 bart      (1000) bart      (1001)      285 2024-05-01 03:45:44.000000 libop-30/op/default.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1397 2024-05-01 03:45:44.000000 libop-30/op/errors.py
--rw-r--r--   0 bart      (1000) bart      (1001)      813 2024-05-01 03:45:44.000000 libop-30/op/event.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2008 2024-05-01 03:45:44.000000 libop-30/op/find.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1430 2024-05-01 03:45:44.000000 libop-30/op/handler.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-01 15:08:12.761974 libop-30/op/mod/
--rw-r--r--   0 bart      (1000) bart      (1001)      507 2024-05-01 13:32:46.000000 libop-30/op/mod/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)      216 2024-05-01 03:45:44.000000 libop-30/op/mod/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1001)      344 2024-05-01 03:45:44.000000 libop-30/op/mod/err.py
--rw-r--r--   0 bart      (1000) bart      (1001)      372 2024-05-01 13:07:43.000000 libop-30/op/mod/flt.py
--rw-r--r--   0 bart      (1000) bart      (1001)      764 2024-05-01 03:45:44.000000 libop-30/op/mod/fnd.py
--rw-r--r--   0 bart      (1000) bart      (1001)    18837 2024-05-01 13:07:56.000000 libop-30/op/mod/irc.py
--rw-r--r--   0 bart      (1000) bart      (1001)      706 2024-05-01 03:45:44.000000 libop-30/op/mod/log.py
--rw-r--r--   0 bart      (1000) bart      (1001)     3577 2024-05-01 03:45:44.000000 libop-30/op/mod/mbx.py
--rw-r--r--   0 bart      (1000) bart      (1001)    17389 2024-05-01 13:51:00.000000 libop-30/op/mod/mdl.py
--rw-r--r--   0 bart      (1000) bart      (1001)      259 2024-05-01 03:45:44.000000 libop-30/op/mod/mod.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2354 2024-05-01 03:45:44.000000 libop-30/op/mod/req.py
--rw-r--r--   0 bart      (1000) bart      (1001)    10834 2024-05-01 13:08:49.000000 libop-30/op/mod/rss.py
--rw-r--r--   0 bart      (1000) bart      (1001)     3169 2024-05-01 03:45:44.000000 libop-30/op/mod/rst.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1159 2024-05-01 03:45:44.000000 libop-30/op/mod/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1001)      988 2024-05-01 03:45:44.000000 libop-30/op/mod/thr.py
--rw-r--r--   0 bart      (1000) bart      (1001)     5200 2024-05-01 13:08:59.000000 libop-30/op/mod/tmr.py
--rw-r--r--   0 bart      (1000) bart      (1001)     3062 2024-05-01 13:09:08.000000 libop-30/op/mod/udp.py
--rw-r--r--   0 bart      (1000) bart      (1001)     5729 2024-05-01 03:45:44.000000 libop-30/op/mod/wsd.py
--rw-r--r--   0 bart      (1000) bart      (1001)     6109 2024-05-01 03:45:44.000000 libop-30/op/object.py
--rw-r--r--   0 bart      (1000) bart      (1001)      278 2024-05-01 03:45:44.000000 libop-30/op/repeater.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-01 15:08:12.761974 libop-30/op/run/
--rw-r--r--   0 bart      (1000) bart      (1001)     1572 2024-05-01 13:37:09.000000 libop-30/op/run/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2056 2024-05-01 13:32:04.000000 libop-30/op/thread.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1085 2024-05-01 03:45:44.000000 libop-30/op/timer.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1120 2024-05-01 03:45:44.000000 libop-30/op/whitelist.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1266 2024-05-01 03:45:44.000000 libop-30/op/workdir.py
--rw-r--r--   0 bart      (1000) bart      (1001)      838 2024-05-01 14:42:57.000000 libop-30/pyproject.toml
--rw-r--r--   0 bart      (1000) bart      (1001)       38 2024-05-01 15:08:12.761974 libop-30/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1001)      164 2024-05-01 15:00:55.000000 libop-30/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-12-31 20:26:04.121652 libop-5/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1219 2023-12-31 20:26:04.121652 libop-5/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      684 2023-12-31 20:25:48.000000 libop-5/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-12-31 20:26:04.117653 libop-5/libop.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1219 2023-12-31 20:26:04.000000 libop-5/libop.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      719 2023-12-31 20:26:04.000000 libop-5/libop.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-12-31 20:26:04.000000 libop-5/libop.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        3 2023-12-31 20:26:04.000000 libop-5/libop.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-12-31 20:26:04.000000 libop-5/libop.egg-info/zip-safe
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-12-31 20:26:04.117653 libop-5/op/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1159 2023-12-31 14:57:27.000000 libop-5/op/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      131 2023-12-31 14:57:27.000000 libop-5/op/__main__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      796 2023-12-31 19:31:40.000000 libop-5/op/brokers.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      597 2023-12-31 19:31:09.000000 libop-5/op/clients.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      557 2023-12-31 14:57:27.000000 libop-5/op/collect.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      741 2023-12-31 19:31:36.000000 libop-5/op/command.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      413 2023-12-31 14:57:27.000000 libop-5/op/default.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1551 2023-12-31 19:31:28.000000 libop-5/op/excepts.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1230 2023-12-31 20:17:14.000000 libop-5/op/handler.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2089 2023-12-31 14:57:27.000000 libop-5/op/locates.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      969 2023-12-31 19:31:46.000000 libop-5/op/message.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-12-31 20:26:04.121652 libop-5/op/mods/
+-rw-r--r--   0 bart      (1000) bart      (1000)      553 2023-12-31 20:17:54.000000 libop-5/op/mods/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      200 2023-12-31 14:57:34.000000 libop-5/op/mods/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      134 2023-12-31 14:57:34.000000 libop-5/op/mods/dbg.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      473 2023-12-31 14:57:34.000000 libop-5/op/mods/err.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      718 2023-12-31 14:57:34.000000 libop-5/op/mods/fnd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    16008 2023-12-31 15:00:03.000000 libop-5/op/mods/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      629 2023-12-31 14:57:34.000000 libop-5/op/mods/log.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3496 2023-12-31 14:57:34.000000 libop-5/op/mods/mbx.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    16920 2023-12-31 14:57:34.000000 libop-5/op/mods/mdl.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      189 2023-12-31 14:57:34.000000 libop-5/op/mods/mod.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      624 2023-12-31 14:57:34.000000 libop-5/op/mods/mre.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      390 2023-12-31 14:57:34.000000 libop-5/op/mods/pwd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2349 2023-12-31 14:57:34.000000 libop-5/op/mods/req.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     6982 2023-12-31 14:57:34.000000 libop-5/op/mods/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2638 2023-12-31 14:57:34.000000 libop-5/op/mods/rst.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1025 2023-12-31 14:57:34.000000 libop-5/op/mods/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      984 2023-12-31 14:57:34.000000 libop-5/op/mods/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1920 2023-12-31 14:57:34.000000 libop-5/op/mods/tmr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2817 2023-12-31 14:57:34.000000 libop-5/op/mods/udp.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5766 2023-12-31 14:57:34.000000 libop-5/op/mods/wsd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5608 2023-12-31 15:00:22.000000 libop-5/op/objects.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     6125 2023-12-31 14:57:27.000000 libop-5/op/parsers.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     4958 2023-12-31 20:22:00.000000 libop-5/op/runtime.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2709 2023-12-31 14:57:27.000000 libop-5/op/storage.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2437 2023-12-31 19:31:59.000000 libop-5/op/threads.py
+-rw-r--r--   0 bart      (1000) bart      (1000)       62 2023-12-31 14:57:27.000000 libop-5/op/utility.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      899 2023-12-31 20:21:50.000000 libop-5/pyproject.toml
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2023-12-31 20:26:04.121652 libop-5/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)      148 2023-12-31 14:56:01.000000 libop-5/setup.py
```

### Comparing `libop-30/bin/op` & `libop-5/op/runtime.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,84 +1,97 @@
-#!/usr/bin/env python3
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C,R,W0201,W0212,W0105,W0613,W0406,E0102,W0611,W0718,W0125,E0401
 
 
-"main"
+"runtime"
 
 
 import getpass
+import inspect
 import os
 import pwd
-import readline
 import sys
 import termios
 import time
+import _thread
 
 
-sys.path.insert(0, os.getcwd()) # pylint: disable=C0413
+from .clients import Client
+from .command import Command
+from .default import Default
+from .excepts import Error, debug
+from .message import Event
+from .objects import Object
+from .parsers import parse_command, spl
+from .storage import Storage, cdir
+from .threads import launch
+
+
+def __dir__():
+    return (
+        'Cfg',
+        'Console',
+        'cmnd',
+        'daemon',
+        'forever',
+        'main',
+        'privileges',
+        'scan',
+        'wrap',
+        'wrapped'
+    )
+
+
+__all__ = __dir__()
+
+
+Cfg         = Default()
+Cfg.mod     = "cmd,err,mod,mre,pwd,thr"
+Cfg.name    = "op"
+Cfg.version = "5"
+Cfg.wd      = os.path.expanduser(f"~/.{Cfg.name}")
+Cfg.pidfile = os.path.join(Cfg.wd, f"{Cfg.name}.pid")
+Cfg.user    = getpass.getuser()
+Storage.wd  = Cfg.wd
 
 
-from op.client  import Client, cmnd, parse_cmd
-from op.default import Default
-from op.errors  import debug, enable, errors
-from op.event   import Event
-from op.object  import cdir
-from op.run     import broker, dte, init, scan
-from op.workdir import Workdir, skel
-
-
-from op import mod
-
-
-Cfg             = Default()
-Cfg.dis         = ""
-Cfg.mod         = "cmd,mod"
-Cfg.opts        = ""
-Cfg.name        = __file__.rsplit(os.sep, maxsplit=1)[-1]
-Cfg.version     = "1"
-Cfg.wdr         = os.path.expanduser(f"~/.{Cfg.name}")
-Cfg.pidfile     = os.path.join(Cfg.wdr, f"{Cfg.name}.pid")
-
-
-Workdir.workdir = Cfg.wdr
+from . import mods as modules
 
 
 class Console(Client):
 
-    "Console"
-
-    def __init__(self):
-        Client.__init__(self)
-        broker.add(self)
-
     def announce(self, txt):
-        "disable announce."
+        pass
 
     def callback(self, evt):
-        "wait for callback."
         Client.callback(self, evt)
         evt.wait()
 
-    def poll(self):
-        "poll console and create event."
+    def poll(self) -> Event:
         evt = Event()
         evt.orig = object.__repr__(self)
         evt.txt = input("> ")
         evt.type = "command"
         return evt
 
-    def say(self, _channel, txt):
-        "print to console"
+    def say(self, channel, txt):
         txt = txt.encode('utf-8', 'replace').decode()
         print(txt)
 
 
+def cmnd(txt):
+    evn = Event()
+    evn.txt = txt
+    Command.handle(evn)
+    evn.wait()
+    return evn
+
+
 def daemon(pidfile, verbose=False):
-    "switch to background."
-    # pylint: disable=W0212
     pid = os.fork()
     if pid != 0:
         os._exit(0)
     os.setsid()
     pid2 = os.fork()
     if pid2 != 0:
         os._exit(0)
@@ -94,67 +107,101 @@
     if os.path.exists(pidfile):
         os.unlink(pidfile)
     cdir(os.path.dirname(pidfile))
     with open(pidfile, "w", encoding="utf-8") as fds:
         fds.write(str(os.getpid()))
 
 
+def forever():
+    while 1:
+        try:
+            time.sleep(1.0)
+        except (KeyboardInterrupt, EOFError):
+            _thread.interrupt_main()
+
+
 def privileges(username):
-    "drop privileges."
     pwnam = pwd.getpwnam(username)
     os.setgid(pwnam.pw_gid)
     os.setuid(pwnam.pw_uid)
 
 
-def wrap(func):
-    "restore console."
+def scan(pkg, modstr, initer=False, wait=True) -> []:
+    mds = []
+    for modname in spl(modstr):
+        module = getattr(pkg, modname, None)
+        if not module:
+            continue
+        for _key, cmd in inspect.getmembers(module, inspect.isfunction):
+            if 'event' in cmd.__code__.co_varnames:
+                Command.add(cmd)
+        for _key, clz in inspect.getmembers(module, inspect.isclass):
+            if not issubclass(clz, Object):
+                continue
+            Storage.add(clz)
+        if initer and "init" in dir(module):
+            module._thr = launch(module.init, name=f"init {modname}")
+            mds.append(module)
+    if wait and initer:
+        for mod in mds:
+            mod._thr.join()
+    return mds
+
+
+def main():
+    Storage.skel()
+    parse_command(Cfg, " ".join(sys.argv[1:]))
+    if "a" in Cfg.opts:
+        Cfg.mod = ",".join(modules.__dir__())
+    if "v" in Cfg.opts:
+        dte = time.ctime(time.time()).replace("  ", " ")
+        debug(f"{Cfg.name.upper()} started {Cfg.opts.upper()} started {dte}")
+    if "d" in Cfg.opts:
+        daemon(Cfg.pidfile)
+        moddir = os.path.join(Storage.wd, "mods")
+        if os.path.exists(moddir) and "m" in Cfg.opts:
+            sys.path.insert(0, os.path.dirname(moddir))
+            import mods
+            if "a" in Cfg.opts:
+                Cfg.mod += "," +  ",".join(mods.__dir__())
+            scan(mods, Cfg.mod, True)
+        privileges(Cfg.user)
+        scan(modules, Cfg.mod, True)
+        forever()
+        return
+    if os.path.exists("mods") and "m" in Cfg.opts:
+        import mods
+        if "a" in Cfg.opts:
+            Cfg.mod += "," +  ",".join(mods.__dir__())
+        scan(mods, Cfg.mod)
+    csl = Console()
+    if "c" in Cfg.opts:
+        scan(modules, Cfg.mod, True, True)
+        csl.start()
+        forever()
+    if Cfg.otxt:
+        scan(modules, Cfg.mod)
+        return cmnd(Cfg.otxt)
+
+
+def wrap(func) -> None:
     old2 = None
     try:
         old2 = termios.tcgetattr(sys.stdin.fileno())
     except termios.error:
         pass
     try:
         func()
     except (KeyboardInterrupt, EOFError):
         print("")
     finally:
         if old2:
             termios.tcsetattr(sys.stdin.fileno(), termios.TCSADRAIN, old2)
 
 
-def main():
-    "main"
-    enable(print)
-    skel()
-    parse_cmd(Cfg, " ".join(sys.argv[1:]))
-    if Cfg.sets.dis:
-        Cfg.dis += "," + Cfg.sets.dis
-    if "a" in Cfg.opts:
-        Cfg.mod = ",".join(mod.__dir__())
-    scan(mod, Cfg.mod, Cfg.dis)
-    if "v" in Cfg.opts:
-        debug(f"{Cfg.name.upper()} {Cfg.opts.upper()} started {dte}")
-        debug(f"scanned {Cfg.mod}")
-    if "h" in Cfg.opts:
-        print(__doc__)
-    elif "d" in Cfg.opts:
-        Cfg.mod  = ",".join(mod.__dir__())
-        Cfg.user = getpass.getuser()
-        daemon(Cfg.pidfile, "v" in Cfg.opts)
-        privileges(Cfg.user)
-        init(mod, Cfg.mod, Cfg.dis)
-        while 1:
-            time.sleep(1.0)
-    elif "c" in Cfg.opts:
-        init(mod, Cfg.mod, Cfg.dis)
-        csl = Console()
-        csl.start()
-        while 1:
-            time.sleep(1.0)
-    elif Cfg.otxt:
-        cmnd(Cfg.otxt, print)
+def wrapped():
+    wrap(main)
+    Error.show()
 
 
 if __name__ == "__main__":
-    readline.redisplay()
-    wrap(main)
-    errors()
+    wrapped()
```

### Comparing `libop-30/op/mod/irc.py` & `libop-5/op/mods/irc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,47 @@
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C,R,E1101,W0105,W0718,W0612,E0611
 
 
 "internet relay chat"
 
 
-import base64
 import os
 import queue
 import socket
 import ssl
 import textwrap
 import threading
 import time
 import _thread
 
 
-from ..client    import Client, command
-from ..default   import Default
-from ..event     import Event
-from ..errors    import Errors, debug, later
-from ..find      import last
-from ..object    import Object, edit, fmt, keys, values
-from ..run       import broker
-from ..thread    import launch
-from ..whitelist import whitelist
-from ..workdir   import sync
+from .. import Default, Object, edit, fmt, keys
+from .. import Client, Command, Error, Event
+from .. import byorig, debug, last, launch, write
 
 
-NAME    = __file__.split(os.sep)[-3]
-saylock = _thread.allocate_lock()
+Error.filter = ["PING", "PONG", "PRIVMSG"]
+
 
+NAME = "op"
 
-Errors.filter = ["PING", "PONG", "PRIVMSG"]
+
+saylock = _thread.allocate_lock()
 
 
 def init():
-    "initialize a irc bot."
     irc = IRC()
     irc.start()
     irc.events.joined.wait()
     return irc
 
 
-def shutdown():
-    "shutdown irc bot."
-    for bot in values(broker.objs):
-        if "irc" not in str(type(bot)).lower():
-            continue
-        debug(f"IRC stopping {repr(bot)}")
-        bot.state.pongcheck = True
-        bot.state.keeprunning = False
-        bot.events.connected.clear()
-        bot.stop()
-
-
-class Config(Default): # pylint: disable=R0902,R0903
-
-    "Config"
+class Config(Default):
 
     channel = f'#{NAME}'
     commands = True
     control = '!'
     edited = time.time()
     nick = NAME
     port = 6667
@@ -80,21 +61,16 @@
         self.nick = self.nick or Config.nick
         self.port = self.port or Config.port
         self.realname = self.realname or Config.realname
         self.server = self.server or Config.server
         self.username = self.username or Config.username
 
 
-whitelist(Config)
-
-
 class TextWrap(textwrap.TextWrapper):
 
-    "TextWrap"
-
     def __init__(self):
         super().__init__()
         self.break_long_words = False
         self.drop_whitespace = False
         self.fix_sentence_endings = True
         self.replace_whitespace = True
         self.tabsize = 4
@@ -102,54 +78,46 @@
 
 
 wrapper = TextWrap()
 
 
 class Output():
 
-    "Output"
-
     cache = Object()
 
     def __init__(self):
         self.dostop = threading.Event()
         self.oqueue = queue.Queue()
 
     def dosay(self, channel, txt):
-        "overload this."
         raise NotImplementedError
 
     @staticmethod
     def extend(channel, txtlist):
-        "add list of txt to channel cache."
         if channel not in Output.cache:
             Output.cache[channel] = []
-        chanlist = getattr(Output.cache, channel)
-        chanlist.extend(txtlist)
+        Output.cache[channel].extend(txtlist)
 
     @staticmethod
     def gettxt(channel):
-        "return text from channel cache."
         txt = None
         try:
             che = getattr(Output.cache, channel, None)
             if che:
                 txt = che.pop(0)
         except (KeyError, IndexError):
             pass
         return txt
 
     def oput(self, channel, txt):
-        "put text to output queue."
-        if channel and channel not in dir(Output.cache):
+        if channel not in dir(Output.cache):
             setattr(Output.cache, channel, [])
         self.oqueue.put_nowait((channel, txt))
 
     def out(self):
-        "output loop."
         while not self.dostop.is_set():
             (channel, txt) = self.oqueue.get()
             if channel is None and txt is None:
                 break
             if self.dostop.is_set():
                 break
             txtlist = wrapper.wrap(txt)
@@ -164,39 +132,34 @@
             _nr = -1
             for txt in txtlist:
                 _nr += 1
                 self.dosay(channel, txt)
 
     @staticmethod
     def size(chan):
-        "return size of channel cache."
         if chan in Output.cache:
-            return len(getattr(Output.cache, chan, []))
+            return len(Output.cache.get(chan, []))
         return 0
 
 
 class IRC(Client, Output):
 
-    "IRC"
-
     def __init__(self):
         Client.__init__(self)
         Output.__init__(self)
         self.buffer = []
         self.cfg = Config()
-        self.channels = []
         self.events = Default()
         self.events.authed = threading.Event()
         self.events.connected = threading.Event()
         self.events.joined = threading.Event()
         self.events.ready = threading.Event()
+        self.channels = []
         self.sock = None
         self.state = Default()
-        self.state.dostop = False
-        self.state.error = ""
         self.state.keeprunning = False
         self.state.lastline = ""
         self.state.nrconnect = 0
         self.state.nrsend = 0
         self.zelf = ''
         self.register('903', cb_h903)
         self.register('904', cb_h903)
@@ -204,23 +167,20 @@
         self.register('CAP', cb_cap)
         self.register('ERROR', cb_error)
         self.register('LOG', cb_log)
         self.register('NOTICE', cb_notice)
         self.register('PRIVMSG', cb_privmsg)
         self.register('QUIT', cb_quit)
         self.register("366", cb_ready)
-        broker.add(self)
 
     def announce(self, txt):
-        "announce on all channels."
         for channel in self.channels:
             self.oput(channel, txt)
 
-    def docommand(self, cmd, *args):
-        "send command to server."
+    def command(self, cmd, *args):
         with saylock:
             if not args:
                 self.raw(cmd)
             elif len(args) == 1:
                 self.raw(f'{cmd.upper()} {args[0]}')
             elif len(args) == 2:
                 txt = ' '.join(args[1:])
@@ -229,15 +189,14 @@
                 txt = ' '.join(args[2:])
                 self.raw("{cmd.upper()} {args[0]} {args[1]} :{txt}")
             if (time.time() - self.state.last) < 5.0:
                 time.sleep(5.0)
             self.state.last = time.time()
 
     def connect(self, server, port=6667):
-        "connect to server."
         self.state.nrconnect += 1
         self.events.connected.clear()
         if self.cfg.password:
             debug("using SASL")
             self.cfg.sasl = True
             self.cfg.port = "6697"
             ctx = ssl.SSLContext(ssl.PROTOCOL_TLS)
@@ -256,113 +215,101 @@
             self.sock.setblocking(True)
             self.sock.settimeout(180.0)
             self.events.connected.set()
             return True
         return False
 
     def direct(self, txt):
-        "send text directly on the socket."
         with saylock:
             self.raw(txt)
             time.sleep(2.0)
 
     def disconnect(self):
-        "disconnect from server."
         try:
             self.sock.shutdown(2)
         except (
                 ssl.SSLError,
                 OSError,
                 BrokenPipeError
-               ) as _ex:
+               ) as ex:
             pass
-        except Exception as ex: # pylint: disable=W0718
-            later(ex)
+        except Exception as ex:
+            Error.errors.append(ex)
 
     def doconnect(self, server, nck, port=6667):
-        "loop until connected."
         while 1:
             try:
                 if self.connect(server, port):
                     break
             except (
                     ssl.SSLError,
                     OSError,
                     ConnectionResetError
                    ) as ex:
-                self.state.error = str(ex)
+                self.state.errors = str(ex)
                 debug(str(ex))
             debug(f"sleeping {self.cfg.sleep} seconds")
             time.sleep(self.cfg.sleep)
         self.logon(server, nck)
 
     def event(self, txt):
-        "create an event."
         evt = self.parsing(txt)
         cmd = evt.command
         if cmd == 'PING':
             self.state.pongcheck = True
-            self.docommand('PONG', evt.txt or '')
+            self.command('PONG', evt.txt or '')
         elif cmd == 'PONG':
             self.state.pongcheck = False
         if cmd == '001':
             self.state.needconnect = False
             if self.cfg.servermodes:
-                self.docommand(f'MODE {self.cfg.nick} {self.cfg.servermodes}')
+                self.command(f'MODE {self.cfg.nick} {self.cfg.servermodes}')
             self.zelf = evt.args[-1]
         elif cmd == "376":
             self.joinall()
         elif cmd == '002':
             self.state.host = evt.args[2][:-1]
         elif cmd == '366':
-            self.state.error = ""
+            self.state.errors = []
             self.events.joined.set()
         elif cmd == '433':
-            self.state.error = txt
+            self.state.errors = txt
             nck = self.cfg.nick + '_'
-            self.docommand('NICK', nck)
+            self.command('NICK', nck)
         return evt
 
     def joinall(self):
-        "join all channels."
         for channel in self.channels:
-            self.docommand('JOIN', channel)
+            self.command('JOIN', channel)
 
     def keep(self):
-        "keep alive."
         while not self.stopped.is_set():
-            if self.state.stopkeep:
-                self.state.stopkeep = False
-                break
             self.events.connected.wait()
             self.events.authed.wait()
             self.state.keeprunning = True
             time.sleep(self.cfg.sleep)
             self.state.pongcheck = True
-            self.docommand('PING', self.cfg.server)
+            self.command('PING', self.cfg.server)
             if self.state.pongcheck:
                 debug("failed pongcheck, restarting")
                 self.state.pongcheck = False
                 self.state.keeprunning = False
                 self.events.connected.clear()
                 self.stop()
                 init()
                 break
 
     def logon(self, server, nck):
-        "log onto server,"
         self.events.connected.wait()
         self.events.authed.wait()
         self.direct(f'NICK {nck}')
         self.direct(f'USER {nck} {server} {server} {nck}')
 
 
     def parsing(self, txt):
-        "parse text into an event."
-        # pylint: disable=R0912,R0915
         rawstr = str(txt)
         rawstr = rawstr.replace('\u0001', '')
         rawstr = rawstr.replace('\001', '')
         debug(txt)
         obj = Event()
         obj.args = []
         obj.rawstr = rawstr
@@ -416,15 +363,14 @@
             obj.rest = " ".join(obj.args)
         obj.orig = object.__repr__(self)
         obj.txt = obj.txt.strip()
         obj.type = obj.command
         return obj
 
     def poll(self):
-        "poll for event."
         self.events.connected.wait()
         if not self.buffer:
             try:
                 self.some()
             except BlockingIOError as ex:
                 time.sleep(1.0)
                 return self.event(str(ex))
@@ -432,27 +378,26 @@
                     OSError,
                     socket.timeout,
                     ssl.SSLError,
                     ssl.SSLZeroReturnError,
                     ConnectionResetError,
                     BrokenPipeError
                    ) as ex:
-                later(ex)
+                Error.add(ex)
                 self.stop()
                 debug("handler stopped")
                 evt = self.event(str(ex))
                 return evt
         try:
             txt = self.buffer.pop(0)
         except IndexError:
             txt = ""
         return self.event(txt)
 
     def raw(self, txt):
-        "send raw text."
         txt = txt.rstrip()
         debug(txt)
         txt = txt[:500]
         txt += '\r\n'
         txt = bytes(txt, 'utf-8')
         if self.sock:
             try:
@@ -460,214 +405,173 @@
             except (
                     OSError,
                     ssl.SSLError,
                     ssl.SSLZeroReturnError,
                     ConnectionResetError,
                     BrokenPipeError
                    ) as ex:
-                later(ex)
+                Error.errors.append(ex)
                 self.stop()
                 return
         self.state.last = time.time()
         self.state.nrsend += 1
 
     def reconnect(self):
-        "reconnect to server."
         debug(f"reconnecting to {self.cfg.server}")
         try:
             self.disconnect()
         except (ssl.SSLError, OSError):
             pass
         self.events.connected.clear()
         self.events.joined.clear()
         self.doconnect(self.cfg.server, self.cfg.nick, int(self.cfg.port))
 
     def dosay(self, channel, txt):
-        "method for output cache."
         self.events.joined.wait()
         txt = str(txt).replace('\n', '')
         txt = txt.replace('  ', ' ')
-        self.docommand('PRIVMSG', channel, txt)
+        self.command('PRIVMSG', channel, txt)
 
     def say(self, channel, txt):
-        "say text on channel."
         self.oput(channel, txt)
 
     def some(self):
-        "parse part of input text."
         self.events.connected.wait()
         if not self.sock:
             return
         inbytes = self.sock.recv(512)
         txt = str(inbytes, 'utf-8')
         if txt == '':
             raise ConnectionResetError
         self.state.lastline += txt
         splitted = self.state.lastline.split('\r\n')
         for line in splitted[:-1]:
             self.buffer.append(line)
         self.state.lastline = splitted[-1]
 
     def start(self):
-        "start bot."
         last(self.cfg)
         if self.cfg.channel not in self.channels:
             self.channels.append(self.cfg.channel)
         self.events.connected.clear()
         self.events.joined.clear()
         launch(Output.out, self)
-        launch(Client.start, self)
+        Client.start(self)
         launch(
                self.doconnect,
                self.cfg.server or "localhost",
                self.cfg.nick,
                int(self.cfg.port or '6667')
               )
         if not self.state.keeprunning:
             launch(self.keep)
 
     def stop(self):
-        "stop bot."
-        self.state.stopkeep = True
         self.disconnect()
         self.dostop.set()
         self.oput(None, None)
         Client.stop(self)
 
     def wait(self):
-        "wait for ready."
         self.events.ready.wait()
 
 
-def cb_auth(bot, evt):
-    "auth callback."
-    bot.docommand(f'AUTHENTICATE {bot.cfg.password}')
+def cb_auth(evt):
+    bot = byorig(evt.orig)
+    bot.command(f'AUTHENTICATE {bot.cfg.password}')
 
 
-def cb_cap(bot, evt):
-    "capabilities callback."
+def cb_cap(evt):
+    bot = byorig(evt.orig)
     if bot.cfg.password and 'ACK' in evt.arguments:
         bot.direct('AUTHENTICATE PLAIN')
     else:
         bot.direct('CAP REQ :sasl')
 
 
-def cb_error(bot, evt):
-    "error callback."
-    if not bot.state.nrerror:
-        bot.state.nrerror = 0
+def cb_error(evt):
+    bot = byorig(evt.orig)
     bot.state.nrerror += 1
-    bot.state.error = evt.txt
+    bot.state.errors.append(evt.txt)
     debug(evt.txt)
 
 
-def cb_h903(bot, evt):
-    "auth succeded callback."
+def cb_h903(evt):
+    bot = byorig(evt.orig)
     bot.direct('CAP END')
     bot.events.authed.set()
 
 
-def cb_h904(bot, evt):
-    "auth succeded callback."
+def cb_h904(evt):
+    bot = byorig(evt.orig)
     bot.direct('CAP END')
     bot.events.authed.set()
 
 
-def cb_kill(bot, evt):
-    "got killed callback."
+def cb_kill(evt):
+    pass
 
 
-def cb_log(bot, evt):
-    "log callback."
+def cb_log(evt):
+    pass
 
 
-def cb_ready(bot, evt):
-    "bot is ready callback."
-    bot.events.ready.set()
+def cb_ready(evt):
+    bot = byorig(evt.orig)
+    if bot:
+        bot.events.ready.set()
 
 
-def cb_001(bot, evt):
-    "first line received callback."
+def cb_001(evt):
+    bot = byorig(evt.orig)
     bot.logon()
 
 
-def cb_notice(bot, evt):
-    "notice callback."
+def cb_notice(evt):
+    bot = byorig(evt.orig)
     if evt.txt.startswith('VERSION'):
         txt = f'\001VERSION {NAME.upper()} 140 - {bot.cfg.username}\001'
-        bot.docommand('NOTICE', evt.channel, txt)
+        bot.command('NOTICE', evt.channel, txt)
 
 
-def cb_privmsg(bot, evt):
-    "privmsg callback."
+def cb_privmsg(evt):
+    bot = byorig(evt.orig)
     if not bot.cfg.commands:
         return
     if evt.txt:
         if evt.txt[0] in ['!',]:
             evt.txt = evt.txt[1:]
         elif evt.txt.startswith(f'{bot.cfg.nick}:'):
             evt.txt = evt.txt[len(bot.cfg.nick)+1:]
         else:
             return
         if evt.txt:
             evt.txt = evt.txt[0].lower() + evt.txt[1:]
         debug(f"command from {evt.origin}: {evt.txt}")
-        command(bot, evt)
+        Command.handle(evt)
 
 
-def cb_quit(bot, evt):
-    "quit callback."
+def cb_quit(evt):
+    bot = byorig(evt.orig)
     debug(f"quit from {bot.cfg.server}")
     if evt.orig and evt.orig in bot.zelf:
         bot.stop()
 
 
+"commands"
+
+
 def cfg(event):
-    "configure command."
     config = Config()
     path = last(config)
     if not event.sets:
         event.reply(
                     fmt(
                         config,
                         keys(config),
                         skip='control,password,realname,sleep,username'.split(",")
                        )
                    )
     else:
         edit(config, event.sets)
-        sync(config, path)
+        write(config, path)
         event.reply('ok')
-
-
-def mre(event):
-    "show from output cache."
-    if not event.channel:
-        event.reply('channel is not set.')
-        return
-    bot = broker.get(event.orig)
-    if 'cache' not in dir(bot):
-        event.reply('bot is missing cache')
-        return
-    if event.channel not in bot.cache:
-        event.reply(f'no output in {event.channel} cache.')
-        return
-    for _x in range(3):
-        txt = bot.gettxt(event.channel)
-        if txt:
-            bot.say(event.channel, txt)
-    size = bot.size(event.channel)
-    event.reply(f'{size} more in cache')
-
-
-def pwd(event):
-    "create a base64 password."
-    if len(event.args) != 2:
-        event.reply('pwd <nick> <password>')
-        return
-    arg1 = event.args[0]
-    arg2 = event.args[1]
-    txt = f'\x00{arg1}\x00{arg2}'
-    enc = txt.encode('ascii')
-    base = base64.b64encode(enc)
-    dcd = base.decode('ascii')
-    event.reply(dcd)
```

### Comparing `libop-30/op/mod/log.py` & `libop-5/op/mods/log.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C0115,C0116,E0402,R0903,E0611
 
 
 "log text"
 
 
 import time
 
 
-from ..client    import laps
-from ..object    import Object
-from ..find      import find, fntime
-from ..workdir   import sync
+from .. import Object, find, fntime, laps, write
 
 
-class Log(Object): # pylint: disable=R0903
-
-    "Log"
+class Log(Object):
 
     def __init__(self):
         super().__init__()
         self.txt = ''
 
 
 def log(event):
-    "log text."
     if not event.rest:
         nmr = 0
         for fnm, obj in find('log'):
             lap = laps(time.time() - fntime(fnm))
             event.reply(f'{nmr} {obj.txt} {lap}')
             nmr += 1
         if not nmr:
             event.reply('no log')
         return
     obj = Log()
     obj.txt = event.rest
-    sync(obj)
+    write(obj)
     event.reply('ok')
```

### Comparing `libop-30/op/mod/mbx.py` & `libop-5/op/mods/mbx.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R
+# pylint: disable=C0103,C0209,C0301,C0115,C0116,W0212,R0903
 
 
 "mailbox"
 
 
 import mailbox
 import os
 import time
 
 
-from ..object    import Object, fmt, update
-from ..client    import laps
-from ..find      import find, fntime
-from ..whitelist import whitelist
-from ..workdir   import sync
+from .. import Object, find, fmt, fntime, laps, write, update
 
 
-MONTH = {
+bdmonths = ['Bo', 'Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul', 'Aug', 'Sep', 'Oct', 'Nov', 'Dec']
+
+
+monthint = {
     'Jan': 1,
     'Feb': 2,
     'Mar': 3,
     'Apr': 4,
     'May': 5,
     'Jun': 6,
     'Jul': 7,
@@ -32,91 +31,84 @@
     'Nov': 11,
     'Dec': 12
 }
 
 
 class Email(Object):
 
-    "Email"
-
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.text = ""
 
 
-whitelist(Email)
-
-
 def to_date(date):
-    "match date in string." 
     date = date.replace("_", ":")
     res = date.split()
     ddd = ""
     try:
         if "+" in res[3]:
             raise ValueError
         if "-" in res[3]:
             raise ValueError
         int(res[3])
-        ddd = "{:4}-{:#02}-{:#02} {:6}".format(res[3], MONTH[res[2]], int(res[1]), res[4])
+        ddd = "{:4}-{:#02}-{:#02} {:6}".format(res[3], monthint[res[2]], int(res[1]), res[4])
     except (IndexError, KeyError, ValueError) as ex:
         try:
             if "+" in res[4]:
                 raise ValueError from ex
             if "-" in res[4]:
                 raise ValueError from ex
             int(res[4])
-            ddd = "{:4}-{:#02}-{:02} {:6}".format(res[4], MONTH[res[1]], int(res[2]), res[3])
+            ddd = "{:4}-{:#02}-{:02} {:6}".format(res[4], monthint[res[1]], int(res[2]), res[3])
         except (IndexError, KeyError, ValueError):
             try:
-                ddd = "{:4}-{:#02}-{:02} {:6}".format(res[2], MONTH[res[1]], int(res[0]), res[3])
+                ddd = "{:4}-{:#02}-{:02} {:6}".format(res[2], monthint[res[1]], int(res[0]), res[3])
             except (IndexError, KeyError):
                 try:
-                    ddd = "{:4}-{:#02}-{:02}".format(res[2], MONTH[res[1]], int(res[0]))
+                    ddd = "{:4}-{:#02}-{:02}".format(res[2], monthint[res[1]], int(res[0]))
                 except (IndexError, KeyError):
                     try:
-                        ddd = "{:4}-{:#02}".format(res[2], MONTH[res[1]])
+                        ddd = "{:4}-{:#02}".format(res[2], monthint[res[1]])
                     except (IndexError, KeyError):
                         try:
                             ddd = "{:4}".format(res[2])
                         except (IndexError, KeyError):
                             ddd = ""
     return ddd
 
 
 def cor(event):
-    "correspondence"
     if not event.args:
         event.reply("cor <email>")
         return
     nr = -1
     for _fn, email in find("email", {"From": event.args[0]}):
         nr += 1
         txt = ""
         if len(event.args) > 1:
             txt = ",".join(event.args[1:])
         else:
             txt = "From,Subject"
         event.reply("%s %s %s" % (nr, fmt(email, txt, plain=True), laps(time.time() - fntime(email.__stp__))))
 
 
+
 def eml(event):
-    "emnail"
     if not event.args:
         event.reply("eml <searchtxtinemail>")
         return
     nr = -1
     for fn, o in find("email"):
         if event.rest in o.text:
             nr += 1
             event.reply("%s %s %s" % (nr, fmt(o, "From,Subject"), laps(time.time() - fntime(fn))))
 
 
+
 def mbx(event):
-    "mailbox"
     if not event.args:
         return
     fn = os.path.expanduser(event.args[0])
     event.reply("reading from %s" % fn)
     nr = 0
     if os.path.isdir(fn):
         thing = mailbox.Maildir(fn, create=False)
@@ -126,17 +118,17 @@
         return
     try:
         thing.lock()
     except FileNotFoundError:
         pass
     for m in thing:
         o = Email()
-        update(o, m._headers) # pylint: disable=W0212
+        update(o, m._headers)
         o.text = ""
         for payload in m.walk():
             if payload.get_content_type() == 'text/plain':
                 o.text += payload.get_payload()
         o.text = o.text.replace("\\n", "\n")
-        sync(o)
+        write(o)
         nr += 1
     if nr:
         event.reply("ok %s" % nr)
```

### Comparing `libop-30/op/mod/mdl.py` & `libop-5/op/mods/mdl.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C,I,R,W0613,E1101,E0402,W0401,W0105
+# flake8: noqa=E501
 
 
-"genocide model of the netherlands since 01-01-2020"
+"genocide model of the netherlands"
 
 
 import datetime
 import time
 
 
-from ..client   import laps
-from ..event    import Event
-from ..object   import Object, construct, keys, values
-from ..repeater import Repeater
-from ..run      import broker
-from ..thread   import launch
+from .. import Object, construct, keys
+from .. import Event, Fleet, Repeater, laps, launch
 
 
-DAY = 24*60*60
-YEAR = 365*DAY
-SOURCE = "https://github.com/xobjectz/otpcr"
-STARTDATE = "2020-01-01 00:00:00"
-STARTTIME = time.mktime(time.strptime(STARTDATE, "%Y-%m-%d %H:%M:%S"))
+def __dir__():
+    return (
+            'init',
+            'now'
+           ) 
 
 
 def init():
-    "start repeaters"
     for key in keys(oorzaken):
         val = getattr(oorzaken, key, None)
         if val and int(val) > 10000:
             evt = Event()
             evt.txt = ""
             evt.rest = key
             sec = seconds(val)
             repeater = Repeater(sec, cbstats, evt, thrname=aliases.get(key))
             repeater.start()
     launch(daily, name="daily")
+    
+
+DAY = 24*60*60
+YEAR = 365*DAY
+SOURCE = "https://github.com/bthate/genocide"
+STARTDATE = "2020-01-01 00:00:00"
+STARTTIME = time.mktime(time.strptime(STARTDATE, "%Y-%m-%d %H:%M:%S"))
 
 
 oor = """"Totaal onderliggende doodsoorzaken (aantal)";
          "1 Infectieuze en parasitaire ziekten/Totaal infectieuze en parasitaire zktn (aantal)";
          "1 Infectieuze en parasitaire ziekten/1.1 Tuberculose (aantal)";
          "1 Infectieuze en parasitaire ziekten/1.2 Meningokokkeninfecties (aantal)";
          "1 Infectieuze en parasitaire ziekten/1.3 Virale hepatitis (aantal)";
@@ -269,89 +274,78 @@
 
 
 oorzaak = Object()
 construct(oorzaak, zip(oor, aantal))
 oorzaken = Object()
 
 
+
 def getalias(txt):
-    "return value of alias."
-    result = None
     for key, value in aliases.items():
         if txt.lower() in key.lower():
-            result = value
-            break
-    return result
+            return value
+
 
 def getday():
-    "timestamp of current day."
     day = datetime.datetime.now()
     day = day.replace(hour=0, minute=0, second=0, microsecond=0)
     return day.timestamp()
 
 
 def getnr(name):
-    "fetch mortality number."
     for k in keys(oorzaken):
         if name.lower() in k.lower():
             return int(getattr(oorzaken, k))
     return 0
 
 
 def seconds(nrs):
-    "convert nr/years to seconds."
     if not nrs:
         return nrs
     return 60*60*24*365 / float(nrs)
 
 
 
 def iswanted(k, line):
-    "see whether filtered or not."
     for word in line:
         if word in k:
             return True
     return False
 
 
 def daily():
-    "daily job"
     while 1:
         time.sleep(24*60*60)
         evt = Event()
         cbnow(evt)
 
 
 def hourly():
-    "hourly job"
     while 1:
         time.sleep(60*60)
         evt = Event()
         cbnow(evt)
 
 
-def cbnow(_evt):
-    "now callback"
+def cbnow(evt):
     delta = time.time() - STARTTIME
     txt = laps(delta) + " "
     for name in sorted(keys(oorzaken), key=lambda x: seconds(getnr(x))):
         needed = seconds(getnr(name))
         if needed > 60*60:
             continue
         nrtimes = int(delta/needed)
-        txt += f"{getalias(name)} {nrtimes} |"
+        txt += "%s: %s " % (getalias(name), nrtimes)
     txt += " http://genocide.rtfd.io"
-    for bot in values(broker.objs):
+    for bot in Fleet.objs:
         if "announce" in dir(bot):
             bot.announce(txt)
 
 
 def cbstats(evt):
-    "stats callback."
-    # pylint: disable=C0209
     name = evt.rest or "Psych"
     needed = seconds(getnr(name))
     if needed:
         delta = time.time() - STARTTIME
         nrtimes = int(delta/needed)
         nryear = int(YEAR/needed)
         nrday = int(DAY/needed)
@@ -361,21 +355,19 @@
                                                                nrtimes,
                                                                getalias(name),
                                                                thisday,
                                                                nrday,
                                                                laps(needed),
                                                                nryear,
                                                               )
-        for bot in values(broker.objs):
+        for bot in Fleet.objs:
             bot.announce(txt)
 
 
 def now(event):
-    "now command."
-    # pylint: disable=C0209
     name = event.rest or "Psych"
     needed = seconds(getnr(name))
     if needed:
         delta = time.time() - STARTTIME
         txt = laps(delta) + " "
         nrtimes = int(delta/needed)
         nryear = int(YEAR/needed)
@@ -391,15 +383,14 @@
                                                                 )
         event.reply(txt)
     else:
         event.reply("not needed")
 
 
 def boot():
-    "construct model"
     _nr = -1
     for key in keys(oorzaak):
         _nr += 1
         if _nr == 0:
             continue
         if key.startswith('"'):
             key = key[1:]
@@ -421,15 +412,8 @@
         atl = atl.replace(", bevalling en kraambed. ", "")
         atl = atl.replace("Aandoeningen v.d. ", "")
         nms = " ".join(atl.split()[1:]).capitalize()
         nms = nms.strip()
         setattr(oorzaken, nms, aantal[_nr])
 
 
-def __dir__():
-    return (
-            'init',
-            'now'
-           )
-
-
 boot()
```

### Comparing `libop-30/op/mod/req.py` & `libop-5/op/mods/req.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C0115,C0116
 
 
 """| **Information and Evidence Unit**
 | **Office of the Prosecutor**
 | **Post Office Box 19519**
 | **2500 CM The Hague**
 | **The Netherlands**
 |
-|
 
-Hello Office of the Prosecutor, ``OTP-CR-117/19``
+Hello Office of the Prosecutor,
 
 i write you in the context of communications and claims under art.15 of
 the Rome Statute. i want to inform the prosecutor that the king of the
 netherlands and his government are commiting 3 of the 5 crimes defined
 in the Rome Statute.
 
 The dutch government has introduced three new forced care laws, the Wfz
@@ -75,9 +76,8 @@
 
 (1) provided are the confirmation letters of both the chamber and the king.
 (2) your reference: OTP-CR-117/19
 """
 
 
 def req(event):
-    "reconsider"
     event.reply(__doc__)
```

### Comparing `libop-30/op/mod/rst.py` & `libop-5/op/mods/rst.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,137 +1,111 @@
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C,R,W0612,W0613
 
 
-"rest"
+""" rest interface. """
 
 
 import os
 import sys
 import time
 
 
 from http.server import HTTPServer, BaseHTTPRequestHandler
 
 
-from ..default import Default
-from ..errors  import debug, later
-from ..find    import fns
-from ..object  import Object
-from ..thread  import launch
-from ..workdir import Workdir
+from .. import Default, Object
+from .. import Error, Storage, debug, launch
 
 
 def init():
-    "start object server."
-    result = None
-    try:
-        result = REST((Config.hostname, int(Config.port)), RESTHandler)
-    except OSError:
-        pass
-    if result:
-        launch(result.start)
-    return result
+    rest = REST((Config.hostname, int(Config.port)), RESTHandler)
+    launch(rest.start)
+    return rest
 
 
-class Config(Default):
+def html(txt):
+    return """<!doctype html>
+<html>
+   %s
+</html>
+""" % txt
+
 
-    "Config"
+class Config(Default):
 
     hostname = "localhost"
     port     = 10102
 
-    def __bla__(self):
-        pass
-
-    def __blabla__(self):
-        pass
-
 
 class REST(HTTPServer, Object):
 
-    "REST"
-
     allow_reuse_address = True
     daemon_thread = True
 
     def __init__(self, *args, **kwargs):
         HTTPServer.__init__(self, *args, **kwargs)
         Object.__init__(self)
         self.host = args[0]
         self._last = time.time()
         self._starttime = time.time()
         self._status = "start"
 
     def exit(self):
-        "shutdown server."
         self._status = ""
         time.sleep(0.2)
         self.shutdown()
 
-    def start(self):
-        "start server/"
+    def start(self): 
         self._status = "ok"
         self.serve_forever()
 
     def request(self):
-        "handler request."
         self._last = time.time()
 
     def error(self, request, addr):
-        "handle error."
-        exctype, excvalue, _tb = sys.exc_info()
+        exctype, excvalue, tb = sys.exc_info()
         exc = exctype(excvalue)
-        later(exc)
-        if request:
-            debug(f'{addr} {excvalue}')
+        Error.add(exc)
+        debug('%s %s' % (addr, excvalue))
 
 
 class RESTHandler(BaseHTTPRequestHandler):
 
-    "RESTHandler"
-
     def setup(self):
-        "setup request."
         BaseHTTPRequestHandler.setup(self)
         self._ip = self.client_address[0]
         self._size = 0
 
     def send(self, txt):
-        "send text."
         self.wfile.write(bytes(txt, "utf-8"))
         self.wfile.flush()
 
     def write_header(self, htype='text/plain'):
-        "write a header."
         self.send_response(200)
-        self.send_header('Content-type', f'{htype}; charset="utf-8"')
+        self.send_header('Content-type', '%s; charset=%s ' % (htype, "utf-8"))
         self.send_header('Server', "1")
         self.end_headers()
 
-    def do_GET(self): # pylint: disable=C0103
-        "handle GET."
+    def do_GET(self):
         if self.path == "/":
             self.write_header("text/html")
             txt = ""
-            for fnm in fns():
+            for fnm in Storage.fns():
                 txt += f'<a href="http://{Config.hostname}:{Config.port}/{fnm}">{fnm}</a>\n'
             self.send(html(txt.strip()))
             return
-        fnm = Workdir.workdir + os.sep + "store" + os.sep + self.path
+        fnm = Storage.wd + os.sep + "store" + os.sep + self.path
         try:
-            with open(fnm, "r", encoding="utf-8") as file:
-                txt = file.read()
-                self.write_header("txt/plain")
-                self.send(html(txt))
+            f = open(fnm, "r", encoding="utf-8")
+            txt = f.read()
+            f.close()
+            self.write_header("txt/plain")
+            self.send(html(txt))
         except (TypeError, FileNotFoundError, IsADirectoryError) as ex:
             self.send_response(404)
-            later(ex)
+            Error.add(ex)
             self.end_headers()
 
     def log(self, code):
-        "log access."
-        debug(f"{self.address_string()} code {code} path {self.path}")
-
-
-def html(txt):
-    "html template."
-    return f"<!doctype html><html>{txt}</html>"
+        debug('%s code %s path %s' % (self.address_string(), code, self.path))
```

### Comparing `libop-30/op/mod/thr.py` & `libop-5/op/mods/thr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C0116,W0105,E0402,E0401,E0611
 
 
 "show running threads"
 
 
 import threading
 import time
 
 
-from ..client import laps
-from ..object import Object, update
+from .. import Object, laps, update
 
 
 STARTTIME = time.time()
 
 
 def thr(event):
-    "show running threads."
     result = []
     for thread in sorted(threading.enumerate(), key=lambda x: x.name):
         if str(thread).startswith('<_'):
             continue
         obj = Object()
         update(obj, vars(thread))
         if getattr(obj, 'sleep', None):
```

### Comparing `libop-30/op/mod/tmr.py` & `libop-5/op/parsers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C,R,W0718,W0702
 
 
-"timer"
+"parsing text"
 
 
 import datetime
+import os
 import re
 import time as ttime
 
 
-from ..client    import laps
-from ..event     import Event
-from ..find      import find
-from ..object    import update
-from ..run       import broker
-from ..thread    import launch
-from ..timer     import Timer
-from ..workdir   import sync
+from .default import Default
 
 
-def init():
-    "start timers."
-    for _fn, obj in find("timer"):
-        if "time" not in obj:
-            continue
-        diff = float(obj.time) - ttime.time()
-        if diff > 0:
-            bot = broker.first()
-            evt = Event()
-            update(evt, obj)
-            evt.orig = object.__repr__(bot)
-            timer = Timer(diff, evt.show)
-            launch(timer.start)
+def __dir__():
+    return (
+        'NoDate',
+        'fntime',
+        'get_day',
+        'get_hour',
+        'get_time',
+        'laps',
+        'parse_command',
+        'parse_time',
+        'spl',
+        'today',
+        'to_day'
+    )
+
 
+__all__ = __dir__()
 
-MONTHS = [
+
+bdmonths = [
     'Bo',
     'Jan',
     'Feb',
     'Mar',
     'Apr',
     'May',
     'Jun',
@@ -47,67 +47,69 @@
     'Sep',
     'Oct',
     'Nov',
     'Dec'
 ]
 
 
-FORMATS = [
+year_formats = [
     "%Y-%m-%d",
     "%d-%m-%Y",
     "%d-%m",
     "%m-%d",
 ]
 
 
 class NoDate(Exception):
 
-    "NoDate"
+    pass
 
 
 def extract_date(daystr):
-    "extract date from string."
-    res = None
-    for fmt in FORMATS:
+    for fmt in year_formats:
         try:
             res = ttime.mktime(ttime.strptime(daystr, fmt))
-            break
-        except ValueError:
+        except:
             res = None
-    return res
+        if res:
+            return res
+
+
+def fntime(daystr) -> float:
+    daystr = daystr.replace('_', ':')
+    datestr = ' '.join(daystr.split(os.sep)[-2:])
+    if '.' in datestr:
+        datestr, rest = datestr.rsplit('.', 1)
+    else:
+        rest = ''
+    timed = ttime.mktime(ttime.strptime(datestr, '%Y-%m-%d %H:%M:%S'))
+    if rest:
+        timed += float('.' + rest)
+    return timed
 
 
 def get_day(daystr):
-    "return day from string."
-    day = None
-    month = None
-    yea = None
     try:
         ymdre = re.search(r'(\d+)-(\d+)-(\d+)', daystr)
-        if ymdre:
-            (day, month, yea) = ymdre.groups()
-    except ValueError:
+        (day, month, yea) = ymdre.groups()
+    except:
         try:
             ymre = re.search(r'(\d+)-(\d+)', daystr)
-            if ymre:
-                (day, month) = ymre.groups()
-                yea = ttime.strftime("%Y", ttime.localtime())
-        except Exception as ex: # pylint: disable=W0212
+            (day, month) = ymre.groups()
+            yea = ttime.strftime("%Y", ttime.localtime())
+        except Exception as ex:
             raise NoDate(daystr) from ex
-    if day:
-        day = int(day)
-        month = int(month)
-        yea = int(yea)
-        date = f"{day} {MONTHS[month]} {yea}"
-        return ttime.mktime(ttime.strptime(date, r"%d %b %Y"))
-    raise NoDate(daystr)
+    day = int(day)
+    month = int(month)
+    yea = int(yea)
+    date = "%s %s %s" % (day, bdmonths[month], yea)
+    return ttime.mktime(ttime.strptime(date, r"%d %b %Y"))
 
 
 def get_hour(daystr):
-    "return hour from string."
     try:
         hmsre = re.search(r'(\d+):(\d+):(\d+)', str(daystr))
         hours = 60 * 60 * (int(hmsre.group(1)))
         hoursmin = hours  + int(hmsre.group(2)) * 60
         hmsres = hoursmin + int(hmsre.group(3))
     except AttributeError:
         pass
@@ -121,27 +123,117 @@
         return 0
     except ValueError:
         return 0
     return hmsres
 
 
 def get_time(txt):
-    "parse full time string."
     try:
         target = get_day(txt)
     except NoDate:
         target = to_day(today())
     hour =  get_hour(txt)
     if hour:
         target += hour
     return target
 
 
+def laps(seconds, short=True) -> str:
+    txt = ""
+    nsec = float(seconds)
+    if nsec < 1:
+        return f"{nsec:.2f}s"
+    yea = 365*24*60*60
+    week = 7*24*60*60
+    nday = 24*60*60
+    hour = 60*60
+    minute = 60
+    yeas = int(nsec/yea)
+    nsec -= yeas*yea
+    weeks = int(nsec/week)
+    nsec -= weeks*week
+    nrdays = int(nsec/nday)
+    nsec -= nrdays*nday
+    hours = int(nsec/hour)
+    nsec -= hours*hour
+    minutes = int(nsec/minute)
+    nsec -= int(minute*minutes)
+    sec = int(nsec)
+    if yeas:
+        txt += f"{yeas}y"
+    if weeks:
+        nrdays += weeks * 7
+    if nrdays:
+        txt += f"{nrdays}d"
+    if short and txt:
+        return txt.strip()
+    if hours:
+        txt += f"{hours}h"
+    if minutes:
+        txt += f"{minutes}m"
+    if sec:
+        txt += f"{sec}s"
+    txt = txt.strip()
+    return txt
+
+
+def parse_command(obj, txt=None) -> None:
+    args = []
+    obj.args    = obj.args or []
+    obj.cmd     = obj.cmd or ""
+    obj.gets    = obj.gets or Default()
+    obj.hasmods = obj.hasmod or False
+    obj.index   = None
+    obj.mod     = obj.mod or ""
+    obj.opts    = obj.opts or ""
+    obj.result  = obj.reult or []
+    obj.sets    = obj.sets or Default()
+    obj.txt     = txt or obj.txt or ""
+    obj.otxt    = obj.txt
+    _nr = -1
+    for spli in obj.otxt.split():
+        if spli.startswith("-"):
+            try:
+                obj.index = int(spli[1:])
+            except ValueError:
+                obj.opts += spli[1:]
+            continue
+        if "==" in spli:
+            key, value = spli.split("==", maxsplit=1)
+            if key in obj.gets:
+                val = getattr(obj.gets, key)
+                value = val + "," + value
+            setattr(obj.gets, key, value)
+            continue
+        if "=" in spli:
+            key, value = spli.split("=", maxsplit=1)
+            if key == "mod":
+                obj.hasmods = True
+                if obj.mod:
+                    obj.mod += f",{value}"
+                else:
+                    obj.mod = value
+                continue
+            setattr(obj.sets, key, value)
+            continue
+        _nr += 1
+        if _nr == 0:
+            obj.cmd = spli
+            continue
+        args.append(spli)
+    if args:
+        obj.args = args
+        obj.txt  = obj.cmd or ""
+        obj.rest = " ".join(obj.args)
+        obj.txt  = obj.cmd + " " + obj.rest
+    else:
+        obj.txt = obj.cmd or ""
+
+
 def parse_time(txt):
-    "parse time from string."
     seconds = 0
     target = 0
     txt = str(txt)
     for word in txt.split():
         if word.startswith("+"):
             seconds = int(word[1:])
             return ttime.time() + seconds
@@ -155,75 +247,33 @@
             target = to_day(today())
         hour =  get_hour(txt)
         if hour:
             target += hour
     return target
 
 
+def spl(txt) -> []:
+    try:
+        res = txt.split(',')
+    except (TypeError, ValueError):
+        res = txt
+    return [x for x in res if x]
+
+
 def to_day(daystr):
-    "parse day from string."
     previous = ""
     line = ""
     daystr = str(daystr)
-    res = None
     for word in daystr.split():
         line = previous + " " + word
         previous = word
         try:
             res = extract_date(line.strip())
-            break
         except ValueError:
             res = None
+        if res:
+            return res
         line = ""
-    return res
 
 
 def today():
-    "return date."
     return str(datetime.datetime.today()).split()[0]
-
-
-def tmr(event):
-    "add a timer."
-    result = ""
-    if not event.rest:
-        nmr = 0
-        for _fn, obj in find('timer'):
-            lap = float(obj.time) - ttime.time()
-            if lap > 0:
-                event.reply(f'{nmr} {obj.txt} {laps(lap)}')
-                nmr += 1
-        return result
-    seconds = 0
-    line = ""
-    for word in event.args:
-        if word.startswith("+"):
-            try:
-                seconds = int(word[1:])
-            except (ValueError, IndexError):
-                event.reply(f"{seconds} is not an integer")
-                return result
-        else:
-            line += word + " "
-    if seconds:
-        target = ttime.time() + seconds
-    else:
-        try:
-            target = get_day(event.rest)
-        except NoDate:
-            target = to_day(today())
-        hour =  get_hour(event.rest)
-        if hour:
-            target += hour
-    if not target or ttime.time() > target:
-        event.reply("already passed given time.")
-        return result
-    event.time = target
-    diff = target - ttime.time()
-    event.reply("ok " +  laps(diff))
-    event.result = []
-    event.result.append(event.rest)
-    timer = Timer(diff, event.show, thrname=event.cmd)
-    update(timer, event)
-    sync(timer)
-    launch(timer.start)
-    return result
```

### Comparing `libop-30/op/mod/udp.py` & `libop-5/op/mods/udp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,64 +1,57 @@
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C0115,C0116,W0105,E0402,R0903
 
 
 "udp to irc relay"
 
 
 import select
 import socket
 import sys
 import threading
 import time
 
 
-from ..object  import Object, values
-from ..thread  import launch
-from ..run     import broker
+from .. import Fleet, Object, launch
 
 
 def init():
-    "start udp to irc relay."
     udpd = UDP()
     udpd.start()
     return udpd
 
 
-class Cfg(Object): # pylint: disable=R0903
-
-    "Cfg"
+class Cfg(Object):
 
     addr = ""
     host = "localhost"
     port = 5500
 
 
 class UDP(Object):
 
-    "UDP"
-
     def __init__(self):
         Object.__init__(self)
         self.stopped = False
         self._sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         self._sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self._sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
         self._sock.setblocking(1)
         self._starttime = time.time()
         self.ready = threading.Event()
 
     def output(self, txt, addr=None):
-        "output to fleet."
         if addr:
             Cfg.addr = addr
-        for bot in values(broker.objs):
+        for bot in Fleet.objs:
             bot.announce(txt.replace("\00", ""))
 
     def loop(self):
-        "udp input loop."
         try:
             self._sock.bind((Cfg.host, Cfg.port))
         except socket.gaierror:
             return
         self.ready.set()
         while not self.stopped:
             (txt, addr) = self._sock.recvfrom(64000)
@@ -66,35 +59,31 @@
                 break
             data = str(txt.rstrip(), "utf-8")
             if not data:
                 break
             self.output(data, addr)
 
     def exit(self):
-        "stop relay."
         self.stopped = True
         self._sock.settimeout(0.01)
         self._sock.sendto(
                           bytes("exit", "utf-8"),
                           (Cfg.host, Cfg.port)
                          )
 
     def start(self):
-        "start relay."
         launch(self.loop)
 
 
 def toudp(host, port, txt):
-    "send udp packet to bot."
     sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     sock.sendto(bytes(txt.strip(), "utf-8"), (host, port))
 
 
 def udp(event):
-    "send udp command."
     if event.rest:
         toudp(Cfg.host, Cfg.port, event.rest)
         event.reply(f"{len(event.rest)} characters sent")
         return
     if not select.select(
                          [sys.stdin, ],
                          [],
```

### Comparing `libop-30/op/mod/wsd.py` & `libop-5/op/mods/wsd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C,I,R,E0401
 
 
 """| wijsheid, wijs !
 
 | OVERDRACHT
 | ==========
 
@@ -71,15 +73,15 @@
 | levenden in materiaal
 | levenden in hell (uitgebeeld)
 | OVERDRACHT
 | company, mens beheer op aarde, ziet atlen komen en gaan
 | poging tot nieuw start
 | de arc types (hier selecteren om einde aan de rest te noemen)
 | boven gelegd woord (zeewier in vissenbak)
-| het 4 leg zysteem (woord gelegd op schepping .. voor making)
+| het 4 leg systeem (woord gelegd op schepping .. voor making)
 | de immer zijnde dreiging tot einde
 | de weigerende mens hier toe (de weerwil)
 | scheppers vragen
 | instappend beeld
 | judgement has passed
 | ring (wit/rood) als mr. evidence calling
 | na de komma als uitleg, buiten lopend reciterende
@@ -180,16 +182,16 @@
 | twee eieren (gemeente huis en buiging naar west)
 | vreedevernoeming
 | duiding
 | coding
 """
 
 
-from random import SystemRandom
+__author__ = "Bart Thate <libbotx@gmail.com>"
+__version__ = 1
 
 
-rand = SystemRandom()
+import random
 
 
 def wsd(event):
-    "show wisdom."
-    event.reply(rand.choice(__doc__.split("\n")).strip()[2:])
+    event.reply(random.choice(__doc__.split("\n")).strip()[2:])
```

### Comparing `libop-30/op/object.py` & `libop-5/op/objects.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,166 @@
 # This file is placed in the Public Domain.
+#
+# pylint: disable=C,R,E0603,E0402,W0401,W0614,W0611,W0622,W0105
 
 
-"clean namespace"
+"a clean namespace"
 
 
+import datetime
 import json
 import os
-import pathlib
-import _thread
+import sys
+import types
 
 
-lock = _thread.allocate_lock()
+def __dir__():
+    return (
+            'Object',
+            'construct',
+            'dump',
+            'dumps',
+            'edit',
+            'fmt',
+            'fqn',
+            'ident',
+            'items',
+            'keys',
+            'load',
+            'loads',
+            'name',
+            'update',
+            'values',
+           )
+
 
+__all__ = __dir__()
 
-class Object: # pylint: disable=R0902
 
-    "Object"
+class Object:
+
 
     def __contains__(self, key):
         return key in dir(self)
 
     def __iter__(self):
         return iter(self.__dict__)
 
     def __len__(self):
         return len(self.__dict__)
 
+    def __repr__(self):
+        return dumps(self)
+
     def __str__(self):
         return str(self.__dict__)
 
 
-def construct(obj, *args, **kwargs):
-    "construct an object from provided arguments."
+"decoder"
+
+
+class ObjectDecoder(json.JSONDecoder):
+
+    def decode(self, s, _w=None):
+        val = json.JSONDecoder.decode(self, s)
+        if not val:
+            val = {}
+        return hook(val)
+
+    def raw_decode(self, s, idx=0):
+        return json.JSONDecoder.raw_decode(self, s, idx)
+
+
+def hook(objdict, typ=None) -> Object:
+    if typ:
+        obj = typ()
+    else:
+        obj = Object()
+    construct(obj, objdict)
+    return obj
+
+
+def load(fpt, *args, **kw) -> Object:
+    kw["cls"] = ObjectDecoder
+    kw["object_hook"] = hook
+    return json.load(fpt, *args, **kw)
+
+
+def loads(string, *args, **kw) -> Object:
+    kw["cls"] = ObjectDecoder
+    kw["object_hook"] = hook
+    return json.loads(string, *args, **kw)
+
+
+"encoder"
+
+
+class ObjectEncoder(json.JSONEncoder):
+
+    def default(self, o) -> str:
+        if isinstance(o, dict):
+            return o.items()
+        if isinstance(o, Object):
+            return vars(o)
+        if isinstance(o, list):
+            return iter(o)
+        if isinstance(
+                      o,
+                      (
+                       type(str),
+                       type(True),
+                       type(False),
+                       type(int),
+                       type(float)
+                      )
+                     ):
+            return o
+        try:
+            return json.JSONEncoder.default(self, o)
+        except TypeError:
+            return object.__repr__(o)
+
+    def encode(self, o) -> str:
+        return json.JSONEncoder.encode(self, o)
+
+    def iterencode(
+                   self,
+                   o,
+                   _one_shot=False
+                  ) -> str:
+        return json.JSONEncoder.iterencode(self, o, _one_shot)
+
+
+def dump(*args, **kw) -> None:
+    kw["cls"] = ObjectEncoder
+    return json.dump(*args, **kw)
+
+
+def dumps(*args, **kw) -> str:
+    kw["cls"] = ObjectEncoder
+    return json.dumps(*args, **kw)
+
+
+"methods"
+
+
+def construct(obj, *args, **kwargs) -> None:
     if args:
         val = args[0]
         if isinstance(val, zip):
             update(obj, dict(val))
         elif isinstance(val, dict):
             update(obj, val)
         elif isinstance(val, Object):
             update(obj, vars(val))
     if kwargs:
         update(obj, kwargs)
 
 
-def edit(obj, setter, skip=False):
-    "edit an object from provided dict/dict-like."
+def edit(obj, setter, skip=False) -> None:
     for key, val in items(setter):
         if skip and val == "":
             continue
         try:
             setattr(obj, key, int(val))
             continue
         except ValueError:
@@ -63,16 +174,15 @@
             setattr(obj, key, True)
         elif val in ["False", "false"]:
             setattr(obj, key, False)
         else:
             setattr(obj, key, val)
 
 
-def fmt(obj, args=None, skip=None, plain=False):
-    "format an object to a printable string."
+def fmt(obj, args=None, skip=None, plain=False) -> str:
     if args is None:
         args = keys(obj)
     if skip is None:
         skip = []
     txt = ""
     for key in args:
         if key.startswith("__"):
@@ -83,190 +193,60 @@
         if value is None:
             continue
         if plain:
             txt += f"{value} "
         elif isinstance(value, str) and len(value.split()) >= 2:
             txt += f'{key}="{value}" '
         else:
-            txt += f"{key}={value} "
+            txt += f'{key}={value} '
     return txt.strip()
 
 
-def fqn(obj):
-    "return full qualified name of an object."
+def fqn(obj) -> str:
     kin = str(type(obj)).split()[-1][1:-2]
     if kin == "type":
         kin = obj.__name__
     return kin
 
 
-def items(obj):
-    "return the items of an object."
+def ident(obj) -> str:
+    return os.path.join(
+                        fqn(obj),
+                        os.path.join(*str(datetime.datetime.now()).split())
+                       )
+
+def items(obj) -> []:
     if isinstance(obj, type({})):
         return obj.items()
     return obj.__dict__.items()
 
 
-def keys(obj):
-    "return keys of an object."
+def keys(obj) -> []:
     if isinstance(obj, type({})):
         return obj.keys()
     return list(obj.__dict__.keys())
 
 
-def read(obj, pth):
-    "read an object from file path."
-    with lock:
-        with open(pth, 'r', encoding='utf-8') as ofile:
-            update(obj, load(ofile))
-
-
-def search(obj, selector):
-    "check if object matches provided values."
-    res = False
-    if not selector:
-        return True
-    for key, value in items(selector):
-        val = getattr(obj, key, None)
-        if str(value).lower() in str(val).lower():
-            res = True
-        else:
-            res = False
-            break
-    return res
+def name(obj) -> str:
+    typ = type(obj)
+    if isinstance(typ, types.ModuleType):
+        return obj.__name__
+    if '__self__' in dir(obj):
+        return f'{obj.__self__.__class__.__name__}.{obj.__name__}'
+    if '__class__' in dir(obj) and '__name__' in dir(obj):
+        return f'{obj.__class__.__name__}.{obj.__name__}'
+    if '__class__' in dir(obj):
+        return f"{obj.__class__.__module__}.{obj.__class__.__name__}"
+    if '__name__' in dir(obj):
+        return f'{obj.__class__.__name__}.{obj.__name__}'
+    return None
 
 
-def update(obj, data, empty=True):
-    "update an object."
+def update(obj, data, empty=True) -> None:
     for key, value in items(data):
         if empty and not value:
             continue
         setattr(obj, key, value)
 
 
-def values(obj):
-    "return values of an object."
+def values(obj) -> []:
     return obj.__dict__.values()
-
-
-def write(obj, pth):
-    "write an object to disk."
-    with lock:
-        cdir(os.path.dirname(pth))
-        with open(pth, 'w', encoding='utf-8') as ofile:
-            dump(obj, ofile, indent=4)
-
-
-class ObjectDecoder(json.JSONDecoder):
-
-    "ObjectDecoder"
-
-    def __init__(self, *args, **kwargs):
-        json.JSONDecoder.__init__(self, *args, **kwargs)
-
-    def decode(self, s, _w=None):
-        "decoding string to object."
-        val = json.JSONDecoder.decode(self, s)
-        if not val:
-            val = {}
-        return hook(val)
-
-    def raw_decode(self, s, idx=0):
-        "decode partial string to object."
-        return json.JSONDecoder.raw_decode(self, s, idx)
-
-
-def hook(objdict, typ=None):
-    "construct object from dict."
-    if typ:
-        obj = typ()
-    else:
-        obj = Object()
-    construct(obj, objdict)
-    return obj
-
-
-def load(fpt, *args, **kw):
-    "load object from file."
-    kw["cls"] = ObjectDecoder
-    kw["object_hook"] = hook
-    return json.load(fpt, *args, **kw)
-
-
-def loads(string, *args, **kw):
-    "load object from string."
-    kw["cls"] = ObjectDecoder
-    kw["object_hook"] = hook
-    return json.loads(string, *args, **kw)
-
-
-class ObjectEncoder(json.JSONEncoder):
-
-    "ObjectEncoder"
-
-    def __init__(self, *args, **kwargs):
-        json.JSONEncoder.__init__(self, *args, **kwargs)
-
-    def default(self, o):
-        "return stringable value."
-        if isinstance(o, dict):
-            return o.items()
-        if isinstance(o, Object):
-            return vars(o)
-        if isinstance(o, list):
-            return iter(o)
-        if isinstance(o, (type(str), type(True), type(False), type(int), type(float))):
-            return o
-        try:
-            return json.JSONEncoder.default(self, o)
-        except TypeError:
-            return o.__dict__
-
-    def encode(self, o) -> str:
-        "encode object to string."
-        return json.JSONEncoder.encode(self, o)
-
-    def iterencode(self, o, _one_shot=False):
-        "loop over object to encode to string."
-        return json.JSONEncoder.iterencode(self, o, _one_shot)
-
-
-def dump(*args, **kw):
-    "dump object to file."
-    kw["cls"] = ObjectEncoder
-    return json.dump(*args, **kw)
-
-
-def dumps(*args, **kw):
-    "dump object to string."
-    kw["cls"] = ObjectEncoder
-    return json.dumps(*args, **kw)
-
-
-def cdir(pth):
-    "create directory."
-    if os.path.exists(pth):
-        return
-    pth = pathlib.Path(pth)
-    os.makedirs(pth, exist_ok=True)
-
-
-def __dir__():
-    return (
-        'Object',
-        'construct',
-        'dump',
-        'dumps',
-        'edit',
-        'fmt',
-        'fqn',
-        'hook',
-        'items',
-        'keys',
-        'load',
-        'loads',
-        'read',
-        'search',
-        'update',
-        'values',
-        'write'
-    )
```

### Comparing `libop-30/pyproject.toml` & `libop-5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,52 @@
 [build-system]
 requires = [
     "setuptools>=43.0.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
+
 [project]
 name = "libop"
 description = "original programmer"
-version = "30"
+version = "5"
 authors = [
-    {name = "Bart Thate",email = "bthate@dds.nl"},
+    {name = "Bart Thate",email = "libbotx@gmail.com"},
 ]
 readme = "README.rst"
 license = {text="Public Domain"}
 classifiers = [ 
     'Development Status :: 3 - Alpha',
     'License :: Public Domain',
     'Operating System :: Unix',
     'Programming Language :: Python',
     'Topic :: Utilities'
 ]
 
+
 [project.urls]
 "home" = "https://pypi.org/project/libop"
-"bugs" = "https://github.com/xobjectz/libop/issues"
-"source" = "https://github.com/xobjectz/libop"
+"bugs" = "https://github.com/botlibx/libop/issues"
+"source" = "https://github.com/botlibx/libop"
 
 
 [tool.setuptools]
-script-files = [
-    'bin/op',
-]
 packages = [
-    "op",
-    "op.mod",
-    "op.run"
+    'op',
+    'op.mods'
 ]
 zip-safe=true
 
 
 [tool.setuptools.data-files]
 "share/doc/libop" = [
-    "README.rst"
+    "README.rst",
 ]
+
+
+[tool.setuptools.exclude-package-data]
+"*" = [
+       "env*",
+       "html*",
+       "test*"
+      ]
```


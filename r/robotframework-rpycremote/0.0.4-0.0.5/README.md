# Comparing `tmp/robotframework_rpycremote-0.0.4.tar.gz` & `tmp/robotframework_rpycremote-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_rpycremote-0.0.4.tar", last modified: Sat Apr 27 06:30:40 2024, max compression
+gzip compressed data, was "robotframework_rpycremote-0.0.5.tar", last modified: Wed May  1 05:25:28 2024, max compression
```

## Comparing `robotframework_rpycremote-0.0.4.tar` & `robotframework_rpycremote-0.0.5.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:30:40.748729 robotframework_rpycremote-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:30:40.744729 robotframework_rpycremote-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:30:40.744729 robotframework_rpycremote-0.0.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:30:40.744729 robotframework_rpycremote-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/.github/workflows/pipeline.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-27 06:30:40.748729 robotframework_rpycremote-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:30:40.744729 robotframework_rpycremote-0.0.4/RPyCRobotRemote/
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/RPyCRobotRemote/RPyCRobotRemoteClient.py
--rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/RPyCRobotRemote/RPyCRobotRemoteServer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/RPyCRobotRemote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-27 06:30:40.000000 robotframework_rpycremote-0.0.4/RPyCRobotRemote/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:30:40.748729 robotframework_rpycremote-0.0.4/robotframework_rpycremote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-27 06:30:40.000000 robotframework_rpycremote-0.0.4/robotframework_rpycremote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-27 06:30:40.000000 robotframework_rpycremote-0.0.4/robotframework_rpycremote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 06:30:40.000000 robotframework_rpycremote-0.0.4/robotframework_rpycremote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-27 06:30:40.000000 robotframework_rpycremote-0.0.4/robotframework_rpycremote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-27 06:30:40.000000 robotframework_rpycremote-0.0.4/robotframework_rpycremote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 06:30:40.748729 robotframework_rpycremote-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 06:30:40.748729 robotframework_rpycremote-0.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/test/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/test/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/test/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-27 06:30:35.000000 robotframework_rpycremote-0.0.4/test/test.robot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:25:28.281065 robotframework_rpycremote-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:25:28.277065 robotframework_rpycremote-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:25:28.277065 robotframework_rpycremote-0.0.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-01 05:25:19.000000 robotframework_rpycremote-0.0.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-01 05:25:19.000000 robotframework_rpycremote-0.0.5/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:25:28.277065 robotframework_rpycremote-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-01 05:25:19.000000 robotframework_rpycremote-0.0.5/.github/workflows/pipeline.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-01 05:25:19.000000 robotframework_rpycremote-0.0.5/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-01 05:25:19.000000 robotframework_rpycremote-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-01 05:25:19.000000 robotframework_rpycremote-0.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-01 05:25:28.281065 robotframework_rpycremote-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-01 05:25:19.000000 robotframework_rpycremote-0.0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:25:28.281065 robotframework_rpycremote-0.0.5/RPyCRobotRemote/
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-05-01 05:25:19.000000 robotframework_rpycremote-0.0.5/RPyCRobotRemote/RPyCRobotRemoteClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7280 2024-05-01 05:25:19.000000 robotframework_rpycremote-0.0.5/RPyCRobotRemote/RPyCRobotRemoteServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-01 05:25:19.000000 robotframework_rpycremote-0.0.5/RPyCRobotRemote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-01 05:25:27.000000 robotframework_rpycremote-0.0.5/RPyCRobotRemote/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-01 05:25:19.000000 robotframework_rpycremote-0.0.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:25:28.281065 robotframework_rpycremote-0.0.5/robotframework_rpycremote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-01 05:25:28.000000 robotframework_rpycremote-0.0.5/robotframework_rpycremote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-01 05:25:28.000000 robotframework_rpycremote-0.0.5/robotframework_rpycremote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 05:25:28.000000 robotframework_rpycremote-0.0.5/robotframework_rpycremote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-01 05:25:28.000000 robotframework_rpycremote-0.0.5/robotframework_rpycremote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 05:25:28.000000 robotframework_rpycremote-0.0.5/robotframework_rpycremote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 05:25:28.281065 robotframework_rpycremote-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-01 05:25:19.000000 robotframework_rpycremote-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:25:28.281065 robotframework_rpycremote-0.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-01 05:25:19.000000 robotframework_rpycremote-0.0.5/test/Model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-01 05:25:19.000000 robotframework_rpycremote-0.0.5/test/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-01 05:25:19.000000 robotframework_rpycremote-0.0.5/test/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-01 05:25:19.000000 robotframework_rpycremote-0.0.5/test/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-01 05:25:19.000000 robotframework_rpycremote-0.0.5/test/test.robot
```

### Comparing `robotframework_rpycremote-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md` & `robotframework_rpycremote-0.0.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `robotframework_rpycremote-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md` & `robotframework_rpycremote-0.0.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `robotframework_rpycremote-0.0.4/.github/workflows/pipeline.yml` & `robotframework_rpycremote-0.0.5/.github/workflows/pipeline.yml`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,15 @@
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          pip install -U setuptools_scm setuptools pylint robotframework pyyaml rpyc
+          pip install -U setuptools_scm setuptools pylint robotframework pyyaml rpyc pydantic
       - name: Analysing the code with pylint
         run: |
           pylint --module-naming-style=any $(git ls-files '*.py')
 
   robot-framework:
     strategy:
       matrix:
@@ -65,26 +65,28 @@
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
       - name: Upgrade pip
         run: |
           python -m pip install --upgrade pip
           pip install -U setuptools_scm setuptools
-      - name: Install PyYaml
+      - name: Install dependencies
         run: |
-          pip install pyyaml
+          pip install pyyaml pydantic
       - name: Install robotframework latest
         if: ${{ matrix.robotframework-version == 'latest' }}
         run: |
           pip install -U robotframework
       - name: Install robotframework ${{ matrix.robotframework-version }}
         if: ${{ matrix.robotframework-version != 'latest' }}
         run: |
           pip install robotframework==${{ matrix.robotframework-version }}
       - name: Install RPyCRobotRemote
         run: |
           pip install -e .
       - name: Executing Robot Framework Tests
+        env:
+          PYTHONPATH: 'test'
         run: |
           python test/server.py 2>&1 &
           sleep 3
           robot test/ 2>&1
```

### Comparing `robotframework_rpycremote-0.0.4/.github/workflows/publish-to-pypi.yml` & `robotframework_rpycremote-0.0.5/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `robotframework_rpycremote-0.0.4/LICENSE.txt` & `robotframework_rpycremote-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotframework_rpycremote-0.0.4/PKG-INFO` & `robotframework_rpycremote-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-rpycremote
-Version: 0.0.4
+Version: 0.0.5
 Summary: Robot Framework Remote Library based on RPyC
 Author-email: René Lehfeld <54720674+rlehfeld@users.noreply.github.com>
 License: MIT
 Project-URL: Homepage, https://github.com/rlehfeld/robotframework-rpycremote
 Project-URL: Bug Reports, https://github.com/rlehfeld/robotframework-rpycremote/issues
 Project-URL: Source, https://github.com/rlehfeld/robotframework-rpycremote/
 Keywords: robotframework,robot-framework,rpyc
```

### Comparing `robotframework_rpycremote-0.0.4/README.rst` & `robotframework_rpycremote-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `robotframework_rpycremote-0.0.4/RPyCRobotRemote/RPyCRobotRemoteClient.py` & `robotframework_rpycremote-0.0.5/RPyCRobotRemote/RPyCRobotRemoteClient.py`

 * *Files 25% similar despite different names*

```diff
@@ -56,14 +56,30 @@
     if this:
         # pylint: disable=E1120
         return sync_request.__get__(this, func.__class__)
         # pylint: enable=E1120
     return sync_request
 
 
+class Service(rpyc.Service):
+    """Extends the simple rpyc.Service with eval and execute"""
+    __slots__ = ()
+
+    def on_connect(self, conn):
+        """called when the connection is established"""
+        super().on_connect(conn)
+        self._install(conn, conn.root)
+
+    @staticmethod
+    def _install(conn, slave):
+        """install commands from remote on the client"""
+        conn.eval = slave.eval
+        conn.execute = slave.execute
+
+
 class RPyCRobotRemoteClient:
     """
     Implements Remote Client Interface for Robot Framework based on RPyC
     """
     ROBOT_LIBRARY_SCOPE = 'GLOBAL'
 
     __slot__ = ()
@@ -103,14 +119,15 @@
                 result_format='number'
             )
         # pylint: enable=duplicate-code
 
         self._client = rpyc.connect(
             peer,
             port,
+            service=Service,
             config=config,
             ipv6=ipv6,
             keepalive=True,
         )
 
         # automatic redirect stdout + stderr from remote during
         # during handling of sync_request
@@ -134,14 +151,22 @@
             else:
                 if name.startswith('ROBOT_LIBRARY_') or callable(obj):
                     return obj
         raise AttributeError(
             f'{type(self).__name__!r} object has no attribute {name!r}'
         )
 
+    def remote_eval(self, text):
+        """evaluate arbitrary code (using ``eval``) on remote"""
+        return self._client.eval(text)
+
+    def remote_execute(self, text):
+        """execute arbitrary code (using ``exec``) on remote"""
+        self._client.execute(text)
+
     def stop_remote_server(self):
         """Stop remote server."""
         self._client.root.stop_remote_server()
         # pylint: disable=W0212
         self._client._is_connected = False
         # pylint: enable=W0212
         self._client.close()
```

### Comparing `robotframework_rpycremote-0.0.4/RPyCRobotRemote/RPyCRobotRemoteServer.py` & `robotframework_rpycremote-0.0.5/RPyCRobotRemote/RPyCRobotRemoteServer.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 import pathlib
 import logging
 import io
 import inspect
 from typing import TextIO, Optional, Union
 from robot.libraries.DateTime import convert_time
 import rpyc
+# pylint: disable=E0611
+from rpyc.lib.compat import execute
+# pylint: enable=E0611
 from rpyc.utils.server import ThreadedServer
 
 
 class RPyCRobotRemoteServer:
     """
     Implements Remote Sever Interface for Robot Framework based on RPyC
     """
@@ -49,22 +52,33 @@
         :param ipv6         If ``True``, allow IPv6 connections,
                             if ``False``, use IPv4 only connections.
         """
         class Service(rpyc.Service):
             """The root service provided"""
             def __init__(self, library):
                 super().__init__()
+                self.namespace = {}
                 self._library = library
 
             if allow_remote_stop:
                 @staticmethod
                 def stop_remote_server():
                     """stop server from remote"""
                     self.stop()
 
+            def execute(self, text):
+                """execute arbitrary code (using ``exec``)"""
+                execute(text, self.namespace)
+
+            def eval(self, text):
+                """evaluate arbitrary code (using ``eval``)"""
+                # pylint: disable=W0123
+                return eval(text, self.namespace)
+                # pylint: enable=W0123
+
             def get_keyword_names(self):
                 """return the methods which can be used as keywords"""
                 get_kw_names = getattr(
                     self._library,
                     'get_keyword_names',
                     None
                 )
```

### Comparing `robotframework_rpycremote-0.0.4/RPyCRobotRemote/__init__.py` & `robotframework_rpycremote-0.0.5/RPyCRobotRemote/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -125,7 +125,41 @@
         )
         return (name_pack, id(obj), 0)
 
     func.__code__ = get_id_pack.__code__
 
 
 patch_get_id_pack(rpyc.lib.get_id_pack)
+
+
+# work around problems with get_methods in RPyC with pydantic BaseModel
+def patch_get_methods(func):
+    """patch get_methods"""
+    def get_methods(obj_attrs, obj):
+        """introspects the given (local) object, returning a list of all of
+         its methods (going up the MRO).
+
+        :param obj: any local (not proxy) python object
+
+        :returns: a list of ``(method name, docstring)`` tuples of all the
+                  methods of the given object
+        """
+        methods = {}
+        attrs = {}
+        if isinstance(obj, type):
+            # don't forget the darn metaclass
+            mros = (
+                list(reversed(type(obj).__mro__)) + list(reversed(obj.__mro__))
+            )
+        else:
+            mros = reversed(type(obj).__mro__)
+        for basecls in mros:
+            attrs.update(basecls.__dict__)
+        for name, attr in attrs.items():
+            if name not in obj_attrs and inspect.isroutine(attr):
+                methods[name] = inspect.getdoc(attr)
+        return methods.items()
+
+    func.__code__ = get_methods.__code__
+
+
+patch_get_methods(rpyc.lib.get_methods)
```

### Comparing `robotframework_rpycremote-0.0.4/pyproject.toml` & `robotframework_rpycremote-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotframework_rpycremote-0.0.4/robotframework_rpycremote.egg-info/PKG-INFO` & `robotframework_rpycremote-0.0.5/robotframework_rpycremote.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-rpycremote
-Version: 0.0.4
+Version: 0.0.5
 Summary: Robot Framework Remote Library based on RPyC
 Author-email: René Lehfeld <54720674+rlehfeld@users.noreply.github.com>
 License: MIT
 Project-URL: Homepage, https://github.com/rlehfeld/robotframework-rpycremote
 Project-URL: Bug Reports, https://github.com/rlehfeld/robotframework-rpycremote/issues
 Project-URL: Source, https://github.com/rlehfeld/robotframework-rpycremote/
 Keywords: robotframework,robot-framework,rpyc
```

### Comparing `robotframework_rpycremote-0.0.4/robotframework_rpycremote.egg-info/SOURCES.txt` & `robotframework_rpycremote-0.0.5/robotframework_rpycremote.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,11 +12,12 @@
 RPyCRobotRemote/__init__.py
 RPyCRobotRemote/_version.py
 robotframework_rpycremote.egg-info/PKG-INFO
 robotframework_rpycremote.egg-info/SOURCES.txt
 robotframework_rpycremote.egg-info/dependency_links.txt
 robotframework_rpycremote.egg-info/requires.txt
 robotframework_rpycremote.egg-info/top_level.txt
+test/Model.py
 test/client.py
 test/provider.py
 test/server.py
 test/test.robot
```

### Comparing `robotframework_rpycremote-0.0.4/test/provider.py` & `robotframework_rpycremote-0.0.5/test/provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Sample service Provide() used for testing RPyCRobot client and server
 """
 import numbers
 from collections import namedtuple
 from robot.api.deco import keyword, not_keyword
+from Model import DummyModel
 
 
 class Region(namedtuple('Region', 'x y width height')):
     """
     namedtuple to reproduce problem in list assignment
     with robot framework
     """
@@ -92,7 +93,11 @@
     def get_question(self):
         """keyword which returns a string"""
         return "what is the airspeed velocity of an unladen swallow?"
 
     def dummy_test(self):
         """keyword which returns an object"""
         return self.Dummy()
+
+    def model_test(self, model: DummyModel):
+        """keyword which returns an object"""
+        return model.value
```

### Comparing `robotframework_rpycremote-0.0.4/test/server.py` & `robotframework_rpycremote-0.0.5/test/server.py`

 * *Files identical despite different names*

### Comparing `robotframework_rpycremote-0.0.4/test/test.robot` & `robotframework_rpycremote-0.0.5/test/test.robot`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 *** Settings ***
 Library    RPyCRobotRemote    localhost    18861    timeout=10 min    WITH NAME    RPyCTest
+Library    Model
 Library    Collections
 
 *** Test Cases ***
 Test Remote
     RPyCTest.Get Answer
     RPyCTest.Use Other Name
 
@@ -11,14 +12,25 @@
     Log    ${obj.value}
     ${ret} =    Call Method    ${obj}   method    1    ${2}    3    key=${5}
     ${ret} =    Call Method    ${obj}    __call__    1    ${2}    3    key=${None}
     ${obj.value}     Set Variable    ${5}
     Log    ${obj.value2}
     ${obj.value2}     Set Variable    ${10}
 
+Test Exec
+    RPyCTest.Remote Execute    import math
+
+Test Eval
+    ${math}    RPyCTest.Remote Eval    math
+    ${ret}    Call Method    ${math}    ceil    ${2.5}
+
+Test Model
+    ${obj}    Model.Get Model
+    ${ret}    RPyCTest.Model Test    ${obj}
+
 Test Region Scalar
     ${region}    RPyCTest.Get Region
 
 Test Region List
     ${region}    RPyCTest.Get Region
     @{region}    Set Variable    ${{tuple($region)}}
```


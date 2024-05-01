# Comparing `tmp/compas_eve-0.3.7.tar.gz` & `tmp/compas_eve-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compas_eve-0.3.7.tar", last modified: Tue Apr  2 23:01:06 2024, max compression
+gzip compressed data, was "compas_eve-0.4.0.tar", last modified: Wed May  1 06:37:23 2024, max compression
```

## Comparing `compas_eve-0.3.7.tar` & `compas_eve-0.4.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 23:01:06.255368 compas_eve-0.3.7/
--rw-rw-rw-   0        0        0      102 2024-04-02 22:58:38.000000 compas_eve-0.3.7/AUTHORS.md
--rw-rw-rw-   0        0        0     2041 2024-04-02 22:58:38.000000 compas_eve-0.3.7/CHANGELOG.md
--rw-rw-rw-   0        0        0     1102 2024-04-02 22:58:38.000000 compas_eve-0.3.7/LICENSE
--rw-rw-rw-   0        0        0      436 2024-04-02 22:58:38.000000 compas_eve-0.3.7/MANIFEST.in
--rw-rw-rw-   0        0        0     3243 2024-04-02 23:01:06.270986 compas_eve-0.3.7/PKG-INFO
--rw-rw-rw-   0        0        0     2195 2024-04-02 22:58:38.000000 compas_eve-0.3.7/README.md
--rw-rw-rw-   0        0        0      713 2024-04-02 22:58:38.000000 compas_eve-0.3.7/pyproject.toml
--rw-rw-rw-   0        0        0       35 2024-04-02 22:58:38.000000 compas_eve-0.3.7/requirements.txt
--rw-rw-rw-   0        0        0      219 2024-04-02 23:01:06.270986 compas_eve-0.3.7/setup.cfg
--rw-rw-rw-   0        0        0     2058 2024-04-02 22:58:38.000000 compas_eve-0.3.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:01:06.239766 compas_eve-0.3.7/src/
-drwxrwxrwx   0        0        0        0 2024-04-02 23:01:06.255368 compas_eve-0.3.7/src/compas_eve/
--rw-rw-rw-   0        0        0     1325 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/__init__.py
--rw-rw-rw-   0        0        0      123 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/__main__.py
--rw-rw-rw-   0        0        0     5258 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/core.py
--rw-rw-rw-   0        0        0     9313 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/event_emitter.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:01:06.255368 compas_eve-0.3.7/src/compas_eve/ghpython/
--rw-rw-rw-   0        0        0      427 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/ghpython/__init__.py
--rw-rw-rw-   0        0        0     7253 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/ghpython/background.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:01:06.255368 compas_eve-0.3.7/src/compas_eve/ghpython/components/
-drwxrwxrwx   0        0        0        0 2024-04-02 23:01:06.255368 compas_eve-0.3.7/src/compas_eve/ghpython/components/Ce_BackgroundTask/
--rw-rw-rw-   0        0        0     2359 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/ghpython/components/Ce_BackgroundTask/code.py
--rw-rw-rw-   0        0        0      492 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/ghpython/components/Ce_BackgroundTask/icon.png
--rw-rw-rw-   0        0        0     1106 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/ghpython/components/Ce_BackgroundTask/metadata.json
--rw-rw-rw-   0        0        0        0 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/ghpython/components/___init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:01:06.255368 compas_eve-0.3.7/src/compas_eve/ghpython/components/ghuser/
--rw-rw-rw-   0        0        0     2235 2024-04-02 23:01:01.000000 compas_eve-0.3.7/src/compas_eve/ghpython/components/ghuser/Ce_BackgroundTask.ghuser
-drwxrwxrwx   0        0        0        0 2024-04-02 23:01:06.255368 compas_eve-0.3.7/src/compas_eve/memory/
--rw-rw-rw-   0        0        0     3547 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/memory/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:01:06.255368 compas_eve-0.3.7/src/compas_eve/mqtt/
--rw-rw-rw-   0        0        0      504 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/mqtt/__init__.py
--rw-rw-rw-   0        0        0     5369 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/mqtt/mqtt_cli.py
--rw-rw-rw-   0        0        0     5456 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/mqtt/mqtt_paho.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:01:06.255368 compas_eve-0.3.7/src/compas_eve/mqtt/netlib/
--rw-rw-rw-   0        0        0   303104 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/mqtt/netlib/MQTTnet.dll
-drwxrwxrwx   0        0        0        0 2024-04-02 23:01:06.255368 compas_eve-0.3.7/src/compas_eve/rhino/
--rw-rw-rw-   0        0        0        0 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/rhino/__init__.py
--rw-rw-rw-   0        0        0     1756 2024-04-02 22:58:38.000000 compas_eve-0.3.7/src/compas_eve/rhino/install.py
-drwxrwxrwx   0        0        0        0 2024-04-02 23:01:06.255368 compas_eve-0.3.7/src/compas_eve.egg-info/
--rw-rw-rw-   0        0        0     3243 2024-04-02 23:01:06.000000 compas_eve-0.3.7/src/compas_eve.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1053 2024-04-02 23:01:06.000000 compas_eve-0.3.7/src/compas_eve.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 23:01:06.000000 compas_eve-0.3.7/src/compas_eve.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-02 22:58:56.000000 compas_eve-0.3.7/src/compas_eve.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       31 2024-04-02 23:01:06.000000 compas_eve-0.3.7/src/compas_eve.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-02 23:01:06.000000 compas_eve-0.3.7/src/compas_eve.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 06:37:23.449645 compas_eve-0.4.0/
+-rw-rw-rw-   0        0        0      102 2024-05-01 06:34:45.000000 compas_eve-0.4.0/AUTHORS.md
+-rw-rw-rw-   0        0        0     2660 2024-05-01 06:34:45.000000 compas_eve-0.4.0/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1102 2024-05-01 06:34:45.000000 compas_eve-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0      436 2024-05-01 06:34:45.000000 compas_eve-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3243 2024-05-01 06:37:23.449645 compas_eve-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2195 2024-05-01 06:34:45.000000 compas_eve-0.4.0/README.md
+-rw-rw-rw-   0        0        0      713 2024-05-01 06:34:45.000000 compas_eve-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       35 2024-05-01 06:34:45.000000 compas_eve-0.4.0/requirements.txt
+-rw-rw-rw-   0        0        0      219 2024-05-01 06:37:23.450188 compas_eve-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     2058 2024-05-01 06:34:45.000000 compas_eve-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 06:37:23.429862 compas_eve-0.4.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-01 06:37:23.439080 compas_eve-0.4.0/src/compas_eve/
+-rw-rw-rw-   0        0        0     1325 2024-05-01 06:34:45.000000 compas_eve-0.4.0/src/compas_eve/__init__.py
+-rw-rw-rw-   0        0        0      123 2024-05-01 06:34:45.000000 compas_eve-0.4.0/src/compas_eve/__main__.py
+-rw-rw-rw-   0        0        0     6257 2024-05-01 06:34:45.000000 compas_eve-0.4.0/src/compas_eve/core.py
+-rw-rw-rw-   0        0        0     9313 2024-05-01 06:34:45.000000 compas_eve-0.4.0/src/compas_eve/event_emitter.py
+drwxrwxrwx   0        0        0        0 2024-05-01 06:37:23.443037 compas_eve-0.4.0/src/compas_eve/ghpython/
+-rw-rw-rw-   0        0        0      427 2024-05-01 06:34:45.000000 compas_eve-0.4.0/src/compas_eve/ghpython/__init__.py
+-rw-rw-rw-   0        0        0     9911 2024-05-01 06:34:45.000000 compas_eve-0.4.0/src/compas_eve/ghpython/background.py
+drwxrwxrwx   0        0        0        0 2024-05-01 06:37:23.443579 compas_eve-0.4.0/src/compas_eve/ghpython/components/
+drwxrwxrwx   0        0        0        0 2024-05-01 06:37:23.444774 compas_eve-0.4.0/src/compas_eve/ghpython/components/Ce_BackgroundTask/
+-rw-rw-rw-   0        0        0     2359 2024-05-01 06:34:45.000000 compas_eve-0.4.0/src/compas_eve/ghpython/components/Ce_BackgroundTask/code.py
+-rw-rw-rw-   0        0        0      492 2024-05-01 06:34:45.000000 compas_eve-0.4.0/src/compas_eve/ghpython/components/Ce_BackgroundTask/icon.png
+-rw-rw-rw-   0        0        0     1106 2024-05-01 06:34:45.000000 compas_eve-0.4.0/src/compas_eve/ghpython/components/Ce_BackgroundTask/metadata.json
+-rw-rw-rw-   0        0        0        0 2024-05-01 06:34:45.000000 compas_eve-0.4.0/src/compas_eve/ghpython/components/___init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 06:37:23.445546 compas_eve-0.4.0/src/compas_eve/ghpython/components/ghuser/
+-rw-rw-rw-   0        0        0     2231 2024-05-01 06:37:17.000000 compas_eve-0.4.0/src/compas_eve/ghpython/components/ghuser/Ce_BackgroundTask.ghuser
+drwxrwxrwx   0        0        0        0 2024-05-01 06:37:23.446085 compas_eve-0.4.0/src/compas_eve/memory/
+-rw-rw-rw-   0        0        0     3547 2024-05-01 06:34:45.000000 compas_eve-0.4.0/src/compas_eve/memory/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 06:37:23.447721 compas_eve-0.4.0/src/compas_eve/mqtt/
+-rw-rw-rw-   0        0        0      504 2024-05-01 06:34:45.000000 compas_eve-0.4.0/src/compas_eve/mqtt/__init__.py
+-rw-rw-rw-   0        0        0     5254 2024-05-01 06:34:45.000000 compas_eve-0.4.0/src/compas_eve/mqtt/mqtt_cli.py
+-rw-rw-rw-   0        0        0     5313 2024-05-01 06:34:45.000000 compas_eve-0.4.0/src/compas_eve/mqtt/mqtt_paho.py
+drwxrwxrwx   0        0        0        0 2024-05-01 06:37:23.447721 compas_eve-0.4.0/src/compas_eve/mqtt/netlib/
+-rw-rw-rw-   0        0        0   303104 2024-05-01 06:34:45.000000 compas_eve-0.4.0/src/compas_eve/mqtt/netlib/MQTTnet.dll
+drwxrwxrwx   0        0        0        0 2024-05-01 06:37:23.449486 compas_eve-0.4.0/src/compas_eve/rhino/
+-rw-rw-rw-   0        0        0        0 2024-05-01 06:34:45.000000 compas_eve-0.4.0/src/compas_eve/rhino/__init__.py
+-rw-rw-rw-   0        0        0     1756 2024-05-01 06:34:45.000000 compas_eve-0.4.0/src/compas_eve/rhino/install.py
+drwxrwxrwx   0        0        0        0 2024-05-01 06:37:23.439080 compas_eve-0.4.0/src/compas_eve.egg-info/
+-rw-rw-rw-   0        0        0     3243 2024-05-01 06:37:23.000000 compas_eve-0.4.0/src/compas_eve.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1053 2024-05-01 06:37:23.000000 compas_eve-0.4.0/src/compas_eve.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 06:37:23.000000 compas_eve-0.4.0/src/compas_eve.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-01 06:35:15.000000 compas_eve-0.4.0/src/compas_eve.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       31 2024-05-01 06:37:23.000000 compas_eve-0.4.0/src/compas_eve.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-01 06:37:23.000000 compas_eve-0.4.0/src/compas_eve.egg-info/top_level.txt
```

### Comparing `compas_eve-0.3.7/CHANGELOG.md` & `compas_eve-0.4.0/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,30 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.4.0] 2024-05-01
+
+### Added
+
+* Added the option to pass arguments into the long running task of a background worker.
+* Added the option to manually control when the background worker task is set to **Done**.
+* Added dispose function to control resource deallocation in a background worker.
+
+### Changed
+
+* Set background threads in the background worker as daemon threads to prevent blocking the main thread.
+* Changed base class of `Message` from `UserDict` to `object` because in IronPython 2.7 `UserDict` is an old-style class. The behavior of dictionary-like is still preserved.
+
+### Removed
+
+
 ## [0.3.7] 2024-04-03
 
 ### Added
 
 ### Changed
 
 * Ensure calling `off()` or `unsubscribe()` does not fail if the callback is not present in the registered event callbacks.
```

### Comparing `compas_eve-0.3.7/LICENSE` & `compas_eve-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `compas_eve-0.3.7/PKG-INFO` & `compas_eve-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas_eve
-Version: 0.3.7
+Version: 0.4.0
 Summary: COMPAS Event Extensions: adds event-based communication infrastructure to the COMPAS framework.
 Home-page: https://github.com/compas-dev/compas_eve
 Author: Gonzalo Casas
 Author-email: casas@arch.ethz.ch
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `compas_eve-0.3.7/README.md` & `compas_eve-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `compas_eve-0.3.7/pyproject.toml` & `compas_eve-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `compas_eve-0.3.7/setup.py` & `compas_eve-0.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 long_description = read("README.md")
 requirements = read("requirements.txt").split("\n")
 optional_requirements = {}
 
 setup(
     name="compas_eve",
-    version="0.3.7",
+    version="0.4.0",
     description="COMPAS Event Extensions: adds event-based communication infrastructure to the COMPAS framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/compas-dev/compas_eve",
     author="Gonzalo Casas",
     author_email="casas@arch.ethz.ch",
     license="MIT license",
```

### Comparing `compas_eve-0.3.7/src/compas_eve/__init__.py` & `compas_eve-0.4.0/src/compas_eve/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import os
 
 
 __author__ = ["Gonzalo Casas"]
 __copyright__ = "Gramazio Kohler Research"
 __license__ = "MIT License"
 __email__ = "casas@arch.ethz.ch"
-__version__ = "0.3.7"
+__version__ = "0.4.0"
 
 from .event_emitter import EventEmitterMixin  # noqa: F401 needed here to avoid circular import on py2.7
 from .core import Message, Publisher, Subscriber, Transport, Topic, get_default_transport, set_default_transport
 from .memory import InMemoryTransport
 
 HERE = os.path.dirname(__file__)
 HOME = os.path.abspath(os.path.join(HERE, "../../"))
```

### Comparing `compas_eve-0.3.7/src/compas_eve/core.py` & `compas_eve-0.4.0/src/compas_eve/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-# Python 2/3 compatibility import list
-try:
-    from collections import UserDict
-except ImportError:
-    from UserDict import UserDict
+from compas.data import json_dumps
+from compas.data import json_loads
 
 DEFAULT_TRANSPORT = None
 
 
 def get_default_transport():
     """Retrieve the default transport implementation to be used system-wide.
 
@@ -57,29 +54,42 @@
     def advertise(self, topic):
         pass
 
     def unadvertise(self, topic):
         pass
 
 
-class Message(UserDict):
+class Message(object):
     """Message objects used for publishing and subscribing to/from topics.
 
     A message is fundamentally a dictionary and behaves as one."""
 
+    def __init__(self, *args, **kwargs):
+        super(Message, self).__init__()
+        self.data = {}
+        self.data.update(*args, **kwargs)
+
+    def ToString(self):
+        return str(self)
+
     def __str__(self):
         return str(self.data)
 
     def __getattr__(self, name):
-        return self.__dict__["data"][name]
+        return self.data[name]
+
+    def __getitem__(self, key):
+        return self.data[key]
+
+    def __setitem__(self, key, value):
+        self.data[key] = value
 
     @classmethod
     def parse(cls, value):
-        instance = cls()
-        instance.update(value)
+        instance = cls(**value)
         return instance
 
 
 class Topic(object):
     """A topic is like a mailbox where messages can be sent and received.
 
     Topics are described by a name, a type of message they accept, and a
@@ -99,14 +109,34 @@
     # TODO: Add documentation/examples of possible options
 
     def __init__(self, name, message_type, **options):
         self.name = name
         self.message_type = message_type
         self.options = options
 
+    def _message_to_json(self, message):
+        """Convert a message to a JSON string.
+
+        Normally, this method expects sub-classes of ``Message`` as input.
+        However, it can deal with regular dictionaries as well as classes
+        implementing the COMPAS data framework.
+        """
+        try:
+            data = message.data
+        except (KeyError, AttributeError):
+            try:
+                data = message.__data__
+            except (KeyError, AttributeError):
+                data = dict(message)
+        return json_dumps(data)
+
+    def _message_from_json(self, json_message):
+        """Converts a JSON string back into a message instance."""
+        return self.message_type.parse(json_loads(json_message))
+
 
 class Publisher(object):
     """Publisher interface."""
 
     def __init__(self, topic, transport=None):
         self.topic = topic
         self.transport = transport or get_default_transport()
```

### Comparing `compas_eve-0.3.7/src/compas_eve/event_emitter.py` & `compas_eve-0.4.0/src/compas_eve/event_emitter.py`

 * *Files identical despite different names*

### Comparing `compas_eve-0.3.7/src/compas_eve/ghpython/background.py` & `compas_eve-0.4.0/src/compas_eve/ghpython/background.py`

 * *Files 18% similar despite different names*

```diff
@@ -50,24 +50,35 @@
 
     Parameters
     ----------
     ghenv : ``GhPython.Component.PythonEnvironment``
         Grasshopper environment object
     long_running_function : function, optional
         This function will be the main entry point for the long-running task.
+    dispose_function : function, optional
+        If defined, this function will be called when the worker is disposed. It can be used for clean-up tasks
+        and resource deallocation.
+    auto_set_done : bool, optional
+        If true, the worker state will be automatically set to ``Done`` after the function returns.
+        Defaults to ``True``.
+    args : tuple, optional
+        List or tuple of arguments for the invocation of the ``long_running_function``. Defaults to ``()``.
     """
 
-    def __init__(self, ghenv, long_running_function=None):
+    def __init__(self, ghenv, long_running_function=None, dispose_function=None, auto_set_done=True, args=()):
         super(BackgroundWorker, self).__init__()
         self.ghenv = ghenv
         self._is_working = False
         self._is_done = False
         self._is_cancelled = False
         self._has_requested_cancellation = False
         self.long_running_function = long_running_function
+        self.dispose_function = dispose_function
+        self.auto_set_done = auto_set_done
+        self.args = args
 
     def is_working(self):
         """Indicate whether the worker is currently working or not."""
         return self._is_working
 
     def is_done(self):
         """Indicate whether the worker is done or not."""
@@ -82,25 +93,45 @@
 
     def start_work(self):
         """Start the background processing thread where work will be performed."""
 
         def _long_running_task_wrapper(worker):
             try:
                 worker.set_internal_state_to_working()
-                result = self.long_running_function(self)
-                worker.set_internal_state_to_done(result)
+                result = self.long_running_function(self, *self.args)
+
+                # There are (at least) two types of long running functions:
+                # 1. Those that block the thread while working
+                #    (e.g. they have a busy-wait or some kind of `while` loop)
+                # 2. Those that hookup event handlers and return immediately
+                #    so then they don't need to block the thread.
+                # The first case means that we can set the state to "DONE"
+                # right after calling the function because if it returned, it really
+                # means it's done.
+                # The second case will return immediately, and setting the state to "DONE"
+                # would be wrong because the handlers are still going to trigger.
+                # In that case we can set the flag `auto_set_done` to `False` so that
+                # we don't automatically set the state to "DONE".
+                if self.auto_set_done:
+                    worker.set_internal_state_to_done(result)
             except Exception as e:
                 worker.display_message(str(e))
                 worker.set_internal_state_to_cancelled()
 
         target = _long_running_task_wrapper
         args = (self,)
         self.thread = threading.Thread(target=target, args=args)
+        self.thread.daemon = True
         self.thread.start()
 
+    def dispose(self):
+        """Invoked when the worker is being disposed."""
+        if callable(self.dispose_function):
+            self.dispose_function(self)
+
     def set_internal_state_to_working(self):
         """Set the internal state to ``working``."""
         self._is_working = True
         self._is_done = False
         self._is_cancelled = False
 
     def set_internal_state_to_done(self, result):
@@ -155,46 +186,63 @@
         def ui_callback():
             self.ghenv.Component.Message = message
             self.ghenv.Component.OnDisplayExpired(True)
 
         Rhino.RhinoApp.InvokeOnUiThread(System.Action(ui_callback))
 
     @classmethod
-    def instance_by_component(cls, ghenv, long_running_function=None, force_new=False):
+    def instance_by_component(
+        cls, ghenv, long_running_function=None, dispose_function=None, auto_set_done=True, force_new=False, args=()
+    ):
         """Get the worker instance assigned to the component.
 
         This will get a persistant instance of a background worker
         for a given component. The parameter `force_new` can
         be set to `True` to request a new instance to be created.
 
         Parameters
         ----------
         ghenv : ``GhPython.Component.PythonEnvironment``
             Grasshopper environment object
         long_running_function : function, optional
             This function will be the main entry point for the long-running task.
+        dispose_function : function, optional
+            If defined, this function will be called when the worker is disposed.
+            It can be used for clean-up tasks and resource deallocation.
+        auto_set_done : bool, optional
+            If true, the worker state will be automatically set to ``Done`` after the function returns.
+            Defaults to ``True``.
         force_new : bool, optional
             Force the creation of a new background worker, by default False.
+        args : tuple, optional
+            List or tuple of arguments for the invocation of the ``long_running_function``. Defaults to ``()``.
 
         Returns
         -------
         :class:`BackgroundWorker`
             Instance of the background worker of the current component.
         """
 
         key = create_id(ghenv.Component, "background_worker")
         worker = scriptcontext.sticky.get(key)
 
         if worker and force_new:
             worker.request_cancellation()
+            worker.dispose()
             worker = None
             del scriptcontext.sticky[key]
 
         if not worker:
-            worker = cls(ghenv, long_running_function=long_running_function)
+            worker = cls(
+                ghenv,
+                long_running_function=long_running_function,
+                dispose_function=dispose_function,
+                auto_set_done=auto_set_done,
+                args=args,
+            )
             scriptcontext.sticky[key] = worker
 
         return worker
 
     @classmethod
     def stop_instance_by_component(cls, ghenv):
         """Stops the worker instance assigned to the component.
@@ -208,9 +256,10 @@
         """
 
         key = create_id(ghenv.Component, "background_worker")
         worker = scriptcontext.sticky.get(key)
 
         if worker:
             worker.request_cancellation()
+            worker.dispose()
             worker = None
             del scriptcontext.sticky[key]
```

### Comparing `compas_eve-0.3.7/src/compas_eve/ghpython/components/Ce_BackgroundTask/code.py` & `compas_eve-0.4.0/src/compas_eve/ghpython/components/Ce_BackgroundTask/code.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 Background Task component.
 
 Executes a long-running task in the background, while keeping Grasshopper reactive.
 
-COMPAS EVE v0.3.7
+COMPAS EVE v0.4.0
 """
 
 import threading
 import scriptcontext as sc
 
 from compas_eve.ghpython import BackgroundWorker
 from ghpythonlib.componentbase import executingcomponent as component
 
 
 DEBUG = False
 
 
 class BackgroundTaskComponent(component):
-    def RunScript(self, reset, task, on):
+    def RunScript(self, task, reset, on):
         if not on:
             BackgroundWorker.stop_instance_by_component(ghenv)  # noqa: F821
             return None
 
         self.worker = BackgroundWorker.instance_by_component(ghenv, task, force_new=reset)  # noqa: F821
 
         if not self.worker.is_working() and not self.worker.is_done() and reset:
```

### Comparing `compas_eve-0.3.7/src/compas_eve/ghpython/components/Ce_BackgroundTask/metadata.json` & `compas_eve-0.4.0/src/compas_eve/ghpython/components/Ce_BackgroundTask/metadata.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970238095238095%*

 * *Differences: {"'ghpython'": "{'inputParameters': {0: {'name': 'task', 'description': 'A Python function that "*

 * *               'will be executed by the background worker. The function does not need to return '*

 * *               'quickly, it can even have an infinite loop and keep running, it will not block the '*

 * *               "UI.'}, 1: {'name': 'reset', 'description': 'Resets the background worker.'}}}"}*

```diff
@@ -2,22 +2,22 @@
     "category": "COMPAS EVE",
     "description": "Launch long-running background tasks.",
     "exposure": 4,
     "ghpython": {
         "iconDisplay": 2,
         "inputParameters": [
             {
-                "description": "Resets the background worker.",
-                "name": "reset"
-            },
-            {
                 "description": "A Python function that will be executed by the background worker. The function does not need to return quickly, it can even have an infinite loop and keep running, it will not block the UI.",
                 "name": "task"
             },
             {
+                "description": "Resets the background worker.",
+                "name": "reset"
+            },
+            {
                 "description": "Turn ON or OFF the background worker.",
                 "name": "on",
                 "typeHintID": "bool"
             }
         ],
         "isAdvancedMode": true,
         "outputParameters": [
```

### Comparing `compas_eve-0.3.7/src/compas_eve/memory/__init__.py` & `compas_eve-0.4.0/src/compas_eve/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_eve-0.3.7/src/compas_eve/mqtt/mqtt_cli.py` & `compas_eve-0.4.0/src/compas_eve/mqtt/mqtt_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 # fmt: off
 from __future__ import print_function
 
 from ..core import Transport
 from ..event_emitter import EventEmitterMixin
 
-from compas.data import json_dumps
-from compas.data import json_loads
-
 import clr
-import json
 import os
 import sys
 
 lib_dir = os.path.join(os.path.dirname(__file__), "netlib")
 if lib_dir not in sys.path:
     sys.path.append(lib_dir)
 
@@ -71,34 +67,34 @@
     def on_ready(self, callback):
         if self._is_connected:
             callback()
         else:
             self.once("ready", callback)
 
     def publish(self, topic, message):
-        # TODO: can we avoid the additional cast to dict?
+        json_message = topic._message_to_json(message)
         application_message = (
             MqttApplicationMessageBuilder()
             .WithTopic(topic.name)
-            .WithPayload(json_dumps(dict(message)))
+            .WithPayload(json_message)
             .Build()
         )
 
         def _callback(**kwargs):
             self.client.PublishAsync(application_message, CancellationToken.None)
 
         self.on_ready(_callback)
 
     def subscribe(self, topic, callback):
         event_key = "event:{}".format(topic.name)
         subscribe_id = "{}:{}".format(event_key, id(callback))
 
         def _local_callback(application_message):
             payload = Encoding.UTF8.GetString(application_message.Payload)
-            msg = topic.message_type.parse(json_loads(payload))
+            msg = topic._message_from_json(payload)
             callback(msg)
 
         def _subscribe_callback(**kwargs):
             subscribe_opts = self.factory.CreateSubscribeOptionsBuilder().WithTopicFilter(lambda f: f.WithTopic(topic.name)).Build()
             self.client.ApplicationMessageReceivedAsync += self._on_message
             self.client.SubscribeAsync(subscribe_opts, self.cancellation_token)
             self.on(event_key, _local_callback)
```

### Comparing `compas_eve-0.3.7/src/compas_eve/mqtt/mqtt_paho.py` & `compas_eve-0.4.0/src/compas_eve/mqtt/mqtt_paho.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-from compas.data import json_dumps
-from compas.data import json_loads
-
 from ..core import Transport
 from ..event_emitter import EventEmitterMixin
 
 import paho.mqtt.client as mqtt
 
 
 class MqttTransport(Transport, EventEmitterMixin):
@@ -59,16 +56,15 @@
         topic : :class:`Topic`
             Instance of the topic to publish to.
         message : :class:`Message`
             Instance of the message to publish.
         """
 
         def _callback(**kwargs):
-            # TODO: can we avoid the additional cast to dict?
-            json_message = json_dumps(dict(message))
+            json_message = topic._message_to_json(message)
             self.client.publish(topic.name, json_message)
 
         self.on_ready(_callback)
 
     def subscribe(self, topic, callback):
         """Subscribe to a topic.
 
@@ -87,15 +83,15 @@
         str
             Returns an identifier of the subscription.
         """
         event_key = "event:{}".format(topic.name)
         subscribe_id = "{}:{}".format(event_key, id(callback))
 
         def _local_callback(msg):
-            msg = topic.message_type.parse(json_loads(msg.payload.decode()))
+            msg = topic._message_from_json(msg.payload.decode())
             callback(msg)
 
         def _subscribe_callback(**kwargs):
             self.client.subscribe(topic.name)
 
             # We only really need to hook up once per client
             if not self.client.on_message:
```

### Comparing `compas_eve-0.3.7/src/compas_eve/mqtt/netlib/MQTTnet.dll` & `compas_eve-0.4.0/src/compas_eve/mqtt/netlib/MQTTnet.dll`

 * *Files identical despite different names*

### Comparing `compas_eve-0.3.7/src/compas_eve/rhino/install.py` & `compas_eve-0.4.0/src/compas_eve/rhino/install.py`

 * *Files identical despite different names*

### Comparing `compas_eve-0.3.7/src/compas_eve.egg-info/PKG-INFO` & `compas_eve-0.4.0/src/compas_eve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compas-eve
-Version: 0.3.7
+Version: 0.4.0
 Summary: COMPAS Event Extensions: adds event-based communication infrastructure to the COMPAS framework.
 Home-page: https://github.com/compas-dev/compas_eve
 Author: Gonzalo Casas
 Author-email: casas@arch.ethz.ch
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `compas_eve-0.3.7/src/compas_eve.egg-info/SOURCES.txt` & `compas_eve-0.4.0/src/compas_eve.egg-info/SOURCES.txt`

 * *Files identical despite different names*


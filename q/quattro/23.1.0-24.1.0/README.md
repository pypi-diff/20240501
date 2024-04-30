# Comparing `tmp/quattro-23.1.0.tar.gz` & `tmp/quattro-24.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed Nov 29 22:31:04 2023, max compression
+gzip compressed data, last modified: Tue Apr 30 22:09:37 2024, max compression
```

## Comparing `quattro-23.1.0.tar` & `quattro-24.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      203 2023-11-29 22:31:04.000000 quattro-23.1.0/Makefile
--rw-r--r--   0        0        0    21646 2023-11-29 22:31:04.000000 quattro-23.1.0/pdm.lock
--rw-r--r--   0        0        0      489 2023-11-29 22:31:04.000000 quattro-23.1.0/tox.ini
--rw-r--r--   0        0        0     3322 2023-11-29 22:31:04.000000 quattro-23.1.0/.github/workflows/main.yml
--rw-r--r--   0        0        0     1577 2023-11-29 22:31:04.000000 quattro-23.1.0/.github/workflows/pypi-package.yml
--rw-r--r--   0        0        0      636 2023-11-29 22:31:04.000000 quattro-23.1.0/src/quattro/__init__.py
--rw-r--r--   0        0        0     6334 2023-11-29 22:31:04.000000 quattro-23.1.0/src/quattro/_gather.py
--rw-r--r--   0        0        0     7712 2023-11-29 22:31:04.000000 quattro-23.1.0/src/quattro/cancelscope.py
--rw-r--r--   0        0        0        0 2023-11-29 22:31:04.000000 quattro-23.1.0/src/quattro/py.typed
--rw-r--r--   0        0        0    10967 2023-11-29 22:31:04.000000 quattro-23.1.0/src/quattro/taskgroup.py
--rw-r--r--   0        0        0     4262 2023-11-29 22:31:04.000000 quattro-23.1.0/tests/test_deadlines.py
--rw-r--r--   0        0        0     6723 2023-11-29 22:31:04.000000 quattro-23.1.0/tests/test_fail_after.py
--rw-r--r--   0        0        0     3816 2023-11-29 22:31:04.000000 quattro-23.1.0/tests/test_gather.py
--rw-r--r--   0        0        0     5025 2023-11-29 22:31:04.000000 quattro-23.1.0/tests/test_move_on.py
--rw-r--r--   0        0        0    19089 2023-11-29 22:31:04.000000 quattro-23.1.0/tests/test_taskgroup.py
--rw-r--r--   0        0        0       20 2023-11-29 22:31:04.000000 quattro-23.1.0/.gitignore
--rw-r--r--   0        0        0     9161 2023-11-29 22:31:04.000000 quattro-23.1.0/LICENSE
--rw-r--r--   0        0        0     8980 2023-11-29 22:31:04.000000 quattro-23.1.0/README.md
--rw-r--r--   0        0        0     1692 2023-11-29 22:31:04.000000 quattro-23.1.0/pyproject.toml
--rw-r--r--   0        0        0     9308 2023-11-29 22:31:04.000000 quattro-23.1.0/PKG-INFO
+-rw-r--r--   0        0        0      203 2024-04-30 22:09:37.000000 quattro-24.1.0/Makefile
+-rw-r--r--   0        0        0    21646 2024-04-30 22:09:37.000000 quattro-24.1.0/pdm.lock
+-rw-r--r--   0        0        0      489 2024-04-30 22:09:37.000000 quattro-24.1.0/tox.ini
+-rw-r--r--   0        0        0     3322 2024-04-30 22:09:37.000000 quattro-24.1.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1577 2024-04-30 22:09:37.000000 quattro-24.1.0/.github/workflows/pypi-package.yml
+-rw-r--r--   0        0        0      636 2024-04-30 22:09:37.000000 quattro-24.1.0/src/quattro/__init__.py
+-rw-r--r--   0        0        0     6303 2024-04-30 22:09:37.000000 quattro-24.1.0/src/quattro/_gather.py
+-rw-r--r--   0        0        0     7712 2024-04-30 22:09:37.000000 quattro-24.1.0/src/quattro/cancelscope.py
+-rw-r--r--   0        0        0        0 2024-04-30 22:09:37.000000 quattro-24.1.0/src/quattro/py.typed
+-rw-r--r--   0        0        0    11066 2024-04-30 22:09:37.000000 quattro-24.1.0/src/quattro/taskgroup.py
+-rw-r--r--   0        0        0     4262 2024-04-30 22:09:37.000000 quattro-24.1.0/tests/test_deadlines.py
+-rw-r--r--   0        0        0     6723 2024-04-30 22:09:37.000000 quattro-24.1.0/tests/test_fail_after.py
+-rw-r--r--   0        0        0     3816 2024-04-30 22:09:37.000000 quattro-24.1.0/tests/test_gather.py
+-rw-r--r--   0        0        0     5025 2024-04-30 22:09:37.000000 quattro-24.1.0/tests/test_move_on.py
+-rw-r--r--   0        0        0    19743 2024-04-30 22:09:37.000000 quattro-24.1.0/tests/test_taskgroup.py
+-rw-r--r--   0        0        0       20 2024-04-30 22:09:37.000000 quattro-24.1.0/.gitignore
+-rw-r--r--   0        0        0     9161 2024-04-30 22:09:37.000000 quattro-24.1.0/LICENSE
+-rw-r--r--   0        0        0     9243 2024-04-30 22:09:37.000000 quattro-24.1.0/README.md
+-rw-r--r--   0        0        0     1892 2024-04-30 22:09:37.000000 quattro-24.1.0/pyproject.toml
+-rw-r--r--   0        0        0     9801 2024-04-30 22:09:37.000000 quattro-24.1.0/PKG-INFO
```

### Comparing `quattro-23.1.0/pdm.lock` & `quattro-24.1.0/pdm.lock`

 * *Files identical despite different names*

### Comparing `quattro-23.1.0/.github/workflows/main.yml` & `quattro-24.1.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `quattro-23.1.0/.github/workflows/pypi-package.yml` & `quattro-24.1.0/.github/workflows/pypi-package.yml`

 * *Files identical despite different names*

### Comparing `quattro-23.1.0/src/quattro/__init__.py` & `quattro-24.1.0/src/quattro/__init__.py`

 * *Files identical despite different names*

### Comparing `quattro-23.1.0/src/quattro/_gather.py` & `quattro-24.1.0/src/quattro/_gather.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,20 +206,19 @@
     (See https://docs.python.org/3/library/asyncio-task.html#asyncio.gather)
 
     .. versionadded:: 23.1.0
     """
     if not coros:
         return ()
 
-    subtasks = []
     async with TaskGroup() as tg:
-        for coro in coros:
-            subtasks.append(
-                tg.create_task(coro if not return_exceptions else _wrap_coro(coro))
-            )
+        subtasks = [
+            tg.create_task(coro if not return_exceptions else _wrap_coro(coro))
+            for coro in coros
+        ]
 
     return tuple([await f for f in subtasks])
 
 
 async def _wrap_coro(coro: Coroutine[Any, Any, _T]) -> _T | BaseException:
     """Adapt a raised exception into the return value."""
     try:
```

### Comparing `quattro-23.1.0/src/quattro/cancelscope.py` & `quattro-24.1.0/src/quattro/cancelscope.py`

 * *Files identical despite different names*

### Comparing `quattro-23.1.0/src/quattro/taskgroup.py` & `quattro-24.1.0/src/quattro/taskgroup.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,25 +165,29 @@
                 errors = self._errors
                 self._errors = []
 
                 me = ExceptionGroup("unhandled errors in a TaskGroup", errors)
                 raise me from None
 
         def create_task(
-            self, coro: Coroutine[Any, Any, R], *, context: Optional[Context] = None
+            self,
+            coro: Coroutine[Any, Any, R],
+            *,
+            name: Optional[str] = None,
+            context: Optional[Context] = None,
         ) -> "Task[R]":
             if self._exiting:
                 raise RuntimeError(f"TaskGroup {self!r} is awaiting in exit")
             if self._loop is None:
                 raise RuntimeError(f"TaskGroup {self!r} has not been entered")
             assert self._parent_task
             if context is None:
-                task = self._loop.create_task(coro)
+                task = self._loop.create_task(coro, name=name)
             else:
-                task = context.run(self._loop.create_task, coro)
+                task = context.run(self._loop.create_task, coro, name=name)
             task.add_done_callback(
                 partial(
                     self._on_task_done, loop=self._loop, parent_task=self._parent_task
                 )
             )
             self._unfinished_tasks += 1
             self._tasks.add(task)
```

### Comparing `quattro-23.1.0/tests/test_deadlines.py` & `quattro-24.1.0/tests/test_deadlines.py`

 * *Files identical despite different names*

### Comparing `quattro-23.1.0/tests/test_fail_after.py` & `quattro-24.1.0/tests/test_fail_after.py`

 * *Files identical despite different names*

### Comparing `quattro-23.1.0/tests/test_gather.py` & `quattro-24.1.0/tests/test_gather.py`

 * *Files identical despite different names*

### Comparing `quattro-23.1.0/tests/test_move_on.py` & `quattro-24.1.0/tests/test_move_on.py`

 * *Files identical despite different names*

### Comparing `quattro-23.1.0/tests/test_taskgroup.py` & `quattro-24.1.0/tests/test_taskgroup.py`

 * *Files 2% similar despite different names*

```diff
@@ -646,14 +646,39 @@
                 collect()  # For PyPy
                 assert len(g._tasks) < 5
         await asyncio.sleep(1.35)
         collect()  # For PyPy
         assert not len(g._tasks)
 
 
+async def test_taskgroup_24():
+    """TaskGroup.create_task 'name' argument attaches name to returned task."""
+
+    task_name = "foo"
+
+    async with taskgroup.TaskGroup() as g:
+        task = g.create_task(asyncio.sleep(0), name=task_name)
+
+    assert task.get_name() == task_name
+
+
+async def test_taskgroup_25():
+    """TaskGroup.create_task 'name' argument attaches name to returned task
+    when given an explicit context.
+    """
+
+    task_name = "foo"
+    context = copy_context()
+
+    async with taskgroup.TaskGroup() as g:
+        task = g.create_task(asyncio.sleep(0), name=task_name, context=context)
+
+    assert task.get_name() == task_name
+
+
 async def test_misc():
     """Test misc edge cases, for coverage."""
 
     async def error():
         1 / 0  # noqa: B018
 
     with pytest.raises(taskgroup.ExceptionGroup) as exc_info:
```

### Comparing `quattro-23.1.0/LICENSE` & `quattro-24.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quattro-23.1.0/README.md` & `quattro-24.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # **quattro**: task control for asyncio
 
 [![PyPI](https://img.shields.io/pypi/v/quattro.svg)](https://pypi.python.org/pypi/quattro)
 [![Build](https://github.com/Tinche/quattro/workflows/CI/badge.svg)](https://github.com/Tinche/quattro/actions?workflow=CI)
 [![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/Tinche/87277dd3077fb1eefebc5d4f71b4c4b7/raw/covbadge.json)](https://github.com/Tinche/quattro/actions/workflows/main.yml)
-[![Supported Python versions](https://img.shields.io/pypi/pyversions/quattro.svg)](https://github.com/Tinche/quattro)
+[![Supported Python versions](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2FTinche%2Fquattro%2Fmain%2Fpyproject.toml)](https://github.com/Tinche/quattro)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ______________________________________________________________________
 
 **quattro** is an Apache 2 licensed library, written in Python, for task control in asyncio applications.
 _quattro_ is influenced by structured concurrency concepts from the [Trio framework](https://trio.readthedocs.io/en/stable/).
 
@@ -161,14 +161,20 @@
 - when a TaskGroup child task raises an exception, all other children and the task inside the context manager are cancelled
 
 The implementation has been borrowed from the EdgeDB project.
 
 
 ## Changelog
 
+### 24.1.0 (2024-05-01)
+
+- Add Trove classifiers.
+- Add `name` keyword-only parameter to `TaskGroup.create_task`.
+  ([#8](https://github.com/Tinche/quattro/pull/8))
+
 ### 23.1.0 (2023-11-29)
 
 - Introduce `quattro.gather`.
   ([#5](https://github.com/Tinche/quattro/pull/5))
 - Add support for Python 3.12.
 - Switch to [PDM](https://pdm.fming.dev/latest/).
```

### Comparing `quattro-23.1.0/pyproject.toml` & `quattro-24.1.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 [build-system]
 requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 name = "quattro"
 authors = [{name = "Tin Tvrtkovic", email = "tinchester@gmail.com"}]
-classifiers = ["License :: OSI Approved :: Apache Software License"]
+classifiers = [
+    "License :: OSI Approved :: Apache Software License",
+    "Intended Audience :: Developers",
+    "Programming Language :: Python :: Implementation :: CPython",
+    "Programming Language :: Python :: Implementation :: PyPy",
+    "Typing :: Typed",
+]
 dynamic = ["description", "version"]
 requires-python = ">=3.9"
 dependencies = [
     "attrs",
     "exceptiongroup; python_version < '3.11'",
 ]
 readme = "README.md"
```

### Comparing `quattro-23.1.0/PKG-INFO` & `quattro-24.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,29 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: quattro
-Version: 23.1.0
+Version: 24.1.0
+Dynamic: Summary
 Author-email: Tin Tvrtkovic <tinchester@gmail.com>
 License-File: LICENSE
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Requires-Dist: attrs
 Requires-Dist: exceptiongroup; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 # **quattro**: task control for asyncio
 
 [![PyPI](https://img.shields.io/pypi/v/quattro.svg)](https://pypi.python.org/pypi/quattro)
 [![Build](https://github.com/Tinche/quattro/workflows/CI/badge.svg)](https://github.com/Tinche/quattro/actions?workflow=CI)
 [![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/Tinche/87277dd3077fb1eefebc5d4f71b4c4b7/raw/covbadge.json)](https://github.com/Tinche/quattro/actions/workflows/main.yml)
-[![Supported Python versions](https://img.shields.io/pypi/pyversions/quattro.svg)](https://github.com/Tinche/quattro)
+[![Supported Python versions](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2FTinche%2Fquattro%2Fmain%2Fpyproject.toml)](https://github.com/Tinche/quattro)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ______________________________________________________________________
 
 **quattro** is an Apache 2 licensed library, written in Python, for task control in asyncio applications.
 _quattro_ is influenced by structured concurrency concepts from the [Trio framework](https://trio.readthedocs.io/en/stable/).
 
@@ -172,14 +177,20 @@
 - when a TaskGroup child task raises an exception, all other children and the task inside the context manager are cancelled
 
 The implementation has been borrowed from the EdgeDB project.
 
 
 ## Changelog
 
+### 24.1.0 (2024-05-01)
+
+- Add Trove classifiers.
+- Add `name` keyword-only parameter to `TaskGroup.create_task`.
+  ([#8](https://github.com/Tinche/quattro/pull/8))
+
 ### 23.1.0 (2023-11-29)
 
 - Introduce `quattro.gather`.
   ([#5](https://github.com/Tinche/quattro/pull/5))
 - Add support for Python 3.12.
 - Switch to [PDM](https://pdm.fming.dev/latest/).
```


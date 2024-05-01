# Comparing `tmp/shellfish-0.4.0.tar.gz` & `tmp/shellfish-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellfish-0.4.0.tar", max compression
+gzip compressed data, was "shellfish-0.5.0.tar", max compression
```

## Comparing `shellfish-0.4.0.tar` & `shellfish-0.5.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     2300 2023-07-26 14:37:12.145796 shellfish-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1029 2023-06-15 16:25:20.011325 shellfish-0.4.0/README.md
--rw-r--r--   0        0        0      295 2023-07-20 15:55:15.334103 shellfish-0.4.0/shellfish/__about__.py
--rw-r--r--   0        0        0     1200 2023-04-21 22:10:02.240905 shellfish-0.4.0/shellfish/__init__.py
--rw-r--r--   0        0        0      483 2023-04-21 00:04:53.526032 shellfish-0.4.0/shellfish/__main__.py
--rw-r--r--   0        0        0      358 2023-04-21 00:04:53.526032 shellfish-0.4.0/shellfish/_meta.py
--rw-r--r--   0        0        0      866 2023-04-19 19:17:33.733686 shellfish-0.4.0/shellfish/_types.py
--rw-r--r--   0        0        0     3278 2023-04-19 19:17:33.734686 shellfish-0.4.0/shellfish/aios/__init__.py
--rw-r--r--   0        0        0      640 2023-04-19 19:16:52.950595 shellfish-0.4.0/shellfish/aios/_path.py
--rw-r--r--   0        0        0      538 2023-04-21 22:10:02.240905 shellfish-0.4.0/shellfish/aioshutil.py
--rw-r--r--   0        0        0     7251 2023-04-19 19:17:33.734686 shellfish-0.4.0/shellfish/batman.py
--rw-r--r--   0        0        0      295 2022-02-17 22:17:07.429546 shellfish-0.4.0/shellfish/const.py
--rw-r--r--   0        0        0       49 2022-02-04 21:32:32.211842 shellfish-0.4.0/shellfish/dev/__init__.py
--rw-r--r--   0        0        0     1439 2023-04-19 19:17:33.735685 shellfish-0.4.0/shellfish/dev/do.py
--rw-r--r--   0        0        0     3456 2023-04-19 19:17:33.735685 shellfish-0.4.0/shellfish/dev/popen_gen.py
--rw-r--r--   0        0        0     8019 2023-06-15 16:25:20.011325 shellfish-0.4.0/shellfish/dev/run_async.py
--rw-r--r--   0        0        0     4265 2023-04-11 22:29:27.086800 shellfish-0.4.0/shellfish/dotenv.py
--rw-r--r--   0        0        0      664 2023-03-31 17:46:06.868732 shellfish-0.4.0/shellfish/echo.py
--rw-r--r--   0        0        0     8039 2023-06-15 16:25:20.011325 shellfish-0.4.0/shellfish/exe.py
--rw-r--r--   0        0        0    54204 2023-06-15 16:25:20.027510 shellfish-0.4.0/shellfish/fs/__init__.py
--rw-r--r--   0        0        0    15169 2023-04-19 19:17:33.738722 shellfish-0.4.0/shellfish/fs/_async.py
--rw-r--r--   0        0        0     1534 2023-02-24 22:45:12.450622 shellfish-0.4.0/shellfish/fs/promises.py
--rw-r--r--   0        0        0     1927 2023-05-03 19:53:18.637683 shellfish-0.4.0/shellfish/libhash.py
--rw-r--r--   0        0        0       50 2023-02-09 22:42:06.315587 shellfish-0.4.0/shellfish/libsh/__init__.py
--rw-r--r--   0        0        0     3655 2023-04-19 19:17:33.739722 shellfish-0.4.0/shellfish/libsh/_dirtree.py
--rw-r--r--   0        0        0     1872 2023-04-19 19:17:33.739722 shellfish-0.4.0/shellfish/libsh/args.py
--rw-r--r--   0        0        0    10653 2023-04-19 19:17:33.739722 shellfish-0.4.0/shellfish/osfs.py
--rw-r--r--   0        0        0     7292 2023-05-23 19:01:12.699434 shellfish-0.4.0/shellfish/process.py
--rw-r--r--   0        0        0      308 2023-03-24 22:14:11.926875 shellfish-0.4.0/shellfish/psu.py
--rw-r--r--   0        0        0        0 2022-02-01 22:06:04.844951 shellfish-0.4.0/shellfish/py.typed
--rw-r--r--   0        0        0    63493 2023-07-20 15:55:15.334103 shellfish-0.4.0/shellfish/sh.py
--rw-r--r--   0        0        0     8275 2023-04-19 19:17:33.741721 shellfish-0.4.0/shellfish/sp.py
--rw-r--r--   0        0        0      228 2023-04-19 19:17:33.741721 shellfish-0.4.0/shellfish/stdio.py
--rw-r--r--   0        0        0     2617 2023-04-11 22:29:27.086800 shellfish-0.4.0/shellfish/testing.py
--rw-r--r--   0        0        0       27 2023-04-19 19:17:33.742721 shellfish-0.4.0/shellfish/tests/__init__.py
--rw-r--r--   0        0        0     3368 2023-04-21 22:10:02.240905 shellfish-0.4.0/shellfish/tests/test_fs.py
--rw-r--r--   0        0        0     2222 1970-01-01 00:00:00.000000 shellfish-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1029 2024-02-22 14:17:28.891830 shellfish-0.5.0/README.md
+-rw-r--r--   0        0        0     2322 2024-05-01 17:31:22.272070 shellfish-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      331 2024-02-22 14:17:28.891830 shellfish-0.5.0/shellfish/__about__.py
+-rw-r--r--   0        0        0     7545 2024-05-01 17:20:40.492154 shellfish-0.5.0/shellfish/__init__.py
+-rw-r--r--   0        0        0      520 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/__main__.py
+-rw-r--r--   0        0        0      395 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/_meta.py
+-rw-r--r--   0        0        0      866 2024-02-22 14:17:28.891830 shellfish-0.5.0/shellfish/_types.py
+-rw-r--r--   0        0        0     3279 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/aios/__init__.py
+-rw-r--r--   0        0        0      640 2024-02-22 14:17:28.891830 shellfish-0.5.0/shellfish/aios/_path.py
+-rw-r--r--   0        0        0      539 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/aioshutil.py
+-rw-r--r--   0        0        0     7252 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/batman.py
+-rw-r--r--   0        0        0      296 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/const.py
+-rw-r--r--   0        0        0       49 2024-02-22 14:17:28.891830 shellfish-0.5.0/shellfish/dev/__init__.py
+-rw-r--r--   0        0        0     1467 2024-04-29 21:13:24.986924 shellfish-0.5.0/shellfish/dev/do.py
+-rw-r--r--   0        0        0     3390 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/dev/popen_gen.py
+-rw-r--r--   0        0        0     8131 2024-04-29 21:13:24.986924 shellfish-0.5.0/shellfish/dev/run_async.py
+-rw-r--r--   0        0        0     4266 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/dotenv.py
+-rw-r--r--   0        0        0      681 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/echo.py
+-rw-r--r--   0        0        0     8126 2024-04-29 21:13:24.986924 shellfish-0.5.0/shellfish/exe.py
+-rw-r--r--   0        0        0    54237 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/fs/__init__.py
+-rw-r--r--   0        0        0    15170 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/fs/_async.py
+-rw-r--r--   0        0        0     1535 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/fs/promises.py
+-rw-r--r--   0        0        0     1963 2024-02-22 14:17:28.891830 shellfish-0.5.0/shellfish/libhash.py
+-rw-r--r--   0        0        0       50 2024-02-22 14:17:28.891830 shellfish-0.5.0/shellfish/libsh/__init__.py
+-rw-r--r--   0        0        0     3656 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/libsh/_dirtree.py
+-rw-r--r--   0        0        0     1872 2024-02-22 14:17:28.891830 shellfish-0.5.0/shellfish/libsh/args.py
+-rw-r--r--   0        0        0    10604 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/osfs.py
+-rw-r--r--   0        0        0     7752 2024-05-01 17:19:37.612163 shellfish-0.5.0/shellfish/process.py
+-rw-r--r--   0        0        0      344 2024-02-22 14:17:28.891830 shellfish-0.5.0/shellfish/psu.py
+-rw-r--r--   0        0        0        0 2024-02-22 14:17:28.891830 shellfish-0.5.0/shellfish/py.typed
+-rw-r--r--   0        0        0    63836 2024-05-01 17:19:37.612163 shellfish-0.5.0/shellfish/sh.py
+-rw-r--r--   0        0        0     8275 2024-02-22 14:17:28.891830 shellfish-0.5.0/shellfish/sp.py
+-rw-r--r--   0        0        0      229 2024-03-21 23:48:47.639525 shellfish-0.5.0/shellfish/stdio.py
+-rw-r--r--   0        0        0     2617 2024-02-22 14:17:28.891830 shellfish-0.5.0/shellfish/testing.py
+-rw-r--r--   0        0        0       27 2024-02-22 14:17:28.891830 shellfish-0.5.0/shellfish/tests/__init__.py
+-rw-r--r--   0        0        0     3369 2024-02-22 14:17:28.891830 shellfish-0.5.0/shellfish/tests/test_fs.py
+-rw-r--r--   0        0        0     2216 1970-01-01 00:00:00.000000 shellfish-0.5.0/PKG-INFO
```

### Comparing `shellfish-0.4.0/pyproject.toml` & `shellfish-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 [tool.poetry]
 name = "shellfish"
-version = "0.4.0"
+version = "0.5.0"
 description = "shellfish ~ shell & file-system utils"
 license = "MIT"
 authors = ["jesse <jesse@dgi.com>"]
 repository = "https://github.com/dynamic-graphics-inc/dgpy-libs"
 homepage = "https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/shellfish"
 readme = 'README.md'
 packages = [
   { include = "shellfish", from = "." },
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Typing :: Typed",
 ]
 keywords = [
   "dgpy",
   "shell",
   "fs",
   "filesystem",
   "typed",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 pydantic = ">=2.0.3"
-aiopen = "^0.5.0"
+aiopen = ">=0.5.0"
 asyncify = ">=0.9.1"
 funkify = ">=0.4.0"
-jsonbourne = ">=0.27.0"
+jsonbourne = ">=0.29.0"
 listless = ">=0.1.0"
 xtyping = ">=0.6.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.4.0"
-pytest-asyncio = "^0.21.1"
-pytest-cov = "^4.1.0"
+pytest = "^8.2.0"
+pytest-asyncio = "^0.23.6"
+pytest-cov = "^5.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
@@ -92,8 +93,7 @@
   '\(Protocol\):$',
   'if 0:',
   'if False:',
 ]
 
 [tool.ruff]
 extend = "../../pyproject.toml"
-target-version = "py37"
```

### Comparing `shellfish-0.4.0/README.md` & `shellfish-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `shellfish-0.4.0/shellfish/_types.py` & `shellfish-0.5.0/shellfish/_types.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 PopenArg = Union[str, bytes, PathLikeStrBytes]
 PopenArgv = Sequence[PopenArg]
 PopenArgs = Union[bytes, str, PopenArgv]
 PopenEnv = Mapping[str, str]
 SymlinkType = Union[Literal["dir"], Literal["file"], Literal["junction"], str]
 
 __all__ = (
+    "FsPath",
     "PathLikeBytes",
     "PathLikeStr",
     "PathLikeStrBytes",
     "PopenArg",
     "PopenArgs",
     "PopenArgv",
     "PopenEnv",
-    "FsPath",
     "SymlinkType",
 )
```

### Comparing `shellfish-0.4.0/shellfish/aios/__init__.py` & `shellfish-0.5.0/shellfish/aios/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 """aios = asyncio + os"""
+
 from __future__ import annotations
 
 import os
 
 from typing import AnyStr, AsyncIterator, Generic
 
 from asyncify import asyncify
```

### Comparing `shellfish-0.4.0/shellfish/aios/_path.py` & `shellfish-0.5.0/shellfish/aios/_path.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.4.0/shellfish/aioshutil.py` & `shellfish-0.5.0/shellfish/aioshutil.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 """aios = asyncio + shutil"""
+
 from __future__ import annotations
 
 import shutil
 
 from asyncify import asyncify
 
 __all__ = (
```

### Comparing `shellfish-0.4.0/shellfish/batman.py` & `shellfish-0.5.0/shellfish/batman.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 """batman = bat/cmd windows utils"""
+
 from __future__ import annotations
 
 import tempfile
 
 from os import fspath as _fspath, getenv as _getenv
 from pathlib import Path
 from shutil import which
```

### Comparing `shellfish-0.4.0/shellfish/dev/do.py` & `shellfish-0.5.0/shellfish/dev/do.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     cwd: Optional[FsPath]
     dryrun: bool
     env: Optional[Dict[str, str]]
     extenv: bool
     ok_code: Union[int, List[int], Tuple[int, ...], Set[int]]
     shell: bool
     tee: bool
-    timeout: Optional[int]
+    timeout: Optional[Union[float, int]]
     verbose: bool
 
 
 class Do(JsonBaseModel):
     """PRun => 'ProcessRun' for finished processes"""
 
     args: Union[List[str], Tuple[str, ...]]
@@ -32,15 +32,15 @@
     cwd: Optional[FsPath] = None
     dryrun: bool = False
     env: Optional[Dict[str, str]] = None
     extenv: bool = True
     ok_code: Union[int, List[int], Tuple[int, ...], Set[int]] = (0,)
     shell: bool = False
     tee: bool = False
-    timeout: Optional[int] = None
+    timeout: Optional[Union[float, int]] = None
     verbose: bool = False
 
     def typed_dict(self) -> DoDict:
         return {
             "args": self.args,
             "check": self.check,
             "cwd": self.cwd,
```

### Comparing `shellfish-0.4.0/shellfish/dev/popen_gen.py` & `shellfish-0.5.0/shellfish/dev/popen_gen.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,18 +55,18 @@
     if proc.stdout is not None and proc.stderr is not None:
         ti = time()
         with ThreadPoolExecutor(2) as pool:
             q_stdout: Queue[AnyStr] = Queue()
             q_stderr: Queue[AnyStr] = Queue()
             _block = True
             stdout_future = pool.submit(
-                _enqueue_output_iter_readline, proc.stdout, q_stdout, _block  # type: ignore[arg-type]
+                _enqueue_output_iter_readline, proc.stdout, q_stdout, _block
             )
             stderr_future = pool.submit(
-                _enqueue_output_iter_readline, proc.stderr, q_stderr, _block  # type: ignore[arg-type]
+                _enqueue_output_iter_readline, proc.stderr, q_stderr, _block
             )
             while proc.poll() is None:
                 try:
                     yield Stdio.stdout, q_stdout.get_nowait()
                 except Empty:
                     pass
                 try:
@@ -96,11 +96,9 @@
 
     Yields:
         Tuple[str, str]: Tuples that are of the form ('stdout', stdout_line)
             or ('stderr', stderr_line) for the stdout and stderr lines for
             the subprocess created.
 
     """
-    with Popen(
-        *popenargs, **popenkwargs, stdout=PIPE, stderr=PIPE, text=True
-    ) as proc:  # type: ignore[call-overload]
+    with Popen(*popenargs, **popenkwargs, stdout=PIPE, stderr=PIPE, text=True) as proc:  # type: ignore[call-overload]
         yield from popen_pipes_gen(proc)
```

### Comparing `shellfish-0.4.0/shellfish/dev/run_async.py` & `shellfish-0.5.0/shellfish/dev/run_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,33 +134,34 @@
                     asyncio.gather(
                         *_bg,
                     ),
                     timeout=timeout,
                 )
                 tf = time()
             except ValueError as ve:
-                tf = time()
+                for task in _bg:
+                    task.cancel()
                 _proc.terminate()
                 raise TimeoutExpired(
                     cmd=_args,
                     timeout=timeout,
                     output=_out_buf.getvalue(),
                     stderr=_err_buf.getvalue(),
                 ) from ve
             except TimeoutError as te:
-                tf = time()
                 for task in _bg:
                     task.cancel()
-                _proc.terminate()
                 raise TimeoutExpired(
                     cmd=_args,
                     timeout=timeout,
                     output=_out_buf.getvalue(),
                     stderr=_err_buf.getvalue(),
                 ) from te
+            finally:
+                await _proc.wait()
         else:
             await asyncio.gather(
                 *_bg,
             )
             tf = time()
     else:
         if timeout:
@@ -173,24 +174,25 @@
                         timeout=timeout,
                     )
                 else:
                     (_stdout, _stderr) = await asyncio.wait_for(
                         _proc.communicate(),  # wait for subprocess to finish
                         timeout=timeout,
                     )
-
                 tf = time()
-            except TimeoutError as te:
+            except (TimeoutError, asyncio.TimeoutError) as te:
                 _proc.terminate()
                 raise TimeoutExpired(
                     cmd=_args,
                     timeout=timeout,
                     output=_out_buf.getvalue(),
                     stderr=_err_buf.getvalue(),
                 ) from te
+            finally:
+                await _proc.wait()
         else:
             (_stdout, _stderr) = await _proc.communicate(input=_input_bytes)
             tf = time()
     if tee:
         _stdout = _out_buf.getvalue()
         _stderr = _err_buf.getvalue()
     if universal_newlines:
```

### Comparing `shellfish-0.4.0/shellfish/dotenv.py` & `shellfish-0.5.0/shellfish/dotenv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 """dot.env utils"""
+
 from __future__ import annotations
 
 import re
 
 from os import getcwd, path
 from shlex import split as shplit
```

### Comparing `shellfish-0.4.0/shellfish/echo.py` & `shellfish-0.5.0/shellfish/echo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # -*- coding: utf-8 -*-
 """Echo/Print"""
+
+from __future__ import annotations
+
 from typing import IO, Any, Optional
 
 __all__ = ("echo",)
 
 
 def echo(
     *objects: Any,
@@ -22,8 +25,8 @@
         flush: Flush the file after writing
 
     Examples:
         >>> echo("shellfish")
         shellfish
 
     """
-    print(*objects, sep=sep, end=end, file=file, flush=flush)  # ruff: noqa: T201
+    print(*objects, sep=sep, end=end, file=file, flush=flush)
```

### Comparing `shellfish-0.4.0/shellfish/exe.py` & `shellfish-0.5.0/shellfish/exe.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 """Exes/commands"""
+
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from shlex import split as _shplit
 from typing import Any, Dict, List, Optional, Set, Tuple, Type, TypeVar, Union
 
 from shellfish import sh
@@ -24,43 +25,43 @@
     cmd: str
     subcmd: Optional[Tuple[str, ...]] = None
     abspath: Optional[str] = None
     env: Optional[Dict[str, str]] = None
     cwd: Optional[str] = None
     shell: bool = False
     verbose: bool = False
-    timeout: Optional[int] = None
+    timeout: Optional[Union[float, int]] = None
     ok_code: Union[int, Set[int]] = field(default_factory=lambda: {0})
     check: bool = False
 
 
 class ExeABC:
     cmd: str
     subcmd: Optional[Tuple[str, ...]] = None
 
     abspath: Optional[str] = None
     env: Optional[Dict[str, str]] = None
     cwd: Optional[FsPath] = None
     shell: bool = False
     verbose: bool = False
-    timeout: Optional[int] = None
+    timeout: Optional[Union[float, int]] = None
     ok_code: Union[int, Set[int]] = 0  # List[int], Tuple[int, ...], Set[int]] = (0,)
     check: bool = False
 
     def __init__(
         self,
         cmd: str,
         subcmd: Optional[Union[Tuple[str, ...], List[str], str]] = None,
         abspath: Optional[str] = None,
         check: bool = False,
         cwd: Optional[FsPath] = None,
         env: Optional[Dict[str, str]] = None,
         ok_code: Union[int, List[int], Tuple[int, ...], Set[int]] = 0,
         shell: bool = False,
-        timeout: Optional[int] = None,
+        timeout: Optional[Union[float, int]] = None,
         verbose: bool = False,
     ):
         self.cmd = cmd
         if subcmd is not None:
             self.subcmd = (subcmd,) if isinstance(subcmd, str) else tuple(subcmd)
         self.abspath = abspath
         self.env = env
@@ -76,15 +77,14 @@
             else set(ok_code)
         )
         self.check = check
         self.__post_init__()
 
     def __post_init__(self) -> None:
         """Post-initialization"""
-        ...
 
     @classmethod
     def _from_exe_config(cls: Type[TExe], config: ExeConfig) -> TExe:
         """Return a new instance from the config"""
         return cls(
             cmd=config.cmd,
             subcmd=config.subcmd,
@@ -156,15 +156,15 @@
         env: Optional[Dict[str, str]] = None,
         extenv: bool = True,
         cwd: Optional[FsPath] = None,
         shell: bool = False,
         check: bool = False,
         verbose: bool = False,
         input: STDIN = None,
-        timeout: Optional[int] = None,
+        timeout: Optional[Union[float, int]] = None,
         ok_code: Union[int, List[int], Tuple[int, ...], Set[int]] = 0,
         dryrun: bool = False,
     ) -> Done:
         _args = self._cmdargs(popenargs, args)
         return sh.do(
             args=_args,
             env=env or self.env,
@@ -188,15 +188,15 @@
         dryrun: bool = False,
         env: Optional[Dict[str, str]] = None,
         extenv: bool = True,
         input: STDIN = None,
         loop: Optional[Any] = None,
         ok_code: Union[int, List[int], Tuple[int, ...], Set[int]] = 0,
         shell: bool = False,
-        timeout: Optional[int] = None,
+        timeout: Optional[Union[float, int]] = None,
         verbose: bool = False,
     ) -> Done:
         _args = self._cmdargs(popenargs, args)
         return await sh.do_async(
             args=_args,
             check=check,
             cwd=cwd or str(self.cwd),
@@ -224,15 +224,15 @@
         env: Optional[Dict[str, str]] = None,
         extenv: bool = True,
         cwd: Optional[FsPath] = None,
         shell: bool = False,
         check: bool = False,
         verbose: bool = False,
         input: STDIN = None,
-        timeout: Optional[int] = None,
+        timeout: Optional[Union[float, int]] = None,
         ok_code: Union[int, List[int], Tuple[int, ...], Set[int]] = 0,
         dryrun: bool = False,
     ) -> Done:
         return self._do(
             *popenargs,
             args=args,
             check=check,
@@ -257,15 +257,15 @@
         cwd: Optional[str] = None,
         dryrun: bool = False,
         env: Optional[Dict[str, str]] = None,
         extenv: bool = True,
         input: STDIN = None,
         loop: Optional[Any] = None,
         shell: bool = False,
-        timeout: Optional[int] = None,
+        timeout: Optional[Union[float, int]] = None,
         verbose: bool = False,
     ) -> Done:
         return await self._do_async(
             *popenargs,
             args=args,
             check=check,
             cwd=cwd,
```

### Comparing `shellfish-0.4.0/shellfish/fs/__init__.py` & `shellfish-0.5.0/shellfish/fs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 """file-system utils"""
+
 from __future__ import annotations
 
 from glob import has_magic, iglob
 from itertools import chain, count
 from os import (
     DirEntry,
     chmod as _chmod,
@@ -844,17 +845,19 @@
         >>> rmtree(tmpdir)
 
     """
     dirpath = str(dirpath)
     if check and not isdir(dirpath):
         raise NotADirectoryError(dirpath)
     return (
-        str(path_string)
-        if abspath
-        else str(path_string).replace(dirpath, "").strip(sep)
+        (
+            str(path_string)
+            if abspath
+            else str(path_string).replace(dirpath, "").strip(sep)
+        )
         for path_string in chain.from_iterable(
             (
                 pwd,
                 *(path.join(pwd, _file) for _file in files),
             )
             for pwd, dirs, files in walk(
                 dirpath,
```

### Comparing `shellfish-0.4.0/shellfish/fs/_async.py` & `shellfish-0.5.0/shellfish/fs/_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 """async file-system utils"""
+
 from __future__ import annotations
 
 import os
 
 from os import fspath as _fspath
 from typing import Any, AsyncIterable, Callable, List, Optional
```

### Comparing `shellfish-0.4.0/shellfish/fs/promises.py` & `shellfish-0.5.0/shellfish/fs/promises.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 """shellfish.fs.promises"""
+
 from __future__ import annotations
 
 from shellfish.fs._async import (
     dir_exists_async as dir_exists,
     exists_async as exists,
     file_exists_async as file_exists,
     is_dir_async as is_dir,
```

### Comparing `shellfish-0.4.0/shellfish/libhash.py` & `shellfish-0.5.0/shellfish/libhash.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from __future__ import annotations
+
 from dataclasses import dataclass
 from hashlib import blake2b, blake2s, md5, sha1, sha224, sha256, sha384, sha512
 from typing import TYPE_CHECKING, Callable, Dict, Iterator, Union
 
 if TYPE_CHECKING:
     from hashlib import _Hash
 
-__all__ = ("string2hasher", "hash_bytes_gen")
+__all__ = ("hash_bytes_gen", "string2hasher")
 
 _HASHERS: Dict[str, Callable[[], "_Hash"]] = {
     "blake2b": blake2b,
     "blake2s": blake2s,
     "md5": md5,
     "sha1": sha1,
     "sha224": sha224,
```

### Comparing `shellfish-0.4.0/shellfish/libsh/_dirtree.py` & `shellfish-0.5.0/shellfish/libsh/_dirtree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 """Directory tree"""
+
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Callable, Iterator, Optional, Union
 
 
 class _DirTree:
```

### Comparing `shellfish-0.4.0/shellfish/libsh/args.py` & `shellfish-0.5.0/shellfish/libsh/args.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.4.0/shellfish/osfs.py` & `shellfish-0.5.0/shellfish/osfs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,64 +1,59 @@
 # -*- coding: utf-8 -*-
 """Os specific filesystem utils/operations"""
+
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from os import makedirs, path, symlink, unlink
 
 from shellfish import batman
 from xtyping import IterableStr, List, Tuple
 
 
 class OsFsAbc(ABC):  # pragma: nocov
     """Abstract base class for OS-specific fns"""
 
     @staticmethod
     @abstractmethod
-    def link_dir(linkpath: str, targetpath: str, *, exist_ok: bool = False) -> None:
-        ...
+    def link_dir(linkpath: str, targetpath: str, *, exist_ok: bool = False) -> None: ...
 
     @staticmethod
     @abstractmethod
     def link_dirs(
         link_target_tuples: List[Tuple[str, str]], *, exist_ok: bool = False
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @staticmethod
     @abstractmethod
-    def link_file(linkpath: str, targetpath: str, *, exist_ok: bool = False) -> None:
-        ...
+    def link_file(
+        linkpath: str, targetpath: str, *, exist_ok: bool = False
+    ) -> None: ...
 
     @staticmethod
     @abstractmethod
     def link_files(
         link_target_tuples: List[Tuple[str, str]], *, exist_ok: bool = False
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @staticmethod
     @abstractmethod
-    def unlink_dir(link: str) -> None:
-        ...
+    def unlink_dir(link: str) -> None: ...
 
     @staticmethod
     @abstractmethod
-    def unlink_dirs(links: IterableStr) -> None:
-        ...
+    def unlink_dirs(links: IterableStr) -> None: ...
 
     @staticmethod
     @abstractmethod
-    def unlink_file(link: str) -> None:
-        ...
+    def unlink_file(link: str) -> None: ...
 
     @staticmethod
     @abstractmethod
-    def unlink_files(links: IterableStr) -> None:
-        ...
+    def unlink_files(links: IterableStr) -> None: ...
 
 
 # =============================================================================
 # /\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/\/
 # =============================================================================
 #  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\  /\
 # /  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \/  \
```

### Comparing `shellfish-0.4.0/shellfish/process.py` & `shellfish-0.5.0/shellfish/process.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 """Current running process info"""
+
 from __future__ import annotations
 
 import platform
 import sys
 
 from contextlib import contextmanager
 from os import environ, name as os_name, pathsep
@@ -25,17 +26,17 @@
 
 IS_WIN = os_name == "nt"
 PYTHON_IMPLEMENTATION = platform.python_implementation()
 SYS_PATH_SEP: str = pathsep
 
 __all__ = (
     "ENV",
-    "Env",
     "PYTHON_IMPLEMENTATION",
     "SYS_PATH_SEP",
+    "Env",
     "env",
     "env_dict",
     "is_cpython",
     "is_mac",
     "is_notebook",
     "is_pypy",
     "is_win",
@@ -248,15 +249,30 @@
     """Return the current process' os type: 'mac' | 'lin' | 'win' | 'wsl'"""
     if is_win():
         return "win"
     if is_wsl():
         return "wsl"
     if is_mac():
         return "mac"
-    return "lin"
+    return linux_version()
+
+
+def linux_version() -> str:
+    """Return rhel7 or rhel8 based on the current linux version"""
+    try:
+        with open("/etc/redhat-release") as file:
+            release_info = file.read()
+            if "release 7" in release_info:
+                return "rhel7"
+            elif "release 8" in release_info:
+                return "rhel8"
+            else:
+                return "other"
+    except FileNotFoundError:
+        return "linux"
 
 
 def hostname() -> str:
     """Return the current computer's hostname
 
     Returns:
         str: hostname
```

### Comparing `shellfish-0.4.0/shellfish/sh.py` & `shellfish-0.5.0/shellfish/sh.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # -*- coding: utf-8 -*-
 """shell utils"""
+
 from __future__ import annotations
 
 import signal
 import sys
 
 from functools import lru_cache
 from os import chdir, environ, fspath as _fspath, getcwd, listdir, makedirs, path
 from pathlib import Path
 from platform import system
 from shlex import quote as _quote, split as _shplit
 from shutil import which as _which
-from subprocess import PIPE, CompletedProcess, SubprocessError, run
+from subprocess import PIPE, CompletedProcess, SubprocessError, TimeoutExpired, run
 from time import time
 from typing import (
     IO,
     Any,
     Callable,
     Dict,
     Iterable,
@@ -156,87 +157,58 @@
 from shellfish.libsh._dirtree import _DirTree
 from shellfish.osfs import LIN as _LIN, WIN as _WIN
 from shellfish.process import is_win
 from shellfish.stdio import Stdio as Stdio
 from xtyping import STDIN, AnyStr, IterableStr, TypedDict
 
 __all__ = (
+    "LIN",
+    "WIN",
     "Done",
     "DoneError",
     "DoneObj",
     "Flag",
     "FlagMeta",
     "HrTime",
-    "LIN",
-    "WIN",
-    "__version__",
-    "basename",
-    "cd",
-    "decode_stdio_bytes",
-    "dirname",
-    "do",
-    "do_",
-    "do_async",
-    "doa",
-    "echo",
-    "export",
-    "flatten_args",
-    "link_dir",
-    "link_dirs",
-    "link_file",
-    "link_files",
-    "ls",
-    "ls_dirs",
-    "ls_files",
-    "ls_files_dirs",
-    "pstderr",
-    "pstdout",
-    "pstdout_pstderr",
-    "pwd",
-    "q",
-    "quote",
-    "run",
-    "setenv",
-    "shell",
-    "shplit",
-    "shx",
-    "source",
-    "sync",
-    "tree",
-    "unlink_dir",
-    "unlink_dirs",
-    "unlink_file",
-    "unlink_files",
-    "where",
-    "which",
-    "which_lru",
-    "x",
     # fs exports
     "Stdio",
     "SymlinkType",
+    "TimeoutExpired",
+    "__version__",
+    "basename",
+    "cd",
     "chmod",
     "copy_file",
     "cp",
+    "decode_stdio_bytes",
     "dir_exists",
     "dir_exists_async",
+    "dirname",
     "dirpath_gen",
     "dirs_gen",
+    "do",
+    "do_",
+    "do_async",
+    "doa",
+    "echo",
     "exists",
     "exists_async",
+    "export",
     "extension",
     "file_exists",
     "file_exists_async",
     "file_lines_gen",
     "filecmp",
     "filepath_gen",
     "filepath_mtimedelta_sec",
     "files_dirs_gen",
     "files_gen",
     "filesize",
     "filesize_async",
+    "flatten_args",
     "fspath",
     "is_dir",
     "is_dir_async",
     "is_file",
     "is_file_async",
     "is_link",
     "is_link_async",
@@ -247,28 +219,42 @@
     "islink",
     "islink_async",
     "lbin",
     "lbytes",
     "lbytes_async",
     "lbytes_gen",
     "lbytes_gen_async",
+    "link_dir",
+    "link_dirs",
+    "link_file",
+    "link_files",
     "listdir_async",
     "listdir_gen",
     "ljson",
     "ljson_async",
+    "ls",
+    "ls_dirs",
+    "ls_files",
+    "ls_files_dirs",
     "lstat_async",
     "lstr",
     "lstr_async",
     "lstring",
     "lstring_async",
     "mkdir",
     "mkdirp",
     "move",
     "mv",
     "path_gen",
+    "pstderr",
+    "pstdout",
+    "pstdout_pstderr",
+    "pwd",
+    "q",
+    "quote",
     "rbin",
     "rbin_async",
     "rbin_gen",
     "rbin_gen_async",
     "rbytes",
     "rbytes_async",
     "rbytes_gen",
@@ -280,14 +266,15 @@
     "rm_gen",
     "rmdir",
     "rmfile",
     "rstr",
     "rstr_async",
     "rstring",
     "rstring_async",
+    "run",
     "safepath",
     "sbin",
     "sbin_async",
     "sbytes",
     "sbytes_async",
     "sbytes_gen",
     "sbytes_gen_async",
@@ -295,40 +282,55 @@
     "scandir_gen",
     "scandir_list",
     "sep_join",
     "sep_lstrip",
     "sep_rstrip",
     "sep_split",
     "sep_strip",
+    "setenv",
     "shebang",
+    "shell",
+    "shplit",
+    "shx",
     "sjson",
     "sjson_async",
+    "source",
     "sstr",
     "sstr_async",
     "sstring",
     "sstring_async",
     "stat",
     "stat_async",
     "symlink",
+    "sync",
     "touch",
+    "tree",
+    "unlink_dir",
+    "unlink_dirs",
+    "unlink_file",
+    "unlink_files",
     "walk_gen",
     "wbin",
     "wbin_async",
     "wbin_gen",
     "wbin_gen_async",
     "wbytes",
     "wbytes_async",
     "wbytes_gen",
     "wbytes_gen_async",
+    "where",
+    "which",
+    "which_lru",
     "wjson",
     "wjson_async",
     "wstr",
     "wstr_async",
     "wstring",
     "wstring_async",
+    "x",
 )
 
 IS_WIN: bool = is_win()
 
 
 class FlagMeta(type):
     """Meta class"""
@@ -350,16 +352,14 @@
         >>> Flag.__help
         '--help'
         >>> Flag._v
         '-v'
 
     """
 
-    ...
-
 
 def mkenv(env: Dict[str, str], extenv: bool = True) -> Dict[str, str]:
     if extenv:
         return {**dict(environ), **env}
     return env
 
 
@@ -670,37 +670,49 @@
         Returns:
             Done object; self
 
         """
         self.write_stderr(filepath, append=True)
         return self
 
-    def json_parse_stdout(self, jsonc: bool = False, ndjson: bool = False) -> Any:
+    def json_parse_stdout(
+        self, jsonc: bool = False, jsonl: bool = False, ndjson: bool = False
+    ) -> Any:
         """Return json parsed stdout"""
-        return JSON.loads(self.stdout, jsonc=jsonc, ndjson=ndjson)
+        return JSON.loads(self.stdout, jsonc=jsonc, jsonl=jsonl, ndjson=ndjson)
 
-    def json_parse_stderr(self, jsonc: bool = False, ndjson: bool = False) -> Any:
+    def json_parse_stderr(
+        self, jsonc: bool = False, jsonl: bool = False, ndjson: bool = False
+    ) -> Any:
         """Return json parsed stderr"""
-        return JSON.loads(self.stderr, jsonc=jsonc, ndjson=ndjson)
+        return JSON.loads(self.stderr, jsonc=jsonc, jsonl=jsonl, ndjson=ndjson)
 
     def json_parse(
-        self, stderr: bool = False, jsonc: bool = False, ndjson: bool = False
+        self,
+        stderr: bool = False,
+        jsonc: bool = False,
+        jsonl: bool = False,
+        ndjson: bool = False,
     ) -> Any:
         """Return json parsed stdout"""
         return (
-            self.json_parse_stdout(jsonc=jsonc, ndjson=ndjson)
+            self.json_parse_stdout(jsonc=jsonc, jsonl=jsonl, ndjson=ndjson)
             if not stderr
-            else self.json_parse_stderr(jsonc=jsonc, ndjson=ndjson)
+            else self.json_parse_stderr(jsonc=jsonc, jsonl=jsonl, ndjson=ndjson)
         )
 
     def parse_json(
-        self, stderr: bool = False, jsonc: bool = False, ndjson: bool = False
+        self,
+        stderr: bool = False,
+        jsonc: bool = False,
+        jsonl: bool = False,
+        ndjson: bool = False,
     ) -> Any:
         """Return json parsed stdout (alias bc I keep flip-flopping the fn name)"""
-        return self.json_parse(stderr=stderr, jsonc=jsonc, ndjson=ndjson)
+        return self.json_parse(stderr=stderr, jsonc=jsonc, jsonl=jsonl, ndjson=ndjson)
 
     def grep(self, string: str) -> List[str]:
         """Return lines in stdout that have
 
         Args:
             string (str): String to search for
 
@@ -871,15 +883,15 @@
     env: Optional[Dict[str, str]] = None,
     extenv: bool = True,
     cwd: Optional[FsPath] = None,
     shell: bool = False,
     check: bool = False,
     verbose: bool = False,
     input: STDIN = None,
-    timeout: Optional[int] = None,
+    timeout: Optional[float] = None,
     text: bool = False,
     tee: bool = False,
     ok_code: Union[int, List[int], Tuple[int, ...], Set[int]] = 0,
     dryrun: bool = False,
 ) -> Done:
     """Run a subprocess synchronously
 
@@ -986,15 +998,15 @@
     extenv: bool = True,
     cwd: Optional[FsPath] = None,
     shell: bool = False,
     check: bool = False,
     tee: bool = False,
     verbose: bool = False,
     input: STDIN = None,
-    timeout: Optional[int] = None,
+    timeout: Optional[Union[float, int]] = None,
     ok_code: Union[int, List[int], Tuple[int, ...], Set[int]] = 0,
     dryrun: bool = False,
 ) -> Done:
     """Run a subprocess synchronously
 
     Args:
         *popenargs: Args given as `*args`; Cannot use both *popenargs and args
@@ -1047,15 +1059,15 @@
     env: Optional[Dict[str, str]] = None,
     shell: bool = True,
     extenv: bool = True,
     cwd: Optional[FsPath] = None,
     check: bool = False,
     verbose: bool = False,
     input: STDIN = None,
-    timeout: Optional[int] = None,
+    timeout: Optional[Union[float, int]] = None,
     ok_code: Union[int, List[int], Tuple[int, ...], Set[int]] = 0,
     dryrun: bool = False,
 ) -> Done:
     """Run a subprocess synchronously in current shell
 
     Args:
         *popenargs: Args given as `*args`; Cannot use both *popenargs and args
@@ -1106,15 +1118,15 @@
     stdin: Optional[Union[IO[AnyStr], int]] = None,
     input: Optional[str] = None,
     stdout: Optional[Union[IO[AnyStr], int]] = None,
     stderr: Optional[Union[IO[AnyStr], int]] = None,
     capture_output: bool = False,
     shell: bool = False,
     cwd: Optional[FsPath] = None,
-    timeout: Optional[int] = None,
+    timeout: Optional[Union[float, int]] = None,
     check: bool = False,
     encoding: Optional[str] = None,
     errors: Optional[str] = None,
     text: bool = False,
     env: Optional[Dict[str, str]] = None,
     universal_newlines: bool = False,
     **other_popen_kwargs: Any,
@@ -1145,15 +1157,15 @@
     env: Optional[Dict[str, str]] = None,
     extenv: bool = True,
     cwd: Optional[str] = None,
     shell: bool = False,
     verbose: bool = False,
     input: STDIN = None,
     check: bool = False,
-    timeout: Optional[int] = None,
+    timeout: Optional[Union[float, int]] = None,
     ok_code: Union[int, List[int], Tuple[int, ...], Set[int]] = 0,
     dryrun: bool = False,
 ) -> Done:
     """Run a subprocess asynchronously using asyncified version of do"""
     done = await _do_asyncify(
         *popenargs,
         args=args,
@@ -1178,15 +1190,15 @@
     env: Optional[Dict[str, str]] = None,
     extenv: bool = True,
     cwd: Optional[str] = None,
     shell: bool = False,
     verbose: bool = False,
     input: STDIN = None,
     check: bool = False,
-    timeout: Optional[int] = None,
+    timeout: Optional[Union[float, int]] = None,
     ok_code: Union[int, List[int], Tuple[int, ...], Set[int]] = 0,
     dryrun: bool = False,
 ) -> Done:
     """Run a subprocess and await completion
 
     Args:
         args: Args as strings for the subprocess
@@ -1253,15 +1265,15 @@
         exe_path = which_lru(_args[0], path=_syspath)
         if exe_path:
             _args[0] = exe_path
 
     if dryrun:
         return Done(
             args=_args,
-            returncode=0,
+            returncode=-1,
             stdout="",
             stderr="",
             ti=0,
             tf=0,
             dt=0,
             hrdt=HrTime(
                 sec=0,
@@ -1280,21 +1292,20 @@
         ok_code=ok_code if isinstance(ok_code, (list, tuple, set)) else {ok_code},
         check=check,
         capture_output=True,
         timeout=timeout,
         input=_input,
         universal_newlines=True,
     )
-
     _args_array = (
         list(map(str, args)) if isinstance(args, (list, tuple)) else [str(args)]
     )
     return Done(
         args=_args_array,
-        returncode=_proc.returncode or -1,
+        returncode=_proc.returncode,
         stdout=decode_stdio_bytes(_proc.stdout),
         stderr=decode_stdio_bytes(_proc.stderr),
         stdin=input.decode(encoding="utf-8") if isinstance(input, bytes) else None,
         ti=_pdt.ti,
         tf=_pdt.tf,
         dt=_pdt.dt,
         hrdt=HrTime.from_seconds(
@@ -1311,15 +1322,15 @@
     env: Optional[Dict[str, str]] = None,
     extenv: bool = True,
     cwd: Optional[str] = None,
     shell: bool = False,
     verbose: bool = False,
     input: STDIN = None,
     check: bool = False,
-    timeout: Optional[int] = None,
+    timeout: Optional[float] = None,
     ok_code: Union[int, List[int], Tuple[int, ...], Set[int]] = 0,
     dryrun: bool = False,
 ) -> Done:
     """Run a subprocess and await its completion
 
     Args:
         *popenargs: Args given as `*args`; Cannot use both *popenargs and args
@@ -1388,15 +1399,15 @@
     env: Optional[Dict[str, str]] = None,
     extenv: bool = True,
     cwd: Optional[str] = None,
     shell: bool = False,
     verbose: bool = False,
     input: STDIN = None,
     check: bool = False,
-    timeout: Optional[int] = None,
+    timeout: Optional[float] = None,
     ok_code: Union[int, List[int], Tuple[int, ...], Set[int]] = 0,
     dryrun: bool = False,
 ) -> Done:
     """Run a subprocess and await its completion
 
     Alias for sh.do_async
```

### Comparing `shellfish-0.4.0/shellfish/sp.py` & `shellfish-0.5.0/shellfish/sp.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -39,24 +39,24 @@
     "CompletedProcess",
     "run",
     "Popen",
     "PIPE",
     "DEVNULL",
 )
 __all__ = (
+    "DEVNULL",
+    "PIPE",
+    # from subprocess
+    "CompletedProcess",
     "CompletedProcessDict",
+    "Popen",
     "completed_process_dict",
+    "run",
     "runb",
     "runs",
-    # from subprocess
-    "CompletedProcess",
-    "run",
-    "Popen",
-    "PIPE",
-    "DEVNULL",
 )
 
 
 @dataclass(frozen=True)
 class ProcessDt:
     """Process time delta dataclass
```

### Comparing `shellfish-0.4.0/shellfish/testing.py` & `shellfish-0.5.0/shellfish/testing.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from typing import Dict, List, Optional
 
 from shellfish.fs import wstring
 from xtyping import FsPath
 
 __all__ = (
     "assert_symlink_exists",
-    "random_string",
-    "random_directory_path",
     "mk_random_dirtree",
+    "random_directory_path",
+    "random_string",
 )
 
 
 def assert_symlink_exists(fspath: FsPath, *, target: Optional[FsPath] = None) -> bool:
     _path = Path(fspath)
     try:
         assert _path.exists()
```

### Comparing `shellfish-0.4.0/shellfish/tests/test_fs.py` & `shellfish-0.5.0/shellfish/tests/test_fs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Testing shelfish.fs"""
+
 from collections import Counter
 from os import path
 from pathlib import Path
 from typing import Callable, Iterable
 
 import pytest
```

### Comparing `shellfish-0.4.0/PKG-INFO` & `shellfish-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: shellfish
-Version: 0.4.0
+Version: 0.5.0
 Summary: shellfish ~ shell & file-system utils
 Home-page: https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/shellfish
 License: MIT
 Keywords: dgpy,shell,fs,filesystem,typed
 Author: jesse
 Author-email: jesse@dgi.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
-Requires-Dist: aiopen (>=0.5.0,<0.6.0)
+Requires-Dist: aiopen (>=0.5.0)
 Requires-Dist: asyncify (>=0.9.1)
 Requires-Dist: funkify (>=0.4.0)
-Requires-Dist: jsonbourne (>=0.27.0)
+Requires-Dist: jsonbourne (>=0.29.0)
 Requires-Dist: listless (>=0.1.0)
 Requires-Dist: pydantic (>=2.0.3)
 Requires-Dist: xtyping (>=0.6.0)
 Project-URL: Repository, https://github.com/dynamic-graphics-inc/dgpy-libs
 Description-Content-Type: text/markdown
 
 <a href="https://github.com/dynamic-graphics-inc/dgpy-libs">
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: shellfish Version: 0.4.0 Summary: shellfish ~ shell
+Metadata-Version: 2.1 Name: shellfish Version: 0.5.0 Summary: shellfish ~ shell
 & file-system utils Home-page: https://github.com/dynamic-graphics-inc/dgpy-
 libs/tree/main/libs/shellfish License: MIT Keywords:
 dgpy,shell,fs,filesystem,typed Author: jesse Author-email: jesse@dgi.com
-Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 5 - Production/
+Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Typing :: Typed Requires-Dist: aiopen (>=0.5.0,<0.6.0) Requires-Dist: asyncify
-(>=0.9.1) Requires-Dist: funkify (>=0.4.0) Requires-Dist: jsonbourne (>=0.27.0)
+:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
+Typing :: Typed Requires-Dist: aiopen (>=0.5.0) Requires-Dist: asyncify
+(>=0.9.1) Requires-Dist: funkify (>=0.4.0) Requires-Dist: jsonbourne (>=0.29.0)
 Requires-Dist: listless (>=0.1.0) Requires-Dist: pydantic (>=2.0.3) Requires-
 Dist: xtyping (>=0.6.0) Project-URL: Repository, https://github.com/dynamic-
 graphics-inc/dgpy-libs Description-Content-Type: text/markdown _[_d_r_a_w_i_n_g_]#
 shellfish [![Wheel](https://img.shields.io/pypi/wheel/shellfish.svg)](https://
 img.shields.io/pypi/wheel/shellfish.svg) [![Version](https://img.shields.io/
 pypi/v/shellfish.svg)](https://img.shields.io/pypi/v/shellfish.svg) [!
 [py_versions](https://img.shields.io/pypi/pyversions/shellfish.svg)](https://
```


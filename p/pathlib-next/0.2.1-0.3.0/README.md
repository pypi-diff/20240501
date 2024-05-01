# Comparing `tmp/pathlib_next-0.2.1.tar.gz` & `tmp/pathlib_next-0.3.0.tar.gz`

## Comparing `pathlib_next-0.2.1.tar` & `pathlib_next-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 pathlib_next-0.2.1/src/example.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 pathlib_next-0.2.1/src/pathlib_next/__init__.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 pathlib_next-0.2.1/src/pathlib_next/fspath.py
--rw-r--r--   0        0        0     5174 2020-02-02 00:00:00.000000 pathlib_next-0.2.1/src/pathlib_next/mempath.py
--rw-r--r--   0        0        0    18038 2020-02-02 00:00:00.000000 pathlib_next-0.2.1/src/pathlib_next/path.py
--rw-r--r--   0        0        0    15590 2020-02-02 00:00:00.000000 pathlib_next-0.2.1/src/pathlib_next/uri/__init__.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 pathlib_next-0.2.1/src/pathlib_next/uri/query.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 pathlib_next-0.2.1/src/pathlib_next/uri/source.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 pathlib_next-0.2.1/src/pathlib_next/uri/schemes/__init__.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 pathlib_next-0.2.1/src/pathlib_next/uri/schemes/file.py
--rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 pathlib_next-0.2.1/src/pathlib_next/uri/schemes/http.py
--rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 pathlib_next-0.2.1/src/pathlib_next/uri/schemes/sftp.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 pathlib_next-0.2.1/src/pathlib_next/utils/__init__.py
--rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 pathlib_next-0.2.1/src/pathlib_next/utils/glob.py
--rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 pathlib_next-0.2.1/src/pathlib_next/utils/stat.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 pathlib_next-0.2.1/src/pathlib_next/utils/sync.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pathlib_next-0.2.1/tests/test_local.py
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 pathlib_next-0.2.1/tests/test_uri.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pathlib_next-0.2.1/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pathlib_next-0.2.1/LICENSE
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pathlib_next-0.2.1/README.md
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 pathlib_next-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 pathlib_next-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/example.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/__init__.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/fspath.py
+-rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/mempath.py
+-rw-r--r--   0        0        0    12834 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/path.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/protocols/__init__.py
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/protocols/fs.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/protocols/io.py
+-rw-r--r--   0        0        0    15590 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/uri/__init__.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/uri/query.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/uri/source.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/uri/schemes/__init__.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/uri/schemes/file.py
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/uri/schemes/http.py
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/uri/schemes/sftp.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/utils/__init__.py
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/utils/glob.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/utils/stat.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/src/pathlib_next/utils/sync.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/tests/test_local.py
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/tests/test_uri.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/LICENSE
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/README.md
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 pathlib_next-0.3.0/PKG-INFO
```

### Comparing `pathlib_next-0.2.1/src/example.py` & `pathlib_next-0.3.0/src/example.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,14 @@
 
 
 syncer = PathSyncer(checksum, remove_missing=False)
 syncer.sync((sftp_root / "root/.ssh"), dest, dry_run=True)
 
 rocky_repo = UriPath("http://dl.rockylinux.org/pub")
 
-glob_test = UriPath("file:./**/*.py")
+glob_test = UriPath("file:src/**/*.py")
 
 for path in glob.glob(glob_test, recursive=True):
     print(path)
 
 print(rocky_repo.is_dir())
 print(list(rocky_repo.iterdir()))
```

### Comparing `pathlib_next-0.2.1/src/pathlib_next/fspath.py` & `pathlib_next-0.3.0/src/pathlib_next/fspath.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.2.1/src/pathlib_next/mempath.py` & `pathlib_next-0.3.0/src/pathlib_next/mempath.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import io
 import posixpath as _posix
 from io import IOBase
 from urllib.parse import quote as _urlquote
 
 from .path import Path, Pathname
-from .utils.stat import FileStat, FileStatLike
+from .utils.stat import FileStat
 
 
 class MemPathBackend(dict): ...
 
 
 class MemBytesIO(io.BytesIO):
-    def __init__(self, initial_bytes: bytearray) -> None:
-        self._bytes = initial_bytes
-        super().__init__(initial_bytes)
+    def __init__(self, dest: bytearray) -> None:
+        self._bytes = dest
+        super().__init__()
 
     def close(self) -> None:
         self.seek(0)
         self._bytes.clear()
         self._bytes.extend(self.read())
         return super().close()
 
@@ -133,15 +133,15 @@
             if missing_ok:
                 return
             raise FileNotFoundError(self)
         elif isinstance(content, dict):
             raise IsADirectoryError(self)
         parent.pop(name)
 
-    def stat(self, *, follow_symlinks=True) -> FileStatLike:
+    def stat(self, *, follow_symlinks=True):
         parent, name = self._parent_container()
         if not name:
             return FileStat(is_dir=True)
 
         if name not in parent:
             return FileNotFoundError(self)
```

### Comparing `pathlib_next-0.2.1/src/pathlib_next/uri/__init__.py` & `pathlib_next-0.3.0/src/pathlib_next/uri/__init__.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.2.1/src/pathlib_next/uri/query.py` & `pathlib_next-0.3.0/src/pathlib_next/uri/query.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.2.1/src/pathlib_next/uri/source.py` & `pathlib_next-0.3.0/src/pathlib_next/uri/source.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.2.1/src/pathlib_next/uri/schemes/file.py` & `pathlib_next-0.3.0/src/pathlib_next/uri/schemes/file.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.2.1/src/pathlib_next/uri/schemes/http.py` & `pathlib_next-0.3.0/src/pathlib_next/uri/schemes/http.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.2.1/src/pathlib_next/uri/schemes/sftp.py` & `pathlib_next-0.3.0/src/pathlib_next/uri/schemes/sftp.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.2.1/src/pathlib_next/utils/__init__.py` & `pathlib_next-0.3.0/src/pathlib_next/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.2.1/src/pathlib_next/utils/glob.py` & `pathlib_next-0.3.0/src/pathlib_next/utils/glob.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.2.1/src/pathlib_next/utils/stat.py` & `pathlib_next-0.3.0/src/pathlib_next/utils/stat.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,21 @@
 import abc as _abc
 import stat as _stat
 import typing as _ty
 
 from .. import utils as _utils
+from ..protocols import FileStatLike as _FStat
 
 if _ty.TYPE_CHECKING:
     from os import stat_result as _os_stat
 
     from ..path import Path
 
 
-class FileStatLike(_ty.Protocol):
-    __slots__ = ()
-
-    @property
-    @_abc.abstractmethod
-    def st_mode(self) -> int: ...
-    @property
-    @_abc.abstractmethod
-    def st_size(self) -> int: ...
-    @property
-    @_abc.abstractmethod
-    def st_mtime(self) -> int: ...
-
-
-class FileStat(FileStatLike):
+class FileStat(_FStat):
     __slots__ = (
         "st_mode",
         "st_nlink",
         "st_uid",
         "st_gid",
         "st_size",
         "st_atime",
```

### Comparing `pathlib_next-0.2.1/src/pathlib_next/utils/sync.py` & `pathlib_next-0.3.0/src/pathlib_next/utils/sync.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.2.1/tests/test_local.py` & `pathlib_next-0.3.0/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.2.1/tests/test_uri.py` & `pathlib_next-0.3.0/tests/test_uri.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.2.1/LICENSE` & `pathlib_next-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.2.1/pyproject.toml` & `pathlib_next-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pathlib_next"
-version = "0.2.1"
+version = "0.3.0"
 authors = [{ name = "Jose A" }]
 description = "Generic Path Protocol based pathlib"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `pathlib_next-0.2.1/PKG-INFO` & `pathlib_next-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pathlib_next
-Version: 0.2.1
+Version: 0.3.0
 Summary: Generic Path Protocol based pathlib
 Project-URL: Homepage, https://github.com/jose-pr/pathlib_next/
 Project-URL: Issues, https://github.com/jose-pr/pathlib_next/issues
 Author: Jose A
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


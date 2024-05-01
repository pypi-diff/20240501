# Comparing `tmp/caustic.cst-1.6.0.tar.gz` & `tmp/caustic.cst-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caustic.cst-1.6.0.tar", last modified: Sat Apr 27 23:16:16 2024, max compression
+gzip compressed data, was "caustic.cst-2.0.0.tar", last modified: Wed May  1 16:07:22 2024, max compression
```

## Comparing `caustic.cst-1.6.0.tar` & `caustic.cst-2.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-27 23:16:16.418887 caustic.cst-1.6.0/
--rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.cst-1.6.0/LICENSE
--rw-r--r--   0 shae      (1000) shae      (1000)     4296 2024-04-27 23:16:16.418887 caustic.cst-1.6.0/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)     3416 2024-04-27 01:33:21.000000 caustic.cst-1.6.0/README.md
--rw-r--r--   0 shae      (1000) shae      (1000)      962 2024-04-27 02:02:13.000000 caustic.cst-1.6.0/pyproject.toml
--rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-27 23:16:16.418887 caustic.cst-1.6.0/setup.cfg
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-27 23:16:16.412221 caustic.cst-1.6.0/src/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-27 23:16:16.412221 caustic.cst-1.6.0/src/caustic/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-27 23:16:16.418887 caustic.cst-1.6.0/src/caustic/cst/
--rw-r--r--   0 shae      (1000) shae      (1000)      441 2024-04-27 01:10:51.000000 caustic.cst-1.6.0/src/caustic/cst/__init__.py
--rw-r--r--   0 shae      (1000) shae      (1000)     1235 2024-04-27 01:12:09.000000 caustic.cst-1.6.0/src/caustic/cst/atom.py
--rw-r--r--   0 shae      (1000) shae      (1000)     1914 2024-04-27 03:49:40.000000 caustic.cst-1.6.0/src/caustic/cst/bases.py
--rw-r--r--   0 shae      (1000) shae      (1000)      485 2024-04-24 01:40:40.000000 caustic.cst-1.6.0/src/caustic/cst/block.py
--rw-r--r--   0 shae      (1000) shae      (1000)      692 2024-04-25 22:29:24.000000 caustic.cst-1.6.0/src/caustic/cst/constant.py
--rw-r--r--   0 shae      (1000) shae      (1000)     5652 2024-04-25 21:43:27.000000 caustic.cst-1.6.0/src/caustic/cst/expression.py
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-27 23:16:16.418887 caustic.cst-1.6.0/src/caustic/cst/mods/
--rw-r--r--   0 shae      (1000) shae      (1000)      946 2024-04-24 16:44:17.000000 caustic.cst-1.6.0/src/caustic/cst/mods/m_exception.py
--rw-r--r--   0 shae      (1000) shae      (1000)     1522 2024-04-24 18:46:52.000000 caustic.cst-1.6.0/src/caustic/cst/serialize.py
--rw-r--r--   0 shae      (1000) shae      (1000)     2663 2024-04-27 23:15:28.000000 caustic.cst-1.6.0/src/caustic/cst/statement.py
--rw-r--r--   0 shae      (1000) shae      (1000)     1381 2024-04-27 03:49:51.000000 caustic.cst-1.6.0/src/caustic/cst/typedecl.py
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-27 23:16:16.418887 caustic.cst-1.6.0/src/caustic.cst.egg-info/
--rw-r--r--   0 shae      (1000) shae      (1000)     4296 2024-04-27 23:16:16.000000 caustic.cst-1.6.0/src/caustic.cst.egg-info/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)      470 2024-04-27 23:16:16.000000 caustic.cst-1.6.0/src/caustic.cst.egg-info/SOURCES.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-27 23:16:16.000000 caustic.cst-1.6.0/src/caustic.cst.egg-info/dependency_links.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-04-27 23:16:16.000000 caustic.cst-1.6.0/src/caustic.cst.egg-info/top_level.txt
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 16:07:22.616207 caustic.cst-2.0.0/
+-rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.cst-2.0.0/LICENSE
+-rw-r--r--   0 shae      (1000) shae      (1000)     3916 2024-05-01 16:07:22.612874 caustic.cst-2.0.0/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)     3036 2024-05-01 16:06:51.000000 caustic.cst-2.0.0/README.md
+-rw-r--r--   0 shae      (1000) shae      (1000)      962 2024-04-29 19:28:18.000000 caustic.cst-2.0.0/pyproject.toml
+-rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-05-01 16:07:22.616207 caustic.cst-2.0.0/setup.cfg
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 16:07:22.599540 caustic.cst-2.0.0/src/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 16:07:22.602874 caustic.cst-2.0.0/src/caustic/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 16:07:22.609540 caustic.cst-2.0.0/src/caustic/cst/
+-rw-r--r--   0 shae      (1000) shae      (1000)     2678 2024-04-30 20:59:39.000000 caustic.cst-2.0.0/src/caustic/cst/__init__.py
+-rw-r--r--   0 shae      (1000) shae      (1000)      324 2024-04-29 19:40:11.000000 caustic.cst-2.0.0/src/caustic/cst/block.py
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 16:07:22.612874 caustic.cst-2.0.0/src/caustic/cst/expressions/
+-rw-r--r--   0 shae      (1000) shae      (1000)      389 2024-04-30 21:36:49.000000 caustic.cst-2.0.0/src/caustic/cst/expressions/__init__.py
+-rw-r--r--   0 shae      (1000) shae      (1000)      782 2024-04-29 19:33:25.000000 caustic.cst-2.0.0/src/caustic/cst/expressions/atoms.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     3555 2024-05-01 15:58:08.000000 caustic.cst-2.0.0/src/caustic/cst/expressions/operators.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     1869 2024-05-01 01:31:21.000000 caustic.cst-2.0.0/src/caustic/cst/procedure.py
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 16:07:22.612874 caustic.cst-2.0.0/src/caustic/cst/statements/
+-rw-r--r--   0 shae      (1000) shae      (1000)     2240 2024-05-01 15:50:31.000000 caustic.cst-2.0.0/src/caustic/cst/statements/__init__.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     2296 2024-05-01 04:13:28.000000 caustic.cst-2.0.0/src/caustic/cst/statements/objects.py
+-rw-r--r--   0 shae      (1000) shae      (1000)      403 2024-05-01 02:40:07.000000 caustic.cst-2.0.0/src/caustic/cst/typedecl.py
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 16:07:22.612874 caustic.cst-2.0.0/src/caustic.cst.egg-info/
+-rw-r--r--   0 shae      (1000) shae      (1000)     3916 2024-05-01 16:07:22.000000 caustic.cst-2.0.0/src/caustic.cst.egg-info/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)      493 2024-05-01 16:07:22.000000 caustic.cst-2.0.0/src/caustic.cst.egg-info/SOURCES.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-05-01 16:07:22.000000 caustic.cst-2.0.0/src/caustic.cst.egg-info/dependency_links.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-05-01 16:07:22.000000 caustic.cst-2.0.0/src/caustic.cst.egg-info/top_level.txt
```

### Comparing `caustic.cst-1.6.0/LICENSE` & `caustic.cst-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caustic.cst-1.6.0/PKG-INFO` & `caustic.cst-2.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustic.cst
-Version: 1.6.0
+Version: 2.0.0
 Summary: Caustic's Abstract Syntax Tree, or CST
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticAST
 Project-URL: Issues, https://codeberg.org/Caustic/CausticAST/issues
 Keywords: caustic,language,parser,ast,syntax,tree
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -18,22 +18,24 @@
 Classifier: Topic :: Software Development :: Interpreters
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Caustic's Abstract Syntax Tree
 
+> !NOTE! `serialize` module not yet re-implemented
+
 Note that the `serialize` module, instead of providing node types,
 provides (de)serialization functions for nodes
 
 # Nodes
 
 > Note: Treat all names as being under `caustic.cst`
 
-> This took way too long to make
+> !NOTE! Outdated!
 
 ```
 bases.CausticASTNode
  ├─ bases.BaseStatement
  │   ├─ statement.ProcedureStatement
  │   ├─ statement.ImportStatement
  │   ├─ statement.ExportStatement
@@ -97,23 +99,7 @@
  │       │   ├─ atom.Bytes
  │       │   └─ atom.String
  │       ├─ atom.Identifier
  │       └─ atom.DottedIdentifier
  ├─ block.Line
  └─ block.Block
 ```
-
-## "Mod" nodes
-
-These nodes are used along with compiler mods (by using the `insmod` directive, for instance)
-
-> Note: Nodes under the `bases` name are not used with mods, but the nodes under them
-inherit from them
-
-### Exceptions
-```
-bases.BaseStatement
- ├─ mods.m_exception.RaiseStatement
- ├─ mods.m_exception.TryStatement
- ├─ mods.m_exception.CatchStatement
- └─ mods.m_exception.LowerStatement
-```
```

### Comparing `caustic.cst-1.6.0/README.md` & `caustic.cst-2.0.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Caustic's Abstract Syntax Tree
 
+> !NOTE! `serialize` module not yet re-implemented
+
 Note that the `serialize` module, instead of providing node types,
 provides (de)serialization functions for nodes
 
 # Nodes
 
 > Note: Treat all names as being under `caustic.cst`
 
-> This took way too long to make
+> !NOTE! Outdated!
 
 ```
 bases.CausticASTNode
  ├─ bases.BaseStatement
  │   ├─ statement.ProcedureStatement
  │   ├─ statement.ImportStatement
  │   ├─ statement.ExportStatement
@@ -75,23 +77,7 @@
  │       │   ├─ atom.Bytes
  │       │   └─ atom.String
  │       ├─ atom.Identifier
  │       └─ atom.DottedIdentifier
  ├─ block.Line
  └─ block.Block
 ```
-
-## "Mod" nodes
-
-These nodes are used along with compiler mods (by using the `insmod` directive, for instance)
-
-> Note: Nodes under the `bases` name are not used with mods, but the nodes under them
-inherit from them
-
-### Exceptions
-```
-bases.BaseStatement
- ├─ mods.m_exception.RaiseStatement
- ├─ mods.m_exception.TryStatement
- ├─ mods.m_exception.CatchStatement
- └─ mods.m_exception.LowerStatement
-```
```

### Comparing `caustic.cst-1.6.0/pyproject.toml` & `caustic.cst-2.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "caustic.cst"
-version = "1.6.0"
+version = "2.0.0"
 dependencies = []
 requires-python = ">=3.9"
 authors = [{name="Shae.c32"}]
 maintainers = []
 description = "Caustic's Abstract Syntax Tree, or CST"
 readme = "README.md"
 keywords = ['caustic', 'language', 'parser', 'ast', 'syntax', 'tree']
```

### Comparing `caustic.cst-1.6.0/src/caustic.cst.egg-info/PKG-INFO` & `caustic.cst-2.0.0/src/caustic.cst.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustic.cst
-Version: 1.6.0
+Version: 2.0.0
 Summary: Caustic's Abstract Syntax Tree, or CST
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticAST
 Project-URL: Issues, https://codeberg.org/Caustic/CausticAST/issues
 Keywords: caustic,language,parser,ast,syntax,tree
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -18,22 +18,24 @@
 Classifier: Topic :: Software Development :: Interpreters
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Caustic's Abstract Syntax Tree
 
+> !NOTE! `serialize` module not yet re-implemented
+
 Note that the `serialize` module, instead of providing node types,
 provides (de)serialization functions for nodes
 
 # Nodes
 
 > Note: Treat all names as being under `caustic.cst`
 
-> This took way too long to make
+> !NOTE! Outdated!
 
 ```
 bases.CausticASTNode
  ├─ bases.BaseStatement
  │   ├─ statement.ProcedureStatement
  │   ├─ statement.ImportStatement
  │   ├─ statement.ExportStatement
@@ -97,23 +99,7 @@
  │       │   ├─ atom.Bytes
  │       │   └─ atom.String
  │       ├─ atom.Identifier
  │       └─ atom.DottedIdentifier
  ├─ block.Line
  └─ block.Block
 ```
-
-## "Mod" nodes
-
-These nodes are used along with compiler mods (by using the `insmod` directive, for instance)
-
-> Note: Nodes under the `bases` name are not used with mods, but the nodes under them
-inherit from them
-
-### Exceptions
-```
-bases.BaseStatement
- ├─ mods.m_exception.RaiseStatement
- ├─ mods.m_exception.TryStatement
- ├─ mods.m_exception.CatchStatement
- └─ mods.m_exception.LowerStatement
-```
```


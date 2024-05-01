# Comparing `tmp/caustic.cst-2.1.0.tar.gz` & `tmp/caustic.cst-2.1.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caustic.cst-2.1.0.tar", last modified: Wed May  1 16:26:15 2024, max compression
+gzip compressed data, was "caustic.cst-2.1.0.post1.tar", last modified: Wed May  1 16:46:37 2024, max compression
```

## Comparing `caustic.cst-2.1.0.tar` & `caustic.cst-2.1.0.post1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 16:26:15.666218 caustic.cst-2.1.0/
--rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.cst-2.1.0/LICENSE
--rw-r--r--   0 shae      (1000) shae      (1000)     3864 2024-05-01 16:26:15.666218 caustic.cst-2.1.0/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)     2984 2024-05-01 16:19:39.000000 caustic.cst-2.1.0/README.md
--rw-r--r--   0 shae      (1000) shae      (1000)      962 2024-05-01 16:07:40.000000 caustic.cst-2.1.0/pyproject.toml
--rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-05-01 16:26:15.666218 caustic.cst-2.1.0/setup.cfg
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 16:26:15.652885 caustic.cst-2.1.0/src/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 16:26:15.652885 caustic.cst-2.1.0/src/caustic/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 16:26:15.662885 caustic.cst-2.1.0/src/caustic/cst/
--rw-r--r--   0 shae      (1000) shae      (1000)     2727 2024-05-01 16:08:03.000000 caustic.cst-2.1.0/src/caustic/cst/__init__.py
--rw-r--r--   0 shae      (1000) shae      (1000)      324 2024-04-29 19:40:11.000000 caustic.cst-2.1.0/src/caustic/cst/block.py
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 16:26:15.662885 caustic.cst-2.1.0/src/caustic/cst/expressions/
--rw-r--r--   0 shae      (1000) shae      (1000)      389 2024-04-30 21:36:49.000000 caustic.cst-2.1.0/src/caustic/cst/expressions/__init__.py
--rw-r--r--   0 shae      (1000) shae      (1000)      782 2024-04-29 19:33:25.000000 caustic.cst-2.1.0/src/caustic/cst/expressions/atoms.py
--rw-r--r--   0 shae      (1000) shae      (1000)     3555 2024-05-01 15:58:08.000000 caustic.cst-2.1.0/src/caustic/cst/expressions/operators.py
--rw-r--r--   0 shae      (1000) shae      (1000)     1869 2024-05-01 01:31:21.000000 caustic.cst-2.1.0/src/caustic/cst/procedure.py
--rw-r--r--   0 shae      (1000) shae      (1000)     1498 2024-05-01 16:25:05.000000 caustic.cst-2.1.0/src/caustic/cst/serialize.py
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 16:26:15.662885 caustic.cst-2.1.0/src/caustic/cst/statements/
--rw-r--r--   0 shae      (1000) shae      (1000)     2240 2024-05-01 15:50:31.000000 caustic.cst-2.1.0/src/caustic/cst/statements/__init__.py
--rw-r--r--   0 shae      (1000) shae      (1000)     2296 2024-05-01 04:13:28.000000 caustic.cst-2.1.0/src/caustic/cst/statements/objects.py
--rw-r--r--   0 shae      (1000) shae      (1000)      403 2024-05-01 02:40:07.000000 caustic.cst-2.1.0/src/caustic/cst/typedecl.py
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 16:26:15.666218 caustic.cst-2.1.0/src/caustic.cst.egg-info/
--rw-r--r--   0 shae      (1000) shae      (1000)     3864 2024-05-01 16:26:15.000000 caustic.cst-2.1.0/src/caustic.cst.egg-info/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)      522 2024-05-01 16:26:15.000000 caustic.cst-2.1.0/src/caustic.cst.egg-info/SOURCES.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-05-01 16:26:15.000000 caustic.cst-2.1.0/src/caustic.cst.egg-info/dependency_links.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-05-01 16:26:15.000000 caustic.cst-2.1.0/src/caustic.cst.egg-info/top_level.txt
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 16:46:37.389511 caustic.cst-2.1.0.post1/
+-rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.cst-2.1.0.post1/LICENSE
+-rw-r--r--   0 shae      (1000) shae      (1000)     3964 2024-05-01 16:46:37.389511 caustic.cst-2.1.0.post1/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)     3078 2024-05-01 16:44:11.000000 caustic.cst-2.1.0.post1/README.md
+-rw-r--r--   0 shae      (1000) shae      (1000)      964 2024-05-01 16:27:31.000000 caustic.cst-2.1.0.post1/pyproject.toml
+-rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-05-01 16:46:37.389511 caustic.cst-2.1.0.post1/setup.cfg
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 16:46:37.379511 caustic.cst-2.1.0.post1/src/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 16:46:37.379511 caustic.cst-2.1.0.post1/src/caustic/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 16:46:37.386178 caustic.cst-2.1.0.post1/src/caustic/cst/
+-rw-r--r--   0 shae      (1000) shae      (1000)     2727 2024-05-01 16:08:03.000000 caustic.cst-2.1.0.post1/src/caustic/cst/__init__.py
+-rw-r--r--   0 shae      (1000) shae      (1000)      324 2024-04-29 19:40:11.000000 caustic.cst-2.1.0.post1/src/caustic/cst/block.py
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 16:46:37.389511 caustic.cst-2.1.0.post1/src/caustic/cst/expressions/
+-rw-r--r--   0 shae      (1000) shae      (1000)      389 2024-04-30 21:36:49.000000 caustic.cst-2.1.0.post1/src/caustic/cst/expressions/__init__.py
+-rw-r--r--   0 shae      (1000) shae      (1000)      782 2024-04-29 19:33:25.000000 caustic.cst-2.1.0.post1/src/caustic/cst/expressions/atoms.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     3555 2024-05-01 15:58:08.000000 caustic.cst-2.1.0.post1/src/caustic/cst/expressions/operators.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     1869 2024-05-01 01:31:21.000000 caustic.cst-2.1.0.post1/src/caustic/cst/procedure.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     1498 2024-05-01 16:25:05.000000 caustic.cst-2.1.0.post1/src/caustic/cst/serialize.py
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 16:46:37.389511 caustic.cst-2.1.0.post1/src/caustic/cst/statements/
+-rw-r--r--   0 shae      (1000) shae      (1000)     2240 2024-05-01 15:50:31.000000 caustic.cst-2.1.0.post1/src/caustic/cst/statements/__init__.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     2296 2024-05-01 04:13:28.000000 caustic.cst-2.1.0.post1/src/caustic/cst/statements/objects.py
+-rw-r--r--   0 shae      (1000) shae      (1000)      403 2024-05-01 02:40:07.000000 caustic.cst-2.1.0.post1/src/caustic/cst/typedecl.py
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-01 16:46:37.389511 caustic.cst-2.1.0.post1/src/caustic.cst.egg-info/
+-rw-r--r--   0 shae      (1000) shae      (1000)     3964 2024-05-01 16:46:37.000000 caustic.cst-2.1.0.post1/src/caustic.cst.egg-info/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)      522 2024-05-01 16:46:37.000000 caustic.cst-2.1.0.post1/src/caustic.cst.egg-info/SOURCES.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-05-01 16:46:37.000000 caustic.cst-2.1.0.post1/src/caustic.cst.egg-info/dependency_links.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-05-01 16:46:37.000000 caustic.cst-2.1.0.post1/src/caustic.cst.egg-info/top_level.txt
```

### Comparing `caustic.cst-2.1.0/LICENSE` & `caustic.cst-2.1.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `caustic.cst-2.1.0/PKG-INFO` & `caustic.cst-2.1.0.post1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,103 +1,75 @@
-Metadata-Version: 2.1
-Name: caustic.cst
-Version: 2.1.0
-Summary: Caustic's Abstract Syntax Tree, or CST
-Author: Shae.c32
-Project-URL: Homepage, https://codeberg.org/Caustic/CausticAST
-Project-URL: Issues, https://codeberg.org/Caustic/CausticAST/issues
-Keywords: caustic,language,parser,ast,syntax,tree
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Other
-Classifier: Topic :: File Formats
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Compilers
-Classifier: Topic :: Software Development :: Documentation
-Classifier: Topic :: Software Development :: Interpreters
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 Caustic's Abstract Syntax Tree
 
 Note that the `serialize` module, instead of providing node types,
 provides (de)serialization functions for nodes
 
 # Nodes
 
 > Note: Treat all names as being under `caustic.cst`
 
-> !NOTE! Outdated!
+> Note: nodes marked with `*` are considered "base" nodes,
+> and nodes prefixed with `_` are implementation details used
+> purely for grouping
 
 ```
-bases.CausticASTNode
- ├─ bases.BaseStatement
- │   ├─ statement.ProcedureStatement
- │   ├─ statement.ImportStatement
- │   ├─ statement.ExportStatement
- │   ├─ statement.IfStatement
- │   │   └─ statement.ElifStatement
- │   ├─ statement.ElseStatement
- │   ├─ statement.ForStatement
- │   ├─ statement.WhileStatement
- │   ├─ statement.Directive
- │   └─ bases.BaseTypeDecl
- │       ├─ typedecl.SingletonType
- │       ├─ typedecl.EnumType
- │       └─ typedecl.StructType
- │           └─ typedecl.ClassType
- ├─ bases.BaseExpression
- │   ├─ expression.Invoke
- │   ├─ expression.ProcedureExpr
- │   ├─ bases.BaseOperator
- │   │   ├─ bases.BaseUnaryOperator
- │   │   │   ├─ expression.UPlus
- │   │   │   ├─ expression.UMinus
- │   │   │   ├─ expression.Increment
- │   │   │   ├─ expression.Decrement
- │   │   │   ├─ expression.BitInvert
- │   │   │   └─ expression.LogNot
- │   │   ├─ bases.BaseBinaryOperator
- │   │   │   ├─ expression.AssignExpr
- │   │   │   ├─ expression.Add
- │   │   │   ├─ expression.Sub
- │   │   │   ├─ expression.Mult
- │   │   │   ├─ expression.Div
- │   │   │   ├─ expression.Mod
- │   │   │   ├─ expression.MMul
- │   │   │   ├─ expression.Pow
- │   │   │   ├─ expression.Equality [EQ]
- │   │   │   ├─ expression.Inequality [NE]
- │   │   │   ├─ expression.LessThan [LT]
- │   │   │   ├─ expression.GreaterThan [GT]
- │   │   │   ├─ expression.LessThanOrEquality [LE]
- │   │   │   ├─ expression.GreaterThanOrEquality [GE]
- │   │   │   ├─ expression.Nullish
- │   │   │   ├─ expression.LogAnd
- │   │   │   ├─ expression.LogOr
- │   │   │   ├─ expression.LogXor
- │   │   │   ├─ expression.BitAnd
- │   │   │   ├─ expression.BitOr
- │   │   │   ├─ expression.BitXor
- │   │   │   ├─ expression.LShift
- │   │   │   └─ expression.RShift
- │   │   └─ expression.Ternary
- │   └─ bases.BaseAtom
- │       ├─ bases.BaseConstant
- │       │   ├─ constant.BoolTrue
- │       │   ├─ constant.BoolFalse
- │       │   ├─ constant.Null
- │       │   └─ constant.Default
- │       ├─ bases.BaseLiteral
- │       │   ├─ atom.Integer
- │       │   ├─ atom.Decimal
- │       │   ├─ atom.Char
- │       │   ├─ atom.Bytes
- │       │   └─ atom.String
- │       ├─ atom.Identifier
- │       └─ atom.DottedIdentifier
- ├─ block.Line
- └─ block.Block
+CSTNode*
+ ├─ CustomNode
+ ├─ block.Block
+ ├─ typedecl.Type
+ ├─ expressions.Expression*
+ │   ├─ procedure.ProcedureExpr
+ │   ├─ procedure.Invokation
+ │   ├─ expressions.atoms.Atom*
+ │   │   ├─ expressions.atoms.Identifier
+ │   │   ├─ expressions.atoms.DottedIdentifier
+ │   │   └─ expressions.atoms.Integer
+ │   ├─ expressions.operators.Operation*
+ │   │   ├─ expressions.operators._UnaryOp*
+ │   │   │   ├─ expressions.operators.Positive
+ │   │   │   ├─ expressions.operators.Negative
+ │   │   │   ├─ expressions.operators.LogInverse
+ │   │   │   ├─ expressions.operators.BitInverse
+ │   │   │   ├─ expressions.operators.Increment
+ │   │   │   └─ expressions.operators.Decrement
+ │   │   ├─ expressions.operators._BinaryOp*
+ │   │   │   ├─ expressions.operators.Subscription
+ │   │   │   ├─ expressions.operators.Add
+ │   │   │   ├─ expressions.operators.Sub
+ │   │   │   ├─ expressions.operators.Mult
+ │   │   │   ├─ expressions.operators.MMul
+ │   │   │   ├─ expressions.operators.Div
+ │   │   │   ├─ expressions.operators.Mod
+ │   │   │   ├─ expressions.operators.Exp
+ │   │   │   ├─ expressions.operators.EQ
+ │   │   │   ├─ expressions.operators.NE
+ │   │   │   ├─ expressions.operators.LT
+ │   │   │   ├─ expressions.operators.LE
+ │   │   │   ├─ expressions.operators.GT
+ │   │   │   ├─ expressions.operators.GE
+ │   │   │   ├─ expressions.operators.NullCoalescing
+ │   │   │   ├─ expressions.operators.LogAnd
+ │   │   │   ├─ expressions.operators.LogOr
+ │   │   │   ├─ expressions.operators.LogXOr
+ │   │   │   ├─ expressions.operators.BitAnd
+ │   │   │   ├─ expressions.operators.BitOr
+ │   │   │   ├─ expressions.operators.BitXOr
+ │   │   │   ├─ expressions.operators.LShift
+ │   │   │   └─ expressions.operators.RShift
+ │   │   └─ expressions.operators.TernaryConditional
+ └─ statements.Statement*
+     ├─ procedure.ProcedureStmt
+     ├─ statements.Declaration
+     ├─ statements.Assignment
+     ├─ statements.If
+     │   └─ statements.Elif
+     ├─ statements.Else
+     ├─ statements.While
+     │   ├─ statements.DoWhile
+     │   └─ statements.For
+     ├─ statements.ForOf
+     └─ statements.objects.Object*
+         ├─ statements.objects.Enum
+         ├─ statements.objects.Struct
+         ├─ statements.objects.Namespace
+         └─ statements.objects.Class
 ```
```

### Comparing `caustic.cst-2.1.0/pyproject.toml` & `caustic.cst-2.1.0.post1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "caustic.cst"
-version = "2.1.0"
+version = "2.1.0-1"
 dependencies = []
 requires-python = ">=3.9"
 authors = [{name="Shae.c32"}]
 maintainers = []
 description = "Caustic's Abstract Syntax Tree, or CST"
 readme = "README.md"
 keywords = ['caustic', 'language', 'parser', 'ast', 'syntax', 'tree']
```

### Comparing `caustic.cst-2.1.0/src/caustic/cst/__init__.py` & `caustic.cst-2.1.0.post1/src/caustic/cst/__init__.py`

 * *Files identical despite different names*

### Comparing `caustic.cst-2.1.0/src/caustic/cst/expressions/atoms.py` & `caustic.cst-2.1.0.post1/src/caustic/cst/expressions/atoms.py`

 * *Files identical despite different names*

### Comparing `caustic.cst-2.1.0/src/caustic/cst/expressions/operators.py` & `caustic.cst-2.1.0.post1/src/caustic/cst/expressions/operators.py`

 * *Files identical despite different names*

### Comparing `caustic.cst-2.1.0/src/caustic/cst/procedure.py` & `caustic.cst-2.1.0.post1/src/caustic/cst/procedure.py`

 * *Files identical despite different names*

### Comparing `caustic.cst-2.1.0/src/caustic/cst/serialize.py` & `caustic.cst-2.1.0.post1/src/caustic/cst/serialize.py`

 * *Files identical despite different names*

### Comparing `caustic.cst-2.1.0/src/caustic/cst/statements/__init__.py` & `caustic.cst-2.1.0.post1/src/caustic/cst/statements/__init__.py`

 * *Files identical despite different names*

### Comparing `caustic.cst-2.1.0/src/caustic/cst/statements/objects.py` & `caustic.cst-2.1.0.post1/src/caustic/cst/statements/objects.py`

 * *Files identical despite different names*

### Comparing `caustic.cst-2.1.0/src/caustic.cst.egg-info/SOURCES.txt` & `caustic.cst-2.1.0.post1/src/caustic.cst.egg-info/SOURCES.txt`

 * *Files identical despite different names*


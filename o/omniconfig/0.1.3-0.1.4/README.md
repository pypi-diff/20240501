# Comparing `tmp/omniconfig-0.1.3.tar.gz` & `tmp/omniconfig-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniconfig-0.1.3.tar", max compression
+gzip compressed data, was "omniconfig-0.1.4.tar", max compression
```

## Comparing `omniconfig-0.1.3.tar` & `omniconfig-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    34523 2024-04-22 18:56:40.046281 omniconfig-0.1.3/LICENSE
--rw-r--r--   0        0        0     6478 2024-04-28 06:53:26.458810 omniconfig-0.1.3/README.md
--rw-r--r--   0        0        0      391 2024-04-30 21:33:49.203985 omniconfig-0.1.3/omniconfig/__init__.py
--rw-r--r--   0        0        0    17446 2024-04-28 06:53:26.502810 omniconfig-0.1.3/omniconfig/args.py
--rw-r--r--   0        0        0    14702 2024-04-30 21:25:09.580828 omniconfig-0.1.3/omniconfig/configclass.py
--rw-r--r--   0        0        0     9495 2024-04-30 21:30:31.694785 omniconfig-0.1.3/omniconfig/parser.py
--rw-r--r--   0        0        0     6473 2024-04-28 06:53:26.510810 omniconfig-0.1.3/omniconfig/utils.py
--rw-r--r--   0        0        0       89 2024-04-30 21:34:02.868068 omniconfig-0.1.3/omniconfig/version.py
--rw-r--r--   0        0        0      858 2024-04-30 21:35:53.460740 omniconfig-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     7127 1970-01-01 00:00:00.000000 omniconfig-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-22 18:56:40.046281 omniconfig-0.1.4/LICENSE
+-rw-r--r--   0        0        0     6478 2024-04-28 06:53:26.458810 omniconfig-0.1.4/README.md
+-rw-r--r--   0        0        0      391 2024-04-30 21:33:49.203985 omniconfig-0.1.4/omniconfig/__init__.py
+-rw-r--r--   0        0        0    17446 2024-04-28 06:53:26.502810 omniconfig-0.1.4/omniconfig/args.py
+-rw-r--r--   0        0        0    14972 2024-05-01 03:48:02.039740 omniconfig-0.1.4/omniconfig/configclass.py
+-rw-r--r--   0        0        0     9495 2024-04-30 21:30:31.694785 omniconfig-0.1.4/omniconfig/parser.py
+-rw-r--r--   0        0        0     6473 2024-04-28 06:53:26.510810 omniconfig-0.1.4/omniconfig/utils.py
+-rw-r--r--   0        0        0       89 2024-05-01 03:43:44.994185 omniconfig-0.1.4/omniconfig/version.py
+-rw-r--r--   0        0        0      858 2024-05-01 03:43:39.490152 omniconfig-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     7127 1970-01-01 00:00:00.000000 omniconfig-0.1.4/PKG-INFO
```

### Comparing `omniconfig-0.1.3/LICENSE` & `omniconfig-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `omniconfig-0.1.3/README.md` & `omniconfig-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `omniconfig-0.1.3/omniconfig/args.py` & `omniconfig-0.1.4/omniconfig/args.py`

 * *Files identical despite different names*

### Comparing `omniconfig-0.1.3/omniconfig/configclass.py` & `omniconfig-0.1.4/omniconfig/configclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -326,15 +326,22 @@
     Args:
         self: Config dataclass instance.
         path (str): Path to dump the config dict. Defaults to ``""``.
 
     Returns:
         dict[str, Any]: The dict.
     """
-    rst = {field.name: _to_dump_value(getattr(self, field.name)) for field in _get_init_fields(self.__class__)}
+    rst = {}
+    for field in _get_init_fields(self.__class__):
+        field_type, field_type_optional = parse_field_type(field.type)
+        value = _to_dump_value(getattr(self, field.name))
+        if field_type_optional and hasattr(field_type, "get_arguments") and value is None:
+            rst[f"enable_{field.name}"] = False
+        else:
+            rst[field.name] = value
     if path:
         if path.endswith(".toml"):
             dump_toml(rst, path)
         elif path.endswith(("yaml", "yml")):
             dump_yaml(rst, path)
         else:
             raise ValueError(f"Unsupported file format {path}")
```

### Comparing `omniconfig-0.1.3/omniconfig/parser.py` & `omniconfig-0.1.4/omniconfig/parser.py`

 * *Files identical despite different names*

### Comparing `omniconfig-0.1.3/omniconfig/utils.py` & `omniconfig-0.1.4/omniconfig/utils.py`

 * *Files identical despite different names*

### Comparing `omniconfig-0.1.3/pyproject.toml` & `omniconfig-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omniconfig"
-version = "0.1.3"
+version = "0.1.4"
 description = "Python package for parsing configurations from YAML and TOML and command-line interface."
 authors = ["Yujun(Xavier) Lin"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10 <4.0"
```

### Comparing `omniconfig-0.1.3/PKG-INFO` & `omniconfig-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniconfig
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python package for parsing configurations from YAML and TOML and command-line interface.
 License: AGPL-3.0-only
 Author: Yujun(Xavier) Lin
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```


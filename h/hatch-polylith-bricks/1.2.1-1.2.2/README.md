# Comparing `tmp/hatch_polylith_bricks-1.2.1.tar.gz` & `tmp/hatch_polylith_bricks-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hatch_polylith_bricks-1.2.1.tar", max compression
+gzip compressed data, was "hatch_polylith_bricks-1.2.2.tar", max compression
```

## Comparing `hatch_polylith_bricks-1.2.1.tar` & `hatch_polylith_bricks-1.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     3140 2024-01-23 22:26:31.652064 hatch_polylith_bricks-1.2.1/README.md
--rw-r--r--   0        0        0       74 2024-04-11 15:26:35.138411 hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/hatch/__init__.py
--rw-r--r--   0        0        0      419 2024-04-11 15:26:35.138667 hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/hatch/core.py
--rw-r--r--   0        0        0        0 2024-01-21 11:02:57.120575 hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/hatch/hooks/__init__.py
--rw-r--r--   0        0        0     1600 2024-04-11 15:26:35.141601 hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/hatch/hooks/bricks.py
--rw-r--r--   0        0        0        0 2024-01-21 11:02:57.119034 hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/hatch_hooks/__init__.py
--rw-r--r--   0        0        0      192 2024-04-11 15:26:35.138145 hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/hatch_hooks/hooks.py
--rw-r--r--   0        0        0      253 2024-04-11 15:26:35.138894 hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/parsing/__init__.py
--rw-r--r--   0        0        0      751 2024-01-23 21:16:34.622595 hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/parsing/core.py
--rw-r--r--   0        0        0     2156 2024-01-23 21:16:34.622843 hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/parsing/rewrite.py
--rw-r--r--   0        0        0      543 2024-04-11 15:26:35.139948 hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/repo/__init__.py
--rw-r--r--   0        0        0      861 2024-04-11 15:26:35.140817 hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/repo/get.py
--rw-r--r--   0        0        0     1964 2024-02-04 09:48:25.380602 hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/repo/repo.py
--rw-r--r--   0        0        0      466 2024-04-11 15:26:35.136568 hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/toml/__init__.py
--rw-r--r--   0        0        0     2919 2024-04-11 15:26:35.137889 hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/toml/core.py
--rw-r--r--   0        0        0      676 2024-04-11 15:26:35.136006 hatch_polylith_bricks-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     3894 1970-01-01 00:00:00.000000 hatch_polylith_bricks-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     3140 2024-02-09 08:50:51.457205 hatch_polylith_bricks-1.2.2/README.md
+-rw-r--r--   0        0        0       74 2024-05-01 07:11:19.859275 hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/hatch/__init__.py
+-rw-r--r--   0        0        0      419 2024-05-01 07:11:19.859554 hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/hatch/core.py
+-rw-r--r--   0        0        0        0 2024-01-22 14:07:16.218717 hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/hatch/hooks/__init__.py
+-rw-r--r--   0        0        0     1602 2024-05-01 07:11:19.860335 hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/hatch/hooks/bricks.py
+-rw-r--r--   0        0        0        0 2024-01-22 14:07:16.215883 hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/hatch_hooks/__init__.py
+-rw-r--r--   0        0        0      192 2024-05-01 07:11:19.859086 hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/hatch_hooks/hooks.py
+-rw-r--r--   0        0        0      253 2024-05-01 07:11:19.860532 hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/parsing/__init__.py
+-rw-r--r--   0        0        0      751 2024-02-09 08:50:51.444767 hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/parsing/core.py
+-rw-r--r--   0        0        0     2156 2024-02-09 08:50:51.445237 hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/parsing/rewrite.py
+-rw-r--r--   0        0        0      543 2024-05-01 07:11:19.861539 hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/repo/__init__.py
+-rw-r--r--   0        0        0      861 2024-05-01 07:11:19.862462 hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/repo/get.py
+-rw-r--r--   0        0        0     1964 2024-02-09 08:50:51.451835 hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/repo/repo.py
+-rw-r--r--   0        0        0      466 2024-05-01 07:11:19.857016 hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/toml/__init__.py
+-rw-r--r--   0        0        0     3253 2024-05-01 07:11:19.858850 hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/toml/core.py
+-rw-r--r--   0        0        0      676 2024-05-01 07:11:19.856553 hatch_polylith_bricks-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3894 1970-01-01 00:00:00.000000 hatch_polylith_bricks-1.2.2/PKG-INFO
```

### Comparing `hatch_polylith_bricks-1.2.1/README.md` & `hatch_polylith_bricks-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/hatch/hooks/bricks.py` & `hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/hatch/hooks/bricks.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         if not bricks:
             print('No bricks found.')
             return
         if not top_ns:
             build_data['force_include'] = bricks
             return
         ns = parsing.parse_brick_namespace_from_path(bricks)
-        for source, brick in bricks.items():
+        for (source, brick) in bricks.items():
             path = parsing.copy_brick(source, brick, work_dir)
             rewritten_bricks = parsing.rewrite_modules(path, ns, top_ns)
             for item in rewritten_bricks:
                 print(f'Updated {item} with new top namespace for local imports.')
         key = work_dir.as_posix()
         build_data['force_include'][key] = top_ns
```

### Comparing `hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/parsing/core.py` & `hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/parsing/core.py`

 * *Files identical despite different names*

### Comparing `hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/parsing/rewrite.py` & `hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/parsing/rewrite.py`

 * *Files identical despite different names*

### Comparing `hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/repo/__init__.py` & `hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/repo/get.py` & `hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/repo/get.py`

 * *Files identical despite different names*

### Comparing `hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/repo/repo.py` & `hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/repo/repo.py`

 * *Files identical despite different names*

### Comparing `hatch_polylith_bricks-1.2.1/hatch_polylith_bricks/polylith/toml/core.py` & `hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/toml/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from functools import reduce
 from pathlib import Path
 from typing import List, Union
 import tomlkit
 from hatch_polylith_bricks.polylith import repo
 
 def transform_to_package(namespace: str, include: str) -> dict:
-    path, _separator, brick = str.partition(include, f'/{namespace}/')
+    (path, _separator, brick) = str.partition(include, f'/{namespace}/')
     return {'include': f'{namespace}/{brick}', 'from': path}
 
 def get_polylith_section(data) -> dict:
     return data.get('tool', {}).get('polylith', {})
 
 def get_custom_top_namespace_from_polylith_section(data) -> Union[str, None]:
     poly_data = get_polylith_section(data)
@@ -38,36 +38,43 @@
 def get_project_name(data) -> str:
     if repo.is_pep_621_ready(data):
         return data['project']['name']
     return data['tool']['poetry']['name']
 
 def parse_pep_621_dependency(dep: str) -> dict:
     parts = re.split('[\\^~=!<>]', dep)
-    name, *_ = parts if parts else ['']
+    (name, *_) = parts if parts else ['']
     version = str.replace(dep, name, '')
     return {name: version} if name else {}
 
 def parse_poetry_dependency(acc: dict, kv: tuple) -> dict:
-    k, v = kv
+    (k, v) = kv
     if isinstance(v, dict):
         extras = sorted(v.get('extras', []))
         version = v.get('version', '')
         name = k + str.replace(f'{extras}', "'", '') if extras else k
         parsed = {name: version}
     else:
         parsed = {k: v}
     return {**acc, **parsed}
 
+def get_pep_621_optional_dependencies(data) -> List[str]:
+    groups = data['project'].get('optional-dependencies', {})
+    matrix = [v for v in groups.values()] if isinstance(groups, dict) else []
+    return sum(matrix, [])
+
 def parse_project_dependencies(data) -> dict:
     if repo.is_poetry(data):
         deps = data['tool']['poetry'].get('dependencies', {})
         res: dict = reduce(parse_poetry_dependency, deps.items(), {})
         return res
     deps = data['project'].get('dependencies', [])
-    return {k: v for dep in deps for k, v in parse_pep_621_dependency(dep).items()}
+    optional_deps = get_pep_621_optional_dependencies(data)
+    all_deps = deps + optional_deps
+    return {k: v for dep in all_deps for (k, v) in parse_pep_621_dependency(dep).items()}
 
 def get_project_dependencies(data) -> dict:
     items = parse_project_dependencies(data)
     return {'items': items, 'source': repo.default_toml}
 
 def read_toml_document(path: Path) -> tomlkit.TOMLDocument:
     with path.open(encoding='utf-8', errors='ignore') as f:
```

### Comparing `hatch_polylith_bricks-1.2.1/pyproject.toml` & `hatch_polylith_bricks-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hatch-polylith-bricks"
-version = "1.2.1"
+version = "1.2.2"
 description = "Hatch build hook plugin for Polylith"
 authors = ['David Vujic']
 homepage = "https://davidvujic.github.io/python-polylith-docs/"
 repository = "https://github.com/davidvujic/python-polylith"
 license = "MIT"
 readme = "README.md"
```

### Comparing `hatch_polylith_bricks-1.2.1/PKG-INFO` & `hatch_polylith_bricks-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-polylith-bricks
-Version: 1.2.1
+Version: 1.2.2
 Summary: Hatch build hook plugin for Polylith
 Home-page: https://davidvujic.github.io/python-polylith-docs/
 License: MIT
 Author: David Vujic
 Requires-Python: >=3.9,<4.0
 Classifier: Framework :: Hatch
 Classifier: License :: OSI Approved :: MIT License
```


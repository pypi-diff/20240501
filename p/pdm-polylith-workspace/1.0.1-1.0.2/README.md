# Comparing `tmp/pdm_polylith_workspace-1.0.1.tar.gz` & `tmp/pdm_polylith_workspace-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_polylith_workspace-1.0.1.tar", max compression
+gzip compressed data, was "pdm_polylith_workspace-1.0.2.tar", max compression
```

## Comparing `pdm_polylith_workspace-1.0.1.tar` & `pdm_polylith_workspace-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1008 2024-01-23 21:16:34.627315 pdm_polylith_workspace-1.0.1/README.md
--rw-r--r--   0        0        0      568 2024-04-11 15:28:15.485401 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/configuration/__init__.py
--rw-r--r--   0        0        0     2194 2024-04-11 15:28:15.486256 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/configuration/core.py
--rw-r--r--   0        0        0      255 2024-04-11 15:28:15.488389 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/parsing/__init__.py
--rw-r--r--   0        0        0      751 2024-01-23 21:16:34.622595 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/parsing/core.py
--rw-r--r--   0        0        0     2156 2024-01-23 21:16:34.622843 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/parsing/rewrite.py
--rw-r--r--   0        0        0        0 2024-01-23 21:16:34.623045 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/pdm/__init__.py
--rw-r--r--   0        0        0     1150 2024-04-11 15:28:15.490864 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/pdm/core.py
--rw-r--r--   0        0        0        0 2024-01-23 21:16:34.623415 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/pdm/hooks/__init__.py
--rw-r--r--   0        0        0      643 2024-04-11 15:28:15.491360 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/pdm/hooks/bricks.py
--rw-r--r--   0        0        0     1022 2024-04-11 15:28:15.492077 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/pdm/hooks/workspace.py
--rw-r--r--   0        0        0        0 2024-01-23 21:16:34.621252 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/pdm_workspace_hooks/__init__.py
--rw-r--r--   0        0        0      465 2024-04-11 15:28:15.488162 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/pdm_workspace_hooks/core.py
--rw-r--r--   0        0        0      545 2024-04-11 15:28:15.489391 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/repo/__init__.py
--rw-r--r--   0        0        0      862 2024-04-11 15:28:15.490231 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/repo/get.py
--rw-r--r--   0        0        0     1964 2024-02-04 09:48:25.380602 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/repo/repo.py
--rw-r--r--   0        0        0      467 2024-04-11 15:28:15.486521 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/toml/__init__.py
--rw-r--r--   0        0        0     2920 2024-04-11 15:28:15.487750 pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/toml/core.py
--rw-r--r--   0        0        0      641 2024-04-11 15:28:15.484828 pdm_polylith_workspace-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1694 1970-01-01 00:00:00.000000 pdm_polylith_workspace-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1008 2024-02-09 08:50:51.458954 pdm_polylith_workspace-1.0.2/README.md
+-rw-r--r--   0        0        0      568 2024-05-01 07:13:05.626149 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/configuration/__init__.py
+-rw-r--r--   0        0        0     2194 2024-05-01 07:13:05.627768 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/configuration/core.py
+-rw-r--r--   0        0        0      255 2024-05-01 07:13:05.630437 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/parsing/__init__.py
+-rw-r--r--   0        0        0      751 2024-02-09 08:50:51.444767 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/parsing/core.py
+-rw-r--r--   0        0        0     2156 2024-02-09 08:50:51.445237 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/parsing/rewrite.py
+-rw-r--r--   0        0        0        0 2024-02-09 08:50:51.445339 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/pdm/__init__.py
+-rw-r--r--   0        0        0     1154 2024-05-01 07:13:05.633175 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/pdm/core.py
+-rw-r--r--   0        0        0        0 2024-02-09 08:50:51.445849 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/pdm/hooks/__init__.py
+-rw-r--r--   0        0        0      643 2024-05-01 07:13:05.633555 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/pdm/hooks/bricks.py
+-rw-r--r--   0        0        0     1022 2024-05-01 07:13:05.634363 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/pdm/hooks/workspace.py
+-rw-r--r--   0        0        0        0 2024-02-09 08:50:51.428428 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/pdm_workspace_hooks/__init__.py
+-rw-r--r--   0        0        0      465 2024-05-01 07:13:05.630250 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/pdm_workspace_hooks/core.py
+-rw-r--r--   0        0        0      545 2024-05-01 07:13:05.631513 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/repo/__init__.py
+-rw-r--r--   0        0        0      862 2024-05-01 07:13:05.632494 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/repo/get.py
+-rw-r--r--   0        0        0     1964 2024-02-09 08:50:51.451835 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/repo/repo.py
+-rw-r--r--   0        0        0      467 2024-05-01 07:13:05.628052 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/toml/__init__.py
+-rw-r--r--   0        0        0     3254 2024-05-01 07:13:05.629877 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/toml/core.py
+-rw-r--r--   0        0        0      641 2024-05-01 07:13:05.625646 pdm_polylith_workspace-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1694 1970-01-01 00:00:00.000000 pdm_polylith_workspace-1.0.2/PKG-INFO
```

### Comparing `pdm_polylith_workspace-1.0.1/README.md` & `pdm_polylith_workspace-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/configuration/__init__.py` & `pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/configuration/core.py` & `pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/configuration/core.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/parsing/core.py` & `pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/parsing/core.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/parsing/rewrite.py` & `pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/parsing/rewrite.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/pdm/core.py` & `pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/pdm/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 def get_work_dir(config: dict) -> Path:
     build_config = config.get('tool', {}).get('pdm', {}).get('build', {})
     work_dir = build_config.get('work-dir', '.polylith_tmp')
     return Path(work_dir)
 
 def copy_bricks_as_is(bricks: dict, build_dir: Path) -> None:
-    for source, brick in bricks.items():
+    for (source, brick) in bricks.items():
         parsing.copy_brick(source, brick, build_dir)
 
 def copy_and_rewrite_bricks(bricks: dict, top_ns: str, work_dir: Path, build_dir: Path) -> None:
     ns = parsing.parse_brick_namespace_from_path(bricks)
-    for source, brick in bricks.items():
+    for (source, brick) in bricks.items():
         path = parsing.copy_brick(source, brick, work_dir)
         rewritten_bricks = parsing.rewrite_modules(path, ns, top_ns)
         destination_dir = build_dir / top_ns
         parsing.copy_brick(path.as_posix(), brick, destination_dir)
         for item in rewritten_bricks:
             print(f'Updated {item} with new top namespace for local imports.')
```

### Comparing `pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/pdm/hooks/bricks.py` & `pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/pdm/hooks/bricks.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/pdm/hooks/workspace.py` & `pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/pdm/hooks/workspace.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/repo/__init__.py` & `pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/repo/get.py` & `pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/repo/get.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/repo/repo.py` & `pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/repo/repo.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.1/pdm_polylith_workspace/polylith/toml/core.py` & `pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/toml/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from functools import reduce
 from pathlib import Path
 from typing import List, Union
 import tomlkit
 from pdm_polylith_workspace.polylith import repo
 
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

### Comparing `pdm_polylith_workspace-1.0.1/pyproject.toml` & `pdm_polylith_workspace-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdm-polylith-workspace"
-version = "1.0.1"
+version = "1.0.2"
 description = "a PDM build hook for a Polylith workspace"
 homepage = "https://davidvujic.github.io/python-polylith-docs/"
 repository = "https://github.com/davidvujic/python-polylith"
 authors = ["David Vujic"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `pdm_polylith_workspace-1.0.1/PKG-INFO` & `pdm_polylith_workspace-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-polylith-workspace
-Version: 1.0.1
+Version: 1.0.2
 Summary: a PDM build hook for a Polylith workspace
 Home-page: https://davidvujic.github.io/python-polylith-docs/
 License: MIT
 Author: David Vujic
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


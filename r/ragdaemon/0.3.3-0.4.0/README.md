# Comparing `tmp/ragdaemon-0.3.3.tar.gz` & `tmp/ragdaemon-0.4.0.tar.gz`

## Comparing `ragdaemon-0.3.3.tar` & `ragdaemon-0.4.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0    13397 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/scratch.ipynb
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/tutorial.ipynb
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/__main__.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/app.py
--rw-r--r--   0        0        0    10163 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/context.py
--rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/errors.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/get_paths.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/graph.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/llm.py
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/utils.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0     8803 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/annotators/chunker.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/annotators/chunker_line.py
--rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/annotators/chunker_llm.py
--rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/annotators/summarizer.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/database/database.py
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/prompts/chunker_llm.toml
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/tests/conftest.py
--rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/tests/test_comments.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/tests/test_context.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/tests/test_daemon.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/tests/test_database.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/tests/test_get_paths.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/tests/test_sample.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/tests/annotators/test_chunker_llm.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/tests/annotators/test_summarizer.py
--rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/tests/data/context_message.txt
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/tests/data/diff_graph.json
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/tests/data/hard_to_chunk.txt
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/README.md
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0    13397 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/scratch.ipynb
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tutorial.ipynb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/app.py
+-rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/context.py
+-rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/errors.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/get_paths.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/graph.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/llm.py
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/utils.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0     8839 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/annotators/chunker.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/annotators/chunker_line.py
+-rw-r--r--   0        0        0     6645 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/annotators/chunker_llm.py
+-rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/annotators/summarizer.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/prompts/chunker_llm.toml
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/test_comments.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/test_context.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/test_daemon.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/test_database.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/test_get_paths.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/test_sample.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/annotators/test_chunker_llm.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/annotators/test_summarizer.py
+-rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/data/context_message.txt
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/data/hard_to_chunk.txt
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/README.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/PKG-INFO
```

### Comparing `ragdaemon-0.3.3/scratch.ipynb` & `ragdaemon-0.4.0/scratch.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/tutorial.ipynb` & `ragdaemon-0.4.0/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/.github/workflows/run-tests.yml` & `ragdaemon-0.4.0/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/ragdaemon/app.py` & `ragdaemon-0.4.0/ragdaemon/app.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/ragdaemon/context.py` & `ragdaemon-0.4.0/ragdaemon/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from copy import deepcopy
 from pathlib import Path
 from typing import Any, Dict, Optional, Union
 
 from dict2xml import dict2xml
 from ragdaemon.annotators.diff import parse_diff_id
 from ragdaemon.database import Database
+from ragdaemon.errors import RagdaemonError
 from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.utils import get_document, hash_str, parse_path_ref
 
 NestedStrDict = Union[str, Dict[str, "NestedStrDict"]]
 
 
 class Comment:
@@ -102,15 +103,15 @@
         path, lines = parse_path_ref(path_ref)
         path_str = path.as_posix()
         if path_str not in self.context:
             self._add_path(path_str)
         self.context[path_str]["tags"].update(tags)
         if not lines:
             document = self.context[path_str]["document"]
-            lines = list(range(1, len(document.splitlines())))
+            lines = list(range(1, len(document.split("\n"))))
         self.context[path_str]["lines"].update(lines)
 
     def add_diff(self, id: str):
         """Take a diff id and add to context"""
         _, path, _ = parse_diff_id(id)
         if not path:  # e.g. diff 'parent' nodes
             return
@@ -202,19 +203,21 @@
                 output += f"<{path_str}>{tags}\n"
             else:
                 output += f"{path_str}{tags}\n"
 
             if 0 in data["comments"]:
                 output += render_comments(data["comments"][0]) + "\n"
             if data["lines"]:
-                file_lines = data["document"].splitlines()
+                file_lines = data["document"].split("\n")
                 last_rendered = 0
                 for line in sorted(data["lines"]):
                     if line - last_rendered > 1:
                         output += "...\n"
+                    if line >= len(file_lines):
+                        raise RagdaemonError(f"Line {line} not found in {path_str}.")
                     line_content = f"{line}:{file_lines[line]}"
                     if line in data["comments"]:
                         line_content += "\n" + render_comments(data["comments"][line])
                     output += line_content + "\n"
                     last_rendered = line
                 if last_rendered < len(file_lines) - 1:
                     output += "...\n"
@@ -231,25 +234,25 @@
         if diff_str != "DEFAULT":
             git_command += f" {diff_str}"
         output += f"{git_command}\n"
         for id in sorted(ids):
             checksum = self.graph.nodes[id]["checksum"]
             document = self.db.get(checksum)["documents"][0]
             # TODO: Add line numbers
-            without_git_command = "\n".join(document.splitlines()[1:])
+            without_git_command = "\n".join(document.split("\n")[1:])
             output += without_git_command + "\n"
         return output
 
     def to_refs(self) -> list[str]:
         """Return a list of path:interval,interval for everything in current context."""
         refs = dict[str, str]()
         for path, data in self.context.items():
             if len(data["lines"]) == 0:
                 continue
-            elif len(data["lines"]) == data["document"].splitlines():
+            elif len(data["lines"]) == data["document"].split("\n"):
                 refs[path] = ""
                 continue
             segments = []
             current_segment = ""
             last_line = 0
             for line in sorted(data["lines"]):
                 if current_segment and line - last_line > 1:
```

### Comparing `ragdaemon-0.3.3/ragdaemon/daemon.py` & `ragdaemon-0.4.0/ragdaemon/daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/ragdaemon/get_paths.py` & `ragdaemon-0.4.0/ragdaemon/get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/ragdaemon/graph.py` & `ragdaemon-0.4.0/ragdaemon/graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/ragdaemon/utils.py` & `ragdaemon-0.4.0/ragdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/ragdaemon/annotators/__init__.py` & `ragdaemon-0.4.0/ragdaemon/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.4.0/ragdaemon/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/ragdaemon/annotators/chunker.py` & `ragdaemon-0.4.0/ragdaemon/annotators/chunker.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,16 @@
         return add_to_db
 
     async def annotate(
         self, graph: KnowledgeGraph, db: Database, refresh: bool = False
     ) -> KnowledgeGraph:
         # Select file nodes and remove all existing chunk nodes from graph.
         files_with_chunks = []
-        for node, data in graph.nodes(data=True):
+        all_nodes = list(graph.nodes(data=True))
+        for node, data in all_nodes:
             if data is None:
                 raise RagdaemonError(f"Node {node} has no data.")
             if data.get("type") == "chunk":
                 graph.remove_node(node)
             elif data.get("type") == "file":
                 if self.chunk_extensions is None:
                     files_with_chunks.append(node)
```

### Comparing `ragdaemon-0.3.3/ragdaemon/annotators/chunker_line.py` & `ragdaemon-0.4.0/ragdaemon/annotators/chunker_line.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     chunk_field_id = "chunks_line"
 
     def __init__(self, *args, lines_per_chunk=50, **kwargs):
         super().__init__(*args, **kwargs)
         self.n = lines_per_chunk
 
     async def chunk_document(self, document: str) -> list[dict[str, Any]]:
-        lines = document.splitlines()
+        lines = document.split("\n")
         file = lines[0]
         file_lines = lines[1:]
         if not file_lines or not any(line for line in file_lines):
             return []
 
         chunks = list[dict[str, Any]]()
         if len(file_lines) > self.n:
```

### Comparing `ragdaemon-0.3.3/ragdaemon/annotators/chunker_llm.py` & `ragdaemon-0.4.0/ragdaemon/annotators/chunker_llm.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
                 )
         return chunks
 
     async def chunk_document(
         self, document: str, batch_size: int = 1000, retries: int = 1
     ) -> list[dict[str, Any]]:
         """Parse file_lines into a list of {id, ref} chunks."""
-        lines = document.splitlines()
+        lines = document.split("\n")
         file = lines[0]
         file_lines = lines[1:]
         if not file_lines or not any(line for line in file_lines):
             return []
         file_lines = [f"{i+1}:{line}" for i, line in enumerate(file_lines)]
 
         # Get raw llm output
```

### Comparing `ragdaemon-0.3.3/ragdaemon/annotators/diff.py` & `ragdaemon-0.4.0/ragdaemon/annotators/diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.4.0/ragdaemon/annotators/hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.4.0/ragdaemon/annotators/layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/ragdaemon/annotators/summarizer.py` & `ragdaemon-0.4.0/ragdaemon/annotators/summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/ragdaemon/database/__init__.py` & `ragdaemon-0.4.0/ragdaemon/database/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/ragdaemon/database/chroma_database.py` & `ragdaemon-0.4.0/ragdaemon/database/chroma_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/ragdaemon/database/database.py` & `ragdaemon-0.4.0/ragdaemon/database/database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/ragdaemon/database/lite_database.py` & `ragdaemon-0.4.0/ragdaemon/database/lite_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/ragdaemon/prompts/chunker_llm.toml` & `ragdaemon-0.4.0/ragdaemon/prompts/chunker_llm.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/ragdaemon/static/favicon.ico` & `ragdaemon-0.4.0/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.4.0/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/ragdaemon/static/js/main.js` & `ragdaemon-0.4.0/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.4.0/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/ragdaemon/static/js/three/node.js` & `ragdaemon-0.4.0/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.4.0/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/ragdaemon/templates/index.html` & `ragdaemon-0.4.0/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/tests/conftest.py` & `ragdaemon-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/tests/test_comments.py` & `ragdaemon-0.4.0/tests/test_comments.py`

 * *Files 10% similar despite different names*

```diff
@@ -72,14 +72,15 @@
             <author>bot</author>
             <content>hello</content>
             <replies>
                 <author>replier</author>
                 <content>Look replies are easy!</content>
             </replies>
             21:    return math.sqrt(a)
+            22:
             """)
     context.remove_comments("src/operations.py", tags=["test-flag"])
     actual = context.render()
     assert actual == dedent("""\
             src/operations.py
 
             1:import math
@@ -114,14 +115,15 @@
             <author>bot</author>
             <content>hello</content>
             <replies>
                 <author>replier</author>
                 <content>Look replies are easy!</content>
             </replies>
             21:    return math.sqrt(a)
+            22:
             """)
     context.remove_comments("src/operations.py")
     actual = context.render()
     assert actual == dedent("""\
             src/operations.py
             1:import math
             2: #modified
@@ -140,8 +142,9 @@
             15:
             16:def divide(a, b):
             17:    return a / b
             18:
             19:
             20:def sqrt(a):
             21:    return math.sqrt(a)
+            22:
             """)
```

### Comparing `ragdaemon-0.3.3/tests/test_context.py` & `ragdaemon-0.4.0/tests/test_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
     different_context = daemon.get_context("")
     different_context.add_ref("src/interface.py:17")
     different_context.add_ref("src/operations.py")
     combined_context = context + different_context
 
     assert combined_context.context["src/interface.py"]["lines"] == set([3, 4, 5, 17])
-    assert combined_context.context["src/operations.py"]["lines"] == set(range(1, 22))
+    assert combined_context.context["src/operations.py"]["lines"] == set(range(1, 23))
 
 
 def test_to_refs(cwd, mock_db):
     path_str = Path("src/interface.py").as_posix()
     ref = path_str
 
     # Setup Context
```

### Comparing `ragdaemon-0.3.3/tests/test_daemon.py` & `ragdaemon-0.4.0/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/tests/test_get_paths.py` & `ragdaemon-0.4.0/tests/test_get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/tests/test_sample.py` & `ragdaemon-0.4.0/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/tests/annotators/test_chunker.py` & `ragdaemon-0.4.0/tests/annotators/test_chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/tests/annotators/test_chunker_llm.py` & `ragdaemon-0.4.0/tests/annotators/test_chunker_llm.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ragdaemon.annotators.chunker_llm import ChunkerLLM
 from ragdaemon.daemon import Daemon
 
 
 @pytest.fixture
 def expected_chunks():
     return [
-        {"id": "src/calculator.py:BASE", "ref": "src/calculator.py:1-4,29,42-44"},
+        {"id": "src/calculator.py:BASE", "ref": "src/calculator.py:1-4,29,42-45"},
         {"id": "src/calculator.py:Calculator", "ref": "src/calculator.py:5-28"},
         {"id": "src/calculator.py:Calculator.__init__", "ref": "src/calculator.py:6-9"},
         {
             "id": "src/calculator.py:Calculator.add_numbers",
             "ref": "src/calculator.py:11-12",
         },
         {
```

### Comparing `ragdaemon-0.3.3/tests/annotators/test_diff.py` & `ragdaemon-0.4.0/tests/annotators/test_diff.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,15 @@
 +def add(a, b): #modified
      return a + b
 @@ -8,3 +8,3 @@ def add(a, b):
  def subtract(a, b):
 -    return a - b
 +return a - b #modified
  
+
 """
     )
 
     # Diffs with files and chunks
     context.remove_diff("DEFAULT:main.py")
     context.add_diff("DEFAULT:src/operations.py:1-5")
     context.add_ref("src/operations.py", tags=["user-included"])
@@ -139,14 +140,15 @@
 15:
 16:def divide(a, b):
 17:    return a / b
 18:
 19:
 20:def sqrt(a):
 21:    return math.sqrt(a)
+22:
 --git diff
 @@ -1,5 +1,5 @@
  import math
 -
 -
 -def add(a, b):
 + #modified
@@ -154,9 +156,10 @@
 +def add(a, b): #modified
      return a + b
 @@ -8,3 +8,3 @@ def add(a, b):
  def subtract(a, b):
 -    return a - b
 +return a - b #modified
  
+
 """
     )
```

### Comparing `ragdaemon-0.3.3/tests/annotators/test_hierarchy.py` & `ragdaemon-0.4.0/tests/annotators/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.4.0/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/tests/annotators/test_summarizer.py` & `ragdaemon-0.4.0/tests/annotators/test_summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/tests/data/chunker_graph.json` & `ragdaemon-0.4.0/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/tests/data/context_message.txt` & `ragdaemon-0.4.0/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/tests/data/diff_graph.json` & `ragdaemon-0.4.0/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/tests/data/hard_to_chunk.txt` & `ragdaemon-0.4.0/tests/data/hard_to_chunk.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/tests/data/hierarchy_graph.json` & `ragdaemon-0.4.0/tests/data/hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.4.0/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/tests/sample/src/interface.py` & `ragdaemon-0.4.0/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/LICENSE` & `ragdaemon-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/README.md` & `ragdaemon-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.3.3/pyproject.toml` & `ragdaemon-0.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.3.3"
+version = "0.4.0"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "chromadb==0.4.24",
     "dict2xml==1.7.5",
     "fastapi==0.109.2",
     "Jinja2==3.1.3",
```

### Comparing `ragdaemon-0.3.3/PKG-INFO` & `ragdaemon-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.3.3
+Version: 0.4.0
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```


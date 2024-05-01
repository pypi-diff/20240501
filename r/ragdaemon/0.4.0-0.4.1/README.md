# Comparing `tmp/ragdaemon-0.4.0.tar.gz` & `tmp/ragdaemon-0.4.1.tar.gz`

## Comparing `ragdaemon-0.4.0.tar` & `ragdaemon-0.4.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0    13397 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/scratch.ipynb
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tutorial.ipynb
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/__main__.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/app.py
--rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/context.py
--rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/errors.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/get_paths.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/graph.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/llm.py
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/utils.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0     8839 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/annotators/chunker.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/annotators/chunker_line.py
--rw-r--r--   0        0        0     6645 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/annotators/chunker_llm.py
--rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/annotators/summarizer.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/database/database.py
--rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/prompts/chunker_llm.toml
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/test_comments.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/test_context.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/test_daemon.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/test_database.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/test_get_paths.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/test_sample.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/annotators/test_chunker_llm.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/annotators/test_summarizer.py
--rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/data/context_message.txt
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/data/diff_graph.json
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/data/hard_to_chunk.txt
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/README.md
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    13397 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/scratch.ipynb
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tutorial.ipynb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/app.py
+-rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/context.py
+-rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/errors.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/get_paths.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/graph.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/llm.py
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/utils.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0     8839 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/annotators/chunker.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/annotators/chunker_line.py
+-rw-r--r--   0        0        0     6345 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/annotators/chunker_llm.py
+-rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/annotators/summarizer.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     3193 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/prompts/chunker_llm.toml
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/conftest.py
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/test_comments.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/test_context.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/test_daemon.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/test_database.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/test_get_paths.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/test_sample.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/annotators/test_chunker_llm.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/annotators/test_summarizer.py
+-rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/data/context_message.txt
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/data/hard_to_chunk.txt
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/README.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.4.1/PKG-INFO
```

### Comparing `ragdaemon-0.4.0/scratch.ipynb` & `ragdaemon-0.4.1/scratch.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/tutorial.ipynb` & `ragdaemon-0.4.1/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/.github/workflows/run-tests.yml` & `ragdaemon-0.4.1/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/ragdaemon/app.py` & `ragdaemon-0.4.1/ragdaemon/app.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/ragdaemon/context.py` & `ragdaemon-0.4.1/ragdaemon/context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/ragdaemon/daemon.py` & `ragdaemon-0.4.1/ragdaemon/daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/ragdaemon/get_paths.py` & `ragdaemon-0.4.1/ragdaemon/get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/ragdaemon/graph.py` & `ragdaemon-0.4.1/ragdaemon/graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/ragdaemon/utils.py` & `ragdaemon-0.4.1/ragdaemon/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -105,7 +105,29 @@
         document = document[: int(len(document) * truncate_ratio)]
         tokens = Spice().count_tokens(document, model=spice_model.name)
     truncate_ratio = 1 - tokens / original_tokens
     if truncate_ratio > 0:
         label = "\n[TRUNCATED]"
         document = document[: -len(label)] + label
     return document, truncate_ratio
+
+
+def lines_set_to_ref(lines: set[int]) -> str:
+    if not lines:
+        return ""
+    refs = []
+    low_to_high = sorted(lines)
+    start = end = low_to_high[0]
+    for i in low_to_high[1:]:
+        if i == end + 1:
+            end = i
+        else:
+            if start == end:
+                refs.append(str(start))
+            else:
+                refs.append(f"{start}-{end}")
+            start = end = i
+    if start == end:
+        refs.append(str(start))
+    else:
+        refs.append(f"{start}-{end}")
+    return ",".join(refs)
```

### Comparing `ragdaemon-0.4.0/ragdaemon/annotators/__init__.py` & `ragdaemon-0.4.1/ragdaemon/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.4.1/ragdaemon/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/ragdaemon/annotators/chunker.py` & `ragdaemon-0.4.1/ragdaemon/annotators/chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/ragdaemon/annotators/chunker_line.py` & `ragdaemon-0.4.1/ragdaemon/annotators/chunker_line.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/ragdaemon/annotators/chunker_llm.py` & `ragdaemon-0.4.1/ragdaemon/annotators/chunker_llm.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from json.decoder import JSONDecodeError
 from typing import Any, Dict, List, Optional
 
 from spice import SpiceMessages
 
 from ragdaemon.annotators.chunker import Chunker
 from ragdaemon.errors import RagdaemonError
+from ragdaemon.utils import lines_set_to_ref
 
 
 def is_chunk_valid(chunk: dict, last_valid_line: int):
     if not set(chunk.keys()) == {"id", "start_line", "end_line"}:
         raise RagdaemonError(f"Chunk is missing fields: {chunk}")
     halves = chunk["id"].split(":")
     if len(halves) != 2 or not halves[0] or not halves[1]:
@@ -86,15 +87,15 @@
         lines = document.split("\n")
         file = lines[0]
         file_lines = lines[1:]
         if not file_lines or not any(line for line in file_lines):
             return []
         file_lines = [f"{i+1}:{line}" for i, line in enumerate(file_lines)]
 
-        # Get raw llm output
+        # Get raw llm output: {id, start_line, end_line}
         chunks = list[dict[str, Any]]()
         n_batches = (len(file_lines) + batch_size - 1) // batch_size
         for i in range(n_batches):
             batch_lines = file_lines[i * batch_size : (i + 1) * batch_size]
             last_chunk = chunks.pop() if chunks else None
             for j in range(retries + 1, 0, -1):
                 try:
@@ -108,53 +109,45 @@
                             + f"{j-1} retries left."
                             if j > 1
                             else "Skipping."
                         )
                     if j == 1:
                         return []
 
-        # Make sure end_line of each 'parent' chunk covers all children
-        def update_end_lines(id: str, _chunks: list[dict[str, Any]]):
-            child_chunks = [c for c in _chunks if c["id"].startswith(id + ".")]
+        # Convert to {id: set(lines)} for easier manipulation
+        chunks = {
+            c["id"]: set(range(c["start_line"], c["end_line"] + 1)) for c in chunks
+        }
+
+        def update_parent_nodes(id: str, _chunks: dict[str, set[int]]):
+            parent_lines = _chunks[id]
+            child_chunks = {k: v for k, v in _chunks.items() if k.startswith(id + ".")}
             if child_chunks:
-                end_line = max(c["end_line"] for c in child_chunks)
-                parent_chunk = next(c for c in _chunks if c["id"] == id)
-                parent_chunk["end_line"] = end_line
+                # Make sure end_line of each 'parent' chunk covers all children
+                start_line = min(parent_lines)
+                end_line = max(max(v) for v in child_chunks.values())
+                parent_lines = set(range(start_line, end_line + 1))
+                # Remove child lines from parent lines
+                for child_lines in child_chunks.values():
+                    parent_lines -= child_lines
+                _chunks[id] = parent_lines
             return _chunks
 
-        for chunk in sorted(chunks, key=lambda c: len(c["id"]), reverse=True):
-            chunks = update_end_lines(chunk["id"], chunks)
+        ids_longest_first = sorted(chunks, key=lambda x: len(x), reverse=True)
+        for id in ids_longest_first:
+            chunks = update_parent_nodes(id, chunks)
 
         # Generate a 'BASE chunk' with all lines not already part of a chunk
         base_chunk_lines = set(range(1, len(file_lines) + 1))
-        for chunk in chunks:
-            for i in range(int(chunk["start_line"]), int(chunk["end_line"]) + 1):
-                base_chunk_lines.discard(i)
-        if len(base_chunk_lines) > 0:
-            base_chunk_lines_sorted = sorted(list(base_chunk_lines))
-            base_chunk_refs = []
-            start = base_chunk_lines_sorted[0]
-            end = start
-            for i in base_chunk_lines_sorted[1:]:
-                if i == end + 1:
-                    end = i
-                else:
-                    if start == end:
-                        base_chunk_refs.append(f"{start}")
-                    else:
-                        base_chunk_refs.append(f"{start}-{end}")
-                    start = end = i
-            base_chunk_refs.append(f"{start}-{end}")
-        else:
-            base_chunk_refs = []
-        lines_str = ":" + ",".join(base_chunk_refs) if base_chunk_refs else ""
-        base_chunk = {"id": f"{file}:BASE", "ref": f"{file}{lines_str}"}
+        for lines in chunks.values():
+            base_chunk_lines -= lines
+        lines_ref = lines_set_to_ref(base_chunk_lines)
+        ref = f"{file}:{lines_ref}" if lines_ref else file
+        base_chunk = {"id": f"{file}:BASE", "ref": ref}
 
         # Convert to refs and return
         output = [base_chunk]
-        for chunk in chunks:
-            if chunk["start_line"] == chunk["end_line"]:
-                lines_str = str(chunk["start_line"])
-            else:
-                lines_str = f"{chunk['start_line']}-{chunk['end_line']}"
-            output.append({"id": chunk["id"], "ref": f"{file}:{lines_str}"})
+        for id, lines in chunks.items():
+            lines_ref = lines_set_to_ref(lines)
+            ref = f"{file}:{lines_ref}" if lines_ref else file
+            output.append({"id": id, "ref": ref})
         return output
```

### Comparing `ragdaemon-0.4.0/ragdaemon/annotators/diff.py` & `ragdaemon-0.4.1/ragdaemon/annotators/diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.4.1/ragdaemon/annotators/hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.4.1/ragdaemon/annotators/layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/ragdaemon/annotators/summarizer.py` & `ragdaemon-0.4.1/ragdaemon/annotators/summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/ragdaemon/database/__init__.py` & `ragdaemon-0.4.1/ragdaemon/database/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/ragdaemon/database/chroma_database.py` & `ragdaemon-0.4.1/ragdaemon/database/chroma_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/ragdaemon/database/database.py` & `ragdaemon-0.4.1/ragdaemon/database/database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/ragdaemon/database/lite_database.py` & `ragdaemon-0.4.1/ragdaemon/database/lite_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/ragdaemon/prompts/chunker_llm.toml` & `ragdaemon-0.4.1/ragdaemon/prompts/chunker_llm.toml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/ragdaemon/static/favicon.ico` & `ragdaemon-0.4.1/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.4.1/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/ragdaemon/static/js/main.js` & `ragdaemon-0.4.1/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.4.1/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/ragdaemon/static/js/three/node.js` & `ragdaemon-0.4.1/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.4.1/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/ragdaemon/templates/index.html` & `ragdaemon-0.4.1/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/tests/conftest.py` & `ragdaemon-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/tests/test_comments.py` & `ragdaemon-0.4.1/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/tests/test_context.py` & `ragdaemon-0.4.1/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/tests/test_daemon.py` & `ragdaemon-0.4.1/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/tests/test_get_paths.py` & `ragdaemon-0.4.1/tests/test_get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/tests/test_sample.py` & `ragdaemon-0.4.1/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/tests/annotators/test_chunker.py` & `ragdaemon-0.4.1/tests/annotators/test_chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/tests/annotators/test_chunker_llm.py` & `ragdaemon-0.4.1/tests/annotators/test_chunker_llm.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 from ragdaemon.daemon import Daemon
 
 
 @pytest.fixture
 def expected_chunks():
     return [
         {"id": "src/calculator.py:BASE", "ref": "src/calculator.py:1-4,29,42-45"},
-        {"id": "src/calculator.py:Calculator", "ref": "src/calculator.py:5-28"},
+        {
+            "id": "src/calculator.py:Calculator",
+            "ref": "src/calculator.py:5,10,13,16,19",
+        },
         {"id": "src/calculator.py:Calculator.__init__", "ref": "src/calculator.py:6-9"},
         {
             "id": "src/calculator.py:Calculator.add_numbers",
             "ref": "src/calculator.py:11-12",
         },
         {
             "id": "src/calculator.py:Calculator.subtract_numbers",
@@ -25,14 +28,27 @@
             "ref": "src/calculator.py:17-18",
         },
         {"id": "src/calculator.py:Calculator.call", "ref": "src/calculator.py:20-28"},
         {"id": "src/calculator.py:main", "ref": "src/calculator.py:30-41"},
     ]
 
 
+"""
+
+{'id': 'src/calculator.py:BASE', 'ref': 'src/calculator.py:1-4,19,29,42-44'}, 
+{'id': 'src/calculator.py:Calculator', 'ref': 'src/calculator.py:5,10,13,16'}, 
+{'id': 'src/calculator.py:Calculator.__init__', 'ref': 'src/calculator.py:6-9'}, 
+{'id': 'src/calculator.py:Calculator.add_numbers', 'ref': 'src/calculator.py:11-12'}, 
+{'id': 'src/calculator.py:Calculator.subtract_numbers', 'ref': 'src/calculator.py:14-15'}, 
+{'id': 'src/calculator.py:Calculator.exp_numbers', 'ref': 'src/calculator.py:17-18'}, 
+{'id': 'src/calculator.py:call', 'ref': 'src/calculator.py:20-28'}, 
+{'id': 'src/calculator.py:main', 'ref': 'src/calculator.py:30-41'}
+"""
+
+
 @pytest.mark.skip(reason="This test requires calling an API")
 @pytest.mark.asyncio
 async def test_chunker_llm_edge_cases(cwd, expected_chunks):
     # NOTE: TO RUN THIS YOU HAVE TO COMMENT_OUT tests/conftest.py/mock_openai_api_key
     daemon = Daemon(cwd, annotators={"hierarchy": {}})
     chunker = ChunkerLLM(spice_client=daemon.spice_client)
 
@@ -40,12 +56,14 @@
     # - First batch ends mid-class, so second batch needs 'call path'
     # - Second batch ends mid-function, third batch needs to pickup where it left off
     # - Third batch is all inside one function, so needs to pass call forward.
     text = Path("tests/data/hard_to_chunk.txt").read_text()
     document = f"src/calculator.py\n{text}"
     actual_chunks = await chunker.chunk_document(document, batch_size=10)
 
+    print(actual_chunks)
+
     assert len(actual_chunks) == len(expected_chunks)
     actual_chunks = sorted(actual_chunks, key=lambda x: x["ref"])
     expected_chunks = sorted(expected_chunks, key=lambda x: x["ref"])
     for actual, expected in zip(actual_chunks, expected_chunks):
         assert actual == expected
```

### Comparing `ragdaemon-0.4.0/tests/annotators/test_diff.py` & `ragdaemon-0.4.1/tests/annotators/test_diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/tests/annotators/test_hierarchy.py` & `ragdaemon-0.4.1/tests/annotators/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.4.1/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/tests/annotators/test_summarizer.py` & `ragdaemon-0.4.1/tests/annotators/test_summarizer.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/tests/data/chunker_graph.json` & `ragdaemon-0.4.1/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/tests/data/context_message.txt` & `ragdaemon-0.4.1/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/tests/data/diff_graph.json` & `ragdaemon-0.4.1/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/tests/data/hard_to_chunk.txt` & `ragdaemon-0.4.1/tests/data/hard_to_chunk.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/tests/data/hierarchy_graph.json` & `ragdaemon-0.4.1/tests/data/hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.4.1/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/tests/sample/src/interface.py` & `ragdaemon-0.4.1/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/LICENSE` & `ragdaemon-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/README.md` & `ragdaemon-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.4.0/pyproject.toml` & `ragdaemon-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.4.0"
+version = "0.4.1"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "chromadb==0.4.24",
     "dict2xml==1.7.5",
     "fastapi==0.109.2",
     "Jinja2==3.1.3",
```

### Comparing `ragdaemon-0.4.0/PKG-INFO` & `ragdaemon-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.4.0
+Version: 0.4.1
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```


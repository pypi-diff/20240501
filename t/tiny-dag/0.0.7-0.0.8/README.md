# Comparing `tmp/tiny_dag-0.0.7.tar.gz` & `tmp/tiny_dag-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiny_dag-0.0.7.tar", last modified: Tue Apr 30 05:36:29 2024, max compression
+gzip compressed data, was "tiny_dag-0.0.8.tar", last modified: Wed May  1 10:19:54 2024, max compression
```

## Comparing `tiny_dag-0.0.7.tar` & `tiny_dag-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-30 05:36:29.989566 tiny_dag-0.0.7/
--rw-rw-r--   0 ossi      (1000) ossi      (1000)     1072 2024-04-27 07:53:55.000000 tiny_dag-0.0.7/LICENSE
--rw-r--r--   0 ossi      (1000) ossi      (1000)     1638 2024-04-30 05:36:29.989566 tiny_dag-0.0.7/PKG-INFO
--rw-rw-r--   0 ossi      (1000) ossi      (1000)     1100 2024-04-29 14:48:03.000000 tiny_dag-0.0.7/README.md
--rw-rw-r--   0 ossi      (1000) ossi      (1000)      104 2024-04-27 09:26:48.000000 tiny_dag-0.0.7/pyproject.toml
--rw-rw-r--   0 ossi      (1000) ossi      (1000)      668 2024-04-30 05:36:29.989566 tiny_dag-0.0.7/setup.cfg
-drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-30 05:36:29.989566 tiny_dag-0.0.7/src/
-drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-30 05:36:29.989566 tiny_dag-0.0.7/src/tiny_dag.egg-info/
--rw-r--r--   0 ossi      (1000) ossi      (1000)     1638 2024-04-30 05:36:29.000000 tiny_dag-0.0.7/src/tiny_dag.egg-info/PKG-INFO
--rw-rw-r--   0 ossi      (1000) ossi      (1000)      312 2024-04-30 05:36:29.000000 tiny_dag-0.0.7/src/tiny_dag.egg-info/SOURCES.txt
--rw-rw-r--   0 ossi      (1000) ossi      (1000)        1 2024-04-30 05:36:29.000000 tiny_dag-0.0.7/src/tiny_dag.egg-info/dependency_links.txt
--rw-rw-r--   0 ossi      (1000) ossi      (1000)        9 2024-04-30 05:36:29.000000 tiny_dag-0.0.7/src/tiny_dag.egg-info/requires.txt
--rw-rw-r--   0 ossi      (1000) ossi      (1000)        8 2024-04-30 05:36:29.000000 tiny_dag-0.0.7/src/tiny_dag.egg-info/top_level.txt
-drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-30 05:36:29.989566 tiny_dag-0.0.7/src/tinydag/
--rw-rw-r--   0 ossi      (1000) ossi      (1000)        0 2024-04-27 07:53:55.000000 tiny_dag-0.0.7/src/tinydag/__init__.py
--rw-rw-r--   0 ossi      (1000) ossi      (1000)       92 2024-04-30 05:29:51.000000 tiny_dag-0.0.7/src/tinydag/exceptions.py
--rw-rw-r--   0 ossi      (1000) ossi      (1000)     7738 2024-04-30 00:57:56.000000 tiny_dag-0.0.7/src/tinydag/graph.py
--rw-rw-r--   0 ossi      (1000) ossi      (1000)     1526 2024-04-30 05:29:47.000000 tiny_dag-0.0.7/src/tinydag/node.py
+drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-05-01 10:19:54.055933 tiny_dag-0.0.8/
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)     1072 2024-04-27 07:53:55.000000 tiny_dag-0.0.8/LICENSE
+-rw-r--r--   0 ossi      (1000) ossi      (1000)     2683 2024-05-01 10:19:54.055933 tiny_dag-0.0.8/PKG-INFO
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)     2145 2024-05-01 10:18:21.000000 tiny_dag-0.0.8/README.md
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)      104 2024-04-27 09:26:48.000000 tiny_dag-0.0.8/pyproject.toml
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)      668 2024-05-01 10:19:54.055933 tiny_dag-0.0.8/setup.cfg
+drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-05-01 10:19:54.051933 tiny_dag-0.0.8/src/
+drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-05-01 10:19:54.055933 tiny_dag-0.0.8/src/tiny_dag.egg-info/
+-rw-r--r--   0 ossi      (1000) ossi      (1000)     2683 2024-05-01 10:19:54.000000 tiny_dag-0.0.8/src/tiny_dag.egg-info/PKG-INFO
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)      312 2024-05-01 10:19:54.000000 tiny_dag-0.0.8/src/tiny_dag.egg-info/SOURCES.txt
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)        1 2024-05-01 10:19:54.000000 tiny_dag-0.0.8/src/tiny_dag.egg-info/dependency_links.txt
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)        9 2024-05-01 10:19:54.000000 tiny_dag-0.0.8/src/tiny_dag.egg-info/requires.txt
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)        8 2024-05-01 10:19:54.000000 tiny_dag-0.0.8/src/tiny_dag.egg-info/top_level.txt
+drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-05-01 10:19:54.055933 tiny_dag-0.0.8/src/tinydag/
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)        0 2024-04-27 07:53:55.000000 tiny_dag-0.0.8/src/tinydag/__init__.py
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)      147 2024-05-01 10:15:23.000000 tiny_dag-0.0.8/src/tinydag/exceptions.py
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)     9709 2024-05-01 10:15:23.000000 tiny_dag-0.0.8/src/tinydag/graph.py
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)     1522 2024-05-01 10:15:23.000000 tiny_dag-0.0.8/src/tinydag/node.py
```

### Comparing `tiny_dag-0.0.7/LICENSE` & `tiny_dag-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tiny_dag-0.0.7/setup.cfg` & `tiny_dag-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tiny-dag
-version = 0.0.7
+version = 0.0.8
 author = Ossi Myllymäki
 author_email = omyllymaki@gmail.com
 description = Minimal DAG implementation with Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/omyllymaki/tiny-dag
 project_urls =
```

### Comparing `tiny_dag-0.0.7/src/tinydag/graph.py` & `tiny_dag-0.0.8/src/tinydag/graph.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import time
 from copy import copy
 from typing import List, Callable, Union, Optional, Any
 
-from tinydag.exceptions import InvalidGraphError, MissingInputError
+from tinydag.exceptions import InvalidGraphError, MissingInputError, InvalidNodeFunctionOutput
 from tinydag.node import Node
 
 logger = logging.getLogger(__name__)
 
 try:
     import graphviz as graphviz
     from graphviz import Digraph
@@ -21,31 +21,35 @@
 
     User provides the graph structure (nodes) and input data for the graph. Every node waits until input data for that
     node is ready. Eventually, the graph executes every node in the graph and returns output of every node as the
     result.
 
     Example:
 
-    add = lambda a, b: a + b
-    mul = lambda a, b: a * b
-    div = lambda a, b: a / b
+    def add(a, b): return {"output": a + b}
+    def mul(a, b): return {"output": a * b}
+    def div(a, b): return {"output": a / b}
+    def add_subtract(a, b): return {"add_output": a + b, "subtract_output": a - b}
 
     nodes = [
-        Node(["add1", "x"], add, "add2"),
-        Node(["add1", "add2"], mul, "mul"),
-        Node(["x", "y"], add, "add1"),
-        Node(["mul", "z"], div, "div"),
+        Node(["add1/output", "x"], add, "add2", ["output"]),
+        Node(["add1/output", "add2/output"], mul, "mul", ["output"]),
+        Node(["x", "y"], add, "add1", ["output"]),
+        Node(["x", "z"], add_subtract, "add_subtract", ["add_output", "subtract_output"]),
+        Node(["mul/output", "add_subtract/add_output"], div, "div", ["output"]),
     ]
+    graph = Graph(nodes)
 
-    where add, mul and div are functions. This determines the graph where
+    Defines a graph with following connections:
 
-    x,y -> add1
-    add1,x -> add2
-    add1,add2 -> mul
-    mul,z -> div
+    x, y -> add1
+    x, z -> add_subtract
+    add1/output, x -> add2
+    add1/output, add2/output -> mul
+    mul/output, add_subtract/add_output -> div
 
     User needs to provide x, y and z as input data for this graph when doing calculation.
     """
 
     def __init__(self,
                  nodes: List[Node],
                  wrappers: Optional[List[Callable]] = None) -> None:
@@ -56,37 +60,43 @@
         """
         self._check_node_names_are_unique(nodes)
         self.nodes = nodes
         self.wrappers = wrappers
         self.required_user_inputs = self._get_required_user_inputs()
         logger.debug(f"Required user input: {self.required_user_inputs}")
 
-    def _get_required_user_inputs(self):
-        node_output_names = [node.output_name for node in self.nodes]
-        required_inputs = []
+    def _get_required_user_inputs(self) -> List[str]:
+        required_inputs, node_outputs = [], []
         for node in self.nodes:
             required_inputs += node.inputs
-        return list(set(required_inputs) - set(node_output_names))
+            node_outputs += node.outputs
+        return list(set(required_inputs) - set(node_outputs))
 
     def render(self,
                path: str = "graph.gv",
                view: bool = True) -> Optional["Digraph"]:
         """
         Render graph. This will only work if graphviz is available.
         :param path: Path to save fig.
         :param view: Show graph fig.
         :return: graphviz Digraph is graphviz is available, otherwise None.
         """
 
         try:
             dot = graphviz.Digraph()
             for node in self.nodes:
-                dot.node(node.name, node.name)
-            for node in self.nodes:
+                dot.node(node.name, node.name, shape='box', style='filled', fillcolor='lightblue')
+                for output in node.outputs:
+                    dot.node(output, output, shape='oval', style='filled', fillcolor='lightgreen')
+                    dot.edge(node.name, output)
                 for node_input in node.inputs:
+                    if node_input in self.required_user_inputs:
+                        dot.node(node_input, node_input, shape='ellipse', style='filled', fillcolor='lightpink')
+                    else:
+                        dot.node(node_input, node_input, shape='oval', style='filled', fillcolor='lightgreen')
                     dot.edge(node_input, node.name)
             dot.render(path, view=view)
             return dot
         except Exception as e:
             logger.warning(f"Graph cannot be rendered, caught error: {e}")
             return None
 
@@ -131,16 +141,23 @@
             nodes_executed = []
             for node_index in nodes_to_execute:
                 node = self.nodes[node_index]
                 logger.debug(f"Executing node {node}")
                 node_input_data = self._get_node_input_data(node, inputs)
                 if len(node_input_data) < len(node.inputs):
                     continue  # All the input data cannot be found for this node yet, so skip this node
-                output = self._run_node(node, node_input_data) if run else "output"
-                inputs[node.output_name] = output
+                if run:
+                    results = self._run_node(node, node_input_data)
+                    self._check_node_output(results, node)
+                    if results is not None:
+                        for key, val in results.items():
+                            inputs[node.name + "/" + key] = val
+                else:
+                    for output in node.outputs:
+                        inputs[output] = None
                 nodes_executed.append(node_index)
                 logger.debug(f"Node {node} executed successfully")
 
             # Check that at least one of the nodes has been executed during this round
             # If not, it means that the graph has invalid structure
             if len(nodes_executed) == 0:
                 raise InvalidGraphError("Graph cannot be executed! The graph has invalid structure.")
@@ -148,46 +165,64 @@
             for node_index in nodes_executed:
                 nodes_to_execute.remove(node_index)
 
         logger.debug("All nodes executed successfully")
         t_graph_end = time.time()
         logger.debug(f"Graph execution took {1000 * (t_graph_end - t_graph_start): 0.2f} ms")
 
-        # As a result we return node outputs
-        # We get this from inputs, by removing the original input data from the dict
-        results = inputs
-        if input_data is not None:
-            for key in input_data.keys():
-                results.pop(key)
+        results = {}
+        for node in self.nodes:
+            for output in node.outputs:
+                results[output] = inputs[output]
 
         return results
 
     def _run_node(self, node: Node, data: list) -> Any:
         func = self._wrap_node_func(node.function)
         t_node_start = time.time()
         output = func(*data)
         t_node_end = time.time()
         logger.debug(f"Node {node} execution took {1000 * (t_node_end - t_node_start): 0.3f} ms")
         return output
 
+    @staticmethod
+    def _check_node_output(output, node):
+        if output is not None:
+            if not isinstance(output, dict):
+                raise InvalidNodeFunctionOutput(f"Node {node.name} output is not a dict!")
+        for item in node.outputs:
+            item = item.replace(f"{node.name}/", "")
+            if item not in output:
+                raise InvalidNodeFunctionOutput(f"Node {node.name} output doesn't contain required item {item}!")
+
     def _wrap_node_func(self, func):
         if self.wrappers is not None:
             for wrapper in self.wrappers:
                 func = wrapper(func)
         return func
 
     def __add__(self, nodes: Union[List[Node], Node]) -> "Graph":
         if isinstance(nodes, list):
             nodes = self.nodes + nodes
         else:
             nodes = self.nodes + [nodes]
         return Graph(nodes, self.wrappers)
 
     def __repr__(self) -> str:
-        return str([n.name for n in self.nodes])
+        repr_str = "\n"
+        for node in self.nodes:
+            name = node.name
+            repr_str += f"Node: {name}\n"
+            repr_str += "├─ Inputs:\n"
+            for input_node in node.inputs:
+                repr_str += f"│  ├─ {input_node}\n"
+            repr_str += "└─ Outputs:\n"
+            for output_node in node.outputs:
+                repr_str += f"   ├─ {output_node}\n"
+        return repr_str
 
     @staticmethod
     def _check_node_names_are_unique(nodes: List[Node]) -> None:
         node_names = [n.name for n in nodes]
         if len(set(node_names)) < len(node_names):
             raise InvalidGraphError("All the nodes need to have unique name!")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


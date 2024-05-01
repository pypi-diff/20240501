# Comparing `tmp/fockstatecircuit-1.0.1.tar.gz` & `tmp/fockstatecircuit-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fockstatecircuit-1.0.1.tar", last modified: Fri Apr 19 06:21:15 2024, max compression
+gzip compressed data, was "fockstatecircuit-1.0.2.tar", last modified: Wed May  1 08:13:03 2024, max compression
```

## Comparing `fockstatecircuit-1.0.1.tar` & `fockstatecircuit-1.0.2.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 06:21:15.338576 fockstatecircuit-1.0.1/
--rw-rw-rw-   0        0        0     1069 2023-11-24 00:31:46.000000 fockstatecircuit-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0    16004 2024-04-19 06:21:15.337184 fockstatecircuit-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    14131 2024-04-19 06:19:32.000000 fockstatecircuit-1.0.1/README.md
--rw-rw-rw-   0        0        0      745 2024-04-19 06:20:54.000000 fockstatecircuit-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-19 06:21:15.340669 fockstatecircuit-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-19 06:21:14.719510 fockstatecircuit-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-19 06:21:15.335685 fockstatecircuit-1.0.1/src/FockStateCircuit.egg-info/
--rw-rw-rw-   0        0        0    16004 2024-04-19 06:21:14.000000 fockstatecircuit-1.0.1/src/FockStateCircuit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1728 2024-04-19 06:21:14.000000 fockstatecircuit-1.0.1/src/FockStateCircuit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 06:21:14.000000 fockstatecircuit-1.0.1/src/FockStateCircuit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-04-19 06:21:14.000000 fockstatecircuit-1.0.1/src/FockStateCircuit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-19 06:21:14.000000 fockstatecircuit-1.0.1/src/FockStateCircuit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-19 06:21:14.889680 fockstatecircuit-1.0.1/src/fock_state_circuit/
--rw-rw-rw-   0        0        0     1685 2024-04-15 04:59:27.000000 fockstatecircuit-1.0.1/src/fock_state_circuit/__init__.py
--rw-rw-rw-   0        0        0    64513 2024-04-16 07:01:30.000000 fockstatecircuit-1.0.1/src/fock_state_circuit/circuit.py
--rw-rw-rw-   0        0        0    66307 2024-04-16 07:01:09.000000 fockstatecircuit-1.0.1/src/fock_state_circuit/collection_of_states.py
--rw-rw-rw-   0        0        0     8305 2024-04-16 07:00:48.000000 fockstatecircuit-1.0.1/src/fock_state_circuit/compound_circuit.py
--rw-rw-rw-   0        0        0    41978 2024-04-16 07:00:36.000000 fockstatecircuit-1.0.1/src/fock_state_circuit/no_signalling_boxes.py
-drwxrwxrwx   0        0        0        0 2024-04-19 06:21:15.035398 fockstatecircuit-1.0.1/src/fock_state_circuit/nodes/
--rw-rw-rw-   0        0        0     1674 2024-04-16 12:09:40.000000 fockstatecircuit-1.0.1/src/fock_state_circuit/nodes/bridge_nodes.py
--rw-rw-rw-   0        0        0     6435 2024-04-16 12:09:21.000000 fockstatecircuit-1.0.1/src/fock_state_circuit/nodes/classical_nodes.py
--rw-rw-rw-   0        0        0    10085 2024-04-16 12:09:06.000000 fockstatecircuit-1.0.1/src/fock_state_circuit/nodes/controlled_nodes.py
--rw-rw-rw-   0        0        0    35888 2024-04-16 12:08:54.000000 fockstatecircuit-1.0.1/src/fock_state_circuit/nodes/custom_nodes.py
--rw-rw-rw-   0        0        0     3182 2024-04-16 12:08:42.000000 fockstatecircuit-1.0.1/src/fock_state_circuit/nodes/measurement_nodes.py
-drwxrwxrwx   0        0        0        0 2024-04-19 06:21:15.052284 fockstatecircuit-1.0.1/src/fock_state_circuit/nodes/nodelist/
--rw-rw-rw-   0        0        0    15206 2024-04-16 12:09:55.000000 fockstatecircuit-1.0.1/src/fock_state_circuit/nodes/nodelist/node_list.py
--rw-rw-rw-   0        0        0     1716 2024-04-16 12:08:32.000000 fockstatecircuit-1.0.1/src/fock_state_circuit/nodes/nonlinear_optical_nodes.py
--rw-rw-rw-   0        0        0    34580 2024-04-16 12:08:13.000000 fockstatecircuit-1.0.1/src/fock_state_circuit/nodes/optical_nodes.py
--rw-rw-rw-   0        0        0    15702 2024-04-16 12:07:37.000000 fockstatecircuit-1.0.1/src/fock_state_circuit/nodes/spectral_nodes.py
--rw-rw-rw-   0        0        0    36995 2024-04-16 07:00:13.000000 fockstatecircuit-1.0.1/src/fock_state_circuit/state.py
-drwxrwxrwx   0        0        0        0 2024-04-19 06:21:15.102050 fockstatecircuit-1.0.1/src/fock_state_circuit/temporal_and_spectral_gate_functionality/
--rw-rw-rw-   0        0        0    14715 2024-04-16 12:06:16.000000 fockstatecircuit-1.0.1/src/fock_state_circuit/temporal_and_spectral_gate_functionality/collection_of_state_columns.py
--rw-rw-rw-   0        0        0    52027 2024-04-16 12:07:11.000000 fockstatecircuit-1.0.1/src/fock_state_circuit/temporal_and_spectral_gate_functionality/column_of_states.py
--rw-rw-rw-   0        0        0    66022 2024-04-16 12:06:32.000000 fockstatecircuit-1.0.1/src/fock_state_circuit/temporal_and_spectral_gate_functionality/interference_group.py
--rw-rw-rw-   0        0        0    25699 2024-04-16 12:05:42.000000 fockstatecircuit-1.0.1/src/fock_state_circuit/temporal_and_spectral_gate_functionality/temporal_functions.py
-drwxrwxrwx   0        0        0        0 2024-04-19 06:21:15.151060 fockstatecircuit-1.0.1/src/fock_state_circuit/visualization/
--rw-rw-rw-   0        0        0    87108 2024-04-16 12:05:28.000000 fockstatecircuit-1.0.1/src/fock_state_circuit/visualization/draw.py
--rw-rw-rw-   0        0        0    23072 2024-04-16 07:01:45.000000 fockstatecircuit-1.0.1/src/fock_state_circuit/visualization/plot.py
-drwxrwxrwx   0        0        0        0 2024-04-19 06:21:15.319026 fockstatecircuit-1.0.1/tests/
--rw-rw-rw-   0        0        0    42027 2024-04-02 05:40:44.000000 fockstatecircuit-1.0.1/tests/test_collection_of_states.py
--rw-rw-rw-   0        0        0    10301 2024-01-18 06:26:50.000000 fockstatecircuit-1.0.1/tests/test_collection_of_states_plot.py
--rw-rw-rw-   0        0        0   106980 2024-04-15 05:01:44.000000 fockstatecircuit-1.0.1/tests/test_fock_state_circuit.py
--rw-rw-rw-   0        0        0    22025 2024-04-11 07:52:56.000000 fockstatecircuit-1.0.1/tests/test_fock_state_circuit_applications.py
--rw-rw-rw-   0        0        0    39516 2024-03-28 07:29:27.000000 fockstatecircuit-1.0.1/tests/test_fock_state_circuit_draw.py
--rw-rw-rw-   0        0        0        4 2024-03-12 14:55:58.000000 fockstatecircuit-1.0.1/tests/test_interference_group.py
--rw-rw-rw-   0        0        0    20785 2024-04-16 06:22:42.000000 fockstatecircuit-1.0.1/tests/test_no_signalling_boxes.py
--rw-rw-rw-   0        0        0   123820 2024-04-10 06:03:04.000000 fockstatecircuit-1.0.1/tests/test_photon_resolved_collection.py
--rw-rw-rw-   0        0        0    17683 2024-04-02 04:30:08.000000 fockstatecircuit-1.0.1/tests/test_state.py
--rw-rw-rw-   0        0        0    15164 2024-04-09 04:51:02.000000 fockstatecircuit-1.0.1/tests/test_time_delay_applications.py
+drwxrwxrwx   0        0        0        0 2024-05-01 08:13:03.886433 fockstatecircuit-1.0.2/
+-rw-rw-rw-   0        0        0     1069 2023-11-24 00:31:46.000000 fockstatecircuit-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0    16075 2024-05-01 08:13:03.882673 fockstatecircuit-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    14202 2024-05-01 08:06:49.000000 fockstatecircuit-1.0.2/README.md
+-rw-rw-rw-   0        0        0      745 2024-05-01 08:06:09.000000 fockstatecircuit-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-01 08:13:03.887542 fockstatecircuit-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-01 08:13:02.656138 fockstatecircuit-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-01 08:13:03.878687 fockstatecircuit-1.0.2/src/FockStateCircuit.egg-info/
+-rw-rw-rw-   0        0        0    16075 2024-05-01 08:13:02.000000 fockstatecircuit-1.0.2/src/FockStateCircuit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1779 2024-05-01 08:13:02.000000 fockstatecircuit-1.0.2/src/FockStateCircuit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 08:13:02.000000 fockstatecircuit-1.0.2/src/FockStateCircuit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-01 08:13:02.000000 fockstatecircuit-1.0.2/src/FockStateCircuit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-01 08:13:02.000000 fockstatecircuit-1.0.2/src/FockStateCircuit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 08:13:03.058170 fockstatecircuit-1.0.2/src/fock_state_circuit/
+-rw-rw-rw-   0        0        0     1760 2024-04-28 14:53:42.000000 fockstatecircuit-1.0.2/src/fock_state_circuit/__init__.py
+-rw-rw-rw-   0        0        0    62549 2024-05-01 07:58:13.000000 fockstatecircuit-1.0.2/src/fock_state_circuit/circuit.py
+-rw-rw-rw-   0        0        0    65593 2024-04-30 14:02:24.000000 fockstatecircuit-1.0.2/src/fock_state_circuit/collection_of_states.py
+-rw-rw-rw-   0        0        0     8305 2024-04-16 07:00:48.000000 fockstatecircuit-1.0.2/src/fock_state_circuit/compound_circuit.py
+-rw-rw-rw-   0        0        0    44674 2024-05-01 06:26:07.000000 fockstatecircuit-1.0.2/src/fock_state_circuit/no_signalling_boxes.py
+drwxrwxrwx   0        0        0        0 2024-05-01 08:13:03.333371 fockstatecircuit-1.0.2/src/fock_state_circuit/nodes/
+-rw-rw-rw-   0        0        0     1674 2024-04-16 12:09:40.000000 fockstatecircuit-1.0.2/src/fock_state_circuit/nodes/bridge_nodes.py
+-rw-rw-rw-   0        0        0     6435 2024-04-16 12:09:21.000000 fockstatecircuit-1.0.2/src/fock_state_circuit/nodes/classical_nodes.py
+-rw-rw-rw-   0        0        0    10085 2024-04-16 12:09:06.000000 fockstatecircuit-1.0.2/src/fock_state_circuit/nodes/controlled_nodes.py
+-rw-rw-rw-   0        0        0    35888 2024-04-16 12:08:54.000000 fockstatecircuit-1.0.2/src/fock_state_circuit/nodes/custom_nodes.py
+-rw-rw-rw-   0        0        0     3182 2024-04-16 12:08:42.000000 fockstatecircuit-1.0.2/src/fock_state_circuit/nodes/measurement_nodes.py
+drwxrwxrwx   0        0        0        0 2024-05-01 08:13:03.363151 fockstatecircuit-1.0.2/src/fock_state_circuit/nodes/nodelist/
+-rw-rw-rw-   0        0        0    14178 2024-05-01 07:18:45.000000 fockstatecircuit-1.0.2/src/fock_state_circuit/nodes/nodelist/node_list.py
+-rw-rw-rw-   0        0        0     1716 2024-04-16 12:08:32.000000 fockstatecircuit-1.0.2/src/fock_state_circuit/nodes/nonlinear_optical_nodes.py
+-rw-rw-rw-   0        0        0    34580 2024-04-16 12:08:13.000000 fockstatecircuit-1.0.2/src/fock_state_circuit/nodes/optical_nodes.py
+-rw-rw-rw-   0        0        0    15702 2024-04-16 12:07:37.000000 fockstatecircuit-1.0.2/src/fock_state_circuit/nodes/spectral_nodes.py
+-rw-rw-rw-   0        0        0     6775 2024-04-29 06:54:10.000000 fockstatecircuit-1.0.2/src/fock_state_circuit/nodes/superquantum_nodes.py
+-rw-rw-rw-   0        0        0    38081 2024-05-01 07:41:19.000000 fockstatecircuit-1.0.2/src/fock_state_circuit/state.py
+drwxrwxrwx   0        0        0        0 2024-05-01 08:13:03.496312 fockstatecircuit-1.0.2/src/fock_state_circuit/temporal_and_spectral_gate_functionality/
+-rw-rw-rw-   0        0        0    14715 2024-04-16 12:06:16.000000 fockstatecircuit-1.0.2/src/fock_state_circuit/temporal_and_spectral_gate_functionality/collection_of_state_columns.py
+-rw-rw-rw-   0        0        0    52027 2024-04-16 12:07:11.000000 fockstatecircuit-1.0.2/src/fock_state_circuit/temporal_and_spectral_gate_functionality/column_of_states.py
+-rw-rw-rw-   0        0        0    66022 2024-04-16 12:06:32.000000 fockstatecircuit-1.0.2/src/fock_state_circuit/temporal_and_spectral_gate_functionality/interference_group.py
+-rw-rw-rw-   0        0        0    25699 2024-04-16 12:05:42.000000 fockstatecircuit-1.0.2/src/fock_state_circuit/temporal_and_spectral_gate_functionality/temporal_functions.py
+drwxrwxrwx   0        0        0        0 2024-05-01 08:13:03.562840 fockstatecircuit-1.0.2/src/fock_state_circuit/visualization/
+-rw-rw-rw-   0        0        0    87108 2024-04-16 12:05:28.000000 fockstatecircuit-1.0.2/src/fock_state_circuit/visualization/draw.py
+-rw-rw-rw-   0        0        0    23072 2024-04-16 07:01:45.000000 fockstatecircuit-1.0.2/src/fock_state_circuit/visualization/plot.py
+drwxrwxrwx   0        0        0        0 2024-05-01 08:13:03.872662 fockstatecircuit-1.0.2/tests/
+-rw-rw-rw-   0        0        0    41998 2024-04-30 11:15:54.000000 fockstatecircuit-1.0.2/tests/test_collection_of_states.py
+-rw-rw-rw-   0        0        0    10301 2024-01-18 06:26:50.000000 fockstatecircuit-1.0.2/tests/test_collection_of_states_plot.py
+-rw-rw-rw-   0        0        0   107131 2024-04-30 14:38:27.000000 fockstatecircuit-1.0.2/tests/test_fock_state_circuit.py
+-rw-rw-rw-   0        0        0    22025 2024-04-11 07:52:56.000000 fockstatecircuit-1.0.2/tests/test_fock_state_circuit_applications.py
+-rw-rw-rw-   0        0        0    39516 2024-03-28 07:29:27.000000 fockstatecircuit-1.0.2/tests/test_fock_state_circuit_draw.py
+-rw-rw-rw-   0        0        0        4 2024-03-12 14:55:58.000000 fockstatecircuit-1.0.2/tests/test_interference_group.py
+-rw-rw-rw-   0        0        0    23884 2024-04-29 06:47:49.000000 fockstatecircuit-1.0.2/tests/test_no_signalling_boxes.py
+-rw-rw-rw-   0        0        0   123820 2024-04-10 06:03:04.000000 fockstatecircuit-1.0.2/tests/test_photon_resolved_collection.py
+-rw-rw-rw-   0        0        0    17683 2024-04-02 04:30:08.000000 fockstatecircuit-1.0.2/tests/test_state.py
+-rw-rw-rw-   0        0        0    15164 2024-05-01 06:58:20.000000 fockstatecircuit-1.0.2/tests/test_time_delay_applications.py
```

### Comparing `fockstatecircuit-1.0.1/LICENSE.txt` & `fockstatecircuit-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fockstatecircuit-1.0.1/PKG-INFO` & `fockstatecircuit-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FockStateCircuit
-Version: 1.0.1
+Version: 1.0.2
 Summary: Modelling quantum optical circuits
 Author: Rob Hendriks
 License: MIT License
         
         Copyright (c) 2023 Rob Hendriks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -71,14 +71,16 @@
 result.plot()
 
 circuit.draw()
 ```
 The code should show this when running `result.plot()`: When using one photon the likelihood of finding it in any of the output ports is 50%. When using two photons (one for each input port) simultaneously we only see outcomes where both photons are in the same output ports, and not outcomes where they are each in a different output port. 
 ![title](./images/output_HOM_effect.png)
 
+
+
 The schematics of the circuit (shown when calling `circuit.draw()` are these:
 ![title](./images/output_fock_state_circuit_example.png)
 
 ## Basic explanation
 ### Circuits
 A FockStateCircuit consists of a series of 'nodes'. The variable `circuit.node_list` contains the nodes with all relevant information for evaluating the states and displaying the nodes. There are 4 types of nodes:
 * Optical nodes: These only contain interactions between optical channels (beamsplitters, wave plates)
@@ -153,14 +155,16 @@
                 GHZ simulation with FockStateCircuit.ipynb
                 Quantum Teleportation with FockStateCircuit.ipynb
 
     * Pydoc documentation generated from the docstrings in the modules
 You can also check https://armchairquantumphysicist.com/ where a number of applications are covered in blogposts
 
 ## Version history
+### Version 1.0.2
+* Minor bug fixes and performance improvements
 ### Version 1.0.0
 * Added feature or drawing stations of a circuit. If we model communication between 'alice' and 'bob' we can draw their specific 'stations' to make 
         clear what is happening at either side. This only affects the visualization.
 * Updated functionality for time delay. We can now model successive time delays. The way the code implements time delay is closer to actual mathemathical
         modelling of a system with (partially) distinguishable photons.
 * The code has been 'refactored' from two .py files into a structure with more classes and an individual .py file per class. This makes the code 
         easier to maintain.
```

### Comparing `fockstatecircuit-1.0.1/README.md` & `fockstatecircuit-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 result.plot()
 
 circuit.draw()
 ```
 The code should show this when running `result.plot()`: When using one photon the likelihood of finding it in any of the output ports is 50%. When using two photons (one for each input port) simultaneously we only see outcomes where both photons are in the same output ports, and not outcomes where they are each in a different output port. 
 ![title](./images/output_HOM_effect.png)
 
+
+
 The schematics of the circuit (shown when calling `circuit.draw()` are these:
 ![title](./images/output_fock_state_circuit_example.png)
 
 ## Basic explanation
 ### Circuits
 A FockStateCircuit consists of a series of 'nodes'. The variable `circuit.node_list` contains the nodes with all relevant information for evaluating the states and displaying the nodes. There are 4 types of nodes:
 * Optical nodes: These only contain interactions between optical channels (beamsplitters, wave plates)
@@ -115,14 +117,16 @@
                 GHZ simulation with FockStateCircuit.ipynb
                 Quantum Teleportation with FockStateCircuit.ipynb
 
     * Pydoc documentation generated from the docstrings in the modules
 You can also check https://armchairquantumphysicist.com/ where a number of applications are covered in blogposts
 
 ## Version history
+### Version 1.0.2
+* Minor bug fixes and performance improvements
 ### Version 1.0.0
 * Added feature or drawing stations of a circuit. If we model communication between 'alice' and 'bob' we can draw their specific 'stations' to make 
         clear what is happening at either side. This only affects the visualization.
 * Updated functionality for time delay. We can now model successive time delays. The way the code implements time delay is closer to actual mathemathical
         modelling of a system with (partially) distinguishable photons.
 * The code has been 'refactored' from two .py files into a structure with more classes and an individual .py file per class. This makes the code 
         easier to maintain.
```

### Comparing `fockstatecircuit-1.0.1/pyproject.toml` & `fockstatecircuit-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=61.0", "wheel>=0.37.1"]
 
 [project]
 name = "FockStateCircuit"
-version = "1.0.1"
+version = "1.0.2"
 dependencies = [
   "numpy >= 1.26.4",
   "matplotlib >= 3.8.4",
 ]
 requires-python = ">=3.12"
 authors = [
   {name = "Rob Hendriks"}
```

### Comparing `fockstatecircuit-1.0.1/src/FockStateCircuit.egg-info/PKG-INFO` & `fockstatecircuit-1.0.2/src/FockStateCircuit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FockStateCircuit
-Version: 1.0.1
+Version: 1.0.2
 Summary: Modelling quantum optical circuits
 Author: Rob Hendriks
 License: MIT License
         
         Copyright (c) 2023 Rob Hendriks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -71,14 +71,16 @@
 result.plot()
 
 circuit.draw()
 ```
 The code should show this when running `result.plot()`: When using one photon the likelihood of finding it in any of the output ports is 50%. When using two photons (one for each input port) simultaneously we only see outcomes where both photons are in the same output ports, and not outcomes where they are each in a different output port. 
 ![title](./images/output_HOM_effect.png)
 
+
+
 The schematics of the circuit (shown when calling `circuit.draw()` are these:
 ![title](./images/output_fock_state_circuit_example.png)
 
 ## Basic explanation
 ### Circuits
 A FockStateCircuit consists of a series of 'nodes'. The variable `circuit.node_list` contains the nodes with all relevant information for evaluating the states and displaying the nodes. There are 4 types of nodes:
 * Optical nodes: These only contain interactions between optical channels (beamsplitters, wave plates)
@@ -153,14 +155,16 @@
                 GHZ simulation with FockStateCircuit.ipynb
                 Quantum Teleportation with FockStateCircuit.ipynb
 
     * Pydoc documentation generated from the docstrings in the modules
 You can also check https://armchairquantumphysicist.com/ where a number of applications are covered in blogposts
 
 ## Version history
+### Version 1.0.2
+* Minor bug fixes and performance improvements
 ### Version 1.0.0
 * Added feature or drawing stations of a circuit. If we model communication between 'alice' and 'bob' we can draw their specific 'stations' to make 
         clear what is happening at either side. This only affects the visualization.
 * Updated functionality for time delay. We can now model successive time delays. The way the code implements time delay is closer to actual mathemathical
         modelling of a system with (partially) distinguishable photons.
 * The code has been 'refactored' from two .py files into a structure with more classes and an individual .py file per class. This makes the code 
         easier to maintain.
```

### Comparing `fockstatecircuit-1.0.1/src/FockStateCircuit.egg-info/SOURCES.txt` & `fockstatecircuit-1.0.2/src/FockStateCircuit.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 src/fock_state_circuit/nodes/classical_nodes.py
 src/fock_state_circuit/nodes/controlled_nodes.py
 src/fock_state_circuit/nodes/custom_nodes.py
 src/fock_state_circuit/nodes/measurement_nodes.py
 src/fock_state_circuit/nodes/nonlinear_optical_nodes.py
 src/fock_state_circuit/nodes/optical_nodes.py
 src/fock_state_circuit/nodes/spectral_nodes.py
+src/fock_state_circuit/nodes/superquantum_nodes.py
 src/fock_state_circuit/nodes/nodelist/node_list.py
 src/fock_state_circuit/temporal_and_spectral_gate_functionality/collection_of_state_columns.py
 src/fock_state_circuit/temporal_and_spectral_gate_functionality/column_of_states.py
 src/fock_state_circuit/temporal_and_spectral_gate_functionality/interference_group.py
 src/fock_state_circuit/temporal_and_spectral_gate_functionality/temporal_functions.py
 src/fock_state_circuit/visualization/draw.py
 src/fock_state_circuit/visualization/plot.py
```

### Comparing `fockstatecircuit-1.0.1/src/fock_state_circuit/__init__.py` & `fockstatecircuit-1.0.2/src/fock_state_circuit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from fock_state_circuit.nodes.optical_nodes import OpticalNodes
 from fock_state_circuit.nodes.bridge_nodes import BridgeNodes
 from fock_state_circuit.nodes.custom_nodes import CustomNodes
 from fock_state_circuit.nodes.controlled_nodes import ControlledNodes
 from fock_state_circuit.nodes.measurement_nodes import MeasurementNodes
 from fock_state_circuit.nodes.classical_nodes import ClassicalNodes
 from fock_state_circuit.nodes.spectral_nodes import SpectralNodes
+from fock_state_circuit.nodes.superquantum_nodes import SuperQuantumNodes
 from fock_state_circuit.nodes.nonlinear_optical_nodes import NonlinearOpticalNodes
 from fock_state_circuit.visualization.draw import Draw
 from fock_state_circuit.collection_of_states import CollectionOfStates
 from fock_state_circuit.visualization.plot import Plot, plot_correlations_from_dict
 from fock_state_circuit.state import State
 from fock_state_circuit.circuit import FockStateCircuit
 from fock_state_circuit.compound_circuit import CompoundFockStateCircuit
```

### Comparing `fockstatecircuit-1.0.1/src/fock_state_circuit/circuit.py` & `fockstatecircuit-1.0.2/src/fock_state_circuit/circuit.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,19 @@
 from fock_state_circuit.nodes.optical_nodes import OpticalNodes
 from fock_state_circuit.nodes.bridge_nodes import BridgeNodes
 from fock_state_circuit.nodes.custom_nodes import CustomNodes
 from fock_state_circuit.nodes.controlled_nodes import ControlledNodes
 from fock_state_circuit.nodes.measurement_nodes import MeasurementNodes
 from fock_state_circuit.nodes.classical_nodes import ClassicalNodes
 from fock_state_circuit.nodes.spectral_nodes import SpectralNodes
+from fock_state_circuit.nodes.superquantum_nodes import SuperQuantumNodes
 from fock_state_circuit.nodes.nonlinear_optical_nodes import NonlinearOpticalNodes
 from fock_state_circuit.visualization.draw import Draw
 from fock_state_circuit.nodes.spectral_nodes import perform_measurement_photon_resolved
+from fock_state_circuit.no_signalling_boxes import perform_measurement_no_signalling_boxes
 from fock_state_circuit.temporal_and_spectral_gate_functionality.temporal_functions import _VERSION as tf_VERSION
 
 
 def about():
     """
     About box for FockStateCircuit. Gives version numbers for
     FockStateCircuit, CollectionOfStates, NumPy and MatPlotLib.
@@ -47,15 +49,15 @@
     print("MeasurementNodes:            %s" % MeasurementNodes._VERSION)   
     print("ClassicalNodes:              %s" % ClassicalNodes._VERSION)
     print("SpectralNodes:               %s" % SpectralNodes._VERSION)
     print("temporal_functions:          %s" % tf_VERSION)
     print("Numpy Version:               %s" % np.__version__)          
     print("Matplotlib version:          %s" % mtplt.__version__)
 
-class FockStateCircuit(OpticalNodes,BridgeNodes, MeasurementNodes, ClassicalNodes, ControlledNodes, CustomNodes, SpectralNodes, NonlinearOpticalNodes, Draw):
+class FockStateCircuit(OpticalNodes,BridgeNodes, MeasurementNodes, ClassicalNodes, ControlledNodes, CustomNodes, SpectralNodes, NonlinearOpticalNodes, SuperQuantumNodes, Draw):
     """ Class for FockStateCircuit. The class is used to model the behavior of systems consisting of optical channels which can be 
         populates with Fock states, or photon number states (https://en.wikipedia.org/wiki/Fock_state). The circuit consistes of
         multiple channels (minimally 2 channels) which interact through optical components like beamsplitters and wave plates. The
         number states can be detected by detectors. Results from measurement are written to classical channels in the circuit. We also
         have the option to make the exact function of the optical components depending on the value in a classical channel. We can 
         for instance let the orientation of a wave plate depend on the value of the classical channels. 
 
@@ -126,17 +128,17 @@
                     Function returns a dictonary with valid components names as keys and the corresponding photon numbers in the channels as values.
 
             get_fock_state_matrix(self, 
                     nodes_to_be_evaluated: list[int] = 'all'
                     ) -> np.array:
                     Function returns the fock state matrix for a given set of nodes in the circuit            
 
-        Last modified: April 16th, 2024              
+        Last modified: May 1st, 2024              
     """
-    _VERSION = '1.0.0'
+    _VERSION = '1.0.2'
 
     def __init__(self, length_of_fock_state: int = 2, 
                  no_of_optical_channels: int = 2, 
                  no_of_classical_channels: int = 0, 
                  channel_0_left_in_state_name: bool = True,
                  threshold_probability_for_setting_to_zero: float = 0.0001,
                  use_full_fock_matrix:bool = False,
@@ -384,14 +386,24 @@
 
                 # perform the measurement
                 collection_of_states_output = perform_measurement_photon_resolved(  collection_of_states=collection_of_states_input, 
                                                                                     optical_channels_to_measure=optical_channels_to_be_read, 
                                                                                     classical_channels_to_write_to=classical_channels_to_be_written,
                                                                                     list_of_projections = list_of_projections)
                 return self.evaluate_circuit(collection_of_states_input = collection_of_states_output, nodes_to_be_evaluated = remaining_nodes)
+            
+            elif collection_of_states_input.has_no_signalling_boxes():
+                # get parameters from node on what channels to measure and where to write the results
+                optical_channels_to_be_read = self.node_list[current_node_index].get('optical_channels_to_be_read')
+                classical_channels_to_be_written = self.node_list[current_node_index].get('classical_channels_to_be_written')  
+                collection_of_states_output = perform_measurement_no_signalling_boxes(  collection_of_states=collection_of_states_input, 
+                                                                    optical_channels_to_measure=optical_channels_to_be_read, 
+                                                                    classical_channels_to_write_to=classical_channels_to_be_written)
+                return self.evaluate_circuit(collection_of_states_input = collection_of_states_output, nodes_to_be_evaluated = remaining_nodes)
+
             else:
                 # generate a number as a string to identify whether this is first, seconde, third etc measurement
                 measurement_identifier = self.__get_identifier_for_measurement(current_node_index)
                         
                 # get parameters from node on what channels to measure and where to write the results
                 optical_channels_to_be_read = self.node_list[current_node_index].get('optical_channels_to_be_read')
                 classical_channels_to_be_written = self.node_list[current_node_index].get('classical_channels_to_be_written')  
@@ -581,15 +593,14 @@
         return string_formatter.format(measurement_number)
 
     def _perform_measurement(self,
                             state: State,
                             optical_channels_to_measure: list = [],
                             classical_channels_to_write_to: list = []
                             ) -> CollectionOfStates:
-        
         """ Perform a measurement on a single state, where the given optical channels are measured and the result is written
             to the given classical channels. The function will return a collection of states, one state for each possible
             measurement outcome. The optical states will be the 'collapsed states' for the measurement outcome. The resulting 
             collection represents a 'statistical mixture' with as weights for each state the likelihood of the corresponding measurement
             result.
 
             List for optical and classical channels should be equally long to avoid unpredictable result
@@ -599,120 +610,64 @@
             optical_channels_to_measure (list, optional): optical channels to measure. list should have equal length list
                 for classical channels to write to
             classical_channels_to_write_to (list, optional): classical channels to write the optical measurements to
 
         Returns:
             CollectionOfStates: collection of states after measurement of single input state
         """        
-
-        # outcomes will be a dictionary with as key the possible measurement outcomes and as value a list of 
-        # indices for the components that lead to that outcome. The index indicates the place of the components
-        # in the self._self._list_of_fock_states.
-        outcomes = dict([])
-        string_format_in_state_as_word = "{:0"+str(self._digits_per_optical_channel)+ "d}"
-        # deep copy existing values of the classical values
-        classical_channel_values_before_measurement = [val for val in state.classical_channel_values]
-
-        vector_in, basis = state.translate_state_components_to_vector()
-
-        for component_index, amplitude in enumerate(vector_in):
-
-            probability = np.abs(amplitude)**2
-            
-            # if amplitude of the component is zero move to next
-            if probability < self._threshold_probability_for_setting_to_zero:
-                continue
-            
-            # get the photon count in the optical component
-            values = self._list_of_fock_states[component_index]
-
-            # determine the new values in classical channels.
-            # first load with the old values, later on overwrite with new values
-            classical_channel_after_measurement = [val for val in classical_channel_values_before_measurement]
-
-            # if the number of classical channels is larger than the number of opticl channels limit the number
-            # of classical channels. 
-            if len(classical_channels_to_write_to) > len(optical_channels_to_measure):
-                classical_channels_to_write_to = classical_channels_to_write_to[:len(optical_channels_to_measure)]
-            measurement_result = ''
-            for channel_index, classical_channel in enumerate(classical_channels_to_write_to):
-                optical_channel = optical_channels_to_measure[channel_index]
-                classical_channel_after_measurement[classical_channel] = values[optical_channel]
-                measurement_result += string_format_in_state_as_word.format(values[optical_channel])
-
-            # make a list of optical components that contribute to a given measurement result
-            if measurement_result not in outcomes.keys():
-                outcomes[measurement_result] = {'probability' : probability,
-                                                'results' :classical_channel_after_measurement,
-                                                'set_of_component_indices': set([component_index])
-                                                }
-            else:
-                outcomes[measurement_result]['probability'] += probability
-                outcomes[measurement_result]['set_of_component_indices'].add(component_index) 
-        
-        # for each measurement result from this state, for this specific measurement there is a key-value pair in the dictionary 'outcomes'
-        # the values are the probability to get that results (so these should ideally add up to 1 when adding up all possible measurement outcomes)
-        # and the list of indices indicated the components, or basis states leading to that outcome.
-
-        # Next we need to make the 'collapsed state' for each measurement outcome. All components contributing to that outcome should be in 
-        # that collapsed state, the components giving a different outcome should get amplitude zero. The result is a collection of states where 
-        # there is one state in the collection for each measurement outcome. 
-        # The cumulative_weight is the likelihood to get to a measurement result, the optical components all contribute to that result and the 
-        # probabilities for the components in each state again add up to one.
-
-        # create an empty collection of states with for same circuit
+        # create empty collection which will be populated with the collapsed states and returned at end of the function
         collection_of_states_after_measurement = CollectionOfStates(fock_state_circuit = self, input_collection_as_a_dict=dict([]))
 
-        # loop over all measurement results and create a new, collapsed state for each result.
-        for measurement_result, components_with_that_result in outcomes.items():
-            
-            # make a collapsed state for each outcome
-            collapsed_state = state.create_initialized_state()
-
-            # prepare the output 'vector' to generate the optical state. First set all to zero.
-            vector_out = [np.cdouble(0)] * len(vector_in)
-            
-            # loop over all components contributing to a particular outcomes
-            for component_index in components_with_that_result['set_of_component_indices']:
-                               
-                # the cumulative probability for this state in the collection is equal to the likelihood of getting to a 
-                # measurement result
-                cumulative_probability = components_with_that_result['probability']
-                if cumulative_probability != 0:
-                    # load amplitudes for remaining components in the output vector for optical state
-                    scale_factor = math.sqrt((1/cumulative_probability))
-                    vector_out[component_index] = vector_in[component_index] * scale_factor
-                
-            # the classical channels contain the measurement result
-            new_classical_channel_values = [i for i in components_with_that_result['results']]
-
-            # prepare the attribute 'measurement_results' for the collapsed state. If there are already
-            # measurement results in the input state copy these to the new collapsed state
-            if state.measurement_results and state.measurement_results is not None:
-                measurement_results = [previous_values for previous_values in state.measurement_results]   
-                measurement_results.append({'measurement_results':new_classical_channel_values, 'probability': cumulative_probability})   
-            else:
-                measurement_results = [{'measurement_results':new_classical_channel_values, 'probability': cumulative_probability}]
-
-            if state.cumulative_probability is not None:
-                cumulative_probability = state.cumulative_probability * cumulative_probability
-            else:
-                cumulative_probability = cumulative_probability
-            
-
-            collapsed_state.initial_state = state.initial_state
-            collapsed_state.cumulative_probability = cumulative_probability
-            # use the vector to populate the attribute 'optical_components' from the collapsed state
-            collapsed_state.set_state_components_from_vector(vector_out)
-            collapsed_state.classical_channel_values = new_classical_channel_values
-            collapsed_state.measurement_results = measurement_results
-
-            collection_of_states_after_measurement.add_state(state=collapsed_state, identifier=measurement_result)
+        # if the number of classical channels is larger than the number of opticl channels limit the number
+        # of classical channels. 
+        if len(classical_channels_to_write_to) > len(optical_channels_to_measure):
+            classical_channels_to_write_to = classical_channels_to_write_to[:len(optical_channels_to_measure)]
 
+        # create a list of tuples with a first tuple element the optical values and second the amplitude (as numpy complex number)
+        val_amp_list = [(self._dict_of_valid_component_names[name], amp_prob['amplitude']) for name, amp_prob in state.optical_components.items()]
+ 
+        # create a dictionary where the list of tuples is split for different measurement outcomes. The measurement outcome is the key
+        dict_of_outcomes = dict([])
+        for item in val_amp_list:
+            dict_of_outcomes.setdefault(tuple(item[0][n] for n in optical_channels_to_measure),[]).append(item)
+
+        # create for each measurement outcome a new 'collapsed' state and add this state to the collection as return value
+        # outcome is a tuple of measured values (like (0,1,2) if you measured three channels). List of outcomes is a list
+        # of tuples with values of all optical channels and the amplitudes
+        # [((0,2,3,1), 0.71), ((0,2,3,2), 0.71)]. For measured optical channels the values should be the same in all items in the list.
+        for outcome, list_of_outcomes in dict_of_outcomes.items():
+            # create a list or amplitudes and take sum and sum squared for normalization
+            old_amplitudes = np.array([item[1] for item in list_of_outcomes])
+            old_probabilities = old_amplitudes.real**2 + old_amplitudes.imag**2
+            tot_amp = np.sum(old_amplitudes )
+            tot_prob = np.sum(old_probabilities )
+            # renormalized to create new amplitudes and probabilities
+            new_amps = old_amplitudes/np.sqrt(tot_prob)
+            new_probs = new_amps.real**2 + new_amps.imag**2
+            # create a new state as collapsed state for a specific measurement result
+            new_state= state.copy()
+            # 1. the new state has a cumulative probability that is multiplied with the probability to detect this specific outcome
+            try:
+                new_state.cumulative_probability *= tot_prob
+            except:
+                new_state.cumulative_probability = np.round(new_state.cumulative_probability*tot_prob,3)
+            # 2. the new state should have classical channel values modified representing the measurement result
+            for i,n in enumerate(classical_channels_to_write_to):
+                new_state.classical_channel_values[n] = outcome[i]
+            # 3. the new state's measurement results need to be updated with 
+            try:
+                new_state.measurement_results.append({'measurement_results':new_state.classical_channel_values, 'probability': tot_prob})   
+            except:
+                new_state.measurement_results = [{'measurement_results':new_state.classical_channel_values, 'probability': tot_prob}]
+            new_state.optical_components = {self._dict_of_optical_values[tuple(name[0])]:{'amplitude':new_amplitude,'probability': new_probability} for name, new_amplitude, new_probability in zip(list_of_outcomes,new_amps, new_probs)}
+            # 4. Other aspects like initial_state and auxiliary_information remain unchanged
+            # add the new state to the collection
+            collection_of_states_after_measurement.add_state(new_state)
         return collection_of_states_after_measurement
+
     
     def __apply_node_or_nodes_to_collection(self,
                                           collection_of_states: CollectionOfStates = None,
                                           nodes_to_be_evaluated: list[int] = ["all"],
                                           single_custom_node = None) -> CollectionOfStates:
         
         """ Apply the node(s) to a collection of states. If no  collection_of_states_input is given the function will generate
```

### Comparing `fockstatecircuit-1.0.1/src/fock_state_circuit/collection_of_states.py` & `fockstatecircuit-1.0.2/src/fock_state_circuit/collection_of_states.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,21 +153,14 @@
                 are grouped together (i.e., replaced by one state with as 'cumulative_probability' the sum of probabilities of the
                 identical states). Finally, states with a low 'cumulative_probability' are removed. The threshold for removing is defined 
                 by the parameter 'threshold_probability_for_setting_to_zero' which can be passed to the FockStateCircuit for which this 
                 collection of states is valid.
                 
                 Warning: Function only checks for same 'initial_state' and same 'optical_components' if any other parameter differs between 
                 the states will be discarded.
-
-        _get_state_name_from_list_of_photon_numbers(self, state: list) -> str:
-                For a list of photon numbers generate a string which can serve as name for the state or a component in the state.
-                Example: state [0,1,3] would become '310' with 0 representing the photon number in channel 0. If we use reversed
-                state notation state [0,1,3] would become '013' (reversed or regular state notation is set in initialization of the 
-                FockStateCircuit). If we allow per channel photon numbers which require more digits (e.g., 10) the format of the string will be adjusted.
-                Example [10,1,3] would become '100103' 
         
         _group_states_together_by_photon_number(self)-> dict[str,list[str]]:
                 Group states together based on the total number of photons in the components of the state. The function
                 returns a dictionary where the key indicates photon number and the value is a list of state identifiers. The 
                 function groups states with components that all have the same photon number 
                 Example: if components in the state are '005', '221' and '230' the key will be '=5'
                 Example: if components in the state are '005', '211' and '200' the key will be '<=5'
@@ -216,16 +209,20 @@
 
                 Number of classical channels can also be extended. These will always be filled with value 0.
 
                 This function will modify the current collection 'in_place'. For a new collection with different
                 settings first create a copy and then modify the copy. 
         
         is_photon_resolved(self):
-                Return False if not all states have data on 'photon_resolution' in their state.auxiliary_information>
-                If this function returns True ALL states 'photon_resolution' have this information.
+                Return False if not all states have data on 'photon_resolution' in their state.auxiliary_information.
+                If this function returns True ALL states have this information.
+
+        has_no_signalling_boxes(self):
+                Return False if not all states have data on 'no_signalling_box' in their state.auxiliary_information.
+                If this function returns True ALL states have this information.
 
         Last modified: April 16th, 2024
         
     """
     _VERSION = '1.0.0'
    
     def __init__(self, fock_state_circuit: any, input_collection_as_a_dict: dict[str,"State"] = None):
@@ -265,22 +262,16 @@
         # this means that if the probability to find an outcome is lower than this threshold the outcome is discarded.
         self._threshold_probability_for_setting_to_zero = fock_state_circuit._threshold_probability_for_setting_to_zero
 
         # parameter use for __str__. With print_only_last_measurement set to True only last measurement is printed. With False the
         # complete history is printed.
         self.print_only_last_measurement = True
 
-        # generate a list of all possible values in the optical channels       
-        index_list = [index for index in range(0,self._length_of_fock_state**self._no_of_optical_channels)]
-        self._list_of_fock_states = [[] for index in index_list]
-        for _ in range(0,self._no_of_optical_channels):
-            for index in range(len(index_list)):
-                n = int(index_list[index]%self._length_of_fock_state)
-                self._list_of_fock_states[index].append(n)
-                index_list[index] = int(index_list[index]/self._length_of_fock_state)
+        # # generate a list of all possible values in the optical channels       
+        self._list_of_fock_states = fock_state_circuit._list_of_fock_states
         
         # create a dict with as keys the valid state names as strings and the list of photon numbers as value
         self._dict_of_valid_component_names = fock_state_circuit._dict_of_valid_component_names
 
         # create a dict with as keys the tuple of the list of photon numbers as value, 
         # and valid state names as strings as value
         self._dict_of_optical_values = fock_state_circuit._dict_of_optical_values 
@@ -627,37 +618,14 @@
         """ Function to completely clear the collection of states.
         """        
 
         self._collection_of_states = dict([])
         
         return
     
-    def _get_state_name_from_list_of_photon_numbers(self, state: list) -> str:
-        """ For a list of photon numbers generate a string which can serve as name for the state or a component in the state.
-            Example: state [0,1,3] would become '310' with 0 representing the photon number in channel 0. If we use reversed
-            state notation state [0,1,3] would become '013' (reversed or regular state notation is set in initialization of the 
-            FockStateCircuit). If we allow per channel photon numbers which require more digits (e.g., 10) the format of the string will be adjusted.
-            Example [10,1,3] would become '100103'
-
-        Args:
-            state (List): state as a list of values with channel 'n' at index 'n'. e.g., [0,1,3]
-
-        Returns:
-            str: name of the state of component derived from photon number per channel. e.g., '013'
-        """        
-        # string_format_in_state_as_word = "{:0"+str(len(str(self._length_of_fock_state-1)))+ "d}"
-
-        # if self._channel_0_left_in_state_name == True:
-        #     name = ''.join([string_format_in_state_as_word.format(number) for number in state])              
-        # else: #self.state_least_significant_digit_left == False:
-        #     name = ''.join([string_format_in_state_as_word.format(number) for number in state[::-1]]) 
-
-
-        return self._fock_state_circuit._dict_of_optical_values[tuple(state)]
-    
     def _group_states_together_by_photon_number(self)-> dict[str,list[str]]:
         """ Group states together based on the total number of photons in the components of the state. The function
             returns a dictionary where the key indicates photon number and the value is a list of state identifiers. The 
             function groups states with components that all have the same photon number 
             Example: if components in the state are '005', '221' and '230' the key will be '=5'
             Example: if components in the state are '005', '211' and '200' the key will be '<=5'
 
@@ -701,15 +669,16 @@
         if initial_state != '':
             set_of_initial_states = set([initial_state])
         else:
             set_of_initial_states = set([state['initial_state'] for state in self._collection_of_states.values()])
 
         dictionary_with_return_values = dict([])
         for initial_state in set_of_initial_states:
-            dm_mixed_state = np.zeros((len(self._list_of_fock_states), len(self._list_of_fock_states)), dtype=np.cdouble)
+            len_of_basis = len(self._dict_of_valid_component_names)
+            dm_mixed_state = np.zeros((len_of_basis, len_of_basis), dtype=np.cdouble)
             for state in self._collection_of_states.values():
                 if state.initial_state == initial_state:
                     vector, basis = state.translate_state_components_to_vector()
                     dm_single_state = np.outer(np.conjugate(vector),vector)
                     dm_mixed_state += state.cumulative_probability * dm_single_state
 
             trace_dm = np.round(np.abs(np.trace(dm_mixed_state)),decimals=decimal_places_for_trace)
@@ -734,14 +703,23 @@
                 optical_channels_to_keep (list): list of optical channel numbers that should remain
                 classical_channels_to_keep (list): list of classical channel numbers that should remain
            
             Returns:
                 Nothing. The 'collection of states' will be modified in-place.
                 
         """
+        def new_component_name_from_list(values):
+            """ function to create string label from list of values"""
+            string_format_in_state_as_word = "{:0"+str(len(str(self._length_of_fock_state-1)))+ "d}"
+            tuple_of_strings = tuple(string_format_in_state_as_word.format(number) for number in range(self._length_of_fock_state))
+            if self._channel_0_left_in_state_name:
+                new_label = ''.join([tuple_of_strings[number] for number in values])
+            else:
+                new_label = ''.join([tuple_of_strings[number] for number in values[::-1]])
+            return new_label
         if optical_channels_to_keep == []:
             optical_channels_to_keep  = [*range(self._no_of_optical_channels)]
         if classical_channels_to_keep ==  []:
             classical_channels_to_keep  = [*range(self._no_of_classical_channels)]
 
         if not all([channel in [*range(self._no_of_optical_channels)] for channel in optical_channels_to_keep]):
             raise Exception('error in channel selection in CollectionOfStates.reduce()')
@@ -763,15 +741,15 @@
 
         # create a lookup table from original component names to reduced component names. 
         # for each original name there will be multiple names in the resulting collection
         lookup_table_component_names = dict([])
         string_format_in_state_as_word = "{:0"+str(len(str(self._length_of_fock_state-1)))+ "d}"
         for name, list in self._dict_of_valid_component_names.items():
             new_list = [list[channel_number] for channel_number in optical_channels_to_keep]
-            new_name = updated_circuit._get_state_name_from_list_of_photon_numbers(new_list)
+            new_name = new_component_name_from_list(new_list)
             traced_out_values = [list[number] for number in range(self._no_of_optical_channels) if number not in optical_channels_to_keep]
             traced_out_name = ''.join([string_format_in_state_as_word.format(number) for number in traced_out_values])
             lookup_table_component_names.update({name: {'new_name' : new_name, 'traced_out_values': traced_out_name }})
 
         for identifier, old_state in self._collection_of_states.items():
             # for each state in original collection group together the optical components that lead to the same 
             # optical component in the resulting state
@@ -804,16 +782,16 @@
                     }
                 new_state = State(collection_of_states=new_collection_of_states, input_state_as_a_dict=new_state_as_a_dict)
                 new_collection_of_states.add_state(state=new_state,identifier=identifier+traced_out_value)
 
             self._collection_of_states = new_collection_of_states.collection_as_dict()
             self._no_of_classical_channels = new_collection_of_states._no_of_classical_channels
             self._no_of_optical_channels = new_collection_of_states._no_of_optical_channels
-            self._list_of_fock_states = new_collection_of_states._list_of_fock_states
             self._dict_of_valid_component_names = new_collection_of_states._dict_of_valid_component_names
+            self._dict_of_optical_values = new_collection_of_states._dict_of_optical_values
 
         return 
     
     def adjust_length_of_fock_state(self, new_length_of_fock_state: int = 0):
         """ Adjusts the 'length of Fock state' for the collection. This determines the maximum
             number of photons per channel. If 'length of Fock state' is for instance 4 the allowed photon
             numbers are 0,1,2 and 3. 
@@ -863,16 +841,16 @@
                                     'auxiliary_information' : state.auxiliary_information
                                     }
             new_state = State(collection_of_states=new_collection_of_states,input_state_as_a_dict=new_state_as_a_dict)
             new_collection_of_states.add_state(state = new_state, identifier=identifier)
  
         self._collection_of_states = new_collection_of_states.collection_as_dict()
         self._length_of_fock_state = new_collection_of_states._length_of_fock_state
-        self._list_of_fock_states = new_collection_of_states._list_of_fock_states
         self._dict_of_valid_component_names = new_collection_of_states._dict_of_valid_component_names
+        self._dict_of_optical_values = new_collection_of_states._dict_of_optical_values
     
         return
 
     
     def clean_up(self, initial_state: str = '') -> None:
         """ Cleans up the collection_of_states. All optical components with low probability are removed and the total set 
             of optical components is renormalized. Then all states with the same 'initial_state' and the same 'optical_components'
@@ -946,14 +924,24 @@
                 extra_classical_channels (int): number of classical channels to be added
                 statistical_distribution (list[int]): probabilities for photon numbers in new channels. Default 
                     new channels will be filled with 0 photons.
            
             Returns:
                 Nothing. The 'collection of states' will be modified in-place.
         """
+        def new_component_name_from_list(values):
+            """ function to create string label from list of values"""
+            string_format_in_state_as_word = "{:0"+str(len(str(self._length_of_fock_state-1)))+ "d}"
+            tuple_of_strings = tuple(string_format_in_state_as_word.format(number) for number in range(self._length_of_fock_state))
+            if self._channel_0_left_in_state_name:
+                new_label = ''.join([tuple_of_strings[number] for number in values])
+            else:
+                new_label = ''.join([tuple_of_strings[number] for number in values[::-1]])
+            return new_label
+        
         # create default value if statistical_distribution is empty list
         if statistical_distribution == []:
             statistical_distribution = [0]*self._length_of_fock_state
             statistical_distribution[0] = 1
         elif len(statistical_distribution) != self._length_of_fock_state:
             raise Exception('error with channel numbers in function collection_of_states.extend')  
     
@@ -972,34 +960,35 @@
         new_collection_of_states = CollectionOfStates(fock_state_circuit= updated_circuit )
         new_collection_of_states.clear()
         new_collection_of_states._channel_0_left_in_state_name = self._channel_0_left_in_state_name
         new_collection_of_states._threshold_probability_for_setting_to_zero = self._threshold_probability_for_setting_to_zero
         new_collection_of_states.print_only_last_measurement = self.print_only_last_measurement
 
         # create a dict with values for extra channels and their probabilities
+
         extra_channel_values = dict({'initial_value' : (1,[])})
         for _ in range(extra_optical_channels):
             new_extra_channel_values = dict([])
             for old_probability, values in extra_channel_values.values():
                 for index, fock_state_value in enumerate(range(self._length_of_fock_state)):
                     new_probability = statistical_distribution[index]*old_probability
                     new_values = values + [fock_state_value]
-                    new_label = updated_circuit._get_state_name_from_list_of_photon_numbers(new_values)
+                    new_label = new_component_name_from_list(new_values)
                     new_extra_channel_values.update({new_label: (new_probability,new_values)})
             extra_channel_values = new_extra_channel_values
 
         # for each existing state create a statistical mixture for possible values in new channels
         for probability, values in extra_channel_values.values():
             for old_state in self._collection_of_states.values():
                 optical_components = old_state['optical_components']
                 new_optical_components = dict([])
                 for component_name, amplitude_probability in optical_components.items():
                     list = self._dict_of_valid_component_names[component_name]
                     new_list = list + values
-                    new_component_name = updated_circuit._get_state_name_from_list_of_photon_numbers(new_list)
+                    new_component_name = new_component_name_from_list(new_list)
                     new_optical_components.update({new_component_name:amplitude_probability})
                 new_state_as_a_dict = {   'initial_state' : old_state['initial_state'],
                     'cumulative_probability' :  old_state['cumulative_probability']*probability,
                     'optical_components' : new_optical_components, 
                     'classical_channel_values' : old_state['classical_channel_values'] + [0]*extra_classical_channels,
                     'measurement_results' : old_state['measurement_results'],
                     'auxiliary_information' : old_state['auxiliary_information']
@@ -1008,20 +997,29 @@
                     new_state = State(collection_of_states=new_collection_of_states, input_state_as_a_dict=new_state_as_a_dict)
                     new_collection_of_states.add_state(state=new_state)
             
 
         self._collection_of_states = new_collection_of_states.collection_as_dict()
         self._no_of_classical_channels = new_collection_of_states._no_of_classical_channels
         self._no_of_optical_channels = new_collection_of_states._no_of_optical_channels
-        self._list_of_fock_states = new_collection_of_states._list_of_fock_states
         self._dict_of_valid_component_names = new_collection_of_states._dict_of_valid_component_names
+        self._dict_of_optical_values = new_collection_of_states._dict_of_optical_values
        
         return
     
     def is_photon_resolved(self):
-        """ Return False if not all states have data on 'photon_resolution' in their state.auxiliary_information>
-            If this function returns True ALL states 'photon_resolution' have this information.
+        """ Return False if not all states have data on 'photon_resolution' in their state.auxiliary_information.
+            If this function returns True ALL states have this information.
         """
         for state in self:
             if not 'photon_resolution' in state.auxiliary_information.keys():
                 return False
+        return True
+    
+    def has_no_signalling_boxes(self):
+        """ Return False if not all states have data on 'no_signalling_box' in their state.auxiliary_information.
+            If this function returns True ALL states have this information.
+        """
+        for state in self:
+            if not 'no_signalling_box' in state.auxiliary_information.keys():
+                return False
         return True
```

### Comparing `fockstatecircuit-1.0.1/src/fock_state_circuit/compound_circuit.py` & `fockstatecircuit-1.0.2/src/fock_state_circuit/compound_circuit.py`

 * *Files identical despite different names*

### Comparing `fockstatecircuit-1.0.1/src/fock_state_circuit/no_signalling_boxes.py` & `fockstatecircuit-1.0.2/src/fock_state_circuit/no_signalling_boxes.py`

 * *Files 2% similar despite different names*

```diff
@@ -296,15 +296,15 @@
             if outcome in configurations_and_amplitudes_grouped_per_outcome.keys():
                 configurations_and_amplitudes_grouped_per_outcome[outcome].update({configuration:amplitude})
             else:
                 configurations_and_amplitudes_grouped_per_outcome.update({outcome : {configuration:amplitude}})
     
     return configurations_and_amplitudes_grouped_per_outcome
 
-def create_collection_with_NS_boxes(state, ns_boxes) -> fsc.CollectionOfStates:
+def create_collection_with_NS_boxes(state, ns_boxes) -> any:
     """ Create a CollectionOfStates which can be processed in a FockStateCircuit. This collection
         represents  set of 'No signalling boxes' which can have 'superquantum' correlations.
 
         The argument 'state' is a state matching the circuit on which the returned collection will
         be evaluated. The exact content of the state is not important, it is used as a 'template' 
         to create the collection from.
 
@@ -388,15 +388,15 @@
         for name, amp_prob in state.optical_components.items():
             values = new_collection._dict_of_valid_component_names[name].copy()
             for configuration_for_this_box,ns_box in zip(configuration,ns_boxes):
                 channels_Ah_Av_Bh_Bv = ns_box['channels_Ah_Av_Bh_Bv']
                 values_in_channels = channel_values_for_config[int(configuration_for_this_box)]
                 for index,channel in enumerate(channels_Ah_Av_Bh_Bv):
                     values[channel] = values_in_channels[index]
-            new_name = new_collection._get_state_name_from_list_of_photon_numbers(values)
+            new_name = new_collection._dict_of_optical_values[tuple(values)]
             new_optical_components.append((new_name, amp_prob['amplitude']))
         new_state.optical_components = new_optical_components
         superentanglement_info = {  'superentanglement': identifier,
                                     'configuration' : configuration,
                                     'quantumness_indicator' : quantumness_indicators
                                 }
         new_state.auxiliary_information.update({'no_signalling_box': superentanglement_info})
@@ -515,20 +515,62 @@
             else:
                 alignment_probability = 0
 
             probability = probability*alignment_probability
 
         histogram.append({ 'output_state' : outcome, 'probability' : probability})
 
-
     return histogram
 
+
+def perform_measurement_no_signalling_boxes(collection_of_states, optical_channels_to_measure,classical_channels_to_write_to):
+    """ Performs a FULL measurement (i.e., measures all optical channels) where the detection probability is determined
+        from the 'no-signalling boxes'. The collection of states needs to be build by using the gate 'create_no_signalling_boxes'.
+
+    Args:
+        collection_of_states (fsc.CollectionOfStates): Collection of states to be measured
+        optical_channels_to_be_measured (list[int]): list of of optical channel numbers to be measured
+        classical_channels_to_be_written (list[int]): list of classical channel numbers to write the measurement result to
+
+    Returns:
+        fsc.CollectionOfStates: Collection with 'collapsed' states and classical channels written
+
+    """
+    output_collection = collection_of_states.copy()
+    output_collection.clear()
+
+    histo = measure_collection_with_NS_boxes(collection_of_states)
+    for state in collection_of_states:
+        reference_state = state
+        break
+    del reference_state.auxiliary_information['no_signalling_box']
+    reference_state.initial_state = 'no_signalling_boxes'
+    for outcome in histo:
+        new_state = reference_state.copy()
+        new_state.cumulative_probability = outcome['probability']
+        new_state.optical_components = [(outcome['output_state'],1)]
+        new_classical_channel_values = [val for val in new_state.classical_channel_values]
+        optical_channel_values = new_state._dict_of_valid_component_names[outcome['output_state']]
+        for classical_channel, optical_channel in zip(classical_channels_to_write_to, optical_channels_to_measure):
+            new_classical_channel_values[classical_channel] = optical_channel_values[optical_channel]
+        new_state.classical_channel_values = new_classical_channel_values
+        # prepare the attribute 'measurement_results' for the collapsed state. If there are already
+        # measurement results in the input state copy these to the new collapsed state
+        if state.measurement_results and state.measurement_results is not None:
+            measurement_results = [previous_values for previous_values in state.measurement_results]   
+            measurement_results.append({'measurement_results':new_state.classical_channel_values.copy(), 'probability': outcome['probability']})   
+        else:
+            measurement_results = [{'measurement_results':new_state.classical_channel_values.copy(), 'probability': outcome['probability']}]
+        new_state.measurement_results = measurement_results
+        output_collection.add_state(state = new_state)
+    return output_collection
+
 def correlations_from_measured_collection_with_NS_boxes(list_of_outcomes: list, 
                                                         channel_combis_for_correlation: list,
-                                                        state: fsc.State) -> list:
+                                                        state: any) -> list:
     """ This function will return a list of correlations for the provided 'list_of_outcomes'. 
 
         list_of_outcomes is of the form       
                 [{ 'output_state' : outcome1, 'probability' : probability1}, 
                 { 'output_state' : outcome2, 'probability' : probability2},
                 { 'output_state' : outcome3, 'probability' : probability3},
                 ...]
```

### Comparing `fockstatecircuit-1.0.1/src/fock_state_circuit/nodes/bridge_nodes.py` & `fockstatecircuit-1.0.2/src/fock_state_circuit/nodes/bridge_nodes.py`

 * *Files identical despite different names*

### Comparing `fockstatecircuit-1.0.1/src/fock_state_circuit/nodes/classical_nodes.py` & `fockstatecircuit-1.0.2/src/fock_state_circuit/nodes/classical_nodes.py`

 * *Files identical despite different names*

### Comparing `fockstatecircuit-1.0.1/src/fock_state_circuit/nodes/controlled_nodes.py` & `fockstatecircuit-1.0.2/src/fock_state_circuit/nodes/controlled_nodes.py`

 * *Files identical despite different names*

### Comparing `fockstatecircuit-1.0.1/src/fock_state_circuit/nodes/custom_nodes.py` & `fockstatecircuit-1.0.2/src/fock_state_circuit/nodes/custom_nodes.py`

 * *Files identical despite different names*

### Comparing `fockstatecircuit-1.0.1/src/fock_state_circuit/nodes/measurement_nodes.py` & `fockstatecircuit-1.0.2/src/fock_state_circuit/nodes/measurement_nodes.py`

 * *Files identical despite different names*

### Comparing `fockstatecircuit-1.0.1/src/fock_state_circuit/nodes/nodelist/node_list.py` & `fockstatecircuit-1.0.2/src/fock_state_circuit/nodes/nodelist/node_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -108,34 +108,32 @@
         # This is optimal for system with large 'length_of_fock_state' and many optical channels, but only a few photons running 
         # through the system.
         self._use_full_fock_matrix = use_full_fock_matrix
         
         # name for the circuit
         self._circuit_name = circuit_name
 
-        # generate a list of all possible values in the optical channels 
-        index_list = [index for index in range(0,length_of_fock_state**self._no_of_optical_channels)]
-        self._list_of_fock_states = [[] for index in index_list]
-        for _ in range(0,self._no_of_optical_channels):
-            for index in range(len(index_list)):
-                n = int(index_list[index]%length_of_fock_state)
-                self._list_of_fock_states[index].append(n)
-                index_list[index] = int(index_list[index]/length_of_fock_state)
-
-        # create a dict with as keys the valid state names as strings and the list of photon numbers as value
-        self._dict_of_valid_component_names = dict([])
-        for optical_state in  self._list_of_fock_states:
-            name = self._get_state_name_from_list_of_photon_numbers(optical_state)
-            self._dict_of_valid_component_names.update({name : optical_state})
-
-        # create a dict with as keys the tuple of the list of photon numbers as value, 
-        # and valid state names as strings as value
-        self._dict_of_optical_values = dict([])
-        for k,v in self._dict_of_valid_component_names.items():
-            self._dict_of_optical_values.update({tuple(v):k})
+        string_format_in_state_as_word = "{:0"+str(len(str(self._length_of_fock_state-1)))+ "d}"
+        tuple_of_strings = tuple(string_format_in_state_as_word.format(number) for number in range(self._length_of_fock_state))
+        self._list_of_fock_states = [[(n//(self._length_of_fock_state**c))%self._length_of_fock_state for c in range(self._no_of_optical_channels)] for n in range(self._length_of_fock_state**self._no_of_optical_channels)]
+        if self._channel_0_left_in_state_name == True:
+            self._dict_of_valid_component_names = {''.join([tuple_of_strings[number] for number in optical_state]):optical_state for optical_state in self._list_of_fock_states}
+        else: #self.state_least_significant_digit_left == False:
+            self._dict_of_valid_component_names = {''.join([tuple_of_strings[number] for number in optical_state[::-1]]):optical_state for optical_state in self._list_of_fock_states}       
+        self._dict_of_optical_values = {tuple(v):k for k,v in self._dict_of_valid_component_names.items()}
+        
+        # create template state
+        name = ''.join([tuple_of_strings[0]] *self._no_of_optical_channels)
+        self._template_state_dict = {   'initial_state' : name,
+                            'cumulative_probability' : 1,
+                            'optical_components' : { name: {'amplitude':1,'probability': 1} }, 
+                            'classical_channel_values' : [0]*self._no_of_classical_channels,
+                            'measurement_results' : [],
+                            'auxiliary_information' : {}
+                            }
 
     def _update_list_of_nodes(self, node_to_be_added: dict = None) -> None:
 
         """ Update the list of nodes for node_list. This is the single function to update the list of nodes which serves as
             as a gatekeeper. node to be added is a dictionary describing the node.
 
         Args:
@@ -198,30 +196,8 @@
             else:
                 tensor_list[0], tensor_list[channel_horizontal] = tensor_list[channel_horizontal],  tensor_list[0]
                 tensor_list[1], tensor_list[channel_vertical] = tensor_list[channel_vertical],  tensor_list[1]  
         
         else:
             raise Exception('error creating tensor list, more than two channels provided')
         
-        return tensor_list
-    
-    def _get_state_name_from_list_of_photon_numbers(self, state: list) -> str:
-        """ For a list of photon numbers generate a string which can serve as name for the state or a component in the state.
-            Example: state [0,1,3] would become '310' with 0 representing the photon number in channel 0. If we use reversed
-            state notation state [0,1,3] would become '013' (reversed or regular state notation is set in initialization of the 
-            FockStateCircuit). If we allow per channel photon numbers which require more digits (e.g., 10) the format of the string will be adjusted.
-            Example [10,1,3] would become '100103'
-
-        Args:
-            state (List): state as a list of values with channel 'n' at index 'n'. e.g., [0,1,3]
-
-        Returns:
-            str: name of the state of component derived from photon number per channel. e.g., '013'
-        """        
-        string_format_in_state_as_word = "{:0"+str(len(str(self._length_of_fock_state-1)))+ "d}"
-
-        if self._channel_0_left_in_state_name == True:
-            name = ''.join([string_format_in_state_as_word.format(number) for number in state])              
-        else: #self.state_least_significant_digit_left == False:
-            name = ''.join([string_format_in_state_as_word.format(number) for number in state[::-1]]) 
-
-        return name
+        return tensor_list
```

### Comparing `fockstatecircuit-1.0.1/src/fock_state_circuit/nodes/nonlinear_optical_nodes.py` & `fockstatecircuit-1.0.2/src/fock_state_circuit/nodes/nonlinear_optical_nodes.py`

 * *Files identical despite different names*

### Comparing `fockstatecircuit-1.0.1/src/fock_state_circuit/nodes/optical_nodes.py` & `fockstatecircuit-1.0.2/src/fock_state_circuit/nodes/optical_nodes.py`

 * *Files identical despite different names*

### Comparing `fockstatecircuit-1.0.1/src/fock_state_circuit/nodes/spectral_nodes.py` & `fockstatecircuit-1.0.2/src/fock_state_circuit/nodes/spectral_nodes.py`

 * *Files identical despite different names*

### Comparing `fockstatecircuit-1.0.1/src/fock_state_circuit/state.py` & `fockstatecircuit-1.0.2/src/fock_state_circuit/state.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,17 +97,17 @@
                     - 'state' can be of type: 
                                 new_components = state1.tensor(state = state2) with state2 of type fsc.State
                     - 'state' can be the optical components: 
                                 new_components = state1.tensor(state = {'100':{'amplitude': 1.0,'probability': 1.0}})
                     - 'state' can be a list of tuples: 
                                 new_components =  state1.tensor([('100',np.sqrt(1/2)),('110',1/2),('111',1/2)])
 
-        Last modified: April 16th, 2024
+        Last modified: May 1st, 2024
     """
-    _VERSION = '1.0.0'
+    _VERSION = '1.0.1'
     
     _KEYS_IN_STATE = ['initial_state', 'cumulative_probability', 'optical_components', 'measurement_results', 'classical_channel_values', 'auxiliary_information']
 
     def __init__(self, collection_of_states : any, input_state_as_a_dict: dict = None):
         """ Constructor for in instance of class "State". The state instance will be created in initialized form.
 
         Args:
@@ -155,22 +155,22 @@
         # complete history is printed.
         self._print_only_last_measurement = collection_of_states.print_only_last_measurement
         
         # initialize the state as an empty state with default values or from the data in the 'input_state_as_a_dict' parameter
         self.initialize_this_state()
 
         # if a dictionary with values is given as argument use those values to populate the state
-        if input_state_as_a_dict is not None and isinstance(input_state_as_a_dict, dict):
+        if input_state_as_a_dict:
             for k,v in input_state_as_a_dict.items():
                 if k in self._KEYS_IN_STATE:
                     self.state[k] = v     
-            # check if state is valid, otherwise raise an exception
-            if not True in (self._check_valid_state(state_to_check = self)):
-                print(self._check_valid_state(state_to_check = self))
-                raise Exception('invalid state')
+        #check if state is valid, otherwise raise an exception
+        if not True in (self._check_valid_state(state_to_check = self)):
+            print(self._check_valid_state(state_to_check = self))
+            raise Exception('invalid state')
             
     @property
     def initial_state(self):
         return self.state['initial_state']
        
     @initial_state.setter
     def initial_state(self, name: str):
@@ -409,48 +409,65 @@
 
     def copy(self) -> "State":       
         """ Return a deep copy of a state with same parameters (i.e., suitable for same fock state circuit)
 
         Returns:
             State: Deep copy of the current state
         """        
-        new_initial_state = "{:s}".format(self.state['initial_state'])
 
-        new_cumulative_probability = self.state['cumulative_probability']
-        
-        new_optical_components = dict([])
-        for oc_name, oc_comp in self.state['optical_components'].items():
-            new_comp_name = "{:s}".format(oc_name)
-            new_comp_values = dict([])
-            for k,v in oc_comp.items():
-                new_comp_values.update({k:v})
-            new_optical_components.update({new_comp_name :  new_comp_values})
-        
-        new_classical_channel_values = self.state['classical_channel_values'].copy()
-        
-        new_measurement_results = []
-        for m_result in self.state['measurement_results']:
-            new_m_result = dict([])
-            for k,v in m_result.items():
-                new_m_result.update({k:v})
-            new_measurement_results.append(new_m_result)
-        
-        new_state_as_a_dict = {   'initial_state' : new_initial_state,
-                            'cumulative_probability' : new_cumulative_probability,
-                            'optical_components' : new_optical_components, 
-                            'classical_channel_values' : new_classical_channel_values,
-                            'measurement_results' : new_measurement_results
+            
+        new_state_as_a_dict = {   'initial_state' : self.state['initial_state'],
+                            'cumulative_probability' : self.state['cumulative_probability'],
+                            'optical_components' : { name:amp_prob.copy() for name, amp_prob in self.state['optical_components'].items() }, 
+                            'classical_channel_values' : self.state['classical_channel_values'].copy(),
+                            'measurement_results' : [{k:v for k,v in m_result.items()} for m_result in self.state['measurement_results']]
                             }
-        
         auxiliary_information = self.state.get('auxiliary_information', None)
-        if auxiliary_information is not None and len(auxiliary_information) > 0:
-            new_auxiliary_information = copy.deepcopy(self.state['auxiliary_information'])
-            new_state_as_a_dict.update({'auxiliary_information' : new_auxiliary_information})
+
+        auxiliary_information = self.state.get('auxiliary_information', {})
+        if auxiliary_information:
+            new_state_as_a_dict.update({'auxiliary_information' : copy.deepcopy(self.state['auxiliary_information'])})
 
         return State(self._collection_of_states, new_state_as_a_dict )
+    
+        # This is an earlier implementation which looks slower but we measure very marginal performance differences.
+        # new_initial_state = "{:s}".format(self.state['initial_state'])
+
+        # new_cumulative_probability = self.state['cumulative_probability']
+        
+        # new_optical_components = dict([])
+        # for oc_name, oc_comp in self.state['optical_components'].items():
+        #     new_comp_name = "{:s}".format(oc_name)
+        #     new_comp_values = dict([])
+        #     for k,v in oc_comp.items():
+        #         new_comp_values.update({k:v})
+        #     new_optical_components.update({new_comp_name :  new_comp_values})
+        
+        # new_classical_channel_values = self.state['classical_channel_values'].copy()
+        
+        # new_measurement_results = []
+        # for m_result in self.state['measurement_results']:
+        #     new_m_result = dict([])
+        #     for k,v in m_result.items():
+        #         new_m_result.update({k:v})
+        #     new_measurement_results.append(new_m_result)
+        
+        # new_state_as_a_dict = {   'initial_state' : new_initial_state,
+        #                     'cumulative_probability' : new_cumulative_probability,
+        #                     'optical_components' : new_optical_components, 
+        #                     'classical_channel_values' : new_classical_channel_values,
+        #                     'measurement_results' : new_measurement_results
+        #                     }
+        
+        # auxiliary_information = self.state.get('auxiliary_information', None)
+        # if auxiliary_information is not None and len(auxiliary_information) > 0:
+        #     new_auxiliary_information = copy.deepcopy(self.state['auxiliary_information'])
+        #     new_state_as_a_dict.update({'auxiliary_information' : new_auxiliary_information})
+
+        # return State(self._collection_of_states, new_state_as_a_dict )
 
     def initialize_this_state(self) -> None:
         """ Initializes the current state to valid default values. The initial state will be '000' (with the right amount of digits) 
             and the classical channels will be [0,0] (again with right amount of digits). Measurement history is empty. The state will not 
             contain any 'auxiliary_information'
         """        
         new_initial_state = list(self._dict_of_valid_component_names)[0]
@@ -529,19 +546,19 @@
 
         list_of_states = list(self._dict_of_valid_component_names.keys())
         optical_components = dict([])
         for index, value in enumerate(state_vector):
             # if value is below threshold set to zero
             if np.abs(value)**2 < self._threshold_probability_for_setting_to_zero:
                 state_vector[index] = 0
+                continue
             amplitude = state_vector[index]
             component = list_of_states[index]
             probability = np.abs(amplitude)**2
-            if probability != 0:
-                optical_components.update({component: {'amplitude': amplitude, 'probability': probability}})
+            optical_components.update({component: {'amplitude': amplitude, 'probability': probability}})
         self.state['optical_components'] = optical_components
 
         return
     
     def _rescale_optical_components(self) -> None:
         """ Rescales optical components by removing the ones with (too) low probability and re-normalizing the remaining ones.
             The limit is set by 'threshold_probability_for_setting_to_zero'
```

### Comparing `fockstatecircuit-1.0.1/src/fock_state_circuit/temporal_and_spectral_gate_functionality/collection_of_state_columns.py` & `fockstatecircuit-1.0.2/src/fock_state_circuit/temporal_and_spectral_gate_functionality/collection_of_state_columns.py`

 * *Files identical despite different names*

### Comparing `fockstatecircuit-1.0.1/src/fock_state_circuit/temporal_and_spectral_gate_functionality/column_of_states.py` & `fockstatecircuit-1.0.2/src/fock_state_circuit/temporal_and_spectral_gate_functionality/column_of_states.py`

 * *Files identical despite different names*

### Comparing `fockstatecircuit-1.0.1/src/fock_state_circuit/temporal_and_spectral_gate_functionality/interference_group.py` & `fockstatecircuit-1.0.2/src/fock_state_circuit/temporal_and_spectral_gate_functionality/interference_group.py`

 * *Files identical despite different names*

### Comparing `fockstatecircuit-1.0.1/src/fock_state_circuit/temporal_and_spectral_gate_functionality/temporal_functions.py` & `fockstatecircuit-1.0.2/src/fock_state_circuit/temporal_and_spectral_gate_functionality/temporal_functions.py`

 * *Files identical despite different names*

### Comparing `fockstatecircuit-1.0.1/src/fock_state_circuit/visualization/draw.py` & `fockstatecircuit-1.0.2/src/fock_state_circuit/visualization/draw.py`

 * *Files identical despite different names*

### Comparing `fockstatecircuit-1.0.1/src/fock_state_circuit/visualization/plot.py` & `fockstatecircuit-1.0.2/src/fock_state_circuit/visualization/plot.py`

 * *Files identical despite different names*

### Comparing `fockstatecircuit-1.0.1/tests/test_collection_of_states.py` & `fockstatecircuit-1.0.2/tests/test_collection_of_states.py`

 * *Files 1% similar despite different names*

```diff
@@ -720,31 +720,31 @@
     no_failure_found = no_failure_found and (state._digits_per_optical_channel == 2)
     initial_collection_of_states.extend(extra_optical_channels=1)
     initial_collection_of_states.reduce(classical_channels_to_keep=[0,3,4])
     initial_collection_of_states.adjust_length_of_fock_state(new_length_of_fock_state=3)
     state = initial_collection_of_states.get_state(initial_state='20202')
 
     no_failure_found = no_failure_found and all([
-        len(initial_collection_of_states._collection_of_states) == 2,
-        initial_collection_of_states._length_of_fock_state == 3,
-        initial_collection_of_states._no_of_classical_channels == 3,
-        initial_collection_of_states._no_of_optical_channels == 3,
-        len(initial_collection_of_states._list_of_fock_states) == 27,
-        len(list(initial_collection_of_states._list_of_fock_states)[0]) == 3,
-        list(initial_collection_of_states._list_of_fock_states)[-1][-1] == 2,
-        state._length_of_fock_state == 3,
-        state._no_of_optical_channels == 3,
-        state._no_of_classical_channels == 3,      
-        state._channel_0_left_in_state_name == False,
-        state._digits_per_optical_channel == 1,
-        state._dict_of_valid_component_names['000'] == [0,0,0],
-        state._threshold_probability_for_setting_to_zero == 0.1,
-        state._print_only_last_measurement == False,
-        True in state._check_valid_state(state_to_check = state),
-        state.measurement_results[0]['measurement_results'] == [1,1,1]])
+    len(initial_collection_of_states._collection_of_states) == 2,
+    initial_collection_of_states._length_of_fock_state == 3,
+    initial_collection_of_states._no_of_classical_channels == 3,
+    initial_collection_of_states._no_of_optical_channels == 3,
+    len(initial_collection_of_states._dict_of_valid_component_names) == 27,
+    len(list(initial_collection_of_states._dict_of_valid_component_names)[0]) == 3,
+    list(initial_collection_of_states._dict_of_valid_component_names.keys())[-1][-1] == '2',
+    state._length_of_fock_state == 3,
+    state._no_of_optical_channels == 3,
+    state._no_of_classical_channels == 3,      
+    state._channel_0_left_in_state_name == False,
+    state._digits_per_optical_channel == 1,
+    state._dict_of_valid_component_names['000'] == [0,0,0],
+    state._threshold_probability_for_setting_to_zero == 0.1,
+    state._print_only_last_measurement == False,
+    True in state._check_valid_state(state_to_check = state),
+    state.measurement_results[0]['measurement_results'] == [1,1,1]])
 
     assert no_failure_found
 
 def test_auxiliary_information():
     no_failure_found = True
     circuit = fsc.FockStateCircuit(length_of_fock_state = 4, 
                                     no_of_optical_channels = 5,
```

### Comparing `fockstatecircuit-1.0.1/tests/test_collection_of_states_plot.py` & `fockstatecircuit-1.0.2/tests/test_collection_of_states_plot.py`

 * *Files identical despite different names*

### Comparing `fockstatecircuit-1.0.1/tests/test_fock_state_circuit.py` & `fockstatecircuit-1.0.2/tests/test_fock_state_circuit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1912,22 +1912,22 @@
                             no_of_classical_channels=2,
                             circuit_name = 'test'
                             )
 
     def generic_function(input_collection,parameters):
         control_channel = parameters[0]
         target_channel = parameters[1]
-    
+        string_format_in_state_as_word = "{:0"+str(len(str(input_collection._length_of_fock_state-1)))+ "d}"
         for state in input_collection:
             new_components = dict([])
             old_components = state.optical_components
             for name, amp_prob in old_components.items():
                 old_values = state._dict_of_valid_component_names[name].copy()
                 old_values[target_channel] = (old_values[target_channel] + old_values[control_channel])%input_collection._length_of_fock_state
-                new_name = input_collection._get_state_name_from_list_of_photon_numbers(old_values)
+                new_name =''.join([("{:0"+str(len(str(input_collection._length_of_fock_state-1)))+ "d}").format(number) for number in old_values])
                 new_components.update({new_name:amp_prob})
             state.optical_components  = new_components
         return input_collection
 
     circuit.generic_function_on_collection(function=generic_function,parameters=[0,1])
 
     input_collection = fsc.CollectionOfStates(fock_state_circuit=circuit)
```

### Comparing `fockstatecircuit-1.0.1/tests/test_fock_state_circuit_applications.py` & `fockstatecircuit-1.0.2/tests/test_fock_state_circuit_applications.py`

 * *Files identical despite different names*

### Comparing `fockstatecircuit-1.0.1/tests/test_fock_state_circuit_draw.py` & `fockstatecircuit-1.0.2/tests/test_fock_state_circuit_draw.py`

 * *Files identical despite different names*

### Comparing `fockstatecircuit-1.0.1/tests/test_no_signalling_boxes.py` & `fockstatecircuit-1.0.2/tests/test_no_signalling_boxes.py`

 * *Files 19% similar despite different names*

```diff
@@ -357,8 +357,60 @@
             lst = []
             lst.append({'output_state': 'first pair, K = 1', 'probability': correlations[0]})
             # function should accept both 'correlation' as well as 'probability'
             lst.append({'output_state': 'second pair, K = 5', 'correlation': correlations[1]}) 
             dict_for_plotting.update({str(np.round(angle/np.pi,3)) + ' pi': lst})
         # plot the resulting correlations for the no-signalling boxes
         fsc.plot_correlations_for_NS_boxes(dict_for_plotting)
-        assert plt_test.compare_images(img1, img2, 0.001) is None
+        assert plt_test.compare_images(img1, img2, 0.001) is None
+
+def test_no_signalling_box_application_with_gates():
+    img1 = "./tests/test_drawings/testdrawing_no_signalling_histogram_from_gates.png"
+    img2 = img1.replace("testdrawing","reference")
+    generate_reference_images = False
+    if not generate_reference_images:
+        def save_drawing():
+            plt.savefig(img1)
+            return
+    else:
+        def save_drawing():
+            plt.savefig(img2)
+            return
+    with patch("fock_state_circuit.circuit.plt.show", wraps=save_drawing) as mock_bar:
+        N = 10
+        angles = [0]
+        circuit_is_already_drawn = False
+
+        ns_boxes = [{'channels_Ah_Av_Bh_Bv':[0,1,2,3],'quantumness_indicator':1},
+                    {'channels_Ah_Av_Bh_Bv':[4,5,6,7],'quantumness_indicator':5}]
+        for angle_first in angles:
+            dict_for_plotting = dict([])
+            for angle in [(a/N)*np.pi/2 for a in range(N)]:
+                circuit = fsc.FockStateCircuit(length_of_fock_state=3,no_of_optical_channels=8,no_of_classical_channels=8)
+                circuit.create_no_signalling_boxes(ns_boxes=ns_boxes)
+                circuit.half_wave_plate(channel_horizontal=2,channel_vertical=3,angle=angle)
+                circuit.half_wave_plate(channel_horizontal=6,channel_vertical=7,angle=angle)
+                circuit.half_wave_plate(channel_horizontal=0,channel_vertical=1,angle=angle_first)
+                circuit.half_wave_plate(channel_horizontal=4,channel_vertical=5,angle=angle_first)
+                circuit.measure_optical_to_classical(optical_channels_to_be_measured=[n for n in range(8)],classical_channels_to_be_written=[n for n in range(8)])
+
+                if not circuit_is_already_drawn:
+                    circuit.draw()
+                    circuit_is_already_drawn = True
+
+                collection = fsc.CollectionOfStates(fock_state_circuit=circuit,input_collection_as_a_dict=dict([]))
+                state = fsc.State(collection_of_states=collection)
+                collection.add_state(state)
+                output_collection = circuit.evaluate_circuit(collection_of_states_input=collection)
+
+                channel_combis_for_correlation = [(0,2),(4,6)]
+                label_for_channel_combinations = ['first pair, K = 1','second pair, K = 5']
+                
+                correlations = output_collection.plot_correlations(channel_combis_for_correlation=channel_combis_for_correlation,
+                                                                correlation_output_instead_of_plot=True)['no_signalling_boxes']
+                lst = []
+                lst.append({'output_state': 'first pair, K = 1', 'probability': correlations[0]})
+                lst.append({'output_state': 'second pair, K = 5', 'probability': correlations[1]})
+                dict_for_plotting.update({str(np.round(angle/np.pi,3)) + ' pi': lst})
+            # plot the resulting correlations for the no-signalling boxes
+            fsc.plot_correlations_from_dict(dict_for_plotting)
+            assert plt_test.compare_images(img1, img2, 0.001) is None
```

### Comparing `fockstatecircuit-1.0.1/tests/test_photon_resolved_collection.py` & `fockstatecircuit-1.0.2/tests/test_photon_resolved_collection.py`

 * *Files identical despite different names*

### Comparing `fockstatecircuit-1.0.1/tests/test_state.py` & `fockstatecircuit-1.0.2/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `fockstatecircuit-1.0.1/tests/test_time_delay_applications.py` & `fockstatecircuit-1.0.2/tests/test_time_delay_applications.py`

 * *Files identical despite different names*


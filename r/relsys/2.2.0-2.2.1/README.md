# Comparing `tmp/relsys-2.2.0.tar.gz` & `tmp/relsys-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relsys-2.2.0.tar", last modified: Mon Apr 29 17:09:02 2024, max compression
+gzip compressed data, was "relsys-2.2.1.tar", last modified: Wed May  1 16:58:27 2024, max compression
```

## Comparing `relsys-2.2.0.tar` & `relsys-2.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 anders    (1000) anders    (1000)        0 2024-04-29 17:09:02.476600 relsys-2.2.0/
--rw-r--r--   0 anders    (1000) anders    (1000)     1077 2024-04-29 17:01:31.000000 relsys-2.2.0/LICENSE
--rw-rw-r--   0 anders    (1000) anders    (1000)       39 2024-04-29 16:55:50.000000 relsys-2.2.0/MANIFEST.in
--rw-r--r--   0 anders    (1000) anders    (1000)     8427 2024-04-29 17:09:02.476600 relsys-2.2.0/PKG-INFO
--rw-r--r--   0 anders    (1000) anders    (1000)     7997 2024-04-29 16:40:36.000000 relsys-2.2.0/README.md
--rw-rw-r--   0 anders    (1000) anders    (1000)      789 2024-04-29 17:08:06.000000 relsys-2.2.0/pyproject.toml
--rw-rw-r--   0 anders    (1000) anders    (1000)       38 2024-04-29 17:09:02.476600 relsys-2.2.0/setup.cfg
-drwxrwxr-x   0 anders    (1000) anders    (1000)        0 2024-04-29 17:09:02.476600 relsys-2.2.0/src/
-drwxrwxr-x   0 anders    (1000) anders    (1000)        0 2024-04-29 17:09:02.476600 relsys-2.2.0/src/relsys/
--rw-r--r--   0 anders    (1000) anders    (1000)       30 2024-04-29 14:45:20.000000 relsys-2.2.0/src/relsys/__init__.py
--rw-r--r--   0 anders    (1000) anders    (1000)     2503 2024-04-29 16:38:58.000000 relsys-2.2.0/src/relsys/model.py
--rw-r--r--   0 anders    (1000) anders    (1000)   310272 2024-04-29 15:38:48.000000 relsys-2.2.0/src/relsys/relsys.cp310-win_amd64.pyd
--rwxrwxr-x   0 anders    (1000) anders    (1000)   720872 2024-04-29 16:07:39.000000 relsys-2.2.0/src/relsys/relsys.cpython-310-x86_64-linux-gnu.so
-drwxrwxr-x   0 anders    (1000) anders    (1000)        0 2024-04-29 17:09:02.476600 relsys-2.2.0/src/relsys.egg-info/
--rw-r--r--   0 anders    (1000) anders    (1000)     8427 2024-04-29 17:09:02.000000 relsys-2.2.0/src/relsys.egg-info/PKG-INFO
--rw-rw-r--   0 anders    (1000) anders    (1000)      311 2024-04-29 17:09:02.000000 relsys-2.2.0/src/relsys.egg-info/SOURCES.txt
--rw-rw-r--   0 anders    (1000) anders    (1000)        1 2024-04-29 17:09:02.000000 relsys-2.2.0/src/relsys.egg-info/dependency_links.txt
--rw-rw-r--   0 anders    (1000) anders    (1000)        7 2024-04-29 17:09:02.000000 relsys-2.2.0/src/relsys.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-01 16:58:27.691270 relsys-2.2.1/
+-rw-rw-rw-   0        0        0     1077 2024-04-29 17:01:30.000000 relsys-2.2.1/LICENSE
+-rw-rw-rw-   0        0        0       39 2024-04-29 16:55:50.000000 relsys-2.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     8639 2024-05-01 16:58:27.688149 relsys-2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7997 2024-04-29 16:36:18.000000 relsys-2.2.1/README.md
+-rw-rw-rw-   0        0        0      789 2024-05-01 16:58:03.000000 relsys-2.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-01 16:58:27.691270 relsys-2.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-01 16:58:27.586482 relsys-2.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-01 16:58:27.672474 relsys-2.2.1/src/relsys/
+-rw-rw-rw-   0        0        0       30 2024-04-29 14:45:20.000000 relsys-2.2.1/src/relsys/__init__.py
+-rw-rw-rw-   0        0        0     2503 2024-04-29 16:38:49.000000 relsys-2.2.1/src/relsys/model.py
+-rw-rw-rw-   0        0        0   310272 2024-04-29 15:38:48.000000 relsys-2.2.1/src/relsys/relsys.cp310-win_amd64.pyd
+-rw-rw-rw-   0        0        0   720872 2024-04-29 16:07:39.000000 relsys-2.2.1/src/relsys/relsys.cpython-310-x86_64-linux-gnu.so
+drwxrwxrwx   0        0        0        0 2024-05-01 16:58:27.685728 relsys-2.2.1/src/relsys.egg-info/
+-rw-rw-rw-   0        0        0     8639 2024-05-01 16:58:27.000000 relsys-2.2.1/src/relsys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2024-05-01 16:58:27.000000 relsys-2.2.1/src/relsys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 16:58:27.000000 relsys-2.2.1/src/relsys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-01 16:58:27.000000 relsys-2.2.1/src/relsys.egg-info/top_level.txt
```

### Comparing `relsys-2.2.0/LICENSE` & `relsys-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `relsys-2.2.0/PKG-INFO` & `relsys-2.2.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,212 +1,197 @@
-Metadata-Version: 2.1
-Name: relsys
-Version: 2.2.0
-Summary: A tool for evaluating a system of queues with finite capacity that are connected through customer relocations.
-Author-email: Anders Reenberg Andersen <andersra@live.dk>
-Project-URL: Homepage, https://github.com/areenberg/RelSys
-Project-URL: Issues, https://github.com/areenberg/RelSys/issues
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# RelSys (**Rel**ocation **Sys**tem)
-RelSys is a tool for evaluating a system of queues where arriving customers can be relocated to an alternative queue if none of the servers in the preferred queue are idle.
-
-# Table of contents
-
-1. Description of RelSys
-2. How to use
-3. How to cite
-4. Licence
-
-# Description of RelSys
-
-Consider a number of parallel queues where the capacity of the queue equals the number of servers. That is, queues where customers arrive according to a Poisson process and have exponentially distributed service-time. In the common M/M/c/c queue (also denoted the Erlang loss or Erlang-B system), a customer is rejected and lost from the system if all the servers are occupied upon arrival. In RelSys, we allow customers to be transferred with a probability to one of the other queues. If there is an idle server in the alternative queue, the customer is accepted and served with an exponentially distributed time with the same rate-parameter as the customer would have in the preferred queue. The figure below depicts an example featuring two queues where customers are relocated (i.e. transferred) with a probability to the other queue whenever the preferred queue is full. 
-
-## Input parameters
-
-RelSys uses five types of input parameters:
-
-* An arrival rate vector, where each element corresponds to a customer type.
-* A service time vector, where each element corresponds to a customer type.
-* A relocation probability matrix. Rows correspond to customer types and columns to queues.  
-* A capacity vector. Each element corresponds to a queue.
-* A preferrence vector. Each element indicates the preferred queue of each customer type.
-
-## Output types
-
-RelSys has six output types:
-
-* Occupancy *probability* distributions.
-* Occupancy *frequency* distributions (only available if the system was evaluated using simulation).
-* Shortage probabilities.
-* Availability probabilities.
-* Expected occupancy.
-* Expected fraction of occupied capacity.
-
-All outputs, except for the *expected occupancy* and *expected fraction of occupied capacity*, can be evaluated from two customer perspectives: The perspective of the customers preferring the queues, and the perspective of all customers arriving to the queues.    
-
-# How to use
-
-## Installation
-
-Download and install `relsys` directly from PyPI.
-
-```
-pip install relsys
-```
-
-## Usage
-
-Start by importing the module,
-
-```python
-import relsys
-```
-
-Now, specify the input parameters for the model. In this example, we consider a system containing 4 customer types and 4 queues.
-
-```python
-arrivalRates = [0.8,2.5,0.6,2.8]
-
-serviceTimes = [10,5,10,8]
-
-capacity = [15,20,10,30]
-
-relocationProbabilities = [[0.0,0.4,0.1,0.5],
-                           [0.3,0.0,0.5,0.0],
-                           [0.0,0.5,0.0,0.5],
-                           [0.2,0.3,0.5,0.0]]
-
-preferredQueue = [0,1,2,3]
-```
-
-Create the model object and import the parameters,
-
-```python
-mdl = relsys.model(arrivalRates,serviceTimes,capacity,relocationProbabilities,preferredQueue)
-```
-
-The model can now be evaluated with `run`,
-
-```python
-mdl.run()
-```
-
-Return the resulting occupancy distributions with `getDensity` and shortage probabilities with `getShortageProb`,
-
-```python
-for queueIdx in range(4):
-    print(mdl.getDensity(queueIdx))
-
-for queueIdx in range(4):
-    print(mdl.getShortageProb(queueIdx))
-```
-
-### The complete example
-
-```python
-#import the module
-import relsys 
-
-#arrival rates of each customer type
-arrivalRates = [0.8,2.5,0.6,2.8]
-
-#mean service time of each customer type
-serviceTimes = [10,5,10,8]
-
-#capacity of each queue
-capacity = [15,20,10,30]
-
-#fraction of rejected customers that are moved to an alternative queue node
-#this is a number of customers x number of queues matrix
-relocationProbabilities = [[0.0,0.4,0.1,0.5],
-                           [0.3,0.0,0.5,0.0],
-                           [0.0,0.5,0.0,0.5],
-                           [0.2,0.3,0.5,0.0]]
-
-#queue indices preferred by each customer type
-preferredQueue = [0,1,2,3]
-
-#create the model object and import the parameters
-mdl = relsys.model(arrivalRates,serviceTimes,capacity,relocationProbabilities,preferredQueue)
-
-#run the model
-mdl.run()
-
-#check the resulting occupancy distribution of each queue 
-for queueIdx in range(4):
-    print(mdl.getDensity(queueIdx))
-
-#check the resulting shortage probabilities of each queue 
-for queueIdx in range(4):
-    print(mdl.getShortageProb(queueIdx))
-```
-
-## List of functions
-
-### Model settings
-
-* `setType(string mdltype)`. Set the method to use in the evaluation of the model ("simulation" (default), "approximation", "auto"). 
-* `queuesEval(list qEvalIdx)`. Set the indices of queues to evaluate.
-* `equalize(bool equalize)`. Specify if service times should be equalized and loads correspondingly adjusted (True: On, False: Off (default)).
-* `setVerbose(bool set)`. Control verbose (True: On, False: Off (default)).
-* `setSeed(int sd)`. Set the seed.
-* `setAccSamType(string stype)`. Set the accuracy estimation type for the simulation ("preferred" (default), "all").
-* `setSimTolerance(double tol)`. Set the tolerance level for the accuracy estimation in the simulation (default: 5e-3).
-* `setBurnIn(double bin)`. Set the burn-in time of the simulation.
-* `setSimTime(double mnTime)`. Set the simulation time.
-* `setSamples(int mnSamples)`. Set the minimum number of open/shortage samples.
-* `setHyperPhases(int openStates, int blockedStates)`. Set the number of phases in the hyper-exponential distributions accounting for the open/shortage time.
-
-### Run calculations
-
-* `run()`. Evaluate the model using the input parameters.
-
-### Get results
-
-* `getDensity(int queueIdx=0, string type="preferred")`. Return the density distribution of a queue. The second argument specifies the arrival type: "all" and "preferred" (default).
-* `getFreq(int queueIdx=0, string type="preferred")`. Return the frequency distribution of a queue. The second argument specifies the arrival type: "all" and "preferred" (default).
-* `getShortageProb(int queueIdx=0, string type="preferred")`. Return the shortage probability of a queue. The second argument specifies the arrival type: "all" and "preferred" (default).
-* `getAvailProb(int queueIdx=0, string type="preferred")`. Return the probability that at least one server is available. The second argument specifies the arrival type: "all" and "preferred" (default).
-* `getExpOccupany(int queueIdx=0)`. Return the expected number of occupied servers.
-* `getExpOccFraction(int queueIdx=0)`. Return the expected fraction of occupied servers.
-
-### Return imported variables
-
-* `getArrivalRates()`. Return the imported arrival rates.
-* `getServiceTimes()`. Return the imported service times.
-* `getCapacity()`. Return the imported capacities.
-* `getReloc()`. Return the imported relocation probabilities.
-* `getPreferredQueue()`. Return the imported preferred queues.
-
-# Capsule on Code Ocean
-
-We have published a capsule for the Linux CLI on Code Ocean. The URL and DOI for the capsule follows below:
-
-* URL: https://codeocean.com/capsule/7104737/tree
-* DOI: https://doi.org/10.24433/CO.2728562.v1
-
-# How to cite
-
-[![DOI](https://zenodo.org/badge/293829002.svg)](https://zenodo.org/badge/latestdoi/293829002)
-
-# License
-
-Copyright 2024 Anders Reenberg Andersen.
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
+# RelSys (**Rel**ocation **Sys**tem)
+RelSys is a tool for evaluating a system of queues where arriving customers can be relocated to an alternative queue if none of the servers in the preferred queue are idle.
+
+# Table of contents
+
+1. Description of RelSys
+2. How to use
+3. How to cite
+4. Licence
+
+# Description of RelSys
+
+Consider a number of parallel queues where the capacity of the queue equals the number of servers. That is, queues where customers arrive according to a Poisson process and have exponentially distributed service-time. In the common M/M/c/c queue (also denoted the Erlang loss or Erlang-B system), a customer is rejected and lost from the system if all the servers are occupied upon arrival. In RelSys, we allow customers to be transferred with a probability to one of the other queues. If there is an idle server in the alternative queue, the customer is accepted and served with an exponentially distributed time with the same rate-parameter as the customer would have in the preferred queue. The figure below depicts an example featuring two queues where customers are relocated (i.e. transferred) with a probability to the other queue whenever the preferred queue is full. 
+
+## Input parameters
+
+RelSys uses five types of input parameters:
+
+* An arrival rate vector, where each element corresponds to a customer type.
+* A service time vector, where each element corresponds to a customer type.
+* A relocation probability matrix. Rows correspond to customer types and columns to queues.  
+* A capacity vector. Each element corresponds to a queue.
+* A preferrence vector. Each element indicates the preferred queue of each customer type.
+
+## Output types
+
+RelSys has six output types:
+
+* Occupancy *probability* distributions.
+* Occupancy *frequency* distributions (only available if the system was evaluated using simulation).
+* Shortage probabilities.
+* Availability probabilities.
+* Expected occupancy.
+* Expected fraction of occupied capacity.
+
+All outputs, except for the *expected occupancy* and *expected fraction of occupied capacity*, can be evaluated from two customer perspectives: The perspective of the customers preferring the queues, and the perspective of all customers arriving to the queues.    
+
+# How to use
+
+## Installation
+
+Download and install `relsys` directly from PyPI.
+
+```
+pip install relsys
+```
+
+## Usage
+
+Start by importing the module,
+
+```python
+import relsys
+```
+
+Now, specify the input parameters for the model. In this example, we consider a system containing 4 customer types and 4 queues.
+
+```python
+arrivalRates = [0.8,2.5,0.6,2.8]
+
+serviceTimes = [10,5,10,8]
+
+capacity = [15,20,10,30]
+
+relocationProbabilities = [[0.0,0.4,0.1,0.5],
+                           [0.3,0.0,0.5,0.0],
+                           [0.0,0.5,0.0,0.5],
+                           [0.2,0.3,0.5,0.0]]
+
+preferredQueue = [0,1,2,3]
+```
+
+Create the model object and import the parameters,
+
+```python
+mdl = relsys.model(arrivalRates,serviceTimes,capacity,relocationProbabilities,preferredQueue)
+```
+
+The model can now be evaluated with `run`,
+
+```python
+mdl.run()
+```
+
+Return the resulting occupancy distributions with `getDensity` and shortage probabilities with `getShortageProb`,
+
+```python
+for queueIdx in range(4):
+    print(mdl.getDensity(queueIdx))
+
+for queueIdx in range(4):
+    print(mdl.getShortageProb(queueIdx))
+```
+
+### The complete example
+
+```python
+#import the module
+import relsys 
+
+#arrival rates of each customer type
+arrivalRates = [0.8,2.5,0.6,2.8]
+
+#mean service time of each customer type
+serviceTimes = [10,5,10,8]
+
+#capacity of each queue
+capacity = [15,20,10,30]
+
+#fraction of rejected customers that are moved to an alternative queue node
+#this is a number of customers x number of queues matrix
+relocationProbabilities = [[0.0,0.4,0.1,0.5],
+                           [0.3,0.0,0.5,0.0],
+                           [0.0,0.5,0.0,0.5],
+                           [0.2,0.3,0.5,0.0]]
+
+#queue indices preferred by each customer type
+preferredQueue = [0,1,2,3]
+
+#create the model object and import the parameters
+mdl = relsys.model(arrivalRates,serviceTimes,capacity,relocationProbabilities,preferredQueue)
+
+#run the model
+mdl.run()
+
+#check the resulting occupancy distribution of each queue 
+for queueIdx in range(4):
+    print(mdl.getDensity(queueIdx))
+
+#check the resulting shortage probabilities of each queue 
+for queueIdx in range(4):
+    print(mdl.getShortageProb(queueIdx))
+```
+
+## List of functions
+
+### Model settings
+
+* `setType(string mdltype)`. Set the method to use in the evaluation of the model ("simulation" (default), "approximation", "auto"). 
+* `queuesEval(list qEvalIdx)`. Set the indices of queues to evaluate.
+* `equalize(bool equalize)`. Specify if service times should be equalized and loads correspondingly adjusted (True: On, False: Off (default)).
+* `setVerbose(bool set)`. Control verbose (True: On, False: Off (default)).
+* `setSeed(int sd)`. Set the seed.
+* `setAccSamType(string stype)`. Set the accuracy estimation type for the simulation ("preferred" (default), "all").
+* `setSimTolerance(double tol)`. Set the tolerance level for the accuracy estimation in the simulation (default: 5e-3).
+* `setBurnIn(double bin)`. Set the burn-in time of the simulation.
+* `setSimTime(double mnTime)`. Set the simulation time.
+* `setSamples(int mnSamples)`. Set the minimum number of open/shortage samples.
+* `setHyperPhases(int openStates, int blockedStates)`. Set the number of phases in the hyper-exponential distributions accounting for the open/shortage time.
+
+### Run calculations
+
+* `run()`. Evaluate the model using the input parameters.
+
+### Get results
+
+* `getDensity(int queueIdx=0, string type="preferred")`. Return the density distribution of a queue. The second argument specifies the arrival type: "all" and "preferred" (default).
+* `getFreq(int queueIdx=0, string type="preferred")`. Return the frequency distribution of a queue. The second argument specifies the arrival type: "all" and "preferred" (default).
+* `getShortageProb(int queueIdx=0, string type="preferred")`. Return the shortage probability of a queue. The second argument specifies the arrival type: "all" and "preferred" (default).
+* `getAvailProb(int queueIdx=0, string type="preferred")`. Return the probability that at least one server is available. The second argument specifies the arrival type: "all" and "preferred" (default).
+* `getExpOccupany(int queueIdx=0)`. Return the expected number of occupied servers.
+* `getExpOccFraction(int queueIdx=0)`. Return the expected fraction of occupied servers.
+
+### Return imported variables
+
+* `getArrivalRates()`. Return the imported arrival rates.
+* `getServiceTimes()`. Return the imported service times.
+* `getCapacity()`. Return the imported capacities.
+* `getReloc()`. Return the imported relocation probabilities.
+* `getPreferredQueue()`. Return the imported preferred queues.
+
+# Capsule on Code Ocean
+
+We have published a capsule for the Linux CLI on Code Ocean. The URL and DOI for the capsule follows below:
+
+* URL: https://codeocean.com/capsule/7104737/tree
+* DOI: https://doi.org/10.24433/CO.2728562.v1
+
+# How to cite
+
+[![DOI](https://zenodo.org/badge/293829002.svg)](https://zenodo.org/badge/latestdoi/293829002)
+
+# License
+
+Copyright 2024 Anders Reenberg Andersen.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
```

### Comparing `relsys-2.2.0/README.md` & `relsys-2.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: relsys
+Version: 2.2.1
+Summary: A tool for evaluating a system of queues with finite capacity that are connected through customer relocations.
+Author-email: Anders Reenberg Andersen <andersra@live.dk>
+Project-URL: Homepage, https://github.com/areenberg/RelSys
+Project-URL: Issues, https://github.com/areenberg/RelSys/issues
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: ==3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # RelSys (**Rel**ocation **Sys**tem)
 RelSys is a tool for evaluating a system of queues where arriving customers can be relocated to an alternative queue if none of the servers in the preferred queue are idle.
 
 # Table of contents
 
 1. Description of RelSys
 2. How to use
```

### Comparing `relsys-2.2.0/pyproject.toml` & `relsys-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "relsys"
-version = "2.2.0"
+version = "2.2.1"
 authors = [
   { name="Anders Reenberg Andersen", email="andersra@live.dk" },
 ]
 description = "A tool for evaluating a system of queues with finite capacity that are connected through customer relocations."
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = "==3.10"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `relsys-2.2.0/src/relsys/model.py` & `relsys-2.2.1/src/relsys/model.py`

 * *Files identical despite different names*

### Comparing `relsys-2.2.0/src/relsys/relsys.cpython-310-x86_64-linux-gnu.so` & `relsys-2.2.1/src/relsys/relsys.cpython-310-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `relsys-2.2.0/src/relsys.egg-info/PKG-INFO` & `relsys-2.2.1/src/relsys.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,212 +1,212 @@
-Metadata-Version: 2.1
-Name: relsys
-Version: 2.2.0
-Summary: A tool for evaluating a system of queues with finite capacity that are connected through customer relocations.
-Author-email: Anders Reenberg Andersen <andersra@live.dk>
-Project-URL: Homepage, https://github.com/areenberg/RelSys
-Project-URL: Issues, https://github.com/areenberg/RelSys/issues
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# RelSys (**Rel**ocation **Sys**tem)
-RelSys is a tool for evaluating a system of queues where arriving customers can be relocated to an alternative queue if none of the servers in the preferred queue are idle.
-
-# Table of contents
-
-1. Description of RelSys
-2. How to use
-3. How to cite
-4. Licence
-
-# Description of RelSys
-
-Consider a number of parallel queues where the capacity of the queue equals the number of servers. That is, queues where customers arrive according to a Poisson process and have exponentially distributed service-time. In the common M/M/c/c queue (also denoted the Erlang loss or Erlang-B system), a customer is rejected and lost from the system if all the servers are occupied upon arrival. In RelSys, we allow customers to be transferred with a probability to one of the other queues. If there is an idle server in the alternative queue, the customer is accepted and served with an exponentially distributed time with the same rate-parameter as the customer would have in the preferred queue. The figure below depicts an example featuring two queues where customers are relocated (i.e. transferred) with a probability to the other queue whenever the preferred queue is full. 
-
-## Input parameters
-
-RelSys uses five types of input parameters:
-
-* An arrival rate vector, where each element corresponds to a customer type.
-* A service time vector, where each element corresponds to a customer type.
-* A relocation probability matrix. Rows correspond to customer types and columns to queues.  
-* A capacity vector. Each element corresponds to a queue.
-* A preferrence vector. Each element indicates the preferred queue of each customer type.
-
-## Output types
-
-RelSys has six output types:
-
-* Occupancy *probability* distributions.
-* Occupancy *frequency* distributions (only available if the system was evaluated using simulation).
-* Shortage probabilities.
-* Availability probabilities.
-* Expected occupancy.
-* Expected fraction of occupied capacity.
-
-All outputs, except for the *expected occupancy* and *expected fraction of occupied capacity*, can be evaluated from two customer perspectives: The perspective of the customers preferring the queues, and the perspective of all customers arriving to the queues.    
-
-# How to use
-
-## Installation
-
-Download and install `relsys` directly from PyPI.
-
-```
-pip install relsys
-```
-
-## Usage
-
-Start by importing the module,
-
-```python
-import relsys
-```
-
-Now, specify the input parameters for the model. In this example, we consider a system containing 4 customer types and 4 queues.
-
-```python
-arrivalRates = [0.8,2.5,0.6,2.8]
-
-serviceTimes = [10,5,10,8]
-
-capacity = [15,20,10,30]
-
-relocationProbabilities = [[0.0,0.4,0.1,0.5],
-                           [0.3,0.0,0.5,0.0],
-                           [0.0,0.5,0.0,0.5],
-                           [0.2,0.3,0.5,0.0]]
-
-preferredQueue = [0,1,2,3]
-```
-
-Create the model object and import the parameters,
-
-```python
-mdl = relsys.model(arrivalRates,serviceTimes,capacity,relocationProbabilities,preferredQueue)
-```
-
-The model can now be evaluated with `run`,
-
-```python
-mdl.run()
-```
-
-Return the resulting occupancy distributions with `getDensity` and shortage probabilities with `getShortageProb`,
-
-```python
-for queueIdx in range(4):
-    print(mdl.getDensity(queueIdx))
-
-for queueIdx in range(4):
-    print(mdl.getShortageProb(queueIdx))
-```
-
-### The complete example
-
-```python
-#import the module
-import relsys 
-
-#arrival rates of each customer type
-arrivalRates = [0.8,2.5,0.6,2.8]
-
-#mean service time of each customer type
-serviceTimes = [10,5,10,8]
-
-#capacity of each queue
-capacity = [15,20,10,30]
-
-#fraction of rejected customers that are moved to an alternative queue node
-#this is a number of customers x number of queues matrix
-relocationProbabilities = [[0.0,0.4,0.1,0.5],
-                           [0.3,0.0,0.5,0.0],
-                           [0.0,0.5,0.0,0.5],
-                           [0.2,0.3,0.5,0.0]]
-
-#queue indices preferred by each customer type
-preferredQueue = [0,1,2,3]
-
-#create the model object and import the parameters
-mdl = relsys.model(arrivalRates,serviceTimes,capacity,relocationProbabilities,preferredQueue)
-
-#run the model
-mdl.run()
-
-#check the resulting occupancy distribution of each queue 
-for queueIdx in range(4):
-    print(mdl.getDensity(queueIdx))
-
-#check the resulting shortage probabilities of each queue 
-for queueIdx in range(4):
-    print(mdl.getShortageProb(queueIdx))
-```
-
-## List of functions
-
-### Model settings
-
-* `setType(string mdltype)`. Set the method to use in the evaluation of the model ("simulation" (default), "approximation", "auto"). 
-* `queuesEval(list qEvalIdx)`. Set the indices of queues to evaluate.
-* `equalize(bool equalize)`. Specify if service times should be equalized and loads correspondingly adjusted (True: On, False: Off (default)).
-* `setVerbose(bool set)`. Control verbose (True: On, False: Off (default)).
-* `setSeed(int sd)`. Set the seed.
-* `setAccSamType(string stype)`. Set the accuracy estimation type for the simulation ("preferred" (default), "all").
-* `setSimTolerance(double tol)`. Set the tolerance level for the accuracy estimation in the simulation (default: 5e-3).
-* `setBurnIn(double bin)`. Set the burn-in time of the simulation.
-* `setSimTime(double mnTime)`. Set the simulation time.
-* `setSamples(int mnSamples)`. Set the minimum number of open/shortage samples.
-* `setHyperPhases(int openStates, int blockedStates)`. Set the number of phases in the hyper-exponential distributions accounting for the open/shortage time.
-
-### Run calculations
-
-* `run()`. Evaluate the model using the input parameters.
-
-### Get results
-
-* `getDensity(int queueIdx=0, string type="preferred")`. Return the density distribution of a queue. The second argument specifies the arrival type: "all" and "preferred" (default).
-* `getFreq(int queueIdx=0, string type="preferred")`. Return the frequency distribution of a queue. The second argument specifies the arrival type: "all" and "preferred" (default).
-* `getShortageProb(int queueIdx=0, string type="preferred")`. Return the shortage probability of a queue. The second argument specifies the arrival type: "all" and "preferred" (default).
-* `getAvailProb(int queueIdx=0, string type="preferred")`. Return the probability that at least one server is available. The second argument specifies the arrival type: "all" and "preferred" (default).
-* `getExpOccupany(int queueIdx=0)`. Return the expected number of occupied servers.
-* `getExpOccFraction(int queueIdx=0)`. Return the expected fraction of occupied servers.
-
-### Return imported variables
-
-* `getArrivalRates()`. Return the imported arrival rates.
-* `getServiceTimes()`. Return the imported service times.
-* `getCapacity()`. Return the imported capacities.
-* `getReloc()`. Return the imported relocation probabilities.
-* `getPreferredQueue()`. Return the imported preferred queues.
-
-# Capsule on Code Ocean
-
-We have published a capsule for the Linux CLI on Code Ocean. The URL and DOI for the capsule follows below:
-
-* URL: https://codeocean.com/capsule/7104737/tree
-* DOI: https://doi.org/10.24433/CO.2728562.v1
-
-# How to cite
-
-[![DOI](https://zenodo.org/badge/293829002.svg)](https://zenodo.org/badge/latestdoi/293829002)
-
-# License
-
-Copyright 2024 Anders Reenberg Andersen.
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
+Metadata-Version: 2.1
+Name: relsys
+Version: 2.2.1
+Summary: A tool for evaluating a system of queues with finite capacity that are connected through customer relocations.
+Author-email: Anders Reenberg Andersen <andersra@live.dk>
+Project-URL: Homepage, https://github.com/areenberg/RelSys
+Project-URL: Issues, https://github.com/areenberg/RelSys/issues
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: ==3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# RelSys (**Rel**ocation **Sys**tem)
+RelSys is a tool for evaluating a system of queues where arriving customers can be relocated to an alternative queue if none of the servers in the preferred queue are idle.
+
+# Table of contents
+
+1. Description of RelSys
+2. How to use
+3. How to cite
+4. Licence
+
+# Description of RelSys
+
+Consider a number of parallel queues where the capacity of the queue equals the number of servers. That is, queues where customers arrive according to a Poisson process and have exponentially distributed service-time. In the common M/M/c/c queue (also denoted the Erlang loss or Erlang-B system), a customer is rejected and lost from the system if all the servers are occupied upon arrival. In RelSys, we allow customers to be transferred with a probability to one of the other queues. If there is an idle server in the alternative queue, the customer is accepted and served with an exponentially distributed time with the same rate-parameter as the customer would have in the preferred queue. The figure below depicts an example featuring two queues where customers are relocated (i.e. transferred) with a probability to the other queue whenever the preferred queue is full. 
+
+## Input parameters
+
+RelSys uses five types of input parameters:
+
+* An arrival rate vector, where each element corresponds to a customer type.
+* A service time vector, where each element corresponds to a customer type.
+* A relocation probability matrix. Rows correspond to customer types and columns to queues.  
+* A capacity vector. Each element corresponds to a queue.
+* A preferrence vector. Each element indicates the preferred queue of each customer type.
+
+## Output types
+
+RelSys has six output types:
+
+* Occupancy *probability* distributions.
+* Occupancy *frequency* distributions (only available if the system was evaluated using simulation).
+* Shortage probabilities.
+* Availability probabilities.
+* Expected occupancy.
+* Expected fraction of occupied capacity.
+
+All outputs, except for the *expected occupancy* and *expected fraction of occupied capacity*, can be evaluated from two customer perspectives: The perspective of the customers preferring the queues, and the perspective of all customers arriving to the queues.    
+
+# How to use
+
+## Installation
+
+Download and install `relsys` directly from PyPI.
+
+```
+pip install relsys
+```
+
+## Usage
+
+Start by importing the module,
+
+```python
+import relsys
+```
+
+Now, specify the input parameters for the model. In this example, we consider a system containing 4 customer types and 4 queues.
+
+```python
+arrivalRates = [0.8,2.5,0.6,2.8]
+
+serviceTimes = [10,5,10,8]
+
+capacity = [15,20,10,30]
+
+relocationProbabilities = [[0.0,0.4,0.1,0.5],
+                           [0.3,0.0,0.5,0.0],
+                           [0.0,0.5,0.0,0.5],
+                           [0.2,0.3,0.5,0.0]]
+
+preferredQueue = [0,1,2,3]
+```
+
+Create the model object and import the parameters,
+
+```python
+mdl = relsys.model(arrivalRates,serviceTimes,capacity,relocationProbabilities,preferredQueue)
+```
+
+The model can now be evaluated with `run`,
+
+```python
+mdl.run()
+```
+
+Return the resulting occupancy distributions with `getDensity` and shortage probabilities with `getShortageProb`,
+
+```python
+for queueIdx in range(4):
+    print(mdl.getDensity(queueIdx))
+
+for queueIdx in range(4):
+    print(mdl.getShortageProb(queueIdx))
+```
+
+### The complete example
+
+```python
+#import the module
+import relsys 
+
+#arrival rates of each customer type
+arrivalRates = [0.8,2.5,0.6,2.8]
+
+#mean service time of each customer type
+serviceTimes = [10,5,10,8]
+
+#capacity of each queue
+capacity = [15,20,10,30]
+
+#fraction of rejected customers that are moved to an alternative queue node
+#this is a number of customers x number of queues matrix
+relocationProbabilities = [[0.0,0.4,0.1,0.5],
+                           [0.3,0.0,0.5,0.0],
+                           [0.0,0.5,0.0,0.5],
+                           [0.2,0.3,0.5,0.0]]
+
+#queue indices preferred by each customer type
+preferredQueue = [0,1,2,3]
+
+#create the model object and import the parameters
+mdl = relsys.model(arrivalRates,serviceTimes,capacity,relocationProbabilities,preferredQueue)
+
+#run the model
+mdl.run()
+
+#check the resulting occupancy distribution of each queue 
+for queueIdx in range(4):
+    print(mdl.getDensity(queueIdx))
+
+#check the resulting shortage probabilities of each queue 
+for queueIdx in range(4):
+    print(mdl.getShortageProb(queueIdx))
+```
+
+## List of functions
+
+### Model settings
+
+* `setType(string mdltype)`. Set the method to use in the evaluation of the model ("simulation" (default), "approximation", "auto"). 
+* `queuesEval(list qEvalIdx)`. Set the indices of queues to evaluate.
+* `equalize(bool equalize)`. Specify if service times should be equalized and loads correspondingly adjusted (True: On, False: Off (default)).
+* `setVerbose(bool set)`. Control verbose (True: On, False: Off (default)).
+* `setSeed(int sd)`. Set the seed.
+* `setAccSamType(string stype)`. Set the accuracy estimation type for the simulation ("preferred" (default), "all").
+* `setSimTolerance(double tol)`. Set the tolerance level for the accuracy estimation in the simulation (default: 5e-3).
+* `setBurnIn(double bin)`. Set the burn-in time of the simulation.
+* `setSimTime(double mnTime)`. Set the simulation time.
+* `setSamples(int mnSamples)`. Set the minimum number of open/shortage samples.
+* `setHyperPhases(int openStates, int blockedStates)`. Set the number of phases in the hyper-exponential distributions accounting for the open/shortage time.
+
+### Run calculations
+
+* `run()`. Evaluate the model using the input parameters.
+
+### Get results
+
+* `getDensity(int queueIdx=0, string type="preferred")`. Return the density distribution of a queue. The second argument specifies the arrival type: "all" and "preferred" (default).
+* `getFreq(int queueIdx=0, string type="preferred")`. Return the frequency distribution of a queue. The second argument specifies the arrival type: "all" and "preferred" (default).
+* `getShortageProb(int queueIdx=0, string type="preferred")`. Return the shortage probability of a queue. The second argument specifies the arrival type: "all" and "preferred" (default).
+* `getAvailProb(int queueIdx=0, string type="preferred")`. Return the probability that at least one server is available. The second argument specifies the arrival type: "all" and "preferred" (default).
+* `getExpOccupany(int queueIdx=0)`. Return the expected number of occupied servers.
+* `getExpOccFraction(int queueIdx=0)`. Return the expected fraction of occupied servers.
+
+### Return imported variables
+
+* `getArrivalRates()`. Return the imported arrival rates.
+* `getServiceTimes()`. Return the imported service times.
+* `getCapacity()`. Return the imported capacities.
+* `getReloc()`. Return the imported relocation probabilities.
+* `getPreferredQueue()`. Return the imported preferred queues.
+
+# Capsule on Code Ocean
+
+We have published a capsule for the Linux CLI on Code Ocean. The URL and DOI for the capsule follows below:
+
+* URL: https://codeocean.com/capsule/7104737/tree
+* DOI: https://doi.org/10.24433/CO.2728562.v1
+
+# How to cite
+
+[![DOI](https://zenodo.org/badge/293829002.svg)](https://zenodo.org/badge/latestdoi/293829002)
+
+# License
+
+Copyright 2024 Anders Reenberg Andersen.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
```


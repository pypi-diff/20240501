# Comparing `tmp/spotinst-agent-2-beta-3.1.12.tar.gz` & `tmp/spotinst-agent-2-beta-3.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotinst-agent-2-beta-3.1.12.tar", last modified: Thu Apr 27 08:02:47 2023, max compression
+gzip compressed data, was "spotinst-agent-2-beta-3.1.13.tar", last modified: Wed May  1 13:08:07 2024, max compression
```

## Comparing `spotinst-agent-2-beta-3.1.12.tar` & `spotinst-agent-2-beta-3.1.13.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 08:02:47.528722 spotinst-agent-2-beta-3.1.12/
--rw-r--r--   0 ayeletc    (502) staff       (20)     1065 2023-03-12 08:32:58.000000 spotinst-agent-2-beta-3.1.12/LICENSE
--rw-r--r--   0 ayeletc    (502) staff       (20)      181 2023-03-12 08:32:58.000000 spotinst-agent-2-beta-3.1.12/MANIFEST.in
--rw-r--r--   0 ayeletc    (502) staff       (20)     1982 2023-04-27 08:02:47.528530 spotinst-agent-2-beta-3.1.12/PKG-INFO
--rw-r--r--   0 ayeletc    (502) staff       (20)     1287 2023-03-12 08:32:58.000000 spotinst-agent-2-beta-3.1.12/README.rst
--rw-r--r--   0 ayeletc    (502) staff       (20)       38 2023-04-27 08:02:47.528780 spotinst-agent-2-beta-3.1.12/setup.cfg
--rw-r--r--   0 ayeletc    (502) staff       (20)     1442 2023-04-27 08:02:44.000000 spotinst-agent-2-beta-3.1.12/setup.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 08:02:47.526051 spotinst-agent-2-beta-3.1.12/spotinst_agent/
--rw-r--r--   0 ayeletc    (502) staff       (20)    12950 2023-04-27 07:09:58.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent/__init__.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     3383 2023-04-27 07:09:58.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent/agent.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     9645 2023-04-27 07:09:58.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent/agentinit.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     1157 2023-04-27 07:09:58.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent/basemodule.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 08:02:47.520011 spotinst-agent-2-beta-3.1.12/spotinst_agent/data/
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 08:02:47.526571 spotinst-agent-2-beta-3.1.12/spotinst_agent/data/configuration/
--rw-r--r--   0 ayeletc    (502) staff       (20)      180 2023-03-12 08:32:58.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent/data/configuration/basemodule.yml
--rw-r--r--   0 ayeletc    (502) staff       (20)      727 2023-03-12 08:32:58.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent/data/configuration/spotinst-agent.yml
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 08:02:47.526835 spotinst-agent-2-beta-3.1.12/spotinst_agent/data/installation/
--rwxr-xr-x   0 ayeletc    (502) staff       (20)     6701 2023-04-27 07:09:58.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent/data/installation/agent-init.sh
--rw-r--r--   0 ayeletc    (502) staff       (20)    21721 2023-04-27 07:09:58.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent/scheduler.py
--rw-r--r--   0 ayeletc    (502) staff       (20)    11165 2023-04-27 07:09:58.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent/taskmanager.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     9662 2023-04-27 07:09:58.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent/utils.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 08:02:47.528255 spotinst-agent-2-beta-3.1.12/spotinst_agent_2_beta.egg-info/
--rw-r--r--   0 ayeletc    (502) staff       (20)     1982 2023-04-27 08:02:47.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent_2_beta.egg-info/PKG-INFO
--rw-r--r--   0 ayeletc    (502) staff       (20)      650 2023-04-27 08:02:47.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent_2_beta.egg-info/SOURCES.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)        1 2023-04-27 08:02:47.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent_2_beta.egg-info/dependency_links.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       56 2023-04-27 08:02:47.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent_2_beta.egg-info/entry_points.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       23 2023-04-27 08:02:47.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent_2_beta.egg-info/requires.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       15 2023-04-27 08:02:47.000000 spotinst-agent-2-beta-3.1.12/spotinst_agent_2_beta.egg-info/top_level.txt
+drwxr-xr-x   0 mavni      (501) staff       (20)        0 2024-05-01 13:08:07.439762 spotinst-agent-2-beta-3.1.13/
+-rw-r--r--   0 mavni      (501) staff       (20)     1065 2024-05-01 09:00:13.000000 spotinst-agent-2-beta-3.1.13/LICENSE
+-rw-r--r--   0 mavni      (501) staff       (20)      181 2024-05-01 09:00:13.000000 spotinst-agent-2-beta-3.1.13/MANIFEST.in
+-rw-r--r--   0 mavni      (501) staff       (20)     2299 2024-05-01 13:08:07.439447 spotinst-agent-2-beta-3.1.13/PKG-INFO
+-rw-r--r--   0 mavni      (501) staff       (20)     1287 2024-05-01 09:00:13.000000 spotinst-agent-2-beta-3.1.13/README.rst
+-rw-r--r--   0 mavni      (501) staff       (20)       38 2024-05-01 13:08:07.439889 spotinst-agent-2-beta-3.1.13/setup.cfg
+-rwxr-xr-x   0 mavni      (501) staff       (20)     1442 2024-05-01 13:00:03.000000 spotinst-agent-2-beta-3.1.13/setup.py
+drwxr-xr-x   0 mavni      (501) staff       (20)        0 2024-05-01 13:08:07.431605 spotinst-agent-2-beta-3.1.13/spotinst_agent/
+-rw-r--r--   0 mavni      (501) staff       (20)    12950 2024-05-01 12:59:03.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent/__init__.py
+-rw-r--r--   0 mavni      (501) staff       (20)     3383 2024-05-01 12:59:03.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent/agent.py
+-rw-r--r--   0 mavni      (501) staff       (20)     9645 2024-05-01 12:59:03.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent/agentinit.py
+-rw-r--r--   0 mavni      (501) staff       (20)     1157 2024-05-01 12:59:03.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent/basemodule.py
+drwxr-xr-x   0 mavni      (501) staff       (20)        0 2024-05-01 13:08:07.422354 spotinst-agent-2-beta-3.1.13/spotinst_agent/data/
+drwxr-xr-x   0 mavni      (501) staff       (20)        0 2024-05-01 13:08:07.433709 spotinst-agent-2-beta-3.1.13/spotinst_agent/data/configuration/
+-rw-r--r--   0 mavni      (501) staff       (20)      180 2024-05-01 09:00:13.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent/data/configuration/basemodule.yml
+-rw-r--r--   0 mavni      (501) staff       (20)      727 2024-05-01 12:59:03.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent/data/configuration/spotinst-agent.yml
+drwxr-xr-x   0 mavni      (501) staff       (20)        0 2024-05-01 13:08:07.434388 spotinst-agent-2-beta-3.1.13/spotinst_agent/data/installation/
+-rwxr-xr-x   0 mavni      (501) staff       (20)     6979 2024-05-01 12:59:03.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent/data/installation/agent-init.sh
+-rw-r--r--   0 mavni      (501) staff       (20)    21721 2024-05-01 12:59:03.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent/scheduler.py
+-rw-r--r--   0 mavni      (501) staff       (20)    11111 2024-05-01 12:59:03.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent/taskmanager.py
+-rw-r--r--   0 mavni      (501) staff       (20)     9662 2024-05-01 12:59:03.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent/utils.py
+drwxr-xr-x   0 mavni      (501) staff       (20)        0 2024-05-01 13:08:07.438172 spotinst-agent-2-beta-3.1.13/spotinst_agent_2_beta.egg-info/
+-rw-r--r--   0 mavni      (501) staff       (20)     2299 2024-05-01 13:08:07.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent_2_beta.egg-info/PKG-INFO
+-rw-r--r--   0 mavni      (501) staff       (20)      650 2024-05-01 13:08:07.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent_2_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 mavni      (501) staff       (20)        1 2024-05-01 13:08:07.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent_2_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 mavni      (501) staff       (20)       56 2024-05-01 13:08:07.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent_2_beta.egg-info/entry_points.txt
+-rw-r--r--   0 mavni      (501) staff       (20)       23 2024-05-01 13:08:07.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent_2_beta.egg-info/requires.txt
+-rw-r--r--   0 mavni      (501) staff       (20)       15 2024-05-01 13:08:07.000000 spotinst-agent-2-beta-3.1.13/spotinst_agent_2_beta.egg-info/top_level.txt
```

### Comparing `spotinst-agent-2-beta-3.1.12/LICENSE` & `spotinst-agent-2-beta-3.1.13/LICENSE`

 * *Files identical despite different names*

### Comparing `spotinst-agent-2-beta-3.1.12/PKG-INFO` & `spotinst-agent-2-beta-3.1.13/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,58 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: spotinst-agent-2-beta
-Version: 3.1.12
+Version: 3.1.13
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
+Description: Agent
+        =======
+        
+        Spotinst Agent executor provides a mechanism to run remote shutdown scripts on machine using polling architecture.
+        
+        Note:
+        The agent must have token to communicate with spotinst API.
+        The credentials ini that holds the token file must be located at: '/root/.spotinst/credentials'
+        
+        Application
+        ===========
+        
+        Manual Executing
+        ~~~~~~~~~~~~~~~~
+        The simplest way to run the agent is by './agent' that start and write basic logs to /var/log/messages/agent.log
+        
+        Otherwise, you can use the following options:
+        
+        Usage:  ./agent [options]
+        
+        -c --config            Use alternate configuration yml file.
+        -l --log               Use alternate Log file for output.
+        -t --test              Test run.  Do not run remote script.
+        -v --verbose           verbose log
+        --stdout               redirect output to stdout
+        --debug                run with dummy credentials for debug purposes
+        
+        Configuration
+        ~~~~~~~~~~~~~
+        There are two levels of configuration representing in yml files.
+        The global configuration 'agent.yml' is responsible of the agent framework and necessary params.
+        The worker configuration, located at the workers folder is responsible of the specific workers parameters.
+        
+        
+        MAKEFILE
+        ~~~~~~~~~~~~~
+        run 'make release'
+        output file is located in the /dist folder
+        
+        Documentation
+        =============
+        
 Keywords: spotinst agent infrastructure monitoring execution deployment
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ==3.*
-License-File: LICENSE
-
-Agent
-=======
-
-Spotinst Agent executor provides a mechanism to run remote shutdown scripts on machine using polling architecture.
-
-Note:
-The agent must have token to communicate with spotinst API.
-The credentials ini that holds the token file must be located at: '/root/.spotinst/credentials'
-
-Application
-===========
-
-Manual Executing
-~~~~~~~~~~~~~~~~
-The simplest way to run the agent is by './agent' that start and write basic logs to /var/log/messages/agent.log
-
-Otherwise, you can use the following options:
-
-Usage:  ./agent [options]
-
--c --config            Use alternate configuration yml file.
--l --log               Use alternate Log file for output.
--t --test              Test run.  Do not run remote script.
--v --verbose           verbose log
---stdout               redirect output to stdout
---debug                run with dummy credentials for debug purposes
-
-Configuration
-~~~~~~~~~~~~~
-There are two levels of configuration representing in yml files.
-The global configuration 'agent.yml' is responsible of the agent framework and necessary params.
-The worker configuration, located at the workers folder is responsible of the specific workers parameters.
-
-
-MAKEFILE
-~~~~~~~~~~~~~
-run 'make release'
-output file is located in the /dist folder
-
-Documentation
-=============
-
-
```

### Comparing `spotinst-agent-2-beta-3.1.12/README.rst` & `spotinst-agent-2-beta-3.1.13/README.rst`

 * *Files identical despite different names*

### Comparing `spotinst-agent-2-beta-3.1.12/setup.py` & `spotinst-agent-2-beta-3.1.13/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='spotinst-agent-2-beta',
 
-    version="3.1.12",
+    version="3.1.13",
 
     description='Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.',
 
     long_description=description,
 
     # The project's main homepage.
     url='https://github.com/spotinst/spotinst-spectrum-agent',
```

### Comparing `spotinst-agent-2-beta-3.1.12/spotinst_agent/__init__.py` & `spotinst-agent-2-beta-3.1.13/spotinst_agent/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         else:
             print ("Please enter the name of the worker which you want to add.")
 
     elif action == "add-collector":
         if argument is not None:
             install_collector(argument, modules_path, s3_base_collectors_link)
         else:
-            print("Please enter the name of the collector which you want to add.")
+            print ("Please enter the name of the collector which you want to add.")
 
     elif action == "add-initiator":
         if argument is not None:
             install_initiator(argument, initiator_modules_path, s3_base_initiator_link)
         else:
             print("Please enter the name of the initiator which you want to add.")
 
@@ -246,26 +246,24 @@
 def install_collector(collector_name, modules_path, s3_base_collectors_link):
     print ("adding collector " + collector_name)
     try:
         handle_prerequisites(s3_base_collectors_link, collector_name)
         get_collector_files(collector_name, modules_path, s3_base_collectors_link)
 
     except Exception as e:
-        print("Could not get collector " + collector_name + " Exception : " + str(e))
-
+        print ("Could not get collector " + collector_name + " Exception : " + str(e))
 
 def install_initiator(initiator_name, initiator_modules_path, s3_base_initiator_link):
     print("adding initiator " + initiator_name)
     try:
         get_initiator_files(initiator_name, initiator_modules_path, s3_base_initiator_link)
 
     except Exception as e:
         print("Could not get initiator " + initiator_name + " Exception : " + str(e))
 
-
 def get_worker_files(modules_path, s3_base_workers_link, worker_name):
     py_response = urllib.request.urlopen(s3_base_workers_link + '/' + worker_name + '/' + worker_name + '.py')
     yml_response = urllib.request.urlopen(s3_base_workers_link + '/' + worker_name + '/' + worker_name + '.yml')
 
     with open(modules_path + '/' + worker_name + '.py', 'wb') as worker:
         worker.write(py_response.read())
     with open(modules_path + '/' + worker_name + '.yml', 'wb') as worker_cfg:
```

### Comparing `spotinst-agent-2-beta-3.1.12/spotinst_agent/agent.py` & `spotinst-agent-2-beta-3.1.13/spotinst_agent/agent.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-2-beta-3.1.12/spotinst_agent/agentinit.py` & `spotinst-agent-2-beta-3.1.13/spotinst_agent/agentinit.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-2-beta-3.1.12/spotinst_agent/basemodule.py` & `spotinst-agent-2-beta-3.1.13/spotinst_agent/basemodule.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-2-beta-3.1.12/spotinst_agent/data/configuration/spotinst-agent.yml` & `spotinst-agent-2-beta-3.1.13/spotinst_agent/data/configuration/spotinst-agent.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 enable: True
 # interval in seconds
 reload_interval: 120
 aws_instance_id_locator_url: 'http://169.254.169.254/latest/meta-data/instance-id'
 aws_metadata_service_token_url: 'http://169.254.169.254/latest/api/token'
 gcp_instance_metadata_url: 'http://metadata.google.internal/computeMetadata/v1'
 azure_instance_id_locator_url: 'http://169.254.169.254/metadata/instance/compute/vmId?api-version=2017-08-01&format=text'
-azure_spot_instance_id_locator_url: 'http://169.254.169.254/metadata/instance/compute/name?api-version=2017-08-01&format=text'
+azure_spot_instance_id_locator_url: 'http://169.254.169.254/metadata/instance/compute/vmId?api-version=2021-02-01&format=text'
 gcp_instance_name: '/instance/name'
 azure_node_id_path: '/etc/spotinst/nodeId.txt'
 azure_pool_id_path: '/etc/spotinst/poolId.txt'
 cloud_provider_path: '/etc/spotinst/cloud_provider.txt'
```

### Comparing `spotinst-agent-2-beta-3.1.12/spotinst_agent/data/installation/agent-init.sh` & `spotinst-agent-2-beta-3.1.13/spotinst_agent/data/installation/agent-init.sh`

 * *Files 4% similar despite different names*

```diff
@@ -262,14 +262,18 @@
   local readonly timestamp="$1"
   shift
   local readonly log_level="$1"
   shift
   local readonly message="$@"
   echo -e "${timestamp} [${log_level}] ${message}"
 }
+log_info "Installation of the Spot Agent is governed by NetApp’s end user license agreement (“EULA”), which can be found at:
+          https://www.netapp.com/how-to-buy/sales-terms-and-conditions/
+          By installing the Spot Agent, you accept and approve the EULA."
+
 log_info "Validating before install..."
 validate
 
 log_info "Installing..."
 install
 
 log_info "Cleaning up after install..."
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `spotinst-agent-2-beta-3.1.12/spotinst_agent/scheduler.py` & `spotinst-agent-2-beta-3.1.13/spotinst_agent/scheduler.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-2-beta-3.1.12/spotinst_agent/taskmanager.py` & `spotinst-agent-2-beta-3.1.13/spotinst_agent/taskmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
         self.scheduler = ThreadedScheduler()
         self.running = True
         self.tasks = {}
         self.instance_details = instance_details
 
     def start(self):
         initiators_folder = '/etc/spotinst/agent/initiators/modules'
-        self.log.debug("service is %s" % self.enable)
 
         # Search for initiators in folder
         initiators = self.load_modules(initiators_folder)
 
         # Setup Modules
         for initiator in initiators.values():
             c = self.init_module(initiator['cls'])
```

### Comparing `spotinst-agent-2-beta-3.1.12/spotinst_agent/utils.py` & `spotinst-agent-2-beta-3.1.13/spotinst_agent/utils.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-2-beta-3.1.12/spotinst_agent_2_beta.egg-info/PKG-INFO` & `spotinst-agent-2-beta-3.1.13/spotinst_agent_2_beta.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,58 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: spotinst-agent-2-beta
-Version: 3.1.12
+Version: 3.1.13
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
+Description: Agent
+        =======
+        
+        Spotinst Agent executor provides a mechanism to run remote shutdown scripts on machine using polling architecture.
+        
+        Note:
+        The agent must have token to communicate with spotinst API.
+        The credentials ini that holds the token file must be located at: '/root/.spotinst/credentials'
+        
+        Application
+        ===========
+        
+        Manual Executing
+        ~~~~~~~~~~~~~~~~
+        The simplest way to run the agent is by './agent' that start and write basic logs to /var/log/messages/agent.log
+        
+        Otherwise, you can use the following options:
+        
+        Usage:  ./agent [options]
+        
+        -c --config            Use alternate configuration yml file.
+        -l --log               Use alternate Log file for output.
+        -t --test              Test run.  Do not run remote script.
+        -v --verbose           verbose log
+        --stdout               redirect output to stdout
+        --debug                run with dummy credentials for debug purposes
+        
+        Configuration
+        ~~~~~~~~~~~~~
+        There are two levels of configuration representing in yml files.
+        The global configuration 'agent.yml' is responsible of the agent framework and necessary params.
+        The worker configuration, located at the workers folder is responsible of the specific workers parameters.
+        
+        
+        MAKEFILE
+        ~~~~~~~~~~~~~
+        run 'make release'
+        output file is located in the /dist folder
+        
+        Documentation
+        =============
+        
 Keywords: spotinst agent infrastructure monitoring execution deployment
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ==3.*
-License-File: LICENSE
-
-Agent
-=======
-
-Spotinst Agent executor provides a mechanism to run remote shutdown scripts on machine using polling architecture.
-
-Note:
-The agent must have token to communicate with spotinst API.
-The credentials ini that holds the token file must be located at: '/root/.spotinst/credentials'
-
-Application
-===========
-
-Manual Executing
-~~~~~~~~~~~~~~~~
-The simplest way to run the agent is by './agent' that start and write basic logs to /var/log/messages/agent.log
-
-Otherwise, you can use the following options:
-
-Usage:  ./agent [options]
-
--c --config            Use alternate configuration yml file.
--l --log               Use alternate Log file for output.
--t --test              Test run.  Do not run remote script.
--v --verbose           verbose log
---stdout               redirect output to stdout
---debug                run with dummy credentials for debug purposes
-
-Configuration
-~~~~~~~~~~~~~
-There are two levels of configuration representing in yml files.
-The global configuration 'agent.yml' is responsible of the agent framework and necessary params.
-The worker configuration, located at the workers folder is responsible of the specific workers parameters.
-
-
-MAKEFILE
-~~~~~~~~~~~~~
-run 'make release'
-output file is located in the /dist folder
-
-Documentation
-=============
-
-
```

### Comparing `spotinst-agent-2-beta-3.1.12/spotinst_agent_2_beta.egg-info/SOURCES.txt` & `spotinst-agent-2-beta-3.1.13/spotinst_agent_2_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/automvs-0.0.4.tar.gz` & `tmp/automvs-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automvs-0.0.4.tar", last modified: Wed May  1 05:50:09 2024, max compression
+gzip compressed data, was "automvs-0.0.5.tar", last modified: Wed May  1 15:55:21 2024, max compression
```

## Comparing `automvs-0.0.4.tar` & `automvs-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-01 05:50:09.675153 automvs-0.0.4/
--rw-rw-r--   0 phil      (1000) phil      (1000)     1069 2024-04-30 16:02:39.000000 automvs-0.0.4/LICENSE
--rw-r--r--   0 phil      (1000) phil      (1000)     1430 2024-05-01 05:50:09.675153 automvs-0.0.4/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      956 2024-04-30 16:02:39.000000 automvs-0.0.4/README.md
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-01 05:50:09.675153 automvs-0.0.4/automvs/
--rw-rw-r--   0 phil      (1000) phil      (1000)    19039 2024-05-01 05:48:13.000000 automvs-0.0.4/automvs/__init__.py
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-01 05:50:09.675153 automvs-0.0.4/automvs.egg-info/
--rw-r--r--   0 phil      (1000) phil      (1000)     1430 2024-05-01 05:50:09.000000 automvs-0.0.4/automvs.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      170 2024-05-01 05:50:09.000000 automvs-0.0.4/automvs.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-01 05:50:09.000000 automvs-0.0.4/automvs.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        8 2024-05-01 05:50:09.000000 automvs-0.0.4/automvs.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-01 05:50:09.675153 automvs-0.0.4/setup.cfg
--rw-rw-r--   0 phil      (1000) phil      (1000)      781 2024-05-01 05:48:06.000000 automvs-0.0.4/setup.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-01 15:55:21.707338 automvs-0.0.5/
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1069 2024-04-30 16:02:39.000000 automvs-0.0.5/LICENSE
+-rw-r--r--   0 phil      (1000) phil      (1000)     1430 2024-05-01 15:55:21.707338 automvs-0.0.5/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      956 2024-04-30 16:02:39.000000 automvs-0.0.5/README.md
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-01 15:55:21.707338 automvs-0.0.5/automvs/
+-rw-rw-r--   0 phil      (1000) phil      (1000)    19906 2024-05-01 15:55:15.000000 automvs-0.0.5/automvs/__init__.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-01 15:55:21.707338 automvs-0.0.5/automvs.egg-info/
+-rw-r--r--   0 phil      (1000) phil      (1000)     1430 2024-05-01 15:55:21.000000 automvs-0.0.5/automvs.egg-info/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      170 2024-05-01 15:55:21.000000 automvs-0.0.5/automvs.egg-info/SOURCES.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-01 15:55:21.000000 automvs-0.0.5/automvs.egg-info/dependency_links.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        8 2024-05-01 15:55:21.000000 automvs-0.0.5/automvs.egg-info/top_level.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-01 15:55:21.707338 automvs-0.0.5/setup.cfg
+-rw-rw-r--   0 phil      (1000) phil      (1000)      781 2024-05-01 15:55:17.000000 automvs-0.0.5/setup.py
```

### Comparing `automvs-0.0.4/LICENSE` & `automvs-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `automvs-0.0.4/PKG-INFO` & `automvs-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automvs
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python library for MVS/CE automation
 Home-page: https://github.com/MVS-sysgen/automvs
 Author: Philip Young
 Author-email: mainframed767@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `automvs-0.0.4/README.md` & `automvs-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `automvs-0.0.4/automvs/__init__.py` & `automvs-0.0.5/automvs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     This library allows the use of MVS/CE in an automated fashion. This can
     be used for deploying XMI files, pushing out updates, building software,
     creating custom MVS deployments.
 
     Using this library requires a recent version of hercules SDL and MVS/CE.
 """
 
-__version__ = '0.0.4'
+__version__ = '0.0.5'
 __author__ = 'Philip Young'
 __license__ = "GPL"
 
 # Copyright (c) 2021, Philip Young
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
@@ -231,69 +231,88 @@
                 hercproc.kill()
                 break
             continue
 
         self.logger.debug("[ERROR] - Hercules Exited Unexpectedly")
         os._exit(1)
 
-    def check_maxcc(self, jobname, steps_cc={}, printer_file='printers/prt00e.txt'):
+    def check_maxcc(self, jobname, steps_cc={}, printer_file='printers/prt00e.txt',ignore=False):
       '''Checks job and steps results, raises error
           If the step is in steps_cc, check the step vs the cc in the dictionary
           otherwise checks if step is zero
 
          jobname (str): name of the job to check from the printer file output
          steps_cc (dict): pairs of step names and expected CC. This should be used
             if you expect a specific step to have a return code other than zero.
          printer_file (str): location of the printer file from hercules that
             contains the job output.
+         ignore (bool): tells the function to ignore failed steps
+
+         returns: a list of dicts with 'jobname, procname, stepname, exitcode'
 
       '''
       self.logger.debug("[AUTOMATION] Checking {} job results".format(jobname))
 
       found_job = False
       failed_step = False
+      job_status = []
 
       logmsg = '[MAXCC] Jobname: {:<8} Procname: {:<8} Stepname: {:<8} Exit Code: {:<8}'
 
       with open(printer_file, 'r', errors='ignore') as f:
           for line in f.readlines():
               if 'IEF142I' in line and jobname in line:
 
                   found_job = True
 
                   x = line.strip().split()
                   y = x.index('IEF142I')
                   j = x[y:]
 
                   log = logmsg.format(j[1],'',j[2],j[10])
+                  step_status = {
+                                    "jobname:" : j[1],
+                                    "procname": '',
+                                    "stepname": j[2],
+                                    "exitcode": j[10]
+                                }
                   maxcc=j[10]
                   stepname = j[2]
 
                   if j[3] != "-":
                       log = logmsg.format(j[1],j[2],j[3],j[11])
+                    step_status = {
+                                        "jobname:" : j[1],
+                                        "procname": j[2],
+                                        "stepname": j[3],
+                                        "exitcode": j[11]
+                                    }
                       stepname = j[3]
                       maxcc=j[11]
 
                   self.logger.debug(log)
+                  job_status.append(step_status)
 
                   if stepname in steps_cc:
                       expected_cc = steps_cc[stepname]
                   else:
                       expected_cc = '0000'
 
                   if maxcc != expected_cc:
                       error = "Step {} Condition Code does not match expected condition code: {} vs {} review prt00e.txt for errors".format(stepname,j[-1],expected_cc)
                       self.logger.error(error)
                       failed_step = True
 
       if not found_job:
           raise ValueError("Job {} not found in printer output {}".format(jobname, printer_file))
 
-      if failed_step:
+      if failed_step and not ignore:
           raise ValueError(error)
+        
+    return(job_status)
 
 
     def reset_hercules(self,clpa=False):
         self.logger.debug('[AUTOMATION] Restarting hercules')
         self.quit_hercules(msg=False)
 
         # drain STDERR and STDOUT
```

### Comparing `automvs-0.0.4/automvs.egg-info/PKG-INFO` & `automvs-0.0.5/automvs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automvs
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python library for MVS/CE automation
 Home-page: https://github.com/MVS-sysgen/automvs
 Author: Philip Young
 Author-email: mainframed767@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `automvs-0.0.4/setup.py` & `automvs-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def read_file(filename):
     with open(os.path.join(os.path.dirname(__file__), filename)) as file:
         return file.read()
 
 setup(
     name='automvs',
-    version='0.0.4',    
+    version='0.0.5',    
     description='Python library for MVS/CE automation',
     url='https://github.com/MVS-sysgen/automvs',
     author='Philip Young',
     author_email='mainframed767@gmail.com',
     license='MIT',
     packages=['automvs'],
     install_requires=[],
```


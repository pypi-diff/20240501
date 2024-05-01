# Comparing `tmp/mbox2m365-3.2.6.tar.gz` & `tmp/mbox2m365-3.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbox2m365-3.2.6.tar", last modified: Fri Sep 22 19:13:32 2023, max compression
+gzip compressed data, was "mbox2m365-3.2.8.tar", last modified: Sun Oct 22 22:41:02 2023, max compression
```

## Comparing `mbox2m365-3.2.6.tar` & `mbox2m365-3.2.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 rudolph   (1000) rudolph   (1000)        0 2023-09-22 19:13:32.155316 mbox2m365-3.2.6/
--rw-r--r--   0 rudolph   (1000) rudolph   (1000)     1551 2023-08-02 00:41:28.000000 mbox2m365-3.2.6/LICENSE
--rw-r--r--   0 rudolph   (1000) rudolph   (1000)       26 2023-08-02 00:41:28.000000 mbox2m365-3.2.6/MANIFEST.in
--rw-rw-r--   0 rudolph   (1000) rudolph   (1000)    11458 2023-09-22 19:13:32.155316 mbox2m365-3.2.6/PKG-INFO
--rw-r--r--   0 rudolph   (1000) rudolph   (1000)    11135 2023-08-02 00:41:28.000000 mbox2m365-3.2.6/README.md
--rw-r--r--   0 rudolph   (1000) rudolph   (1000)    11135 2023-08-02 00:41:28.000000 mbox2m365-3.2.6/README.rst
-drwxrwxr-x   0 rudolph   (1000) rudolph   (1000)        0 2023-09-22 19:13:32.153317 mbox2m365-3.2.6/jobber/
--rw-r--r--   0 rudolph   (1000) rudolph   (1000)     5167 2023-08-02 00:41:28.000000 mbox2m365-3.2.6/jobber/jobber.py
-drwxrwxr-x   0 rudolph   (1000) rudolph   (1000)        0 2023-09-22 19:13:32.155316 mbox2m365-3.2.6/mbox2m365/
--rwxr-xr-x   0 rudolph   (1000) rudolph   (1000)      268 2023-08-02 00:41:28.000000 mbox2m365-3.2.6/mbox2m365/__init__.py
--rw-r--r--   0 rudolph   (1000) rudolph   (1000)    11547 2023-08-02 00:41:28.000000 mbox2m365-3.2.6/mbox2m365/__main__.py
--rwxrwxr-x   0 rudolph   (1000) rudolph   (1000)     2068 2023-08-04 23:40:05.000000 mbox2m365-3.2.6/mbox2m365/mailSink.py
--rw-rw-r--   0 rudolph   (1000) rudolph   (1000)    32449 2023-09-22 19:11:09.000000 mbox2m365-3.2.6/mbox2m365/mbox2m365.py
-drwxrwxr-x   0 rudolph   (1000) rudolph   (1000)        0 2023-09-22 19:13:32.155316 mbox2m365-3.2.6/mbox2m365.egg-info/
--rw-r--r--   0 rudolph   (1000) rudolph   (1000)    11458 2023-09-22 19:13:32.000000 mbox2m365-3.2.6/mbox2m365.egg-info/PKG-INFO
--rw-rw-r--   0 rudolph   (1000) rudolph   (1000)      380 2023-09-22 19:13:32.000000 mbox2m365-3.2.6/mbox2m365.egg-info/SOURCES.txt
--rw-rw-r--   0 rudolph   (1000) rudolph   (1000)        1 2023-09-22 19:13:32.000000 mbox2m365-3.2.6/mbox2m365.egg-info/dependency_links.txt
--rw-rw-r--   0 rudolph   (1000) rudolph   (1000)       54 2023-09-22 19:13:32.000000 mbox2m365-3.2.6/mbox2m365.egg-info/entry_points.txt
--rw-rw-r--   0 rudolph   (1000) rudolph   (1000)       20 2023-09-22 19:13:32.000000 mbox2m365-3.2.6/mbox2m365.egg-info/requires.txt
--rw-rw-r--   0 rudolph   (1000) rudolph   (1000)       17 2023-09-22 19:13:32.000000 mbox2m365-3.2.6/mbox2m365.egg-info/top_level.txt
--rw-rw-r--   0 rudolph   (1000) rudolph   (1000)      260 2023-09-22 19:09:42.000000 mbox2m365-3.2.6/pyproject.toml
--rw-r--r--   0 rudolph   (1000) rudolph   (1000)      449 2023-09-22 19:13:32.157317 mbox2m365-3.2.6/setup.cfg
--rw-r--r--   0 rudolph   (1000) rudolph   (1000)      441 2023-08-02 00:41:28.000000 mbox2m365-3.2.6/setup.py
+drwxr-xr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-10-22 22:41:02.575011 mbox2m365-3.2.8/
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     1551 2023-08-14 00:56:03.000000 mbox2m365-3.2.8/LICENSE
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)       26 2023-08-14 00:56:03.000000 mbox2m365-3.2.8/MANIFEST.in
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)    11458 2023-10-22 22:41:02.575236 mbox2m365-3.2.8/PKG-INFO
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)    11135 2023-08-14 00:56:03.000000 mbox2m365-3.2.8/README.md
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)    11135 2023-08-14 00:56:03.000000 mbox2m365-3.2.8/README.rst
+drwxr-xr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-10-22 22:41:02.570520 mbox2m365-3.2.8/jobber/
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)     5186 2023-10-22 12:57:18.000000 mbox2m365-3.2.8/jobber/jobber.py
+drwxr-xr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-10-22 22:41:02.572119 mbox2m365-3.2.8/mbox2m365/
+-rwxr-xr-x   0 rudolph  (2090878) fnndsc    (1102)      268 2023-08-14 00:56:03.000000 mbox2m365-3.2.8/mbox2m365/__init__.py
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)    11547 2023-08-14 00:56:03.000000 mbox2m365-3.2.8/mbox2m365/__main__.py
+-rwxr-xr-x   0 rudolph  (2090878) fnndsc    (1102)     2068 2023-08-14 00:56:03.000000 mbox2m365-3.2.8/mbox2m365/mailSink.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    32824 2023-10-22 22:38:15.000000 mbox2m365-3.2.8/mbox2m365/mbox2m365.py
+drwxr-xr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-10-22 22:41:02.574684 mbox2m365-3.2.8/mbox2m365.egg-info/
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)    11458 2023-10-22 22:41:02.000000 mbox2m365-3.2.8/mbox2m365.egg-info/PKG-INFO
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      380 2023-10-22 22:41:02.000000 mbox2m365-3.2.8/mbox2m365.egg-info/SOURCES.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2023-10-22 22:41:02.000000 mbox2m365-3.2.8/mbox2m365.egg-info/dependency_links.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       54 2023-10-22 22:41:02.000000 mbox2m365-3.2.8/mbox2m365.egg-info/entry_points.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       20 2023-10-22 22:41:02.000000 mbox2m365-3.2.8/mbox2m365.egg-info/requires.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       17 2023-10-22 22:41:02.000000 mbox2m365-3.2.8/mbox2m365.egg-info/top_level.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      260 2023-10-22 22:38:36.000000 mbox2m365-3.2.8/pyproject.toml
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)      449 2023-10-22 22:41:02.576038 mbox2m365-3.2.8/setup.cfg
+-rw-r--r--   0 rudolph  (2090878) fnndsc    (1102)      441 2023-08-14 00:56:03.000000 mbox2m365-3.2.8/setup.py
```

### Comparing `mbox2m365-3.2.6/LICENSE` & `mbox2m365-3.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mbox2m365-3.2.6/PKG-INFO` & `mbox2m365-3.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbox2m365
-Version: 3.2.6
+Version: 3.2.8
 Summary: 'Send a message stored within an mbox using m365 (Office365)'
 Home-page: https://github.com/FNNDSC/mbox2m365
 Author: Rudolph Pienaar
 Author-email: rudolph.pienaar@childrens.harvard.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mbox2m365-3.2.6/README.md` & `mbox2m365-3.2.8/README.md`

 * *Files identical despite different names*

### Comparing `mbox2m365-3.2.6/README.rst` & `mbox2m365-3.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `mbox2m365-3.2.6/jobber/jobber.py` & `mbox2m365-3.2.8/jobber/jobber.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 
 
 import  subprocess
 import  os
 import  pudb
 import  json
+import  shlex
 
 class jobber:
 
     def __init__(self, d_args : dict):
         """Constructor for the jobber class.
 
         Args:
@@ -100,15 +101,15 @@
             'cwd':          "",
             'returncode':   0
         }
         str_stdoutLine  : str   = ""
         str_stdout      : str   = ""
 
         p = subprocess.Popen(
-                    str_cmd.split(),
+                    shlex.split(str_cmd),
                     stdout      = subprocess.PIPE,
                     stderr      = subprocess.PIPE,
         )
 
         # Realtime output on stdout
         while True:
             stdout      = p.stdout.readline()
```

### Comparing `mbox2m365-3.2.6/mbox2m365/__main__.py` & `mbox2m365-3.2.8/mbox2m365/__main__.py`

 * *Files identical despite different names*

### Comparing `mbox2m365-3.2.6/mbox2m365/mailSink.py` & `mbox2m365-3.2.8/mbox2m365/mailSink.py`

 * *Files identical despite different names*

### Comparing `mbox2m365-3.2.6/mbox2m365/mbox2m365.py` & `mbox2m365-3.2.8/mbox2m365/mbox2m365.py`

 * *Files 2% similar despite different names*

```diff
@@ -694,28 +694,37 @@
 
         def txscript_save(str_content) -> None:
             self.transmissionCmd = self.configPath / Path(baseFileName + "_tx.cmd")
             with open(self.transmissionCmd, "w") as f:
                 f.write(f'%s' % str_content)
             self.transmissionCmd.chmod(0o755)
 
+        def execstr_build(input:Path) -> str:
+            ret:str             = ""
+            t_parts:tuple       = input.parts
+            ret                 = '/'.join(['"{0}"'.format(arg) if ' ' in arg else arg for arg in t_parts])
+            return ret
+
         b_status        : bool  = False
         d_m365          : dict  = {}
         ld_m365         : list  = []
         baseFileName    : str   = ""
 
         if d_consolidated['status']:
             shell       = jobber.jobber({'verbosity': 1, 'noJobLogging': True})
             # First send all the messages...
             for m365message in d_consolidated['ld_transmit']:
                 b_status        = True
                 baseFileName    = self.urlify(m365message['subject'])
                 bodyToFile_check(m365message)
                 txscript_save(txscript_content(m365message))
-                d_m365  = shell.job_run(str(self.transmissionCmd))
+                test    = execstr_build(self.transmissionCmd)
+                d_m365  = shell.job_run(
+                        execstr_build(self.transmissionCmd)
+                )
                 self.log(
                     "Transmitted message (%s), return code '%s', recipients '%s'" %\
                          (m365message['bodyHash'],
                           d_m365['returncode'],
                           m365message['to'])
                 )
                 b_status    = True
```

### Comparing `mbox2m365-3.2.6/mbox2m365.egg-info/PKG-INFO` & `mbox2m365-3.2.8/mbox2m365.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbox2m365
-Version: 3.2.6
+Version: 3.2.8
 Summary: 'Send a message stored within an mbox using m365 (Office365)'
 Home-page: https://github.com/FNNDSC/mbox2m365
 Author: Rudolph Pienaar
 Author-email: rudolph.pienaar@childrens.harvard.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```


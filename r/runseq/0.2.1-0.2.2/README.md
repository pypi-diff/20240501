# Comparing `tmp/runseq-0.2.1.tar.gz` & `tmp/runseq-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runseq-0.2.1.tar", last modified: Wed May  1 13:44:17 2024, max compression
+gzip compressed data, was "runseq-0.2.2.tar", last modified: Wed May  1 14:21:50 2024, max compression
```

## Comparing `runseq-0.2.1.tar` & `runseq-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 lgomes    (1000) lgomes    (1000)        0 2024-05-01 13:44:17.460854 runseq-0.2.1/
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)    35149 2024-04-23 13:58:13.000000 runseq-0.2.1/LICENSE
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)    43180 2024-05-01 13:44:17.460854 runseq-0.2.1/PKG-INFO
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)     2309 2024-05-01 13:43:31.000000 runseq-0.2.1/README.md
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)      469 2024-05-01 13:44:03.000000 runseq-0.2.1/pyproject.toml
-drwxr-xr-x   0 lgomes    (1000) lgomes    (1000)        0 2024-05-01 13:44:17.460854 runseq-0.2.1/runseq.egg-info/
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)    43180 2024-05-01 13:44:17.000000 runseq-0.2.1/runseq.egg-info/PKG-INFO
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)      216 2024-05-01 13:44:17.000000 runseq-0.2.1/runseq.egg-info/SOURCES.txt
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)        1 2024-05-01 13:44:17.000000 runseq-0.2.1/runseq.egg-info/dependency_links.txt
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)       39 2024-05-01 13:44:17.000000 runseq-0.2.1/runseq.egg-info/entry_points.txt
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)        7 2024-05-01 13:44:17.000000 runseq-0.2.1/runseq.egg-info/top_level.txt
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)     5782 2024-04-30 15:52:35.000000 runseq-0.2.1/runseq.py
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)       38 2024-05-01 13:44:17.460854 runseq-0.2.1/setup.cfg
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)       38 2024-04-23 15:30:44.000000 runseq-0.2.1/setup.py
+drwxr-xr-x   0 lgomes    (1000) lgomes    (1000)        0 2024-05-01 14:21:50.729229 runseq-0.2.2/
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)    35149 2024-04-23 13:58:13.000000 runseq-0.2.2/LICENSE
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)    43180 2024-05-01 14:21:50.729229 runseq-0.2.2/PKG-INFO
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)     2309 2024-05-01 13:43:31.000000 runseq-0.2.2/README.md
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)      469 2024-05-01 14:21:19.000000 runseq-0.2.2/pyproject.toml
+drwxr-xr-x   0 lgomes    (1000) lgomes    (1000)        0 2024-05-01 14:21:50.729229 runseq-0.2.2/runseq.egg-info/
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)    43180 2024-05-01 14:21:50.000000 runseq-0.2.2/runseq.egg-info/PKG-INFO
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)      216 2024-05-01 14:21:50.000000 runseq-0.2.2/runseq.egg-info/SOURCES.txt
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)        1 2024-05-01 14:21:50.000000 runseq-0.2.2/runseq.egg-info/dependency_links.txt
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)       39 2024-05-01 14:21:50.000000 runseq-0.2.2/runseq.egg-info/entry_points.txt
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)        7 2024-05-01 14:21:50.000000 runseq-0.2.2/runseq.egg-info/top_level.txt
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)     5932 2024-05-01 14:20:51.000000 runseq-0.2.2/runseq.py
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)       38 2024-05-01 14:21:50.729229 runseq-0.2.2/setup.cfg
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)       38 2024-04-23 15:30:44.000000 runseq-0.2.2/setup.py
```

### Comparing `runseq-0.2.1/LICENSE` & `runseq-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `runseq-0.2.1/PKG-INFO` & `runseq-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runseq
-Version: 0.2.1
+Version: 0.2.2
 Summary: Simple job manager to run jobs sequentially in a Linux machine.
 Author-email: Luís Gomes <luismsgomes@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `runseq-0.2.1/README.md` & `runseq-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `runseq-0.2.1/runseq.egg-info/PKG-INFO` & `runseq-0.2.2/runseq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runseq
-Version: 0.2.1
+Version: 0.2.2
 Summary: Simple job manager to run jobs sequentially in a Linux machine.
 Author-email: Luís Gomes <luismsgomes@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `runseq-0.2.1/runseq.py` & `runseq-0.2.2/runseq.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 
 def run_jobs():
     sql = (
         "SELECT job_id "
         "FROM jobs "
         "WHERE status = 'queued' "
-        "ORDER BY -priority LIMIT 1"
+        "ORDER BY -priority, submitted LIMIT 1"
     )
     with db_connect() as con:
         while True:
             for (job_id,) in con.execute(sql):
                 run_job(job_id)
                 break  # rerun SQL to fetch next job
             else:
@@ -126,15 +126,19 @@
         "started",
         "finished",
         "returncode",
         "command",
     ]
     sql = (
         "SELECT " + ", ".join(columns) + " FROM jobs "
-        "ORDER BY status, -priority, submitted"
+        "ORDER BY CASE "
+        "WHEN status = 'finished' THEN 0 "
+        "WHEN status = 'running' THEN 1 "
+        "WHEN status = 'queued' THEN 2 "
+        "END, -priority, submitted"
     )
     with db_connect() as con:
         for line in con.execute(sql):
             line = ["n/a" if value is None else value for value in line]
             print(
                 *["%s: %s" % key_value for key_value in zip(columns, line)], sep=" | "
             )
```


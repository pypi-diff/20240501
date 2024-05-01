# Comparing `tmp/mytot-2024.4.546183-py3-none-any.whl.zip` & `tmp/mytot-2024.5.963441-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 27712 bytes, number of entries: 9
+Zip file size: 27764 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx        0 b- defN 24-Apr-18 09:16 mytot/__init__.py
--rw-rw-r--  2.0 unx     3951 b- defN 24-Apr-25 12:57 mytot/main.py
--rwxrwxr-x  2.0 unx    35149 b- defN 24-Apr-18 09:16 mytot-2024.4.546183.data/data/LICENSE
--rwxrwxr-x  2.0 unx    35149 b- defN 24-Apr-29 04:58 mytot-2024.4.546183.dist-info/LICENSE
--rw-rw-r--  2.0 unx      774 b- defN 24-Apr-29 04:58 mytot-2024.4.546183.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-29 04:58 mytot-2024.4.546183.dist-info/WHEEL
--rw-rw-r--  2.0 unx       85 b- defN 24-Apr-29 04:58 mytot-2024.4.546183.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        6 b- defN 24-Apr-29 04:58 mytot-2024.4.546183.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      752 b- defN 24-Apr-29 04:58 mytot-2024.4.546183.dist-info/RECORD
-9 files, 75958 bytes uncompressed, 26402 bytes compressed:  65.2%
+-rw-rw-r--  2.0 unx     4094 b- defN 24-May-01 03:30 mytot/main.py
+-rwxrwxr-x  2.0 unx    35149 b- defN 24-Apr-18 09:16 mytot-2024.5.963441.data/data/LICENSE
+-rwxrwxr-x  2.0 unx    35149 b- defN 24-May-01 03:30 mytot-2024.5.963441.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      774 b- defN 24-May-01 03:30 mytot-2024.5.963441.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-01 03:30 mytot-2024.5.963441.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       85 b- defN 24-May-01 03:30 mytot-2024.5.963441.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        6 b- defN 24-May-01 03:30 mytot-2024.5.963441.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      752 b- defN 24-May-01 03:30 mytot-2024.5.963441.dist-info/RECORD
+9 files, 76101 bytes uncompressed, 26454 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: mytot/__init__.py
 Comment: 
 
 Filename: mytot/main.py
 Comment: 
 
-Filename: mytot-2024.4.546183.data/data/LICENSE
+Filename: mytot-2024.5.963441.data/data/LICENSE
 Comment: 
 
-Filename: mytot-2024.4.546183.dist-info/LICENSE
+Filename: mytot-2024.5.963441.dist-info/LICENSE
 Comment: 
 
-Filename: mytot-2024.4.546183.dist-info/METADATA
+Filename: mytot-2024.5.963441.dist-info/METADATA
 Comment: 
 
-Filename: mytot-2024.4.546183.dist-info/WHEEL
+Filename: mytot-2024.5.963441.dist-info/WHEEL
 Comment: 
 
-Filename: mytot-2024.4.546183.dist-info/entry_points.txt
+Filename: mytot-2024.5.963441.dist-info/entry_points.txt
 Comment: 
 
-Filename: mytot-2024.4.546183.dist-info/top_level.txt
+Filename: mytot-2024.5.963441.dist-info/top_level.txt
 Comment: 
 
-Filename: mytot-2024.4.546183.dist-info/RECORD
+Filename: mytot-2024.5.963441.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mytot/main.py

```diff
@@ -26,14 +26,17 @@
                 for child in children:
                     pid_list.append(child.pid)
             cmdline = " ".join(parent.cmdline())
             print(f"kill {parent.pid} {cmdline}")
             parent.send_signal(sig)
 
 
+PID = os.getpid()
+
+
 def mkdir(path):
     if not os.path.exists(path):
         os.makedirs(path)
 
 
 def RUN():
     if len(sys.argv) < 2:
@@ -102,19 +105,21 @@
     # check the pragma
     date = today()
     mkdir(os.path.expanduser("~/.cache/task_log/"))
     task_log = os.path.expanduser(f"~/.cache/task_log/out.{date}")
     for process in psutil.process_iter(["pid", "name", "cmdline"]):
         if process.info["cmdline"] is None:
             continue
+        if process.info["pid"] == PID:
+            continue
         cmdline = " ".join(list(process.info["cmdline"]))
-        if script_file in cmdline:
+        if script_file in cmdline and "vim " not in cmdline and "nvim " not in cmdline:
             with open(task_log, "a") as f:
                 now = datetime.datetime.now()
-                f.write(f"{now} | {script_file} is running\n")
+                f.write(f"{now} | {script_file} is running {cmdline}\n")
             return
     path, name = os.path.split(script_file)
     log_path = os.path.join(path, "log")
     mkdir(log_path)
     if script_file.endswith(".py"):
         cmd = ["python", "-Wignore", script_file]
     elif script_file.endswith(".sh"):
```

## Comparing `mytot-2024.4.546183.data/data/LICENSE` & `mytot-2024.5.963441.data/data/LICENSE`

 * *Files identical despite different names*

## Comparing `mytot-2024.4.546183.dist-info/LICENSE` & `mytot-2024.5.963441.dist-info/LICENSE`

 * *Files identical despite different names*


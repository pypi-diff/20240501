# Comparing `tmp/makefile_checker-0.0.0-py2.py3-none-any.whl.zip` & `tmp/makefile_checker-0.0.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 2792 bytes, number of entries: 6
--rw-r--r--  2.0 unx     2917 b- defN 80-Jan-01 00:00 makefile_checker/checker.py
+Zip file size: 3162 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     1029 b- defN 80-Jan-01 00:00 makefile_checker/check.py
+-rw-r--r--  2.0 unx     2374 b- defN 80-Jan-01 00:00 makefile_checker/checker.py
 -rw-r--r--  2.0 unx      325 b- defN 80-Jan-01 00:00 makefile_checker/exceptions.py
--rw-r--r--  2.0 unx      674 b- defN 80-Jan-01 00:00 makefile_checker-0.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 makefile_checker-0.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       65 b- defN 80-Jan-01 00:00 makefile_checker-0.0.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      506 b- defN 16-Jan-01 00:00 makefile_checker-0.0.0.dist-info/RECORD
-6 files, 4579 bytes uncompressed, 1866 bytes compressed:  59.2%
+-rw-r--r--  2.0 unx      674 b- defN 80-Jan-01 00:00 makefile_checker-0.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 80-Jan-01 00:00 makefile_checker-0.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       63 b- defN 80-Jan-01 00:00 makefile_checker-0.0.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      588 b- defN 16-Jan-01 00:00 makefile_checker-0.0.1.dist-info/RECORD
+7 files, 5145 bytes uncompressed, 2110 bytes compressed:  59.0%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
+Filename: makefile_checker/check.py
+Comment: 
+
 Filename: makefile_checker/checker.py
 Comment: 
 
 Filename: makefile_checker/exceptions.py
 Comment: 
 
-Filename: makefile_checker-0.0.0.dist-info/METADATA
+Filename: makefile_checker-0.0.1.dist-info/METADATA
 Comment: 
 
-Filename: makefile_checker-0.0.0.dist-info/WHEEL
+Filename: makefile_checker-0.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: makefile_checker-0.0.0.dist-info/entry_points.txt
+Filename: makefile_checker-0.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: makefile_checker-0.0.0.dist-info/RECORD
+Filename: makefile_checker-0.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## makefile_checker/checker.py

```diff
@@ -1,100 +1,76 @@
-import os, fnmatch
 from pathlib import Path
 from typing import List
 
-from makefile_checker.makefile_checker.exceptions import MissingFilesException
 
+class Checker:
 
-def read_file_contents(path: str) -> str:
-    """
-    Given a path, read the contents of the file at that path.
-    """
-    makefile_contents = None
-    with open(path) as file:
-        makefile_contents = file.read()
-
-    assert makefile_contents is not None, f"Empty file at {path}"
-    return makefile_contents
-
-
-def clean_and_parse_makefile_scripts(makefile_contents: str) -> List[str]:
-    """    
-    Clean the raw contents of a Makefile.
-    Parse out the paths to scripts that are to be run.
-    For example, remove comments and any line that is not a path to a script.
-
-    e.g. If the Makefile contains:
-
-    ```
-    # This is a comment
-    target:
-        python this/is/a/script.py
-        # This is another comment python this/is/a/script5.py
-        python3 this/is/a/script2.py
-    ```
-
-    Then the cleaned contents should be:
-    [
-        "this/is/a/script.py",
-        "this/is/a/script2.py"
-    ]
-
-    TODO(rohantilva): just use a regex to parse out the paths to scripts.
-    """
-
-    # remove lines that do not start with "python"
-    python_lines = [line.strip() for line in makefile_contents.split("\n") if line.strip().startswith("python")]
-
-    scripts = []
-    for line in python_lines:
-        end_index = line.find(".py")
-        line = line[:end_index + 3]
-        start_index = line.rindex(" ")
-        line = line[start_index + 1:]
-        scripts.append(line)
-
-    return scripts
-
-
-def get_makefiles_in_current_working_directory(pattern: str = "Makefile") -> List[str]:
-    """
-    Get all Makefiles that might exist in current working directory.
-    There may be multiple Makefiles in different directories / projects.
-    Grab them all, and validate them one by one.
-    """
-    path = os.getcwd()
-
-    result = []
-    for root, _, files in os.walk(path):
-        for name in files:
-            if fnmatch.fnmatch(name, pattern):
-                result.append(os.path.join(root, name))
-    return result
-
-
-def get_missing_scripts_for_makefile(path_to_makefile: str) -> List[str]:
-    makefile_contents = read_file_contents(path_to_makefile)
-    all_scripts = clean_and_parse_makefile_scripts(makefile_contents)
-
-    # get base path that the scripts live under
-    parts = path_to_makefile.strip("/").split("/")
-    base_path = "/".join(parts[:len(parts) - 1])
-
-    alerts = []
-    for script in all_scripts:
-        file_path = f"/{base_path}/{script.strip()}"
-        if not Path(file_path).is_file():
-            alerts.append(file_path)
-
-    return alerts
-
-
-def check():
-    makefiles = get_makefiles_in_current_working_directory()
-
-    all_alerts = []
-    for makefile in makefiles:
-        all_alerts.extend(get_missing_scripts_for_makefile(makefile))
+    def __init__(self, path_to_makefile: str):
+        self.path_to_makefile = path_to_makefile
 
-    if len(all_alerts) > 0:
-        raise MissingFilesException(all_alerts)
+
+    def read_file_contents(self) -> str:
+        """
+        Given a path, read the contents of the file at that path.
+        """
+        makefile_contents = None
+        with open(self.path_to_makefile) as file:
+            makefile_contents = file.read()
+
+        assert makefile_contents is not None, f"Empty file at {self.path_to_makefile}"
+        return makefile_contents
+
+
+    def clean_and_parse_makefile_scripts(self, makefile_contents: str) -> List[str]:
+        """    
+        Clean the raw contents of a Makefile.
+        Parse out the paths to scripts that are to be run.
+        For example, remove comments and any line that is not a path to a script.
+
+        e.g. If the Makefile contains:
+
+        ```
+        # This is a comment
+        target:
+            python this/is/a/script.py
+            # This is another comment python this/is/a/script5.py
+            python3 this/is/a/script2.py
+        ```
+
+        Then the cleaned contents should be:
+        [
+            "this/is/a/script.py",
+            "this/is/a/script2.py"
+        ]
+
+        TODO(rohantilva): just use a regex to parse out the paths to scripts.
+        """
+
+        # remove lines that do not start with "python"
+        python_lines = [line.strip() for line in makefile_contents.split("\n") if line.strip().startswith("python")]
+
+        scripts = []
+        for line in python_lines:
+            end_index = line.find(".py")
+            line = line[:end_index + 3]
+            start_index = line.rindex(" ")
+            line = line[start_index + 1:]
+            scripts.append(line)
+
+        return scripts
+
+
+    def get_missing_scripts_for_makefile(self) -> List[str]:
+        makefile_contents = self.read_file_contents(self.path_to_makefile)
+        all_scripts = self.clean_and_parse_makefile_scripts(makefile_contents)
+
+        # get base path that the scripts live under
+        parts = self.path_to_makefile.strip("/").split("/")
+        base_path = "/".join(parts[:len(parts) - 1])
+
+        alerts = []
+        for script in all_scripts:
+            file_path = f"/{base_path}/{script.strip()}"
+            if not Path(file_path).is_file():
+                alerts.append(file_path)
+
+        return alerts
```

## Comparing `makefile_checker-0.0.0.dist-info/METADATA` & `makefile_checker-0.0.1.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makefile-checker
-Version: 0.0.0
+Version: 0.0.1
 Summary: Package to validate makefile contents
 Author: rohantilva
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```


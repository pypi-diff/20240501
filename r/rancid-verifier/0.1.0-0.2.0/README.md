# Comparing `tmp/rancid_verifier-0.1.0.tar.gz` & `tmp/rancid_verifier-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rancid_verifier-0.1.0.tar", max compression
+gzip compressed data, was "rancid_verifier-0.2.0.tar", max compression
```

## Comparing `rancid_verifier-0.1.0.tar` & `rancid_verifier-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1070 2023-04-29 10:17:35.126663 rancid_verifier-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2023-04-29 09:53:53.109997 rancid_verifier-0.1.0/README.md
--rw-r--r--   0        0        0      467 2023-05-07 13:09:39.156666 rancid_verifier-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-29 09:53:53.073330 rancid_verifier-0.1.0/rancid_verifier/__init__.py
--rw-r--r--   0        0        0     1900 2023-05-07 13:09:39.160000 rancid_verifier-0.1.0/rancid_verifier/main.py
--rw-r--r--   0        0        0      346 1970-01-01 00:00:00.000000 rancid_verifier-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-29 10:17:35.126663 rancid_verifier-0.2.0/LICENSE
+-rw-r--r--   0        0        0      663 2024-05-01 19:48:03.907473 rancid_verifier-0.2.0/README.md
+-rw-r--r--   0        0        0      694 2024-05-01 19:48:03.910473 rancid_verifier-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-29 09:53:53.073330 rancid_verifier-0.2.0/rancid_verifier/__init__.py
+-rw-r--r--   0        0        0     1340 2024-05-01 19:48:03.914472 rancid_verifier-0.2.0/rancid_verifier/main.py
+-rw-r--r--   0        0        0     1379 2024-05-01 19:48:03.918472 rancid_verifier-0.2.0/rancid_verifier/verification.py
+-rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 rancid_verifier-0.2.0/PKG-INFO
```

### Comparing `rancid_verifier-0.1.0/LICENSE` & `rancid_verifier-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rancid_verifier-0.1.0/rancid_verifier/main.py` & `rancid_verifier-0.2.0/rancid_verifier/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,57 @@
 import argparse
 import pathlib
 import sys
-from dataclasses import dataclass, field
-from typing import Any
 
-
-@dataclass
-class VerificationResult:
-    file_path: pathlib.Path
-    errors: dict[str, bool] = field(default_factory=dict)
-
-
-def get_file_list(path_raw: str, file_name: str = "router.db") -> list[pathlib.Path]:
-    """Get files from provided path."""
-
-    path = pathlib.Path(path_raw)
-
-    if path.is_file():
-        return [path]
-
-    return list(path.glob(file_name))
-
-
-def verify_file(file_path: str | pathlib.Path) -> Any:
-    file_path = pathlib.Path(file_path)
-    result = VerificationResult(file_path=pathlib.Path(file_path))
-
-    if not file_path.exists():
-        result.errors["not_found"] = True
-        return result
-
-    try:
-        open(file_path, "r", encoding="utf-8").read()
-    except UnicodeDecodeError:
-        result.errors["not_utf8"] = True
-
-    return result
+from rancid_verifier.verification import VerificationResult, verify_file
 
 
 def print_results(results: list[VerificationResult]) -> None:
     for result in results:
-        if len(result.errors) == 0:
+        if not result.error:
             status: str = "OK"
         else:
             status: str = "Error"
         print(f"{str(result.file_path)} {status}")
 
 
 def parse_args() -> argparse.Namespace:
     parser: argparse.ArgumentParser = argparse.ArgumentParser()
 
-    parser.add_argument("path", help="Folder to look for router.db in")
+    parser.add_argument("path", help="Path to router.db")
     parser.add_argument(
-        "-q", "--quite", action="store_true", help="Dont print anything"
+        "-q",
+        "--quite",
+        action="store_true",
+        help=(
+            "Dont print anything, "
+            "exit with non-zero exit code if file contains errors."
+        ),
     )
 
     return parser.parse_args()
 
 
 def cli() -> None:
     args: argparse.Namespace = parse_args()
 
     results: list[VerificationResult] = []
 
+    router_db_path = pathlib.Path(args.path)
+    if not router_db_path.exists():
+        if not args.quite:
+            print(f"File {router_db_path} doesn't exist.")
+        sys.exit(2)
+
     exit_code: int = 0
 
-    for file_path in get_file_list(args.path):
-        result: VerificationResult = verify_file(file_path)
-        if len(result.errors) > 0:
-            exit_code = 1
-        results.append(result)
+    result: VerificationResult = verify_file(router_db_path)
+    if result.error:
+        exit_code = 1
+    results.append(result)
 
     if args.quite:
         sys.exit(exit_code)
 
     print_results(results)
 
     sys.exit(exit_code)
```


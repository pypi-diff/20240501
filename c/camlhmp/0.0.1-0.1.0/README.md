# Comparing `tmp/camlhmp-0.0.1.tar.gz` & `tmp/camlhmp-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camlhmp-0.0.1.tar", max compression
+gzip compressed data, was "camlhmp-0.1.0.tar", max compression
```

## Comparing `camlhmp-0.0.1.tar` & `camlhmp-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0     1076 2024-04-25 04:33:35.881917 camlhmp-0.0.1/LICENSE
--rw-r--r--   0        0        0     7938 2024-04-25 04:33:35.881917 camlhmp-0.0.1/README.md
--rw-r--r--   0        0        0      111 2024-04-25 04:33:35.881917 camlhmp-0.0.1/camlhmp/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 04:33:35.881917 camlhmp-0.0.1/camlhmp/cli/__init__.py
--rw-r--r--   0        0        0     4818 2024-04-25 04:33:35.881917 camlhmp-0.0.1/camlhmp/cli/camlhmp.py
--rw-r--r--   0        0        0        0 2024-04-25 04:33:35.885917 camlhmp-0.0.1/camlhmp/engines/__init__.py
--rw-r--r--   0        0        0     1957 2024-04-25 04:33:35.885917 camlhmp-0.0.1/camlhmp/engines/blast.py
--rw-r--r--   0        0        0     2625 2024-04-25 04:33:35.885917 camlhmp-0.0.1/camlhmp/framework.py
--rw-r--r--   0        0        0     2655 2024-04-25 04:33:35.885917 camlhmp-0.0.1/camlhmp/utils.py
--rw-r--r--   0        0        0        0 2024-04-25 04:33:35.885917 camlhmp-0.0.1/camlhmp/visuals/__init__.py
--rw-r--r--   0        0        0     2782 2024-04-25 04:33:35.885917 camlhmp-0.0.1/camlhmp/visuals/framework.py
--rw-r--r--   0        0        0      764 2024-04-25 04:33:35.885917 camlhmp-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     8721 1970-01-01 00:00:00.000000 camlhmp-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-01 00:00:53.676576 camlhmp-0.1.0/LICENSE
+-rw-r--r--   0        0        0    16938 2024-05-01 00:00:53.676576 camlhmp-0.1.0/README.md
+-rw-r--r--   0        0        0      111 2024-05-01 00:00:53.676576 camlhmp-0.1.0/camlhmp/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 00:00:53.676576 camlhmp-0.1.0/camlhmp/cli/__init__.py
+-rw-r--r--   0        0        0     9044 2024-05-01 00:00:53.676576 camlhmp-0.1.0/camlhmp/cli/blast.py
+-rw-r--r--   0        0        0     1567 2024-05-01 00:00:53.676576 camlhmp-0.1.0/camlhmp/cli/camlhmp.py
+-rw-r--r--   0        0        0     4482 2024-05-01 00:00:53.676576 camlhmp-0.1.0/camlhmp/cli/extract.py
+-rw-r--r--   0        0        0        0 2024-05-01 00:00:53.676576 camlhmp-0.1.0/camlhmp/engines/__init__.py
+-rw-r--r--   0        0        0     2038 2024-05-01 00:00:53.676576 camlhmp-0.1.0/camlhmp/engines/blast.py
+-rw-r--r--   0        0        0     3941 2024-05-01 00:00:53.676576 camlhmp-0.1.0/camlhmp/framework.py
+-rw-r--r--   0        0        0     4672 2024-05-01 00:00:53.676576 camlhmp-0.1.0/camlhmp/utils.py
+-rw-r--r--   0        0        0        0 2024-05-01 00:00:53.676576 camlhmp-0.1.0/camlhmp/visuals/__init__.py
+-rw-r--r--   0        0        0     2782 2024-05-01 00:00:53.676576 camlhmp-0.1.0/camlhmp/visuals/framework.py
+-rw-r--r--   0        0        0      870 2024-05-01 00:00:53.676576 camlhmp-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    17760 1970-01-01 00:00:00.000000 camlhmp-0.1.0/PKG-INFO
```

### Comparing `camlhmp-0.0.1/LICENSE` & `camlhmp-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `camlhmp-0.0.1/camlhmp/engines/blast.py` & `camlhmp-0.1.0/camlhmp/engines/blast.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Functions for running and parsing BLAST results
+import csv
 import logging
 
 from camlhmp.utils import execute
 
 BLASTN_COLS = [
     "qseqid",
     "sseqid",
@@ -19,14 +20,38 @@
     "sstart",
     "send",
     "evalue",
     "bitscore",
 ]
 
 
+def get_blast_target_hits(targets: list, results: dict) -> dict:
+    """
+    Find the target hits in the BLAST results.
+
+    Args:
+        targets (list): The list of target sequences
+        results (dict): The BLAST results
+
+    Returns:
+        dict: The target hits
+    """
+    target_hits = {}
+    for target in targets:
+        target_hits[target] = False
+        if target in results:
+            target_hits[target] = True
+
+    # Debugging information
+    logging.debug("camlhmp.engines.blast.get_blast_target_hits")
+    logging.debug(f"Profile Hits: {target_hits}")
+
+    return target_hits
+
+
 def run_blastn(subject: str, query: str, min_pident: float, min_coverage: int) -> dict:
     """
     Query sequences against a input subject using BLASTN.
 
     Args:
         subject (str): The subject database
         query (str): The query file
@@ -39,40 +64,18 @@
     outfmt = " ".join(BLASTN_COLS)
     cat_type = "zcat" if str(subject).endswith(".gz") else "cat"
     stdout, stderr = execute(
         f"{cat_type} {subject} | blastn -query {query} -subject - -outfmt '6 {outfmt}' -qcov_hsp_perc {min_coverage} -perc_identity {min_pident}",
         capture=True,
     )
 
-    # Convert BLAST results to a dictionary
-    results = {}
+    # Convert BLAST results to a list of dicts
+    results = []
+    target_hits = []
     for line in stdout.split("\n"):
         if line == "":
             continue
         cols = line.split("\t")
-        results[cols[0]] = dict(zip(BLASTN_COLS, cols))
+        results.append(dict(zip(BLASTN_COLS, cols)))
+        target_hits.append(cols[0])
 
-    return [results, stderr]
-
-
-def get_blast_target_hits(targets: list, results: dict) -> dict:
-    """
-    Find the target hits in the BLAST results.
-
-    Args:
-        targets (list): The list of target sequences
-        results (dict): The BLAST results
-
-    Returns:
-        dict: The target hits
-    """
-    target_hits = {}
-    for target in targets:
-        target_hits[target] = False
-        if target in results:
-            target_hits[target] = True
-
-    # Debugging information
-    logging.debug("camlhmp.engines.blast.get_blast_target_hits")
-    logging.debug(f"Profile Hits: {target_hits}")
-
-    return target_hits
+    return [target_hits, results, stderr]
```

### Comparing `camlhmp-0.0.1/camlhmp/visuals/framework.py` & `camlhmp-0.1.0/camlhmp/visuals/framework.py`

 * *Files identical despite different names*

### Comparing `camlhmp-0.0.1/pyproject.toml` & `camlhmp-0.1.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 [tool.poetry]
 name = "camlhmp"
-version = "0.0.1"
+version = "0.1.0"
 description = "Classification through yAML Heuristic Mapping Protocol"
 authors = [
     "Robert A. Petit III <robbie.petit@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rpetit3/camlhmp"
 repository = "https://github.com/rpetit3/camlhmp"
 keywords = ["bioinformatics", "bacteria", "serotype", "genotype"]
 
 [tool.poetry.scripts]
 camlhmp = "camlhmp.cli.camlhmp:main"
+camlhmp-blast = "camlhmp.cli.blast:main"
+camlhmp-extract = "camlhmp.cli.extract:main"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pyyaml = "^6.0.1"
 executor = "^23.2"
 rich = "^13.7.1"
 rich-click = "^1.7.4"
+biopython = "^1.83"
 
 [tool.poetry.group.dev.dependencies]
 executor = "^23.2"
 flake8 = "^7.0.0"
 isort = "^5.13.2"
 black = "^24.4.0"
```


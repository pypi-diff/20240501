# Comparing `tmp/bam-filter-1.4.8.tar.gz` & `tmp/bam-filter-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bam-filter-1.4.8.tar", last modified: Tue Apr 30 16:56:52 2024, max compression
+gzip compressed data, was "bam-filter-1.4.9.tar", last modified: Wed May  1 19:56:28 2024, max compression
```

## Comparing `bam-filter-1.4.8.tar` & `bam-filter-1.4.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:56:52.053972 bam-filter-1.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-30 16:56:49.000000 bam-filter-1.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 16:56:49.000000 bam-filter-1.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-30 16:56:52.053972 bam-filter-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21540 2024-04-30 16:56:49.000000 bam-filter-1.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:56:52.053972 bam-filter-1.4.8/bam_filter/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-30 16:56:49.000000 bam-filter-1.4.8/bam_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-30 16:56:49.000000 bam-filter-1.4.8/bam_filter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-30 16:56:52.053972 bam-filter-1.4.8/bam_filter/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-04-30 16:56:49.000000 bam-filter-1.4.8/bam_filter/entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-04-30 16:56:49.000000 bam-filter-1.4.8/bam_filter/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    23868 2024-04-30 16:56:49.000000 bam-filter-1.4.8/bam_filter/lca.py
--rw-r--r--   0 runner    (1001) docker     (127)    40569 2024-04-30 16:56:49.000000 bam-filter-1.4.8/bam_filter/reassign.py
--rw-r--r--   0 runner    (1001) docker     (127)    50509 2024-04-30 16:56:49.000000 bam-filter-1.4.8/bam_filter/sam_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    44025 2024-04-30 16:56:49.000000 bam-filter-1.4.8/bam_filter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 16:56:52.053972 bam-filter-1.4.8/bam_filter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-30 16:56:52.000000 bam-filter-1.4.8/bam_filter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-30 16:56:52.000000 bam-filter-1.4.8/bam_filter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 16:56:52.000000 bam-filter-1.4.8/bam_filter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-30 16:56:52.000000 bam-filter-1.4.8/bam_filter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-30 16:56:52.000000 bam-filter-1.4.8/bam_filter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-30 16:56:52.000000 bam-filter-1.4.8/bam_filter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-30 16:56:52.053972 bam-filter-1.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-30 16:56:49.000000 bam-filter-1.4.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    70238 2024-04-30 16:56:49.000000 bam-filter-1.4.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:56:28.264374 bam-filter-1.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-01 19:56:24.000000 bam-filter-1.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-01 19:56:24.000000 bam-filter-1.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-01 19:56:28.264374 bam-filter-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21540 2024-05-01 19:56:24.000000 bam-filter-1.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:56:28.264374 bam-filter-1.4.9/bam_filter/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-01 19:56:24.000000 bam-filter-1.4.9/bam_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-01 19:56:24.000000 bam-filter-1.4.9/bam_filter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-01 19:56:28.264374 bam-filter-1.4.9/bam_filter/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6414 2024-05-01 19:56:24.000000 bam-filter-1.4.9/bam_filter/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-05-01 19:56:24.000000 bam-filter-1.4.9/bam_filter/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23868 2024-05-01 19:56:24.000000 bam-filter-1.4.9/bam_filter/lca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40656 2024-05-01 19:56:24.000000 bam-filter-1.4.9/bam_filter/reassign.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50190 2024-05-01 19:56:24.000000 bam-filter-1.4.9/bam_filter/sam_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44025 2024-05-01 19:56:24.000000 bam-filter-1.4.9/bam_filter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 19:56:28.264374 bam-filter-1.4.9/bam_filter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-01 19:56:28.000000 bam-filter-1.4.9/bam_filter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-01 19:56:28.000000 bam-filter-1.4.9/bam_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 19:56:28.000000 bam-filter-1.4.9/bam_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-01 19:56:28.000000 bam-filter-1.4.9/bam_filter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-01 19:56:28.000000 bam-filter-1.4.9/bam_filter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-01 19:56:28.000000 bam-filter-1.4.9/bam_filter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-01 19:56:28.264374 bam-filter-1.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-01 19:56:24.000000 bam-filter-1.4.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70238 2024-05-01 19:56:24.000000 bam-filter-1.4.9/versioneer.py
```

### Comparing `bam-filter-1.4.8/LICENSE` & `bam-filter-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bam-filter-1.4.8/README.md` & `bam-filter-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `bam-filter-1.4.8/bam_filter/__main__.py` & `bam-filter-1.4.9/bam_filter/__main__.py`

 * *Files identical despite different names*

### Comparing `bam-filter-1.4.8/bam_filter/entropy.py` & `bam-filter-1.4.9/bam_filter/entropy.py`

 * *Files identical despite different names*

### Comparing `bam-filter-1.4.8/bam_filter/filter.py` & `bam-filter-1.4.9/bam_filter/filter.py`

 * *Files identical despite different names*

### Comparing `bam-filter-1.4.8/bam_filter/lca.py` & `bam-filter-1.4.9/bam_filter/lca.py`

 * *Files identical despite different names*

### Comparing `bam-filter-1.4.8/bam_filter/reassign.py` & `bam-filter-1.4.9/bam_filter/reassign.py`

 * *Files 2% similar despite different names*

```diff
@@ -290,15 +290,17 @@
     refs_idx = {sys.intern(str(x)): i for i, x in enumerate(ref_names)}
     if threads > 4:
         write_threads = 4
     else:
         write_threads = threads
 
     new_header = header.to_dict()
-    new_header["SQ"] = [x for x in new_header["SQ"] if x["SN"] in ref_names]
+    new_header["SQ"] = [x for x in new_header["SQ"] if x["SN"] in list(ref_names)]
+    new_header["SQ"].sort(key=lambda x: list(ref_names).index(x["SN"]))
+    new_header["HD"]["SO"] = "unsorted"
 
     out_bam_file = pysam.AlignmentFile(
         out_files["bam_reassigned_tmp"],
         "wb",
         referencenames=list(ref_names),
         referencelengths=list(ref_lengths),
         threads=write_threads,
@@ -411,27 +413,27 @@
         for chrom in samfile.references:
             chr_lengths.append(samfile.get_reference_length(chrom))
         max_chr_length = np.max(chr_lengths)
         pysam.set_verbosity(save)
         samfile.close()
 
         if max_chr_length > 536870912:
-            logging.info("A reference is longer than 2^29, indexing with csi")
-            pysam.index(
-                "-c",
-                "-@",
-                str(threads),
-                out_bam,
-            )
-        else:
-            pysam.index(
-                "-@",
-                str(threads),
-                out_bam,
-            )
+            logging.info("A reference is longer than 2^29")
+        pysam.index(
+            "-c",
+            "-@",
+            str(threads),
+            out_bam,
+        )
+        # else:
+        #     pysam.index(
+        #         "-@",
+        #         str(threads),
+        #         out_bam,
+        #     )
 
         os.remove(out_files["bam_reassigned_tmp"])
     else:
         logging.info("Skipping BAM file sorting...")
         shutil.move(out_files["bam_reassigned_tmp"], out_bam)
```

### Comparing `bam-filter-1.4.8/bam_filter/sam_utils.py` & `bam-filter-1.4.9/bam_filter/sam_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,28 +84,33 @@
 
     if threads > 4:
         write_threads = 4
     else:
         write_threads = threads
 
     new_header = header.to_dict()
-    new_header["SQ"] = [x for x in new_header["SQ"] if x["SN"] in ref_names]
+    new_header["SQ"] = [x for x in new_header["SQ"] if x["SN"] in list(ref_names)]
+    new_header["SQ"].sort(key=lambda x: list(ref_names).index(x["SN"]))
+    # change it to unsorted
+    new_header["HD"]["SO"] = "unsorted"
 
     out_bam_file = pysam.AlignmentFile(
         output_files["bam_tmp"],
         "wb",
         referencenames=list(ref_names),
         referencelengths=ref_lengths,
         threads=write_threads,
         header=new_header,
     )
     # out_bam_file.set_tag(read_groups)
     # out_bam_file.set(pg)
     references = [x for x in samfile.references if x in refs_idx.keys()]
 
+    # sort new_header["SQ"] using the references order
+
     logging.info(f"::: ::: Filtering {len(references):,} references sequentially...")
     for reference in tqdm.tqdm(
         references,
         total=len(references),
         leave=False,
         ncols=80,
         desc="References processed",
@@ -149,27 +154,21 @@
     for chrom in samfile.references:
         chr_lengths.append(samfile.get_reference_length(chrom))
     max_chr_length = np.max(chr_lengths)
     pysam.set_verbosity(save)
     samfile.close()
 
     if max_chr_length > 536870912:
-        logging.info("::: ::: A reference is longer than 2^29, indexing with csi")
-        pysam.index(
-            "-c",
-            "-@",
-            str(s_threads),
-            output_files["bam_tmp_sorted"],
-        )
-    else:
-        pysam.index(
-            "-@",
-            str(s_threads),
-            output_files["bam_tmp_sorted"],
-        )
+        logging.info("::: ::: A reference is longer than 2^29")
+    pysam.index(
+        "-c",
+        "-@",
+        str(s_threads),
+        output_files["bam_tmp_sorted"],
+    )
 
     os.remove(output_files["bam_tmp"])
     return output_files["bam_tmp_sorted"]
 
 
 def get_tad(cov, trim_min=10, trim_max=90):
     """
@@ -825,22 +824,17 @@
                 else:
                     s_threads = threads
                 samfile = pysam.AlignmentFile(bam, "rb", threads=s_threads)
 
             if not samfile.has_index():
                 logging.info("BAM index not found. Indexing...")
                 if max_chr_length > 536870912:
-                    logging.info("A reference is longer than 2^29, indexing with csi")
-                    pysam.index("-c", "-@", str(threads), bam)
-                else:
-                    pysam.index(
-                        "-@",
-                        str(threads),
-                        bam,
-                    )
+                    logging.info("A reference is longer than 2^29")
+                pysam.index("-c", "-@", str(threads), bam)
+
             logging.info("::: BAM file looks good.")
 
         return bam  # No need to reload the samfile after creating index, thanks to the with statement
     except ValueError as ve:
         if "file has no sequences defined (mode='rb')" in str(ve):
             return None
         else:
@@ -1183,15 +1177,21 @@
             samfile.close()
             refs_idx = {sys.intern(str(x)): i for i, x in enumerate(ref_names)}
             if threads > 4:
                 write_threads = 4
             else:
                 write_threads = threads
             new_header = header.to_dict()
-            new_header["SQ"] = [x for x in new_header["SQ"] if x["SN"] in ref_names]
+            new_header["SQ"] = [
+                x for x in new_header["SQ"] if x["SN"] in list(ref_names)
+            ]
+
+            new_header["SQ"].sort(key=lambda x: list(ref_names).index(x["SN"]))
+            new_header["HD"]["SO"] = "unsorted"
+
             out_bam_file = pysam.AlignmentFile(
                 out_files["bam_filtered_tmp"],
                 "wb",
                 referencenames=list(ref_names),
                 referencelengths=list(ref_lengths),
                 threads=write_threads,
                 header=new_header,
@@ -1322,29 +1322,21 @@
                     for chrom in samfile.references:
                         chr_lengths.append(samfile.get_reference_length(chrom))
                     max_chr_length = np.max(chr_lengths)
                     pysam.set_verbosity(save)
                     samfile.close()
 
                     if max_chr_length > 536870912:
-                        logging.info(
-                            "A reference is longer than 2^29, indexing with csi"
-                        )
-                        pysam.index(
-                            "-c",
-                            "-@",
-                            str(threads),
-                            out_files["bam_filtered"],
-                        )
-                    else:
-                        pysam.index(
-                            "-@",
-                            str(threads),
-                            out_files["bam_filtered"],
-                        )
+                        logging.info("A reference is longer than 2^29")
+                    pysam.index(
+                        "-c",
+                        "-@",
+                        str(threads),
+                        out_files["bam_filtered"],
+                    )
 
                 os.remove(out_files["bam_filtered_tmp"])
             else:
                 logging.info("Skipping BAM file sorting...")
                 shutil.move(out_files["bam_filtered_tmp"], out_files["bam_filtered"])
         else:
             logging.info("Skipping filtering BAM file creation...")
```

### Comparing `bam-filter-1.4.8/bam_filter/utils.py` & `bam-filter-1.4.9/bam_filter/utils.py`

 * *Files identical despite different names*

### Comparing `bam-filter-1.4.8/setup.cfg` & `bam-filter-1.4.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `bam-filter-1.4.8/setup.py` & `bam-filter-1.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `bam-filter-1.4.8/versioneer.py` & `bam-filter-1.4.9/versioneer.py`

 * *Files identical despite different names*


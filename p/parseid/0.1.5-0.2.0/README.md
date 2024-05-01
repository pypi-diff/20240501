# Comparing `tmp/parseid-0.1.5.tar.gz` & `tmp/parseid-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parseid-0.1.5.tar", last modified: Mon Apr  1 14:32:10 2024, max compression
+gzip compressed data, was "parseid-0.2.0.tar", last modified: Wed May  1 15:06:22 2024, max compression
```

## Comparing `parseid-0.1.5.tar` & `parseid-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:10.206391 parseid-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-01 14:32:10.206391 parseid-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-01 14:32:06.000000 parseid-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 14:32:10.206391 parseid-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-01 14:32:06.000000 parseid-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:10.202391 parseid-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:10.202391 parseid-0.1.5/src/parseid/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-01 14:32:06.000000 parseid-0.1.5/src/parseid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-01 14:32:06.000000 parseid-0.1.5/src/parseid/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-01 14:32:06.000000 parseid-0.1.5/src/parseid/ditrie.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-01 14:32:06.000000 parseid-0.1.5/src/parseid/process_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-01 14:32:06.000000 parseid-0.1.5/src/parseid/read_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-04-01 14:32:06.000000 parseid-0.1.5/src/parseid/trie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-01 14:32:06.000000 parseid-0.1.5/src/parseid/trie_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:10.206391 parseid-0.1.5/src/parseid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-01 14:32:10.000000 parseid-0.1.5/src/parseid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-01 14:32:10.000000 parseid-0.1.5/src/parseid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:32:10.000000 parseid-0.1.5/src/parseid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-01 14:32:10.000000 parseid-0.1.5/src/parseid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-01 14:32:10.000000 parseid-0.1.5/src/parseid.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:32:10.206391 parseid-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-01 14:32:06.000000 parseid-0.1.5/tests/test_ditrie.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-01 14:32:06.000000 parseid-0.1.5/tests/test_env.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-01 14:32:06.000000 parseid-0.1.5/tests/test_process_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-01 14:32:06.000000 parseid-0.1.5/tests/test_trie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-01 14:32:06.000000 parseid-0.1.5/tests/test_trie_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:06:22.446424 parseid-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-01 15:06:22.446424 parseid-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-01 15:06:12.000000 parseid-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 15:06:22.446424 parseid-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-01 15:06:12.000000 parseid-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:06:22.442424 parseid-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:06:22.442424 parseid-0.2.0/src/parseid/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-01 15:06:12.000000 parseid-0.2.0/src/parseid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-01 15:06:12.000000 parseid-0.2.0/src/parseid/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-01 15:06:12.000000 parseid-0.2.0/src/parseid/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-01 15:06:12.000000 parseid-0.2.0/src/parseid/ditrie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-01 15:06:12.000000 parseid-0.2.0/src/parseid/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-01 15:06:12.000000 parseid-0.2.0/src/parseid/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-01 15:06:12.000000 parseid-0.2.0/src/parseid/read_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-05-01 15:06:12.000000 parseid-0.2.0/src/parseid/trie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-05-01 15:06:12.000000 parseid-0.2.0/src/parseid/trie_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:06:22.446424 parseid-0.2.0/src/parseid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-01 15:06:22.000000 parseid-0.2.0/src/parseid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-01 15:06:22.000000 parseid-0.2.0/src/parseid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 15:06:22.000000 parseid-0.2.0/src/parseid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 15:06:22.000000 parseid-0.2.0/src/parseid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 15:06:22.000000 parseid-0.2.0/src/parseid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:06:22.446424 parseid-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-01 15:06:12.000000 parseid-0.2.0/tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-01 15:06:12.000000 parseid-0.2.0/tests/test_ditrie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-01 15:06:12.000000 parseid-0.2.0/tests/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-01 15:06:12.000000 parseid-0.2.0/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-01 15:06:12.000000 parseid-0.2.0/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-01 15:06:12.000000 parseid-0.2.0/tests/test_trie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-01 15:06:12.000000 parseid-0.2.0/tests/test_trie_node.py
```

### Comparing `parseid-0.1.5/PKG-INFO` & `parseid-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: parseid
-Version: 0.1.5
+Version: 0.2.0
 Summary: suck, parse identifiers or accession numbers
 Home-page: https://github.com/Tiezhengyuan/parse_identifier
 Author: Tiezheng Yuan
 Author-email: tiezhengyuan@hotmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+Requires-Dist: bioomics
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: requests
 Requires-Dist: obonet
 Requires-Dist: python-dotenv
 
 \n# parseID: suck, parse identifiers or accession numbers
@@ -43,15 +44,15 @@
 There is one example about how huge accession numbers are sucked into Trie.
 The mapping file could be downloaded from https://ftp.ncbi.nlm.nih.gov/gene/DATA/gene_refseq_uniprotkb_collab.gz into local space.
 Retrieve 176,513,729 (03/25/2024) UniProt Accession numbers from the file and feed them into Trie.
 Showed as the example below, accession numbers are stored in the object uniprotkb_acc_trie. 
 ```
 from parseid import ProcessID
 infile = 'gene_refseq_uniprotkb_collab'
-uniprotkb_acc_trie = ProcessID(infile).uniprotkb_accession()
+uniprotkb_acc_trie = ProcessID(infile).uniprotkb_protein_accession()
 ```
 
 Retrieve pairs of NCBI protein accession number and UniProt Accession numbers
 from file and feed them into Ditrie. Showed as the example below, 
 the mapping fo two accession numbers are stored in the object map_trie, 
 which is ready for query or parsing.
 ```
```

### Comparing `parseid-0.1.5/README.md` & `parseid-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 There is one example about how huge accession numbers are sucked into Trie.
 The mapping file could be downloaded from https://ftp.ncbi.nlm.nih.gov/gene/DATA/gene_refseq_uniprotkb_collab.gz into local space.
 Retrieve 176,513,729 (03/25/2024) UniProt Accession numbers from the file and feed them into Trie.
 Showed as the example below, accession numbers are stored in the object uniprotkb_acc_trie. 
 ```
 from parseid import ProcessID
 infile = 'gene_refseq_uniprotkb_collab'
-uniprotkb_acc_trie = ProcessID(infile).uniprotkb_accession()
+uniprotkb_acc_trie = ProcessID(infile).uniprotkb_protein_accession()
 ```
 
 Retrieve pairs of NCBI protein accession number and UniProt Accession numbers
 from file and feed them into Ditrie. Showed as the example below, 
 the mapping fo two accession numbers are stored in the object map_trie, 
 which is ready for query or parsing.
 ```
```

### Comparing `parseid-0.1.5/setup.py` & `parseid-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,24 +5,31 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="parseid",
-    version='0.1.5',
+    version='0.2.0',
     author="Tiezheng Yuan",
     author_email="tiezhengyuan@hotmail.com",
     description="suck, parse identifiers or accession numbers",
     url = "https://github.com/Tiezhengyuan/parse_identifier",
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=['parseid'],
     package_dir={'': 'src'},
-    install_requires=['numpy', 'pandas', 'requests', 'obonet', 'python-dotenv'],
+    install_requires=[
+        'bioomics',
+        'numpy',
+        'pandas',
+        'requests',
+        'obonet',
+        'python-dotenv'
+    ],
     keywords=['pypi', 'cicd', 'python'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

### Comparing `parseid-0.1.5/src/parseid/ditrie.py` & `parseid-0.2.0/src/parseid/ditrie.py`

 * *Files identical despite different names*

### Comparing `parseid-0.1.5/src/parseid/process_id.py` & `parseid-0.2.0/src/parseid/build.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,47 @@
-"""
-data structure: The di-trie. Here are the features:
-Define A trie and B trie:
-one leave node of A trie is mapped to one or more leave nodes of B trie
-"""
+'''
+Build trie of IDs
+'''
+
+import os
+
 from .read_file import ReadFile
 from .trie import Trie
-from .ditrie import DiTrie
 
-class ProcessID:
-    def __init__(self, infile:str):
-        self.infile = infile
-    
-    def uniprotkb_protein_accession(self) -> Trie:
+class Build:
+    def __init__(self, local_path:str=None):
+        self.local_path = local_path
+        self.save = True if local_path and os.path.isdir(local_path) else False
+        self.meta = {'records': 0, 'trie': None}
+
+
+    def ncbi_refseq_pacc(self, infile:str) -> dict:
         """
         source file: gene_refseq_uniprotkb_collab downloaded from NCBI/Entrez
-        suck UniProtKB protein accession numbers
+        suck NCBI protein accepython setup.pyssion numbers
         """
         acc_trie = Trie()
-        n = 0
-        self.records = ReadFile(self.infile).gene_refseq_uniprotkb_collab()
-        for items in self.records:
-                acc = items[1]
-                acc_trie.insert(acc)
-                n += 1
-        print(f"Total number of {n} UniProtKB protein accession numbers are fed into Trie.")
-        return acc_trie
-
-    def ncbi_protein_accession(self) -> Trie:
+        acc_iter = ReadFile.gene_refseq_uniprotkb_collab(infile, col=0)
+        for acc in acc_iter:
+            acc_trie.insert(acc)
+            self.meta['records'] += 1
+        self.meta['trie'] = acc_trie
+        # save trie
+        if self.save:
+            outfile = os.path.join(self.local_path, 'ncbi_refseq_protein_accession.trie')
+            ReadFile.dump_data(acc_trie, outfile)
+            self.meta['pickle_file'] = outfile
+        return self.meta
+    
+    def ncbi_uniprotkb_pacc(self, infile:str) -> dict:
         """
         source file: gene_refseq_uniprotkb_collab downloaded from NCBI/Entrez
-        suck NCBI protein accepython setup.pyssion numbers
+        suck UniProtKB protein accession numbers
         """
         acc_trie = Trie()
-        n = 0
-        self.records = ReadFile(self.infile).gene_refseq_uniprotkb_collab()
-        for items in self.records:
-            acc = items[0]
+        acc_iter = ReadFile.gene_refseq_uniprotkb_collab(infile, 1)
+        for acc in acc_iter:
             acc_trie.insert(acc)
-            n += 1
-        print(f"Total number of {n} NCBI protein accession numbers are fed into Trie.")
-        return acc_trie
-
-
-    def map_ncbi_uniprotkb(self) -> DiTrie:
-        '''
-        source file: gene_refseq_uniprotkb_collab downloaded from NCBI/Entrez
-        map: UniProtKB accession number ~ NCBI protein accession number
-        '''
-        uniprotkb_acc_trie = Trie()
-        ncbi_acc_trie = Trie()
-        map_trie = DiTrie(uniprotkb_acc_trie, ncbi_acc_trie)
-
-        n = 0
-        self.records = ReadFile(self.infile).gene_refseq_uniprotkb_collab()
-        for items in self.records:
-            ncbi_acc, uniprotkb_acc = items[:2]
-            map_trie.insert(ncbi_acc, uniprotkb_acc)
-            n += 1
-        return map_trie
-    
+            self.meta['records'] += 1
+        self.meta['trie'] = acc_trie
+        return self.meta
```

### Comparing `parseid-0.1.5/src/parseid/trie.py` & `parseid-0.2.0/src/parseid/trie.py`

 * *Files identical despite different names*

### Comparing `parseid-0.1.5/src/parseid/trie_node.py` & `parseid-0.2.0/src/parseid/trie_node.py`

 * *Files identical despite different names*

### Comparing `parseid-0.1.5/src/parseid.egg-info/PKG-INFO` & `parseid-0.2.0/src/parseid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: parseid
-Version: 0.1.5
+Version: 0.2.0
 Summary: suck, parse identifiers or accession numbers
 Home-page: https://github.com/Tiezhengyuan/parse_identifier
 Author: Tiezheng Yuan
 Author-email: tiezhengyuan@hotmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+Requires-Dist: bioomics
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: requests
 Requires-Dist: obonet
 Requires-Dist: python-dotenv
 
 \n# parseID: suck, parse identifiers or accession numbers
@@ -43,15 +44,15 @@
 There is one example about how huge accession numbers are sucked into Trie.
 The mapping file could be downloaded from https://ftp.ncbi.nlm.nih.gov/gene/DATA/gene_refseq_uniprotkb_collab.gz into local space.
 Retrieve 176,513,729 (03/25/2024) UniProt Accession numbers from the file and feed them into Trie.
 Showed as the example below, accession numbers are stored in the object uniprotkb_acc_trie. 
 ```
 from parseid import ProcessID
 infile = 'gene_refseq_uniprotkb_collab'
-uniprotkb_acc_trie = ProcessID(infile).uniprotkb_accession()
+uniprotkb_acc_trie = ProcessID(infile).uniprotkb_protein_accession()
 ```
 
 Retrieve pairs of NCBI protein accession number and UniProt Accession numbers
 from file and feed them into Ditrie. Showed as the example below, 
 the mapping fo two accession numbers are stored in the object map_trie, 
 which is ready for query or parsing.
 ```
```

### Comparing `parseid-0.1.5/tests/test_ditrie.py` & `parseid-0.2.0/tests/test_ditrie.py`

 * *Files identical despite different names*

### Comparing `parseid-0.1.5/tests/test_trie.py` & `parseid-0.2.0/tests/test_trie.py`

 * *Files identical despite different names*

### Comparing `parseid-0.1.5/tests/test_trie_node.py` & `parseid-0.2.0/tests/test_trie_node.py`

 * *Files identical despite different names*


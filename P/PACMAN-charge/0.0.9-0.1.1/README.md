# Comparing `tmp/PACMAN-charge-0.0.9.tar.gz` & `tmp/PACMAN-charge-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PACMAN-charge-0.0.9.tar", last modified: Wed May  1 02:34:19 2024, max compression
+gzip compressed data, was "PACMAN-charge-0.1.1.tar", last modified: Wed May  1 03:55:44 2024, max compression
```

## Comparing `PACMAN-charge-0.0.9.tar` & `PACMAN-charge-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 02:34:19.909228 PACMAN-charge-0.0.9/
--rwxrwxrwx   0 root         (0) root         (0)     1068 2024-03-25 02:54:44.000000 PACMAN-charge-0.0.9/LICENSE
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 02:34:19.789228 PACMAN-charge-0.0.9/PACMANCharge/
--rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-29 12:12:36.000000 PACMAN-charge-0.0.9/PACMANCharge/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    28392 2024-01-10 01:22:23.000000 PACMAN-charge-0.0.9/PACMANCharge/atom_init.json
--rwxrwxrwx   0 root         (0) root         (0)    27962 2024-05-01 02:12:18.000000 PACMAN-charge-0.0.9/PACMANCharge/pmcharge.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 02:34:19.854228 PACMAN-charge-0.0.9/PACMAN_charge.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     3306 2024-05-01 02:34:19.000000 PACMAN-charge-0.0.9/PACMAN_charge.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      334 2024-05-01 02:34:19.000000 PACMAN-charge-0.0.9/PACMAN_charge.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-01 02:34:19.000000 PACMAN-charge-0.0.9/PACMAN_charge.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      121 2024-05-01 02:34:19.000000 PACMAN-charge-0.0.9/PACMAN_charge.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2024-05-01 02:34:19.000000 PACMAN-charge-0.0.9/PACMAN_charge.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)     3306 2024-05-01 02:34:19.907228 PACMAN-charge-0.0.9/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2918 2024-05-01 02:30:46.000000 PACMAN-charge-0.0.9/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-01 02:34:19.909228 PACMAN-charge-0.0.9/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1038 2024-05-01 02:34:13.000000 PACMAN-charge-0.0.9/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 02:34:19.893228 PACMAN-charge-0.0.9/test/
--rwxrwxrwx   0 root         (0) root         (0)    34098 2024-04-30 05:03:22.000000 PACMAN-charge-0.0.9/test/Cu-BTC.cif
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-25 03:31:56.000000 PACMAN-charge-0.0.9/test/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      151 2024-04-30 05:03:05.000000 PACMAN-charge-0.0.9/test/test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 03:55:44.883831 PACMAN-charge-0.1.1/
+-rwxrwxrwx   0 root         (0) root         (0)     1068 2024-03-25 02:54:44.000000 PACMAN-charge-0.1.1/LICENSE
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 03:55:44.766829 PACMAN-charge-0.1.1/PACMANCharge/
+-rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-29 12:12:36.000000 PACMAN-charge-0.1.1/PACMANCharge/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    28392 2024-01-10 01:22:23.000000 PACMAN-charge-0.1.1/PACMANCharge/atom_init.json
+-rwxrwxrwx   0 root         (0) root         (0)    28212 2024-05-01 02:39:25.000000 PACMAN-charge-0.1.1/PACMANCharge/pmcharge.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 03:55:44.828830 PACMAN-charge-0.1.1/PACMAN_charge.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     3306 2024-05-01 03:55:44.000000 PACMAN-charge-0.1.1/PACMAN_charge.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      334 2024-05-01 03:55:44.000000 PACMAN-charge-0.1.1/PACMAN_charge.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-01 03:55:44.000000 PACMAN-charge-0.1.1/PACMAN_charge.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      121 2024-05-01 03:55:44.000000 PACMAN-charge-0.1.1/PACMAN_charge.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2024-05-01 03:55:44.000000 PACMAN-charge-0.1.1/PACMAN_charge.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     3306 2024-05-01 03:55:44.881831 PACMAN-charge-0.1.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2918 2024-05-01 02:30:46.000000 PACMAN-charge-0.1.1/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-01 03:55:44.883831 PACMAN-charge-0.1.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1038 2024-05-01 03:55:25.000000 PACMAN-charge-0.1.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-01 03:55:44.866830 PACMAN-charge-0.1.1/test/
+-rwxrwxrwx   0 root         (0) root         (0)    34098 2024-05-01 02:36:11.000000 PACMAN-charge-0.1.1/test/Cu-BTC.cif
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-25 03:31:56.000000 PACMAN-charge-0.1.1/test/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       76 2024-05-01 02:36:03.000000 PACMAN-charge-0.1.1/test/test.py
```

### Comparing `PACMAN-charge-0.0.9/LICENSE` & `PACMAN-charge-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PACMAN-charge-0.0.9/PACMANCharge/atom_init.json` & `PACMAN-charge-0.1.1/PACMANCharge/atom_init.json`

 * *Files identical despite different names*

### Comparing `PACMAN-charge-0.0.9/PACMANCharge/pmcharge.py` & `PACMAN-charge-0.1.1/PACMANCharge/pmcharge.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,16 @@
     'At', 'Rn', 'Fr', 'Ra', 'Ac', 'Th', 'Pa', 'U', 'Np', 'Pu', 'Am', 'Cm',
     'Bk', 'Cf', 'Es', 'Fm', 'Md', 'No', 'Lr', 'Rf', 'Db', 'Sg', 'Bh', 'Hs',
     'Mt', 'Ds', 'Rg', 'Cn', 'Nh', 'Fl', 'Mc', 'Lv', 'Ts', 'Og'
     ]
 
 device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
+print("using: " + device)
+
 def ase_format(mof):
     try:
         with warnings.catch_warnings():
             warnings.simplefilter('ignore')
             mof_temp = Structure.from_file(mof)
             mof_temp.to(filename=mof, fmt="cif")
             struc = read(mof)
@@ -527,15 +529,23 @@
         raise ValueError("For COF, please use DDEC charges.")
     try:
         with open(nor_name, 'rb') as f:
             charge_nor = pickle.load(f)
         f.close()
     except FileNotFoundError:
         print(f"Please use correct charge")
-         
+    
+
+    print(f"CIF Name: {cif_file}")
+    print(f"Model Name: {model_name}")
+    print(f"Charge Type: {charge_type}")
+    print(f"Digits: {digits}")
+    print(f"Atom Type: {atom_type}")
+    print(f"Neutral: {neutral}")
+
     try:
         struc = ase_format(cif_file)
         crystal_data = CIF2json(struc,cif_file)
         cell,pos=pre4pre(cif_file)
         dataset = CIFData(crystal_data,pos,cell,6,0,0.2)
         loader= get_data_loader(dataset=dataset, batch_size=1, num_workers=0, collate_fn=collate_pool, pin_memory=False)
         for batch in loader:
```

### Comparing `PACMAN-charge-0.0.9/PACMAN_charge.egg-info/PKG-INFO` & `PACMAN-charge-0.1.1/PACMAN_charge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PACMAN-charge
-Version: 0.0.9
+Version: 0.1.1
 Summary: Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)
 Home-page: https://github.com/sxm13/PACMAN
 Author: Guobin Zhao
 Author-email: sxmzhaogb@gmai.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PACMAN-charge-0.0.9/PKG-INFO` & `PACMAN-charge-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PACMAN-charge
-Version: 0.0.9
+Version: 0.1.1
 Summary: Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)
 Home-page: https://github.com/sxm13/PACMAN
 Author: Guobin Zhao
 Author-email: sxmzhaogb@gmai.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PACMAN-charge-0.0.9/README.md` & `PACMAN-charge-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `PACMAN-charge-0.0.9/setup.py` & `PACMAN-charge-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 from setuptools import setup, find_packages
 
 setup(
     name="PACMAN-charge",
-    version="0.0.9",
+    version="0.1.1",
     packages=find_packages(),
     description="Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)",
     author="Guobin Zhao",
     author_email="sxmzhaogb@gmai.com",
     url="https://github.com/sxm13/PACMAN",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

### Comparing `PACMAN-charge-0.0.9/test/Cu-BTC.cif` & `PACMAN-charge-0.1.1/test/Cu-BTC.cif`

 * *Files identical despite different names*


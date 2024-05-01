# Comparing `tmp/lielab-0.3.0-cp39-none-win_amd64.whl.zip` & `tmp/lielab-0.3.1-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 520546 bytes, number of entries: 18
+Zip file size: 544248 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat      280 b- defN 24-Apr-30 20:01 lielab/__init__.py
--rw-rw-rw-  2.0 fat  1417216 b- defN 24-Apr-30 20:11 lielab/cppLielab.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat  1513472 b- defN 24-May-01 01:47 lielab/cppLielab.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat       69 b- defN 24-Apr-29 19:07 lielab/domain/__init__.py
 -rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-29 14:50 lielab/domain/domain.py
 -rw-rw-rw-  2.0 fat       36 b- defN 24-Apr-29 19:07 lielab/dynamics/__init__.py
 -rw-rw-rw-  2.0 fat       37 b- defN 24-Apr-29 19:07 lielab/functions/__init__.py
 -rw-rw-rw-  2.0 fat       53 b- defN 24-Apr-29 19:07 lielab/kinematics/__init__.py
 -rw-rw-rw-  2.0 fat       40 b- defN 24-Apr-29 14:50 lielab/optim/__init__.py
 -rw-rw-rw-  2.0 fat     1493 b- defN 24-Apr-29 19:08 lielab/optim/optim.py
 -rw-rw-rw-  2.0 fat       26 b- defN 24-Apr-29 14:50 lielab/testing/__init__.py
 -rw-rw-rw-  2.0 fat     1121 b- defN 24-Apr-30 15:29 lielab/testing/test_main.py
 -rw-rw-rw-  2.0 fat      299 b- defN 24-Apr-29 19:08 lielab/topos/__init__.py
 -rw-rw-rw-  2.0 fat     7311 b- defN 24-Apr-30 20:01 lielab/topos/topos.py
 -rw-rw-rw-  2.0 fat       52 b- defN 24-Apr-29 19:08 lielab/transform/__init__.py
--rw-rw-rw-  2.0 fat      426 b- defN 24-Apr-30 20:11 lielab-0.3.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       99 b- defN 24-Apr-30 20:11 lielab-0.3.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 24-Apr-30 20:11 lielab-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1430 b- defN 24-Apr-30 20:11 lielab-0.3.0.dist-info/RECORD
-18 files, 1430001 bytes uncompressed, 518196 bytes compressed:  63.8%
+-rw-rw-rw-  2.0 fat      426 b- defN 24-May-01 01:47 lielab-0.3.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       99 b- defN 24-May-01 01:47 lielab-0.3.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 24-May-01 01:47 lielab-0.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1430 b- defN 24-May-01 01:47 lielab-0.3.1.dist-info/RECORD
+18 files, 1526257 bytes uncompressed, 541898 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: lielab/topos/topos.py
 Comment: 
 
 Filename: lielab/transform/__init__.py
 Comment: 
 
-Filename: lielab-0.3.0.dist-info/METADATA
+Filename: lielab-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: lielab-0.3.0.dist-info/WHEEL
+Filename: lielab-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: lielab-0.3.0.dist-info/top_level.txt
+Filename: lielab-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: lielab-0.3.0.dist-info/RECORD
+Filename: lielab-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `lielab-0.3.0.dist-info/RECORD` & `lielab-0.3.1.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 lielab/__init__.py,sha256=LFQi2iGSbohs3WadEnQPu8HFx2jvFbkdbElI1YPacss,280
-lielab/cppLielab.cp39-win_amd64.pyd,sha256=EPCIBE_c88M7j0mE0EEwxKyHUp5fkcw9ZLl6kVdcLBk,1417216
+lielab/cppLielab.cp39-win_amd64.pyd,sha256=jBJM0Q2gPCfMtvXYCDwT8RJq2LWpa5yrUxI-0V7P9CQ,1513472
 lielab/domain/__init__.py,sha256=PStXsJzII6Wlvwp7_qz83qmFRK6W_ukms-wixW30Fvo,69
 lielab/domain/domain.py,sha256=4LqLcvNhtvT3HceKC3pXBHW91E4XbKrWBLoTQghHVAM,6
 lielab/dynamics/__init__.py,sha256=uY2bANdqe1Ync84sNlPZ7dXvzs_-ShLRxdO14iaXBIo,36
 lielab/functions/__init__.py,sha256=C7X_4ZXbxT0eZk6s16XnaYcuGrtcHB2tCw5I3vJCOMk,37
 lielab/kinematics/__init__.py,sha256=uJ4DSgyf7R-DEAqx4o7VclzM8KX19MZCvEWzJ7zPfcE,53
 lielab/optim/__init__.py,sha256=IAW-KAH333WntIfg8q8npBprslakfzm6HXW51cYpSiI,40
 lielab/optim/optim.py,sha256=oGRsWUpIEEZff-orJJCp_7a982P28uDmUOltt272DiI,1493
 lielab/testing/__init__.py,sha256=XpODxsRFa9XoccjVmyJbodn-8fGcImF6-FWiOwiF5zc,26
 lielab/testing/test_main.py,sha256=O9njGD00F9EGArHp7mxriPaZJEDmDgmtSBM46fchcRY,1121
 lielab/topos/__init__.py,sha256=a-GKNPzGlHdDFi2CKHq_mTHhgRbGyOPdUK3bnfErDe4,299
 lielab/topos/topos.py,sha256=qzG3O6DwI7MmrEFh6VHjRK6W6slzwAPw2Xz7lpV8yAo,7311
 lielab/transform/__init__.py,sha256=SZuzG6ZwX9m8FyMj_eaEcg4NNvRpg-YefeFQ0QjoK4o,52
-lielab-0.3.0.dist-info/METADATA,sha256=GkVhDq1nVmBu3OklAWDqBFPfcJLY4jXjN7tbS8mjypE,426
-lielab-0.3.0.dist-info/WHEEL,sha256=84k4JvWE8cV5_6CN8EU9agcTRj3pW9Rpqf6Ri4aXgxo,99
-lielab-0.3.0.dist-info/top_level.txt,sha256=dxN-YjUmd9gmjZjUxDqBVJrK1sF1eZ3zfmF47S_xXD8,7
-lielab-0.3.0.dist-info/RECORD,,
+lielab-0.3.1.dist-info/METADATA,sha256=ewBXHGo7N64i6QFL0kGqq85gIVTf78hYpi7AhM3TpZY,426
+lielab-0.3.1.dist-info/WHEEL,sha256=84k4JvWE8cV5_6CN8EU9agcTRj3pW9Rpqf6Ri4aXgxo,99
+lielab-0.3.1.dist-info/top_level.txt,sha256=dxN-YjUmd9gmjZjUxDqBVJrK1sF1eZ3zfmF47S_xXD8,7
+lielab-0.3.1.dist-info/RECORD,,
```


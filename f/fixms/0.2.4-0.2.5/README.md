# Comparing `tmp/fixms-0.2.4.tar.gz` & `tmp/fixms-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixms-0.2.4.tar", max compression
+gzip compressed data, was "fixms-0.2.5.tar", max compression
```

## Comparing `fixms-0.2.4.tar` & `fixms-0.2.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2024-04-09 08:59:49.808570 fixms-0.2.4/LICENSE
--rw-r--r--   0        0        0     4935 2024-04-09 08:59:49.808570 fixms-0.2.4/README.md
--rw-r--r--   0        0        0        0 2024-04-09 08:59:49.808570 fixms-0.2.4/fixms/__init__.py
--rw-r--r--   0        0        0     1812 2024-04-09 08:59:49.808570 fixms-0.2.4/fixms/fix_ms.py
--rw-r--r--   0        0        0    20122 2024-04-09 08:59:49.808570 fixms-0.2.4/fixms/fix_ms_corrs.py
--rw-r--r--   0        0        0    14376 2024-04-09 08:59:49.808570 fixms-0.2.4/fixms/fix_ms_dir.py
--rw-r--r--   0        0        0     5105 2024-04-09 08:59:49.808570 fixms-0.2.4/fixms/logger.py
--rw-r--r--   0        0        0      886 2024-04-09 08:59:49.808570 fixms-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     5631 1970-01-01 00:00:00.000000 fixms-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-01 02:30:27.777394 fixms-0.2.5/LICENSE
+-rw-r--r--   0        0        0     4935 2024-05-01 02:30:27.777394 fixms-0.2.5/README.md
+-rw-r--r--   0        0        0        0 2024-05-01 02:30:27.777394 fixms-0.2.5/fixms/__init__.py
+-rw-r--r--   0        0        0     1812 2024-05-01 02:30:27.777394 fixms-0.2.5/fixms/fix_ms.py
+-rw-r--r--   0        0        0    20445 2024-05-01 02:30:27.777394 fixms-0.2.5/fixms/fix_ms_corrs.py
+-rw-r--r--   0        0        0    14376 2024-05-01 02:30:27.777394 fixms-0.2.5/fixms/fix_ms_dir.py
+-rw-r--r--   0        0        0     5105 2024-05-01 02:30:27.777394 fixms-0.2.5/fixms/logger.py
+-rw-r--r--   0        0        0      886 2024-05-01 02:30:27.777394 fixms-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     5631 1970-01-01 00:00:00.000000 fixms-0.2.5/PKG-INFO
```

### Comparing `fixms-0.2.4/LICENSE` & `fixms-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fixms-0.2.4/README.md` & `fixms-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `fixms-0.2.4/fixms/fix_ms.py` & `fixms-0.2.5/fixms/fix_ms.py`

 * *Files identical despite different names*

### Comparing `fixms-0.2.4/fixms/fix_ms_corrs.py` & `fixms-0.2.5/fixms/fix_ms_corrs.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,20 @@
 def set_pol_axis(ms: Path, pol_ang: u.Quantity, feed_idx: Optional[int] = None) -> None:
     with table((ms / "FEED").as_posix(), readonly=True, ack=False) as tf:
         ms_feed = tf.getcol("RECEPTOR_ANGLE") * u.rad
         # PAF is at 45deg to feeds
         # 45 - feed_angle = pol_angle
         pol_axes = -(ms_feed - 45.0 * u.deg)
 
+    # Backup the original RECEPTOR_ANGLE to INSTRUMENT_RECEPTOR_ANGLE
+    with table((ms / "FEED").as_posix(), readonly=False, ack=False) as tf:
+        tf.putcol("INSTRUMENT_RECEPTOR_ANGLE", ms_feed.to(u.rad).value)
+        tf.flush()
+    logger.info("Backed up the original RECEPTOR_ANGLE to INSTRUMENT_RECEPTOR_ANGLE")
+
     if feed_idx is None:
         assert (ms_feed[:, 0] == ms_feed[0, 0]).all() & (
             ms_feed[:, 1] == ms_feed[0, 1]
         ).all(), "The RECEPTOR_ANGLE changes with time, please check the MS"
 
         old_pol_ang = pol_axes[0, 0].to(u.deg)
     else:
```

### Comparing `fixms-0.2.4/fixms/fix_ms_dir.py` & `fixms-0.2.5/fixms/fix_ms_dir.py`

 * *Files identical despite different names*

### Comparing `fixms-0.2.4/fixms/logger.py` & `fixms-0.2.5/fixms/logger.py`

 * *Files identical despite different names*

### Comparing `fixms-0.2.4/pyproject.toml` & `fixms-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fixms"
-version = "0.2.4"
+version = "0.2.5"
 description = ""
 authors = ["Alec Thomson (S&A, Kensington WA) <alec.thomson@csiro.au>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
```

### Comparing `fixms-0.2.4/PKG-INFO` & `fixms-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixms
-Version: 0.2.4
+Version: 0.2.5
 Summary: 
 License: MIT
 Author: Alec Thomson (S&A, Kensington WA)
 Author-email: alec.thomson@csiro.au
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


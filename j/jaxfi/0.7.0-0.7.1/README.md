# Comparing `tmp/jaxfi-0.7.0-py3-none-any.whl.zip` & `tmp/jaxfi-0.7.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 16110 bytes, number of entries: 15
--rw-rw-r--  2.0 unx      524 b- defN 24-Apr-17 16:44 jaxfi/__init__.py
--rw-rw-r--  2.0 unx     7143 b- defN 24-Apr-17 16:49 jaxfi/api.py
--rw-rw-r--  2.0 unx     2679 b- defN 24-Apr-17 16:49 jaxfi/dynamic_lib_loading.py
--rw-rw-r--  2.0 unx    16362 b- defN 24-Apr-17 16:24 jaxfi/enumerated_jnp_members.py
+Zip file size: 16182 bytes, number of entries: 15
+-rw-rw-r--  2.0 unx      524 b- defN 24-May-01 17:37 jaxfi/__init__.py
+-rw-rw-r--  2.0 unx     7166 b- defN 24-May-01 17:37 jaxfi/api.py
+-rw-rw-r--  2.0 unx     2679 b- defN 24-May-01 17:37 jaxfi/dynamic_lib_loading.py
+-rw-rw-r--  2.0 unx    16362 b- defN 24-May-01 17:37 jaxfi/enumerated_jnp_members.py
 -rw-rw-r--  2.0 unx      114 b- defN 23-Apr-26 03:31 jaxfi/globals.py
 -rw-rw-r--  2.0 unx      169 b- defN 24-Jan-24 19:31 jaxfi/types.py
--rw-rw-r--  2.0 unx     6204 b- defN 24-Apr-17 16:49 jaxfi/utils.py
+-rw-rw-r--  2.0 unx     6345 b- defN 24-May-01 17:37 jaxfi/utils.py
 -rw-rw-r--  2.0 unx        0 b- defN 24-Jan-24 19:29 jaxfi/experimental/__init__.py
 -rw-rw-r--  2.0 unx     3035 b- defN 24-Jan-03 16:31 jaxfi/experimental/auto_pmap.py
 -rw-rw-r--  2.0 unx     3517 b- defN 23-Nov-10 18:47 jaxfi/experimental/jit.py
--rw-rw-r--  2.0 unx     1068 b- defN 24-Apr-17 17:05 jaxfi-0.7.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     6223 b- defN 24-Apr-17 17:05 jaxfi-0.7.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-17 17:05 jaxfi-0.7.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        6 b- defN 24-Apr-17 17:05 jaxfi-0.7.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1158 b- defN 24-Apr-17 17:05 jaxfi-0.7.0.dist-info/RECORD
-15 files, 48294 bytes uncompressed, 14214 bytes compressed:  70.6%
+-rw-rw-r--  2.0 unx     1068 b- defN 24-May-01 17:38 jaxfi-0.7.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     6223 b- defN 24-May-01 17:38 jaxfi-0.7.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-01 17:38 jaxfi-0.7.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        6 b- defN 24-May-01 17:38 jaxfi-0.7.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1158 b- defN 24-May-01 17:38 jaxfi-0.7.1.dist-info/RECORD
+15 files, 48458 bytes uncompressed, 14286 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: jaxfi/experimental/auto_pmap.py
 Comment: 
 
 Filename: jaxfi/experimental/jit.py
 Comment: 
 
-Filename: jaxfi-0.7.0.dist-info/LICENSE
+Filename: jaxfi-0.7.1.dist-info/LICENSE
 Comment: 
 
-Filename: jaxfi-0.7.0.dist-info/METADATA
+Filename: jaxfi-0.7.1.dist-info/METADATA
 Comment: 
 
-Filename: jaxfi-0.7.0.dist-info/WHEEL
+Filename: jaxfi-0.7.1.dist-info/WHEEL
 Comment: 
 
-Filename: jaxfi-0.7.0.dist-info/top_level.txt
+Filename: jaxfi-0.7.1.dist-info/top_level.txt
 Comment: 
 
-Filename: jaxfi-0.7.0.dist-info/RECORD
+Filename: jaxfi-0.7.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jaxfi/api.py

```diff
@@ -205,11 +205,11 @@
 # module bindings
 jax = jax
 numpy = jnp
 lax = jax.lax
 scipy = jsp
 random = jrandom
 
-_enable_pickling_fixes()
+_enable_pickling_fixes() # not currently in use
 
 ####################################################################################################
 globals.jaxm = sys.modules[__name__]
```

## jaxfi/utils.py

```diff
@@ -125,15 +125,18 @@
 def _make_jax_array(arr_value, device):
     import jax
 
     return jax.device_put(arr_value, device=device)
 
 
 def _pickle_array(arr: Array):
-    return _make_jax_array, (np.array(arr), arr.devices())
+    devices = tuple(arr.devices())
+    if len(devices) > 1:
+        raise NotImplementedError("jaxfi does not support pickling sharded arrays")
+    return _make_jax_array, (np.array(arr), devices[0])
 
 
 def _enable_pickling_fixes():
     import jaxlib
 
     copyreg.pickle(jaxlib.xla_extension.Device, _pickle_device)
     try:
```

## Comparing `jaxfi-0.7.0.dist-info/LICENSE` & `jaxfi-0.7.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jaxfi-0.7.0.dist-info/METADATA` & `jaxfi-0.7.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxfi
-Version: 0.7.0
+Version: 0.7.1
 Summary: Friendly Interface to JAX, that behaves similar to PyTorch while maintaining compatibility.
 Author: Robert Dyro
 Author-email: Robert Dyro <robert.dyro@gmail.com>
 Project-URL: Homepage, https://github.com/rdyro/jaxfi-JAXFriendlyInterface
 Project-URL: Bug Tracker, https://github.com/rdyro/jaxfi-JAXFriendlyInterface
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `jaxfi-0.7.0.dist-info/RECORD` & `jaxfi-0.7.1.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 jaxfi/__init__.py,sha256=qPGWAslLYk2I2asB8P4G93Si6RNqjlW4kzIzkrNYP8c,524
-jaxfi/api.py,sha256=laYe4ipVF6rf8iDua7P_3xLfCiujEqywpeelF1kmzpc,7143
+jaxfi/api.py,sha256=g8491iuPez1pKHLTsc7CWK3G3Ny9JHvvJgX_1SLX0ro,7166
 jaxfi/dynamic_lib_loading.py,sha256=vka7l2bbUwfGIZZsoWWHwEGUHVE21mwilUZqPB2r7do,2679
 jaxfi/enumerated_jnp_members.py,sha256=8i7LPXSwF5y8Ps-XRhXg8c90E4w1aJKK0MDF3KOtyKg,16362
 jaxfi/globals.py,sha256=PVptT3X5WjKXe3SO6yPkbBQ-1nIKpRHu5ehue2fS5JQ,114
 jaxfi/types.py,sha256=g6QfE9scN3B-YsVMtX35rJlZj-z99zN-MgD19mXHExU,169
-jaxfi/utils.py,sha256=HLtLrg8htLKrOPv7GXlfTtUHxEIpqoCQOpA7MNJCmSg,6204
+jaxfi/utils.py,sha256=hoDvWxfg7j5TOaIaibxNCDEKHz1DZ5EZN-DxIpfs0x4,6345
 jaxfi/experimental/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 jaxfi/experimental/auto_pmap.py,sha256=gZlWfEcKjApYu6yfkefKukc7ORFdIMe1uf7USxazPx8,3035
 jaxfi/experimental/jit.py,sha256=jDwrcaAHWRxQHZxHiBTzBP56lvRH4rRCKotZOYvg5bQ,3517
-jaxfi-0.7.0.dist-info/LICENSE,sha256=Y_vRJ8ePCccT_XKyn3V3moM24W2NoXqcKq0cSeZhCng,1068
-jaxfi-0.7.0.dist-info/METADATA,sha256=XXtWxpZ3vsydYcO8MjzyVNEMF700U65oFEP2xzbarVw,6223
-jaxfi-0.7.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-jaxfi-0.7.0.dist-info/top_level.txt,sha256=pMa_rDYgwq1q_ibjcWBU-h-oDQfzeSB_5UZ_I-76Pdw,6
-jaxfi-0.7.0.dist-info/RECORD,,
+jaxfi-0.7.1.dist-info/LICENSE,sha256=Y_vRJ8ePCccT_XKyn3V3moM24W2NoXqcKq0cSeZhCng,1068
+jaxfi-0.7.1.dist-info/METADATA,sha256=PcOUo2GSU8RBXJ2c_IWNFFW_tHcCQCC7JJ5WHr95Y9o,6223
+jaxfi-0.7.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+jaxfi-0.7.1.dist-info/top_level.txt,sha256=pMa_rDYgwq1q_ibjcWBU-h-oDQfzeSB_5UZ_I-76Pdw,6
+jaxfi-0.7.1.dist-info/RECORD,,
```


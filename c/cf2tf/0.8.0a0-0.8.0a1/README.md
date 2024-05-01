# Comparing `tmp/cf2tf-0.8.0a0.tar.gz` & `tmp/cf2tf-0.8.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cf2tf-0.8.0a0.tar", max compression
+gzip compressed data, was "cf2tf-0.8.0a1.tar", max compression
```

## Comparing `cf2tf-0.8.0a0.tar` & `cf2tf-0.8.0a1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/LICENSE.txt
--rw-r--r--   0        0        0     7485 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/README.md
--rw-r--r--   0        0        0     1089 2024-05-01 03:26:08.302907 cf2tf-0.8.0a0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/__init__.py
--rw-r--r--   0        0        0     1451 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/app.py
--rw-r--r--   0        0        0       46 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/cloudformation/__init__.py
--rw-r--r--   0        0        0     2621 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/cloudformation/_template.py
--rw-r--r--   0        0        0        0 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/conversion/__init__.py
--rw-r--r--   0        0        0    32457 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/conversion/expressions.py
--rw-r--r--   0        0        0     2026 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/conversion/overrides.py
--rw-r--r--   0        0        0    21718 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/convert.py
--rw-r--r--   0        0        0     2673 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/save.py
--rw-r--r--   0        0        0        0 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/terraform/__init__.py
--rw-r--r--   0        0        0      368 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/terraform/_configuration.py
--rw-r--r--   0        0        0     2199 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/terraform/blocks.py
--rw-r--r--   0        0        0     4099 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/terraform/code.py
--rw-r--r--   0        0        0     4691 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/terraform/doc_file.py
--rw-r--r--   0        0        0      304 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/terraform/hcl2/__init__.py
--rw-r--r--   0        0        0     2971 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/terraform/hcl2/_block.py
--rw-r--r--   0        0        0     1815 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/terraform/hcl2/complex.py
--rw-r--r--   0        0        0      868 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/terraform/hcl2/custom.py
--rw-r--r--   0        0        0     2673 2024-05-01 03:25:57.282929 cf2tf-0.8.0a0/src/cf2tf/terraform/hcl2/primitive.py
--rw-r--r--   0        0        0     8533 1970-01-01 00:00:00.000000 cf2tf-0.8.0a0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-01 03:40:56.920723 cf2tf-0.8.0a1/LICENSE.txt
+-rw-r--r--   0        0        0     7485 2024-05-01 03:40:56.920723 cf2tf-0.8.0a1/README.md
+-rw-r--r--   0        0        0     1089 2024-05-01 03:41:07.020805 cf2tf-0.8.0a1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-01 03:40:56.920723 cf2tf-0.8.0a1/src/cf2tf/__init__.py
+-rw-r--r--   0        0        0     1451 2024-05-01 03:40:56.920723 cf2tf-0.8.0a1/src/cf2tf/app.py
+-rw-r--r--   0        0        0       46 2024-05-01 03:40:56.920723 cf2tf-0.8.0a1/src/cf2tf/cloudformation/__init__.py
+-rw-r--r--   0        0        0     2621 2024-05-01 03:40:56.920723 cf2tf-0.8.0a1/src/cf2tf/cloudformation/_template.py
+-rw-r--r--   0        0        0        0 2024-05-01 03:40:56.920723 cf2tf-0.8.0a1/src/cf2tf/conversion/__init__.py
+-rw-r--r--   0        0        0    32457 2024-05-01 03:40:56.920723 cf2tf-0.8.0a1/src/cf2tf/conversion/expressions.py
+-rw-r--r--   0        0        0     2648 2024-05-01 03:40:56.920723 cf2tf-0.8.0a1/src/cf2tf/conversion/overrides.py
+-rw-r--r--   0        0        0    21720 2024-05-01 03:40:56.920723 cf2tf-0.8.0a1/src/cf2tf/convert.py
+-rw-r--r--   0        0        0     2673 2024-05-01 03:40:56.920723 cf2tf-0.8.0a1/src/cf2tf/save.py
+-rw-r--r--   0        0        0        0 2024-05-01 03:40:56.920723 cf2tf-0.8.0a1/src/cf2tf/terraform/__init__.py
+-rw-r--r--   0        0        0      368 2024-05-01 03:40:56.920723 cf2tf-0.8.0a1/src/cf2tf/terraform/_configuration.py
+-rw-r--r--   0        0        0     2199 2024-05-01 03:40:56.920723 cf2tf-0.8.0a1/src/cf2tf/terraform/blocks.py
+-rw-r--r--   0        0        0     4099 2024-05-01 03:40:56.920723 cf2tf-0.8.0a1/src/cf2tf/terraform/code.py
+-rw-r--r--   0        0        0     4691 2024-05-01 03:40:56.920723 cf2tf-0.8.0a1/src/cf2tf/terraform/doc_file.py
+-rw-r--r--   0        0        0      304 2024-05-01 03:40:56.920723 cf2tf-0.8.0a1/src/cf2tf/terraform/hcl2/__init__.py
+-rw-r--r--   0        0        0     2971 2024-05-01 03:40:56.920723 cf2tf-0.8.0a1/src/cf2tf/terraform/hcl2/_block.py
+-rw-r--r--   0        0        0     1815 2024-05-01 03:40:56.920723 cf2tf-0.8.0a1/src/cf2tf/terraform/hcl2/complex.py
+-rw-r--r--   0        0        0      868 2024-05-01 03:40:56.920723 cf2tf-0.8.0a1/src/cf2tf/terraform/hcl2/custom.py
+-rw-r--r--   0        0        0     2673 2024-05-01 03:40:56.920723 cf2tf-0.8.0a1/src/cf2tf/terraform/hcl2/primitive.py
+-rw-r--r--   0        0        0     8533 1970-01-01 00:00:00.000000 cf2tf-0.8.0a1/PKG-INFO
```

### Comparing `cf2tf-0.8.0a0/LICENSE.txt` & `cf2tf-0.8.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cf2tf-0.8.0a0/README.md` & `cf2tf-0.8.0a1/README.md`

 * *Files identical despite different names*

### Comparing `cf2tf-0.8.0a0/pyproject.toml` & `cf2tf-0.8.0a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cf2tf"
-version = "0.8.0a0"
+version = "0.8.0a1"
 description = "Convert Cloudformation Templates to Terraform."
 readme = "README.md"
 authors = ["Levi Blaney <shadycuz@gmail.com>"]
 repository = "https://github.com/DontShaveTheYak/cf2tf"
 keywords = ["cloudformation", "terraform", "cf2tf", "convert", "cloud", "conversion"]
 license = "GPL-3.0-only"
```

### Comparing `cf2tf-0.8.0a0/src/cf2tf/app.py` & `cf2tf-0.8.0a1/src/cf2tf/app.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.8.0a0/src/cf2tf/cloudformation/_template.py` & `cf2tf-0.8.0a1/src/cf2tf/cloudformation/_template.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.8.0a0/src/cf2tf/conversion/expressions.py` & `cf2tf-0.8.0a1/src/cf2tf/conversion/expressions.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.8.0a0/src/cf2tf/conversion/overrides.py` & `cf2tf-0.8.0a1/src/cf2tf/conversion/overrides.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import TYPE_CHECKING, Callable, Dict
 
+from cf2tf.terraform.hcl2.complex import ListType, MapType
 from cf2tf.terraform.hcl2.custom import LiteralType
 from cf2tf.terraform.hcl2.primitive import NullType, StringType, TerraformType
-from cf2tf.terraform.hcl2.complex import ListType, MapType
 
 if TYPE_CHECKING:
     from cf2tf.convert import TemplateConverter
 
 CFParams = Dict[str, TerraformType]
 
 Override = Callable[["TemplateConverter", CFParams], CFParams]
@@ -46,22 +46,41 @@
     return params
 
 
 def tag_conversion(_tc: "TemplateConverter", params: CFParams) -> CFParams:
     if isinstance(params["Tags"], dict):
         return params
 
-    orginal_tags: ListType = params["Tags"]  # type: ignore
+    original_tags: ListType = params["Tags"]  # type: ignore
 
-    new_tags = {LiteralType(tag["Key"]): tag["Value"] for tag in orginal_tags}
+    first_item = original_tags[0]
 
-    del params["Tags"]
-    params["tags"] = MapType(new_tags)
+    # It's possible that the tags might be one or more
+    # conditional statements of LiteralType
+    # This wont fix every case, but it should fix most
+    # and it's better than nothing
+    if not isinstance(first_item, (dict, MapType)):
+        del params["Tags"]
+        params["tags"] = first_item
+        return params
 
-    return params
+    try:
+        new_tags = {LiteralType(tag["Key"]): tag["Value"] for tag in original_tags}
+
+        del params["Tags"]
+        params["tags"] = MapType(new_tags)
+        return params
+    except Exception:
+        del params["Tags"]
+        params["tags"] = LiteralType(
+            f"// Could not convert tags: {original_tags.render(4)}"
+        )
+        return params
+
+    raise Exception("Could not convert tags")
 
 
 OVERRIDE_DISPATCH: ResourceOverride = {
     "aws_s3_bucket": {"AccessControl": s3_bucket_acl},
     "aws_s3_bucket_policy": {"PolicyDocument": s3_bucket_policy},
 }
```

### Comparing `cf2tf-0.8.0a0/src/cf2tf/convert.py` & `cf2tf-0.8.0a1/src/cf2tf/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -618,15 +618,15 @@
     if log.level == logging.DEBUG:
         print()
 
 
 def perform_resource_overrides(
     tf_type: str, params: Dict[str, TerraformType], tc: TemplateConverter
 ):
-    log.debug("Overiding params for {tf_type}")
+    log.debug(f"Overiding params for {tf_type}")
     if tf_type not in OVERRIDE_DISPATCH:
         return params
 
     param_overrides = OVERRIDE_DISPATCH[tf_type]
 
     for param, override in param_overrides.items():
         if param in params:
@@ -634,15 +634,15 @@
 
     return params
 
 
 def perform_global_overrides(
     tf_type: str, params: Dict[str, TerraformType], tc: TemplateConverter
 ):
-    log.debug("Performing global overrides for {tf_type}")
+    log.debug(f"Performing global overrides for {tf_type}")
 
     for param, override in GLOBAL_OVERRIDES.items():
         if param in params:
             params = override(tc, params)
 
     return params
```

### Comparing `cf2tf-0.8.0a0/src/cf2tf/save.py` & `cf2tf-0.8.0a1/src/cf2tf/save.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.8.0a0/src/cf2tf/terraform/blocks.py` & `cf2tf-0.8.0a1/src/cf2tf/terraform/blocks.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.8.0a0/src/cf2tf/terraform/code.py` & `cf2tf-0.8.0a1/src/cf2tf/terraform/code.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.8.0a0/src/cf2tf/terraform/doc_file.py` & `cf2tf-0.8.0a1/src/cf2tf/terraform/doc_file.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.8.0a0/src/cf2tf/terraform/hcl2/_block.py` & `cf2tf-0.8.0a1/src/cf2tf/terraform/hcl2/_block.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.8.0a0/src/cf2tf/terraform/hcl2/complex.py` & `cf2tf-0.8.0a1/src/cf2tf/terraform/hcl2/complex.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.8.0a0/src/cf2tf/terraform/hcl2/custom.py` & `cf2tf-0.8.0a1/src/cf2tf/terraform/hcl2/custom.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.8.0a0/src/cf2tf/terraform/hcl2/primitive.py` & `cf2tf-0.8.0a1/src/cf2tf/terraform/hcl2/primitive.py`

 * *Files identical despite different names*

### Comparing `cf2tf-0.8.0a0/PKG-INFO` & `cf2tf-0.8.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf2tf
-Version: 0.8.0a0
+Version: 0.8.0a1
 Summary: Convert Cloudformation Templates to Terraform.
 Home-page: https://github.com/DontShaveTheYak/cf2tf
 License: GPL-3.0-only
 Keywords: cloudformation,terraform,cf2tf,convert,cloud,conversion
 Author: Levi Blaney
 Author-email: shadycuz@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cf2tf Version: 0.8.0a0 Summary: Convert
+Metadata-Version: 2.1 Name: cf2tf Version: 0.8.0a1 Summary: Convert
 Cloudformation Templates to Terraform. Home-page: https://github.com/
 DontShaveTheYak/cf2tf License: GPL-3.0-only Keywords:
 cloudformation,terraform,cf2tf,convert,cloud,conversion Author: Levi Blaney
 Author-email: shadycuz@gmail.com Requires-Python: >=3.8.1,<4.0.0 Classifier:
 License :: OSI Approved :: GNU General Public License v3 (GPLv3) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```


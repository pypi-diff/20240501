# Comparing `tmp/japr-1.1.0.tar.gz` & `tmp/japr-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "japr-1.1.0.tar", max compression
+gzip compressed data, was "japr-1.2.0.tar", max compression
```

## Comparing `japr-1.1.0.tar` & `japr-1.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1067 2024-04-30 11:34:37.985451 japr-1.1.0/LICENSE.md
--rw-r--r--   0        0        0    20994 2024-04-30 11:34:37.985451 japr-1.1.0/README.md
--rw-r--r--   0        0        0      680 2024-04-30 11:34:37.989451 japr-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1148 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/check.py
--rw-r--r--   0        0        0     1160 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/check_providers/__init__.py
--rw-r--r--   0        0        0     1661 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/check_providers/ci_check_provider.py
--rw-r--r--   0        0        0     2526 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/check_providers/contributing_check_provider.py
--rw-r--r--   0        0        0     5633 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/check_providers/csharp_check_provider.py
--rw-r--r--   0        0        0     6577 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/check_providers/git_check_provider.py
--rw-r--r--   0        0        0     6645 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/check_providers/github_check_provider.py
--rw-r--r--   0        0        0     4379 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/check_providers/javascript_check_provider.py
--rw-r--r--   0        0        0     1392 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/check_providers/license_check_provider.py
--rw-r--r--   0        0        0     8043 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/check_providers/python_check_provider.py
--rw-r--r--   0        0        0     5201 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/check_providers/readme_check_provider.py
--rw-r--r--   0        0        0     2118 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/check_providers/rust_check_provider.py
--rw-r--r--   0        0        0     8449 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/check_providers/terraform_check_provider.py
--rw-r--r--   0        0        0    11543 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/japr.py
--rw-r--r--   0        0        0      968 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/template_util.py
--rw-r--r--   0        0        0     9470 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/templates/CONTRIBUTING.md
--rw-r--r--   0        0        0     1093 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/templates/README.md
--rw-r--r--   0        0        0      826 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/templates/bug_report_issue_template.md
--rw-r--r--   0        0        0      601 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/templates/feature_request_issue_template.md
--rw-r--r--   0        0        0      915 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/templates/pull_request_template.md
--rw-r--r--   0        0        0     1042 2024-04-30 11:34:37.989451 japr-1.1.0/src/japr/util.py
--rw-r--r--   0        0        0    21696 1970-01-01 00:00:00.000000 japr-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-01 14:35:47.709237 japr-1.2.0/LICENSE.md
+-rw-r--r--   0        0        0    21514 2024-05-01 14:35:47.709237 japr-1.2.0/README.md
+-rw-r--r--   0        0        0      680 2024-05-01 14:35:47.713237 japr-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1148 2024-05-01 14:35:47.713237 japr-1.2.0/src/japr/check.py
+-rw-r--r--   0        0        0     1160 2024-05-01 14:35:47.713237 japr-1.2.0/src/japr/check_providers/__init__.py
+-rw-r--r--   0        0        0     1661 2024-05-01 14:35:47.713237 japr-1.2.0/src/japr/check_providers/ci_check_provider.py
+-rw-r--r--   0        0        0     2526 2024-05-01 14:35:47.713237 japr-1.2.0/src/japr/check_providers/contributing_check_provider.py
+-rw-r--r--   0        0        0     5633 2024-05-01 14:35:47.713237 japr-1.2.0/src/japr/check_providers/csharp_check_provider.py
+-rw-r--r--   0        0        0     6577 2024-05-01 14:35:47.713237 japr-1.2.0/src/japr/check_providers/git_check_provider.py
+-rw-r--r--   0        0        0     6645 2024-05-01 14:35:47.713237 japr-1.2.0/src/japr/check_providers/github_check_provider.py
+-rw-r--r--   0        0        0     4379 2024-05-01 14:35:47.713237 japr-1.2.0/src/japr/check_providers/javascript_check_provider.py
+-rw-r--r--   0        0        0     1392 2024-05-01 14:35:47.713237 japr-1.2.0/src/japr/check_providers/license_check_provider.py
+-rw-r--r--   0        0        0     8043 2024-05-01 14:35:47.713237 japr-1.2.0/src/japr/check_providers/python_check_provider.py
+-rw-r--r--   0        0        0     5201 2024-05-01 14:35:47.713237 japr-1.2.0/src/japr/check_providers/readme_check_provider.py
+-rw-r--r--   0        0        0     2118 2024-05-01 14:35:47.713237 japr-1.2.0/src/japr/check_providers/rust_check_provider.py
+-rw-r--r--   0        0        0    10498 2024-05-01 14:35:47.713237 japr-1.2.0/src/japr/check_providers/terraform_check_provider.py
+-rw-r--r--   0        0        0    11543 2024-05-01 14:35:47.713237 japr-1.2.0/src/japr/japr.py
+-rw-r--r--   0        0        0      968 2024-05-01 14:35:47.713237 japr-1.2.0/src/japr/template_util.py
+-rw-r--r--   0        0        0     9470 2024-05-01 14:35:47.713237 japr-1.2.0/src/japr/templates/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1093 2024-05-01 14:35:47.713237 japr-1.2.0/src/japr/templates/README.md
+-rw-r--r--   0        0        0      826 2024-05-01 14:35:47.713237 japr-1.2.0/src/japr/templates/bug_report_issue_template.md
+-rw-r--r--   0        0        0      601 2024-05-01 14:35:47.713237 japr-1.2.0/src/japr/templates/feature_request_issue_template.md
+-rw-r--r--   0        0        0      915 2024-05-01 14:35:47.713237 japr-1.2.0/src/japr/templates/pull_request_template.md
+-rw-r--r--   0        0        0     1042 2024-05-01 14:35:47.713237 japr-1.2.0/src/japr/util.py
+-rw-r--r--   0        0        0    22216 1970-01-01 00:00:00.000000 japr-1.2.0/PKG-INFO
```

### Comparing `japr-1.1.0/LICENSE.md` & `japr-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `japr-1.1.0/README.md` & `japr-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -211,7 +211,8 @@
 |----|----------|---------------------------|-------------|--------|
 | TF004 | Medium | open-source, inner-source, team, personal | Terraform projects should have their Terraform lock files committed into Git | When using Terraform, the lock files should be comitted into Git. This ensures that all dependencies of packages are installed at the same version no matter when and on what machine the project is installed. |
 | TF005 | Medium | open-source, inner-source, team, personal | Terraform projects should not have their .terraform directory committed into Git | The .terraform directory contains binaries, thrid party modules and other things that are generated during a terraform init. This folder should not be committed into git. |
 | TF006 | High | open-source, inner-source, team, personal | Terraform state files should not be committed into git | Terraform state files can contain secrets and are stored unencrypted. These secrets can be easily leaked when stored in git. Additionally, terraform state in git does not provide a single source of truth nor state locking and so can cause major issues when used in teams.</br></br>Instead of storing state in git, use another terraform backend</br></br>See https://developer.hashicorp.com/terraform/language/settings/backends/configuration |
 | TF007 | Low | open-source, inner-source, team, personal | Terraform modules should contain a main.tf file | When creating terraform modules (or using terraform in general) each module should contain a minimum of a main.tf, outputs.tf and a variables.tf file, even if these are empty.</br></br>See https://developer.hashicorp.com/terraform/language/modules/develop/structure |
 | TF008 | Low | open-source, inner-source, team, personal | Terraform modules should contain an outputs.tf file | When creating terraform modules (or using terraform in general) each module should contain a minimum of a main.tf, outputs.tf and a variables.tf file, even if these are empty.</br></br>See https://developer.hashicorp.com/terraform/language/modules/develop/structure |
 | TF009 | Low | open-source, inner-source, team, personal | Terraform modules should contain a variables.tf file | When creating terraform modules (or using terraform in general) each module should contain a minimum of a main.tf, outputs.tf and a variables.tf file, even if these are empty.</br></br>See https://developer.hashicorp.com/terraform/language/modules/develop/structure |
+| TF010 | Low | open-source, inner-source, team, personal | Terraform submodules should be contained in a 'modules' directory | When creating submodules in a terraform module or project the submodules should be contained in a 'modules' directory. For example:</br>root/</br>|- modules/</br>|  '- my-submodule/</br>|     |-main.tf</br>|     |-outputs.tf</br>|     '-variables.tf</br>|-main.tf</br>|-outputs.tf</br>'-variables.tf</br></br>See https://developer.hashicorp.com/terraform/language/modules/develop/structure |
```

### Comparing `japr-1.1.0/pyproject.toml` & `japr-1.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Japr"
-version = "1.1.0"
+version = "1.2.0"
 description = "A cross-language tool for rating the overall quality of open source, commercial and personal projects"
 authors = ["Jamie Read <hey@jread.dev>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "japr", from = "src"}]
 
 [tool.poetry.scripts]
```

### Comparing `japr-1.1.0/src/japr/check.py` & `japr-1.2.0/src/japr/check.py`

 * *Files identical despite different names*

### Comparing `japr-1.1.0/src/japr/check_providers/__init__.py` & `japr-1.2.0/src/japr/check_providers/__init__.py`

 * *Files identical despite different names*

### Comparing `japr-1.1.0/src/japr/check_providers/ci_check_provider.py` & `japr-1.2.0/src/japr/check_providers/ci_check_provider.py`

 * *Files identical despite different names*

### Comparing `japr-1.1.0/src/japr/check_providers/contributing_check_provider.py` & `japr-1.2.0/src/japr/check_providers/contributing_check_provider.py`

 * *Files identical despite different names*

### Comparing `japr-1.1.0/src/japr/check_providers/csharp_check_provider.py` & `japr-1.2.0/src/japr/check_providers/csharp_check_provider.py`

 * *Files identical despite different names*

### Comparing `japr-1.1.0/src/japr/check_providers/git_check_provider.py` & `japr-1.2.0/src/japr/check_providers/git_check_provider.py`

 * *Files identical despite different names*

### Comparing `japr-1.1.0/src/japr/check_providers/github_check_provider.py` & `japr-1.2.0/src/japr/check_providers/github_check_provider.py`

 * *Files identical despite different names*

### Comparing `japr-1.1.0/src/japr/check_providers/javascript_check_provider.py` & `japr-1.2.0/src/japr/check_providers/javascript_check_provider.py`

 * *Files identical despite different names*

### Comparing `japr-1.1.0/src/japr/check_providers/license_check_provider.py` & `japr-1.2.0/src/japr/check_providers/license_check_provider.py`

 * *Files identical despite different names*

### Comparing `japr-1.1.0/src/japr/check_providers/python_check_provider.py` & `japr-1.2.0/src/japr/check_providers/python_check_provider.py`

 * *Files identical despite different names*

### Comparing `japr-1.1.0/src/japr/check_providers/readme_check_provider.py` & `japr-1.2.0/src/japr/check_providers/readme_check_provider.py`

 * *Files identical despite different names*

### Comparing `japr-1.1.0/src/japr/check_providers/rust_check_provider.py` & `japr-1.2.0/src/japr/check_providers/rust_check_provider.py`

 * *Files identical despite different names*

### Comparing `japr-1.1.0/src/japr/check_providers/terraform_check_provider.py` & `japr-1.2.0/src/japr/check_providers/terraform_check_provider.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 from japr.check import Check, CheckProvider, CheckResult, Result, Severity
 import japr.util
 from git import InvalidGitRepositoryError
 from git.repo import Repo
 import os
 
 
+def _is_subdir(path, directory):
+    path = os.path.realpath(path)
+    directory = os.path.realpath(directory)
+
+    relative = os.path.relpath(path, directory)
+
+    if relative.startswith(os.pardir):
+        return False
+    else:
+        return True
+
+
 class TerraformCheckProvider(CheckProvider):
     def name(self):
         return "Terraform"
 
     def test(self, directory):
         terraform_locks = list(
             japr.util.find_files_with_name(directory, ".terraform.lock.hcl")
@@ -120,18 +132,45 @@
                     os.path.join(terraform_dir, "variables.tf") in terraform_files
                 )
                 yield CheckResult(
                     "TF009",
                     Result.PASSED if has_variables_file else Result.FAILED,
                     terraform_dir,
                 )
+
+                # If we're a subdir of any other directory there should be a /modules/ directory between us
+                # Find closest parent from the other dirs
+                closest_parent = None
+                for other_dir in terraform_dirs:
+                    if terraform_dir != other_dir and _is_subdir(
+                        terraform_dir, other_dir
+                    ):
+                        if closest_parent is None or _is_subdir(
+                            closest_parent, other_dir
+                        ):
+                            closest_parent = other_dir
+
+                if closest_parent is not None:
+                    is_in_modules_dir = os.path.join(
+                        closest_parent, "modules"
+                    ) == os.path.dirname(terraform_dir)
+
+                    yield CheckResult(
+                        "TF010",
+                        Result.PASSED if is_in_modules_dir else Result.FAILED,
+                        terraform_dir,
+                    )
+                else:
+                    yield CheckResult("TF010", Result.NOT_APPLICABLE, terraform_dir)
+
         else:
             yield CheckResult("TF007", Result.NOT_APPLICABLE)
             yield CheckResult("TF008", Result.NOT_APPLICABLE)
             yield CheckResult("TF009", Result.NOT_APPLICABLE)
+            yield CheckResult("TF010", Result.NOT_APPLICABLE)
 
     def checks(self):
         return [
             Check(
                 "TF004",
                 Severity.MEDIUM,
                 ["open-source", "inner-source", "team", "personal"],
@@ -179,8 +218,26 @@
                 Severity.LOW,
                 ["open-source", "inner-source", "team", "personal"],
                 "Terraform modules should contain a variables.tf file",
                 """When creating terraform modules (or using terraform in general) each module should contain a minimum of a main.tf, outputs.tf and a variables.tf file, even if these are empty.
 
 See https://developer.hashicorp.com/terraform/language/modules/develop/structure""",
             ),
+            Check(
+                "TF010",
+                Severity.LOW,
+                ["open-source", "inner-source", "team", "personal"],
+                "Terraform submodules should be contained in a 'modules' directory",
+                """When creating submodules in a terraform module or project the submodules should be contained in a 'modules' directory. For example:
+root/
+|- modules/
+|  '- my-submodule/
+|     |-main.tf
+|     |-outputs.tf
+|     '-variables.tf
+|-main.tf
+|-outputs.tf
+'-variables.tf
+
+See https://developer.hashicorp.com/terraform/language/modules/develop/structure""",
+            ),
         ]
```

### Comparing `japr-1.1.0/src/japr/japr.py` & `japr-1.2.0/src/japr/japr.py`

 * *Files identical despite different names*

### Comparing `japr-1.1.0/src/japr/template_util.py` & `japr-1.2.0/src/japr/template_util.py`

 * *Files identical despite different names*

### Comparing `japr-1.1.0/src/japr/templates/CONTRIBUTING.md` & `japr-1.2.0/src/japr/templates/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `japr-1.1.0/src/japr/templates/README.md` & `japr-1.2.0/src/japr/templates/README.md`

 * *Files identical despite different names*

### Comparing `japr-1.1.0/src/japr/templates/bug_report_issue_template.md` & `japr-1.2.0/src/japr/templates/bug_report_issue_template.md`

 * *Files identical despite different names*

### Comparing `japr-1.1.0/src/japr/templates/feature_request_issue_template.md` & `japr-1.2.0/src/japr/templates/feature_request_issue_template.md`

 * *Files identical despite different names*

### Comparing `japr-1.1.0/src/japr/templates/pull_request_template.md` & `japr-1.2.0/src/japr/templates/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `japr-1.1.0/src/japr/util.py` & `japr-1.2.0/src/japr/util.py`

 * *Files identical despite different names*

### Comparing `japr-1.1.0/PKG-INFO` & `japr-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Japr
-Version: 1.1.0
+Version: 1.2.0
 Summary: A cross-language tool for rating the overall quality of open source, commercial and personal projects
 License: MIT
 Author: Jamie Read
 Author-email: hey@jread.dev
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -230,8 +230,9 @@
 |----|----------|---------------------------|-------------|--------|
 | TF004 | Medium | open-source, inner-source, team, personal | Terraform projects should have their Terraform lock files committed into Git | When using Terraform, the lock files should be comitted into Git. This ensures that all dependencies of packages are installed at the same version no matter when and on what machine the project is installed. |
 | TF005 | Medium | open-source, inner-source, team, personal | Terraform projects should not have their .terraform directory committed into Git | The .terraform directory contains binaries, thrid party modules and other things that are generated during a terraform init. This folder should not be committed into git. |
 | TF006 | High | open-source, inner-source, team, personal | Terraform state files should not be committed into git | Terraform state files can contain secrets and are stored unencrypted. These secrets can be easily leaked when stored in git. Additionally, terraform state in git does not provide a single source of truth nor state locking and so can cause major issues when used in teams.</br></br>Instead of storing state in git, use another terraform backend</br></br>See https://developer.hashicorp.com/terraform/language/settings/backends/configuration |
 | TF007 | Low | open-source, inner-source, team, personal | Terraform modules should contain a main.tf file | When creating terraform modules (or using terraform in general) each module should contain a minimum of a main.tf, outputs.tf and a variables.tf file, even if these are empty.</br></br>See https://developer.hashicorp.com/terraform/language/modules/develop/structure |
 | TF008 | Low | open-source, inner-source, team, personal | Terraform modules should contain an outputs.tf file | When creating terraform modules (or using terraform in general) each module should contain a minimum of a main.tf, outputs.tf and a variables.tf file, even if these are empty.</br></br>See https://developer.hashicorp.com/terraform/language/modules/develop/structure |
 | TF009 | Low | open-source, inner-source, team, personal | Terraform modules should contain a variables.tf file | When creating terraform modules (or using terraform in general) each module should contain a minimum of a main.tf, outputs.tf and a variables.tf file, even if these are empty.</br></br>See https://developer.hashicorp.com/terraform/language/modules/develop/structure |
+| TF010 | Low | open-source, inner-source, team, personal | Terraform submodules should be contained in a 'modules' directory | When creating submodules in a terraform module or project the submodules should be contained in a 'modules' directory. For example:</br>root/</br>|- modules/</br>|  '- my-submodule/</br>|     |-main.tf</br>|     |-outputs.tf</br>|     '-variables.tf</br>|-main.tf</br>|-outputs.tf</br>'-variables.tf</br></br>See https://developer.hashicorp.com/terraform/language/modules/develop/structure |
```


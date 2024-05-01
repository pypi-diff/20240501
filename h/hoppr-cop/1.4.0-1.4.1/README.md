# Comparing `tmp/hoppr_cop-1.4.0.tar.gz` & `tmp/hoppr_cop-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoppr_cop-1.4.0.tar", max compression
+gzip compressed data, was "hoppr_cop-1.4.1.tar", max compression
```

## Comparing `hoppr_cop-1.4.0.tar` & `hoppr_cop-1.4.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1084 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/LICENSE.md
--rw-r--r--   0        0        0       94 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/combined/__init__.py
--rw-r--r--   0        0        0     7988 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/combined/cli.py
--rw-r--r--   0        0        0     9899 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/combined/combined_scanner.py
--rw-r--r--   0        0        0        0 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/combined/py.typed
--rw-r--r--   0        0        0    18103 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/enhancements/analysis_assessment.py
--rw-r--r--   0        0        0        0 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/enhancements/epss/__init__.py
--rw-r--r--   0        0        0      586 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/enhancements/epss/models.py
--rw-r--r--   0        0        0     4328 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/enhancements/epss_enhancer.py
--rw-r--r--   0        0        0        0 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/gemnasium/__init__.py
--rw-r--r--   0        0        0    13609 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/gemnasium/gemnasium_scanner.py
--rw-r--r--   0        0        0     1974 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/gemnasium/models.py
--rw-r--r--   0        0        0        0 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/gemnasium/py.typed
--rwxr-xr-x   0        0        0      113 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/gemnasium/semver
--rw-r--r--   0        0        0        0 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/grype/__init__.py
--rw-r--r--   0        0        0    14796 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/grype/grype_scanner.py
--rw-r--r--   0        0        0     8574 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/grype/models.py
--rw-r--r--   0        0        0        0 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/grype/py.typed
--rw-r--r--   0        0        0        0 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/hoppr_plugin/__init__.py
--rw-r--r--   0        0        0     4867 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/hoppr_plugin/hopprcop_plugin.py
--rw-r--r--   0        0        0        0 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/hoppr_plugin/py.typed
--rw-r--r--   0        0        0      478 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/ossindex/README.md
--rw-r--r--   0        0        0        0 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/ossindex/__init__.py
--rw-r--r--   0        0        0      832 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/ossindex/api/__init__.py
--rw-r--r--   0        0        0     1048 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/ossindex/api/exception.py
--rw-r--r--   0        0        0     9278 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/ossindex/api/model.py
--rw-r--r--   0        0        0    10293 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/ossindex/api/ossindex.py
--rw-r--r--   0        0        0      153 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/ossindex/api/py.typed
--rw-r--r--   0        0        0     2997 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/ossindex/api/serializer.py
--rw-r--r--   0        0        0    10447 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/ossindex/oss_index_scanner.py
--rw-r--r--   0        0        0        0 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/ossindex/py.typed
--rw-r--r--   0        0        0        0 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/py.typed
--rw-r--r--   0        0        0    19750 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/reporting/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/reporting/gitlab/__init__.py
--rw-r--r--   0        0        0    23684 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/reporting/gitlab/models.py
--rw-r--r--   0        0        0     1729 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/reporting/models.py
--rw-r--r--   0        0        0        0 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/reporting/py.typed
--rw-r--r--   0        0        0    13776 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/reporting/templates/assets/vulnerabilities.css
--rw-r--r--   0        0        0    62168 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/reporting/templates/package-lock.json
--rw-r--r--   0        0        0       56 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/reporting/templates/package.json
--rw-r--r--   0        0        0      135 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/reporting/templates/tailwind.config.js
--rw-r--r--   0        0        0     3423 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/reporting/templates/vulnerabilities.html
--rw-r--r--   0        0        0       58 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/reporting/templates/vulnerability.css
--rw-r--r--   0        0        0    10840 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/reporting/templates/vulnerability_details.html
--rw-r--r--   0        0        0        0 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/trivy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/trivy/py.typed
--rw-r--r--   0        0        0    10960 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/trivy/trivy_scanner.py
--rw-r--r--   0        0        0    10374 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/utils.py
--rw-r--r--   0        0        0     4179 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/vulnerability_combiner.py
--rw-r--r--   0        0        0     2652 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/vulnerability_enhancer.py
--rw-r--r--   0        0        0     6973 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/hopprcop/vulnerability_scanner.py
--rw-r--r--   0        0        0     6425 2024-04-04 05:06:18.000000 hoppr_cop-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 hoppr_cop-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-05-01 15:06:24.000000 hoppr_cop-1.4.1/LICENSE.md
+-rw-r--r--   0        0        0       94 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/combined/__init__.py
+-rw-r--r--   0        0        0     7988 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/combined/cli.py
+-rw-r--r--   0        0        0     9899 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/combined/combined_scanner.py
+-rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/combined/py.typed
+-rw-r--r--   0        0        0    18103 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/enhancements/analysis_assessment.py
+-rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/enhancements/epss/__init__.py
+-rw-r--r--   0        0        0      586 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/enhancements/epss/models.py
+-rw-r--r--   0        0        0     4328 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/enhancements/epss_enhancer.py
+-rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/gemnasium/__init__.py
+-rw-r--r--   0        0        0    13609 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/gemnasium/gemnasium_scanner.py
+-rw-r--r--   0        0        0     1974 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/gemnasium/models.py
+-rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/gemnasium/py.typed
+-rwxr-xr-x   0        0        0      113 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/gemnasium/semver
+-rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/grype/__init__.py
+-rw-r--r--   0        0        0    14796 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/grype/grype_scanner.py
+-rw-r--r--   0        0        0     8574 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/grype/models.py
+-rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/grype/py.typed
+-rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/hoppr_plugin/__init__.py
+-rw-r--r--   0        0        0     4989 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/hoppr_plugin/hopprcop_plugin.py
+-rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/hoppr_plugin/py.typed
+-rw-r--r--   0        0        0      478 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/ossindex/README.md
+-rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/ossindex/__init__.py
+-rw-r--r--   0        0        0      832 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/ossindex/api/__init__.py
+-rw-r--r--   0        0        0     1048 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/ossindex/api/exception.py
+-rw-r--r--   0        0        0     9278 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/ossindex/api/model.py
+-rw-r--r--   0        0        0    10293 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/ossindex/api/ossindex.py
+-rw-r--r--   0        0        0      153 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/ossindex/api/py.typed
+-rw-r--r--   0        0        0     2997 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/ossindex/api/serializer.py
+-rw-r--r--   0        0        0    10447 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/ossindex/oss_index_scanner.py
+-rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/ossindex/py.typed
+-rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/py.typed
+-rw-r--r--   0        0        0    19750 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/reporting/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/reporting/gitlab/__init__.py
+-rw-r--r--   0        0        0    23684 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/reporting/gitlab/models.py
+-rw-r--r--   0        0        0     1729 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/reporting/models.py
+-rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/reporting/py.typed
+-rw-r--r--   0        0        0    13776 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/reporting/templates/assets/vulnerabilities.css
+-rw-r--r--   0        0        0    62168 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/reporting/templates/package-lock.json
+-rw-r--r--   0        0        0       56 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/reporting/templates/package.json
+-rw-r--r--   0        0        0      135 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/reporting/templates/tailwind.config.js
+-rw-r--r--   0        0        0     3423 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/reporting/templates/vulnerabilities.html
+-rw-r--r--   0        0        0       58 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/reporting/templates/vulnerability.css
+-rw-r--r--   0        0        0    10840 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/reporting/templates/vulnerability_details.html
+-rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/trivy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/trivy/py.typed
+-rw-r--r--   0        0        0    10960 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/trivy/trivy_scanner.py
+-rw-r--r--   0        0        0    10374 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/utils.py
+-rw-r--r--   0        0        0     4179 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/vulnerability_combiner.py
+-rw-r--r--   0        0        0     2652 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/vulnerability_enhancer.py
+-rw-r--r--   0        0        0     6973 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/hopprcop/vulnerability_scanner.py
+-rw-r--r--   0        0        0     6425 2024-05-01 15:06:25.000000 hoppr_cop-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 hoppr_cop-1.4.1/PKG-INFO
```

### Comparing `hoppr_cop-1.4.0/LICENSE.md` & `hoppr_cop-1.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.0/hopprcop/combined/cli.py` & `hoppr_cop-1.4.1/hopprcop/combined/cli.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.0/hopprcop/combined/combined_scanner.py` & `hoppr_cop-1.4.1/hopprcop/combined/combined_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.0/hopprcop/enhancements/analysis_assessment.py` & `hoppr_cop-1.4.1/hopprcop/enhancements/analysis_assessment.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.0/hopprcop/enhancements/epss/models.py` & `hoppr_cop-1.4.1/hopprcop/enhancements/epss/models.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.0/hopprcop/enhancements/epss_enhancer.py` & `hoppr_cop-1.4.1/hopprcop/enhancements/epss_enhancer.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.0/hopprcop/gemnasium/gemnasium_scanner.py` & `hoppr_cop-1.4.1/hopprcop/gemnasium/gemnasium_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.0/hopprcop/gemnasium/models.py` & `hoppr_cop-1.4.1/hopprcop/gemnasium/models.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.0/hopprcop/grype/grype_scanner.py` & `hoppr_cop-1.4.1/hopprcop/grype/grype_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.0/hopprcop/grype/models.py` & `hoppr_cop-1.4.1/hopprcop/grype/models.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.0/hopprcop/hoppr_plugin/hopprcop_plugin.py` & `hoppr_cop-1.4.1/hopprcop/hoppr_plugin/hopprcop_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,16 @@
             version: int,
             vulnerabilities: list[Vulnerability] | None = None,
         ):
             self.serial_number = serial_number
             self.version = version
             self.vulnerabilities = vulnerabilities or []
 
+    products: Final[list[str]] = ["generic/*", "generic/hopprcop-vulnerability-results-details/*"]  # type: ignore[misc]
+
     EMBEDDED_VEX: Final[str] = "embedded_cyclone_dx_vex"
     LINKED_VEX: Final[str] = "linked_cyclone_dx_vex"
 
     bom_access = BomAccess.FULL_ACCESS
 
     DEFAULT_SCANNERS: Final[list[str]] = [
         "hopprcop.gemnasium.gemnasium_scanner.GemnasiumScanner",
```

### Comparing `hoppr_cop-1.4.0/hopprcop/ossindex/api/__init__.py` & `hoppr_cop-1.4.1/hopprcop/ossindex/api/__init__.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.0/hopprcop/ossindex/api/exception.py` & `hoppr_cop-1.4.1/hopprcop/ossindex/api/exception.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.0/hopprcop/ossindex/api/model.py` & `hoppr_cop-1.4.1/hopprcop/ossindex/api/model.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.0/hopprcop/ossindex/api/ossindex.py` & `hoppr_cop-1.4.1/hopprcop/ossindex/api/ossindex.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.0/hopprcop/ossindex/api/serializer.py` & `hoppr_cop-1.4.1/hopprcop/ossindex/api/serializer.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.0/hopprcop/ossindex/oss_index_scanner.py` & `hoppr_cop-1.4.1/hopprcop/ossindex/oss_index_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.0/hopprcop/reporting/__init__.py` & `hoppr_cop-1.4.1/hopprcop/reporting/__init__.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.0/hopprcop/reporting/gitlab/models.py` & `hoppr_cop-1.4.1/hopprcop/reporting/gitlab/models.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.0/hopprcop/reporting/models.py` & `hoppr_cop-1.4.1/hopprcop/reporting/models.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.0/hopprcop/reporting/templates/assets/vulnerabilities.css` & `hoppr_cop-1.4.1/hopprcop/reporting/templates/assets/vulnerabilities.css`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.0/hopprcop/reporting/templates/package-lock.json` & `hoppr_cop-1.4.1/hopprcop/reporting/templates/package-lock.json`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.0/hopprcop/reporting/templates/vulnerabilities.html` & `hoppr_cop-1.4.1/hopprcop/reporting/templates/vulnerabilities.html`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.0/hopprcop/reporting/templates/vulnerability_details.html` & `hoppr_cop-1.4.1/hopprcop/reporting/templates/vulnerability_details.html`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.0/hopprcop/trivy/trivy_scanner.py` & `hoppr_cop-1.4.1/hopprcop/trivy/trivy_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.0/hopprcop/utils.py` & `hoppr_cop-1.4.1/hopprcop/utils.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.0/hopprcop/vulnerability_combiner.py` & `hoppr_cop-1.4.1/hopprcop/vulnerability_combiner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.0/hopprcop/vulnerability_enhancer.py` & `hoppr_cop-1.4.1/hopprcop/vulnerability_enhancer.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.0/hopprcop/vulnerability_scanner.py` & `hoppr_cop-1.4.1/hopprcop/vulnerability_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_cop-1.4.0/pyproject.toml` & `hoppr_cop-1.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hoppr-cop"
-version = "1.4.0"
+version = "1.4.1"
 description = ""
 authors = ["kganger <keith.e.ganger@lmco.com>"]
 license = "MIT"
 
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
```

### Comparing `hoppr_cop-1.4.0/PKG-INFO` & `hoppr_cop-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoppr-cop
-Version: 1.4.0
+Version: 1.4.1
 Summary: 
 License: MIT
 Author: kganger
 Author-email: keith.e.ganger@lmco.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```


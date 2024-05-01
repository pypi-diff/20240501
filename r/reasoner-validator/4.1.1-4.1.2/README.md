# Comparing `tmp/reasoner_validator-4.1.1.tar.gz` & `tmp/reasoner_validator-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-4.1.1.tar", max compression
+gzip compressed data, was "reasoner_validator-4.1.2.tar", max compression
```

## Comparing `reasoner_validator-4.1.1.tar` & `reasoner_validator-4.1.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1153 2024-04-30 20:33:48.759168 reasoner_validator-4.1.1/LICENSE
--rw-r--r--   0        0        0    13727 2024-04-30 20:33:48.759168 reasoner_validator-4.1.1/README.md
--rw-r--r--   0        0        0      131 2024-04-30 20:33:48.759168 reasoner_validator-4.1.1/docs/.nojekyll
--rw-r--r--   0        0        0      634 2024-04-30 20:33:48.759168 reasoner_validator-4.1.1/docs/Makefile
--rw-r--r--   0        0        0     2291 2024-04-30 20:33:48.759168 reasoner_validator-4.1.1/docs/conf.py
--rw-r--r--   0        0        0    20365 2024-04-30 20:33:48.759168 reasoner_validator-4.1.1/docs/index.rst
--rw-r--r--   0        0        0      795 2024-04-30 20:33:48.759168 reasoner_validator-4.1.1/docs/make.bat
--rw-r--r--   0        0        0      136 2024-04-30 20:33:48.759168 reasoner_validator-4.1.1/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2024-04-30 20:33:48.759168 reasoner_validator-4.1.1/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      152 2024-04-30 20:33:48.759168 reasoner_validator-4.1.1/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2024-04-30 20:33:48.759168 reasoner_validator-4.1.1/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2024-04-30 20:33:48.759168 reasoner_validator-4.1.1/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2024-04-30 20:33:48.759168 reasoner_validator-4.1.1/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2024-04-30 20:33:48.759168 reasoner_validator-4.1.1/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    42104 2024-04-30 20:33:48.759168 reasoner_validator-4.1.1/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2298 2024-04-30 20:33:48.759168 reasoner_validator-4.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-30 20:33:48.759168 reasoner_validator-4.1.1/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    94021 2024-04-30 20:33:48.763168 reasoner_validator-4.1.1/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    45890 2024-04-30 20:33:48.763168 reasoner_validator-4.1.1/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0     1761 2024-04-30 20:33:48.763168 reasoner_validator-4.1.1/reasoner_validator/github.py
--rw-r--r--   0        0        0     3973 2024-04-30 20:33:48.763168 reasoner_validator-4.1.1/reasoner_validator/message.py
--rw-r--r--   0        0        0    46755 2024-04-30 20:33:48.763168 reasoner_validator-4.1.1/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2024-04-30 20:33:48.763168 reasoner_validator-4.1.1/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4754 2024-04-30 20:33:48.763168 reasoner_validator-4.1.1/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0    15057 2024-04-30 20:33:48.763168 reasoner_validator-4.1.1/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1120 2024-04-30 20:33:48.763168 reasoner_validator-4.1.1/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    14745 2024-04-30 20:33:48.763168 reasoner_validator-4.1.1/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0    35576 2024-04-30 20:33:48.763168 reasoner_validator-4.1.1/reasoner_validator/validator.py
--rw-r--r--   0        0        0    12127 2024-04-30 20:33:48.763168 reasoner_validator-4.1.1/reasoner_validator/versioning.py
--rw-r--r--   0        0        0      866 2024-04-30 20:33:48.763168 reasoner_validator-4.1.1/reasoner_validator/versions.yaml
--rw-r--r--   0        0        0     3601 2024-04-30 20:33:48.763168 reasoner_validator-4.1.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 20:33:48.763168 reasoner_validator-4.1.1/tests/conftest.py
--rw-r--r--   0        0        0   145466 2024-04-30 20:33:48.763168 reasoner_validator-4.1.1/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    62107 2024-04-30 20:33:48.763168 reasoner_validator-4.1.1/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
--rw-r--r--   0        0        0    41308 2024-04-30 20:33:48.763168 reasoner_validator-4.1.1/tests/test_response_validator.py
--rw-r--r--   0        0        0     6157 2024-04-30 20:33:48.763168 reasoner_validator-4.1.1/tests/test_semver.py
--rw-r--r--   0        0        0     2248 2024-04-30 20:33:48.763168 reasoner_validator-4.1.1/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    36620 2024-04-30 20:33:48.763168 reasoner_validator-4.1.1/tests/test_validate.py
--rw-r--r--   0        0        0    30223 2024-04-30 20:33:48.767168 reasoner_validator-4.1.1/tests/test_validation_report.py
--rw-r--r--   0        0        0     3411 2024-04-30 20:33:48.767168 reasoner_validator-4.1.1/tests/test_workflows.py
--rw-r--r--   0        0        0    15315 1970-01-01 00:00:00.000000 reasoner_validator-4.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1153 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/LICENSE
+-rw-r--r--   0        0        0    13727 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/README.md
+-rw-r--r--   0        0        0      131 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/docs/Makefile
+-rw-r--r--   0        0        0     2291 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/docs/conf.py
+-rw-r--r--   0        0        0    20564 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/docs/index.rst
+-rw-r--r--   0        0        0      795 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/docs/make.bat
+-rw-r--r--   0        0        0      136 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      152 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    42104 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2298 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-01 05:39:56.315559 reasoner_validator-4.1.2/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    94288 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    45890 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0     1761 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/reasoner_validator/github.py
+-rw-r--r--   0        0        0     3973 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/reasoner_validator/message.py
+-rw-r--r--   0        0        0    46755 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4754 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0    15057 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1120 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    14745 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0    35576 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/reasoner_validator/validator.py
+-rw-r--r--   0        0        0    12127 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0      866 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/reasoner_validator/versions.yaml
+-rw-r--r--   0        0        0     3601 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/tests/conftest.py
+-rw-r--r--   0        0        0   145790 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    62107 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
+-rw-r--r--   0        0        0    41308 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/tests/test_response_validator.py
+-rw-r--r--   0        0        0     6157 2024-05-01 05:39:56.319559 reasoner_validator-4.1.2/tests/test_semver.py
+-rw-r--r--   0        0        0     2248 2024-05-01 05:39:56.323559 reasoner_validator-4.1.2/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    36620 2024-05-01 05:39:56.323559 reasoner_validator-4.1.2/tests/test_validate.py
+-rw-r--r--   0        0        0    30223 2024-05-01 05:39:56.323559 reasoner_validator-4.1.2/tests/test_validation_report.py
+-rw-r--r--   0        0        0     3411 2024-05-01 05:39:56.323559 reasoner_validator-4.1.2/tests/test_workflows.py
+-rw-r--r--   0        0        0    15315 1970-01-01 00:00:00.000000 reasoner_validator-4.1.2/PKG-INFO
```

### Comparing `reasoner_validator-4.1.1/LICENSE` & `reasoner_validator-4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.1/README.md` & `reasoner_validator-4.1.2/README.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.1/docs/Makefile` & `reasoner_validator-4.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.1/docs/conf.py` & `reasoner_validator-4.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.1/docs/index.rst` & `reasoner_validator-4.1.2/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 
 Checkout then setup dependencies and the standard virtual environment using poetry, as follows:
 
 .. code-block:: bash
 
     git checkout https://github.com/NCATSTranslator/reasoner-validator.git
     cd reasoner-validator
-    poetry install
     poetry shell
+    poetry install
 
 These operations install the software and creates a virtual operation for running the software in a simple fashion.
 
 You can optionally, `use a tool like pyenv to set your local shell Python version to a 3.9 release <https://python-poetry.org/docs/managing-environments/>`_  prior to the poetry installation.
 
 Basic Programmatic Usage
 ========================
@@ -46,15 +46,15 @@
 Top level programmatic validation of a TRAPI Response uses a TRAPIResponseValidator class wrapper as follows (sample script):
 
 .. code-block:: python
 
     #!/usr/bin/env python
     from typing import Optional, List, Dict
     from reasoner_validator.validator import TRAPIResponseValidator
-    from reasoner_validator import MESSAGE_CATALOG
+    from reasoner_validator import MESSAGES_BY_TARGET
 
     SAMPLE_RESPONSE = {
       "message": {
         "query_graph": {
             "nodes": {
                 "type-2 diabetes": {"ids": ["MONDO:0005148"]},
                 "drug": {"categories": ["biolink:Drug"]}
@@ -82,20 +82,20 @@
                     "treats": [{"id": "df87ff82"}]
                 }
             }
         ]
     }
 
     }
-    validator = TRAPIResponseValidator(
-        trapi_version="1.4.2",
+    validator: TRAPIResponseValidator = TRAPIResponseValidator(
+        trapi_version="1.5.0",
 
         # If omit or set the Biolink Model version parameter to None,
         # then the current Biolink Model Toolkit default release applies
-        biolink_version="3.5.0",
+        biolink_version="4.2.0",
 
         # 'sources' are set to trigger checking of expected edge knowledge source provenance
         sources={
                 "ara_source": "infores:molepro",
                 "kp_source": "infores:hmdb",
                 "kp_source_type": "primary"
         },
@@ -110,15 +110,15 @@
     # TRAPI.Message JSON schema model component of the TRAPI Response (not the full TRAPI Response...yet)
 
     # this method validates a complete TRAPI Response JSON result
     validator.check_compliance_of_trapi_response(response=SAMPLE_RESPONSE)
 
     if validator.has_messages():
         # Raw message data is retrieved from the validator object as follows:
-        messages: MESSAGE_CATALOG = validator.get_messages()
+        messages: MESSAGES_BY_TARGET = validator.get_all_messages()
 
         # this method dumps a human readable text report of
         # the validation messages (default) to stdout
         # See the method signature for options that
         # allow customization of the text format.
         validator.dump()
 
@@ -250,25 +250,25 @@
         "_comment": "If the TRAPI version is omitted or set to None, then the 'latest' TRAPI version is used.
 
         # Note: for TRAPI releases from 1.4.0 onwards, the Response message will state the assumed 'schema_version'.
         # This modifies slightly the interpretation of this parameter, as follows:
         # If the following trapi_version parameter is given, then it overrides the TRAPI Response 'schema_version';
         # Otherwise, a TRAPI 1.4.0 Response embedded 'schema_version' (not 'latest') becomes the default validation version."
 
-        "trapi_version": "1.4.2",
+        "trapi_version": "1.5.0",
 
         "_comment": "If the Biolink Model version is omitted or set to None, then the current Biolink Model Toolkit is used.
 
         # Note: for TRAPI releases from 1.4.0 onwards, the Response message will state the assumed 'biolink_version'.
         # This modifies slightly the interpretation of this parameter, as follows:
         # If the 'biolink_version' given here is assumed, which overrides the TRAPI Response stated 'biolink_version';
-        # Otherwise, a TRAPI 1.4.0 Response embedded 'biolink_version' (not BMT) becomes the default validation version.
+        # Otherwise, a TRAPI 1.5.0 Response embedded 'biolink_version' (not BMT) becomes the default validation version.
         # The biolink_version may also be set to the string 'suppress', in which case, most Biolink Model validation is NOT done during the validation of a TRAPI Response."
 
-        "biolink_version": "3.5.0",
+        "biolink_version": "4.2.0",
 
         "sources": {
             "ara_source": "infores:aragorn",
             "kp_source": "infores:panther",
             "kp_source_type": "primary"
         },
         "strict_validation": true,
@@ -306,16 +306,16 @@
 --------------
 
 As an example of the kind of output to expect, if one posts the following TRAPI Response JSON data as input to the **/validate** endpoint:
 
 .. code-block:: json
 
     {
-        "schema_version": "1.4.2",
-        "biolink_version": "3.5.0",
+        "schema_version": "1.5.0",
+        "biolink_version": "4.2.0",
         "message": {
             "query_graph": {
                 "nodes": {
                     "type-2 diabetes": {"ids": ["MONDO:0005148"]},
                     "drug": {"categories": ["biolink:Drug"]}
                 },
                 "edges": {
@@ -370,16 +370,16 @@
     }
 
 then, one should typically get a response body like the following JSON validation result back:
 
 .. code-block:: json
 
     {
-      "trapi_version": "1.4.2",
-      "biolink_version": "3.5.0",
+      "trapi_version": "1.5.0",
+      "biolink_version": "4.2.0",
       "messages": {
         "critical": {},
         "errors": {
           "error.knowledge_graph.node.category.missing": {
              "infores:chebi -> infores:molepro -> infores:arax": {
                 "MONDO:0005148": [
                   {
@@ -455,14 +455,16 @@
 The Reasoner Validator package is evolving along with progress in TRAPI and Biolink standards within the NCATS Biomedical Knowledge Translator. This documentation pertains to the 3.* releases of the package. A synopsis of the evolution of the package is:
 
 * 1.# releases - very preliminary releases of the validation code, now obsolete
 * 2.# releases - had a base TRAPI schema 'validate' with errors throwing a Python exception; later minor iterations added in Biolink Model validation returning a flat dictionary of arcane string messages
 * 3.0.# releases
   - wrapped the all validation with a ValidatorReporter class serving to collect and return validation messages in a disciplined, codified manner (as a [master YAML file with hierarchically-indexed Python string templates](reasoner_validator/codes.yaml)). Generally still reliably validates Biolink Model release <= 2.4.8
 * 3.1.# releases: mainly supports Biolink Model releases >= 3.0.* and will likely generate some spurious validation warnings or errors for Biolink Model release <= 2.4.8 (reflects non-backward compatible changes to the Biolink Model Toolkit)
+* 4.0.# restructured output messages indexing by target (endpoint url) and indexing by test identifier;
+# 4.1.# TRAPI 1.5 and Biolink Model 4.2.0 validation support
 
 The `full change log is here <https://github.com/NCATSTranslator/reasoner-validator/blob/master/CHANGELOG.md>`_.
 
 Community
 =========
 
 See `project README for full details <https://github.com/NCATSTranslator/reasoner-validator/blob/master/README.md>`_
```

### Comparing `reasoner_validator-4.1.1/docs/make.bat` & `reasoner_validator-4.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.1/docs/validation_codes_dictionary.md` & `reasoner_validator-4.1.2/docs/validation_codes_dictionary.md`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.1/pyproject.toml` & `reasoner_validator-4.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "4.1.1"
+version = "4.1.2"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
```

### Comparing `reasoner_validator-4.1.1/reasoner_validator/biolink/__init__.py` & `reasoner_validator-4.1.2/reasoner_validator/biolink/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -683,20 +683,25 @@
         :param edge_id: str, identifier of the edge being validated
         :param found: bool, current status of slot detection, True if already seen previously (return 'True' value here)
         :param value: Optional[str], the value to be validated
         :return: None (validation messages recorded in the BiolinkValidator)
         """
         return self.validate_slot_value(slot_name="agent_type", context=edge_id, found=found, value=value)
 
-    # 13-July-2023: Certain attribute_type_id's are slated for future implementation in the Biolink Model
-    #               but not in the current model release; however, some teams have started to use the terms.
-    #               We therefore put them on a special "inclusion list" (like the CATEGORY_INCLUSIONS below)
-    #               to permit them to pass through the validation without any complaints.
-    # ATTRIBUTE_TYPE_ID_INCLUSIONS = ["biolink:knowledge_level", "biolink:agent_type"]
-    ATTRIBUTE_TYPE_ID_INCLUSIONS = []
+    def get_attribute_type_exclusions(self) -> List[str]:
+        if self.minimum_required_biolink_version("4.2.0"):
+            return list()
+        else:
+            # 13-July-2023: Certain attribute_type_id's are slated for future implementation in the Biolink Model
+            #               but not in the current model release; however, some teams have started to use the terms.
+            #               We therefore put them on a special "inclusion list" (like the CATEGORY_INCLUSIONS below)
+            #               to permit them to pass through the validation without any complaints.
+            # Still not defined in Biolink releases prior to "4.2.0'
+            # but sometimes implemented: ignore in validation
+            return ["biolink:knowledge_level", "biolink:agent_type"]
 
     def validate_attributes(
             self,
             graph_type: TRAPIGraphType,
             edge_id: str,
             edge: Dict,
             source_trail: Optional[str] = None
@@ -832,15 +837,15 @@
                                 )
                             elif self.validate_biolink():
                                 # 'attribute_type_id' is a CURIE, but how well does it map?
                                 prefix = attribute_type_id.split(":", 1)[0]
                                 if prefix == 'biolink':
                                     # We will skip further validation of terms
                                     # in the ATTRIBUTE_TYPE_ID_INCLUSIONS list...
-                                    if attribute_type_id not in self.ATTRIBUTE_TYPE_ID_INCLUSIONS:
+                                    if attribute_type_id not in self.get_attribute_type_exclusions():
 
                                         # ... but further validate everything else...
                                         biolink_class = self.validate_element_status(
                                             graph_type=graph_type,
                                             context="knowledge_graph.edge.attribute.type_id",
                                             identifier=attribute_type_id,
                                             edge_id=edge_id,
```

### Comparing `reasoner_validator-4.1.1/reasoner_validator/codes.yaml` & `reasoner_validator-4.1.2/reasoner_validator/codes.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.1/reasoner_validator/github.py` & `reasoner_validator-4.1.2/reasoner_validator/github.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.1/reasoner_validator/message.py` & `reasoner_validator-4.1.2/reasoner_validator/message.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.1/reasoner_validator/report.py` & `reasoner_validator-4.1.2/reasoner_validator/report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.1/reasoner_validator/sri/util.py` & `reasoner_validator-4.1.2/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.1/reasoner_validator/trapi/__init__.py` & `reasoner_validator-4.1.2/reasoner_validator/trapi/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.1/reasoner_validator/trapi/mapping.py` & `reasoner_validator-4.1.2/reasoner_validator/trapi/mapping.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.1/reasoner_validator/validation_codes.py` & `reasoner_validator-4.1.2/reasoner_validator/validation_codes.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.1/reasoner_validator/validator.py` & `reasoner_validator-4.1.2/reasoner_validator/validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.1/reasoner_validator/versioning.py` & `reasoner_validator-4.1.2/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.1/reasoner_validator/versions.yaml` & `reasoner_validator-4.1.2/reasoner_validator/versions.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.1/tests/__init__.py` & `reasoner_validator-4.1.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.1/tests/test_biolink_compliance_validation.py` & `reasoner_validator-4.1.2/tests/test_biolink_compliance_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -3595,14 +3595,26 @@
                            "attribute_type_id": "biolink:agent_type",
                            "value": "not-an-agent-type"
                         }
                     ]
                 )
             },
             "error.knowledge_graph.edge.agent_type.invalid"
+        ),
+(
+            "4.1.6",
+
+            # Query 42: Sample full valid TRAPI Knowledge Graph
+            {
+                # Sample nodes
+                'nodes': SAMPLE_NODES_WITH_ATTRIBUTES,
+                # Sample edge
+                'edges': SAMPLE_EDGE_WITH_ATTRIBUTES_AND_SOURCES
+            },
+            ""
         )
     ]
 )
 def test_check_biolink_model_compliance_of_knowledge_graph(
         biolink_version: str,
         graph_data: Dict,
         code: str
```

### Comparing `reasoner_validator-4.1.1/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml` & `reasoner_validator-4.1.2/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.1/tests/test_response_validator.py` & `reasoner_validator-4.1.2/tests/test_response_validator.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.1/tests/test_semver.py` & `reasoner_validator-4.1.2/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.1/tests/test_trapi_versioning.py` & `reasoner_validator-4.1.2/tests/test_trapi_versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.1/tests/test_validate.py` & `reasoner_validator-4.1.2/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.1/tests/test_validation_report.py` & `reasoner_validator-4.1.2/tests/test_validation_report.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.1/tests/test_workflows.py` & `reasoner_validator-4.1.2/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-4.1.1/PKG-INFO` & `reasoner_validator-4.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 4.1.1
+Version: 4.1.2
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
```


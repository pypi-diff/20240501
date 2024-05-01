# Comparing `tmp/airbyte_source_monday-2.1.1.tar.gz` & `tmp/airbyte_source_monday-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_monday-2.1.1.tar", max compression
+gzip compressed data, was "airbyte_source_monday-2.1.2.tar", max compression
```

## Comparing `airbyte_source_monday-2.1.1.tar` & `airbyte_source_monday-2.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     4496 2024-04-08 10:22:07.860112 airbyte_source_monday-2.1.1/README.md
--rw-r--r--   0        0        0      739 2024-04-08 10:24:48.511521 airbyte_source_monday-2.1.1/pyproject.toml
--rw-r--r--   0        0        0      203 2024-04-08 10:22:07.860112 airbyte_source_monday-2.1.1/source_monday/__init__.py
--rw-r--r--   0        0        0    10241 2024-04-08 10:22:07.860112 airbyte_source_monday-2.1.1/source_monday/components.py
--rw-r--r--   0        0        0     4839 2024-04-08 10:22:07.860112 airbyte_source_monday-2.1.1/source_monday/extractor.py
--rw-r--r--   0        0        0    11056 2024-04-08 10:22:07.860112 airbyte_source_monday-2.1.1/source_monday/graphql_requester.py
--rw-r--r--   0        0        0     4401 2024-04-08 10:22:07.860112 airbyte_source_monday-2.1.1/source_monday/item_pagination_strategy.py
--rw-r--r--   0        0        0     6843 2024-04-08 10:22:07.860112 airbyte_source_monday-2.1.1/source_monday/manifest.yaml
--rw-r--r--   0        0        0      230 2024-04-08 10:22:07.860112 airbyte_source_monday-2.1.1/source_monday/run.py
--rw-r--r--   0        0        0      481 2024-04-08 10:22:07.860112 airbyte_source_monday-2.1.1/source_monday/schemas/activity_logs.json
--rw-r--r--   0        0        0     3633 2024-04-08 10:22:07.860112 airbyte_source_monday-2.1.1/source_monday/schemas/boards.json
--rw-r--r--   0        0        0     2694 2024-04-08 10:22:07.860112 airbyte_source_monday-2.1.1/source_monday/schemas/items.json
--rw-r--r--   0        0        0      232 2024-04-08 10:22:07.860112 airbyte_source_monday-2.1.1/source_monday/schemas/tags.json
--rw-r--r--   0        0        0      474 2024-04-08 10:22:07.860112 airbyte_source_monday-2.1.1/source_monday/schemas/teams.json
--rw-r--r--   0        0        0     1916 2024-04-08 10:22:07.860112 airbyte_source_monday-2.1.1/source_monday/schemas/updates.json
--rw-r--r--   0        0        0     1408 2024-04-08 10:22:07.860112 airbyte_source_monday-2.1.1/source_monday/schemas/users.json
--rw-r--r--   0        0        0     1982 2024-04-08 10:22:07.860112 airbyte_source_monday-2.1.1/source_monday/schemas/workspaces.json
--rw-r--r--   0        0        0      474 2024-04-08 10:22:07.860112 airbyte_source_monday-2.1.1/source_monday/source.py
--rw-r--r--   0        0        0     3989 2024-04-08 10:22:07.860112 airbyte_source_monday-2.1.1/source_monday/spec.json
--rw-r--r--   0        0        0     5198 1970-01-01 00:00:00.000000 airbyte_source_monday-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4496 2024-05-01 17:36:40.425745 airbyte_source_monday-2.1.2/README.md
+-rw-r--r--   0        0        0      739 2024-05-01 17:40:00.229242 airbyte_source_monday-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0      203 2024-05-01 17:36:40.429745 airbyte_source_monday-2.1.2/source_monday/__init__.py
+-rw-r--r--   0        0        0    10241 2024-05-01 17:36:40.429745 airbyte_source_monday-2.1.2/source_monday/components.py
+-rw-r--r--   0        0        0     5036 2024-05-01 17:36:40.429745 airbyte_source_monday-2.1.2/source_monday/extractor.py
+-rw-r--r--   0        0        0    10219 2024-05-01 17:36:40.429745 airbyte_source_monday-2.1.2/source_monday/graphql_requester.py
+-rw-r--r--   0        0        0     4401 2024-05-01 17:36:40.429745 airbyte_source_monday-2.1.2/source_monday/item_pagination_strategy.py
+-rw-r--r--   0        0        0     6843 2024-05-01 17:36:40.429745 airbyte_source_monday-2.1.2/source_monday/manifest.yaml
+-rw-r--r--   0        0        0      230 2024-05-01 17:36:40.429745 airbyte_source_monday-2.1.2/source_monday/run.py
+-rw-r--r--   0        0        0      481 2024-05-01 17:36:40.429745 airbyte_source_monday-2.1.2/source_monday/schemas/activity_logs.json
+-rw-r--r--   0        0        0     3633 2024-05-01 17:36:40.429745 airbyte_source_monday-2.1.2/source_monday/schemas/boards.json
+-rw-r--r--   0        0        0     2694 2024-05-01 17:36:40.429745 airbyte_source_monday-2.1.2/source_monday/schemas/items.json
+-rw-r--r--   0        0        0      232 2024-05-01 17:36:40.429745 airbyte_source_monday-2.1.2/source_monday/schemas/tags.json
+-rw-r--r--   0        0        0      474 2024-05-01 17:36:40.429745 airbyte_source_monday-2.1.2/source_monday/schemas/teams.json
+-rw-r--r--   0        0        0     1916 2024-05-01 17:36:40.429745 airbyte_source_monday-2.1.2/source_monday/schemas/updates.json
+-rw-r--r--   0        0        0     1408 2024-05-01 17:36:40.429745 airbyte_source_monday-2.1.2/source_monday/schemas/users.json
+-rw-r--r--   0        0        0     1982 2024-05-01 17:36:40.429745 airbyte_source_monday-2.1.2/source_monday/schemas/workspaces.json
+-rw-r--r--   0        0        0      474 2024-05-01 17:36:40.429745 airbyte_source_monday-2.1.2/source_monday/source.py
+-rw-r--r--   0        0        0     3989 2024-05-01 17:36:40.429745 airbyte_source_monday-2.1.2/source_monday/spec.json
+-rw-r--r--   0        0        0     5198 1970-01-01 00:00:00.000000 airbyte_source_monday-2.1.2/PKG-INFO
```

### Comparing `airbyte_source_monday-2.1.1/README.md` & `airbyte_source_monday-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_monday-2.1.1/pyproject.toml` & `airbyte_source_monday-2.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.1.1"
+version = "2.1.2"
 name = "airbyte-source-monday"
 description = "Source implementation for Monday."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_monday-2.1.1/source_monday/components.py` & `airbyte_source_monday-2.1.2/source_monday/components.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_monday-2.1.1/source_monday/extractor.py` & `airbyte_source_monday-2.1.2/source_monday/extractor.py`

 * *Files 7% similar despite different names*

```diff
@@ -101,13 +101,18 @@
     def extract_records(self, response: requests.Response) -> List[Record]:
         result = self.try_extract_records(response, field_path=self.field_path)
         if not result and self.field_path_pagination:
             result = self.try_extract_records(response, self.field_path_pagination)
         if not result and self.field_path_incremental:
             result = self.try_extract_records(response, self.field_path_incremental)
 
-        for item_index in range(len(result)):
-            if "updated_at" in result[item_index]:
-                result[item_index]["updated_at_int"] = int(
-                    datetime.strptime(result[item_index]["updated_at"], "%Y-%m-%dT%H:%M:%S%z").timestamp()
-                )
+        for record in result:
+            if "updated_at" in record:
+                record["updated_at_int"] = int(datetime.strptime(record["updated_at"], "%Y-%m-%dT%H:%M:%S%z").timestamp())
+
+            column_values = record.get("column_values", [])
+            for values in column_values:
+                display_value, text = values.get("display_value"), values.get("text")
+                if display_value and not text:
+                    values["text"] = display_value
+
         return result
```

### Comparing `airbyte_source_monday-2.1.1/source_monday/graphql_requester.py` & `airbyte_source_monday-2.1.2/source_monday/graphql_requester.py`

 * *Files 7% similar despite different names*

```diff
@@ -73,37 +73,22 @@
                 # fields.append(self._build_query(field, nested_fields, **preconfigured_arguments))
                 fields.append(self._build_query(field, nested_fields))
             else:
                 fields.append(field)
 
         arguments = self._get_object_arguments(**object_arguments)
         arguments = f"({arguments})" if arguments else ""
-        fields = ",".join(fields)
 
-        # Essentially, we construct a query based on schema properties; however, some fields in the schema are conditional.
-        # These conditional fields can be obtained by defining them as inline fragments (The docs: https://spec.graphql.org/October2021/#sec-Inline-Fragments).
-        # This is an example of a query built for the Items stream, with a `display_value` property defined as an `MirrorValue` inline fragment:
-        # query {
-        #   boards (limit:1) {
-        #     items_page (limit:20) {
-        #       <a field>,
-        #       ...,
-        #       column_values {
-        #         id,
-        #         text,
-        #         type,
-        #         value,
-        #         ... on MirrorValue {display_value}
-        #       }
-        #     }
-        #   }
-        # }
-        # When constructing a query, we replace the `display_value` field with the `... on MirrorValue {display_value}` inline fragment.
-        if object_name == "column_values" and "display_value" in fields:
-            fields = fields.replace("display_value", "... on MirrorValue{display_value}")
+        if object_name == "column_values":
+            fields.remove("display_value")
+            fields.extend(
+                ["... on MirrorValue{display_value}", "... on BoardRelationValue{display_value}", "... on DependencyValue{display_value}"]
+            )
+
+        fields = ",".join(fields)
 
         if object_name in ["items_page", "next_items_page"]:
             query = f"{object_name}{arguments}{{cursor,items{{{fields}}}}}"
         else:
             query = f"{object_name}{arguments}{{{fields}}}"
         return query
```

### Comparing `airbyte_source_monday-2.1.1/source_monday/item_pagination_strategy.py` & `airbyte_source_monday-2.1.2/source_monday/item_pagination_strategy.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_monday-2.1.1/source_monday/manifest.yaml` & `airbyte_source_monday-2.1.2/source_monday/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_monday-2.1.1/source_monday/schemas/boards.json` & `airbyte_source_monday-2.1.2/source_monday/schemas/boards.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_monday-2.1.1/source_monday/schemas/items.json` & `airbyte_source_monday-2.1.2/source_monday/schemas/items.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_monday-2.1.1/source_monday/schemas/updates.json` & `airbyte_source_monday-2.1.2/source_monday/schemas/updates.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_monday-2.1.1/source_monday/schemas/users.json` & `airbyte_source_monday-2.1.2/source_monday/schemas/users.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_monday-2.1.1/source_monday/schemas/workspaces.json` & `airbyte_source_monday-2.1.2/source_monday/schemas/workspaces.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_monday-2.1.1/source_monday/spec.json` & `airbyte_source_monday-2.1.2/source_monday/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_monday-2.1.1/PKG-INFO` & `airbyte_source_monday-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-monday
-Version: 2.1.1
+Version: 2.1.2
 Summary: Source implementation for Monday.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```


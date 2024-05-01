# Comparing `tmp/odd_great_expectations-0.1.9.tar.gz` & `tmp/odd_great_expectations-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odd_great_expectations-0.1.9.tar", max compression
+gzip compressed data, was "odd_great_expectations-0.2.0.tar", max compression
```

## Comparing `odd_great_expectations-0.1.9.tar` & `odd_great_expectations-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-02-08 21:09:18.000000 odd_great_expectations-0.1.9/LICENSE
--rw-r--r--   0        0        0     1583 2023-02-08 21:09:18.000000 odd_great_expectations-0.1.9/README.md
--rw-r--r--   0        0        0        0 2023-02-08 21:09:18.000000 odd_great_expectations-0.1.9/odd_great_expectations/__init__.py
--rw-r--r--   0        0        0     2675 2023-02-08 21:09:18.000000 odd_great_expectations-0.1.9/odd_great_expectations/action.py
--rw-r--r--   0        0        0     2102 2023-02-08 21:09:18.000000 odd_great_expectations-0.1.9/odd_great_expectations/client.py
--rw-r--r--   0        0        0       80 2023-02-08 21:09:18.000000 odd_great_expectations-0.1.9/odd_great_expectations/dataset/__init__.py
--rw-r--r--   0        0        0      698 2023-02-08 21:09:18.000000 odd_great_expectations-0.1.9/odd_great_expectations/dataset/file.py
--rw-r--r--   0        0        0      769 2023-02-08 21:09:18.000000 odd_great_expectations-0.1.9/odd_great_expectations/dataset/get_dataset.py
--rw-r--r--   0        0        0     1726 2023-02-08 21:09:18.000000 odd_great_expectations-0.1.9/odd_great_expectations/dataset/sql_table.py
--rw-r--r--   0        0        0      565 2023-02-08 21:09:18.000000 odd_great_expectations-0.1.9/odd_great_expectations/errors.py
--rw-r--r--   0        0        0     4622 2023-02-08 21:09:18.000000 odd_great_expectations-0.1.9/odd_great_expectations/mapper.py
--rw-r--r--   0        0        0      747 2023-02-08 21:09:37.000000 odd_great_expectations-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     2513 1970-01-01 00:00:00.000000 odd_great_expectations-0.1.9/setup.py
--rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 odd_great_expectations-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-01 12:30:00.424308 odd_great_expectations-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1800 2024-05-01 12:30:00.424308 odd_great_expectations-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-01 12:30:00.428308 odd_great_expectations-0.2.0/odd_great_expectations/__init__.py
+-rw-r--r--   0        0        0     2994 2024-05-01 12:30:00.428308 odd_great_expectations-0.2.0/odd_great_expectations/action.py
+-rw-r--r--   0        0        0       80 2024-05-01 12:30:00.428308 odd_great_expectations-0.2.0/odd_great_expectations/dataset/__init__.py
+-rw-r--r--   0        0        0      786 2024-05-01 12:30:00.428308 odd_great_expectations-0.2.0/odd_great_expectations/dataset/file.py
+-rw-r--r--   0        0        0      721 2024-05-01 12:30:00.428308 odd_great_expectations-0.2.0/odd_great_expectations/dataset/get_dataset.py
+-rw-r--r--   0        0        0     2310 2024-05-01 12:30:00.428308 odd_great_expectations-0.2.0/odd_great_expectations/dataset/sql_table.py
+-rw-r--r--   0        0        0      460 2024-05-01 12:30:00.428308 odd_great_expectations-0.2.0/odd_great_expectations/logger.py
+-rw-r--r--   0        0        0     4521 2024-05-01 12:30:00.428308 odd_great_expectations-0.2.0/odd_great_expectations/mapper.py
+-rw-r--r--   0        0        0      777 2024-05-01 12:30:13.024219 odd_great_expectations-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2732 1970-01-01 00:00:00.000000 odd_great_expectations-0.2.0/setup.py
+-rw-r--r--   0        0        0     2725 1970-01-01 00:00:00.000000 odd_great_expectations-0.2.0/PKG-INFO
```

### Comparing `odd_great_expectations-0.1.9/LICENSE` & `odd_great_expectations-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `odd_great_expectations-0.1.9/README.md` & `odd_great_expectations-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,55 @@
-## OpenDataDiscovery Great Expectations metadata collecting.
-[![PyPI version](https://badge.fury.io/py/odd-great-expectations.svg)](https://badge.fury.io/py/odd-great-expectations)
+## OpenDataDiscovery Action for handling Great Expectations tests results.
 
-## Supporting
-| Feature                     | Supporting |
-| --------------------------- | ---------- |
-| V3 API +                    | +          |
-| SqlAlchemyEngine            | +          |
-| PandasEngine                | +          |
-| Great Expectations V2 API - | -          |
-| Cloud Solution              | -          |
+[![PyPI version](https://badge.fury.io/py/odd-great-expectations.svg)](https://badge.fury.io/py/odd-great-expectations)
 
+![image](assets/screenshot.png)
 
+# What is it?
 `odd_great_expectation.action.ODDAction`
-Is a class derived from `ValidationAction` and can be used in checkpoint actions lists.
+Is a class derived from GX `ValidationAction` which will be run by GreatExpectations at runtime with `ValidationResult`s for checkpoint.
 
-## How to:
 
-### Install odd-great-expectations package
+# How to use it?:
+Install `odd-great-expectations` package
 ```bash
 pip install odd-great-expectations
 ```
-
-### Add action to checkpoint:
+Add `ODDAction` action to some checkpoint's action list:
 ```yaml
 name: <CHECKPOINT_NAME>
 config_version: 1.0
-template_name:
-module_name: great_expectations.checkpoint
-class_name: Checkpoint
-run_name_template: '%Y%m%d-%H%M%S-my-run-name-template'
-expectation_suite_name:
-batch_request: {}
+...
 action_list:
   # other actions
-  - name: store_metadata_to_odd 
+  - name: store_metadata_to_odd
     action:
       module_name: odd_great_expectations.action
       class_name: ODDAction
-      platform_host: <PLATFORM_HOST> # OpenDataDiscovery platform, i.e. http://localhost:8080
-      platform_token: <PLATFORM_TOKEN> # OpenDataDiscovery token
-      data_source_name: <DATA_SOURCE_NAME> # Unique name for data source, i.e. local_qa_test
-evaluation_parameters: {}
+      platform_host: <PLATFORM_HOST>
+      data_source_name: <DATA_SOURCE_NAME>
 ```
 
-### Run checkpoint
+Parameters:
+
+`platform_host` - Location of OpenDataDiscovery platform, i.e. http://localhost:8080
+
+`platform_token` - OpenDataDiscovery token, how to get it - https://docs.opendatadiscovery.org/configuration-and-deployment/trylocally#create-collector-entity
+
+`data_source_name` - Unique name for data source, i.e. local_qa_test
+
+Both `platform_host` and `platform_token`  can be set using `ODD_PLATFORM_HOST` and `ODD_PLATFORM_PLATFORM` env variables accordingly.
+
+Run checkpoint
 ```bash
-great_expectations checkpoint run <CHECKPOINT_NAME> 
+great_expectations checkpoint run <CHECKPOINT_NAME>
 ```
-### Check result
-Check results on <PLATFORM_HOST> UI.
-
+Check results on `PLATFORM_HOST` UI.
 
+## Supporting features
+| Feature                     | Supporting |
+| --------------------------- | ---------- |
+| V3 API +                    | +          |
+| SqlAlchemyEngine            | +          |
+| PandasEngine                | +          |
+| Great Expectations V2 API - | -          |
+| Cloud Solution              | -          |
```

### Comparing `odd_great_expectations-0.1.9/odd_great_expectations/action.py` & `odd_great_expectations-0.2.0/odd_great_expectations/action.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,78 +1,84 @@
-from typing import Any, Union
+import traceback
+from typing import Union, Optional
 
 from great_expectations.checkpoint.actions import (
     ExpectationSuiteValidationResult,
     GXCloudIdentifier,
     ValidationAction,
     ValidationResultIdentifier,
 )
 from great_expectations.validator.validator import Validator
-from loguru import logger
 from oddrn_generator.generators import GreatExpectationsGenerator
 
-from odd_great_expectations.client import Client
+from odd_models.api_client.v2.odd_api_client import Client
 from odd_great_expectations.dataset.get_dataset import get_datasets
+from odd_great_expectations.logger import logger
 from odd_great_expectations.mapper import MapValidationResult
 
 
 class ODDAction(ValidationAction):
     def __init__(
         self,
         data_context,
         data_source_name: str,
         platform_host: str = None,
         platform_token: str = None,
     ):
+        super().__init__(data_context)
+
         self._odd_client = Client(platform_host, platform_token)
         self._data_source_name = data_source_name
-        self._host = "local"
-
-        super().__init__(data_context)
 
     def _run(
         self,
         validation_result_suite: ExpectationSuiteValidationResult,
         validation_result_suite_identifier: Union[
             ValidationResultIdentifier, GXCloudIdentifier
         ],
-        data_asset: Union[Validator, Any],
+        data_asset: Validator,
         expectation_suite_identifier=None,
         checkpoint_identifier=None,
-        payload=None,
+        **kwargs,
     ):
         try:
-            logger.info("Start collecting metadata")
             client = self._odd_client
+
             expectation_suite = data_asset.expectation_suite
             suite_name = expectation_suite.expectation_suite_name
             generator = GreatExpectationsGenerator(
-                host_settings=self._host, suites=suite_name
+                host_settings="local", suites=suite_name
             )
-
-            docs_link = None
-            if payload:
-                if data_docs := payload.get("update_data_docs"):
-                    docs_link = data_docs.get("local_site")
-
-            client.ingest_data_source(
+            client.create_data_source(
                 data_source_oddrn=generator.get_data_source_oddrn(),
-                name=self._data_source_name,
+                data_source_name=self._data_source_name,
             )
 
-            datasets = get_datasets(data_asset.execution_engine)
+            datasets: list[str] = get_datasets(data_asset.execution_engine)
+            docs_link: Optional[str] = get_docs_links(kwargs.get("payload", None))
 
             data_entity_list = MapValidationResult(
                 suite_result=validation_result_suite,
                 suite_result_identifier=validation_result_suite_identifier,
                 generator=generator,
                 datasets=datasets,
                 docs_link=docs_link,
             ).map()
 
-            client.ingest_data_entities(data_entity_list)
+            client.ingest_data_entity_list(data_entities=data_entity_list)
 
             logger.success(
                 f"Metadata successfully loaded to Platform. Ingested {len(data_entity_list.items)} entities"
             )
+            return {"odd_action_status": "success"}
         except Exception as e:
+            logger.debug(traceback.format_exc())
             logger.error(f"Error during collecting metadata. {e}")
+            return {"odd_action_status": "failed"}
+
+
+def get_docs_links(payload: Optional[dict]) -> Optional[str]:
+    if not payload:
+        return None
+    for action_name in payload.keys():
+        if payload[action_name]["class"] == "UpdateDataDocsAction":
+            return payload[action_name].get("local_site")
```

### Comparing `odd_great_expectations-0.1.9/odd_great_expectations/dataset/file.py` & `odd_great_expectations-0.2.0/odd_great_expectations/dataset/file.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from pathlib import Path
 
+from great_expectations.core.id_dict import BatchSpec
 from great_expectations.execution_engine import PandasExecutionEngine
-from loguru import logger
+from odd_great_expectations.logger import logger
 from oddrn_generator.generators import FilesystemGenerator
 
 
 def get_file_dataset(engine: PandasExecutionEngine) -> list[str]:
-    batch_spec = engine.batch_manager.active_batch.batch_spec
+    batch_spec: BatchSpec = engine.batch_manager.active_batch.batch_spec
 
     logger.debug("Batch spec")
     logger.debug(batch_spec.__dict__)
     logger.debug(f"Resolved path: {Path(batch_spec['path']).resolve()}")
 
     batch_path = str(Path(batch_spec["path"]).resolve())
     generator = FilesystemGenerator(host_settings="local", path=batch_path)
```

### Comparing `odd_great_expectations-0.1.9/odd_great_expectations/dataset/get_dataset.py` & `odd_great_expectations-0.2.0/odd_great_expectations/dataset/get_dataset.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
-from great_expectations.execution_engine import (ExecutionEngine,
-                                                 PandasExecutionEngine)
-from great_expectations.execution_engine.sqlalchemy_execution_engine import \
-    SqlAlchemyExecutionEngine
+from great_expectations.execution_engine import ExecutionEngine, PandasExecutionEngine
+from great_expectations.execution_engine.sqlalchemy_execution_engine import (
+    SqlAlchemyExecutionEngine,
+)
 
 from odd_great_expectations.dataset.file import get_file_dataset
 from odd_great_expectations.dataset.sql_table import get_sql_table_dataset
 
 
 def get_datasets(execution_engine: ExecutionEngine) -> List[str]:
     datasets: List[str] = []
```

### Comparing `odd_great_expectations-0.1.9/odd_great_expectations/dataset/sql_table.py` & `odd_great_expectations-0.2.0/odd_great_expectations/dataset/sql_table.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import List
-from loguru import logger
 
 from great_expectations.execution_engine.sqlalchemy_execution_engine import (
-    SqlAlchemyBatchData, SqlAlchemyExecutionEngine)
-from oddrn_generator import PostgresqlGenerator, SnowflakeGenerator
+    SqlAlchemyBatchData,
+    SqlAlchemyExecutionEngine,
+)
+from loguru import logger
+from oddrn_generator import MssqlGenerator, PostgresqlGenerator, SnowflakeGenerator
 from sqlalchemy.engine import Engine
 
 
 def postgres_dataset(engine: Engine, batch_data: SqlAlchemyBatchData) -> str:
     generator_params = {
         "host_settings": engine.url.host,
         "databases": engine.url.database,
@@ -19,29 +21,45 @@
     return generator.get_oddrn_by_path("tables")
 
 
 def snowflake_dataset(engine: Engine, batch_data: SqlAlchemyBatchData) -> str:
     # Snowflake might create SqlAlchemy database name like <DATABASE_NAME>/<SCHEMA_NAME>
     generator_params = {
         "host_settings": engine.engine.url.host,
-        "databases": engine.engine.url.database.split('/')[0],
+        "databases": engine.engine.url.database.split("/")[0],
         "schemas": batch_data.source_schema_name or "public",
         "tables": batch_data.source_table_name,
     }
 
     generator = SnowflakeGenerator(**generator_params)
-    oddrn = generator.get_oddrn_by_path('tables')
-    logger.info(f"{oddrn=}")
+    oddrn = generator.get_oddrn_by_path("tables")
+    logger.info(f"Snowflake source {oddrn=}")
+    return oddrn
+
+
+def mssql_dataset(engine: Engine, batch_data: SqlAlchemyBatchData) -> str:
+    generator_params = {
+        "host_settings": engine.url.host,
+        "databases": engine.url.database,
+        "schemas": batch_data.source_schema_name or "dbo",
+        "tables": batch_data.source_table_name,
+    }
+
+    generator = MssqlGenerator(**generator_params)
+    oddrn = generator.get_oddrn_by_path("tables")
+    logger.info(f"MSSQL source {oddrn=}")
     return oddrn
 
 
 def get_sql_table_dataset(exec_engine: SqlAlchemyExecutionEngine) -> List[str]:
     dialect_name = exec_engine.dialect_name
     engine = exec_engine.engine
     batch_data = exec_engine.batch_manager.active_batch_data
 
     if dialect_name == "postgresql":
         return [postgres_dataset(engine, batch_data)]
     elif dialect_name == "snowflake":
         return [snowflake_dataset(engine, batch_data)]
+    elif dialect_name == "mssql":
+        return [mssql_dataset(engine, batch_data)]
 
     raise ValueError(f"Unknown {dialect_name=}")
```

### Comparing `odd_great_expectations-0.1.9/odd_great_expectations/mapper.py` & `odd_great_expectations-0.2.0/odd_great_expectations/mapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,62 @@
 import datetime
 from typing import Any, Optional, Tuple
 
+from funcy import lmapcat
 from great_expectations.checkpoint.actions import (
-    ExpectationSuiteValidationResult, ValidationResultIdentifier)
+    ExpectationSuiteValidationResult,
+    ValidationResultIdentifier,
+)
 from great_expectations.core import ExpectationConfiguration
 from great_expectations.expectations.registry import get_expectation_impl
 from great_expectations.validator.validator import ExpectationValidationResult
-from odd_models.models import (DataEntity, DataEntityList, DataEntityType,
-                               DataQualityTest, DataQualityTestExpectation,
-                               DataQualityTestRun, LinkedUrl, QualityRunStatus)
+from odd_models.models import (
+    DataEntity,
+    DataEntityList,
+    DataEntityType,
+    DataQualityTest,
+    DataQualityTestExpectation,
+    DataQualityTestRun,
+    LinkedUrl,
+    QualityRunStatus,
+)
 from oddrn_generator.generators import GreatExpectationsGenerator
 
 
 class MapValidationResult:
     def __init__(
         self,
         suite_result: ExpectationSuiteValidationResult,
         suite_result_identifier: ValidationResultIdentifier,
         generator: GreatExpectationsGenerator,
         datasets: list[str],
         docs_link: Optional[str],
     ) -> None:
-        self._generator = generator
-        self._datasets = datasets
         self._result = suite_result
         self._result_identifier = suite_result_identifier
+
+        self._generator = generator
+        self._datasets = datasets
         self._docs_link = docs_link
 
     def map(self) -> DataEntityList:
-        data_entities = []
-        for result in self._result.results:
-            data_entities.extend(self._map_result(result))
+        data_entities = lmapcat(self._map_result, self._result.results)
 
         return DataEntityList(
             data_source_oddrn=self._generator.get_data_source_oddrn(),
             items=data_entities,
         )
 
     def _map_result(
         self, validation_result: ExpectationValidationResult
     ) -> tuple[DataEntity, DataEntity]:
-        run_id = self._result_identifier.run_id
-        status, status_reason = self.get_status(validation_result)
-
         job = self.map_config(validation_result.expectation_config)
+        status, status_reason = get_status(validation_result)
+
+        run_id = self._result_identifier.run_id
         oddrn = self._generator.get_oddrn_by_path("runs", run_id.run_name)
 
         run = DataEntity(
             oddrn=oddrn,
             name=f"{job.name}:{run_id.run_name}",
             type=DataEntityType.JOB_RUN,
             data_quality_test_run=DataQualityTestRun(
@@ -56,30 +65,14 @@
                 end_time=datetime.datetime.now().astimezone(),
                 status_reason=status_reason,
                 status=status,
             ),
         )
         return job, run
 
-    def get_status(
-        self, validation_result: ExpectationValidationResult
-    ) -> Tuple[QualityRunStatus, str]:
-        status = QualityRunStatus.SUCCESS
-        status_reason = None
-
-        if not validation_result.success:
-            status = QualityRunStatus.FAILED
-
-            if unexpected := validation_result.result.get("partial_unexpected_list"):
-                status_reason = (
-                    f"Unexpected values {str(unexpected)}" if unexpected else None
-                )
-
-        return status, status_reason
-
     def map_config(self, config: ExpectationConfiguration) -> DataEntity:
         original_type = config.expectation_type
         unique_path = uniq_name(config)
 
         oddrn = self._generator.get_oddrn_by_path("types", unique_path)
         suite_name = (
             self._result_identifier.expectation_suite_identifier.expectation_suite_name
@@ -102,27 +95,45 @@
             oddrn=oddrn,
             name=f"{suite_name}:{original_type}",
             type=DataEntityType.JOB,
             data_quality_test=dqt,
         )
 
 
+def get_status(
+    validation_result: ExpectationValidationResult,
+) -> Tuple[QualityRunStatus, str]:
+    status = QualityRunStatus.SUCCESS
+    status_reason = None
+
+    if not validation_result.success:
+        status = QualityRunStatus.FAILED
+
+        if unexpected := validation_result.result.get("partial_unexpected_list"):
+            status_reason = (
+                f"Unexpected values {str(unexpected)}" if unexpected else None
+            )
+
+    return status, status_reason
+
+
 def flat_kwargs(kwargs: dict[str, Any]):
     for k, v in kwargs.items():
         if isinstance(v, (list, set, tuple)):
             kwargs[k] = str(list(v))
         elif isinstance(v, dict):
             kwargs[k] = str(v)
     return kwargs
 
 
-def uniq_name(config: ExpectationConfiguration):
+def uniq_name(config: ExpectationConfiguration) -> str:
     result = config.expectation_type
     impl = get_expectation_impl(config.expectation_type)
 
     result += f":{config.kwargs.get('batch_id')}"
+
     for key in impl.args_keys:
         if value := config.kwargs.get(key):
             if isinstance(value, (list, set, tuple)):
                 value = "|".join(value)
             result += f":{key}:{value}"
     return result
```

### Comparing `odd_great_expectations-0.1.9/pyproject.toml` & `odd_great_expectations-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 [tool.poetry]
 name = "odd-great-expectations"
-version = "0.1.9"
+version = "0.2.0"
 description = "OpenDataDiscovery Action for Great Expectations"
 authors = ["Pavel Makarichev <vixtir90@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ['Open Data Discovery', 'Great Expectations', "Metadata", "Data Discovery", "Data Observability"]
 packages = [{include = "odd_great_expectations"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-odd-models = "^2.0.10"
-oddrn-generator = "0.1.62"
+odd-models = "2.0.17"
+oddrn-generator = "^0.1.68"
 great-expectations = "^0.15.44"
 funcy = "^1.17"
 sqlalchemy = "^1.4.46"
 psycopg2 = "^2.9.5"
 loguru = "^0.6.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 isort = "^5.11.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.isort]
+profile="black"
```

### Comparing `odd_great_expectations-0.1.9/setup.py` & `odd_great_expectations-0.2.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['funcy>=1.17,<2.0',
  'great-expectations>=0.15.44,<0.16.0',
  'loguru>=0.6.0,<0.7.0',
- 'odd-models>=2.0.10,<3.0.0',
- 'oddrn-generator==0.1.62',
+ 'odd-models==2.0.17',
+ 'oddrn-generator>=0.1.68,<0.2.0',
  'psycopg2>=2.9.5,<3.0.0',
  'sqlalchemy>=1.4.46,<2.0.0']
 
 setup_kwargs = {
     'name': 'odd-great-expectations',
-    'version': '0.1.9',
+    'version': '0.2.0',
     'description': 'OpenDataDiscovery Action for Great Expectations',
-    'long_description': "## OpenDataDiscovery Great Expectations metadata collecting.\n[![PyPI version](https://badge.fury.io/py/odd-great-expectations.svg)](https://badge.fury.io/py/odd-great-expectations)\n\n## Supporting\n| Feature                     | Supporting |\n| --------------------------- | ---------- |\n| V3 API +                    | +          |\n| SqlAlchemyEngine            | +          |\n| PandasEngine                | +          |\n| Great Expectations V2 API - | -          |\n| Cloud Solution              | -          |\n\n\n`odd_great_expectation.action.ODDAction`\nIs a class derived from `ValidationAction` and can be used in checkpoint actions lists.\n\n## How to:\n\n### Install odd-great-expectations package\n```bash\npip install odd-great-expectations\n```\n\n### Add action to checkpoint:\n```yaml\nname: <CHECKPOINT_NAME>\nconfig_version: 1.0\ntemplate_name:\nmodule_name: great_expectations.checkpoint\nclass_name: Checkpoint\nrun_name_template: '%Y%m%d-%H%M%S-my-run-name-template'\nexpectation_suite_name:\nbatch_request: {}\naction_list:\n  # other actions\n  - name: store_metadata_to_odd \n    action:\n      module_name: odd_great_expectations.action\n      class_name: ODDAction\n      platform_host: <PLATFORM_HOST> # OpenDataDiscovery platform, i.e. http://localhost:8080\n      platform_token: <PLATFORM_TOKEN> # OpenDataDiscovery token\n      data_source_name: <DATA_SOURCE_NAME> # Unique name for data source, i.e. local_qa_test\nevaluation_parameters: {}\n```\n\n### Run checkpoint\n```bash\ngreat_expectations checkpoint run <CHECKPOINT_NAME> \n```\n### Check result\nCheck results on <PLATFORM_HOST> UI.\n\n\n",
+    'long_description': "## OpenDataDiscovery Action for handling Great Expectations tests results.\n\n[![PyPI version](https://badge.fury.io/py/odd-great-expectations.svg)](https://badge.fury.io/py/odd-great-expectations)\n\n![image](assets/screenshot.png)\n\n# What is it?\n`odd_great_expectation.action.ODDAction`\nIs a class derived from GX `ValidationAction` which will be run by GreatExpectations at runtime with `ValidationResult`s for checkpoint.\n\n\n# How to use it?:\nInstall `odd-great-expectations` package\n```bash\npip install odd-great-expectations\n```\nAdd `ODDAction` action to some checkpoint's action list:\n```yaml\nname: <CHECKPOINT_NAME>\nconfig_version: 1.0\n...\naction_list:\n  # other actions\n  - name: store_metadata_to_odd\n    action:\n      module_name: odd_great_expectations.action\n      class_name: ODDAction\n      platform_host: <PLATFORM_HOST>\n      data_source_name: <DATA_SOURCE_NAME>\n```\n\nParameters:\n\n`platform_host` - Location of OpenDataDiscovery platform, i.e. http://localhost:8080\n\n`platform_token` - OpenDataDiscovery token, how to get it - https://docs.opendatadiscovery.org/configuration-and-deployment/trylocally#create-collector-entity\n\n`data_source_name` - Unique name for data source, i.e. local_qa_test\n\nBoth `platform_host` and `platform_token`  can be set using `ODD_PLATFORM_HOST` and `ODD_PLATFORM_PLATFORM` env variables accordingly.\n\nRun checkpoint\n```bash\ngreat_expectations checkpoint run <CHECKPOINT_NAME>\n```\nCheck results on `PLATFORM_HOST` UI.\n\n## Supporting features\n| Feature                     | Supporting |\n| --------------------------- | ---------- |\n| V3 API +                    | +          |\n| SqlAlchemyEngine            | +          |\n| PandasEngine                | +          |\n| Great Expectations V2 API - | -          |\n| Cloud Solution              | -          |\n",
     'author': 'Pavel Makarichev',
     'author_email': 'vixtir90@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `odd_great_expectations-0.1.9/PKG-INFO` & `odd_great_expectations-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,77 +1,79 @@
 Metadata-Version: 2.1
 Name: odd-great-expectations
-Version: 0.1.9
+Version: 0.2.0
 Summary: OpenDataDiscovery Action for Great Expectations
 License: Apache-2.0
 Keywords: Open Data Discovery,Great Expectations,Metadata,Data Discovery,Data Observability
 Author: Pavel Makarichev
 Author-email: vixtir90@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: funcy (>=1.17,<2.0)
 Requires-Dist: great-expectations (>=0.15.44,<0.16.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
-Requires-Dist: odd-models (>=2.0.10,<3.0.0)
-Requires-Dist: oddrn-generator (==0.1.62)
+Requires-Dist: odd-models (==2.0.17)
+Requires-Dist: oddrn-generator (>=0.1.68,<0.2.0)
 Requires-Dist: psycopg2 (>=2.9.5,<3.0.0)
 Requires-Dist: sqlalchemy (>=1.4.46,<2.0.0)
 Description-Content-Type: text/markdown
 
-## OpenDataDiscovery Great Expectations metadata collecting.
-[![PyPI version](https://badge.fury.io/py/odd-great-expectations.svg)](https://badge.fury.io/py/odd-great-expectations)
+## OpenDataDiscovery Action for handling Great Expectations tests results.
 
-## Supporting
-| Feature                     | Supporting |
-| --------------------------- | ---------- |
-| V3 API +                    | +          |
-| SqlAlchemyEngine            | +          |
-| PandasEngine                | +          |
-| Great Expectations V2 API - | -          |
-| Cloud Solution              | -          |
+[![PyPI version](https://badge.fury.io/py/odd-great-expectations.svg)](https://badge.fury.io/py/odd-great-expectations)
 
+![image](assets/screenshot.png)
 
+# What is it?
 `odd_great_expectation.action.ODDAction`
-Is a class derived from `ValidationAction` and can be used in checkpoint actions lists.
+Is a class derived from GX `ValidationAction` which will be run by GreatExpectations at runtime with `ValidationResult`s for checkpoint.
 
-## How to:
 
-### Install odd-great-expectations package
+# How to use it?:
+Install `odd-great-expectations` package
 ```bash
 pip install odd-great-expectations
 ```
-
-### Add action to checkpoint:
+Add `ODDAction` action to some checkpoint's action list:
 ```yaml
 name: <CHECKPOINT_NAME>
 config_version: 1.0
-template_name:
-module_name: great_expectations.checkpoint
-class_name: Checkpoint
-run_name_template: '%Y%m%d-%H%M%S-my-run-name-template'
-expectation_suite_name:
-batch_request: {}
+...
 action_list:
   # other actions
-  - name: store_metadata_to_odd 
+  - name: store_metadata_to_odd
     action:
       module_name: odd_great_expectations.action
       class_name: ODDAction
-      platform_host: <PLATFORM_HOST> # OpenDataDiscovery platform, i.e. http://localhost:8080
-      platform_token: <PLATFORM_TOKEN> # OpenDataDiscovery token
-      data_source_name: <DATA_SOURCE_NAME> # Unique name for data source, i.e. local_qa_test
-evaluation_parameters: {}
+      platform_host: <PLATFORM_HOST>
+      data_source_name: <DATA_SOURCE_NAME>
 ```
 
-### Run checkpoint
+Parameters:
+
+`platform_host` - Location of OpenDataDiscovery platform, i.e. http://localhost:8080
+
+`platform_token` - OpenDataDiscovery token, how to get it - https://docs.opendatadiscovery.org/configuration-and-deployment/trylocally#create-collector-entity
+
+`data_source_name` - Unique name for data source, i.e. local_qa_test
+
+Both `platform_host` and `platform_token`  can be set using `ODD_PLATFORM_HOST` and `ODD_PLATFORM_PLATFORM` env variables accordingly.
+
+Run checkpoint
 ```bash
-great_expectations checkpoint run <CHECKPOINT_NAME> 
+great_expectations checkpoint run <CHECKPOINT_NAME>
 ```
-### Check result
-Check results on <PLATFORM_HOST> UI.
-
+Check results on `PLATFORM_HOST` UI.
 
+## Supporting features
+| Feature                     | Supporting |
+| --------------------------- | ---------- |
+| V3 API +                    | +          |
+| SqlAlchemyEngine            | +          |
+| PandasEngine                | +          |
+| Great Expectations V2 API - | -          |
+| Cloud Solution              | -          |
```


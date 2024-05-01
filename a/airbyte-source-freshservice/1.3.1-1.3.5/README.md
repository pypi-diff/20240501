# Comparing `tmp/airbyte-source-freshservice-1.3.1.tar.gz` & `tmp/airbyte_source_freshservice-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-freshservice-1.3.1.tar", last modified: Thu Feb  8 16:28:05 2024, max compression
+gzip compressed data, was "airbyte_source_freshservice-1.3.5.tar", max compression
```

## Comparing `airbyte-source-freshservice-1.3.1.tar` & `airbyte_source_freshservice-1.3.5.tar`

### file list

```diff
@@ -1,41 +1,8 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:28:05.817923 airbyte-source-freshservice-1.3.1/
--rw-r--r--   0 root         (0) root         (0)     4227 2024-02-08 16:28:05.817923 airbyte-source-freshservice-1.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4091 2024-02-08 16:06:01.000000 airbyte-source-freshservice-1.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:28:05.817923 airbyte-source-freshservice-1.3.1/airbyte_source_freshservice.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4227 2024-02-08 16:28:05.000000 airbyte-source-freshservice-1.3.1/airbyte_source_freshservice.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1361 2024-02-08 16:28:05.000000 airbyte-source-freshservice-1.3.1/airbyte_source_freshservice.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-08 16:28:05.000000 airbyte-source-freshservice-1.3.1/airbyte_source_freshservice.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2024-02-08 16:28:05.000000 airbyte-source-freshservice-1.3.1/airbyte_source_freshservice.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       60 2024-02-08 16:28:05.000000 airbyte-source-freshservice-1.3.1/airbyte_source_freshservice.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-08 16:28:05.000000 airbyte-source-freshservice-1.3.1/airbyte_source_freshservice.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:28:05.813923 airbyte-source-freshservice-1.3.1/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-02-08 16:06:01.000000 airbyte-source-freshservice-1.3.1/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      249 2024-02-08 16:06:01.000000 airbyte-source-freshservice-1.3.1/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-02-08 16:06:01.000000 airbyte-source-freshservice-1.3.1/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     4935 2024-02-08 16:06:01.000000 airbyte-source-freshservice-1.3.1/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)      119 2024-02-08 16:06:01.000000 airbyte-source-freshservice-1.3.1/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)      111 2024-02-08 16:06:01.000000 airbyte-source-freshservice-1.3.1/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)      249 2024-02-08 16:06:01.000000 airbyte-source-freshservice-1.3.1/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     4136 2024-02-08 16:28:05.821923 airbyte-source-freshservice-1.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      903 2024-02-08 16:28:03.000000 airbyte-source-freshservice-1.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:28:05.813923 airbyte-source-freshservice-1.3.1/source_freshservice/
--rw-r--r--   0 root         (0) root         (0)      136 2024-02-08 16:06:01.000000 airbyte-source-freshservice-1.3.1/source_freshservice/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5819 2024-02-08 16:06:01.000000 airbyte-source-freshservice-1.3.1/source_freshservice/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      248 2024-02-08 16:06:01.000000 airbyte-source-freshservice-1.3.1/source_freshservice/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-08 16:28:05.817923 airbyte-source-freshservice-1.3.1/source_freshservice/schemas/
--rw-r--r--   0 root         (0) root         (0)     3295 2024-02-08 16:06:01.000000 airbyte-source-freshservice-1.3.1/source_freshservice/schemas/agents.json
--rw-r--r--   0 root         (0) root         (0)     1292 2024-02-08 16:06:01.000000 airbyte-source-freshservice-1.3.1/source_freshservice/schemas/assets.json
--rw-r--r--   0 root         (0) root         (0)     2324 2024-02-08 16:06:01.000000 airbyte-source-freshservice-1.3.1/source_freshservice/schemas/changes.json
--rw-r--r--   0 root         (0) root         (0)     1178 2024-02-08 16:06:01.000000 airbyte-source-freshservice-1.3.1/source_freshservice/schemas/locations.json
--rw-r--r--   0 root         (0) root         (0)     2075 2024-02-08 16:06:01.000000 airbyte-source-freshservice-1.3.1/source_freshservice/schemas/problems.json
--rw-r--r--   0 root         (0) root         (0)      657 2024-02-08 16:06:01.000000 airbyte-source-freshservice-1.3.1/source_freshservice/schemas/products.json
--rw-r--r--   0 root         (0) root         (0)     1549 2024-02-08 16:06:01.000000 airbyte-source-freshservice-1.3.1/source_freshservice/schemas/purchase_orders.json
--rw-r--r--   0 root         (0) root         (0)     1219 2024-02-08 16:06:01.000000 airbyte-source-freshservice-1.3.1/source_freshservice/schemas/releases.json
--rw-r--r--   0 root         (0) root         (0)      956 2024-02-08 16:06:01.000000 airbyte-source-freshservice-1.3.1/source_freshservice/schemas/requested_items.json
--rw-r--r--   0 root         (0) root         (0)     1995 2024-02-08 16:06:01.000000 airbyte-source-freshservice-1.3.1/source_freshservice/schemas/requesters.json
--rw-r--r--   0 root         (0) root         (0)     1351 2024-02-08 16:06:01.000000 airbyte-source-freshservice-1.3.1/source_freshservice/schemas/satisfaction_survey_responses.json
--rw-r--r--   0 root         (0) root         (0)     1150 2024-02-08 16:06:01.000000 airbyte-source-freshservice-1.3.1/source_freshservice/schemas/software.json
--rw-r--r--   0 root         (0) root         (0)     2383 2024-02-08 16:06:01.000000 airbyte-source-freshservice-1.3.1/source_freshservice/schemas/tickets.json
--rw-r--r--   0 root         (0) root         (0)     1224 2024-02-08 16:06:01.000000 airbyte-source-freshservice-1.3.1/source_freshservice/schemas/vendors.json
--rw-r--r--   0 root         (0) root         (0)      481 2024-02-08 16:06:01.000000 airbyte-source-freshservice-1.3.1/source_freshservice/source.py
--rw-r--r--   0 root         (0) root         (0)     1024 2024-02-08 16:06:01.000000 airbyte-source-freshservice-1.3.1/source_freshservice/spec.yaml
+-rw-r--r--   0        0        0     4604 2024-05-01 18:44:13.227403 airbyte_source_freshservice-1.3.5/README.md
+-rw-r--r--   0        0        0      754 2024-05-01 18:47:57.042502 airbyte_source_freshservice-1.3.5/pyproject.toml
+-rw-r--r--   0        0        0      136 2024-05-01 18:44:13.227403 airbyte_source_freshservice-1.3.5/source_freshservice/__init__.py
+-rw-r--r--   0        0        0    60080 2024-05-01 18:44:13.227403 airbyte_source_freshservice-1.3.5/source_freshservice/manifest.yaml
+-rw-r--r--   0        0        0      248 2024-05-01 18:44:13.227403 airbyte_source_freshservice-1.3.5/source_freshservice/run.py
+-rw-r--r--   0        0        0      481 2024-05-01 18:44:13.227403 airbyte_source_freshservice-1.3.5/source_freshservice/source.py
+-rw-r--r--   0        0        0     1024 2024-05-01 18:44:13.227403 airbyte_source_freshservice-1.3.5/source_freshservice/spec.yaml
+-rw-r--r--   0        0        0     5326 1970-01-01 00:00:00.000000 airbyte_source_freshservice-1.3.5/PKG-INFO
```

### Comparing `airbyte-source-freshservice-1.3.1/PKG-INFO` & `airbyte_source_freshservice-1.3.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,91 @@
-Metadata-Version: 2.1
-Name: airbyte-source-freshservice
-Version: 1.3.1
-Summary: Source implementation for Freshservice.
-Author: Airbyte
-Author-email: contact@airbyte.io
-Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.55.2
-Provides-Extra: tests
-Requires-Dist: pytest~=6.2; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
+# Freshservice source connector
 
-# Freshservice Source
 
-This is the repository for the Freshservice configuration based source connector.
+This is the repository for the Freshservice source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/freshservice).
 
+## Local development
 
+### Prerequisites
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
+
+
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
+```
+
+
+### Create credentials
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/freshservice)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_freshservice/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source freshservice test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
+```
+poetry run source-freshservice spec
+poetry run source-freshservice check --config secrets/config.json
+poetry run source-freshservice discover --config secrets/config.json
+poetry run source-freshservice read --config secrets/config.json --catalog sample_files/configured_catalog.json
+```
 
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-freshservice build
 ```
 
-An image will be built with the tag `airbyte/source-freshservice:dev`.
+An image will be available on your host with the tag `airbyte/source-freshservice:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-freshservice:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-freshservice:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-freshservice:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-freshservice:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-freshservice:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-freshservice test
 ```
 
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+### Customizing acceptance Tests
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
+## Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-freshservice test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/freshservice.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/freshservice.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-freshservice-1.3.1/airbyte_source_freshservice.egg-info/PKG-INFO` & `airbyte_source_freshservice-1.3.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,110 @@
 Metadata-Version: 2.1
 Name: airbyte-source-freshservice
-Version: 1.3.1
+Version: 1.3.5
 Summary: Source implementation for Freshservice.
+Home-page: https://airbyte.com
+License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: airbyte-cdk (==0.80.0)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/freshservice
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.55.2
-Provides-Extra: tests
-Requires-Dist: pytest~=6.2; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
 
-# Freshservice Source
+# Freshservice source connector
 
-This is the repository for the Freshservice configuration based source connector.
+
+This is the repository for the Freshservice source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/freshservice).
 
+## Local development
+
+### Prerequisites
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
+
+
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
+```
 
+
+### Create credentials
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/freshservice)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_freshservice/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source freshservice test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
+```
+poetry run source-freshservice spec
+poetry run source-freshservice check --config secrets/config.json
+poetry run source-freshservice discover --config secrets/config.json
+poetry run source-freshservice read --config secrets/config.json --catalog sample_files/configured_catalog.json
+```
 
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-freshservice build
 ```
 
-An image will be built with the tag `airbyte/source-freshservice:dev`.
+An image will be available on your host with the tag `airbyte/source-freshservice:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-freshservice:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-freshservice:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-freshservice:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-freshservice:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-freshservice:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-freshservice test
 ```
 
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+### Customizing acceptance Tests
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
+## Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-freshservice test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/freshservice.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/freshservice.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-freshservice-1.3.1/source_freshservice/spec.yaml` & `airbyte_source_freshservice-1.3.5/source_freshservice/spec.yaml`

 * *Files identical despite different names*


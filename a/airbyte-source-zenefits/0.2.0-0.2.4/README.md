# Comparing `tmp/airbyte-source-zenefits-0.2.0.tar.gz` & `tmp/airbyte_source_zenefits-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-zenefits-0.2.0.tar", last modified: Thu Feb  1 11:13:55 2024, max compression
+gzip compressed data, was "airbyte_source_zenefits-0.2.4.tar", max compression
```

## Comparing `airbyte-source-zenefits-0.2.0.tar` & `airbyte_source_zenefits-0.2.4.tar`

### file list

```diff
@@ -1,36 +1,7 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 11:13:55.191618 airbyte-source-zenefits-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     4502 2024-02-01 11:13:55.191618 airbyte-source-zenefits-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4346 2024-02-01 11:08:10.000000 airbyte-source-zenefits-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 11:13:55.191618 airbyte-source-zenefits-0.2.0/airbyte_source_zenefits.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4502 2024-02-01 11:13:55.000000 airbyte-source-zenefits-0.2.0/airbyte_source_zenefits.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1102 2024-02-01 11:13:55.000000 airbyte-source-zenefits-0.2.0/airbyte_source_zenefits.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-01 11:13:55.000000 airbyte-source-zenefits-0.2.0/airbyte_source_zenefits.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2024-02-01 11:13:55.000000 airbyte-source-zenefits-0.2.0/airbyte_source_zenefits.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-01 11:13:55.000000 airbyte-source-zenefits-0.2.0/airbyte_source_zenefits.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       34 2024-02-01 11:13:55.000000 airbyte-source-zenefits-0.2.0/airbyte_source_zenefits.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 11:13:55.183618 airbyte-source-zenefits-0.2.0/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-02-01 11:08:10.000000 airbyte-source-zenefits-0.2.0/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      314 2024-02-01 11:08:10.000000 airbyte-source-zenefits-0.2.0/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     5522 2024-02-01 11:08:10.000000 airbyte-source-zenefits-0.2.0/integration_tests/catalog.json
--rw-r--r--   0 root         (0) root         (0)     5522 2024-02-01 11:08:10.000000 airbyte-source-zenefits-0.2.0/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)       25 2024-02-01 11:08:10.000000 airbyte-source-zenefits-0.2.0/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)       50 2024-02-01 11:08:10.000000 airbyte-source-zenefits-0.2.0/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)     4375 2024-02-01 11:13:55.191618 airbyte-source-zenefits-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      907 2024-02-01 11:13:53.000000 airbyte-source-zenefits-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 11:13:55.187618 airbyte-source-zenefits-0.2.0/source_zenefits/
--rw-r--r--   0 root         (0) root         (0)      128 2024-02-01 11:08:10.000000 airbyte-source-zenefits-0.2.0/source_zenefits/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13045 2024-02-01 11:08:10.000000 airbyte-source-zenefits-0.2.0/source_zenefits/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      236 2024-02-01 11:08:10.000000 airbyte-source-zenefits-0.2.0/source_zenefits/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 11:13:55.187618 airbyte-source-zenefits-0.2.0/source_zenefits/schemas/
--rw-r--r--   0 root         (0) root         (0)      896 2024-02-01 11:08:10.000000 airbyte-source-zenefits-0.2.0/source_zenefits/schemas/custom_field_values.json
--rw-r--r--   0 root         (0) root         (0)     1766 2024-02-01 11:08:10.000000 airbyte-source-zenefits-0.2.0/source_zenefits/schemas/custom_fields.json
--rw-r--r--   0 root         (0) root         (0)     1165 2024-02-01 11:08:10.000000 airbyte-source-zenefits-0.2.0/source_zenefits/schemas/departments.json
--rw-r--r--   0 root         (0) root         (0)     1305 2024-02-01 11:08:10.000000 airbyte-source-zenefits-0.2.0/source_zenefits/schemas/employments.json
--rw-r--r--   0 root         (0) root         (0)      885 2024-02-01 11:08:10.000000 airbyte-source-zenefits-0.2.0/source_zenefits/schemas/labor_group_types.json
--rw-r--r--   0 root         (0) root         (0)     1480 2024-02-01 11:08:10.000000 airbyte-source-zenefits-0.2.0/source_zenefits/schemas/labor_groups.json
--rw-r--r--   0 root         (0) root         (0)     1553 2024-02-01 11:08:10.000000 airbyte-source-zenefits-0.2.0/source_zenefits/schemas/locations.json
--rw-r--r--   0 root         (0) root         (0)     4470 2024-02-01 11:08:10.000000 airbyte-source-zenefits-0.2.0/source_zenefits/schemas/people.json
--rw-r--r--   0 root         (0) root         (0)     1504 2024-02-01 11:08:10.000000 airbyte-source-zenefits-0.2.0/source_zenefits/schemas/time_durations.json
--rw-r--r--   0 root         (0) root         (0)     1584 2024-02-01 11:08:10.000000 airbyte-source-zenefits-0.2.0/source_zenefits/schemas/vacation_requests.json
--rw-r--r--   0 root         (0) root         (0)     1063 2024-02-01 11:08:10.000000 airbyte-source-zenefits-0.2.0/source_zenefits/schemas/vacation_types.json
--rw-r--r--   0 root         (0) root         (0)      477 2024-02-01 11:08:10.000000 airbyte-source-zenefits-0.2.0/source_zenefits/source.py
+-rw-r--r--   0        0        0     4532 2024-04-30 23:37:40.676178 airbyte_source_zenefits-0.2.4/README.md
+-rw-r--r--   0        0        0      755 2024-04-30 23:41:19.442305 airbyte_source_zenefits-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      128 2024-04-30 23:37:40.676178 airbyte_source_zenefits-0.2.4/source_zenefits/__init__.py
+-rw-r--r--   0        0        0    52321 2024-04-30 23:37:40.676178 airbyte_source_zenefits-0.2.4/source_zenefits/manifest.yaml
+-rw-r--r--   0        0        0      236 2024-04-30 23:37:40.676178 airbyte_source_zenefits-0.2.4/source_zenefits/run.py
+-rw-r--r--   0        0        0      477 2024-04-30 23:37:40.676178 airbyte_source_zenefits-0.2.4/source_zenefits/source.py
+-rw-r--r--   0        0        0     5242 1970-01-01 00:00:00.000000 airbyte_source_zenefits-0.2.4/PKG-INFO
```

### Comparing `airbyte-source-zenefits-0.2.0/PKG-INFO` & `airbyte_source_zenefits-0.2.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,91 @@
-Metadata-Version: 2.1
-Name: airbyte-source-zenefits
-Version: 0.2.0
-Summary: Source implementation for Zenefits.
-Author: Airbyte
-Author-email: contact@airbyte.io
-Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.2; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
+# Zenefits source connector
 
-# *How to access the token from Zenefits*
 
-Login into the Zenefits portal. <br>
-Follow the steps in the given link [Here](https://developers.zenefits.com/docs/sync-with-zenefits-button), This will generate and Bearer token for the user which can be used to interact with the API using the source-zenefits connector.
+This is the repository for the Zenefits source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/zenefits).
 
+## Local development
 
+### Prerequisites
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 
-This is the repository for the Zenefits configuration based source connector.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/zenefits).
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
+```
 
 
+### Create credentials
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/zenefits)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_zenefits/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source zenefits test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
+```
+poetry run source-zenefits spec
+poetry run source-zenefits check --config secrets/config.json
+poetry run source-zenefits discover --config secrets/config.json
+poetry run source-zenefits read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-zenefits build
 ```
 
-An image will be built with the tag `airbyte/source-zenefits:dev`.
+An image will be available on your host with the tag `airbyte/source-zenefits:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-zenefits:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-zenefits:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-zenefits:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-zenefits:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-zenefits:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-zenefits test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-zenefits test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/zenefits.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/zenefits.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-zenefits-0.2.0/airbyte_source_zenefits.egg-info/PKG-INFO` & `airbyte_source_zenefits-0.2.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,110 @@
 Metadata-Version: 2.1
 Name: airbyte-source-zenefits
-Version: 0.2.0
+Version: 0.2.4
 Summary: Source implementation for Zenefits.
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
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/zenefits
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.2; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
 
-# *How to access the token from Zenefits*
+# Zenefits source connector
 
-Login into the Zenefits portal. <br>
-Follow the steps in the given link [Here](https://developers.zenefits.com/docs/sync-with-zenefits-button), This will generate and Bearer token for the user which can be used to interact with the API using the source-zenefits connector.
 
+This is the repository for the Zenefits source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/zenefits).
 
+## Local development
 
+### Prerequisites
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-This is the repository for the Zenefits configuration based source connector.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/zenefits).
 
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
+```
 
+
+### Create credentials
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/zenefits)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_zenefits/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source zenefits test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
+```
+poetry run source-zenefits spec
+poetry run source-zenefits check --config secrets/config.json
+poetry run source-zenefits discover --config secrets/config.json
+poetry run source-zenefits read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-zenefits build
 ```
 
-An image will be built with the tag `airbyte/source-zenefits:dev`.
+An image will be available on your host with the tag `airbyte/source-zenefits:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-zenefits:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-zenefits:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-zenefits:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-zenefits:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-zenefits:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-zenefits test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-zenefits test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/zenefits.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/zenefits.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```


# Comparing `tmp/airbyte-source-recreation-0.1.0.tar.gz` & `tmp/airbyte_source_recreation-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-recreation-0.1.0.tar", last modified: Wed Jan 31 16:43:51 2024, max compression
+gzip compressed data, was "airbyte_source_recreation-0.1.3.tar", max compression
```

## Comparing `airbyte-source-recreation-0.1.0.tar` & `airbyte_source_recreation-0.1.3.tar`

### file list

```diff
@@ -1,39 +1,8 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:43:51.746065 airbyte-source-recreation-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     4754 2024-01-31 16:43:51.746065 airbyte-source-recreation-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4571 2024-01-31 16:34:25.000000 airbyte-source-recreation-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:43:51.746065 airbyte-source-recreation-0.1.0/airbyte_source_recreation.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4754 2024-01-31 16:43:51.000000 airbyte-source-recreation-0.1.0/airbyte_source_recreation.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1229 2024-01-31 16:43:51.000000 airbyte-source-recreation-0.1.0/airbyte_source_recreation.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-31 16:43:51.000000 airbyte-source-recreation-0.1.0/airbyte_source_recreation.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-01-31 16:43:51.000000 airbyte-source-recreation-0.1.0/airbyte_source_recreation.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-01-31 16:43:51.000000 airbyte-source-recreation-0.1.0/airbyte_source_recreation.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2024-01-31 16:43:51.000000 airbyte-source-recreation-0.1.0/airbyte_source_recreation.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:43:51.742065 airbyte-source-recreation-0.1.0/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 16:34:25.000000 airbyte-source-recreation-0.1.0/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)       58 2024-01-31 16:34:25.000000 airbyte-source-recreation-0.1.0/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-01-31 16:34:25.000000 airbyte-source-recreation-0.1.0/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     2494 2024-01-31 16:34:25.000000 airbyte-source-recreation-0.1.0/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)       30 2024-01-31 16:34:25.000000 airbyte-source-recreation-0.1.0/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)       54 2024-01-31 16:34:25.000000 airbyte-source-recreation-0.1.0/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)       46 2024-01-31 16:34:25.000000 airbyte-source-recreation-0.1.0/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     4615 2024-01-31 16:43:51.746065 airbyte-source-recreation-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      933 2024-01-31 16:43:49.000000 airbyte-source-recreation-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:43:51.742065 airbyte-source-recreation-0.1.0/source_recreation/
--rw-r--r--   0 root         (0) root         (0)      132 2024-01-31 16:34:25.000000 airbyte-source-recreation-0.1.0/source_recreation/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3568 2024-01-31 16:34:25.000000 airbyte-source-recreation-0.1.0/source_recreation/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      242 2024-01-31 16:34:25.000000 airbyte-source-recreation-0.1.0/source_recreation/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 16:43:51.746065 airbyte-source-recreation-0.1.0/source_recreation/schemas/
--rw-r--r--   0 root         (0) root         (0)      315 2024-01-31 16:34:25.000000 airbyte-source-recreation-0.1.0/source_recreation/schemas/activities.json
--rw-r--r--   0 root         (0) root         (0)     2435 2024-01-31 16:34:25.000000 airbyte-source-recreation-0.1.0/source_recreation/schemas/campsites.json
--rw-r--r--   0 root         (0) root         (0)      249 2024-01-31 16:34:25.000000 airbyte-source-recreation-0.1.0/source_recreation/schemas/events.json
--rw-r--r--   0 root         (0) root         (0)     7294 2024-01-31 16:34:25.000000 airbyte-source-recreation-0.1.0/source_recreation/schemas/facilities.json
--rw-r--r--   0 root         (0) root         (0)      716 2024-01-31 16:34:25.000000 airbyte-source-recreation-0.1.0/source_recreation/schemas/facilityaddresses.json
--rw-r--r--   0 root         (0) root         (0)      438 2024-01-31 16:34:25.000000 airbyte-source-recreation-0.1.0/source_recreation/schemas/links.json
--rw-r--r--   0 root         (0) root         (0)      827 2024-01-31 16:34:25.000000 airbyte-source-recreation-0.1.0/source_recreation/schemas/media.json
--rw-r--r--   0 root         (0) root         (0)      612 2024-01-31 16:34:25.000000 airbyte-source-recreation-0.1.0/source_recreation/schemas/organizations.json
--rw-r--r--   0 root         (0) root         (0)     2697 2024-01-31 16:34:25.000000 airbyte-source-recreation-0.1.0/source_recreation/schemas/permits.json
--rw-r--r--   0 root         (0) root         (0)      710 2024-01-31 16:34:25.000000 airbyte-source-recreation-0.1.0/source_recreation/schemas/recreationareaaddresses.json
--rw-r--r--   0 root         (0) root         (0)     6089 2024-01-31 16:34:25.000000 airbyte-source-recreation-0.1.0/source_recreation/schemas/recreationareas.json
--rw-r--r--   0 root         (0) root         (0)     2276 2024-01-31 16:34:25.000000 airbyte-source-recreation-0.1.0/source_recreation/schemas/tours.json
--rw-r--r--   0 root         (0) root         (0)      479 2024-01-31 16:34:25.000000 airbyte-source-recreation-0.1.0/source_recreation/source.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-01-31 16:34:25.000000 airbyte-source-recreation-0.1.0/source_recreation/spec.yaml
+-rw-r--r--   0        0        0     4568 2024-05-01 17:12:23.331291 airbyte_source_recreation-0.1.3/README.md
+-rw-r--r--   0        0        0      767 2024-05-01 17:16:23.811740 airbyte_source_recreation-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      132 2024-05-01 17:12:23.331291 airbyte_source_recreation-0.1.3/source_recreation/__init__.py
+-rw-r--r--   0        0        0    49924 2024-05-01 17:12:23.331291 airbyte_source_recreation-0.1.3/source_recreation/manifest.yaml
+-rw-r--r--   0        0        0      242 2024-05-01 17:12:23.331291 airbyte_source_recreation-0.1.3/source_recreation/run.py
+-rw-r--r--   0        0        0      479 2024-05-01 17:12:23.331291 airbyte_source_recreation-0.1.3/source_recreation/source.py
+-rw-r--r--   0        0        0      435 2024-05-01 17:12:23.331291 airbyte_source_recreation-0.1.3/source_recreation/spec.yaml
+-rw-r--r--   0        0        0     5284 1970-01-01 00:00:00.000000 airbyte_source_recreation-0.1.3/PKG-INFO
```

### Comparing `airbyte-source-recreation-0.1.0/PKG-INFO` & `airbyte_source_recreation-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,110 @@
 Metadata-Version: 2.1
 Name: airbyte-source-recreation
-Version: 0.1.0
+Version: 0.1.3
 Summary: Source implementation for Recreation.
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
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/recreation
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.1
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.1; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
 
-# Recreation Source
+# Recreation source connector
 
-This is the repository for the Recreation configuration based source connector.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/recreation).
 
-The Recreation Information Database (RIDB) provides data resources to citizens, offering a single point of access to information about recreational opportunities nationwide. The RIDB represents an authoritative source of information and services for millions of visitors to federal lands, historic sites, museums, and other attractions/resources. This initiative integrates multiple Federal channels and sources about recreation opportunities into a one-stop, searchable database of recreational areas nationwide.
+This is the repository for the Recreation source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/recreation).
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/recreation)
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
+
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/recreation)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_recreation/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source recreation test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
+```
+poetry run source-recreation spec
+poetry run source-recreation check --config secrets/config.json
+poetry run source-recreation discover --config secrets/config.json
+poetry run source-recreation read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-recreation build
 ```
 
-An image will be built with the tag `airbyte/source-recreation:dev`.
+An image will be available on your host with the tag `airbyte/source-recreation:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-recreation:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-recreation:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-recreation:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-recreation:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-recreation:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-recreation test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-recreation test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/recreation.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/recreation.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-recreation-0.1.0/README.md` & `airbyte_source_recreation-0.1.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,91 @@
-# Recreation Source
+# Recreation source connector
 
-This is the repository for the Recreation configuration based source connector.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/recreation).
 
-The Recreation Information Database (RIDB) provides data resources to citizens, offering a single point of access to information about recreational opportunities nationwide. The RIDB represents an authoritative source of information and services for millions of visitors to federal lands, historic sites, museums, and other attractions/resources. This initiative integrates multiple Federal channels and sources about recreation opportunities into a one-stop, searchable database of recreational areas nationwide.
+This is the repository for the Recreation source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/recreation).
+
 ## Local development
 
-#### Create credentials
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/recreation)
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
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/recreation)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_recreation/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source recreation test creds`
-and place them into `secrets/config.json`.
 
-### Locally running the connector docker image
+### Locally running the connector
+```
+poetry run source-recreation spec
+poetry run source-recreation check --config secrets/config.json
+poetry run source-recreation discover --config secrets/config.json
+poetry run source-recreation read --config secrets/config.json --catalog sample_files/configured_catalog.json
+```
 
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-#### Build
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-recreation build
 ```
 
-An image will be built with the tag `airbyte/source-recreation:dev`.
+An image will be available on your host with the tag `airbyte/source-recreation:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-recreation:dev .
-```
 
-#### Run
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-recreation:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-recreation:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-recreation:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-recreation:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-## Testing
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-recreation test
 ```
 
 ### Customizing acceptance Tests
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-## Dependency Management
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
 
-### Publishing a new version of the connector
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
+
+## Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-recreation test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/recreation.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/recreation.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```


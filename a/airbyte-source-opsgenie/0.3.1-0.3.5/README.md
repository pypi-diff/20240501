# Comparing `tmp/airbyte-source-opsgenie-0.3.1.tar.gz` & `tmp/airbyte_source_opsgenie-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-opsgenie-0.3.1.tar", last modified: Fri Feb 16 20:11:23 2024, max compression
+gzip compressed data, was "airbyte_source_opsgenie-0.3.5.tar", max compression
```

## Comparing `airbyte-source-opsgenie-0.3.1.tar` & `airbyte_source_opsgenie-0.3.5.tar`

### file list

```diff
@@ -1,36 +1,8 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 20:11:23.170480 airbyte-source-opsgenie-0.3.1/
--rw-r--r--   0 root         (0) root         (0)     4777 2024-02-16 20:11:23.170480 airbyte-source-opsgenie-0.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4611 2024-02-16 19:40:33.000000 airbyte-source-opsgenie-0.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 20:11:23.170480 airbyte-source-opsgenie-0.3.1/airbyte_source_opsgenie.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4777 2024-02-16 20:11:23.000000 airbyte-source-opsgenie-0.3.1/airbyte_source_opsgenie.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1049 2024-02-16 20:11:23.000000 airbyte-source-opsgenie-0.3.1/airbyte_source_opsgenie.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-16 20:11:23.000000 airbyte-source-opsgenie-0.3.1/airbyte_source_opsgenie.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2024-02-16 20:11:23.000000 airbyte-source-opsgenie-0.3.1/airbyte_source_opsgenie.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       91 2024-02-16 20:11:23.000000 airbyte-source-opsgenie-0.3.1/airbyte_source_opsgenie.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       34 2024-02-16 20:11:23.000000 airbyte-source-opsgenie-0.3.1/airbyte_source_opsgenie.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 20:11:23.166480 airbyte-source-opsgenie-0.3.1/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-02-16 19:40:33.000000 airbyte-source-opsgenie-0.3.1/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      229 2024-02-16 19:40:33.000000 airbyte-source-opsgenie-0.3.1/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      258 2024-02-16 19:40:33.000000 airbyte-source-opsgenie-0.3.1/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     2623 2024-02-16 19:40:33.000000 airbyte-source-opsgenie-0.3.1/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)      114 2024-02-16 19:40:33.000000 airbyte-source-opsgenie-0.3.1/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)      107 2024-02-16 19:40:33.000000 airbyte-source-opsgenie-0.3.1/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)      229 2024-02-16 19:40:33.000000 airbyte-source-opsgenie-0.3.1/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     4607 2024-02-16 20:11:23.170480 airbyte-source-opsgenie-0.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      940 2024-02-16 20:11:21.000000 airbyte-source-opsgenie-0.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 20:11:23.170480 airbyte-source-opsgenie-0.3.1/source_opsgenie/
--rw-r--r--   0 root         (0) root         (0)      128 2024-02-16 19:40:33.000000 airbyte-source-opsgenie-0.3.1/source_opsgenie/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6299 2024-02-16 19:40:33.000000 airbyte-source-opsgenie-0.3.1/source_opsgenie/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      236 2024-02-16 19:40:33.000000 airbyte-source-opsgenie-0.3.1/source_opsgenie/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-16 20:11:23.170480 airbyte-source-opsgenie-0.3.1/source_opsgenie/schemas/
--rw-r--r--   0 root         (0) root         (0)      465 2024-02-16 19:40:33.000000 airbyte-source-opsgenie-0.3.1/source_opsgenie/schemas/alert_logs.json
--rw-r--r--   0 root         (0) root         (0)      622 2024-02-16 19:40:33.000000 airbyte-source-opsgenie-0.3.1/source_opsgenie/schemas/alert_recipients.json
--rw-r--r--   0 root         (0) root         (0)     3319 2024-02-16 19:40:33.000000 airbyte-source-opsgenie-0.3.1/source_opsgenie/schemas/alerts.json
--rw-r--r--   0 root         (0) root         (0)     1593 2024-02-16 19:40:33.000000 airbyte-source-opsgenie-0.3.1/source_opsgenie/schemas/incidents.json
--rw-r--r--   0 root         (0) root         (0)      523 2024-02-16 19:40:33.000000 airbyte-source-opsgenie-0.3.1/source_opsgenie/schemas/integrations.json
--rw-r--r--   0 root         (0) root         (0)      704 2024-02-16 19:40:33.000000 airbyte-source-opsgenie-0.3.1/source_opsgenie/schemas/services.json
--rw-r--r--   0 root         (0) root         (0)      483 2024-02-16 19:40:33.000000 airbyte-source-opsgenie-0.3.1/source_opsgenie/schemas/teams.json
--rw-r--r--   0 root         (0) root         (0)      264 2024-02-16 19:40:33.000000 airbyte-source-opsgenie-0.3.1/source_opsgenie/schemas/user_teams.json
--rw-r--r--   0 root         (0) root         (0)     1583 2024-02-16 19:40:33.000000 airbyte-source-opsgenie-0.3.1/source_opsgenie/schemas/users.json
--rw-r--r--   0 root         (0) root         (0)      476 2024-02-16 19:40:33.000000 airbyte-source-opsgenie-0.3.1/source_opsgenie/source.py
--rw-r--r--   0 root         (0) root         (0)     1009 2024-02-16 19:40:33.000000 airbyte-source-opsgenie-0.3.1/source_opsgenie/spec.yaml
+-rw-r--r--   0        0        0     4532 2024-05-01 19:00:52.928049 airbyte_source_opsgenie-0.3.5/README.md
+-rw-r--r--   0        0        0      777 2024-05-01 19:04:17.310850 airbyte_source_opsgenie-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      128 2024-05-01 19:00:52.928049 airbyte_source_opsgenie-0.3.5/source_opsgenie/__init__.py
+-rw-r--r--   0        0        0    27750 2024-05-01 19:00:52.928049 airbyte_source_opsgenie-0.3.5/source_opsgenie/manifest.yaml
+-rw-r--r--   0        0        0      236 2024-05-01 19:00:52.928049 airbyte_source_opsgenie-0.3.5/source_opsgenie/run.py
+-rw-r--r--   0        0        0      476 2024-05-01 19:00:52.928049 airbyte_source_opsgenie-0.3.5/source_opsgenie/source.py
+-rw-r--r--   0        0        0     1009 2024-05-01 19:00:52.928049 airbyte_source_opsgenie-0.3.5/source_opsgenie/spec.yaml
+-rw-r--r--   0        0        0     5242 1970-01-01 00:00:00.000000 airbyte_source_opsgenie-0.3.5/PKG-INFO
```

### Comparing `airbyte-source-opsgenie-0.3.1/README.md` & `airbyte_source_opsgenie-0.3.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,83 +1,91 @@
-# Opsgenie Source
+# Opsgenie source connector
 
-This is the repository for the Opsgenie source connector, written in low-code configuration based source connector.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/opsgenie).
+
+This is the repository for the Opsgenie source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/opsgenie).
 
 ## Local development
 
-#### Building via Gradle
-You can also build the connector in Gradle. This is typically used in CI and not needed for your development workflow.
+### Prerequisites
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-To build using Gradle, from the Airbyte repository root, run:
-```
-./gradlew :airbyte-integrations:connectors:source-opsgenie:build
+
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
 ```
 
-#### Create credentials
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/opsgenie)
+
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/opsgenie)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_opsgenie/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source opsgenie test creds`
-and place them into `secrets/config.json`.
 
 ### Locally running the connector
 ```
-python main.py spec
-python main.py check --config secrets/config.json
-python main.py discover --config secrets/config.json
-python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-opsgenie spec
+poetry run source-opsgenie check --config secrets/config.json
+poetry run source-opsgenie discover --config secrets/config.json
+poetry run source-opsgenie read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
-### Locally running the connector docker image
-
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
 airbyte-ci connectors --name=source-opsgenie build
 ```
 
-An image will be built with the tag `airbyte/source-opsgenie:dev`.
+An image will be available on your host with the tag `airbyte/source-opsgenie:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-opsgenie:dev .
-```
 
-#### Run
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-opsgenie:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-opsgenie:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-opsgenie:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-opsgenie:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-## Testing
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-opsgenie test
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
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
-### Publishing a new version of the connector
+## Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-opsgenie test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/opsgenie.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/opsgenie.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-opsgenie-0.3.1/setup.cfg` & `airbyte_source_opsgenie-0.3.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,82 +1,110 @@
-[metadata]
-name = airbyte-source-opsgenie
-version = 0.3.1
-author = Airbyte
-author_email = contact@airbyte.io
-long_description = # Opsgenie Source
-	
-	This is the repository for the Opsgenie source connector, written in low-code configuration based source connector.
-	For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/opsgenie).
-	
-	
-	You can also build the connector in Gradle. This is typically used in CI and not needed for your development workflow.
-	
-	To build using Gradle, from the Airbyte repository root, run:
-	```
-	./gradlew :airbyte-integrations:connectors:source-opsgenie:build
-	```
-	
-	**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/opsgenie)
-	to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_opsgenie/spec.yaml` file.
-	Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-	See `integration_tests/sample_config.json` for a sample config file.
-	
-	**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source opsgenie test creds`
-	and place them into `secrets/config.json`.
-	
-	```
-	python main.py spec
-	python main.py check --config secrets/config.json
-	python main.py discover --config secrets/config.json
-	python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
-	```
-	
-	
-	
-	**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
-	```bash
-	airbyte-ci connectors --name=source-opsgenie build
-	```
-	
-	An image will be built with the tag `airbyte/source-opsgenie:dev`.
-	
-	**Via `docker build`:**
-	```bash
-	docker build -t airbyte/source-opsgenie:dev .
-	```
-	
-	Then run any of the connector commands as follows:
-	```
-	docker run --rm airbyte/source-opsgenie:dev spec
-	docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-opsgenie:dev check --config /secrets/config.json
-	docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-opsgenie:dev discover --config /secrets/config.json
-	docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-opsgenie:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
-	```
-	
-	You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
-	```bash
-	airbyte-ci connectors --name=source-opsgenie test
-	```
-	
-	Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
-	If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
-	
-	All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-	We split dependencies between two groups, dependencies that are:
-	* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-	* required for the testing need to go to `TEST_REQUIREMENTS` list
-	
-	You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
-	1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-opsgenie test`
-	2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
-	3. Make sure the `metadata.yaml` content is up to date.
-	4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/opsgenie.md`).
-	5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
-	6. Pat yourself on the back for being an awesome contributor.
-	7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-long_description_content_type = text/markdown
-
-[egg_info]
-tag_build = 
-tag_date = 0
+Metadata-Version: 2.1
+Name: airbyte-source-opsgenie
+Version: 0.3.5
+Summary: Source implementation for Opsgenie.
+Home-page: https://airbyte.com
+License: MIT
+Author: Airbyte
+Author-email: contact@airbyte.io
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: airbyte-cdk (==0.80.0)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/opsgenie
+Project-URL: Repository, https://github.com/airbytehq/airbyte
+Description-Content-Type: text/markdown
 
+# Opsgenie source connector
+
+
+This is the repository for the Opsgenie source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/opsgenie).
+
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
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/opsgenie)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_opsgenie/spec.yaml` file.
+Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
+See `sample_files/sample_config.json` for a sample config file.
+
+
+### Locally running the connector
+```
+poetry run source-opsgenie spec
+poetry run source-opsgenie check --config secrets/config.json
+poetry run source-opsgenie discover --config secrets/config.json
+poetry run source-opsgenie read --config secrets/config.json --catalog sample_files/configured_catalog.json
+```
+
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
+
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
+```bash
+airbyte-ci connectors --name=source-opsgenie build
+```
+
+An image will be available on your host with the tag `airbyte/source-opsgenie:dev`.
+
+
+### Running as a docker container
+Then run any of the connector commands as follows:
+```
+docker run --rm airbyte/source-opsgenie:dev spec
+docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-opsgenie:dev check --config /secrets/config.json
+docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-opsgenie:dev discover --config /secrets/config.json
+docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-opsgenie:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
+```
+
+### Running our CI test suite
+You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+```bash
+airbyte-ci connectors --name=source-opsgenie test
+```
+
+### Customizing acceptance Tests
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
+
+### Dependency Management
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
+
+## Publishing a new version of the connector
+You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-opsgenie test`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
+3. Make sure the `metadata.yaml` content is up to date.
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/opsgenie.md`).
+5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
+6. Pat yourself on the back for being an awesome contributor.
+7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-opsgenie-0.3.1/source_opsgenie/spec.yaml` & `airbyte_source_opsgenie-0.3.5/source_opsgenie/spec.yaml`

 * *Files identical despite different names*


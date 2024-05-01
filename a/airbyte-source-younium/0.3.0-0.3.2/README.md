# Comparing `tmp/airbyte-source-younium-0.3.0.tar.gz` & `tmp/airbyte_source_younium-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-younium-0.3.0.tar", last modified: Thu Feb  1 09:41:05 2024, max compression
+gzip compressed data, was "airbyte_source_younium-0.3.2.tar", max compression
```

## Comparing `airbyte-source-younium-0.3.0.tar` & `airbyte_source_younium-0.3.2.tar`

### file list

```diff
@@ -1,32 +1,8 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:41:05.184661 airbyte-source-younium-0.3.0/
--rw-r--r--   0 root         (0) root         (0)     4402 2024-02-01 09:41:05.184661 airbyte-source-younium-0.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4230 2024-02-01 09:38:30.000000 airbyte-source-younium-0.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:41:05.180662 airbyte-source-younium-0.3.0/airbyte_source_younium.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4402 2024-02-01 09:41:05.000000 airbyte-source-younium-0.3.0/airbyte_source_younium.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      876 2024-02-01 09:41:05.000000 airbyte-source-younium-0.3.0/airbyte_source_younium.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-01 09:41:05.000000 airbyte-source-younium-0.3.0/airbyte_source_younium.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2024-02-01 09:41:05.000000 airbyte-source-younium-0.3.0/airbyte_source_younium.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-01 09:41:05.000000 airbyte-source-younium-0.3.0/airbyte_source_younium.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-02-01 09:41:05.000000 airbyte-source-younium-0.3.0/airbyte_source_younium.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:41:05.180662 airbyte-source-younium-0.3.0/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-02-01 09:38:30.000000 airbyte-source-younium-0.3.0/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2024-02-01 09:38:30.000000 airbyte-source-younium-0.3.0/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-02-01 09:38:30.000000 airbyte-source-younium-0.3.0/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     1132 2024-02-01 09:38:30.000000 airbyte-source-younium-0.3.0/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)      145 2024-02-01 09:38:30.000000 airbyte-source-younium-0.3.0/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)      109 2024-02-01 09:38:30.000000 airbyte-source-younium-0.3.0/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)       63 2024-02-01 09:38:30.000000 airbyte-source-younium-0.3.0/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     4270 2024-02-01 09:41:05.184661 airbyte-source-younium-0.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      919 2024-02-01 09:41:02.000000 airbyte-source-younium-0.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:41:05.180662 airbyte-source-younium-0.3.0/source_younium/
--rw-r--r--   0 root         (0) root         (0)      126 2024-02-01 09:38:30.000000 airbyte-source-younium-0.3.0/source_younium/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3591 2024-02-01 09:38:30.000000 airbyte-source-younium-0.3.0/source_younium/components.py
--rw-r--r--   0 root         (0) root         (0)     3132 2024-02-01 09:38:30.000000 airbyte-source-younium-0.3.0/source_younium/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      233 2024-02-01 09:38:30.000000 airbyte-source-younium-0.3.0/source_younium/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:41:05.180662 airbyte-source-younium-0.3.0/source_younium/schemas/
--rw-r--r--   0 root         (0) root         (0)     4683 2024-02-01 09:38:30.000000 airbyte-source-younium-0.3.0/source_younium/schemas/account.json
--rw-r--r--   0 root         (0) root         (0)     7405 2024-02-01 09:38:30.000000 airbyte-source-younium-0.3.0/source_younium/schemas/booking.json
--rw-r--r--   0 root         (0) root         (0)     9235 2024-02-01 09:38:30.000000 airbyte-source-younium-0.3.0/source_younium/schemas/invoice.json
--rw-r--r--   0 root         (0) root         (0)     5039 2024-02-01 09:38:30.000000 airbyte-source-younium-0.3.0/source_younium/schemas/product.json
--rw-r--r--   0 root         (0) root         (0)    23044 2024-02-01 09:38:30.000000 airbyte-source-younium-0.3.0/source_younium/schemas/subscription.json
--rw-r--r--   0 root         (0) root         (0)      476 2024-02-01 09:38:30.000000 airbyte-source-younium-0.3.0/source_younium/source.py
+-rw-r--r--   0        0        0     4514 2024-05-01 18:26:35.304865 airbyte_source_younium-0.3.2/README.md
+-rw-r--r--   0        0        0      749 2024-05-01 18:30:08.688631 airbyte_source_younium-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      126 2024-05-01 18:26:35.304865 airbyte_source_younium-0.3.2/source_younium/__init__.py
+-rw-r--r--   0        0        0     3591 2024-05-01 18:26:35.304865 airbyte_source_younium-0.3.2/source_younium/components.py
+-rw-r--r--   0        0        0   104754 2024-05-01 18:26:35.308865 airbyte_source_younium-0.3.2/source_younium/manifest.yaml
+-rw-r--r--   0        0        0      233 2024-05-01 18:26:35.308865 airbyte_source_younium-0.3.2/source_younium/run.py
+-rw-r--r--   0        0        0      476 2024-05-01 18:26:35.308865 airbyte_source_younium-0.3.2/source_younium/source.py
+-rw-r--r--   0        0        0     5221 1970-01-01 00:00:00.000000 airbyte_source_younium-0.3.2/PKG-INFO
```

### Comparing `airbyte-source-younium-0.3.0/PKG-INFO` & `airbyte_source_younium-0.3.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,91 @@
-Metadata-Version: 2.1
-Name: airbyte-source-younium
-Version: 0.3.0
-Summary: Source implementation for Younium.
-Author: Airbyte
-Author-email: contact@airbyte.io
-Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.2; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
+# Younium source connector
 
-# Zapier Supported Storage Source
 
-This is the repository for the Zapier Supported Storage configuration based source connector.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/zapier-supported-storage).
+This is the repository for the Younium source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/younium).
 
+## Local development
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/zapier-supported-storage)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_zapier_supported_storage/spec.yaml` file.
-Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+### Prerequisites
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source zapier-supported-storage test creds`
-and place them into `secrets/config.json`.
 
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
+```
 
 
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
-```bash
-airbyte-ci connectors --name source-zapier-supported-storage build
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/younium)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_younium/spec.yaml` file.
+Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
+See `sample_files/sample_config.json` for a sample config file.
+
+
+### Locally running the connector
+```
+poetry run source-younium spec
+poetry run source-younium check --config secrets/config.json
+poetry run source-younium discover --config secrets/config.json
+poetry run source-younium read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
-An image will be built with the tag `airbyte/source-zapier-supported-storage:dev`.
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-**Via `docker build`:**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
-docker build -t airbyte/source-zapier-supported-storage:dev .
+airbyte-ci connectors --name=source-younium build
 ```
 
+An image will be available on your host with the tag `airbyte/source-younium:dev`.
+
+
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
-docker run --rm airbyte/source-zapier-supported-storage:dev spec
-docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-zapier-supported-storage:dev check --config /secrets/config.json
-docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-zapier-supported-storage:dev discover --config /secrets/config.json
-docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-zapier-supported-storage:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
+docker run --rm airbyte/source-younium:dev spec
+docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-younium:dev check --config /secrets/config.json
+docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-younium:dev discover --config /secrets/config.json
+docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-younium:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-younium test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-younium test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/younium.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/younium.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-younium-0.3.0/source_younium/components.py` & `airbyte_source_younium-0.3.2/source_younium/components.py`

 * *Files identical despite different names*


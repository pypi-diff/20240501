# Comparing `tmp/airbyte-source-outreach-0.5.0.tar.gz` & `tmp/airbyte_source_outreach-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-outreach-0.5.0.tar", last modified: Wed Jan 31 15:50:18 2024, max compression
+gzip compressed data, was "airbyte_source_outreach-0.5.4.tar", max compression
```

## Comparing `airbyte-source-outreach-0.5.0.tar` & `airbyte_source_outreach-0.5.4.tar`

### file list

```diff
@@ -1,48 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:50:18.155364 airbyte-source-outreach-0.5.0/
--rw-r--r--   0 root         (0) root         (0)     5403 2024-01-31 15:50:18.155364 airbyte-source-outreach-0.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5395 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:50:18.151364 airbyte-source-outreach-0.5.0/airbyte_source_outreach.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5403 2024-01-31 15:50:18.000000 airbyte-source-outreach-0.5.0/airbyte_source_outreach.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1454 2024-01-31 15:50:18.000000 airbyte-source-outreach-0.5.0/airbyte_source_outreach.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-31 15:50:18.000000 airbyte-source-outreach-0.5.0/airbyte_source_outreach.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2024-01-31 15:50:18.000000 airbyte-source-outreach-0.5.0/airbyte_source_outreach.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-01-31 15:50:18.000000 airbyte-source-outreach-0.5.0/airbyte_source_outreach.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       45 2024-01-31 15:50:18.000000 airbyte-source-outreach-0.5.0/airbyte_source_outreach.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:50:18.147364 airbyte-source-outreach-0.5.0/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1065 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      314 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     7697 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)      219 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)      325 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)     1063 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     5299 2024-01-31 15:50:18.155364 airbyte-source-outreach-0.5.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      922 2024-01-31 15:50:16.000000 airbyte-source-outreach-0.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:50:18.147364 airbyte-source-outreach-0.5.0/source_outreach/
--rw-r--r--   0 root         (0) root         (0)      128 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/source_outreach/__init__.py
--rw-r--r--   0 root         (0) root         (0)      236 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/source_outreach/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:50:18.151364 airbyte-source-outreach-0.5.0/source_outreach/schemas/
--rw-r--r--   0 root         (0) root         (0)    11462 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/source_outreach/schemas/accounts.json
--rw-r--r--   0 root         (0) root         (0)      831 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/source_outreach/schemas/call_dispositions.json
--rw-r--r--   0 root         (0) root         (0)      696 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/source_outreach/schemas/call_purposes.json
--rw-r--r--   0 root         (0) root         (0)     3206 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/source_outreach/schemas/calls.json
--rw-r--r--   0 root         (0) root         (0)     4253 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/source_outreach/schemas/mailboxes.json
--rw-r--r--   0 root         (0) root         (0)     5273 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/source_outreach/schemas/mailings.json
--rw-r--r--   0 root         (0) root         (0)    11815 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/source_outreach/schemas/opportunities.json
--rw-r--r--   0 root         (0) root         (0)      587 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/source_outreach/schemas/personas.json
--rw-r--r--   0 root         (0) root         (0)    19271 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/source_outreach/schemas/prospects.json
--rw-r--r--   0 root         (0) root         (0)     3036 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/source_outreach/schemas/sequence_states.json
--rw-r--r--   0 root         (0) root         (0)     2419 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/source_outreach/schemas/sequence_steps.json
--rw-r--r--   0 root         (0) root         (0)     4308 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/source_outreach/schemas/sequences.json
--rw-r--r--   0 root         (0) root         (0)     1124 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/source_outreach/schemas/snippets.json
--rw-r--r--   0 root         (0) root         (0)      873 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/source_outreach/schemas/stages.json
--rw-r--r--   0 root         (0) root         (0)     4542 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/source_outreach/schemas/tasks.json
--rw-r--r--   0 root         (0) root         (0)     2678 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/source_outreach/schemas/templates.json
--rw-r--r--   0 root         (0) root         (0)     9190 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/source_outreach/schemas/users.json
--rw-r--r--   0 root         (0) root         (0)    11011 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/source_outreach/source.py
--rw-r--r--   0 root         (0) root         (0)     1684 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/source_outreach/spec.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 15:50:18.151364 airbyte-source-outreach-0.5.0/unit_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/unit_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2161 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/unit_tests/test_incremental_streams.py
--rw-r--r--   0 root         (0) root         (0)      363 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/unit_tests/test_source.py
--rw-r--r--   0 root         (0) root         (0)     2897 2024-01-31 15:33:11.000000 airbyte-source-outreach-0.5.0/unit_tests/test_streams.py
+-rw-r--r--   0        0        0     4532 2024-05-01 18:15:32.081971 airbyte_source_outreach-0.5.4/README.md
+-rw-r--r--   0        0        0      755 2024-05-01 18:23:46.562435 airbyte_source_outreach-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0      128 2024-05-01 18:15:32.081971 airbyte_source_outreach-0.5.4/source_outreach/__init__.py
+-rw-r--r--   0        0        0      236 2024-05-01 18:15:32.081971 airbyte_source_outreach-0.5.4/source_outreach/run.py
+-rw-r--r--   0        0        0    19492 2024-05-01 18:15:32.081971 airbyte_source_outreach-0.5.4/source_outreach/schemas/accounts.json
+-rw-r--r--   0        0        0     1509 2024-05-01 18:15:32.081971 airbyte_source_outreach-0.5.4/source_outreach/schemas/call_dispositions.json
+-rw-r--r--   0        0        0     1240 2024-05-01 18:15:32.081971 airbyte_source_outreach-0.5.4/source_outreach/schemas/call_purposes.json
+-rw-r--r--   0        0        0     5480 2024-05-01 18:15:32.081971 airbyte_source_outreach-0.5.4/source_outreach/schemas/calls.json
+-rw-r--r--   0        0        0     8487 2024-05-01 18:15:32.081971 airbyte_source_outreach-0.5.4/source_outreach/schemas/mailboxes.json
+-rw-r--r--   0        0        0     9190 2024-05-01 18:15:32.081971 airbyte_source_outreach-0.5.4/source_outreach/schemas/mailings.json
+-rw-r--r--   0        0        0    20237 2024-05-01 18:15:32.081971 airbyte_source_outreach-0.5.4/source_outreach/schemas/opportunities.json
+-rw-r--r--   0        0        0      996 2024-05-01 18:15:32.081971 airbyte_source_outreach-0.5.4/source_outreach/schemas/personas.json
+-rw-r--r--   0        0        0    20075 2024-05-01 18:15:32.081971 airbyte_source_outreach-0.5.4/source_outreach/schemas/prospects.json
+-rw-r--r--   0        0        0     5059 2024-05-01 18:15:32.081971 airbyte_source_outreach-0.5.4/source_outreach/schemas/sequence_states.json
+-rw-r--r--   0        0        0     4726 2024-05-01 18:15:32.081971 airbyte_source_outreach-0.5.4/source_outreach/schemas/sequence_steps.json
+-rw-r--r--   0        0        0     7948 2024-05-01 18:15:32.081971 airbyte_source_outreach-0.5.4/source_outreach/schemas/sequences.json
+-rw-r--r--   0        0        0     1884 2024-05-01 18:15:32.081971 airbyte_source_outreach-0.5.4/source_outreach/schemas/snippets.json
+-rw-r--r--   0        0        0     1499 2024-05-01 18:15:32.081971 airbyte_source_outreach-0.5.4/source_outreach/schemas/stages.json
+-rw-r--r--   0        0        0     7737 2024-05-01 18:15:32.081971 airbyte_source_outreach-0.5.4/source_outreach/schemas/tasks.json
+-rw-r--r--   0        0        0     5201 2024-05-01 18:15:32.081971 airbyte_source_outreach-0.5.4/source_outreach/schemas/templates.json
+-rw-r--r--   0        0        0    17728 2024-05-01 18:15:32.081971 airbyte_source_outreach-0.5.4/source_outreach/schemas/users.json
+-rw-r--r--   0        0        0    11011 2024-05-01 18:15:32.081971 airbyte_source_outreach-0.5.4/source_outreach/source.py
+-rw-r--r--   0        0        0     1684 2024-05-01 18:15:32.081971 airbyte_source_outreach-0.5.4/source_outreach/spec.json
+-rw-r--r--   0        0        0     5242 1970-01-01 00:00:00.000000 airbyte_source_outreach-0.5.4/PKG-INFO
```

### Comparing `airbyte-source-outreach-0.5.0/PKG-INFO` & `airbyte_source_outreach-0.5.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,99 +1,110 @@
 Metadata-Version: 2.1
 Name: airbyte-source-outreach
-Version: 0.5.0
+Version: 0.5.4
 Summary: Source implementation for Outreach.
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
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/outreach
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.1; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
 
-# Outreach Source
+# Outreach source connector
 
-This is the repository for the Outreach source connector, written in Python.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/outreach).
 
+This is the repository for the Outreach source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/outreach).
 
-**To iterate on this connector, make sure to complete this prerequisites section.**
+## Local development
 
+### Prerequisites
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-From this connector directory, create a virtual environment:
-```
-python -m venv .venv
-```
 
-This will generate a virtualenv for this module in `.venv/`. Make sure this venv is active in your
-development environment of choice. To activate it from the terminal, run:
-```
-source .venv/bin/activate
-pip install -r requirements.txt
-pip install '.[tests]'
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
 ```
-If you are in an IDE, follow your IDE's instructions to activate the virtualenv.
 
-Note that while we are installing dependencies from `requirements.txt`, you should only edit `setup.py` for your dependencies. `requirements.txt` is
-used for editable installs (`pip install -e`) to pull in Python dependencies from the monorepo and will call `setup.py`.
-If this is mumbo jumbo to you, don't worry about it, just put your deps in `setup.py` but install using `pip install -r requirements.txt` and everything
-should work as you expect.
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/outreach)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_outreach/spec.json` file.
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/outreach)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_outreach/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source outreach test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
 ```
-python main.py spec
-python main.py check --config secrets/config.json
-python main.py discover --config secrets/config.json
-python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-outreach spec
+poetry run source-outreach check --config secrets/config.json
+poetry run source-outreach discover --config secrets/config.json
+poetry run source-outreach read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-outreach build
 ```
 
-An image will be built with the tag `airbyte/source-outreach:dev`.
+An image will be available on your host with the tag `airbyte/source-outreach:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-outreach:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-outreach:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-outreach:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-outreach:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-outreach:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-outreach test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-outreach test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/outreach.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/outreach.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-outreach-0.5.0/README.md` & `airbyte_source_outreach-0.5.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,100 +1,91 @@
-# Outreach Source
+# Outreach source connector
+
 
 This is the repository for the Outreach source connector, written in Python.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/outreach).
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/outreach).
 
 ## Local development
 
 ### Prerequisites
-**To iterate on this connector, make sure to complete this prerequisites section.**
-
-#### Minimum Python version required `= 3.7.0`
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
-#### Build & Activate Virtual Environment and install dependencies
-From this connector directory, create a virtual environment:
-```
-python -m venv .venv
-```
 
-This will generate a virtualenv for this module in `.venv/`. Make sure this venv is active in your
-development environment of choice. To activate it from the terminal, run:
-```
-source .venv/bin/activate
-pip install -r requirements.txt
-pip install '.[tests]'
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
 ```
-If you are in an IDE, follow your IDE's instructions to activate the virtualenv.
 
-Note that while we are installing dependencies from `requirements.txt`, you should only edit `setup.py` for your dependencies. `requirements.txt` is
-used for editable installs (`pip install -e`) to pull in Python dependencies from the monorepo and will call `setup.py`.
-If this is mumbo jumbo to you, don't worry about it, just put your deps in `setup.py` but install using `pip install -r requirements.txt` and everything
-should work as you expect.
 
-#### Create credentials
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/outreach)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_outreach/spec.json` file.
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/outreach)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_outreach/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source outreach test creds`
-and place them into `secrets/config.json`.
 
 ### Locally running the connector
 ```
-python main.py spec
-python main.py check --config secrets/config.json
-python main.py discover --config secrets/config.json
-python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-outreach spec
+poetry run source-outreach check --config secrets/config.json
+poetry run source-outreach discover --config secrets/config.json
+poetry run source-outreach read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-outreach build
 ```
 
-An image will be built with the tag `airbyte/source-outreach:dev`.
+An image will be available on your host with the tag `airbyte/source-outreach:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-outreach:dev .
-```
 
-#### Run
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-outreach:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-outreach:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-outreach:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-outreach:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
-## Testing
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-outreach test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-outreach test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/outreach.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/outreach.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-outreach-0.5.0/source_outreach/schemas/mailings.json` & `airbyte_source_outreach-0.5.4/source_outreach/schemas/sequence_states.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8936471193415638%*

 * *Differences: {"'properties'": "{'id': {'description': 'Unique identifier for the sequence state'}, "*

 * *                 "'clickCount': {'description': 'Number of link clicks in emails sent'}, "*

 * *                 "'errorReason': {'description': 'Reason for any errors encountered'}, "*

 * *                 "'openCount': {'description': 'Count of email opens'}, 'repliedAt': "*

 * *                 "{'description': 'Timestamp when a reply was sent'}, 'state': {'description': "*

 * *                 "'Current state of the sequence'}, 'stateCh […]*

```diff
@@ -1,471 +1,313 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "additionalProperties": true,
     "properties": {
-        "attachments": {
+        "account": {
+            "description": "Account associated with the sequence state",
+            "items": {
+                "type": [
+                    "null",
+                    "integer"
+                ]
+            },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "attributableSequenceId": {
+        "activeAt": {
+            "description": "Timestamp when the sequence state became active",
+            "format": "date-time",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "attributableSequenceName": {
+        "activeStepMailings": {
+            "description": "Mailings related to the currently active step",
+            "items": {
+                "type": [
+                    "null",
+                    "integer"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         },
-        "bodyHtml": {
+        "activeStepTasks": {
+            "description": "Tasks related to the currently active step",
+            "items": {
+                "type": [
+                    "null",
+                    "integer"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         },
-        "bodyText": {
+        "bounceCount": {
+            "description": "Number of bounced emails for the sequence state",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "bouncedAt": {
+        "callCompletedAt": {
+            "description": "Timestamp when the call was completed",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "calendar": {
+        "calls": {
+            "description": "Calls made in relation to the sequence state",
+            "items": {
+                "type": [
+                    "null",
+                    "integer"
+                ]
+            },
             "type": [
                 "null",
                 "array"
             ]
         },
         "clickCount": {
+            "description": "Number of link clicks in emails sent",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "clickedAt": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
         "createdAt": {
+            "description": "Timestamp when the sequence state was created",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "deliveredAt": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "desiredAt": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "errorBacktrace": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "errorReason": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "followUpSequence": {
+        "creator": {
+            "description": "Person who created the sequence state",
             "items": {
                 "type": [
                     "null",
                     "integer"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "followUpSequenceId": {
+        "deliverCount": {
+            "description": "Number of successfully delivered emails",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "followUpSequenceName": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "followUpSequenceStartingDate": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "followUpTaskScheduledAt": {
-            "format": "date-time",
+        "errorReason": {
+            "description": "Reason for any errors encountered",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "followUpTaskType": {
+        "failureCount": {
+            "description": "Count of failed activities",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
         "id": {
+            "description": "Unique identifier for the sequence state",
             "type": "integer"
         },
         "mailbox": {
+            "description": "Mailbox associated with the sequence state",
             "items": {
                 "type": [
                     "null",
                     "integer"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "mailboxAddress": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "mailingType": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "markedAsSpamAt": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "meetingDescription": {
+        "mailings": {
+            "description": "Mailings sent in the sequence",
+            "items": {
+                "type": [
+                    "null",
+                    "integer"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         },
-        "meetingDuration": {
+        "negativeReplyCount": {
+            "description": "Count of negative replies received",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "meetingLocation": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "meetingTitle": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "messageId": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "notifyThreadCondition": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "notifyThreadScheduledAt": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "notifyThreadStatus": {
+        "neutralReplyCount": {
+            "description": "Count of neutral replies received",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
         "openCount": {
+            "description": "Count of email opens",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "openedAt": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
         "opportunity": {
+            "description": "Opportunity linked to the sequence state",
             "items": {
                 "type": [
                     "null",
                     "integer"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "optimizedScheduledAt": {
-            "format": "date-time",
+        "optOutCount": {
+            "description": "Count of opt-outs",
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "overrideSafetySettings": {
+        "pauseReason": {
+            "description": "Reason for pausing the sequence state",
             "type": [
                 "null",
-                "boolean"
+                "string"
             ]
         },
-        "prospect": {
-            "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
-            },
+        "positiveReplyCount": {
+            "description": "Count of positive replies received",
             "type": [
                 "null",
-                "array"
+                "integer"
             ]
         },
-        "recipients": {
+        "prospect": {
+            "description": "Prospect associated with the sequence state",
             "items": {
                 "type": [
                     "null",
                     "integer"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "references": {
-            "type": [
-                "null",
-                "array"
-            ]
-        },
         "repliedAt": {
+            "description": "Timestamp when a reply was sent",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "replySentiment": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "retryAt": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "retryCount": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "retryInterval": {
+        "replyCount": {
+            "description": "Total number of replies received",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "schedule": {
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "scheduleId": {
+        "scheduleCount": {
+            "description": "Count of scheduled activities",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "scheduledAt": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
         "sequence": {
-            "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "sequenceState": {
+            "description": "Sequence that the state is part of",
             "items": {
                 "type": [
                     "null",
                     "integer"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
         "sequenceStep": {
+            "description": "Current step within the sequence",
             "items": {
                 "type": [
                     "null",
                     "integer"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
         "state": {
+            "description": "Current state of the sequence",
             "type": [
                 "null",
                 "string"
             ]
         },
         "stateChangedAt": {
+            "description": "Timestamp when the state changed",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "subject": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "task": {
-            "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
         "tasks": {
+            "description": "Tasks associated with the sequence state",
             "items": {
                 "type": [
                     "null",
                     "integer"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "template": {
-            "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "trackLinks": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "trackOpens": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "unsubscribedAt": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
         "updatedAt": {
+            "description": "Timestamp when the sequence state was last updated",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
-        },
-        "user": {
-            "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte-source-outreach-0.5.0/source_outreach/schemas/prospects.json` & `airbyte_source_outreach-0.5.4/source_outreach/schemas/prospects.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988468634686347%*

 * *Differences: {"'properties'": "{'touchedAt': {'description': 'Date and time when the prospect was last "*

 * *                 "contacted'}, 'trashedAt': {'description': 'Date and time when the prospect was "*

 * *                 "moved to trash'}, 'trashedByAccount': {'description': 'Details of the account "*

 * *                 'that moved the prospect to trash\'}, \'twitterUrl\': {\'description\': "URL of '*

 * *                 'the prospect\'s Twitter profile"}, \'twitterUsername\': {\'description\': '*

 * *                 "'Username of […]*

```diff
@@ -1752,46 +1752,52 @@
         "title": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "touchedAt": {
+            "description": "Date and time when the prospect was last contacted",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "trashedAt": {
+            "description": "Date and time when the prospect was moved to trash",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "trashedByAccount": {
+            "description": "Details of the account that moved the prospect to trash",
             "type": [
                 "null",
                 "array"
             ]
         },
         "twitterUrl": {
+            "description": "URL of the prospect's Twitter profile",
             "type": [
                 "null",
                 "string"
             ]
         },
         "twitterUsername": {
+            "description": "Username of the prospect on Twitter",
             "type": [
                 "null",
                 "string"
             ]
         },
         "updatedAt": {
+            "description": "Date and time when the prospect data was last updated",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "updater": {
@@ -1803,20 +1809,22 @@
             },
             "type": [
                 "null",
                 "array"
             ]
         },
         "updaterId": {
+            "description": "ID of the user who last updated the prospect information",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "updaterType": {
+            "description": "Type of user who last updated the prospect information",
             "type": [
                 "null",
                 "string"
             ]
         },
         "voipPhones": {
             "items": {
@@ -1824,26 +1832,29 @@
             },
             "type": [
                 "null",
                 "array"
             ]
         },
         "websiteUrl1": {
+            "description": "First website URL associated with the prospect",
             "type": [
                 "null",
                 "string"
             ]
         },
         "websiteUrl2": {
+            "description": "Second website URL associated with the prospect",
             "type": [
                 "null",
                 "string"
             ]
         },
         "websiteUrl3": {
+            "description": "Third website URL associated with the prospect",
             "type": [
                 "null",
                 "string"
             ]
         },
         "workPhones": {
             "items": {
```

### Comparing `airbyte-source-outreach-0.5.0/source_outreach/schemas/sequence_states.json` & `airbyte_source_outreach-0.5.4/source_outreach/schemas/stages.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8856907894736842%*

 * *Differences: {"'properties'": "{'id': {'description': 'The unique identifier of the stage.'}, 'createdAt': "*

 * *                 "{'description': 'The date and time when the stage was created.'}, 'updatedAt': "*

 * *                 "{'description': 'The date and time when the stage was last updated.'}, "*

 * *                 "'creator': {'description': 'Information about the user who created the stage.'}, "*

 * *                 "'name': OrderedDict([('description', 'The name of the stage.'), ('type', "*

 * *                 "['null', 'stri […]*

```diff
@@ -1,280 +1,87 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "additionalProperties": true,
     "properties": {
-        "account": {
-            "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "activeAt": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "activeStepMailings": {
-            "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "activeStepTasks": {
-            "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "bounceCount": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "callCompletedAt": {
-            "format": "date-time",
+        "color": {
+            "description": "The color associated with the stage.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "calls": {
-            "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "clickCount": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
         "createdAt": {
+            "description": "The date and time when the stage was created.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "creator": {
+            "description": "Information about the user who created the stage.",
             "items": {
                 "type": [
                     "null",
                     "integer"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "deliverCount": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "errorReason": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "failureCount": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
         "id": {
+            "description": "The unique identifier of the stage.",
             "type": "integer"
         },
-        "mailbox": {
-            "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "mailings": {
-            "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "negativeReplyCount": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "neutralReplyCount": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "openCount": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "opportunity": {
-            "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "optOutCount": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "pauseReason": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "positiveReplyCount": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "prospect": {
-            "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "repliedAt": {
-            "format": "date-time",
+        "name": {
+            "description": "The name of the stage.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "replyCount": {
+        "order": {
+            "description": "The order or sequence of the stage in the workflow.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "scheduleCount": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "sequence": {
+        "prospects": {
+            "description": "Information about the prospects associated with this stage.",
             "items": {
                 "type": [
                     "null",
                     "integer"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "sequenceStep": {
-            "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "state": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "stateChangedAt": {
+        "updatedAt": {
+            "description": "The date and time when the stage was last updated.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "tasks": {
+        "updater": {
+            "description": "Information about the user who last updated the stage.",
             "items": {
                 "type": [
                     "null",
                     "integer"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
-        },
-        "updatedAt": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte-source-outreach-0.5.0/source_outreach/schemas/sequence_steps.json` & `airbyte_source_outreach-0.5.4/source_outreach/schemas/snippets.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8888888888888888%*

 * *Differences: {"'properties'": "{'id': {'description': 'Unique identifier of the snippet.'}, 'createdAt': "*

 * *                 "{'description': 'The date and time when the snippet was created.'}, 'updatedAt': "*

 * *                 "{'description': 'The date and time when the snippet was last updated.'}, "*

 * *                 "'creator': {'items': {'type': ['null', 'integer']}, 'description': 'The creator "*

 * *                 "of the snippet.'}, 'updater': {'items': {'type': ['null', 'integer']}, "*

 * *                 "'description':  […]*

```diff
@@ -1,206 +1,112 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "additionalProperties": true,
     "properties": {
-        "bounceCount": {
+        "bodyHtml": {
+            "description": "The HTML content body of the snippet.",
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "callPurpose": {
-            "items": {
-                "type": "integer"
-            },
+        "bodyText": {
+            "description": "The plain text content body of the snippet.",
             "type": [
                 "null",
-                "array"
+                "string"
             ]
         },
-        "calls": {
+        "contentCategoryMemberships": {
+            "description": "Categories that the snippet belongs to.",
             "items": {
-                "type": "integer"
+                "type": [
+                    "null",
+                    "integer"
+                ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "clickCount": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
         "createdAt": {
+            "description": "The date and time when the snippet was created.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "creator": {
+            "description": "The creator of the snippet.",
             "items": {
-                "type": "string"
+                "type": [
+                    "null",
+                    "integer"
+                ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "date": {
-            "format": "date",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "deliverCount": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "displayName": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "failureCount": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
         "id": {
+            "description": "Unique identifier of the snippet.",
             "type": "integer"
         },
-        "interval": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "mailings": {
-            "items": {
-                "type": "integer"
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "negativeReplyCount": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "neutralReplyCount": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "openCount": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "optOutCount": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "order": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "positiveReplyCount": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "replyCount": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "scheduleCount": {
+        "name": {
+            "description": "Name or title of the snippet.",
             "type": [
                 "null",
-                "integer"
-            ]
-        },
-        "sequence": {
-            "items": {
-                "type": "integer"
-            },
-            "type": [
-                "null",
-                "array"
+                "string"
             ]
         },
-        "sequenceTemplates": {
+        "owner": {
+            "description": "The owner of the snippet.",
             "items": {
-                "type": "integer"
+                "type": [
+                    "null",
+                    "integer"
+                ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "stepType": {
+        "shareType": {
+            "description": "The share type of the snippet, such as public or private.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "taskAutoDisplay": {
+        "tags": {
+            "description": "Tags associated with the snippet.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "taskPriority": {
-            "items": {
-                "type": "integer"
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "tasks": {
-            "items": {
-                "type": "integer"
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
         "updatedAt": {
+            "description": "The date and time when the snippet was last updated.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "updater": {
+            "description": "The user who last updated the snippet.",
             "items": {
-                "type": "integer"
+                "type": [
+                    "null",
+                    "integer"
+                ]
             },
             "type": [
                 "null",
                 "array"
             ]
         }
     },
```

### Comparing `airbyte-source-outreach-0.5.0/source_outreach/schemas/sequences.json` & `airbyte_source_outreach-0.5.4/source_outreach/schemas/sequence_steps.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9044858870967742%*

 * *Differences: {"'properties'": "{'id': {'description': 'The unique identifier of the sequence step.'}, "*

 * *                 "'bounceCount': {'description': 'The count of bounced emails in the sequence "*

 * *                 "step.'}, 'clickCount': {'description': 'The count of clicks on links in the "*

 * *                 "emails of the sequence step.'}, 'createdAt': {'description': 'The date and time "*

 * *                 "when the sequence step was created.'}, 'deliverCount': {'description': 'The "*

 * *                 "count of succes […]*

```diff
@@ -1,392 +1,235 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "additionalProperties": true,
     "properties": {
-        "automationPercentage": {
+        "bounceCount": {
+            "description": "The count of bounced emails in the sequence step.",
             "type": [
                 "null",
-                "number"
+                "integer"
             ]
         },
-        "bounceCount": {
+        "callPurpose": {
+            "description": "The purpose of the call associated with the sequence step.",
+            "items": {
+                "type": "integer"
+            },
             "type": [
                 "null",
-                "integer"
+                "array"
             ]
         },
         "calls": {
+            "description": "The calls made in the sequence step.",
             "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
+                "type": "integer"
             },
             "type": [
                 "null",
                 "array"
             ]
         },
         "clickCount": {
+            "description": "The count of clicks on links in the emails of the sequence step.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "contentCategoryMemberships": {
-            "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
         "createdAt": {
+            "description": "The date and time when the sequence step was created.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "creator": {
+            "description": "The creator or person responsible for the sequence step.",
             "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
+                "type": "string"
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "deliverCount": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "description": {
+        "date": {
+            "description": "The date associated with the sequence step.",
+            "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "durationInDays": {
+        "deliverCount": {
+            "description": "The count of successfully delivered emails in the sequence step.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "enabled": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "enabledAt": {
-            "format": "date-time",
+        "displayName": {
+            "description": "The display name of the sequence step.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "failureCount": {
+            "description": "The count of failed tasks or steps in the sequence.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "finishOnReply": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
         "id": {
+            "description": "The unique identifier of the sequence step.",
             "type": "integer"
         },
-        "lastUsedAt": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "locked": {
+        "interval": {
+            "description": "The time interval or gap between different steps in the sequence.",
             "type": [
                 "null",
-                "boolean"
-            ]
-        },
-        "lockedAt": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
+                "integer"
             ]
         },
         "mailings": {
+            "description": "The mailings associated with the sequence step.",
             "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
+                "type": "integer"
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "maxActivations": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "name": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
         "negativeReplyCount": {
+            "description": "The count of negative replies received in response to the sequence.",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "neutralReplyCount": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "numContactedProspects": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "numRepliedProspects": {
+            "description": "The count of neutral replies received in response to the sequence.",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "openCount": {
+            "description": "The count of opened emails in the sequence step.",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "optOutCount": {
+            "description": "The count of recipients who opted out of further communication in the sequence step.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "owner": {
-            "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "positiveReplyCount": {
+        "order": {
+            "description": "The order or sequence index of the step in the overall sequence.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "primaryReplyAction": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "primaryReplyPauseDuration": {
+        "positiveReplyCount": {
+            "description": "The count of positive replies received in response to the sequence.",
             "type": [
                 "null",
                 "integer"
             ]
         },
         "replyCount": {
+            "description": "The total count of replies received in response to the sequence.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "ruleset": {
-            "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
-        "schedule": {
-            "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
         "scheduleCount": {
+            "description": "The count of scheduled tasks or steps in the sequence.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "scheduleIntervalType": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "secondaryReplyAction": {
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "secondaryReplyPauseDuration": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "sequenceStates": {
+        "sequence": {
+            "description": "The sequence associated with the step.",
             "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
+                "type": "integer"
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "sequenceStepCount": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "sequenceSteps": {
+        "sequenceTemplates": {
+            "description": "The templates associated with the sequence step.",
             "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
+                "type": "integer"
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "sequenceType": {
+        "stepType": {
+            "description": "The type or category of the sequence step.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "shareType": {
+        "taskAutoDisplay": {
+            "description": "Flag indicating if tasks in the step are automatically displayed.",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "tags": {
+        "taskPriority": {
+            "description": "The priority level of tasks associated with the sequence step.",
             "items": {
-                "type": [
-                    "null",
-                    "string"
-                ]
+                "type": "integer"
             },
             "type": [
                 "null",
                 "array"
             ]
         },
         "tasks": {
+            "description": "The tasks associated with the sequence step.",
             "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
+                "type": "integer"
             },
             "type": [
                 "null",
                 "array"
             ]
         },
-        "throttleCapacity": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "throttleMaxAddsPerDay": {
-            "type": [
-                "null",
-                "integer"
-            ]
-        },
-        "throttlePaused": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
-        "throttlePausedAt": {
-            "format": "date-time",
-            "type": [
-                "null",
-                "string"
-            ]
-        },
-        "transactional": {
-            "type": [
-                "null",
-                "boolean"
-            ]
-        },
         "updatedAt": {
+            "description": "The date and time when the sequence step was last updated.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "updater": {
+            "description": "The user who last updated the sequence step.",
             "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
+                "type": "integer"
             },
             "type": [
                 "null",
                 "array"
             ]
         }
     },
```

### Comparing `airbyte-source-outreach-0.5.0/source_outreach/schemas/stages.json` & `airbyte_source_outreach-0.5.4/source_outreach/schemas/call_purposes.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.934375%*

 * *Differences: {"'properties'": "{'id': {'description': 'A unique identifier for the call purpose data.'}, "*

 * *                 "'name': {'description': 'The name or title of the call purpose.'}, 'order': "*

 * *                 "{'description': 'The order in which this call purpose appears in a list or "*

 * *                 "sequence.'}, 'createdAt': {'description': 'The date and time when the call "*

 * *                 "purpose data was created.'}, 'updatedAt': {'description': 'The date and time "*

 * *                 "when the call pur […]*

```diff
@@ -1,78 +1,67 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "additionalProperties": true,
     "properties": {
-        "color": {
+        "calls": {
+            "description": "List of call purposes associated with this data object.",
+            "items": {
+                "type": [
+                    "null",
+                    "integer"
+                ]
+            },
             "type": [
                 "null",
-                "string"
+                "array"
             ]
         },
         "createdAt": {
+            "description": "The date and time when the call purpose data was created.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "creator": {
+            "description": "The user who created this call purpose data.",
             "items": {
                 "type": [
                     "null",
                     "integer"
                 ]
             },
             "type": [
                 "null",
                 "array"
             ]
         },
         "id": {
+            "description": "A unique identifier for the call purpose data.",
             "type": "integer"
         },
         "name": {
+            "description": "The name or title of the call purpose.",
             "type": [
                 "null",
                 "string"
             ]
         },
         "order": {
+            "description": "The order in which this call purpose appears in a list or sequence.",
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "prospects": {
-            "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
-        },
         "updatedAt": {
+            "description": "The date and time when the call purpose data was last updated.",
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
-        },
-        "updater": {
-            "items": {
-                "type": [
-                    "null",
-                    "integer"
-                ]
-            },
-            "type": [
-                "null",
-                "array"
-            ]
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte-source-outreach-0.5.0/source_outreach/source.py` & `airbyte_source_outreach-0.5.4/source_outreach/source.py`

 * *Files identical despite different names*

### Comparing `airbyte-source-outreach-0.5.0/source_outreach/spec.json` & `airbyte_source_outreach-0.5.4/source_outreach/spec.json`

 * *Files identical despite different names*


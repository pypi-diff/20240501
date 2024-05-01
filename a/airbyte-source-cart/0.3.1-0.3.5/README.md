# Comparing `tmp/airbyte-source-cart-0.3.1.tar.gz` & `tmp/airbyte_source_cart-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-cart-0.3.1.tar", last modified: Tue Jan 30 14:42:14 2024, max compression
+gzip compressed data, was "airbyte_source_cart-0.3.5.tar", max compression
```

## Comparing `airbyte-source-cart-0.3.1.tar` & `airbyte_source_cart-0.3.5.tar`

### file list

```diff
@@ -1,34 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:42:14.409313 airbyte-source-cart-0.3.1/
--rw-r--r--   0 root         (0) root         (0)     5316 2024-01-30 14:42:14.409313 airbyte-source-cart-0.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5316 2024-01-30 14:29:13.000000 airbyte-source-cart-0.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:42:14.409313 airbyte-source-cart-0.3.1/airbyte_source_cart.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5316 2024-01-30 14:42:14.000000 airbyte-source-cart-0.3.1/airbyte_source_cart.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      934 2024-01-30 14:42:14.000000 airbyte-source-cart-0.3.1/airbyte_source_cart.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-30 14:42:14.000000 airbyte-source-cart-0.3.1/airbyte_source_cart.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-01-30 14:42:14.000000 airbyte-source-cart-0.3.1/airbyte_source_cart.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-01-30 14:42:14.000000 airbyte-source-cart-0.3.1/airbyte_source_cart.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-01-30 14:42:14.000000 airbyte-source-cart-0.3.1/airbyte_source_cart.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:42:14.405313 airbyte-source-cart-0.3.1/integration_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-30 14:29:13.000000 airbyte-source-cart-0.3.1/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      478 2024-01-30 14:29:13.000000 airbyte-source-cart-0.3.1/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      314 2024-01-30 14:29:13.000000 airbyte-source-cart-0.3.1/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     2412 2024-01-30 14:29:13.000000 airbyte-source-cart-0.3.1/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)     2184 2024-01-30 14:29:13.000000 airbyte-source-cart-0.3.1/integration_tests/configured_catalog_wo_order_statuses.json
--rw-r--r--   0 root         (0) root         (0)      106 2024-01-30 14:29:13.000000 airbyte-source-cart-0.3.1/integration_tests/integration_test.py
--rw-r--r--   0 root         (0) root         (0)      195 2024-01-30 14:29:13.000000 airbyte-source-cart-0.3.1/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)     5215 2024-01-30 14:42:14.409313 airbyte-source-cart-0.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      910 2024-01-30 14:42:12.000000 airbyte-source-cart-0.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:42:14.405313 airbyte-source-cart-0.3.1/source_cart/
--rw-r--r--   0 root         (0) root         (0)     1250 2024-01-30 14:29:13.000000 airbyte-source-cart-0.3.1/source_cart/__init__.py
--rw-r--r--   0 root         (0) root         (0)      224 2024-01-30 14:29:13.000000 airbyte-source-cart-0.3.1/source_cart/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:42:14.409313 airbyte-source-cart-0.3.1/source_cart/schemas/
--rw-r--r--   0 root         (0) root         (0)     1337 2024-01-30 14:29:13.000000 airbyte-source-cart-0.3.1/source_cart/schemas/addresses.json
--rw-r--r--   0 root         (0) root         (0)     2578 2024-01-30 14:29:13.000000 airbyte-source-cart-0.3.1/source_cart/schemas/customers_cart.json
--rw-r--r--   0 root         (0) root         (0)     3169 2024-01-30 14:29:13.000000 airbyte-source-cart-0.3.1/source_cart/schemas/order_items.json
--rw-r--r--   0 root         (0) root         (0)     2288 2024-01-30 14:29:13.000000 airbyte-source-cart-0.3.1/source_cart/schemas/order_payments.json
--rw-r--r--   0 root         (0) root         (0)      854 2024-01-30 14:29:13.000000 airbyte-source-cart-0.3.1/source_cart/schemas/order_statuses.json
--rw-r--r--   0 root         (0) root         (0)     4254 2024-01-30 14:29:13.000000 airbyte-source-cart-0.3.1/source_cart/schemas/orders.json
--rw-r--r--   0 root         (0) root         (0)     8331 2024-01-30 14:29:13.000000 airbyte-source-cart-0.3.1/source_cart/schemas/products.json
--rw-r--r--   0 root         (0) root         (0)     6301 2024-01-30 14:29:13.000000 airbyte-source-cart-0.3.1/source_cart/source.py
--rw-r--r--   0 root         (0) root         (0)     3024 2024-01-30 14:29:13.000000 airbyte-source-cart-0.3.1/source_cart/spec.json
--rw-r--r--   0 root         (0) root         (0)     6199 2024-01-30 14:29:13.000000 airbyte-source-cart-0.3.1/source_cart/streams.py
+-rw-r--r--   0        0        0     4460 2024-05-01 18:33:10.246414 airbyte_source_cart-0.3.5/README.md
+-rw-r--r--   0        0        0      731 2024-05-01 18:36:35.110264 airbyte_source_cart-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     1250 2024-05-01 18:33:10.246414 airbyte_source_cart-0.3.5/source_cart/__init__.py
+-rw-r--r--   0        0        0      224 2024-05-01 18:33:10.246414 airbyte_source_cart-0.3.5/source_cart/run.py
+-rw-r--r--   0        0        0     2782 2024-05-01 18:33:10.246414 airbyte_source_cart-0.3.5/source_cart/schemas/addresses.json
+-rw-r--r--   0        0        0     5103 2024-05-01 18:33:10.246414 airbyte_source_cart-0.3.5/source_cart/schemas/customers_cart.json
+-rw-r--r--   0        0        0     6378 2024-05-01 18:33:10.246414 airbyte_source_cart-0.3.5/source_cart/schemas/order_items.json
+-rw-r--r--   0        0        0     4705 2024-05-01 18:33:10.246414 airbyte_source_cart-0.3.5/source_cart/schemas/order_payments.json
+-rw-r--r--   0        0        0     1996 2024-05-01 18:33:10.250414 airbyte_source_cart-0.3.5/source_cart/schemas/order_statuses.json
+-rw-r--r--   0        0        0     8649 2024-05-01 18:33:10.250414 airbyte_source_cart-0.3.5/source_cart/schemas/orders.json
+-rw-r--r--   0        0        0    16936 2024-05-01 18:33:10.250414 airbyte_source_cart-0.3.5/source_cart/schemas/products.json
+-rw-r--r--   0        0        0     6301 2024-05-01 18:33:10.250414 airbyte_source_cart-0.3.5/source_cart/source.py
+-rw-r--r--   0        0        0     3024 2024-05-01 18:33:10.250414 airbyte_source_cart-0.3.5/source_cart/spec.json
+-rw-r--r--   0        0        0     6199 2024-05-01 18:33:10.250414 airbyte_source_cart-0.3.5/source_cart/streams.py
+-rw-r--r--   0        0        0     5158 1970-01-01 00:00:00.000000 airbyte_source_cart-0.3.5/PKG-INFO
```

### Comparing `airbyte-source-cart-0.3.1/PKG-INFO` & `airbyte_source_cart-0.3.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,98 +1,110 @@
 Metadata-Version: 2.1
 Name: airbyte-source-cart
-Version: 0.3.1
+Version: 0.3.5
 Summary: Source implementation for Cart.
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
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/cart
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
-Requires-Dist: pytest~=6.1; extra == "tests"
 
-# Cart.com Source
+# Cart source connector
 
-This is the repository for the Cart.com source connector, written in Python.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/cart).
 
+This is the repository for the Cart source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/cart).
 
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
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/cart)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_cart/spec.json` file.
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/cart)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_cart/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source cart test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
 ```
-python main.py spec
-python main.py check --config secrets/config.json
-python main.py discover --config secrets/config.json
-python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-cart spec
+poetry run source-cart check --config secrets/config.json
+poetry run source-cart discover --config secrets/config.json
+poetry run source-cart read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-cart build
 ```
 
-An image will be built with the tag `airbyte/source-cart:dev`.
+An image will be available on your host with the tag `airbyte/source-cart:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-cart:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-cart:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-cart:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-cart:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-cart:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-cart test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-cart test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/cart.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/cart.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-cart-0.3.1/airbyte_source_cart.egg-info/PKG-INFO` & `airbyte_source_cart-0.3.5/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,98 +1,91 @@
-Metadata-Version: 2.1
-Name: airbyte-source-cart
-Version: 0.3.1
-Summary: Source implementation for Cart.
-Author: Airbyte
-Author-email: contact@airbyte.io
-Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
-Requires-Dist: pytest~=6.1; extra == "tests"
+# Cart source connector
 
-# Cart.com Source
 
-This is the repository for the Cart.com source connector, written in Python.
-For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.io/integrations/sources/cart).
+This is the repository for the Cart source connector, written in Python.
+For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/cart).
 
+## Local development
 
-**To iterate on this connector, make sure to complete this prerequisites section.**
+### Prerequisites
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 
-From this connector directory, create a virtual environment:
-```
-python -m venv .venv
-```
-
-This will generate a virtualenv for this module in `.venv/`. Make sure this venv is active in your
-development environment of choice. To activate it from the terminal, run:
-```
-source .venv/bin/activate
-pip install -r requirements.txt
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
 
-**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.io/integrations/sources/cart)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_cart/spec.json` file.
+### Create credentials
+**If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/cart)
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_cart/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source cart test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
 ```
-python main.py spec
-python main.py check --config secrets/config.json
-python main.py discover --config secrets/config.json
-python main.py read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+poetry run source-cart spec
+poetry run source-cart check --config secrets/config.json
+poetry run source-cart discover --config secrets/config.json
+poetry run source-cart read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-cart build
 ```
 
-An image will be built with the tag `airbyte/source-cart:dev`.
+An image will be available on your host with the tag `airbyte/source-cart:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-cart:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-cart:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-cart:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-cart:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-cart:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-cart test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-cart test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/cart.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/cart.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-cart-0.3.1/source_cart/__init__.py` & `airbyte_source_cart-0.3.5/source_cart/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte-source-cart-0.3.1/source_cart/schemas/order_items.json` & `airbyte_source_cart-0.3.5/source_cart/schemas/addresses.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8793269230769231%*

 * *Differences: {"'properties'": "{'id': {'description': 'The unique identifier of the address record'}, "*

 * *                 "'updated_at': {'description': 'The date and time when the address was last "*

 * *                 "updated'}, 'created_at': {'description': 'The date and time when the address was "*

 * *                 "created'}, 'customer_id': OrderedDict([('description', 'The unique identifier of "*

 * *                 "the customer associated with the address'), ('type', ['integer', 'null'])]), "*

 * *                 "'address_ […]*

```diff
@@ -1,292 +1,144 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "additionalProperties": true,
     "properties": {
-        "admin_comments": {
+        "address_line_1": {
+            "description": "The address line 1 of the customer",
             "type": [
                 "string",
                 "null"
             ]
         },
-        "configuration": {
+        "address_line_2": {
+            "description": "The address line 2 of the customer, if applicable",
             "type": [
                 "string",
                 "null"
             ]
         },
-        "cost": {
-            "type": [
-                "number",
-                "null"
-            ]
-        },
-        "created_at": {
+        "address_type": {
+            "description": "The type of address, e.g., residential or commercial",
             "type": [
                 "string",
                 "null"
             ]
         },
-        "delivery_date": {
+        "alternate_phone": {
+            "description": "An alternate phone number associated with the address",
             "type": [
                 "string",
                 "null"
             ]
         },
-        "description": {
+        "city": {
+            "description": "The city where the address is located",
             "type": [
                 "string",
                 "null"
             ]
         },
-        "discount_amount": {
-            "type": [
-                "number",
-                "null"
-            ]
-        },
-        "discount_percentage": {
-            "type": [
-                "number",
-                "null"
-            ]
-        },
-        "do_not_discount": {
-            "type": [
-                "boolean",
-                "null"
-            ]
-        },
-        "fitment": {
-            "type": [
-                "string",
-                "null"
-            ]
-        },
-        "gift_message": {
-            "type": [
-                "string",
-                "null"
-            ]
-        },
-        "height": {
-            "type": [
-                "number",
-                "null"
-            ]
-        },
-        "id": {
-            "type": "integer"
-        },
-        "is_discount_item": {
-            "type": [
-                "boolean",
-                "null"
-            ]
-        },
-        "is_non_shipping_item": {
-            "type": [
-                "boolean",
-                "null"
-            ]
-        },
-        "is_quantity_bound_to_parent": {
-            "type": [
-                "boolean",
-                "null"
-            ]
-        },
-        "is_subscription_product": {
-            "type": [
-                "boolean",
-                "null"
-            ]
-        },
-        "is_taxable": {
-            "type": [
-                "boolean",
-                "null"
-            ]
-        },
-        "item_name": {
+        "comments": {
+            "description": "Any additional comments or notes related to the address",
             "type": [
                 "string",
                 "null"
             ]
         },
-        "item_number": {
+        "company": {
+            "description": "The name of the company associated with the address",
             "type": [
                 "string",
                 "null"
             ]
         },
-        "item_number_full": {
+        "country": {
+            "description": "The country where the address is located",
             "type": [
                 "string",
                 "null"
             ]
         },
-        "length": {
-            "type": [
-                "number",
-                "null"
-            ]
-        },
-        "line_item_note": {
+        "created_at": {
+            "description": "The date and time when the address was created",
             "type": [
                 "string",
                 "null"
             ]
         },
-        "order_id": {
+        "customer_id": {
+            "description": "The unique identifier of the customer associated with the address",
             "type": [
                 "integer",
                 "null"
             ]
         },
-        "order_shipping_address_id": {
+        "fax": {
+            "description": "The fax number associated with the address",
             "type": [
                 "string",
                 "null"
             ]
         },
-        "parent_order_item_id": {
-            "type": [
-                "integer",
-                "null"
-            ]
-        },
-        "personalizations": {
-            "type": [
-                "array",
-                "null"
-            ]
-        },
-        "price": {
-            "type": [
-                "number",
-                "null"
-            ]
-        },
-        "product_id": {
-            "type": [
-                "integer",
-                "null"
-            ]
-        },
-        "quantity": {
-            "type": [
-                "integer",
-                "null"
-            ]
-        },
-        "selected_shipping_method": {
+        "first_name": {
+            "description": "The first name of the customer",
             "type": [
                 "string",
                 "null"
             ]
         },
-        "selected_shipping_method_id": {
-            "type": [
-                "string",
-                "null"
-            ]
+        "id": {
+            "description": "The unique identifier of the address record",
+            "type": "integer"
         },
-        "selected_shipping_provider_service": {
+        "is_default_billing_address": {
+            "description": "Indicates if this is the default billing address for the customer",
             "type": [
-                "string",
+                "boolean",
                 "null"
             ]
         },
-        "shipping_classification_code": {
+        "is_default_shipping_address": {
+            "description": "Indicates if this is the default shipping address for the customer",
             "type": [
-                "string",
+                "boolean",
                 "null"
             ]
         },
-        "shipping_total": {
+        "last_name": {
+            "description": "The last name of the customer",
             "type": [
                 "string",
                 "null"
             ]
         },
-        "size_unit": {
+        "phone": {
+            "description": "The primary phone number associated with the address",
             "type": [
                 "string",
                 "null"
             ]
         },
-        "status": {
+        "postal_code": {
+            "description": "The postal or ZIP code of the address",
             "type": [
                 "string",
                 "null"
             ]
         },
-        "tax": {
-            "type": [
-                "number",
-                "null"
-            ]
-        },
-        "tax_code": {
+        "state": {
+            "description": "The state or region where the address is located",
             "type": [
                 "string",
                 "null"
             ]
         },
         "updated_at": {
+            "description": "The date and time when the address was last updated",
             "type": [
                 "string",
                 "null"
             ]
-        },
-        "variant_inventory_id": {
-            "type": [
-                "string",
-                "null"
-            ]
-        },
-        "variants": {
-            "type": [
-                "array",
-                "null"
-            ]
-        },
-        "vendor_store_id": {
-            "type": [
-                "integer",
-                "null"
-            ]
-        },
-        "warehouse_id": {
-            "type": [
-                "integer",
-                "null"
-            ]
-        },
-        "weigh_unit": {
-            "type": [
-                "string",
-                "null"
-            ]
-        },
-        "weight": {
-            "type": [
-                "number",
-                "null"
-            ]
-        },
-        "weight_unit": {
-            "type": [
-                "string",
-                "null"
-            ]
-        },
-        "width": {
-            "type": [
-                "number",
-                "null"
-            ]
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte-source-cart-0.3.1/source_cart/source.py` & `airbyte_source_cart-0.3.5/source_cart/source.py`

 * *Files identical despite different names*

### Comparing `airbyte-source-cart-0.3.1/source_cart/spec.json` & `airbyte_source_cart-0.3.5/source_cart/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-cart-0.3.1/source_cart/streams.py` & `airbyte_source_cart-0.3.5/source_cart/streams.py`

 * *Files identical despite different names*


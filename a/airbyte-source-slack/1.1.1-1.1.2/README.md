# Comparing `tmp/airbyte_source_slack-1.1.1.tar.gz` & `tmp/airbyte_source_slack-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_slack-1.1.1.tar", max compression
+gzip compressed data, was "airbyte_source_slack-1.1.2.tar", max compression
```

## Comparing `airbyte_source_slack-1.1.1.tar` & `airbyte_source_slack-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     4478 2024-05-07 10:58:05.000000 airbyte_source_slack-1.1.1/README.md
--rw-r--r--   0        0        0      779 2024-05-07 12:31:37.134699 airbyte_source_slack-1.1.1/pyproject.toml
--rw-r--r--   0        0        0       59 2024-05-07 10:58:05.000000 airbyte_source_slack-1.1.1/source_slack/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 10:58:05.000000 airbyte_source_slack-1.1.1/source_slack/components/__init__.py
--rw-r--r--   0        0        0      660 2024-05-07 10:58:05.000000 airbyte_source_slack-1.1.1/source_slack/components/channel_members_extractor.py
--rw-r--r--   0        0        0     5080 2024-05-07 10:58:05.000000 airbyte_source_slack-1.1.1/source_slack/components/join_channels.py
--rw-r--r--   0        0        0     2883 2024-05-07 10:58:05.000000 airbyte_source_slack-1.1.1/source_slack/config_migrations.py
--rw-r--r--   0        0        0     7992 2024-05-07 10:58:05.000000 airbyte_source_slack-1.1.1/source_slack/manifest.yaml
--rw-r--r--   0        0        0      344 2024-05-07 10:58:05.000000 airbyte_source_slack-1.1.1/source_slack/run.py
--rw-r--r--   0        0        0      407 2024-05-07 10:58:05.000000 airbyte_source_slack-1.1.1/source_slack/schemas/channel_members.json
--rw-r--r--   0        0        0     9372 2024-05-07 10:58:05.000000 airbyte_source_slack-1.1.1/source_slack/schemas/channel_messages.json
--rw-r--r--   0        0        0     5187 2024-05-07 10:58:05.000000 airbyte_source_slack-1.1.1/source_slack/schemas/channels.json
--rw-r--r--   0        0        0     4230 2024-05-07 10:58:05.000000 airbyte_source_slack-1.1.1/source_slack/schemas/threads.json
--rw-r--r--   0        0        0     6625 2024-05-07 10:58:05.000000 airbyte_source_slack-1.1.1/source_slack/schemas/users.json
--rw-r--r--   0        0        0     2365 2024-05-07 10:58:05.000000 airbyte_source_slack-1.1.1/source_slack/source.py
--rw-r--r--   0        0        0     5681 2024-05-07 10:58:05.000000 airbyte_source_slack-1.1.1/source_slack/spec.json
--rw-r--r--   0        0        0    12505 2024-05-07 10:58:05.000000 airbyte_source_slack-1.1.1/source_slack/streams.py
--rw-r--r--   0        0        0      835 2024-05-07 10:58:05.000000 airbyte_source_slack-1.1.1/source_slack/utils.py
--rw-r--r--   0        0        0     5255 1970-01-01 00:00:00.000000 airbyte_source_slack-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4488 2024-05-24 15:15:17.822814 airbyte_source_slack-1.1.2/README.md
+-rw-r--r--   0        0        0      779 2024-05-24 15:20:02.190641 airbyte_source_slack-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0       59 2024-05-24 15:15:17.834814 airbyte_source_slack-1.1.2/source_slack/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 15:15:17.834814 airbyte_source_slack-1.1.2/source_slack/components/__init__.py
+-rw-r--r--   0        0        0      660 2024-05-24 15:15:17.834814 airbyte_source_slack-1.1.2/source_slack/components/channel_members_extractor.py
+-rw-r--r--   0        0        0     5080 2024-05-24 15:15:17.834814 airbyte_source_slack-1.1.2/source_slack/components/join_channels.py
+-rw-r--r--   0        0        0     2883 2024-05-24 15:15:17.834814 airbyte_source_slack-1.1.2/source_slack/config_migrations.py
+-rw-r--r--   0        0        0     7992 2024-05-24 15:15:17.834814 airbyte_source_slack-1.1.2/source_slack/manifest.yaml
+-rw-r--r--   0        0        0      344 2024-05-24 15:15:17.834814 airbyte_source_slack-1.1.2/source_slack/run.py
+-rw-r--r--   0        0        0      407 2024-05-24 15:15:17.834814 airbyte_source_slack-1.1.2/source_slack/schemas/channel_members.json
+-rw-r--r--   0        0        0     9372 2024-05-24 15:15:17.834814 airbyte_source_slack-1.1.2/source_slack/schemas/channel_messages.json
+-rw-r--r--   0        0        0     5187 2024-05-24 15:15:17.834814 airbyte_source_slack-1.1.2/source_slack/schemas/channels.json
+-rw-r--r--   0        0        0     4230 2024-05-24 15:15:17.834814 airbyte_source_slack-1.1.2/source_slack/schemas/threads.json
+-rw-r--r--   0        0        0     6625 2024-05-24 15:15:17.834814 airbyte_source_slack-1.1.2/source_slack/schemas/users.json
+-rw-r--r--   0        0        0     2365 2024-05-24 15:15:17.834814 airbyte_source_slack-1.1.2/source_slack/source.py
+-rw-r--r--   0        0        0     5681 2024-05-24 15:15:17.834814 airbyte_source_slack-1.1.2/source_slack/spec.json
+-rw-r--r--   0        0        0    12505 2024-05-24 15:15:17.834814 airbyte_source_slack-1.1.2/source_slack/streams.py
+-rw-r--r--   0        0        0      835 2024-05-24 15:15:17.834814 airbyte_source_slack-1.1.2/source_slack/utils.py
+-rw-r--r--   0        0        0     5265 1970-01-01 00:00:00.000000 airbyte_source_slack-1.1.2/PKG-INFO
```

### Comparing `airbyte_source_slack-1.1.1/README.md` & `airbyte_source_slack-1.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # Slack source connector
 
-
 This is the repository for the Slack source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/slack).
 
 ## Local development
 
 ### Prerequisites
-* Python (~=3.9)
-* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
+- Python (~=3.9)
+- Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 ### Installing the connector
+
 From this connector directory, run:
+
 ```bash
 poetry install --with dev
 ```
 
-
 ### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/slack)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_slack/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-slack spec
 poetry run source-slack check --config secrets/config.json
 poetry run source-slack discover --config secrets/config.json
 poetry run source-slack read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
 ### Running unit tests
+
 To run unit tests locally, from the connector directory run:
+
 ```
 poetry run pytest unit_tests
 ```
 
 ### Building the docker image
+
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
+
 ```bash
 airbyte-ci connectors --name=source-slack build
 ```
 
 An image will be available on your host with the tag `airbyte/source-slack:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-slack:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-slack:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-slack:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-slack:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-slack test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ### Dependency Management
-All of your dependencies should be managed via Poetry. 
+
+All of your dependencies should be managed via Poetry.
 To add a new dependency, run:
+
 ```bash
 poetry add <package-name>
 ```
 
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
 ## Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-slack test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/slack.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_slack-1.1.1/pyproject.toml` & `airbyte_source_slack-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "1.1.1"
+version = "1.1.2"
 name = "airbyte-source-slack"
 description = "Source implementation for Slack."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_slack-1.1.1/source_slack/components/channel_members_extractor.py` & `airbyte_source_slack-1.1.2/source_slack/components/channel_members_extractor.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_slack-1.1.1/source_slack/components/join_channels.py` & `airbyte_source_slack-1.1.2/source_slack/components/join_channels.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_slack-1.1.1/source_slack/config_migrations.py` & `airbyte_source_slack-1.1.2/source_slack/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_slack-1.1.1/source_slack/manifest.yaml` & `airbyte_source_slack-1.1.2/source_slack/manifest.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -215,15 +215,15 @@
               inject_into: "request_parameter"
     incremental_sync:
       type: DatetimeBasedCursor
       cursor_field: float_ts
       cursor_datetime_formats:
         - "%s"
       step: P100D
-      cursor_granularity: P10D
+      cursor_granularity: PT1S
       lookback_window: "P{{ config.get('lookback_window', 0) }}D"
       datetime_format: "%s"
       start_datetime:
         type: MinMaxDatetime
         datetime: "{{ config['start_date'] }}"
         datetime_format: "%Y-%m-%dT%H:%M:%SZ"
       start_time_option:
```

### Comparing `airbyte_source_slack-1.1.1/source_slack/schemas/channel_messages.json` & `airbyte_source_slack-1.1.2/source_slack/schemas/channel_messages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_slack-1.1.1/source_slack/schemas/channels.json` & `airbyte_source_slack-1.1.2/source_slack/schemas/channels.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_slack-1.1.1/source_slack/schemas/threads.json` & `airbyte_source_slack-1.1.2/source_slack/schemas/threads.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_slack-1.1.1/source_slack/schemas/users.json` & `airbyte_source_slack-1.1.2/source_slack/schemas/users.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_slack-1.1.1/source_slack/source.py` & `airbyte_source_slack-1.1.2/source_slack/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_slack-1.1.1/source_slack/spec.json` & `airbyte_source_slack-1.1.2/source_slack/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_slack-1.1.1/source_slack/streams.py` & `airbyte_source_slack-1.1.2/source_slack/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_slack-1.1.1/source_slack/utils.py` & `airbyte_source_slack-1.1.2/source_slack/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_slack-1.1.1/PKG-INFO` & `airbyte_source_slack-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-slack
-Version: 1.1.1
+Version: 1.1.2
 Summary: Source implementation for Slack.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -17,96 +17,110 @@
 Requires-Dist: pendulum (==2.1.2)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/slack
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Slack source connector
 
-
 This is the repository for the Slack source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/slack).
 
 ## Local development
 
 ### Prerequisites
-* Python (~=3.9)
-* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
+- Python (~=3.9)
+- Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 ### Installing the connector
+
 From this connector directory, run:
+
 ```bash
 poetry install --with dev
 ```
 
-
 ### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/slack)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_slack/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-slack spec
 poetry run source-slack check --config secrets/config.json
 poetry run source-slack discover --config secrets/config.json
 poetry run source-slack read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
 ### Running unit tests
+
 To run unit tests locally, from the connector directory run:
+
 ```
 poetry run pytest unit_tests
 ```
 
 ### Building the docker image
+
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
+
 ```bash
 airbyte-ci connectors --name=source-slack build
 ```
 
 An image will be available on your host with the tag `airbyte/source-slack:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-slack:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-slack:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-slack:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-slack:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-slack test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ### Dependency Management
-All of your dependencies should be managed via Poetry. 
+
+All of your dependencies should be managed via Poetry.
 To add a new dependency, run:
+
 ```bash
 poetry add <package-name>
 ```
 
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
 ## Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-slack test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/slack.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```


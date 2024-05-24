# Comparing `tmp/airbyte_source_marketo-1.4.0.tar.gz` & `tmp/airbyte_source_marketo-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_marketo-1.4.0.tar", max compression
+gzip compressed data, was "airbyte_source_marketo-1.4.1.tar", max compression
```

## Comparing `airbyte_source_marketo-1.4.0.tar` & `airbyte_source_marketo-1.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     4519 2024-04-29 17:04:46.000000 airbyte_source_marketo-1.4.0/README.md
--rw-r--r--   0        0        0      772 2024-04-29 18:17:32.035382 airbyte_source_marketo-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     1171 2024-04-29 17:04:46.000000 airbyte_source_marketo-1.4.0/source_marketo/__init__.py
--rw-r--r--   0        0        0     5854 2024-04-29 17:04:46.000000 airbyte_source_marketo-1.4.0/source_marketo/manifest.yaml
--rw-r--r--   0        0        0      233 2024-04-29 17:04:46.000000 airbyte_source_marketo-1.4.0/source_marketo/run.py
--rw-r--r--   0        0        0     1542 2024-04-29 17:04:46.000000 airbyte_source_marketo-1.4.0/source_marketo/schemas/activity_types.json
--rw-r--r--   0        0        0     1471 2024-04-29 17:04:46.000000 airbyte_source_marketo-1.4.0/source_marketo/schemas/campaigns.json
--rw-r--r--   0        0        0    11717 2024-04-29 17:04:46.000000 airbyte_source_marketo-1.4.0/source_marketo/schemas/leads.json
--rw-r--r--   0        0        0     1158 2024-04-29 17:04:46.000000 airbyte_source_marketo-1.4.0/source_marketo/schemas/lists.json
--rw-r--r--   0        0        0     2254 2024-04-29 17:04:46.000000 airbyte_source_marketo-1.4.0/source_marketo/schemas/programs.json
--rw-r--r--   0        0        0     1620 2024-04-29 17:04:46.000000 airbyte_source_marketo-1.4.0/source_marketo/schemas/segmentations.json
--rw-r--r--   0        0        0    19219 2024-04-29 17:04:46.000000 airbyte_source_marketo-1.4.0/source_marketo/source.py
--rw-r--r--   0        0        0     1803 2024-04-29 17:04:46.000000 airbyte_source_marketo-1.4.0/source_marketo/spec.json
--rw-r--r--   0        0        0     2069 2024-04-29 17:04:46.000000 airbyte_source_marketo-1.4.0/source_marketo/utils.py
--rw-r--r--   0        0        0     5223 1970-01-01 00:00:00.000000 airbyte_source_marketo-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     4529 2024-05-24 05:53:22.914483 airbyte_source_marketo-1.4.1/README.md
+-rw-r--r--   0        0        0      776 2024-05-24 06:01:47.809139 airbyte_source_marketo-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1171 2024-05-24 05:53:22.914483 airbyte_source_marketo-1.4.1/source_marketo/__init__.py
+-rw-r--r--   0        0        0     5854 2024-05-24 05:53:22.914483 airbyte_source_marketo-1.4.1/source_marketo/manifest.yaml
+-rw-r--r--   0        0        0      233 2024-05-24 05:53:22.914483 airbyte_source_marketo-1.4.1/source_marketo/run.py
+-rw-r--r--   0        0        0     1542 2024-05-24 05:53:22.914483 airbyte_source_marketo-1.4.1/source_marketo/schemas/activity_types.json
+-rw-r--r--   0        0        0     1471 2024-05-24 05:53:22.914483 airbyte_source_marketo-1.4.1/source_marketo/schemas/campaigns.json
+-rw-r--r--   0        0        0    11717 2024-05-24 05:53:22.914483 airbyte_source_marketo-1.4.1/source_marketo/schemas/leads.json
+-rw-r--r--   0        0        0     1158 2024-05-24 05:53:22.914483 airbyte_source_marketo-1.4.1/source_marketo/schemas/lists.json
+-rw-r--r--   0        0        0     2254 2024-05-24 05:53:22.914483 airbyte_source_marketo-1.4.1/source_marketo/schemas/programs.json
+-rw-r--r--   0        0        0     1620 2024-05-24 05:53:22.914483 airbyte_source_marketo-1.4.1/source_marketo/schemas/segmentations.json
+-rw-r--r--   0        0        0    19253 2024-05-24 05:53:22.914483 airbyte_source_marketo-1.4.1/source_marketo/source.py
+-rw-r--r--   0        0        0     1803 2024-05-24 05:53:22.914483 airbyte_source_marketo-1.4.1/source_marketo/spec.json
+-rw-r--r--   0        0        0     2069 2024-05-24 05:53:22.914483 airbyte_source_marketo-1.4.1/source_marketo/utils.py
+-rw-r--r--   0        0        0     5235 1970-01-01 00:00:00.000000 airbyte_source_marketo-1.4.1/PKG-INFO
```

### Comparing `airbyte_source_marketo-1.4.0/README.md` & `airbyte_source_marketo-1.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # Marketo source connector
 
-
 This is the repository for the Marketo source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/marketo).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/marketo)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_marketo/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-marketo spec
 poetry run source-marketo check --config secrets/config.json
 poetry run source-marketo discover --config secrets/config.json
 poetry run source-marketo read --config secrets/config.json --catalog integration_tests/configured_catalog.json
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
 airbyte-ci connectors --name=source-marketo build
 ```
 
 An image will be available on your host with the tag `airbyte/source-marketo:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-marketo:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-marketo:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-marketo:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-marketo:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-marketo test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-marketo test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/marketo.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_marketo-1.4.0/pyproject.toml` & `airbyte_source_marketo-1.4.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "1.4.0"
+version = "1.4.1"
 name = "airbyte-source-marketo"
 description = "Source implementation for Marketo."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_marketo" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "^0"
+airbyte-cdk = "0.90.0"
 
 [tool.poetry.scripts]
 source-marketo = "source_marketo.run:run"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.1"
 requests-mock = "^1.11.0"
```

### Comparing `airbyte_source_marketo-1.4.0/source_marketo/__init__.py` & `airbyte_source_marketo-1.4.1/source_marketo/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_marketo-1.4.0/source_marketo/manifest.yaml` & `airbyte_source_marketo-1.4.1/source_marketo/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_marketo-1.4.0/source_marketo/schemas/activity_types.json` & `airbyte_source_marketo-1.4.1/source_marketo/schemas/activity_types.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_marketo-1.4.0/source_marketo/schemas/campaigns.json` & `airbyte_source_marketo-1.4.1/source_marketo/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_marketo-1.4.0/source_marketo/schemas/leads.json` & `airbyte_source_marketo-1.4.1/source_marketo/schemas/leads.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_marketo-1.4.0/source_marketo/schemas/lists.json` & `airbyte_source_marketo-1.4.1/source_marketo/schemas/lists.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_marketo-1.4.0/source_marketo/schemas/programs.json` & `airbyte_source_marketo-1.4.1/source_marketo/schemas/programs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_marketo-1.4.0/source_marketo/schemas/segmentations.json` & `airbyte_source_marketo-1.4.1/source_marketo/schemas/segmentations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_marketo-1.4.0/source_marketo/source.py` & `airbyte_source_marketo-1.4.1/source_marketo/source.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import requests
 from airbyte_cdk.models import SyncMode
 from airbyte_cdk.sources.declarative.exceptions import ReadException
 from airbyte_cdk.sources.declarative.yaml_declarative_source import YamlDeclarativeSource
 from airbyte_cdk.sources.streams import Stream
 from airbyte_cdk.sources.streams.availability_strategy import AvailabilityStrategy
 from airbyte_cdk.sources.streams.http import HttpStream
-from airbyte_cdk.sources.streams.http.auth import Oauth2Authenticator
+from airbyte_cdk.sources.streams.http.requests_native_auth import Oauth2Authenticator
 from airbyte_cdk.utils import AirbyteTracedException
 from airbyte_protocol.models import FailureType
 
 from .utils import STRING_TYPES, clean_string, format_value, to_datetime_str
 
 
 class MarketoStream(HttpStream, ABC):
@@ -446,26 +446,26 @@
             client_secret=config["client_secret"],
             refresh_token=None,
         )
 
     def get_refresh_request_params(self) -> Mapping[str, Any]:
         payload: MutableMapping[str, Any] = {
             "grant_type": "client_credentials",
-            "client_id": self.client_id,
-            "client_secret": self.client_secret,
+            "client_id": self.get_client_id(),
+            "client_secret": self.get_client_secret(),
         }
 
         return payload
 
     def refresh_access_token(self) -> Tuple[str, int]:
         """
         Returns a tuple of (access_token, token_lifespan_in_seconds)
         """
         try:
-            response = requests.request(method="GET", url=self.token_refresh_endpoint, params=self.get_refresh_request_params())
+            response = requests.request(method="GET", url=self.get_token_refresh_endpoint(), params=self.get_refresh_request_params())
             response.raise_for_status()
             response_json = response.json()
             return response_json["access_token"], response_json["expires_in"]
         except Exception as e:
             raise Exception(f"Error while refreshing access token: {e}") from e
```

### Comparing `airbyte_source_marketo-1.4.0/source_marketo/spec.json` & `airbyte_source_marketo-1.4.1/source_marketo/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_marketo-1.4.0/source_marketo/utils.py` & `airbyte_source_marketo-1.4.1/source_marketo/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_marketo-1.4.0/PKG-INFO` & `airbyte_source_marketo-1.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,110 +1,124 @@
 Metadata-Version: 2.1
 Name: airbyte-source-marketo
-Version: 1.4.0
+Version: 1.4.1
 Summary: Source implementation for Marketo.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (>=0,<1)
+Requires-Dist: airbyte-cdk (==0.90.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/marketo
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Marketo source connector
 
-
 This is the repository for the Marketo source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/marketo).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/marketo)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_marketo/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-marketo spec
 poetry run source-marketo check --config secrets/config.json
 poetry run source-marketo discover --config secrets/config.json
 poetry run source-marketo read --config secrets/config.json --catalog integration_tests/configured_catalog.json
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
 airbyte-ci connectors --name=source-marketo build
 ```
 
 An image will be available on your host with the tag `airbyte/source-marketo:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-marketo:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-marketo:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-marketo:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-marketo:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-marketo test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-marketo test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/marketo.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```


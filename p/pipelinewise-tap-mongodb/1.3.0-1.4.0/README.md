# Comparing `tmp/pipelinewise-tap-mongodb-1.3.0.tar.gz` & `tmp/pipelinewise_tap_mongodb-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipelinewise-tap-mongodb-1.3.0.tar", last modified: Mon Jan  3 14:25:28 2022, max compression
+gzip compressed data, was "pipelinewise_tap_mongodb-1.4.0.tar", last modified: Fri May 24 14:36:15 2024, max compression
```

## Comparing `pipelinewise-tap-mongodb-1.3.0.tar` & `pipelinewise_tap_mongodb-1.4.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 14:25:28.053801 pipelinewise-tap-mongodb-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)    32386 2022-01-03 14:25:14.000000 pipelinewise-tap-mongodb-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4973 2022-01-03 14:25:28.053801 pipelinewise-tap-mongodb-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4395 2022-01-03 14:25:14.000000 pipelinewise-tap-mongodb-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 14:25:28.053801 pipelinewise-tap-mongodb-1.3.0/pipelinewise_tap_mongodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4973 2022-01-03 14:25:27.000000 pipelinewise-tap-mongodb-1.3.0/pipelinewise_tap_mongodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      611 2022-01-03 14:25:27.000000 pipelinewise-tap-mongodb-1.3.0/pipelinewise_tap_mongodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-03 14:25:27.000000 pipelinewise-tap-mongodb-1.3.0/pipelinewise_tap_mongodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-01-03 14:25:27.000000 pipelinewise-tap-mongodb-1.3.0/pipelinewise_tap_mongodb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-01-03 14:25:27.000000 pipelinewise-tap-mongodb-1.3.0/pipelinewise_tap_mongodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-01-03 14:25:27.000000 pipelinewise-tap-mongodb-1.3.0/pipelinewise_tap_mongodb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-03 14:25:28.053801 pipelinewise-tap-mongodb-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1308 2022-01-03 14:25:14.000000 pipelinewise-tap-mongodb-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 14:25:28.053801 pipelinewise-tap-mongodb-1.3.0/tap_mongodb/
--rw-r--r--   0 runner    (1001) docker     (121)    11540 2022-01-03 14:25:14.000000 pipelinewise-tap-mongodb-1.3.0/tap_mongodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1388 2022-01-03 14:25:14.000000 pipelinewise-tap-mongodb-1.3.0/tap_mongodb/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6531 2022-01-03 14:25:14.000000 pipelinewise-tap-mongodb-1.3.0/tap_mongodb/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2022-01-03 14:25:14.000000 pipelinewise-tap-mongodb-1.3.0/tap_mongodb/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     4199 2022-01-03 14:25:14.000000 pipelinewise-tap-mongodb-1.3.0/tap_mongodb/stream_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 14:25:28.053801 pipelinewise-tap-mongodb-1.3.0/tap_mongodb/sync_strategies/
--rw-r--r--   0 runner    (1001) docker     (121)     9195 2022-01-03 14:25:14.000000 pipelinewise-tap-mongodb-1.3.0/tap_mongodb/sync_strategies/change_streams.py
--rw-r--r--   0 runner    (1001) docker     (121)     9394 2022-01-03 14:25:14.000000 pipelinewise-tap-mongodb-1.3.0/tap_mongodb/sync_strategies/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     6089 2022-01-03 14:25:14.000000 pipelinewise-tap-mongodb-1.3.0/tap_mongodb/sync_strategies/full_table.py
--rw-r--r--   0 runner    (1001) docker     (121)     4642 2022-01-03 14:25:14.000000 pipelinewise-tap-mongodb-1.3.0/tap_mongodb/sync_strategies/incremental.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:36:15.915726 pipelinewise_tap_mongodb-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    32386 2024-05-24 14:36:07.000000 pipelinewise_tap_mongodb-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-05-24 14:36:15.915726 pipelinewise_tap_mongodb-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-24 14:36:07.000000 pipelinewise_tap_mongodb-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:36:15.915726 pipelinewise_tap_mongodb-1.4.0/pipelinewise_tap_mongodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-05-24 14:36:15.000000 pipelinewise_tap_mongodb-1.4.0/pipelinewise_tap_mongodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-24 14:36:15.000000 pipelinewise_tap_mongodb-1.4.0/pipelinewise_tap_mongodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 14:36:15.000000 pipelinewise_tap_mongodb-1.4.0/pipelinewise_tap_mongodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-24 14:36:15.000000 pipelinewise_tap_mongodb-1.4.0/pipelinewise_tap_mongodb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-24 14:36:15.000000 pipelinewise_tap_mongodb-1.4.0/pipelinewise_tap_mongodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-24 14:36:15.000000 pipelinewise_tap_mongodb-1.4.0/pipelinewise_tap_mongodb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 14:36:15.915726 pipelinewise_tap_mongodb-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-24 14:36:07.000000 pipelinewise_tap_mongodb-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:36:15.915726 pipelinewise_tap_mongodb-1.4.0/tap_mongodb/
+-rw-r--r--   0 runner    (1001) docker     (127)    11540 2024-05-24 14:36:07.000000 pipelinewise_tap_mongodb-1.4.0/tap_mongodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-24 14:36:07.000000 pipelinewise_tap_mongodb-1.4.0/tap_mongodb/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-05-24 14:36:07.000000 pipelinewise_tap_mongodb-1.4.0/tap_mongodb/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-24 14:36:07.000000 pipelinewise_tap_mongodb-1.4.0/tap_mongodb/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-24 14:36:07.000000 pipelinewise_tap_mongodb-1.4.0/tap_mongodb/stream_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:36:15.915726 pipelinewise_tap_mongodb-1.4.0/tap_mongodb/sync_strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)     9195 2024-05-24 14:36:07.000000 pipelinewise_tap_mongodb-1.4.0/tap_mongodb/sync_strategies/change_streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9394 2024-05-24 14:36:07.000000 pipelinewise_tap_mongodb-1.4.0/tap_mongodb/sync_strategies/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-05-24 14:36:07.000000 pipelinewise_tap_mongodb-1.4.0/tap_mongodb/sync_strategies/full_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-24 14:36:07.000000 pipelinewise_tap_mongodb-1.4.0/tap_mongodb/sync_strategies/incremental.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 14:36:15.915726 pipelinewise_tap_mongodb-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-24 14:36:07.000000 pipelinewise_tap_mongodb-1.4.0/tests/test_connection_string.py
```

### Comparing `pipelinewise-tap-mongodb-1.3.0/LICENSE` & `pipelinewise_tap_mongodb-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mongodb-1.3.0/PKG-INFO` & `pipelinewise_tap_mongodb-1.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 Metadata-Version: 2.1
 Name: pipelinewise-tap-mongodb
-Version: 1.3.0
+Version: 1.4.0
 Summary: Singer.io tap for extracting data from MongoDB - Pipelinewise compatible
 Home-page: https://github.com/transferwise/pipelinewise-tap-mongodb
 Author: Wise
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pipelinewise-singer-python==1.*
+Requires-Dist: pymongo==4.7.*
+Requires-Dist: tzlocal==2.1.*
+Requires-Dist: terminaltables==3.1.*
+Requires-Dist: dnspython==2.1.*
 Provides-Extra: dev
+Requires-Dist: pylint==2.12; extra == "dev"
+Requires-Dist: ipdb==0.13.*; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: pytest==6.2.5; extra == "test"
+Requires-Dist: pytest-cov==3.0.0; extra == "test"
 
 # pipelinewise-tap-mongodb
 
 This is a [Singer](https://singer.io) tap that produces JSON-formatted data following the [Singer spec](https://github.com/singer-io/getting-started/blob/master/SPEC.md) from a MongoDB source.
 
 ## Set up local dev environment:
 
@@ -152,9 +159,7 @@
 ## Logging configuration
 The tap uses a predefined logging config if none is provided, however, you can set your own config by setting the environment variable `LOGGING_CONFIG_FILE` as the path to the logging config.
 A sample config is available [here](./sample_logging.conf).
 
 ---
 
 Copyright &copy; 2020 TransferWise
-
-
```

#### html2text {}

```diff
@@ -1,34 +1,38 @@
-Metadata-Version: 2.1 Name: pipelinewise-tap-mongodb Version: 1.3.0 Summary:
+Metadata-Version: 2.1 Name: pipelinewise-tap-mongodb Version: 1.4.0 Summary:
 Singer.io tap for extracting data from MongoDB - Pipelinewise compatible Home-
 page: https://github.com/transferwise/pipelinewise-tap-mongodb Author: Wise
-License: UNKNOWN Platform: UNKNOWN Classifier: Programming Language :: Python
-:: 3 :: Only Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Description-Content-Type: text/markdown Provides-Extra: dev
-Provides-Extra: test License-File: LICENSE # pipelinewise-tap-mongodb This is a
-[Singer](https://singer.io) tap that produces JSON-formatted data following the
-[Singer spec](https://github.com/singer-io/getting-started/blob/master/SPEC.md)
-from a MongoDB source. ## Set up local dev environment: ```shell script make
-setup ``` ## Activate virtual environment ```shell script . venv/bin/activate
-``` ## Set up Config file Create json file called `config.json`, with the
-following contents: ```json { "password": "", "user": "", "host": "",
-"auth_database": "", "database": "" } ``` The following parameters are optional
-for your config file: | Name | Type | Default value| Description | | -----|----
---|--------|------------ | | `srv` | Boolean | false | uses a `mongodb+srv`
-protocol to connect. Disables the usage of `port` argument if set to `True` | |
-`port` | Integer | false | Connection port. Required if a non-srv connection is
-being used. | | `replica_set` | string | null | name of replica set | | `ssl` |
-Boolean | false | can be set to true to connect using ssl | | `verify_mode` |
-Boolean | true | Default SSL verify mode | |
-`include_schemas_in_destination_stream_name` | Boolean |false | forces the
-stream names to take the form `-` instead of ``| | `update_buffer_size` | int |
-1 | [LOG_BASED] The size of the buffer that holds detected update operations in
-memory, the buffer is flushed once the size is reached | | `await_time_ms` |
-int | 1000 | [LOG_BASED] The maximum amount of time in milliseconds the
-loge_base method waits for new data changes before exiting. | All of the above
-attributes are required by the tap to connect to your mongo instance. here is a
-[sample configuration file](./sample_config.json). ## Run in discovery mode Run
-the following command and redirect the output into the catalog file ```shell
-script tap-mongodb --config ~/config.json --discover > ~/catalog.json ``` Your
-catalog file should now look like this: ```json { "streams": [ { "table_name":
-"
+Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Description-Content-Type:
+text/markdown License-File: LICENSE Requires-Dist: pipelinewise-singer-
+python==1.* Requires-Dist: pymongo==4.7.* Requires-Dist: tzlocal==2.1.*
+Requires-Dist: terminaltables==3.1.* Requires-Dist: dnspython==2.1.* Provides-
+Extra: dev Requires-Dist: pylint==2.12; extra == "dev" Requires-Dist:
+ipdb==0.13.*; extra == "dev" Provides-Extra: test Requires-Dist: pytest==6.2.5;
+extra == "test" Requires-Dist: pytest-cov==3.0.0; extra == "test" #
+pipelinewise-tap-mongodb This is a [Singer](https://singer.io) tap that
+produces JSON-formatted data following the [Singer spec](https://github.com/
+singer-io/getting-started/blob/master/SPEC.md) from a MongoDB source. ## Set up
+local dev environment: ```shell script make setup ``` ## Activate virtual
+environment ```shell script . venv/bin/activate ``` ## Set up Config file
+Create json file called `config.json`, with the following contents: ```json
+{ "password": "", "user": "", "host": "", "auth_database": "", "database": "" }
+``` The following parameters are optional for your config file: | Name | Type |
+Default value| Description | | -----|------|--------|------------ | | `srv` |
+Boolean | false | uses a `mongodb+srv` protocol to connect. Disables the usage
+of `port` argument if set to `True` | | `port` | Integer | false | Connection
+port. Required if a non-srv connection is being used. | | `replica_set` |
+string | null | name of replica set | | `ssl` | Boolean | false | can be set to
+true to connect using ssl | | `verify_mode` | Boolean | true | Default SSL
+verify mode | | `include_schemas_in_destination_stream_name` | Boolean |false |
+forces the stream names to take the form `-` instead of ``| |
+`update_buffer_size` | int | 1 | [LOG_BASED] The size of the buffer that holds
+detected update operations in memory, the buffer is flushed once the size is
+reached | | `await_time_ms` | int | 1000 | [LOG_BASED] The maximum amount of
+time in milliseconds the loge_base method waits for new data changes before
+exiting. | All of the above attributes are required by the tap to connect to
+your mongo instance. here is a [sample configuration file](./
+sample_config.json). ## Run in discovery mode Run the following command and
+redirect the output into the catalog file ```shell script tap-mongodb --config
+~/config.json --discover > ~/catalog.json ``` Your catalog file should now look
+like this: ```json { "streams": [ { "table_name": "
```

### Comparing `pipelinewise-tap-mongodb-1.3.0/README.md` & `pipelinewise_tap_mongodb-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mongodb-1.3.0/pipelinewise_tap_mongodb.egg-info/PKG-INFO` & `pipelinewise_tap_mongodb-1.4.0/pipelinewise_tap_mongodb.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 Metadata-Version: 2.1
 Name: pipelinewise-tap-mongodb
-Version: 1.3.0
+Version: 1.4.0
 Summary: Singer.io tap for extracting data from MongoDB - Pipelinewise compatible
 Home-page: https://github.com/transferwise/pipelinewise-tap-mongodb
 Author: Wise
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pipelinewise-singer-python==1.*
+Requires-Dist: pymongo==4.7.*
+Requires-Dist: tzlocal==2.1.*
+Requires-Dist: terminaltables==3.1.*
+Requires-Dist: dnspython==2.1.*
 Provides-Extra: dev
+Requires-Dist: pylint==2.12; extra == "dev"
+Requires-Dist: ipdb==0.13.*; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: pytest==6.2.5; extra == "test"
+Requires-Dist: pytest-cov==3.0.0; extra == "test"
 
 # pipelinewise-tap-mongodb
 
 This is a [Singer](https://singer.io) tap that produces JSON-formatted data following the [Singer spec](https://github.com/singer-io/getting-started/blob/master/SPEC.md) from a MongoDB source.
 
 ## Set up local dev environment:
 
@@ -152,9 +159,7 @@
 ## Logging configuration
 The tap uses a predefined logging config if none is provided, however, you can set your own config by setting the environment variable `LOGGING_CONFIG_FILE` as the path to the logging config.
 A sample config is available [here](./sample_logging.conf).
 
 ---
 
 Copyright &copy; 2020 TransferWise
-
-
```

#### html2text {}

```diff
@@ -1,34 +1,38 @@
-Metadata-Version: 2.1 Name: pipelinewise-tap-mongodb Version: 1.3.0 Summary:
+Metadata-Version: 2.1 Name: pipelinewise-tap-mongodb Version: 1.4.0 Summary:
 Singer.io tap for extracting data from MongoDB - Pipelinewise compatible Home-
 page: https://github.com/transferwise/pipelinewise-tap-mongodb Author: Wise
-License: UNKNOWN Platform: UNKNOWN Classifier: Programming Language :: Python
-:: 3 :: Only Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Description-Content-Type: text/markdown Provides-Extra: dev
-Provides-Extra: test License-File: LICENSE # pipelinewise-tap-mongodb This is a
-[Singer](https://singer.io) tap that produces JSON-formatted data following the
-[Singer spec](https://github.com/singer-io/getting-started/blob/master/SPEC.md)
-from a MongoDB source. ## Set up local dev environment: ```shell script make
-setup ``` ## Activate virtual environment ```shell script . venv/bin/activate
-``` ## Set up Config file Create json file called `config.json`, with the
-following contents: ```json { "password": "", "user": "", "host": "",
-"auth_database": "", "database": "" } ``` The following parameters are optional
-for your config file: | Name | Type | Default value| Description | | -----|----
---|--------|------------ | | `srv` | Boolean | false | uses a `mongodb+srv`
-protocol to connect. Disables the usage of `port` argument if set to `True` | |
-`port` | Integer | false | Connection port. Required if a non-srv connection is
-being used. | | `replica_set` | string | null | name of replica set | | `ssl` |
-Boolean | false | can be set to true to connect using ssl | | `verify_mode` |
-Boolean | true | Default SSL verify mode | |
-`include_schemas_in_destination_stream_name` | Boolean |false | forces the
-stream names to take the form `-` instead of ``| | `update_buffer_size` | int |
-1 | [LOG_BASED] The size of the buffer that holds detected update operations in
-memory, the buffer is flushed once the size is reached | | `await_time_ms` |
-int | 1000 | [LOG_BASED] The maximum amount of time in milliseconds the
-loge_base method waits for new data changes before exiting. | All of the above
-attributes are required by the tap to connect to your mongo instance. here is a
-[sample configuration file](./sample_config.json). ## Run in discovery mode Run
-the following command and redirect the output into the catalog file ```shell
-script tap-mongodb --config ~/config.json --discover > ~/catalog.json ``` Your
-catalog file should now look like this: ```json { "streams": [ { "table_name":
-"
+Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Description-Content-Type:
+text/markdown License-File: LICENSE Requires-Dist: pipelinewise-singer-
+python==1.* Requires-Dist: pymongo==4.7.* Requires-Dist: tzlocal==2.1.*
+Requires-Dist: terminaltables==3.1.* Requires-Dist: dnspython==2.1.* Provides-
+Extra: dev Requires-Dist: pylint==2.12; extra == "dev" Requires-Dist:
+ipdb==0.13.*; extra == "dev" Provides-Extra: test Requires-Dist: pytest==6.2.5;
+extra == "test" Requires-Dist: pytest-cov==3.0.0; extra == "test" #
+pipelinewise-tap-mongodb This is a [Singer](https://singer.io) tap that
+produces JSON-formatted data following the [Singer spec](https://github.com/
+singer-io/getting-started/blob/master/SPEC.md) from a MongoDB source. ## Set up
+local dev environment: ```shell script make setup ``` ## Activate virtual
+environment ```shell script . venv/bin/activate ``` ## Set up Config file
+Create json file called `config.json`, with the following contents: ```json
+{ "password": "", "user": "", "host": "", "auth_database": "", "database": "" }
+``` The following parameters are optional for your config file: | Name | Type |
+Default value| Description | | -----|------|--------|------------ | | `srv` |
+Boolean | false | uses a `mongodb+srv` protocol to connect. Disables the usage
+of `port` argument if set to `True` | | `port` | Integer | false | Connection
+port. Required if a non-srv connection is being used. | | `replica_set` |
+string | null | name of replica set | | `ssl` | Boolean | false | can be set to
+true to connect using ssl | | `verify_mode` | Boolean | true | Default SSL
+verify mode | | `include_schemas_in_destination_stream_name` | Boolean |false |
+forces the stream names to take the form `-` instead of ``| |
+`update_buffer_size` | int | 1 | [LOG_BASED] The size of the buffer that holds
+detected update operations in memory, the buffer is flushed once the size is
+reached | | `await_time_ms` | int | 1000 | [LOG_BASED] The maximum amount of
+time in milliseconds the loge_base method waits for new data changes before
+exiting. | All of the above attributes are required by the tap to connect to
+your mongo instance. here is a [sample configuration file](./
+sample_config.json). ## Run in discovery mode Run the following command and
+redirect the output into the catalog file ```shell script tap-mongodb --config
+~/config.json --discover > ~/catalog.json ``` Your catalog file should now look
+like this: ```json { "streams": [ { "table_name": "
```

### Comparing `pipelinewise-tap-mongodb-1.3.0/pipelinewise_tap_mongodb.egg-info/SOURCES.txt` & `pipelinewise_tap_mongodb-1.4.0/pipelinewise_tap_mongodb.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -11,8 +11,9 @@
 tap_mongodb/config_utils.py
 tap_mongodb/db_utils.py
 tap_mongodb/errors.py
 tap_mongodb/stream_utils.py
 tap_mongodb/sync_strategies/change_streams.py
 tap_mongodb/sync_strategies/common.py
 tap_mongodb/sync_strategies/full_table.py
-tap_mongodb/sync_strategies/incremental.py
+tap_mongodb/sync_strategies/incremental.py
+tests/test_connection_string.py
```

### Comparing `pipelinewise-tap-mongodb-1.3.0/setup.py` & `pipelinewise_tap_mongodb-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 with open('README.md', 'r') as fh:
     long_desc = fh.read()
 
 setup(name='pipelinewise-tap-mongodb',
-      version='1.3.0',
+      version='1.4.0',
       description='Singer.io tap for extracting data from MongoDB - Pipelinewise compatible',
       long_description=long_desc,
       long_description_content_type='text/markdown',
       author='Wise',
       url='https://github.com/transferwise/pipelinewise-tap-mongodb',
       classifiers=[
           'Programming Language :: Python :: 3 :: Only',
           'Programming Language :: Python :: 3.6',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
       ],
       py_modules=['tap_mongodb'],
       install_requires=[
           'pipelinewise-singer-python==1.*',
-          'pymongo==3.12.*',
+          'pymongo==4.7.*',
           'tzlocal==2.1.*',
           'terminaltables==3.1.*',
           'dnspython==2.1.*',
       ],
       extras_require={
           'dev': [
               'pylint==2.12',
```

### Comparing `pipelinewise-tap-mongodb-1.3.0/tap_mongodb/__init__.py` & `pipelinewise_tap_mongodb-1.4.0/tap_mongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mongodb-1.3.0/tap_mongodb/config_utils.py` & `pipelinewise_tap_mongodb-1.4.0/tap_mongodb/config_utils.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mongodb-1.3.0/tap_mongodb/db_utils.py` & `pipelinewise_tap_mongodb-1.4.0/tap_mongodb/db_utils.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mongodb-1.3.0/tap_mongodb/errors.py` & `pipelinewise_tap_mongodb-1.4.0/tap_mongodb/errors.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mongodb-1.3.0/tap_mongodb/stream_utils.py` & `pipelinewise_tap_mongodb-1.4.0/tap_mongodb/stream_utils.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mongodb-1.3.0/tap_mongodb/sync_strategies/change_streams.py` & `pipelinewise_tap_mongodb-1.4.0/tap_mongodb/sync_strategies/change_streams.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mongodb-1.3.0/tap_mongodb/sync_strategies/common.py` & `pipelinewise_tap_mongodb-1.4.0/tap_mongodb/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mongodb-1.3.0/tap_mongodb/sync_strategies/full_table.py` & `pipelinewise_tap_mongodb-1.4.0/tap_mongodb/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mongodb-1.3.0/tap_mongodb/sync_strategies/incremental.py` & `pipelinewise_tap_mongodb-1.4.0/tap_mongodb/sync_strategies/incremental.py`

 * *Files identical despite different names*


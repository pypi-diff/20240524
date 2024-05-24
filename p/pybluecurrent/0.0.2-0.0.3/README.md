# Comparing `tmp/pybluecurrent-0.0.2.tar.gz` & `tmp/pybluecurrent-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybluecurrent-0.0.2.tar", last modified: Mon Oct  9 15:11:50 2023, max compression
+gzip compressed data, was "pybluecurrent-0.0.3.tar", last modified: Fri May 24 11:07:01 2024, max compression
```

## Comparing `pybluecurrent-0.0.2.tar` & `pybluecurrent-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 15:11:50.134039 pybluecurrent-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 15:11:50.122038 pybluecurrent-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 15:11:50.126038 pybluecurrent-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2023-10-09 15:11:37.000000 pybluecurrent-0.0.2/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      533 2023-10-09 15:11:37.000000 pybluecurrent-0.0.2/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2023-10-09 15:11:37.000000 pybluecurrent-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      852 2023-10-09 15:11:37.000000 pybluecurrent-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-10-09 15:11:37.000000 pybluecurrent-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12297 2023-10-09 15:11:50.130039 pybluecurrent-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11330 2023-10-09 15:11:37.000000 pybluecurrent-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2023-10-09 15:11:37.000000 pybluecurrent-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-09 15:11:50.134039 pybluecurrent-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 15:11:50.122038 pybluecurrent-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 15:11:50.130039 pybluecurrent-0.0.2/src/pybluecurrent/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-10-09 15:11:37.000000 pybluecurrent-0.0.2/src/pybluecurrent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-09 15:11:50.000000 pybluecurrent-0.0.2/src/pybluecurrent/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    19891 2023-10-09 15:11:37.000000 pybluecurrent-0.0.2/src/pybluecurrent/client.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-10-09 15:11:37.000000 pybluecurrent-0.0.2/src/pybluecurrent/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-09 15:11:37.000000 pybluecurrent-0.0.2/src/pybluecurrent/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2023-10-09 15:11:37.000000 pybluecurrent-0.0.2/src/pybluecurrent/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 15:11:50.130039 pybluecurrent-0.0.2/src/pybluecurrent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12297 2023-10-09 15:11:50.000000 pybluecurrent-0.0.2/src/pybluecurrent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      571 2023-10-09 15:11:50.000000 pybluecurrent-0.0.2/src/pybluecurrent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-09 15:11:50.000000 pybluecurrent-0.0.2/src/pybluecurrent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-10-09 15:11:50.000000 pybluecurrent-0.0.2/src/pybluecurrent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-10-09 15:11:50.000000 pybluecurrent-0.0.2/src/pybluecurrent.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-09 15:11:50.130039 pybluecurrent-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2023-10-09 15:11:37.000000 pybluecurrent-0.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6625 2023-10-09 15:11:37.000000 pybluecurrent-0.0.2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2023-10-09 15:11:37.000000 pybluecurrent-0.0.2/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:07:01.881958 pybluecurrent-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:07:01.877958 pybluecurrent-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:07:01.877958 pybluecurrent-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-24 11:06:57.000000 pybluecurrent-0.0.3/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-24 11:06:57.000000 pybluecurrent-0.0.3/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-24 11:06:57.000000 pybluecurrent-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-24 11:06:57.000000 pybluecurrent-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-24 11:06:57.000000 pybluecurrent-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12816 2024-05-24 11:07:01.881958 pybluecurrent-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11849 2024-05-24 11:06:57.000000 pybluecurrent-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-24 11:06:57.000000 pybluecurrent-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 11:07:01.881958 pybluecurrent-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:07:01.877958 pybluecurrent-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:07:01.881958 pybluecurrent-0.0.3/src/pybluecurrent/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-24 11:06:57.000000 pybluecurrent-0.0.3/src/pybluecurrent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-24 11:07:01.000000 pybluecurrent-0.0.3/src/pybluecurrent/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20300 2024-05-24 11:06:57.000000 pybluecurrent-0.0.3/src/pybluecurrent/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-24 11:06:57.000000 pybluecurrent-0.0.3/src/pybluecurrent/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 11:06:57.000000 pybluecurrent-0.0.3/src/pybluecurrent/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-24 11:06:57.000000 pybluecurrent-0.0.3/src/pybluecurrent/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:07:01.881958 pybluecurrent-0.0.3/src/pybluecurrent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12816 2024-05-24 11:07:01.000000 pybluecurrent-0.0.3/src/pybluecurrent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-24 11:07:01.000000 pybluecurrent-0.0.3/src/pybluecurrent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 11:07:01.000000 pybluecurrent-0.0.3/src/pybluecurrent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-24 11:07:01.000000 pybluecurrent-0.0.3/src/pybluecurrent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-24 11:07:01.000000 pybluecurrent-0.0.3/src/pybluecurrent.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:07:01.881958 pybluecurrent-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-24 11:06:57.000000 pybluecurrent-0.0.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-05-24 11:06:57.000000 pybluecurrent-0.0.3/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-24 11:06:57.000000 pybluecurrent-0.0.3/tests/test_utilities.py
```

### Comparing `pybluecurrent-0.0.2/.github/workflows/publish.yaml` & `pybluecurrent-0.0.3/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `pybluecurrent-0.0.2/.github/workflows/test.yaml` & `pybluecurrent-0.0.3/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `pybluecurrent-0.0.2/.gitignore` & `pybluecurrent-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pybluecurrent-0.0.2/.pre-commit-config.yaml` & `pybluecurrent-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pybluecurrent-0.0.2/LICENSE` & `pybluecurrent-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pybluecurrent-0.0.2/PKG-INFO` & `pybluecurrent-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybluecurrent
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python client for BlueCurrent charge points.
 Author-email: Rogier van der Geer <rogier@vander-geer.nl>
 License: MIT
 Project-URL: Repository, https://github.com/rogiervandergeer/pybluecurrent
 Keywords: api,blue current,electric vehicle,ev
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -17,16 +17,16 @@
 Requires-Dist: asyncio-multisubscriber-queue>=0.4.1
 Requires-Dist: requests>=2.31.0
 Requires-Dist: sjcl>=0.2.1
 Requires-Dist: websockets>=11.0.3
 Provides-Extra: dev
 Requires-Dist: black==23.3.0; extra == "dev"
 Requires-Dist: pre-commit>=3.3.3; extra == "dev"
-Requires-Dist: pytest>=7.3.1; extra == "dev"
-Requires-Dist: pytest-asyncio>=0.21.1; extra == "dev"
+Requires-Dist: pytest==8.1.2; extra == "dev"
+Requires-Dist: pytest-asyncio==0.21.1; extra == "dev"
 
 # pybluecurrent
 
 Python client for [BlueCurrent](https://www.bluecurrent.nl) charge points.
 
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/rogiervandergeer/pybluecurrent/test.yaml) 
 ![PyPI](https://img.shields.io/pypi/v/pybluecurrent)
@@ -55,14 +55,15 @@
  - [Asynchronous](#asynchronous)
    - [`get_account`](#getaccount---get-your-account-information)
    - [`get_charge_cards`](#getchargecards---get-your-charge-cards)
    - [`get_charge_points`](#getchargepoints---get-your-charge-points)
    - [`get_charge_point_settings`](#getchargepointsettings---get-the-settings-of-a-charge-point)
    - [`get_grid_status`](#getgridstatus---get-the-grid-status-associated-to-a-charge-point)
    - [`get_sustainability_status`](#getsustainabilitystatus---get-statistics-on-the-sustainability-of-all-your-charge-points)
+   - [`set_plug_and_charge_charge_card`](#setplugandchargechargecard---set-the-charge-card-for-plug-and-charge)
    - [`set_status`](#setstatus---enable-or-disable-a-charge-point)
  - [Synchronous](#synchronous)
    - [`login`](#login---log-in)
    - [`get_charge_point_status`](#getchargepointstatus---get-the-status-of-a-charge-point)
    - [`get_contracts`](#getcontracts---get-your-contracts)
    - [`get_grids`](#getgrids---get-your-grid-connections)
    - [`get_transactions`](#gettransactions---get-a-list-of-transactions)
@@ -163,15 +164,15 @@
 
 #### `get_charge_point_settings` - Get the settings of a charge point.
 
 All the information returned by this endpoint is already included 
 in the response of [`get_charge_points`](#getchargepoints---get-your-charge-points).
 
 ```python
-async def get_charge_point_settings(self, evse_id: str) -> dict[str, bool | dict | str]
+async def get_charge_point_settings(self, evse_id: str) -> dict[str, bool | dict[str, Any] | str]
 ```
 
 ##### Arguments
 - `evse_id`: The ID of the charge point.
 
 ##### Returns
 A dictionary describing the settings:
@@ -224,14 +225,22 @@
 ```python
 async def get_sustainability_status(self) -> dict[str, float | int]
 ```
 
 ##### Returns
 A dictionary with two keys: `{"trees": 1, "co2": 12.345}`
 
+#### `set_plug_and_charge_charge_card` - Set the charge card for plug-and-charge
+
+```python
+async def set_plug_and_charge_charge_card(self, evse_id: str, uid: str | None = None) -> None
+```
+
+Sets the plug-and-charge card for the charge point. The uid must be a `uid` of one of your charge cards (see [`get_charge_cards`](#getchargecards---get-your-charge-cards)) or `None` to use no charge card.
+
 #### `set_status` - Enable or disable a charge point.
 
 ```python
 async def set_status(self, evse_id: str, enabled: bool) -> None
 ```
 
 ##### Arguments
```

### Comparing `pybluecurrent-0.0.2/README.md` & `pybluecurrent-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
  - [Asynchronous](#asynchronous)
    - [`get_account`](#getaccount---get-your-account-information)
    - [`get_charge_cards`](#getchargecards---get-your-charge-cards)
    - [`get_charge_points`](#getchargepoints---get-your-charge-points)
    - [`get_charge_point_settings`](#getchargepointsettings---get-the-settings-of-a-charge-point)
    - [`get_grid_status`](#getgridstatus---get-the-grid-status-associated-to-a-charge-point)
    - [`get_sustainability_status`](#getsustainabilitystatus---get-statistics-on-the-sustainability-of-all-your-charge-points)
+   - [`set_plug_and_charge_charge_card`](#setplugandchargechargecard---set-the-charge-card-for-plug-and-charge)
    - [`set_status`](#setstatus---enable-or-disable-a-charge-point)
  - [Synchronous](#synchronous)
    - [`login`](#login---log-in)
    - [`get_charge_point_status`](#getchargepointstatus---get-the-status-of-a-charge-point)
    - [`get_contracts`](#getcontracts---get-your-contracts)
    - [`get_grids`](#getgrids---get-your-grid-connections)
    - [`get_transactions`](#gettransactions---get-a-list-of-transactions)
@@ -137,15 +138,15 @@
 
 #### `get_charge_point_settings` - Get the settings of a charge point.
 
 All the information returned by this endpoint is already included 
 in the response of [`get_charge_points`](#getchargepoints---get-your-charge-points).
 
 ```python
-async def get_charge_point_settings(self, evse_id: str) -> dict[str, bool | dict | str]
+async def get_charge_point_settings(self, evse_id: str) -> dict[str, bool | dict[str, Any] | str]
 ```
 
 ##### Arguments
 - `evse_id`: The ID of the charge point.
 
 ##### Returns
 A dictionary describing the settings:
@@ -198,14 +199,22 @@
 ```python
 async def get_sustainability_status(self) -> dict[str, float | int]
 ```
 
 ##### Returns
 A dictionary with two keys: `{"trees": 1, "co2": 12.345}`
 
+#### `set_plug_and_charge_charge_card` - Set the charge card for plug-and-charge
+
+```python
+async def set_plug_and_charge_charge_card(self, evse_id: str, uid: str | None = None) -> None
+```
+
+Sets the plug-and-charge card for the charge point. The uid must be a `uid` of one of your charge cards (see [`get_charge_cards`](#getchargecards---get-your-charge-cards)) or `None` to use no charge card.
+
 #### `set_status` - Enable or disable a charge point.
 
 ```python
 async def set_status(self, evse_id: str, enabled: bool) -> None
 ```
 
 ##### Arguments
```

### Comparing `pybluecurrent-0.0.2/pyproject.toml` & `pybluecurrent-0.0.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "requests>=2.31.0",
     "sjcl>=0.2.1",
     "websockets>=11.0.3",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
-dev = ["black==23.3.0", "pre-commit>=3.3.3", "pytest>=7.3.1", "pytest-asyncio>=0.21.1"]
+dev = ["black==23.3.0", "pre-commit>=3.3.3", "pytest==8.1.2", "pytest-asyncio==0.21.1"]
 
 [project.urls]
 Repository = "https://github.com/rogiervandergeer/pybluecurrent"
 
 [tool.setuptools.package-data]
 pybluecurrent = ["py.typed"]
```

### Comparing `pybluecurrent-0.0.2/src/pybluecurrent/client.py` & `pybluecurrent-0.0.3/src/pybluecurrent/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         )
 
     async def get_charge_points(self) -> list[dict[str, bool | dict | str]]:
         """
         Get a list of your charge points.
 
         Returns:
-            A list of dictionaries, each representing a charge card:
+            A list of dictionaries, each representing a charge point:
             {
                 "evse_id": "BCU123456",
                 "name": "",
                 "model_type": "H:MOVE-C32T2",
                 "chargepoint_type": "HIDDEN",
                 "is_cable": True,
                 "public_charging": {"value": False, "permission": "write"},
@@ -129,15 +129,15 @@
                              "zipcode": "3526KS", "city": "Utrecht", "country": "NL"},
                 "delayed_charging": {"value": False, "permission": "none"}
             }
         """
         await self._send(dict(command="GET_CHARGE_POINTS"), token=True)
         return (await self._receive("CHARGE_POINTS"))["data"]
 
-    async def get_charge_point_settings(self, evse_id: str) -> dict[str, bool | dict | str]:
+    async def get_charge_point_settings(self, evse_id: str) -> dict[str, bool | dict[str, Any] | str]:
         """
         Get the settings of a charge point.
 
         All of this information is already included in the response of get_charge_points.
 
         Args:
             evse_id: A charge point ID.
@@ -189,32 +189,42 @@
         return (await self._receive("GRID_STATUS"))["data"]
 
     async def get_sessions(self, evse_id: str):
         """Does not work"""
         await self._send(dict(command="GET_SESSIONS"), token=True)
         return await self._receive("SESSIONS")
 
-    async def get_status(self, evse_id: str):
-        """Returns a useless object with evse_id and your full name"""
-        await self._send(dict(command="GET_STATUS", evse_id=evse_id), token=True)
-        return await self._receive("STATUS")
-
     async def get_sustainability_status(self) -> dict[str, float | int]:
         """
         Get statistics on the sustainability of all your charge points.
 
         Returns:
             A dictionary with two keys:
             {"trees": 1, "co2": 12.345}
         """
         await self._send(dict(command="GET_SUSTAINABILITY_STATUS"), token=True)
         result = await self._receive("SUSTAINABILITY_STATUS")
         result.pop("object")
         return result
 
+    async def set_plug_and_charge_charge_card(self, evse_id: str, uid: str | None = None) -> None:
+        """
+        Set a plug-and-charge charge card for the charge point.
+
+        Args:
+            evse_id: A charge point ID.
+            uid: A charge card UID or None (for no charge card). Defaults to None.
+        """
+        await self._send(
+            dict(command="SET_PLUG_AND_CHARGE_CHARGE_CARD", evse_id=evse_id, token_uid=uid or "BCU-APP"), token=True
+        )
+        result = await self._receive("STATUS_SET_PLUG_AND_CHARGE_CHARGE_CARD")
+        if not result.get("success"):
+            raise BlueCurrentException(result)
+
     async def set_status(self, evse_id: str, enabled: bool) -> None:
         """
         Enable or disable a charge point.
 
         Args:
             evse_id: The ID of the charge point.
             enabled: Boolean that indicates the desired status.
```

### Comparing `pybluecurrent-0.0.2/src/pybluecurrent/utilities.py` & `pybluecurrent-0.0.3/src/pybluecurrent/utilities.py`

 * *Files identical despite different names*

### Comparing `pybluecurrent-0.0.2/src/pybluecurrent.egg-info/PKG-INFO` & `pybluecurrent-0.0.3/src/pybluecurrent.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybluecurrent
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python client for BlueCurrent charge points.
 Author-email: Rogier van der Geer <rogier@vander-geer.nl>
 License: MIT
 Project-URL: Repository, https://github.com/rogiervandergeer/pybluecurrent
 Keywords: api,blue current,electric vehicle,ev
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -17,16 +17,16 @@
 Requires-Dist: asyncio-multisubscriber-queue>=0.4.1
 Requires-Dist: requests>=2.31.0
 Requires-Dist: sjcl>=0.2.1
 Requires-Dist: websockets>=11.0.3
 Provides-Extra: dev
 Requires-Dist: black==23.3.0; extra == "dev"
 Requires-Dist: pre-commit>=3.3.3; extra == "dev"
-Requires-Dist: pytest>=7.3.1; extra == "dev"
-Requires-Dist: pytest-asyncio>=0.21.1; extra == "dev"
+Requires-Dist: pytest==8.1.2; extra == "dev"
+Requires-Dist: pytest-asyncio==0.21.1; extra == "dev"
 
 # pybluecurrent
 
 Python client for [BlueCurrent](https://www.bluecurrent.nl) charge points.
 
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/rogiervandergeer/pybluecurrent/test.yaml) 
 ![PyPI](https://img.shields.io/pypi/v/pybluecurrent)
@@ -55,14 +55,15 @@
  - [Asynchronous](#asynchronous)
    - [`get_account`](#getaccount---get-your-account-information)
    - [`get_charge_cards`](#getchargecards---get-your-charge-cards)
    - [`get_charge_points`](#getchargepoints---get-your-charge-points)
    - [`get_charge_point_settings`](#getchargepointsettings---get-the-settings-of-a-charge-point)
    - [`get_grid_status`](#getgridstatus---get-the-grid-status-associated-to-a-charge-point)
    - [`get_sustainability_status`](#getsustainabilitystatus---get-statistics-on-the-sustainability-of-all-your-charge-points)
+   - [`set_plug_and_charge_charge_card`](#setplugandchargechargecard---set-the-charge-card-for-plug-and-charge)
    - [`set_status`](#setstatus---enable-or-disable-a-charge-point)
  - [Synchronous](#synchronous)
    - [`login`](#login---log-in)
    - [`get_charge_point_status`](#getchargepointstatus---get-the-status-of-a-charge-point)
    - [`get_contracts`](#getcontracts---get-your-contracts)
    - [`get_grids`](#getgrids---get-your-grid-connections)
    - [`get_transactions`](#gettransactions---get-a-list-of-transactions)
@@ -163,15 +164,15 @@
 
 #### `get_charge_point_settings` - Get the settings of a charge point.
 
 All the information returned by this endpoint is already included 
 in the response of [`get_charge_points`](#getchargepoints---get-your-charge-points).
 
 ```python
-async def get_charge_point_settings(self, evse_id: str) -> dict[str, bool | dict | str]
+async def get_charge_point_settings(self, evse_id: str) -> dict[str, bool | dict[str, Any] | str]
 ```
 
 ##### Arguments
 - `evse_id`: The ID of the charge point.
 
 ##### Returns
 A dictionary describing the settings:
@@ -224,14 +225,22 @@
 ```python
 async def get_sustainability_status(self) -> dict[str, float | int]
 ```
 
 ##### Returns
 A dictionary with two keys: `{"trees": 1, "co2": 12.345}`
 
+#### `set_plug_and_charge_charge_card` - Set the charge card for plug-and-charge
+
+```python
+async def set_plug_and_charge_charge_card(self, evse_id: str, uid: str | None = None) -> None
+```
+
+Sets the plug-and-charge card for the charge point. The uid must be a `uid` of one of your charge cards (see [`get_charge_cards`](#getchargecards---get-your-charge-cards)) or `None` to use no charge card.
+
 #### `set_status` - Enable or disable a charge point.
 
 ```python
 async def set_status(self, evse_id: str, enabled: bool) -> None
 ```
 
 ##### Arguments
```

### Comparing `pybluecurrent-0.0.2/src/pybluecurrent.egg-info/SOURCES.txt` & `pybluecurrent-0.0.3/src/pybluecurrent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybluecurrent-0.0.2/tests/conftest.py` & `pybluecurrent-0.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pybluecurrent-0.0.2/tests/test_client.py` & `pybluecurrent-0.0.3/tests/test_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -67,19 +67,14 @@
     @mark.asyncio
     async def test_get_grid_status(self, connected_client: BlueCurrentClient, evse_id: str):
         status = await connected_client.get_grid_status(evse_id=evse_id)
         assert "grid_actual_p1" in status
         assert "id" in status
 
     @mark.asyncio
-    async def test_get_status(self, connected_client: BlueCurrentClient, evse_id: str):
-        status = await connected_client.get_status(evse_id=evse_id)
-        assert status["evse_id"] == evse_id
-
-    @mark.asyncio
     async def test_get_charge_point_settings(self, connected_client: BlueCurrentClient, evse_id: str):
         settings = await connected_client.get_charge_point_settings(evse_id=evse_id)
         assert isinstance(settings, dict)
         assert settings["evse_id"] == evse_id
 
     @mark.asyncio
     @mark.skip("Does not work")
@@ -101,14 +96,49 @@
     @mark.asyncio
     @mark.skip("Do not change chargepoint status.")
     async def test_soft_reset(self, connected_client: BlueCurrentClient, evse_id: str):
         _ = await connected_client.soft_reset(evse_id=evse_id)
 
     @mark.asyncio
     @mark.skipif(environ.get("BLUECURRENT_READ_ONLY", "TRUE") != "FALSE", reason="Running read-only tests.")
+    async def test_set_plug_and_charge_card(self, connected_client: BlueCurrentClient, evse_id: str):
+        async def _get_plug_and_charge_card_uid() -> str | None:
+            settings = await connected_client.get_charge_point_settings(evse_id=evse_id)
+            try:
+                return settings["plug_and_charge_charge_card"]["uid"]  # type: ignore
+            except KeyError:
+                return None
+
+        # Get the original card, if any
+        before_card = await _get_plug_and_charge_card_uid()
+
+        # Get all possible cards, including no card
+        charge_cards = await connected_client.get_charge_cards()
+        if len(charge_cards) == 0:
+            skip(reason="No charge cards.")
+        uids: list[str | None] = [charge_card["uid"] for charge_card in charge_cards] + [None]  # type: ignore
+        # Set each card as plug_and_charge_card
+        for uid in uids:
+            if uid != before_card:
+                await connected_client.set_plug_and_charge_charge_card(evse_id=evse_id, uid=uid)
+                assert await _get_plug_and_charge_card_uid() == uid
+        # Set the original card as plug_and_charge_card
+        await connected_client.set_plug_and_charge_charge_card(evse_id=evse_id, uid=before_card)
+        assert await _get_plug_and_charge_card_uid() == before_card
+
+    @mark.asyncio
+    @mark.skipif(environ.get("BLUECURRENT_READ_ONLY", "TRUE") != "FALSE", reason="Running read-only tests.")
+    async def test_set_invalid_plug_and_charge_card(self, connected_client: BlueCurrentClient, evse_id: str):
+        settings = await connected_client.get_charge_point_settings(evse_id=evse_id)
+        with raises(BlueCurrentException):
+            await connected_client.set_plug_and_charge_charge_card(evse_id=evse_id, uid="INVALID_CARD")
+        assert await connected_client.get_charge_point_settings(evse_id=evse_id) == settings
+
+    @mark.asyncio
+    @mark.skipif(environ.get("BLUECURRENT_READ_ONLY", "TRUE") != "FALSE", reason="Running read-only tests.")
     async def test_set_status(self, connected_client: BlueCurrentClient, evse_id: str):
         before_status = connected_client.get_charge_point_status(evse_id=evse_id)
         if before_status["activity"] != "available":
             skip(reason="Only perform this test if the charge point is available.")
         await connected_client.set_status(evse_id=evse_id, enabled=False)
         assert connected_client.get_charge_point_status(evse_id=evse_id)["activity"] == "unavailable"
         await connected_client.set_status(evse_id=evse_id, enabled=True)
```

### Comparing `pybluecurrent-0.0.2/tests/test_utilities.py` & `pybluecurrent-0.0.3/tests/test_utilities.py`

 * *Files identical despite different names*


# Comparing `tmp/pychlorinator-0.2.8.tar.gz` & `tmp/pychlorinator-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychlorinator-0.2.8.tar", max compression
+gzip compressed data, was "pychlorinator-0.2.9.tar", max compression
```

## Comparing `pychlorinator-0.2.8.tar` & `pychlorinator-0.2.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1078 2024-02-04 05:23:55.439162 pychlorinator-0.2.8/LICENSE
--rw-r--r--   0        0        0      816 2024-02-04 05:23:55.439162 pychlorinator-0.2.8/README.md
--rw-r--r--   0        0        0        0 2024-02-04 05:23:55.439162 pychlorinator-0.2.8/pychlorinator/__init__.py
--rw-r--r--   0        0        0     6114 2024-02-04 05:23:55.439162 pychlorinator-0.2.8/pychlorinator/chlorinator.py
--rw-r--r--   0        0        0    11337 2024-02-04 05:23:55.439162 pychlorinator-0.2.8/pychlorinator/chlorinator_parsers.py
--rw-r--r--   0        0        0    40219 2024-02-04 05:23:55.439162 pychlorinator-0.2.8/pychlorinator/halo_parsers.py
--rw-r--r--   0        0        0    10978 2024-02-04 05:23:55.439162 pychlorinator-0.2.8/pychlorinator/halochlorinator.py
--rw-r--r--   0        0        0      538 2024-02-04 05:23:55.439162 pychlorinator-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1537 1970-01-01 00:00:00.000000 pychlorinator-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-02-10 04:35:42.730943 pychlorinator-0.2.9/LICENSE
+-rw-r--r--   0        0        0      816 2024-02-10 04:35:42.730943 pychlorinator-0.2.9/README.md
+-rw-r--r--   0        0        0        0 2024-02-10 04:35:42.730943 pychlorinator-0.2.9/pychlorinator/__init__.py
+-rw-r--r--   0        0        0     6114 2024-02-10 04:35:42.730943 pychlorinator-0.2.9/pychlorinator/chlorinator.py
+-rw-r--r--   0        0        0    11337 2024-02-10 04:35:42.730943 pychlorinator-0.2.9/pychlorinator/chlorinator_parsers.py
+-rw-r--r--   0        0        0    42692 2024-02-10 04:35:42.730943 pychlorinator-0.2.9/pychlorinator/halo_parsers.py
+-rw-r--r--   0        0        0    12057 2024-02-10 04:35:42.730943 pychlorinator-0.2.9/pychlorinator/halochlorinator.py
+-rw-r--r--   0        0        0      538 2024-02-10 04:35:42.730943 pychlorinator-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     1537 1970-01-01 00:00:00.000000 pychlorinator-0.2.9/PKG-INFO
```

### Comparing `pychlorinator-0.2.8/LICENSE` & `pychlorinator-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pychlorinator-0.2.8/README.md` & `pychlorinator-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pychlorinator-0.2.8/pychlorinator/chlorinator.py` & `pychlorinator-0.2.9/pychlorinator/chlorinator.py`

 * *Files identical despite different names*

### Comparing `pychlorinator-0.2.8/pychlorinator/chlorinator_parsers.py` & `pychlorinator-0.2.9/pychlorinator/chlorinator_parsers.py`

 * *Files identical despite different names*

### Comparing `pychlorinator-0.2.8/pychlorinator/halo_parsers.py` & `pychlorinator-0.2.9/pychlorinator/halo_parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,33 @@
     NoAction = 0
     Off = 1
     Auto = 2
     On = 3
     Low = 4
     Medium = 5
     High = 6
+    Pool = 7
+    Spa = 8
+
+
+class HeaterAppActions(IntEnum):
+    NoAction = 0
+    HeaterPumpOff = 1
+    HeaterPumpAuto = 2
+    HeaterPumpOn = 3
+    HeaterOff = 4
+    HeaterOn = 5
+    IncreaseSetpoint = 6
+    DecreaseSetpoint = 7
+    Pool = 8
+    Spa = 9
+    DisableUseTimers = 10
+    EnableUseTimers = 11
+    ModeHeating = 12
+    ModeCooling = 13
 
 
 class ChlorinatorAction:
     """Represent an action command"""
 
     # period_minutes only used for setting ChlorinatorActions:DisableAcidDosingForPeriod
 
@@ -34,14 +53,31 @@
 
     def __bytes__(self):
         fmt = "=3s B i 12x"
         _LOGGER.info("Selected Action is %s", self.action)
         return struct.pack(fmt, self.header_bytes, self.action, self.period_minutes)
 
 
+class HeaterAction:
+    """Represent an Heater action command"""
+
+    def __init__(
+        self,
+        action: HeaterAppActions = HeaterAppActions.NoAction,
+        header_bytes: bytes = b"\x03\xF6\x01",
+    ) -> None:
+        self.action = action
+        self.header_bytes = header_bytes
+
+    def __bytes__(self):
+        fmt = "=3s B 16x"
+        _LOGGER.info("Selected Heater Action is %s", self.action)
+        return struct.pack(fmt, self.header_bytes, self.action)
+
+
 class ScanResponse:
     _fmt = "<BBBBBBI4sBBBBBBB"
 
     def __init__(self, data) -> None:
         fields = struct.unpack(self._fmt, data[: struct.calcsize(self._fmt)])
         (
             # self.ManufacturerIdLo,
@@ -895,25 +931,34 @@
         )
         self.IgnitionServiceRequired = bool(
             self.HeaterStatusFlagValues.IgnitionServiceRequired & self.HeaterStatusFlag
         )
         self.CoolingAvailable = bool(
             self.HeaterStatusFlagValues.CoolingAvailable & self.HeaterStatusFlag
         )
-        self.HeaterMode = Mode(self.HeaterMode)  ## to confirm if mode enum
+        self.HeaterMode = self.HeaterModeValues(
+            self.HeaterMode
+        )  ##Looks like just on / off
         self.HeaterPumpMode = Mode(self.HeaterPumpMode)
         self.HeatPumpMode = self.HeatpumpModeValues(self.HeatPumpMode)
         self.HeaterForced = self.HeaterForcedEnum(self.HeaterForced)
         self.HeaterWaterTempValid = self.TempValidEnum(self.HeaterWaterTempValid)
         self.HeaterWaterTemp /= 10
 
     @property
     def heater_status_flags(self):
         return HeaterStateCharacteristic.HeaterStatusFlagValues(self.HeaterStatusFlag)
 
+    class HeaterModeValues(Enum):
+        Off = 0
+        On = 1
+
+        def __str__(self):
+            return self.name
+
     class HeaterStatusFlagValues(IntFlag):
         HeaterOn = 1
         Pressure = 2
         GasValve = 4
         Flame = 8
         Lockout = 16
         GeneralServiceRequired = 32
@@ -1229,14 +1274,57 @@
         WaterFeature = 4
         Waterfall = 5
 
         def __str__(self):
             return self.name
 
 
+class GPOCustomNameStruct:
+    def __init__(self, data, fmt="<BBBB12s"):
+        # Format: 4 bytes followed by a 12-byte string
+        (
+            self.DeviceType,
+            self.Index,
+            self.MessageNumber,
+            self.CustomNameLength,
+            self.CustomNameFragment,
+        ) = struct.unpack(fmt, data[: struct.calcsize(fmt)])
+
+        # Decode the custom name fragment, removing any null bytes
+        self.CustomNameFragment = self.CustomNameFragment.decode("utf-8").rstrip("\x00")
+
+
+class RelayCustomNameStruct:
+    def __init__(self, data, fmt="<BBB13s"):
+        # Format: 4 bytes followed by a 12-byte string
+        (
+            self.Index,
+            self.MessageNumber,
+            self.CustomNameLength,
+            self.CustomNameFragment,
+        ) = struct.unpack(fmt, data[: struct.calcsize(fmt)])
+
+        # Decode the custom name fragment, removing any null bytes
+        self.CustomNameFragment = self.CustomNameFragment.decode("utf-8").rstrip("\x00")
+
+
+class ValveCustomNameStruct:
+    def __init__(self, data, fmt="<BBB13s"):
+        # Format: 4 bytes followed by a 12-byte string
+        (
+            self.Index,
+            self.MessageNumber,
+            self.CustomNameLength,
+            self.CustomNameFragment,
+        ) = struct.unpack(fmt, data[: struct.calcsize(fmt)])
+
+        # Decode the custom name fragment, removing any null bytes
+        self.CustomNameFragment = self.CustomNameFragment.decode("utf-8").rstrip("\x00")
+
+
 class DeviceProtocol(Enum):
     """ScanResponse Device Protocol"""
 
     Unknown = -1
     Protocol0 = 0
     Firmware57 = 1
     NextGen = 2
```

### Comparing `pychlorinator-0.2.8/pychlorinator/halochlorinator.py` & `pychlorinator-0.2.9/pychlorinator/halochlorinator.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     CellCharacteristic2,
     ChlorinatorAction,
     ChlorinatorActions,
     DeviceProfileCharacteristic2,
     EquipmentModeCharacteristic,
     EquipmentParameterCharacteristic,
     GPOSetupCharacteristic,
+    HeaterAction,
+    HeaterAppActions,
     HeaterCapabilitiesCharacteristic,
     HeaterConfigCharacteristic,
     HeaterCooldownStateCharacteristic,
     HeaterStateCharacteristic,
     LightCapabilitiesCharacteristic,
     LightSetupCharacteristic,
     LightStateCharacteristic,
@@ -122,14 +124,34 @@
 
             data = ChlorinatorAction(action).__bytes__()
             _LOGGER.debug("Data to write %s", data.hex())
             data = encrypt_characteristic(data, self._session_key)
             _LOGGER.debug("Encrypted data to write %s", data.hex())
             await client.write_gatt_char(UUID_RX_CHARACTERISTIC, data)
 
+    async def async_write_heater_action(self, action: HeaterAppActions):
+        """Connect to the Chlorinator and write an action command to it."""
+        while self._connected:
+            _LOGGER.debug("Already connected, Waiting")
+            await asyncio.sleep(5)
+
+        async with BleakClient(self._ble_device, timeout=10) as client:
+            self._session_key = await client.read_gatt_char(UUID_SLAVE_SESSION_KEY_2)
+            _LOGGER.debug("Got session key %s", self._session_key.hex())
+
+            mac = encrypt_mac_key(self._session_key, bytes(self._access_code, "utf_8"))
+            _LOGGER.debug("Mac key to write %s", mac)
+            await client.write_gatt_char(UUID_MASTER_AUTHENTICATION_2, mac)
+
+            data = HeaterAction(action).__bytes__()
+            _LOGGER.info("Data to write %s", data.hex())
+            data = encrypt_characteristic(data, self._session_key)
+            _LOGGER.debug("Encrypted data to write %s", data.hex())
+            await client.write_gatt_char(UUID_RX_CHARACTERISTIC, data)
+
     async def async_gatherdata(self) -> dict[str, Any]:
         """Connect to the Chlorinator to get data."""
         if self._ble_device is None:
             self._result = {}
             return self._result
 
         self._result = {}
```

### Comparing `pychlorinator-0.2.8/pyproject.toml` & `pychlorinator-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pychlorinator"
-version = "0.2.8"
+version = "0.2.9"
 description = ""
 authors = ["pbutterworth <3683210+pbutterworth@users.noreply.github.com>"]
 readme = "README.md"
 repository = "https://github.com/pbutterworth/pychlorinator"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `pychlorinator-0.2.8/PKG-INFO` & `pychlorinator-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pychlorinator
-Version: 0.2.8
+Version: 0.2.9
 Summary: 
 Home-page: https://github.com/pbutterworth/pychlorinator
 Author: pbutterworth
 Author-email: 3683210+pbutterworth@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pychlorinator Version: 0.2.8 Summary: Home-page:
+Metadata-Version: 2.1 Name: pychlorinator Version: 0.2.9 Summary: Home-page:
 https://github.com/pbutterworth/pychlorinator Author: pbutterworth Author-
 email: 3683210+pbutterworth@users.noreply.github.com Requires-Python:
 >=3.8,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: bleak (>=0.19.0) Requires-Dist: pycryptodome
```


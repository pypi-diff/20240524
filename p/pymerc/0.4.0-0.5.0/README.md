# Comparing `tmp/pymerc-0.4.0.tar.gz` & `tmp/pymerc-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymerc-0.4.0.tar", max compression
+gzip compressed data, was "pymerc-0.5.0.tar", max compression
```

## Comparing `pymerc-0.4.0.tar` & `pymerc-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,33 @@
--rw-r--r--   0        0        0     1096 2024-05-21 04:48:12.666119 pymerc-0.4.0/README.md
--rw-r--r--   0        0        0      381 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/api/base.py
--rw-r--r--   0        0        0     1225 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/api/buildings.py
--rw-r--r--   0        0        0      640 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/api/businesses.py
--rw-r--r--   0        0        0      571 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/api/map.py
--rw-r--r--   0        0        0     1279 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/api/models/buildings.py
--rw-r--r--   0        0        0      855 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/api/models/businesses.py
--rw-r--r--   0        0        0    18770 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/api/models/common.py
--rw-r--r--   0        0        0      593 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/api/models/map.py
--rw-r--r--   0        0        0     1396 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/api/models/player.py
--rw-r--r--   0        0        0     2692 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/api/models/static.py
--rw-r--r--   0        0        0     3131 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/api/models/towns.py
--rw-r--r--   0        0        0      483 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/api/player.py
--rw-r--r--   0        0        0     2210 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/api/static.py
--rw-r--r--   0        0        0     1830 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/api/towns.py
--rw-r--r--   0        0        0     5022 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/client.py
--rw-r--r--   0        0        0      107 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/exceptions.py
--rw-r--r--   0        0        0     2416 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/game/building.py
--rw-r--r--   0        0        0     2020 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/game/player.py
--rw-r--r--   0        0        0     3607 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/game/town.py
--rw-r--r--   0        0        0      599 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/util/data.py
--rw-r--r--   0        0        0     1602 2024-05-21 04:48:12.666119 pymerc-0.4.0/pymerc/util/towns.py
--rw-r--r--   0        0        0      777 2024-05-21 04:48:12.666119 pymerc-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1825 1970-01-01 00:00:00.000000 pymerc-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     4677 2024-05-24 21:36:31.962610 pymerc-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-24 21:36:31.962610 pymerc-0.5.0/pymerc/__init__.py
+-rw-r--r--   0        0        0      382 2024-05-24 21:36:31.962610 pymerc-0.5.0/pymerc/api/base.py
+-rw-r--r--   0        0        0     1985 2024-05-24 21:36:31.962610 pymerc-0.5.0/pymerc/api/buildings.py
+-rw-r--r--   0        0        0      607 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/businesses.py
+-rw-r--r--   0        0        0      571 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/map.py
+-rw-r--r--   0        0        0     1325 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/models/buildings.py
+-rw-r--r--   0        0        0      912 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/models/businesses.py
+-rw-r--r--   0        0        0    22082 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/models/common.py
+-rw-r--r--   0        0        0      593 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/models/map.py
+-rw-r--r--   0        0        0     1448 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/models/player.py
+-rw-r--r--   0        0        0     2693 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/models/static.py
+-rw-r--r--   0        0        0   128191 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/models/test.json
+-rw-r--r--   0        0        0     3140 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/models/towns.py
+-rw-r--r--   0        0        0     1732 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/models/transports.py
+-rw-r--r--   0        0        0      482 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/player.py
+-rw-r--r--   0        0        0     2377 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/static.py
+-rw-r--r--   0        0        0     5264 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/towns.py
+-rw-r--r--   0        0        0     1541 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/api/transports.py
+-rw-r--r--   0        0        0     5939 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/client.py
+-rw-r--r--   0        0        0      334 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/exceptions.py
+-rw-r--r--   0        0        0     7540 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/game/building.py
+-rw-r--r--   0        0        0     6779 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/game/exports.py
+-rw-r--r--   0        0        0     6826 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/game/imports.py
+-rw-r--r--   0        0        0     3889 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/game/player.py
+-rw-r--r--   0        0        0     2840 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/game/recipe.py
+-rw-r--r--   0        0        0    10978 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/game/storehouse.py
+-rw-r--r--   0        0        0     4588 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/game/town.py
+-rw-r--r--   0        0        0     9016 2024-05-24 21:36:31.966610 pymerc-0.5.0/pymerc/game/transport.py
+-rw-r--r--   0        0        0      600 2024-05-24 21:36:31.970610 pymerc-0.5.0/pymerc/util/data.py
+-rw-r--r--   0        0        0     1602 2024-05-24 21:36:31.970610 pymerc-0.5.0/pymerc/util/towns.py
+-rw-r--r--   0        0        0      835 2024-05-24 21:36:31.970610 pymerc-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5448 1970-01-01 00:00:00.000000 pymerc-0.5.0/PKG-INFO
```

### Comparing `pymerc-0.4.0/pymerc/api/buildings.py` & `pymerc-0.5.0/pymerc/api/buildings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from pydantic import TypeAdapter
-
 from pymerc.api.base import BaseAPI
 from pymerc.api.models import buildings, common
+from pymerc.exceptions import SetManagerFailedException
 from pymerc.util import data
 
 BASE_URL = "https://play.mercatorio.io/api/buildings/"
 
+
 class BuildingsAPI(BaseAPI):
     """A class for interacting with the buildings API endpoint."""
 
     async def get(self, id: int) -> buildings.Building:
         """Get a building by its ID.
 
         Args:
@@ -17,20 +17,44 @@
 
         Returns:
             Building: The building.
         """
         response = await self.client.get(f"{BASE_URL}{id}")
         return buildings.Building.model_validate(response.json())
 
-    async def set_manager(self, id: int, item: common.Item, manager: common.InventoryManager) -> bool:
+    async def get_operations(self, id: int) -> buildings.BuildingOperation:
+        """Get the operations for a building.
+
+        Args:
+            id (int): The ID of the building.
+
+        Returns:
+            BuildingOperation: The building operation information.
+        """
+        response = await self.client.get(f"{BASE_URL}{id}/operations")
+        return buildings.BuildingOperation.model_validate(response.json())
+
+    async def set_manager(
+        self, id: int, item: common.Item, manager: common.InventoryManager
+    ) -> buildings.Building:
         """Set the manager for an item in a building.
 
         Args:
             item (Item): The item.
             manager (InventoryManager): The manager.
 
         Returns:
-            bool: Whether the manager was set.
+            Building: The updated building.
         """
         json = data.convert_floats_to_strings(manager.model_dump(exclude_unset=True))
-        response = await self.client.patch(f"{BASE_URL}{id}/storage/inventory/{item.name.lower()}", json=json)
-        return response.status_code == 200
+        response = await self.client.patch(
+            f"{BASE_URL}{id}/storage/inventory/{item.value}", json=json
+        )
+
+        if response.status_code == 200:
+            return buildings.Building.model_validate(
+                response.json()["_embedded"][f"/buildings/{id}"]
+            )
+
+        raise SetManagerFailedException(
+            f"Failed to set manager for {item.name} on building {id}: {response.text}"
+        )
```

### Comparing `pymerc-0.4.0/pymerc/api/businesses.py` & `pymerc-0.5.0/pymerc/api/businesses.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from pydantic import TypeAdapter
 
 from pymerc.api.base import BaseAPI
 from pymerc.api.models import businesses
 
 BASE_URL = "https://play.mercatorio.io/api/businesses/"
```

### Comparing `pymerc-0.4.0/pymerc/api/map.py` & `pymerc-0.5.0/pymerc/api/map.py`

 * *Files identical despite different names*

### Comparing `pymerc-0.4.0/pymerc/api/models/buildings.py` & `pymerc-0.5.0/pymerc/api/models/buildings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
+
 from typing import Optional
 
 from pydantic import BaseModel
 
 from pymerc.api.models import common
 
 
 class Building(BaseModel):
     """Represents a building."""
 
     capacity: Optional[int] = None
     construction: Optional[BuildingConstruction] = None
-    delivery_cost: BuildingDeliveryCost
+    delivery_cost: common.DeliveryCost
     id: int
     land: Optional[list[common.Location]] = None
     name: str
     owner_id: int
     producer: Optional[common.Producer] = None
     provider_id: Optional[int] = None
     size: Optional[int] = None
@@ -33,19 +34,18 @@
     progress: int
     reference: str
     stage: str
     time: int
     upgrade_type: Optional[common.BuildingUpgradeType] = None
 
 
-class BuildingDeliveryCost(BaseModel):
-    """Represents the delivery cost of a building."""
-
-    land_distance: float
-
-
 class BuildingStorage(BaseModel):
     """Represents the storage of a building."""
 
     inventory: common.Inventory
     operations: list[str]
     reference: str
+
+
+class BuildingOperation(BaseModel):
+    total_flow: Optional[dict[common.Item, common.InventoryFlow]] = None
+    operations: Optional[list[common.Operation]] = None
```

### Comparing `pymerc-0.4.0/pymerc/api/models/common.py` & `pymerc-0.5.0/pymerc/api/models/common.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+
 from enum import Enum
 from typing import Optional
 
 from pydantic import BaseModel, Field
 
 
 class Asset(Enum):
@@ -213,15 +214,15 @@
     Ploughs = "ploughs"
     Protection = "protection"
     Resin = "resin"
     Rope = "rope"
     Salt = "salt"
     Scythes = "scythes"
     SilverBars = "silver bars"
-    SlackedLime = "slacked lime"
+    SlakedLime = "slaked lime"
     Snekkja = "snekkja"
     Spirits = "spirits"
     SteelIngots = "steel ingots"
     Stockfish = "stockfish"
     Swords = "swords"
     Tar = "tar"
     Thread = "thread"
@@ -241,14 +242,15 @@
 class ItemType(Enum):
     """Represents an item type."""
 
     Commodity = "commodity"
     Service = "service"
     Special = "special"
 
+
 class Recipe(Enum):
     BakeBread1 = "bake bread 1"
     BakeBread2 = "bake bread 2"
     BakePasties1 = "bake pasties 1"
     BakePasties2 = "bake pasties 2"
     BakePies1 = "bake pies 1"
     BindGarments1 = "bind garments 1"
@@ -290,14 +292,15 @@
     ButcherCattle1a = "butcher cattle 1a"
     ButcherCattle1b = "butcher cattle 1b"
     ButcherCattle2 = "butcher cattle 2"
     Carting1 = "carting 1"
     Carting2 = "carting 2"
     ChurnButter1 = "churn butter 1"
     ChurnButter2 = "churn butter 2"
+    CogOperations = "cog operations"
     CraftArms1 = "craft arms 1"
     CraftBelts1 = "craft belts 1"
     CraftBelts2 = "craft belts 2"
     CraftBelts3 = "craft belts 3"
     CraftCookware1 = "craft cookware 1"
     CraftFurniture1 = "craft furniture 1"
     CraftFurniture2 = "craft furniture 2"
@@ -370,14 +373,15 @@
     GrowGrain3a = "grow grain 3a"
     GrowGrain3b = "grow grain 3b"
     GrowGrain4a = "grow grain 4a"
     GrowGrain4b = "grow grain 4b"
     GrowHerbs1 = "grow herbs 1"
     GrowHerbs2 = "grow herbs 2"
     HammerNails1 = "hammer nails 1"
+    HandcartOperations = "handcart operations"
     HarnessOx1 = "harness ox 1"
     HarnessOx2a = "harness ox 2a"
     HarnessOx2b = "harness ox 2b"
     HarnessOx3a = "harness ox 3a"
     HarnessOx3b = "harness ox 3b"
     HarnessOx4a = "harness ox 4a"
     HarnessOx4b = "harness ox 4b"
@@ -517,36 +521,37 @@
     SmeltLead2b = "smelt lead 2b"
     SmokingFish1 = "smoking fish 1"
     SmokingFish2 = "smoking fish 2"
     SmokingHam1 = "smoking ham 1"
     SmokingHam2 = "smoking ham 2"
     SmokingMeat1 = "smoking meat 1"
     SmokingMeat2 = "smoking meat 2"
+    SnekkjaOperations = "snekkja operations"
     SpinThread1 = "spin thread 1"
     SpinThread2 = "spin thread 2"
     SpinYarn1 = "spin yarn 1"
     SpinYarn2 = "spin yarn 2"
     SplitTimber1 = "split timber 1"
     SplitTimber2 = "split timber 2"
     TanHides1 = "tan hides 1"
     TanHides2 = "tan hides 2"
+    TumbrelOperations = "tumbrel operations"
     WeaveCloth1 = "weave cloth 1"
     WeaveCloth2a = "weave cloth 2a"
     WeaveCloth2b = "weave cloth 2b"
     WeaveCloth3a = "weave cloth 3a"
     WeaveCloth3b = "weave cloth 3b"
     WeaveCloth4a = "weave cloth 4a"
     WeaveCloth4b = "weave cloth 4b"
     YokeOx1a = "yoke ox 1a"
     YokeOx1b = "yoke ox 1b"
     YokeOx2a = "yoke ox 2a"
     YokeOx2b = "yoke ox 2b"
 
 
-
 class Skill(Enum):
     """Represents a worker skill."""
 
     Crafting = "crafting"
     Forging = "forging"
     Maritime = "maritime"
     Mercantile = "mercantile"
@@ -590,71 +595,190 @@
 
     account: InventoryAccount
     capacity: int
     managers: Optional[dict[Item, InventoryManager]] = None
     previous_flows: Optional[dict[Item, InventoryFlow]] = {}
     reserved: Optional[int] = None
 
+    @property
+    def items(self) -> dict[Item, InventoryAccountAsset]:
+        """The items in the inventory."""
+        return self.account.assets
+
 
 class InventoryAccount(BaseModel):
     """Represents an inventory account."""
 
     assets: dict[Item, InventoryAccountAsset]
     id: str
+    master_id: Optional[str] = None
     name: Optional[str] = None
     owner_id: int
-    sponsor_id: Optional[int] = None
+    sponsor_id: Optional[str] = None
 
 
 class InventoryAccountAsset(BaseModel):
     """Represents an asset in an inventory account."""
 
     balance: float
     capacity: Optional[float] = None
     purchase: Optional[float] = None
-    purchase_cost: Optional[float] = None
+    purchase_price: Optional[float] = None
     reserved: float
     reserved_capacity: Optional[float] = None
     sale: Optional[float] = None
     sale_price: Optional[float] = None
     unit_cost: Optional[float] = None
 
+    @property
+    def purchased(self) -> bool:
+        """Whether the asset was purchased."""
+        return self.purchase is not None
+
+    @property
+    def sold(self) -> bool:
+        """Whether the asset was sold."""
+        return self.sale is not None
+
+    @property
+    def total_purchase(self) -> float:
+        """The total purchase cost of the asset."""
+        return self.purchase * self.purchase_price
+
+    @property
+    def total_sale(self) -> float:
+        """The total sale cost of the asset."""
+        return self.sale * self.sale_price
+
+    @property
+    def total_value(self) -> float:
+        """The total value of the asset."""
+        return self.balance * self.unit_cost
+
 
 class InventoryManager(BaseModel):
     """Represents an inventory manager."""
 
     buy_price: Optional[float] = None
     buy_volume: Optional[int] = None
     capacity: Optional[int] = None
     max_holding: Optional[int] = None
     sell_price: Optional[float] = None
     sell_volume: Optional[int] = None
 
+    @property
+    def buying(self) -> bool:
+        """Whether the manager is buying."""
+        return self.buy_price is not None and self.buy_volume is not None
+
+    @property
+    def max_buy_price(self) -> float:
+        """The maximum buy price of the manager."""
+        return self.buy_price * self.buy_volume
+
+    @property
+    def max_sell_price(self) -> float:
+        """The maximum sell price of the manager."""
+        return self.sell_price * self.sell_volume
+
+    @property
+    def selling(self) -> bool:
+        """Whether the manager is selling."""
+        return self.sell_price is not None and self.sell_volume is not None
+
 
 class InventoryFlow(BaseModel):
     """Represents an inventory flow."""
 
-    consumption: Optional[float] = None
-    expiration: Optional[float] = None
+    consumption: Optional[float] = 0.0
+    expiration: Optional[float] = 0.0
     export: Optional[int] = None
     imported: Optional[int] = Field(None, alias="import")
-    production: Optional[float] = None
-    production_cost: Optional[float] = None
+    production: Optional[float] = 0.0
+    production_cost: Optional[float] = 0.0
     purchase: Optional[int] = None
+    purchase_cost: Optional[float] = 0.0
+    resident: Optional[float] = None
     sale: Optional[int] = None
+    sale_value: Optional[float] = 0.0
+    shortfall: Optional[float] = 0.0
+
+
+class DeliveryCost(BaseModel):
+    """Represents the delivery cost of a building."""
+
+    land_distance: float
+    ferry_fee: Optional[float] = None
+
 
 class Operation(BaseModel):
     """Represents an operation."""
-    target: float
-    production: float
-    provision: float
+
+    target: float = None
+    production: Optional[float] = None
+    provision: Optional[float] = None
+    reference: Optional[str] = None
+    recipe: Optional[Recipe] = None
+    volume: Optional[float] = None
+    tax_rate: Optional[float] = None
+    tax: Optional[float] = None
+    delivery_cost: Optional[DeliveryCost] = None
+    flows: Optional[dict[Item, InventoryFlow]] = None
+
+    @property
+    def surplus(self) -> float:
+        """The surplus of the operation."""
+        return self.production - self.target
+
+    @property
+    def shortfall(self) -> float:
+        """The shortfall of the operation."""
+        return self.target - self.production
+
+
+class Path(BaseModel):
+    """Represents part of a path."""
+
+    x: int
+    y: int
+    c: float
+
 
 class Producer(BaseModel):
     """Represents a producer."""
+
     inventory: Inventory
     limited: bool
     manager: str
     previous_operation: Operation
-    provider_id: int
+    provider_id: Optional[int] = None
     recipe: Recipe
     reference: str
-    target: Optional[float] = None
+    target: Optional[float] = None
+
+
+class ItemTrade(BaseModel):
+    """Data for buying/selling an item."""
+
+    direction: str
+    expected_balance: float
+    operation: str
+    price: float
+    volume: int
+
+
+class ItemTradeResult(BaseModel):
+    """Result of buying/selling an item."""
+
+    settlements: Optional[list[ItemTradeSettlement]] = None
+    order_id: Optional[int] = None
+    embedded: Optional[dict] = Field(alias="_embedded", default_factory=dict)
+
+    class Config:
+        arbitrary_types_allowed = True
+
+
+class ItemTradeSettlement(BaseModel):
+    """Settlement of an item trade."""
+
+    volume: int
+    price: float
```

### Comparing `pymerc-0.4.0/pymerc/api/models/map.py` & `pymerc-0.5.0/pymerc/api/models/map.py`

 * *Files identical despite different names*

### Comparing `pymerc-0.4.0/pymerc/api/models/player.py` & `pymerc-0.5.0/pymerc/api/models/player.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from __future__ import annotations
+
 from typing import Optional
 
 from pydantic import BaseModel
 
 from pymerc.api.models import common
 
 
 class Player(BaseModel):
     username: str
     household: Household
-    discord_id: str
+    discord_id: Optional[str] = None
     settings: Settings
     active: bool
 
 
 class Household(BaseModel):
     id: str
     name: str
     town_id: int
     portrait: str
     gender: str
     account_id: str
     business_ids: list[str]
     prestige: float
-    prestige_impacts: list[PrestigeImpact]
+    prestige_impacts: Optional[list[PrestigeImpact]] = None
     workers: list[Worker]
     operations: list[str]
     caps: dict[str, int]
     sustenance: Sustenance
 
 
 class PrestigeImpact(BaseModel):
@@ -41,15 +42,15 @@
     name: str
     skills: dict[common.Skill, float]
 
 
 class Sustenance(BaseModel):
     reference: str
     inventory: common.Inventory
-    provider_id: str
+    provider_id: Optional[str] = None
 
 
 class Settings(BaseModel):
     sound_volume: int
     notifications: NotificationSettings
     commoners_splash: bool
     construction_splash: bool
```

### Comparing `pymerc-0.4.0/pymerc/api/models/static.py` & `pymerc-0.5.0/pymerc/api/models/static.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 from typing import Optional
+
 from pydantic import BaseModel, Field
 
 from pymerc.api.models import common
 
 
 class Building(BaseModel):
     """Represents a building in the game."""
```

### Comparing `pymerc-0.4.0/pymerc/api/models/towns.py` & `pymerc-0.5.0/pymerc/api/models/towns.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
-from pydantic import BaseModel, Field
 from typing import Optional
 
+from pydantic import BaseModel, Field
+
 from pymerc.api.models import common
 
 
 class Town(BaseModel):
     """Represents a town in the game."""
 
     id: str
@@ -102,15 +103,15 @@
 
     special_market_pressure: Optional[dict[int, float]] = {}
 
 
 class TownMarket(BaseModel):
     """Represents the market in a town."""
 
-    markets: dict[str, TownMarketItem]
+    markets: dict[common.Item, TownMarketItem]
     ts: int = Field(alias="_ts")
 
 
 class TownMarketItem(BaseModel):
     """Represents the market data for a single item in a town."""
 
     price: Optional[float] = 0.0
```

### Comparing `pymerc-0.4.0/pymerc/api/static.py` & `pymerc-0.5.0/pymerc/api/static.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,67 +1,72 @@
 import json
 import re
 from typing import Any
 
+from async_lru import alru_cache
 from pydantic import TypeAdapter
 
 from pymerc.api.base import BaseAPI
 from pymerc.api.models import static
 
 BASE_URL = "https://play.mercatorio.io/static/js/"
 ROOT_URL = "https://play.mercatorio.io/"
 
 
 class StaticAPI(BaseAPI):
     """A class for interacting with the static data from the game."""
 
+    @alru_cache(maxsize=1)
     async def get_buildings(self) -> list[static.Building]:
         """Get the buildings from the game.
 
         Returns:
             list[static.Building]: The buildings from the game.
         """
         data = await self._get()
 
         type_adapter = TypeAdapter(list[static.Building])
         return type_adapter.validate_python(data["Gm"])
 
+    @alru_cache(maxsize=1)
     async def get_items(self) -> list[static.Item]:
         """Get the items from the game.
 
         Returns:
             list[static.Item]: The items from the game.
         """
         data = await self._get()
 
         type_adapter = TypeAdapter(list[static.Item])
         return type_adapter.validate_python(data["RB"])
 
+    @alru_cache(maxsize=1)
     async def get_recipes(self) -> list[static.Recipe]:
         """Get the recipes from the game.
 
         Returns:
             list[static.Recipe]: The recipes from the game.
         """
         data = await self._get()
-
         type_adapter = TypeAdapter(list[static.Recipe])
         return type_adapter.validate_python(data["F_"])
 
+    @alru_cache(maxsize=1)
     async def get_transport(self) -> list[static.Transport]:
         """Get the transport from the game.
 
         Returns:
             list[static.Transport]: The transport from the game.
         """
         data = await self._get()
 
         type_adapter = TypeAdapter(list[static.Transport])
         return type_adapter.validate_python(data["g$"])
 
+    @alru_cache(maxsize=1)
     async def _get(self) -> Any:
         """Get the static data from the game.
 
         Returns:
             The static data from the game.
         """
         response = await self.client.get(ROOT_URL)
```

### Comparing `pymerc-0.4.0/pymerc/client.py` & `pymerc-0.5.0/pymerc/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from __future__ import annotations
+
 import asyncio
 
 import httpx
 
 from pymerc.api.buildings import BuildingsAPI
 from pymerc.api.businesses import BusinessesAPI
 from pymerc.api.map import MapAPI
 from pymerc.api.player import PlayerAPI
 from pymerc.api.static import StaticAPI
 from pymerc.api.towns import TownsAPI
+from pymerc.api.transports import TransportsAPI
 from pymerc.exceptions import TurnInProgressException
 from pymerc.game.building import Building
 from pymerc.game.player import Player
+from pymerc.game.storehouse import Storehouse
 from pymerc.game.town import Town
+from pymerc.game.transport import Transport
 
 
 class Client:
     """A simple API client for the Mercatorio API."""
 
     session: httpx.AsyncClient
     token: str
@@ -24,14 +28,15 @@
 
     buildings_api: BuildingsAPI
     businesses_api: BusinessesAPI
     map_api: MapAPI
     player_api: PlayerAPI
     static_api: StaticAPI
     towns_api: TownsAPI
+    transports_api: TransportsAPI
 
     def __init__(self, user: str, token: str):
         self.session = httpx.AsyncClient(http2=True)
         self.user = user
         self.token = token
 
         self.session.headers.setdefault("X-Merc-User", self.user)
@@ -39,14 +44,15 @@
 
         self.buildings_api = BuildingsAPI(self)
         self.businesses_api = BusinessesAPI(self)
         self.map_api = MapAPI(self)
         self.player_api = PlayerAPI(self)
         self.static_api = StaticAPI(self)
         self.towns_api = TownsAPI(self)
+        self.transports_api = TransportsAPI(self)
 
     async def close(self):
         await self.session.aclose()
 
     async def get(self, url: str, **kwargs) -> httpx.Response:
         """Make a GET request to the given URL.
 
@@ -119,14 +125,28 @@
             Player: The player.
         """
         p = Player(self)
         await p.load()
 
         return p
 
+    async def storehouse(self, player: Player) -> Storehouse:
+        """Get the player's storehouse.
+
+        Args:
+            player (Player): The player.
+
+        Returns:
+            Storehouse: The player's storehouse.
+        """
+        s = Storehouse(self, player)
+        await s.load()
+
+        return s
+
     async def town(self, town_id: int) -> Town:
         """Get a town by its ID.
 
         Args:
             town_id (int): The ID of the town.
 
         Returns:
@@ -149,14 +169,29 @@
         tasks = []
         for town in await self.towns_api.get_all():
             if filter and town.name not in filter:
                 continue
             tasks.append(self.town(town.id))
         return await asyncio.gather(*tasks)
 
+    async def transport(self, player: Player, id: int) -> Transport:
+        """Get a transport by its ID.
+
+        Args:
+            id (int): The ID of the transport.
+            player (Player): The player.
+
+        Returns:
+            Transport: The transport with the given ID.
+        """
+        t = Transport(self, player, id)
+        await t.load()
+
+        return t
+
     async def turn(client: Client) -> int:
         """Get the current turn number.
 
         Args:
             client (Client): The Mercatorio API client.
 
         Returns:
```

### Comparing `pymerc-0.4.0/pymerc/util/data.py` & `pymerc-0.5.0/pymerc/util/data.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,8 @@
         if isinstance(value, dict):
             converted_dict[key] = convert_floats_to_strings(value)
         elif isinstance(value, float):
             converted_dict[key] = str(value)
         else:
             converted_dict[key] = value
 
-    return converted_dict
+    return converted_dict
```

### Comparing `pymerc-0.4.0/pymerc/util/towns.py` & `pymerc-0.5.0/pymerc/util/towns.py`

 * *Files identical despite different names*

### Comparing `pymerc-0.4.0/pyproject.toml` & `pymerc-0.5.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 [tool.poetry]
 name = "pymerc"
-version = "0.4.0"
+version = "0.5.0"
 description = "A Python library for interacting with the Mercatorio browser based game"
 authors = ["Joshua Gilman <joshuagilman@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/jmgilman/pymerc"
 keywords = ["mercatorio", "python", "library", "game"]
 packages = [{ include = "pymerc" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 httpx = { extras = ["http2"], version = "^0.27.0" }
 loguru = "^0.7.2"
 asyncio = "^3.4.3"
 pydantic = "^2.7.1"
+async-lru = "^2.0.4"
 
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.24.0"
 pytest = "^8.2.0"
 pytest-asyncio = "^0.23.6"
 python-dotenv = "^1.0.1"
 pytest-subtests = "^0.12.1"
 ruff = "^0.4.4"
+tabulate = "^0.9.0"
+mypy = "^1.10.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```


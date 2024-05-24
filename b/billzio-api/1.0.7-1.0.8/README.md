# Comparing `tmp/billzio_api-1.0.7.tar.gz` & `tmp/billzio_api-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "billzio_api-1.0.7.tar", max compression
+gzip compressed data, was "billzio_api-1.0.8.tar", max compression
```

## Comparing `billzio_api-1.0.7.tar` & `billzio_api-1.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2024-05-23 09:02:33.964650 billzio_api-1.0.7/LICENSE
--rw-r--r--   0        0        0     1287 2024-05-23 09:02:33.964650 billzio_api-1.0.7/README.md
--rw-r--r--   0        0        0      565 2024-05-23 09:02:33.964650 billzio_api-1.0.7/billzio_api/__init__.py
--rw-r--r--   0        0        0      273 2024-05-23 09:02:33.964650 billzio_api-1.0.7/billzio_api/__version__.py
--rw-r--r--   0        0        0      188 2024-05-23 09:02:33.964650 billzio_api-1.0.7/billzio_api/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-23 09:02:33.964650 billzio_api-1.0.7/billzio_api/handlers/__init__.py
--rw-r--r--   0        0        0     8704 2024-05-23 09:02:33.964650 billzio_api-1.0.7/billzio_api/handlers/async_handler.py
--rw-r--r--   0        0        0     2692 2024-05-23 09:02:33.964650 billzio_api-1.0.7/billzio_api/handlers/base.py
--rw-r--r--   0        0        0     8088 2024-05-23 09:02:33.964650 billzio_api-1.0.7/billzio_api/handlers/handler.py
--rw-r--r--   0        0        0      151 2024-05-23 09:02:33.964650 billzio_api-1.0.7/billzio_api/models/auth.py
--rw-r--r--   0        0        0      361 2024-05-23 09:02:33.964650 billzio_api-1.0.7/billzio_api/models/brands.py
--rw-r--r--   0        0        0      831 2024-05-23 09:02:33.964650 billzio_api-1.0.7/billzio_api/models/categories.py
--rw-r--r--   0        0        0     1183 2024-05-23 09:02:33.968649 billzio_api-1.0.7/billzio_api/models/clients.py
--rw-r--r--   0        0        0      495 2024-05-23 09:02:33.968649 billzio_api-1.0.7/billzio_api/models/currencies.py
--rw-r--r--   0        0        0      396 2024-05-23 09:02:33.968649 billzio_api-1.0.7/billzio_api/models/orders.py
--rw-r--r--   0        0        0      374 2024-05-23 09:02:33.968649 billzio_api-1.0.7/billzio_api/models/payment_types.py
--rw-r--r--   0        0        0     1513 2024-05-23 09:02:33.968649 billzio_api-1.0.7/billzio_api/models/products.py
--rw-r--r--   0        0        0      698 2024-05-23 09:02:33.968649 billzio_api-1.0.7/billzio_api/models/shops.py
--rw-r--r--   0        0        0      395 2024-05-23 09:02:33.968649 billzio_api-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     1891 1970-01-01 00:00:00.000000 billzio_api-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-24 10:06:54.811566 billzio_api-1.0.8/LICENSE
+-rw-r--r--   0        0        0     1287 2024-05-24 10:06:54.811566 billzio_api-1.0.8/README.md
+-rw-r--r--   0        0        0      565 2024-05-24 10:06:54.811566 billzio_api-1.0.8/billzio_api/__init__.py
+-rw-r--r--   0        0        0      273 2024-05-24 10:06:54.811566 billzio_api-1.0.8/billzio_api/__version__.py
+-rw-r--r--   0        0        0      188 2024-05-24 10:06:54.811566 billzio_api-1.0.8/billzio_api/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-24 10:06:54.811566 billzio_api-1.0.8/billzio_api/handlers/__init__.py
+-rw-r--r--   0        0        0     8704 2024-05-24 10:06:54.811566 billzio_api-1.0.8/billzio_api/handlers/async_handler.py
+-rw-r--r--   0        0        0     2692 2024-05-24 10:06:54.811566 billzio_api-1.0.8/billzio_api/handlers/base.py
+-rw-r--r--   0        0        0     8088 2024-05-24 10:06:54.811566 billzio_api-1.0.8/billzio_api/handlers/handler.py
+-rw-r--r--   0        0        0      151 2024-05-24 10:06:54.811566 billzio_api-1.0.8/billzio_api/models/auth.py
+-rw-r--r--   0        0        0      361 2024-05-24 10:06:54.811566 billzio_api-1.0.8/billzio_api/models/brands.py
+-rw-r--r--   0        0        0      831 2024-05-24 10:06:54.811566 billzio_api-1.0.8/billzio_api/models/categories.py
+-rw-r--r--   0        0        0     1183 2024-05-24 10:06:54.811566 billzio_api-1.0.8/billzio_api/models/clients.py
+-rw-r--r--   0        0        0      495 2024-05-24 10:06:54.811566 billzio_api-1.0.8/billzio_api/models/currencies.py
+-rw-r--r--   0        0        0      396 2024-05-24 10:06:54.811566 billzio_api-1.0.8/billzio_api/models/orders.py
+-rw-r--r--   0        0        0      374 2024-05-24 10:06:54.811566 billzio_api-1.0.8/billzio_api/models/payment_types.py
+-rw-r--r--   0        0        0     1521 2024-05-24 10:06:54.811566 billzio_api-1.0.8/billzio_api/models/products.py
+-rw-r--r--   0        0        0      698 2024-05-24 10:06:54.811566 billzio_api-1.0.8/billzio_api/models/shops.py
+-rw-r--r--   0        0        0      395 2024-05-24 10:06:54.811566 billzio_api-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1891 1970-01-01 00:00:00.000000 billzio_api-1.0.8/PKG-INFO
```

### Comparing `billzio_api-1.0.7/LICENSE` & `billzio_api-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `billzio_api-1.0.7/README.md` & `billzio_api-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `billzio_api-1.0.7/billzio_api/__init__.py` & `billzio_api-1.0.8/billzio_api/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.7"
+__version__ = "1.0.8"
 
 from .handlers.async_handler import AsyncBillzHandler
 from .handlers.handler import BillzHandler
 from .models.shops import ShopsListFilters, ShopsListData
 from .models.products import ProductsListFilters, ProductListData
 from .models.categories import CategoriesListFilters, CategoriesListData
 from .models.currencies import CurrenciesListData
```

### Comparing `billzio_api-1.0.7/billzio_api/handlers/async_handler.py` & `billzio_api-1.0.8/billzio_api/handlers/async_handler.py`

 * *Files identical despite different names*

### Comparing `billzio_api-1.0.7/billzio_api/handlers/base.py` & `billzio_api-1.0.8/billzio_api/handlers/base.py`

 * *Files identical despite different names*

### Comparing `billzio_api-1.0.7/billzio_api/handlers/handler.py` & `billzio_api-1.0.8/billzio_api/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `billzio_api-1.0.7/billzio_api/models/categories.py` & `billzio_api-1.0.8/billzio_api/models/categories.py`

 * *Files identical despite different names*

### Comparing `billzio_api-1.0.7/billzio_api/models/clients.py` & `billzio_api-1.0.8/billzio_api/models/clients.py`

 * *Files identical despite different names*

### Comparing `billzio_api-1.0.7/billzio_api/models/products.py` & `billzio_api-1.0.8/billzio_api/models/products.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     attribute_id: str
     attribute_name: Optional[str]
     attribute_value: str
     attribute_value_id: str
 
 
 class ShopMeasurementValue(BaseModel):
-    active_measurement_value: int
+    active_measurement_value: int | float
     shop_id: str
     shop_name: str
 
 
 class ShopPrice(BaseModel):
     retail_currency: str
     retail_price: int
```

### Comparing `billzio_api-1.0.7/billzio_api/models/shops.py` & `billzio_api-1.0.8/billzio_api/models/shops.py`

 * *Files identical despite different names*

### Comparing `billzio_api-1.0.7/PKG-INFO` & `billzio_api-1.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: billzio-api
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python wrapper for Billz.io Public API
 License: Apache 2.0
 Author: Sirojiddin Mustafayev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```


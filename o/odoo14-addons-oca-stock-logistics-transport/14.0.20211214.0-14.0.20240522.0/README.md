# Comparing `tmp/odoo14_addons_oca_stock_logistics_transport-14.0.20211214.0-py3-none-any.whl.zip` & `tmp/odoo14_addons_oca_stock_logistics_transport-14.0.20240522.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1533 bytes, number of entries: 4
--rw-r--r--  2.0 unx      534 b- defN 21-Dec-15 04:53 odoo14_addons_oca_stock_logistics_transport-14.0.20211214.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Dec-15 04:53 odoo14_addons_oca_stock_logistics_transport-14.0.20211214.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 21-Dec-15 04:53 odoo14_addons_oca_stock_logistics_transport-14.0.20211214.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      480 b- defN 21-Dec-15 04:53 odoo14_addons_oca_stock_logistics_transport-14.0.20211214.0.dist-info/RECORD
-4 files, 1107 bytes uncompressed, 583 bytes compressed:  47.3%
+Zip file size: 1557 bytes, number of entries: 4
+-rw-r--r--  2.0 unx      664 b- defN 24-May-24 07:49 odoo14_addons_oca_stock_logistics_transport-14.0.20240522.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 07:49 odoo14_addons_oca_stock_logistics_transport-14.0.20240522.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-May-24 07:49 odoo14_addons_oca_stock_logistics_transport-14.0.20240522.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      480 b- defN 24-May-24 07:49 odoo14_addons_oca_stock_logistics_transport-14.0.20240522.0.dist-info/RECORD
+4 files, 1237 bytes uncompressed, 607 bytes compressed:  50.9%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo14_addons_oca_stock_logistics_transport-14.0.20211214.0.dist-info/METADATA
+Filename: odoo14_addons_oca_stock_logistics_transport-14.0.20240522.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addons_oca_stock_logistics_transport-14.0.20211214.0.dist-info/WHEEL
+Filename: odoo14_addons_oca_stock_logistics_transport-14.0.20240522.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addons_oca_stock_logistics_transport-14.0.20211214.0.dist-info/top_level.txt
+Filename: odoo14_addons_oca_stock_logistics_transport-14.0.20240522.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addons_oca_stock_logistics_transport-14.0.20211214.0.dist-info/RECORD
+Filename: odoo14_addons_oca_stock_logistics_transport-14.0.20240522.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo14_addons_oca_stock_logistics_transport-14.0.20211214.0.dist-info/METADATA` & `odoo14_addons_oca_stock_logistics_transport-14.0.20240522.0.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: odoo14-addons-oca-stock-logistics-transport
-Version: 14.0.20211214.0
+Version: 14.0.20240522.0
 Summary: Meta package for oca-stock-logistics-transport Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
 Requires-Dist: odoo14-addon-shipment-advice
+Requires-Dist: odoo14-addon-shipment-advice-bill-auto-complete
+Requires-Dist: odoo14-addon-shipment-advice-bill-auto-complete-mrp
 Requires-Dist: odoo14-addon-stock-dock
 Requires-Dist: odoo14-addon-stock-location-address
 Requires-Dist: odoo14-addon-stock-location-address-purchase
 
 UNKNOWN
```


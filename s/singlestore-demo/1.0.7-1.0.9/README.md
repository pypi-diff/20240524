# Comparing `tmp/singlestore_demo-1.0.7-py3-none-any.whl.zip` & `tmp/singlestore_demo-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11619 bytes, number of entries: 9
+Zip file size: 11626 bytes, number of entries: 9
 -rw-r--r--  2.0 unx        0 b- defN 23-Jan-13 14:14 singlestore_demo/__init__.py
--rw-r--r--  2.0 unx    16178 b- defN 23-Jan-16 11:59 singlestore_demo/generate.py
+-rw-r--r--  2.0 unx    16188 b- defN 23-Jan-16 12:06 singlestore_demo/generate.py
 -rw-r--r--  2.0 unx     8631 b- defN 23-Jan-12 15:15 singlestore_demo/schema.sql
--rw-r--r--  2.0 unx     1072 b- defN 23-Jan-16 12:01 singlestore_demo-1.0.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     9317 b- defN 23-Jan-16 12:01 singlestore_demo-1.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-16 12:01 singlestore_demo-1.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       62 b- defN 23-Jan-16 12:01 singlestore_demo-1.0.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       17 b- defN 23-Jan-16 12:01 singlestore_demo-1.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      787 b- defN 23-Jan-16 12:01 singlestore_demo-1.0.7.dist-info/RECORD
-9 files, 36156 bytes uncompressed, 10241 bytes compressed:  71.7%
+-rw-r--r--  2.0 unx     1072 b- defN 23-Jan-16 12:08 singlestore_demo-1.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9317 b- defN 23-Jan-16 12:08 singlestore_demo-1.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jan-16 12:08 singlestore_demo-1.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       62 b- defN 23-Jan-16 12:08 singlestore_demo-1.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       17 b- defN 23-Jan-16 12:08 singlestore_demo-1.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      787 b- defN 23-Jan-16 12:08 singlestore_demo-1.0.9.dist-info/RECORD
+9 files, 36166 bytes uncompressed, 10248 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: singlestore_demo/generate.py
 Comment: 
 
 Filename: singlestore_demo/schema.sql
 Comment: 
 
-Filename: singlestore_demo-1.0.7.dist-info/LICENSE
+Filename: singlestore_demo-1.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: singlestore_demo-1.0.7.dist-info/METADATA
+Filename: singlestore_demo-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: singlestore_demo-1.0.7.dist-info/WHEEL
+Filename: singlestore_demo-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: singlestore_demo-1.0.7.dist-info/entry_points.txt
+Filename: singlestore_demo-1.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: singlestore_demo-1.0.7.dist-info/top_level.txt
+Filename: singlestore_demo-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: singlestore_demo-1.0.7.dist-info/RECORD
+Filename: singlestore_demo-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## singlestore_demo/generate.py

```diff
@@ -189,15 +189,15 @@
     with conn.cursor() as cur:
       print("Generating and Inserting `supplier` data")
       for supplier in np.arange(int(TOTALSUPPLIERS/ROWSPERINSERT)):
         rows = [[
           mimefinance.company()[:25],
           mimeaddress.address(),
           17,
-          mimeperson.telephone(),
+          mimeperson.telephone()[:15],
           round(mimenumeric.decimal_number(start=0.00,end=9999999.00),2),
           mimetext.sentence()[:50]
          ] for x in np.arange(ROWSPERINSERT)]
 
         insertRows = (','.join('("{}", "{}", {}, "{}", {}, "{}")'.format(row[0], row[1], row[2], row[3], row[4], row[5]) for row in rows))
 
         print("Inserting records {}/{}".format((supplier + 1) * ROWSPERINSERT, TOTALSUPPLIERS));
@@ -219,15 +219,15 @@
 def create_parts():
   ths = []
   with get_connection(DATABASE) as conn:
     with conn.cursor() as cur:
       print("Generation and inserting `part` data")
       for part in np.arange(int(TOTALPARTS/ROWSPERINSERT)):
         rows = [[
-          mimefinance.stock_name(),
+          mimefinance.stock_name()[:55],
           mimerandom.custom_code(mask="Manufacturer####", digit='#'),
           mimerandom.custom_code(mask="Brand####", digit='#'),
           random.choice(PARTTYPES),
           mimenumeric.integer_number(start=0, end=99),
           random.choice(CONTAINERTYPES),
           round(mimenumeric.decimal_number(start=0.00,end=999.00),2),
           mimetext.sentence()[:23]
```

## Comparing `singlestore_demo-1.0.7.dist-info/LICENSE` & `singlestore_demo-1.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `singlestore_demo-1.0.7.dist-info/METADATA` & `singlestore_demo-1.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singlestore-demo
-Version: 1.0.7
+Version: 1.0.9
 Summary: Generates a demo datasource for SingleStore
 Author-email: Ricardo Santos <rsantos@singlestore.com>
 License: MIT License
         
         Copyright (c) 2023 singlestore_demo
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```


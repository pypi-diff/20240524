# Comparing `tmp/py_text_clock-0.2.1-py3-none-any.whl.zip` & `tmp/py_text_clock-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 7072 bytes, number of entries: 12
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 18:34 source/__init__.py
--rw-r--r--  2.0 unx     2591 b- defN 23-Jun-26 18:34 source/clockFace.py
--rw-r--r--  2.0 unx      795 b- defN 23-Jun-26 18:34 source/command_line.py
--rw-r--r--  2.0 unx     7776 b- defN 23-Jun-26 18:34 source/fontMods.py
--rw-r--r--  2.0 unx      343 b- defN 23-Jun-26 18:34 source/mylogger.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 18:34 tests/__init__.py
--rw-r--r--  2.0 unx     2966 b- defN 23-Jun-26 18:34 tests/test_clock.py
--rw-r--r--  2.0 unx      980 b- defN 23-Jun-26 18:35 py_text_clock-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-26 18:35 py_text_clock-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       54 b- defN 23-Jun-26 18:35 py_text_clock-0.2.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-Jun-26 18:35 py_text_clock-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      944 b- defN 23-Jun-26 18:35 py_text_clock-0.2.1.dist-info/RECORD
-12 files, 16554 bytes uncompressed, 5480 bytes compressed:  66.9%
+Zip file size: 7085 bytes, number of entries: 12
+-rw-r--r--  2.0 unx        0 b- defN 24-May-24 14:44 source/__init__.py
+-rw-r--r--  2.0 unx     2591 b- defN 24-May-24 14:44 source/clockFace.py
+-rw-r--r--  2.0 unx      795 b- defN 24-May-24 14:44 source/command_line.py
+-rw-r--r--  2.0 unx     7767 b- defN 24-May-24 14:44 source/fontMods.py
+-rw-r--r--  2.0 unx      343 b- defN 24-May-24 14:44 source/mylogger.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-24 14:44 tests/__init__.py
+-rw-r--r--  2.0 unx     2966 b- defN 24-May-24 14:44 tests/test_clock.py
+-rw-r--r--  2.0 unx      980 b- defN 24-May-24 14:44 py_text_clock-0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 14:44 py_text_clock-0.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       54 b- defN 24-May-24 14:44 py_text_clock-0.2.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 24-May-24 14:44 py_text_clock-0.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      944 b- defN 24-May-24 14:44 py_text_clock-0.2.2.dist-info/RECORD
+12 files, 16545 bytes uncompressed, 5493 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_clock.py
 Comment: 
 
-Filename: py_text_clock-0.2.1.dist-info/METADATA
+Filename: py_text_clock-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: py_text_clock-0.2.1.dist-info/WHEEL
+Filename: py_text_clock-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: py_text_clock-0.2.1.dist-info/entry_points.txt
+Filename: py_text_clock-0.2.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: py_text_clock-0.2.1.dist-info/top_level.txt
+Filename: py_text_clock-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: py_text_clock-0.2.1.dist-info/RECORD
+Filename: py_text_clock-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## source/fontMods.py

```diff
@@ -74,25 +74,24 @@
         # self.time_sentence = "it is ten o'clock"
         # self.time_sentence = "it is five minutes past zero"
         # self.time_sentence = "it is zero o'clock"
         self.get_word_locations()
 
     def get_word_locations(self):
         logger.debug(f'Showing matrix for "{self.time_sentence}"')
-        
+
         # from the time as sentence, take each word
         logger.debug(self.time_sentence.split(' '))
         self.word_locations = []
         for each_word in self.time_sentence.split(' '):
 
-
             # corner case
-            if each_word == 'quarter': each_word = 'fifteen'
-            if each_word == 'half': each_word = 'thirty'
-            if each_word == 'zero': each_word = 'twelve'
+            if each_word == 'QUARTER': each_word = 'FIFTEEN'
+            if each_word == 'HALF': each_word = 'THIRTY'
+            if each_word == 'ZERO': each_word = 'TWELVE'
 
             logger.debug(f'Checking word "{each_word}" in one {["".join(s) for s in self.all_lines]}')
             
 
             # check that word in each line
             for each_line in self.all_lines:
```

## Comparing `py_text_clock-0.2.1.dist-info/METADATA` & `py_text_clock-0.2.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-text-clock
-Version: 0.2.1
+Version: 0.2.2
 Summary: A verbose Clock
 Home-page: https://github.com/manojmanivannan/py-clock
 Author: Manoj Manivannan
 Author-email: manojm18@live.in
 Requires-Dist: pytest
 Requires-Dist: click
```

## Comparing `py_text_clock-0.2.1.dist-info/RECORD` & `py_text_clock-0.2.2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 source/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 source/clockFace.py,sha256=Skw6U2G0v25HW1bOUJbbQfVXz9w1oGAC9kKQWfSWomA,2591
 source/command_line.py,sha256=mIB-KxaVcVZ0ybXC5849VCyJDs6Yn-fQBH9-p7j5P2s,795
-source/fontMods.py,sha256=eHY61LKCQ8iYGVInYvXRs1p5g7LvAHlin4NjI6AUvEo,7776
+source/fontMods.py,sha256=bjPSJEb0Pf4t8Ahaswqtw8WqDTifUx_qI6oVG9pJIHI,7767
 source/mylogger.py,sha256=EHjrkgt7X1wV15thQzo7V69Cr80q4f-oFskTybj65vY,343
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_clock.py,sha256=i4iI2RUFOmOlF4r-7Zi6L5qgAr41DRCO4XqtW50DerE,2966
-py_text_clock-0.2.1.dist-info/METADATA,sha256=9Wayzd1Pr4V6gKUyDXdEnGGmztlvK9jP5O13OBAs85U,980
-py_text_clock-0.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-py_text_clock-0.2.1.dist-info/entry_points.txt,sha256=IqdtME5yBvILSZYRbEd3YnBoEj11caRI9bUQBc84y0E,54
-py_text_clock-0.2.1.dist-info/top_level.txt,sha256=BqYZ1ZMe01jBY8kLNgfGcae4HTOnpoTmWp8eYoM8rnY,13
-py_text_clock-0.2.1.dist-info/RECORD,,
+py_text_clock-0.2.2.dist-info/METADATA,sha256=7FmXtPLlSuLVgv8aupv_DZ9wvAvFC_LWR5Crp-rmauM,980
+py_text_clock-0.2.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+py_text_clock-0.2.2.dist-info/entry_points.txt,sha256=IqdtME5yBvILSZYRbEd3YnBoEj11caRI9bUQBc84y0E,54
+py_text_clock-0.2.2.dist-info/top_level.txt,sha256=BqYZ1ZMe01jBY8kLNgfGcae4HTOnpoTmWp8eYoM8rnY,13
+py_text_clock-0.2.2.dist-info/RECORD,,
```


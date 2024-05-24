# Comparing `tmp/report_pdf_wrapper-0.2.0-py3-none-any.whl.zip` & `tmp/report_pdf_wrapper-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5232 bytes, number of entries: 7
+Zip file size: 5380 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       68 b- defN 24-May-24 17:55 report_pdf_wrapper/__init__.py
--rw-r--r--  2.0 unx    12711 b- defN 24-May-24 17:09 report_pdf_wrapper/report_pdf_wrapper.py
--rw-r--r--  2.0 unx     1068 b- defN 24-May-24 17:56 report_pdf_wrapper-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      712 b- defN 24-May-24 17:56 report_pdf_wrapper-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-24 17:56 report_pdf_wrapper-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 24-May-24 17:56 report_pdf_wrapper-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      623 b- defN 24-May-24 17:56 report_pdf_wrapper-0.2.0.dist-info/RECORD
-7 files, 15293 bytes uncompressed, 4110 bytes compressed:  73.1%
+-rw-r--r--  2.0 unx    13180 b- defN 24-May-24 18:39 report_pdf_wrapper/report_pdf_wrapper.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-24 18:40 report_pdf_wrapper-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      712 b- defN 24-May-24 18:40 report_pdf_wrapper-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 18:40 report_pdf_wrapper-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 24-May-24 18:40 report_pdf_wrapper-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      623 b- defN 24-May-24 18:40 report_pdf_wrapper-0.3.0.dist-info/RECORD
+7 files, 15762 bytes uncompressed, 4258 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: report_pdf_wrapper/__init__.py
 Comment: 
 
 Filename: report_pdf_wrapper/report_pdf_wrapper.py
 Comment: 
 
-Filename: report_pdf_wrapper-0.2.0.dist-info/LICENSE
+Filename: report_pdf_wrapper-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: report_pdf_wrapper-0.2.0.dist-info/METADATA
+Filename: report_pdf_wrapper-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: report_pdf_wrapper-0.2.0.dist-info/WHEEL
+Filename: report_pdf_wrapper-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: report_pdf_wrapper-0.2.0.dist-info/top_level.txt
+Filename: report_pdf_wrapper-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: report_pdf_wrapper-0.2.0.dist-info/RECORD
+Filename: report_pdf_wrapper-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## report_pdf_wrapper/report_pdf_wrapper.py

```diff
@@ -20,22 +20,27 @@
             # create new document
             self.document = fitz.open()
         self.page = self.document.new_page()
         self.logo_path = logo_path
         if draw_dimensions:
             self.draw_dimensions()
 
-    def draw_report_pdf(self):
+    def draw_report_pdf(self, page_num=0):
         if self.logo_path is not None:
             self.draw_logo(self.logo_path)
+        # if document is multiple pages, then add suffix to mutable widget keys to prevent duplication
+        if page_num != 0:
+            widget_suffix = f"_{page_num}"
+        else:
+            widget_suffix = ""
         self.draw_technician_info()
         self.draw_customer_info()
-        self.draw_equipment_info()
-        self.draw_checklist()
-        self.draw_comments()
+        self.draw_equipment_info(widget_suffix)
+        self.draw_checklist(widget_suffix)
+        self.draw_comments(widget_suffix)
 
     def draw_service_call_pdf(self):
         if self.logo_path is not None:
             self.draw_logo(self.logo_path)
         self.draw_technician_info()
         self.draw_customer_info()
         self.draw_equipment_info()
@@ -101,38 +106,38 @@
             field_x = top_left.x + width + 5
             field.rect = fitz.Rect(field_x, top_left.y, field_x + 390, top_left.y + height - adjust)
             self.draw_underline(field.rect)
             self.page.add_widget(field)
             start_point = Point(top_left.x, top_left.y + height)  # update start point for next label
         self.draw_box(Point(60, 175), Point(520, 175), Point(520, 277), Point(60, 277))
 
-    def draw_equipment_info(self):
+    def draw_equipment_info(self, widget_suffix=""):
         self.page.insert_text(Point(62, 306), "Equipment Info", fontsize=12)
         self.draw_box(Point(60, 310), Point(520, 310), Point(520, 403), Point(60, 403))
         self.page.insert_text(Point(70, 330), "Make:", fontsize=11)
-        self._add_text_widget("equipment_make_field", Point(70, 314), 25, 170)
+        self._add_text_widget(f"equipment_make_field{widget_suffix}", Point(70, 314), 25, 170)
         self.page.insert_text(Point(70, 360), "Model:", fontsize=11)
-        self._add_text_widget("equipment_model_field", Point(70, 344), 25, 170)
+        self._add_text_widget(f"equipment_model_field{widget_suffix}", Point(70, 344), 25, 170)
         self.page.insert_text(Point(300, 330), "Site ID:", fontsize=11)
-        self._add_text_widget("equipment_site_field", Point(300, 314), 25, 160)
+        self._add_text_widget(f"equipment_site_field{widget_suffix}", Point(300, 314), 25, 160)
         self.page.insert_text(Point(300, 360), "Equipment ID:", fontsize=11)
-        self._add_text_widget("equipment_id_field", Point(320, 344), 25, 140)
+        self._add_text_widget(f"equipment_id_field{widget_suffix}", Point(320, 344), 25, 140)
         self.page.insert_text(Point(70, 390), "Notes:", fontsize=11)
-        self._add_text_widget("equipment_notes_field", Point(70, 374), 25, 390)
+        self._add_text_widget(f"equipment_notes_field{widget_suffix}", Point(70, 374), 25, 390)
 
     def _add_text_widget(self, name, top_left, height, width):
         field = fitz.Widget()
         field.field_name = name
         field.field_type = fitz.PDF_WIDGET_TYPE_TEXT
         field.text_fontsize = 11
         field.rect = fitz.Rect(top_left.x + 50, top_left.y, top_left.x + 50 + width, top_left.y + height)
         self.draw_underline(field.rect)
         self.page.add_widget(field)
 
-    def draw_checklist(self):
+    def draw_checklist(self, widget_suffix=""):
         self.page.insert_text(Point(62, 431), "Inspection Checklist: ", fontsize=12)
         field = fitz.Widget()
         field.field_name = "report_type_field"
         field.field_type = fitz.PDF_WIDGET_TYPE_TEXT
         field.text_fontsize = 11
         field.rect = fitz.Rect(175, 415, 300, 435)
         self.page.add_widget(field)
@@ -142,48 +147,47 @@
         self.draw_box(Point(60, 435), Point(520, 435), Point(520, 700), Point(60, 700))
         self.draw_line(Point(60, 460), Point(520, 460))  # title separator
         self.draw_line(Point(350, 435), Point(350, 700))  # middle separator
         self.draw_line(Point(430, 435), Point(430, 700))  # right separator
         # draw checkboxes
         line = 1
         for i in range(463, 700, 15):
+            # add completed checkbox
             point = Point(385, i)
-            field_name = f"completed_{line}_field"
+            field_name = f"completed_{line}_field{widget_suffix}"
             self._add_checkbox_widget(point, field_name, (0, 0, 0))
             # add line item
             field = fitz.Widget()
             field.field_name = f"task_{line}_field"
             field.field_type = fitz.PDF_WIDGET_TYPE_TEXT
             field.text_maxlen = 100
             field.field_flags |= fitz.PDF_FIELD_IS_READ_ONLY
             field.rect = fitz.Rect(68, point.y - 2, 340, point.y + 10)
             self.draw_line(Point(60, i - 3), Point(520, i - 3))
             self.page.add_widget(field)
-            line += 1
-        line = 1
-        for i in range(463, 700, 15):
-            point = Point(470, i)
-            field_name = f"attention_{i}_field"
-            self._add_checkbox_widget(point, field_name, getColor("red"))
+            # add red attention checkbox
+            attention_point = Point(470, i)
+            field_name = f"attention_{i}_field{widget_suffix}"
+            self._add_checkbox_widget(attention_point, field_name, getColor("red"))
             line += 1
 
     def _add_checkbox_widget(self, top_left, name, color):
         field = fitz.Widget()
         field.field_name = name
         field.field_type = fitz.PDF_WIDGET_TYPE_CHECKBOX
         field.border_color = color
         field.border_width = 1
         field.rect = fitz.Rect(top_left, top_left.x + 10, top_left.y + 10)
         self.page.add_widget(field)
 
-    def draw_comments(self):
+    def draw_comments(self, widget_suffix=""):
         self.page.insert_text(Point(62, 726), "Comments", fontsize=12)
         self.draw_box(Point(60, 730), Point(520, 730), Point(520, 810), Point(60, 810))
         field = fitz.Widget()
-        field.field_name = "comments_field"
+        field.field_name = f"comments_field{widget_suffix}"
         field.field_type = fitz.PDF_WIDGET_TYPE_TEXT
         field.text_fontsize = 11
         field.text_maxlen = 450
         field.rect = fitz.Rect(Point(60, 730), Point(520, 810))
         self.page.add_widget(field)
 
     def draw_work_summary(self):
```

## Comparing `report_pdf_wrapper-0.2.0.dist-info/LICENSE` & `report_pdf_wrapper-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `report_pdf_wrapper-0.2.0.dist-info/METADATA` & `report_pdf_wrapper-0.3.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: report-pdf-wrapper
-Version: 0.2.0
+Version: 0.3.0
 Summary: A simple pip module for creating generic PDF reports.
 Home-page: https://github.com/nr-software/Report-PDF-Creation.git
 Author: Alex Nuccio
 Author-email: nrsoftwareservices@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `report_pdf_wrapper-0.2.0.dist-info/RECORD` & `report_pdf_wrapper-0.3.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 report_pdf_wrapper/__init__.py,sha256=bOUIDadGljW4JgkMxkcJnQ9guJ5BF_AgrA3tHNOr8y8,68
-report_pdf_wrapper/report_pdf_wrapper.py,sha256=dFR-gGYTlv6l1hBeIs8h2DSy6PoQZ3HQn8_v7wh-mwM,12711
-report_pdf_wrapper-0.2.0.dist-info/LICENSE,sha256=J45dd5o-jpQZlgZvfs77QxFtQ9WxrpBY6OYYrpb_bKk,1068
-report_pdf_wrapper-0.2.0.dist-info/METADATA,sha256=ZvYsXtLNhk4XzLq1RK_Ovjra9BUI-0UUr2WDS_lHchA,712
-report_pdf_wrapper-0.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-report_pdf_wrapper-0.2.0.dist-info/top_level.txt,sha256=7RK52XVFxPTqtewESdqMKt6-7wpBzJducMXUk4eeinc,19
-report_pdf_wrapper-0.2.0.dist-info/RECORD,,
+report_pdf_wrapper/report_pdf_wrapper.py,sha256=uGjrbao09xm92mmauip1uK-nPezrjlpmkciqINObyic,13180
+report_pdf_wrapper-0.3.0.dist-info/LICENSE,sha256=J45dd5o-jpQZlgZvfs77QxFtQ9WxrpBY6OYYrpb_bKk,1068
+report_pdf_wrapper-0.3.0.dist-info/METADATA,sha256=eF7L2OEvM_EC7miSWf6r8W7i1Rd4-MMaGotQaBMto3g,712
+report_pdf_wrapper-0.3.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+report_pdf_wrapper-0.3.0.dist-info/top_level.txt,sha256=7RK52XVFxPTqtewESdqMKt6-7wpBzJducMXUk4eeinc,19
+report_pdf_wrapper-0.3.0.dist-info/RECORD,,
```


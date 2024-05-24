# Comparing `tmp/tkchart-2.1.2.tar.gz` & `tmp/tkchart-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkchart-2.1.2.tar", last modified: Sat Apr 27 04:51:23 2024, max compression
+gzip compressed data, was "tkchart-2.1.3.tar", last modified: Fri May 24 21:13:32 2024, max compression
```

## Comparing `tkchart-2.1.2.tar` & `tkchart-2.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 04:51:23.066944 tkchart-2.1.2/
--rw-rw-rw-   0        0        0     1091 2024-02-14 05:02:34.000000 tkchart-2.1.2/LICENSE
--rw-rw-rw-   0        0        0     5665 2024-04-27 04:51:23.066944 tkchart-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3272 2024-04-27 04:02:39.000000 tkchart-2.1.2/README.md
--rw-rw-rw-   0        0        0     1259 2024-04-27 04:49:13.000000 tkchart-2.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-27 04:51:23.067926 tkchart-2.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-27 04:51:23.053007 tkchart-2.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-27 04:51:23.062780 tkchart-2.1.2/src/tkchart/
--rw-rw-rw-   0        0        0     1561 2024-04-26 18:08:54.000000 tkchart-2.1.2/src/tkchart/FontStyle.py
--rw-rw-rw-   0        0        0     8876 2024-04-26 18:04:34.000000 tkchart-2.1.2/src/tkchart/Line.py
--rw-rw-rw-   0        0        0    97149 2024-04-26 18:17:01.000000 tkchart-2.1.2/src/tkchart/LineChart.py
--rw-rw-rw-   0        0        0     1954 2024-04-26 18:10:43.000000 tkchart-2.1.2/src/tkchart/Utils.py
--rw-rw-rw-   0        0        0     9885 2024-04-26 19:09:11.000000 tkchart-2.1.2/src/tkchart/Validate.py
--rw-rw-rw-   0        0        0      430 2024-04-26 18:13:27.000000 tkchart-2.1.2/src/tkchart/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 04:51:23.065745 tkchart-2.1.2/src/tkchart.egg-info/
--rw-rw-rw-   0        0        0     5665 2024-04-27 04:51:23.000000 tkchart-2.1.2/src/tkchart.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2024-04-27 04:51:23.000000 tkchart-2.1.2/src/tkchart.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 04:51:23.000000 tkchart-2.1.2/src/tkchart.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-27 04:51:23.000000 tkchart-2.1.2/src/tkchart.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 21:13:32.013097 tkchart-2.1.3/
+-rw-rw-rw-   0        0        0     1091 2024-02-14 05:02:34.000000 tkchart-2.1.3/LICENSE
+-rw-rw-rw-   0        0        0     5667 2024-05-24 21:13:32.013097 tkchart-2.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3273 2024-05-24 21:12:02.000000 tkchart-2.1.3/README.md
+-rw-rw-rw-   0        0        0     1259 2024-05-24 21:08:05.000000 tkchart-2.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-24 21:13:32.013097 tkchart-2.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-24 21:13:31.913872 tkchart-2.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-24 21:13:31.998094 tkchart-2.1.3/src/tkchart/
+-rw-rw-rw-   0        0        0     1561 2024-04-26 18:08:54.000000 tkchart-2.1.3/src/tkchart/FontStyle.py
+-rw-rw-rw-   0        0        0     9967 2024-05-24 20:40:55.000000 tkchart-2.1.3/src/tkchart/Line.py
+-rw-rw-rw-   0        0        0   101101 2024-05-24 20:58:19.000000 tkchart-2.1.3/src/tkchart/LineChart.py
+-rw-rw-rw-   0        0        0     1954 2024-04-26 18:10:43.000000 tkchart-2.1.3/src/tkchart/Utils.py
+-rw-rw-rw-   0        0        0     9885 2024-04-26 19:09:11.000000 tkchart-2.1.3/src/tkchart/Validate.py
+-rw-rw-rw-   0        0        0      433 2024-05-24 20:53:50.000000 tkchart-2.1.3/src/tkchart/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 21:13:32.013097 tkchart-2.1.3/src/tkchart.egg-info/
+-rw-rw-rw-   0        0        0     5667 2024-05-24 21:13:31.000000 tkchart-2.1.3/src/tkchart.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-05-24 21:13:31.000000 tkchart-2.1.3/src/tkchart.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 21:13:31.000000 tkchart-2.1.3/src/tkchart.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-24 21:13:31.000000 tkchart-2.1.3/src/tkchart.egg-info/top_level.txt
```

### Comparing `tkchart-2.1.2/LICENSE` & `tkchart-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tkchart-2.1.2/PKG-INFO` & `tkchart-2.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkchart
-Version: 2.1.2
+Version: 2.1.3
 Summary: tkchart is a Python library for creating live updating line charts in Tkinter.
 Author: Thisal-D
 License: Copyright (c) 2024 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -38,19 +38,20 @@
 
 [![tkchart](https://snyk.io/advisor/python/tkchart/badge.svg)](https://snyk.io/advisor/python/tkchart)
 
 <img src="https://drive.google.com/thumbnail?id=16Y00GIKEpmC4t3gAlUv7IJutE4yzFszo&sz=w2500" style="width: 100%">
 
 [![Downloads](https://static.pepy.tech/badge/tkchart)](https://pepy.tech/project/tkchart) [![Downloads](https://static.pepy.tech/badge/tkchart/month)](https://pepy.tech/project/tkchart) [![Downloads](https://static.pepy.tech/badge/tkchart/week)](https://pepy.tech/project/tkchart)
 
-<img src="https://drive.google.com/thumbnail?id=1uZJAjUZPIt79V0FMZ6KpF_x1ln7LFNmg&sz=w180">
+<img src="https://drive.google.com/thumbnail?id=1AxbfzWOvbTbH4uLDgoDgPZqorS6jlBCN&sz=w180">
 </div>
 
 **<li>tkchart is a Python library for creating live updating line charts in tkinter.</li>**
 
+
 ---
 
 ### Features
 
 - **Live Update**: Display live data with line charts.
 - **Multiple Lines**: Support for plotting multiple lines on the same chart for easy comparison.
 - **Color Customization**: Customize colors to match your application's design or data representation.
```

### Comparing `tkchart-2.1.2/README.md` & `tkchart-2.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 
 [![tkchart](https://snyk.io/advisor/python/tkchart/badge.svg)](https://snyk.io/advisor/python/tkchart)
 
 <img src="https://drive.google.com/thumbnail?id=16Y00GIKEpmC4t3gAlUv7IJutE4yzFszo&sz=w2500" style="width: 100%">
 
 [![Downloads](https://static.pepy.tech/badge/tkchart)](https://pepy.tech/project/tkchart) [![Downloads](https://static.pepy.tech/badge/tkchart/month)](https://pepy.tech/project/tkchart) [![Downloads](https://static.pepy.tech/badge/tkchart/week)](https://pepy.tech/project/tkchart)
 
-<img src="https://drive.google.com/thumbnail?id=1uZJAjUZPIt79V0FMZ6KpF_x1ln7LFNmg&sz=w180">
+<img src="https://drive.google.com/thumbnail?id=1AxbfzWOvbTbH4uLDgoDgPZqorS6jlBCN&sz=w180">
 </div>
 
 **<li>tkchart is a Python library for creating live updating line charts in tkinter.</li>**
 
+
 ---
 
 ### Features
 
 - **Live Update**: Display live data with line charts.
 - **Multiple Lines**: Support for plotting multiple lines on the same chart for easy comparison.
 - **Color Customization**: Customize colors to match your application's design or data representation.
```

### Comparing `tkchart-2.1.2/pyproject.toml` & `tkchart-2.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tkchart"
-version = "2.1.2"
+version = "2.1.3"
 authors = [
   { name = "Thisal-D" }
 ]
 
 license = { file = "LICENSE" }
 
 description = "tkchart is a Python library for creating live updating line charts in Tkinter."
```

### Comparing `tkchart-2.1.2/src/tkchart/FontStyle.py` & `tkchart-2.1.3/src/tkchart/FontStyle.py`

 * *Files identical despite different names*

### Comparing `tkchart-2.1.2/src/tkchart/Line.py` & `tkchart-2.1.3/src/tkchart/Line.py`

 * *Files 14% similar despite different names*

```diff
@@ -152,27 +152,27 @@
         self.__data = []
 
     def reset(self) -> None:
         """
         Reset the line.
         """
         self.__reset()
-        self.__master._LineChart__call_reshow_data()
+        self.__master._LineChart__apply_line_configuration()
 
     def set_visible(self, state: bool) -> None:
         """
         Set the visibility of the line.
 
         Args:
             state (bool): True if the line should be visible, False otherwise.
         """
         Validate._isBool(state, "state")
         if self.__visibility != state:
             self.__visibility = state
-            self.__master._LineChart__call_reshow_data()
+            self.__master._LineChart__apply_line_configuration()
 
     def cget(
             self,
             attribute_name: Literal[
                 "master", "color", "size", "style", "style_type", "point_highlight",
                 "point_highlight_size", "point_highlight_color", "fill", "fill_color",
                 "__all__"]) -> Any:
@@ -227,7 +227,41 @@
         """
         Get the visibility of the line.
 
         Returns:
             bool: True if the line is visible, False otherwise.
         """
         return self.__visibility
+
+    
+    def __del__(self) -> None:
+        """Destructor method to delete instance attributes."""
+        del self.__master
+        del self.__color
+        del self.__size
+        del self.__y_end
+        del self.__x_end
+        del self.__data
+        del self.__temp_data
+        del self.__ret_data
+        del self.__visibility
+        del self.__style
+        del self.__style_type
+        del self.__point_highlight
+        del self.__point_highlight_size
+        del self.__point_highlight_color
+        del self.__fill
+        del self.__fill_color
+
+    def destroy(self) -> None:
+        """
+        Removes the instance from its master's line chart and 
+        applies the updated line configuration. Calls the destructor 
+        to clean up resources.
+        """
+        try:
+            self.__master._LineChart__lines.remove(self)
+            self.__master._LineChart__apply_line_configuration()
+        except ValueError:
+            pass  # In case the line is not in the list
+        finally:
+            self.__del__()
```

### Comparing `tkchart-2.1.2/src/tkchart/LineChart.py` & `tkchart-2.1.3/src/tkchart/LineChart.py`

 * *Files 2% similar despite different names*

```diff
@@ -308,20 +308,20 @@
 
         self.__main_frame.configure(bg=self.__bg_color)
         self.__output_frame.configure(bg=self.__fg_color)
         self.__output_canvas.configure(bg=self.__fg_color)
 
         self.__y_axis_data_label.configure(bg=self.__bg_color, fg=self.__y_axis_data_font_color)
         for label in self.__x_axis_values_frame.winfo_children():
-            if type(label) == tkinter.Label:
+            if type(label) is tkinter.Label:
                 label.configure(bg=self.__bg_color, fg=self.__x_axis_font_color)
 
         self.__x_axis_data_label.configure(bg=self.__bg_color, fg=self.__x_axis_data_font_color)
         for label in self.__y_axis_values_frame.winfo_children():
-            if type(label) == tkinter.Label:
+            if type(label) is tkinter.Label:
                 label.configure(bg=self.__bg_color, fg=self.__y_axis_font_color)
 
         self.__pointer.configure(bg=self.__pointer_color)
 
     def __set_widgets_fonts(self) -> None:
         """
         Set the fonts for LineChart widgets.
@@ -331,19 +331,19 @@
         and x-axis values labels, using the specified data font style and axis font style.
         """
 
         self.__y_axis_data_label.configure(font=self.__data_font_style)
         self.__x_axis_data_label.configure(font=self.__data_font_style)
 
         for label in self.__y_axis_values_frame.winfo_children():
-            if type(label) == tkinter.Label:
+            if type(label) is tkinter.Label:
                 label.configure(font=self.__axis_font_style)
 
         for label in self.__x_axis_values_frame.winfo_children():
-            if type(label) == tkinter.Label:
+            if type(label) is tkinter.Label:
                 label.configure(font=self.__axis_font_style)
 
     def __set_pointer_size(self) -> None:
         """
         Set the size of the pointer.
 
         This method adjusts the width and height of the pointer widget based on the specified pointer size.
@@ -375,27 +375,26 @@
                     y=self.__y_space + self.__y_special_height_space + self.__real_height / 2,
                     anchor="w"
                 )
 
         if self.__x_axis_data != "":
             if self.__x_axis_data_position == "top":
                 self.__x_axis_data_label.place(
-                    rely=1,
                     relx=1,
                     x=-self.__x_axis_data_req_width,
-                    y=-self.__x_axis_data_req_height
+                    y=self.__height - self.__x_axis_data_req_height
                 )
             else:
                 self.__x_axis_data_label.place(
                     rely=1,
                     y=-self.__x_axis_data_req_height, relx=0, anchor="n",
                     x=(
-                        self.__const_real_width / 2 + self.__y_axis_data_req_width_space_side +
-                        self.__y_value_req_width_space + self.__axis_size + self.__x_axis_data_req_width_space_top +
-                        self.__x_special_width_space
+                            self.__const_real_width / 2 + self.__y_axis_data_req_width_space_side +
+                            self.__y_value_req_width_space + self.__axis_size + self.__x_axis_data_req_width_space_top +
+                            self.__x_special_width_space
                     )
                 )
 
         self.__y_axis_frame.configure(width=self.__axis_size)
         self.__x_axis_frame.configure(height=self.__axis_size)
 
         self.__y_axis_frame.place(
@@ -405,16 +404,16 @@
                 (self.__y_value_req_height_space / 2) +
                 self.__y_special_height_space
             ),
             height=self.__const_real_height + self.__y_space + self.__axis_size
         )
         self.__x_axis_frame.place(
             x=self.__y_value_req_width_space + self.__y_axis_data_req_width_space_side,
-            rely=1,
-            y=-self.__axis_size + -self.__x_value_req_height_space + -self.__x_axis_data_req_height_space_side,
+            y=(self.__height - self.__axis_size + -self.__x_value_req_height_space +
+               -self.__x_axis_data_req_height_space_side),
             width=self.__const_real_width + self.__axis_size + self.__x_space
         )
 
         self.__output_frame.place(
             x=self.__y_value_req_width_space + self.__axis_size + self.__y_axis_data_req_width_space_side,
             width=self.__const_real_width,
             height=self.__const_real_height,
@@ -434,16 +433,15 @@
             )
         else:
             self.__y_axis_values_frame.place_forget()
 
         if self.__x_values_frame_place_req:
             self.__x_axis_values_frame.place(
                 x=0,
-                rely=1,
-                y=-self.__x_value_req_height_space + -self.__x_axis_data_req_height_space_side,
+                y=self.__height - self.__x_value_req_height_space + -self.__x_axis_data_req_height_space_side,
                 height=self.__x_value_req_height_space,
                 width=self.__width
             )
         else:
             self.__x_axis_values_frame.place_forget()
 
     def __configure_x_axis_point_spacing(self) -> None:
@@ -850,15 +848,15 @@
         """
         Destroy all x-axis and y-axis sections.
 
         This method destroys all sections created on both the x-axis and y-axis by removing them from the output frame.
         """
 
         for widget in self.__output_frame.winfo_children():
-            if type(widget) == tkinter.Frame:
+            if type(widget) is tkinter.Frame:
                 widget.place_forget()
                 widget.destroy()
 
     def configure(
             self,
             width: int = None,
             height: int = None,
@@ -2080,7 +2078,116 @@
                 "columnspan": self.__grid_info_columnspan,
                 "padx": self.__grid_info_padx,
                 "pady": self.__grid_info_pady,
                 "sticky": self.__grid_info_sticky
             }
 
         Validate._invalidCget(attribute_name)
+
+    def __del__(self) -> None:
+        """
+        Destructor to clean up resources and perform necessary cleanup.
+        This method will be called when the object is about to be destroyed.
+        It ensures that all widgets are destroyed and attributes are deleted
+        to aid in garbage collection.
+        """
+        # Destroy widgets
+        self.__main_frame.destroy()
+        self.__x_axis_values_frame.destroy()
+        self.__y_axis_values_frame.destroy()
+        self.__y_axis_data_label.destroy()
+        self.__x_axis_data_label.destroy()
+        self.__output_frame.destroy()
+        self.__output_canvas.destroy()
+        self.__y_axis_frame.destroy()
+        self.__x_axis_frame.destroy()
+        self.__pointer.destroy()
+
+        # Deleting attributes to help with garbage collection
+        del self.__main_frame
+        del self.__x_axis_values_frame
+        del self.__y_axis_values_frame
+        del self.__y_axis_data_label
+        del self.__x_axis_data_label
+        del self.__output_frame
+        del self.__output_canvas
+        del self.__y_axis_frame
+        del self.__x_axis_frame
+        del self.__pointer
+        del self.__master
+        del self.__height
+        del self.__width
+        del self.__axis_size
+        del self.__axis_color
+        del self.__x_axis_point_spacing
+        del self.__x_axis_point_spacing_handle_by
+        del self.__data_font_style
+        del self.__axis_font_style
+        del self.__lines
+        del self.__bg_color
+        del self.__fg_color
+        del self.__y_axis_font_color
+        del self.__y_axis_data_font_color
+        del self.__y_axis_section_color
+        del self.__y_axis_section_style
+        del self.__y_axis_section_style_type
+        del self.__y_axis_section_count
+        del self.__y_axis_label_count
+        del self.__y_axis_data
+        del self.__y_axis_data_position
+        del self.__y_axis_values
+        del self.__y_axis_min_value
+        del self.__y_axis_max_value
+        del self.__y_axis_precision
+        del self.__y_space
+        del self.__x_axis_font_color
+        del self.__x_axis_data_font_color
+        del self.__x_axis_section_color
+        del self.__x_axis_section_style
+        del self.__x_axis_section_style_type
+        del self.__x_axis_section_count
+        del self.__x_axis_label_count
+        del self.__x_axis_display_values_indices
+        del self.__x_labels_values_index_change
+        del self.__x_axis_data
+        del self.__x_axis_data_position
+        del self.__x_axis_values
+        del self.__x_axis_values_handle_by
+        del self.__x_space
+        del self.__pointer_state
+        del self.__pointing_callback_function
+        del self.__pointing_values_precision
+        del self.__pointer_lock
+        del self.__pointer_size
+        del self.__pointer_color
+        del self.__x_values_frame_place_req
+        del self.__y_values_frame_place_req
+        del self.__place_x
+        del self.__real_height
+        del self.__real_width
+        del self.__const_real_height
+        del self.__const_real_width
+        del self.__visibility
+        del self.__place_info_x
+        del self.__place_info_y
+        del self.__place_info_rely
+        del self.__place_info_relx
+        del self.__place_info_anchor
+        del self.__pack_info_pady
+        del self.__pack_info_padx
+        del self.__pack_info_before
+        del self.__pack_info_after
+        del self.__pack_info_side
+        del self.__pack_info_anchor
+        del self.__grid_info_column
+        del self.__grid_info_columnspan
+        del self.__grid_info_padx
+        del self.__grid_info_pady
+        del self.__grid_info_row
+        del self.__grid_info_rowspan
+        del self.__grid_info_sticky
+
+    def destroy(self) -> None:
+        for line in self.__lines:
+            line.destroy()
+
+        self.__del__()
```

### Comparing `tkchart-2.1.2/src/tkchart/Utils.py` & `tkchart-2.1.3/src/tkchart/Utils.py`

 * *Files identical despite different names*

### Comparing `tkchart-2.1.2/src/tkchart/Validate.py` & `tkchart-2.1.3/src/tkchart/Validate.py`

 * *Files identical despite different names*

### Comparing `tkchart-2.1.2/src/tkchart.egg-info/PKG-INFO` & `tkchart-2.1.3/src/tkchart.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkchart
-Version: 2.1.2
+Version: 2.1.3
 Summary: tkchart is a Python library for creating live updating line charts in Tkinter.
 Author: Thisal-D
 License: Copyright (c) 2024 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -38,19 +38,20 @@
 
 [![tkchart](https://snyk.io/advisor/python/tkchart/badge.svg)](https://snyk.io/advisor/python/tkchart)
 
 <img src="https://drive.google.com/thumbnail?id=16Y00GIKEpmC4t3gAlUv7IJutE4yzFszo&sz=w2500" style="width: 100%">
 
 [![Downloads](https://static.pepy.tech/badge/tkchart)](https://pepy.tech/project/tkchart) [![Downloads](https://static.pepy.tech/badge/tkchart/month)](https://pepy.tech/project/tkchart) [![Downloads](https://static.pepy.tech/badge/tkchart/week)](https://pepy.tech/project/tkchart)
 
-<img src="https://drive.google.com/thumbnail?id=1uZJAjUZPIt79V0FMZ6KpF_x1ln7LFNmg&sz=w180">
+<img src="https://drive.google.com/thumbnail?id=1AxbfzWOvbTbH4uLDgoDgPZqorS6jlBCN&sz=w180">
 </div>
 
 **<li>tkchart is a Python library for creating live updating line charts in tkinter.</li>**
 
+
 ---
 
 ### Features
 
 - **Live Update**: Display live data with line charts.
 - **Multiple Lines**: Support for plotting multiple lines on the same chart for easy comparison.
 - **Color Customization**: Customize colors to match your application's design or data representation.
```


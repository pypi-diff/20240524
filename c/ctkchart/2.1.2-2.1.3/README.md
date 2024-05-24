# Comparing `tmp/ctkchart-2.1.2.tar.gz` & `tmp/ctkchart-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctkchart-2.1.2.tar", last modified: Sat Apr 27 04:34:04 2024, max compression
+gzip compressed data, was "ctkchart-2.1.3.tar", last modified: Fri May 24 21:18:26 2024, max compression
```

## Comparing `ctkchart-2.1.2.tar` & `ctkchart-2.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 04:34:04.982429 ctkchart-2.1.2/
--rw-rw-rw-   0        0        0     1091 2024-02-14 05:02:34.000000 ctkchart-2.1.2/LICENSE
--rw-rw-rw-   0        0        0     5254 2024-04-27 04:34:04.982429 ctkchart-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3385 2024-04-27 04:33:49.000000 ctkchart-2.1.2/README.md
--rw-rw-rw-   0        0        0     1545 2024-04-27 04:24:48.000000 ctkchart-2.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       13 2024-04-15 03:53:34.000000 ctkchart-2.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 04:34:04.983410 ctkchart-2.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-27 04:34:04.972037 ctkchart-2.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-27 04:34:04.978508 ctkchart-2.1.2/src/ctkchart/
--rw-rw-rw-   0        0        0     9246 2024-04-26 18:04:37.000000 ctkchart-2.1.2/src/ctkchart/CTkLine.py
--rw-rw-rw-   0        0        0   101695 2024-04-26 18:17:01.000000 ctkchart-2.1.2/src/ctkchart/CTkLineChart.py
--rw-rw-rw-   0        0        0     1559 2024-04-26 08:35:50.000000 ctkchart-2.1.2/src/ctkchart/FontStyle.py
--rw-rw-rw-   0        0        0     1539 2024-04-26 15:17:46.000000 ctkchart-2.1.2/src/ctkchart/ThemeManager.py
--rw-rw-rw-   0        0        0     2066 2024-04-26 18:10:27.000000 ctkchart-2.1.2/src/ctkchart/Utils.py
--rw-rw-rw-   0        0        0    10441 2024-04-26 18:01:26.000000 ctkchart-2.1.2/src/ctkchart/Validate.py
--rw-rw-rw-   0        0        0      450 2024-04-26 18:13:14.000000 ctkchart-2.1.2/src/ctkchart/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 04:34:04.981448 ctkchart-2.1.2/src/ctkchart.egg-info/
--rw-rw-rw-   0        0        0     5254 2024-04-27 04:34:04.000000 ctkchart-2.1.2/src/ctkchart.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      415 2024-04-27 04:34:04.000000 ctkchart-2.1.2/src/ctkchart.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 04:34:04.000000 ctkchart-2.1.2/src/ctkchart.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-04-27 04:34:04.000000 ctkchart-2.1.2/src/ctkchart.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-27 04:34:04.000000 ctkchart-2.1.2/src/ctkchart.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 21:18:26.875339 ctkchart-2.1.3/
+-rw-rw-rw-   0        0        0     1091 2024-02-14 05:02:34.000000 ctkchart-2.1.3/LICENSE
+-rw-rw-rw-   0        0        0     5256 2024-05-24 21:18:26.875339 ctkchart-2.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3386 2024-05-24 21:12:45.000000 ctkchart-2.1.3/README.md
+-rw-rw-rw-   0        0        0     1545 2024-05-24 21:17:32.000000 ctkchart-2.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       13 2024-04-15 03:53:34.000000 ctkchart-2.1.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-24 21:18:26.875339 ctkchart-2.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-24 21:18:26.808379 ctkchart-2.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-24 21:18:26.842791 ctkchart-2.1.3/src/ctkchart/
+-rw-rw-rw-   0        0        0    10339 2024-05-24 20:23:52.000000 ctkchart-2.1.3/src/ctkchart/CTkLine.py
+-rw-rw-rw-   0        0        0   105753 2024-05-24 20:39:08.000000 ctkchart-2.1.3/src/ctkchart/CTkLineChart.py
+-rw-rw-rw-   0        0        0     1559 2024-04-26 08:35:50.000000 ctkchart-2.1.3/src/ctkchart/FontStyle.py
+-rw-rw-rw-   0        0        0     1725 2024-05-24 20:31:51.000000 ctkchart-2.1.3/src/ctkchart/ThemeManager.py
+-rw-rw-rw-   0        0        0     2066 2024-04-26 18:10:27.000000 ctkchart-2.1.3/src/ctkchart/Utils.py
+-rw-rw-rw-   0        0        0    10441 2024-04-26 18:01:26.000000 ctkchart-2.1.3/src/ctkchart/Validate.py
+-rw-rw-rw-   0        0        0      450 2024-05-24 17:25:25.000000 ctkchart-2.1.3/src/ctkchart/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 21:18:26.875339 ctkchart-2.1.3/src/ctkchart.egg-info/
+-rw-rw-rw-   0        0        0     5256 2024-05-24 21:18:26.000000 ctkchart-2.1.3/src/ctkchart.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      415 2024-05-24 21:18:26.000000 ctkchart-2.1.3/src/ctkchart.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 21:18:26.000000 ctkchart-2.1.3/src/ctkchart.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-05-24 21:18:26.000000 ctkchart-2.1.3/src/ctkchart.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-24 21:18:26.000000 ctkchart-2.1.3/src/ctkchart.egg-info/top_level.txt
```

### Comparing `ctkchart-2.1.2/LICENSE` & `ctkchart-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ctkchart-2.1.2/PKG-INFO` & `ctkchart-2.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctkchart
-Version: 2.1.2
+Version: 2.1.3
 Summary: ctkchart is a Python library for creating live updating line charts in customtkinter.
 Author: Thisal-D
 License: Copyright (c) 2024 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -35,15 +35,16 @@
 
 [![ctkchart](https://snyk.io/advisor/python/ctkchart/badge.svg)](https://snyk.io/advisor/python/ctkchart)
 
 <img src="https://drive.google.com/thumbnail?id=1f4Q2dA64iJGUVWpAZsl0q6Mq0NVkGCDR&sz=w900">
 
 [![Downloads](https://static.pepy.tech/badge/ctkchart)](https://pepy.tech/project/ctkchart) [![Downloads](https://static.pepy.tech/badge/ctkchart/month)](https://pepy.tech/project/ctkchart) [![Downloads](https://static.pepy.tech/badge/ctkchart/week)](https://pepy.tech/project/ctkchart)
 
-<img src="https://drive.google.com/thumbnail?id=1uZJAjUZPIt79V0FMZ6KpF_x1ln7LFNmg&sz=w180">
+<img src="https://drive.google.com/thumbnail?id=1AxbfzWOvbTbH4uLDgoDgPZqorS6jlBCN&sz=w180">
+
 
 </div>
 
 **<li>ctkchart is a  python library for creating live updating line charts in customtkinter.</li>**
 
 ---
```

### Comparing `ctkchart-2.1.2/README.md` & `ctkchart-2.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 [![ctkchart](https://snyk.io/advisor/python/ctkchart/badge.svg)](https://snyk.io/advisor/python/ctkchart)
 
 <img src="https://drive.google.com/thumbnail?id=1f4Q2dA64iJGUVWpAZsl0q6Mq0NVkGCDR&sz=w900">
 
 [![Downloads](https://static.pepy.tech/badge/ctkchart)](https://pepy.tech/project/ctkchart) [![Downloads](https://static.pepy.tech/badge/ctkchart/month)](https://pepy.tech/project/ctkchart) [![Downloads](https://static.pepy.tech/badge/ctkchart/week)](https://pepy.tech/project/ctkchart)
 
-<img src="https://drive.google.com/thumbnail?id=1uZJAjUZPIt79V0FMZ6KpF_x1ln7LFNmg&sz=w180">
+<img src="https://drive.google.com/thumbnail?id=1AxbfzWOvbTbH4uLDgoDgPZqorS6jlBCN&sz=w180">
+
 
 </div>
 
 **<li>ctkchart is a  python library for creating live updating line charts in customtkinter.</li>**
 
 ---
```

### Comparing `ctkchart-2.1.2/pyproject.toml` & `ctkchart-2.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ctkchart"
-version = "2.1.2"
+version = "2.1.3"
 authors = [{ name = "Thisal-D" }]
 license = { file = "LICENSE" }
 description = "ctkchart is a Python library for creating live updating line charts in customtkinter."
 readme = "README.md"
 requires-python = ">=3.0"
 
 dynamic = ["dependencies", "optional-dependencies"]
```

### Comparing `ctkchart-2.1.2/src/ctkchart/CTkLine.py` & `ctkchart-2.1.3/src/ctkchart/CTkLine.py`

 * *Files 17% similar despite different names*

```diff
@@ -156,27 +156,27 @@
         self.__data = []
 
     def reset(self) -> None:
         """
         Reset the line.
         """
         self.__reset()
-        self.__master._CTkLineChart__call_reshow_data()
+        self.__master._CTkLineChart__apply_line_configuration()
 
     def set_visible(self, state: bool) -> None:
         """
         Set the visibility of the line.
 
         Args:
             state (bool): True if the line should be visible, False otherwise.
         """
         Validate._isBool(state, "state")
         if self.__visibility != state:
             self.__visibility = state
-            self.__master._CTkLineChart__call_reshow_data()
+            self.__master._CTkLineChart__apply_line_configuration()
 
     def cget(
             self,
             attribute_name: Literal[
                 "master", "color", "size", "style", "style_type", "point_highlight",
                 "point_highlight_size", "point_highlight_color", "fill", "fill_color",
                 "__all__"]) -> any:
@@ -231,7 +231,40 @@
         Get the visibility of the line.
 
         Returns:
             bool: True if the line is visible, False otherwise.
         """
 
         return self.__visibility
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
+            self.__master._CTkLineChart__lines.remove(self)
+            self.__master._CTkLineChart__apply_line_configuration()
+        except ValueError:
+            pass  # In case the line is not in the list
+        finally:
+            self.__del__()
```

### Comparing `ctkchart-2.1.2/src/ctkchart/CTkLineChart.py` & `ctkchart-2.1.3/src/ctkchart/CTkLineChart.py`

 * *Files 11% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             pointer_lock: Literal["enabled", "disabled"] = "disabled",
             pointer_size: int = 1,
 
             *args: Any) -> None:
         """
         Initialize Theme manager
         """
-
+        ThemeManager.bind_widget(self)
         if ThemeManager.running_state is not True:
             ThemeManager.run()
 
         """
         Initialize the CTkLineChart.
 
         Args:
@@ -150,19 +150,19 @@
         Validate._isValidPointerState_Lock(pointer_state, "pointer_state")
         Validate._isValidPointerState_Lock(pointer_lock, "pointer_lock")
         Validate._isValidFunction(pointing_callback_function, "pointing_callback_function")
         Validate._isValidXAxisIndices(x_axis_values, x_axis_display_values_indices, "x_axis_display_values_indices")
         Validate._isValidXAxisLabelCount(x_axis_label_count, "x_axis_label_count")
 
         if master is not None:
-            self.master = master
+            self.__master = master
         elif len(args) != 0:
-            self.master = args[0]
+            self.__master = args[0]
         else:
-            self.master = master
+            self.__master = master
 
         self.__height: int = height
         self.__width: int = width
         self.__axis_size: int = axis_size
         self.__axis_color: Union[Tuple[str, str], str] = axis_color
         self.__x_axis_point_spacing: Union[int, float, Literal["auto"]] = x_axis_point_spacing
         self.__x_axis_point_spacing_handle_by: str = "auto"
@@ -176,15 +176,15 @@
         self.__y_axis_section_color: Union[Tuple[str, str], str] = y_axis_section_color
         self.__y_axis_section_style: Literal["normal", "dashed"] = y_axis_section_style
         self.__y_axis_section_style_type: Tuple[int, int] = y_axis_section_style_type
         self.__y_axis_section_count: int = y_axis_section_count
         self.__y_axis_label_count: int = y_axis_label_count
         self.__y_axis_data = str(y_axis_data)
         self.__y_axis_data_position: Literal["top", "side"] = y_axis_data_position
-        self.__y_axis_values: Tuple[Union[int,float], Union[int, float]] = y_axis_values
+        self.__y_axis_values: Tuple[Union[int, float], Union[int, float]] = y_axis_values
         self.__y_axis_min_value: Union[int, float] = y_axis_values[0]
         self.__y_axis_max_value: Union[int, float] = y_axis_values[1]
         self.__y_axis_precision: int = y_axis_precision
         self.__y_space: int = y_space
         self.__x_axis_font_color: Union[Tuple[str, str], str] = x_axis_font_color
         self.__x_axis_data_font_color: Union[Tuple[str, str], str] = x_axis_data_font_color
         self.__x_axis_section_color: Union[Tuple[str, str], str] = x_axis_section_color
@@ -198,17 +198,17 @@
         self.__x_axis_data_position: Literal["top", "side"] = x_axis_data_position
         self.__x_axis_values: Tuple[Any, ...] = x_axis_values
         self.__x_axis_values_handle_by: str = "label_count"
         self.__x_space: int = x_space
         self.__pointer_state: Literal["enabled", 'disabled'] = pointer_state
         self.__pointing_callback_function: Callable = pointing_callback_function
         self.__pointing_values_precision: int = pointing_values_precision
-        self.__pointer_lock: Literal["enabled", 'disabled']  = pointer_lock
+        self.__pointer_lock: Literal["enabled", 'disabled'] = pointer_lock
         self.__pointer_size: int = pointer_size
-        self.__pointer_color: Union[Tuple[str, str], str]  = pointer_color
+        self.__pointer_color: Union[Tuple[str, str], str] = pointer_color
         self.__x_values_frame_place_req: bool = True
         self.__y_values_frame_place_req: bool = True
 
         self.__place_x: int = 0
         self.__real_height: int = 0
         self.__real_width: int = 0
         self.__const_real_height: int = 0
@@ -265,15 +265,14 @@
         self.__set_pointer_size()
         self.__set_widgets_fonts()
         self.__set_customtkinter_widgets_colors()
         self.__set_tkinter_widgets_colors()
         self.__place_widgets()
         self.__reset_chart_info()
         self.__configure_theme_mode()
-        ThemeManager.bind_widget(self)
 
     def __configure_theme_mode(self) -> None:
         """
         Configure the widget appearance to match changes in the theme.
 
         This method adjusts the colors and sections of the widget to match the current theme.
         """
@@ -289,15 +288,15 @@
         Create widgets for the CTkLineChart.
 
         This method initializes the main frame along with frames for the y-axis, x-axis,
         y-axis values, x-axis values, y-axis data label, x-axis data label, output frame,
         output canvas, and pointer.
         """
 
-        self.__main_frame = customtkinter.CTkFrame(master=self.master)
+        self.__main_frame = customtkinter.CTkFrame(master=self.__master)
         self.__x_axis_values_frame = customtkinter.CTkFrame(master=self.__main_frame)
         self.__y_axis_values_frame = customtkinter.CTkFrame(master=self.__main_frame)
         self.__y_axis_data_label = customtkinter.CTkLabel(master=self.__main_frame)
         self.__x_axis_data_label = customtkinter.CTkLabel(master=self.__main_frame)
         self.__output_frame = customtkinter.CTkFrame(master=self.__main_frame)
         self.__output_canvas = tkinter.Canvas(master=self.__output_frame, highlightthickness=0)
         self.__y_axis_frame = tkinter.Frame(master=self.__main_frame)
@@ -422,18 +421,17 @@
                     y=self.__y_space + self.__y_special_height_space + self.__real_height / 2,
                     anchor="w"
                 )
 
         if self.__x_axis_data != "":
             if self.__x_axis_data_position == "top":
                 self.__x_axis_data_label.place(
-                    rely=1,
                     relx=1,
                     x=-self.__x_axis_data_req_width + -self.__margin,
-                    y=-self.__x_axis_data_req_height
+                    y=self.__height - self.__x_axis_data_req_height
                 )
             else:
                 self.__x_axis_data_label.place(
                     rely=1,
                     y=-self.__x_axis_data_req_height,
                     relx=0,
                     anchor="n",
@@ -454,16 +452,16 @@
                 (self.__y_value_req_height_space / 2) +
                 self.__y_special_height_space
             ),
         )
         self.__y_axis_frame.configure(height=self.__const_real_height + self.__y_space + self.__axis_size)
         self.__x_axis_frame.place(
             x=self.__y_value_req_width_space + self.__y_axis_data_req_width_space_side + self.__margin,
-            rely=1,
-            y=-self.__axis_size + -self.__x_value_req_height_space + -self.__x_axis_data_req_height_space_side,
+            y=(self.__height - self.__axis_size + -self.__x_value_req_height_space +
+               -self.__x_axis_data_req_height_space_side),
         )
 
         self.__x_axis_frame.configure(width=self.__const_real_width + self.__axis_size + self.__x_space)
 
         self.__output_frame.place(
             x=(
                 self.__y_value_req_width_space + self.__axis_size + self.__y_axis_data_req_width_space_side +
@@ -486,16 +484,16 @@
             self.__y_axis_values_frame.place(x=self.__y_axis_data_req_width_space_side + self.__margin)
             self.__y_axis_values_frame.configure(width=self.__y_value_req_width_space, height=self.__height)
         else:
             self.__y_axis_values_frame.place_forget()
 
         if self.__x_values_frame_place_req:
             self.__x_axis_values_frame.place(
-                x=self.__margin, rely=1,
-                y=-self.__x_value_req_height_space + -self.__x_axis_data_req_height_space_side
+                x=self.__margin,
+                y=self.__height - self.__x_value_req_height_space + -self.__x_axis_data_req_height_space_side
             )
             self.__x_axis_values_frame.configure(
                 height=self.__x_value_req_height_space,
                 width=self.__width - (self.__margin * 2)
             )
         else:
             self.__x_axis_values_frame.place_forget()
@@ -551,15 +549,15 @@
         self.__x_values_frame_place_req = True
         # self.__y_axis_data_req_height = Utils._RequiredHeight(text=self.__y_axis_data, font=self.__data_font_style)
         # self.__y_axis_data_req_width = Utils._RequiredWidth(text=self.__y_axis_data, font=self.__data_font_style)
         if self.__y_axis_data != "":
             if self.__y_axis_data_position == "top":
                 self.__y_special_height_space = 15
                 self.__y_axis_data_req_height_space_top = Utils._RequiredHeight(
-                    text=self.__y_axis_data,font=self.__data_font_style
+                    text=self.__y_axis_data, font=self.__data_font_style
                 )
             else:
                 self.__y_axis_data_req_width_space_side = Utils._RequiredWidth(
                     text=self.__y_axis_data[0], font=self.__data_font_style
                 )
 
         if self.__y_axis_label_count == 0:
@@ -2137,7 +2135,119 @@
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
+        del self.__theme
+        del self.__margin
+
+    def destroy(self) -> None:
+        ThemeManager.unbind_widget(self)
+        for line in self.__lines:
+            line.destroy()
+
+        self.__del__()
```

### Comparing `ctkchart-2.1.2/src/ctkchart/FontStyle.py` & `ctkchart-2.1.3/src/ctkchart/FontStyle.py`

 * *Files identical despite different names*

### Comparing `ctkchart-2.1.2/src/ctkchart/ThemeManager.py` & `ctkchart-2.1.3/src/ctkchart/ThemeManager.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,35 +17,37 @@
             else:
                 return color_s[1]
         else:
             return color_s
 
     @staticmethod
     def theme_tracker() -> None:
-        while True:
+        while len(ThemeManager.child_objects) != 0:
             if ctk.get_appearance_mode() != ThemeManager.theme:
                 ThemeManager.theme = ctk.get_appearance_mode()
                 for child_object in ThemeManager.child_objects:
                     try:
                         child_object._CTkLineChart__configure_theme_mode()
-                    except:
-                        try:
-                            ThemeManager.child_objects.remove(child_object)
-                        except:
-                            pass
+                    except Exception as error:
+                        print(f"Line Chart theme configure failed : {error}")
+                        
             time.sleep(1)
+        ThemeManager.running_state = False
 
     @staticmethod
     def run():
-        running_state = True
-        threading.Thread(target=ThemeManager.theme_tracker).start()
-
+        ThemeManager.running_state = True
+        thread = threading.Thread(target=ThemeManager.theme_tracker)
+        thread.daemon = True
+        thread.start()
+    
     @staticmethod
     def bind_widget(widget: Any) -> None:
         ThemeManager.child_objects.append(widget)
 
     @staticmethod
     def unbind_widget(widget: Any) -> None:
         try:
             ThemeManager.child_objects.remove(widget)
-        except:
-            pass
+        except Exception as error:
+            print(f"Unable to remove widgets from Theme Manager : {error}")
+
```

### Comparing `ctkchart-2.1.2/src/ctkchart/Utils.py` & `ctkchart-2.1.3/src/ctkchart/Utils.py`

 * *Files identical despite different names*

### Comparing `ctkchart-2.1.2/src/ctkchart/Validate.py` & `ctkchart-2.1.3/src/ctkchart/Validate.py`

 * *Files identical despite different names*

### Comparing `ctkchart-2.1.2/src/ctkchart.egg-info/PKG-INFO` & `ctkchart-2.1.3/src/ctkchart.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctkchart
-Version: 2.1.2
+Version: 2.1.3
 Summary: ctkchart is a Python library for creating live updating line charts in customtkinter.
 Author: Thisal-D
 License: Copyright (c) 2024 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -35,15 +35,16 @@
 
 [![ctkchart](https://snyk.io/advisor/python/ctkchart/badge.svg)](https://snyk.io/advisor/python/ctkchart)
 
 <img src="https://drive.google.com/thumbnail?id=1f4Q2dA64iJGUVWpAZsl0q6Mq0NVkGCDR&sz=w900">
 
 [![Downloads](https://static.pepy.tech/badge/ctkchart)](https://pepy.tech/project/ctkchart) [![Downloads](https://static.pepy.tech/badge/ctkchart/month)](https://pepy.tech/project/ctkchart) [![Downloads](https://static.pepy.tech/badge/ctkchart/week)](https://pepy.tech/project/ctkchart)
 
-<img src="https://drive.google.com/thumbnail?id=1uZJAjUZPIt79V0FMZ6KpF_x1ln7LFNmg&sz=w180">
+<img src="https://drive.google.com/thumbnail?id=1AxbfzWOvbTbH4uLDgoDgPZqorS6jlBCN&sz=w180">
+
 
 </div>
 
 **<li>ctkchart is a  python library for creating live updating line charts in customtkinter.</li>**
 
 ---
```


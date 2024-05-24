# Comparing `tmp/imviz-0.2.4.tar.gz` & `tmp/imviz-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imviz-0.2.4.tar", last modified: Thu May  2 10:12:15 2024, max compression
+gzip compressed data, was "imviz-0.2.5.tar", last modified: Fri May 24 08:47:33 2024, max compression
```

## Comparing `imviz-0.2.4.tar` & `imviz-0.2.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 ruof      (1000) ruof      (1000)        0 2024-05-02 10:12:15.711217 imviz-0.2.4/
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     5499 2024-05-02 10:00:45.000000 imviz-0.2.4/CMakeLists.txt
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     1071 2024-05-02 10:00:45.000000 imviz-0.2.4/LICENSE
--rw-rw-r--   0 ruof      (1000) ruof      (1000)       61 2021-11-18 07:19:23.000000 imviz-0.2.4/MANIFEST.in
--rw-r--r--   0 ruof      (1000) ruof      (1000)     2410 2024-05-02 10:12:15.711217 imviz-0.2.4/PKG-INFO
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     2006 2024-05-02 10:00:45.000000 imviz-0.2.4/README.md
-drwxrwxr-x   0 ruof      (1000) ruof      (1000)        0 2024-05-02 10:12:15.707217 imviz-0.2.4/imviz/
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     1677 2024-05-02 09:40:07.000000 imviz-0.2.4/imviz/__init__.py
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     9777 2024-05-02 10:00:53.000000 imviz-0.2.4/imviz/autogui.py
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     6200 2024-05-02 09:40:07.000000 imviz-0.2.4/imviz/common.py
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     5573 2024-05-02 09:40:07.000000 imviz-0.2.4/imviz/dev.py
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     1187 2024-05-02 09:40:07.000000 imviz-0.2.4/imviz/dev_main.py
--rw-rw-r--   0 ruof      (1000) ruof      (1000)    23863 2024-05-02 09:40:07.000000 imviz-0.2.4/imviz/export.py
--rw-rw-r--   0 ruof      (1000) ruof      (1000)       33 2024-05-02 09:40:07.000000 imviz-0.2.4/imviz/storage.py
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     1824 2023-08-10 10:02:29.000000 imviz-0.2.4/imviz/task.py
-drwxrwxr-x   0 ruof      (1000) ruof      (1000)        0 2024-05-02 10:12:15.711217 imviz-0.2.4/imviz.egg-info/
--rw-r--r--   0 ruof      (1000) ruof      (1000)     2410 2024-05-02 10:12:15.000000 imviz-0.2.4/imviz.egg-info/PKG-INFO
--rw-rw-r--   0 ruof      (1000) ruof      (1000)      731 2024-05-02 10:12:15.000000 imviz-0.2.4/imviz.egg-info/SOURCES.txt
--rw-rw-r--   0 ruof      (1000) ruof      (1000)        1 2024-05-02 10:12:15.000000 imviz-0.2.4/imviz.egg-info/dependency_links.txt
--rw-rw-r--   0 ruof      (1000) ruof      (1000)        1 2024-05-02 10:12:15.000000 imviz-0.2.4/imviz.egg-info/not-zip-safe
--rw-rw-r--   0 ruof      (1000) ruof      (1000)       56 2024-05-02 10:12:15.000000 imviz-0.2.4/imviz.egg-info/requires.txt
--rw-rw-r--   0 ruof      (1000) ruof      (1000)       15 2024-05-02 10:12:15.000000 imviz-0.2.4/imviz.egg-info/top_level.txt
--rw-rw-r--   0 ruof      (1000) ruof      (1000)      117 2024-05-02 09:40:07.000000 imviz-0.2.4/pyproject.toml
--rw-rw-r--   0 ruof      (1000) ruof      (1000)       38 2024-05-02 10:12:15.711217 imviz-0.2.4/setup.cfg
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     4337 2024-05-02 10:00:45.000000 imviz-0.2.4/setup.py
-drwxrwxr-x   0 ruof      (1000) ruof      (1000)        0 2024-05-02 10:12:15.711217 imviz-0.2.4/src/
--rw-rw-r--   0 ruof      (1000) ruof      (1000)    10227 2024-05-02 09:40:07.000000 imviz-0.2.4/src/binding_helpers.cpp
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     5202 2024-05-02 09:40:07.000000 imviz-0.2.4/src/binding_helpers.hpp
--rw-rw-r--   0 ruof      (1000) ruof      (1000)    14972 2024-05-02 10:00:45.000000 imviz-0.2.4/src/bindings.cpp
--rw-rw-r--   0 ruof      (1000) ruof      (1000)    73814 2024-05-02 10:00:45.000000 imviz-0.2.4/src/bindings_imgui.cpp
--rw-rw-r--   0 ruof      (1000) ruof      (1000)      146 2023-02-13 10:53:33.000000 imviz-0.2.4/src/bindings_imgui.hpp
--rw-rw-r--   0 ruof      (1000) ruof      (1000)    36660 2024-05-02 10:00:45.000000 imviz-0.2.4/src/bindings_implot.cpp
--rw-rw-r--   0 ruof      (1000) ruof      (1000)      125 2023-02-13 10:53:33.000000 imviz-0.2.4/src/bindings_implot.hpp
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     5856 2024-05-02 09:40:07.000000 imviz-0.2.4/src/file_dialog.cpp
--rw-rw-r--   0 ruof      (1000) ruof      (1000)      204 2023-09-14 13:48:19.000000 imviz-0.2.4/src/file_dialog.hpp
--rw-rw-r--   0 ruof      (1000) ruof      (1000)      159 2024-05-02 10:00:45.000000 imviz-0.2.4/src/im_user_config.h
--rw-rw-r--   0 ruof      (1000) ruof      (1000)    11091 2024-05-02 09:40:07.000000 imviz-0.2.4/src/implot_ext.cpp
--rw-rw-r--   0 ruof      (1000) ruof      (1000)      229 2024-05-02 09:40:07.000000 imviz-0.2.4/src/implot_ext.hpp
--rw-rw-r--   0 ruof      (1000) ruof      (1000)    10847 2024-05-02 10:00:45.000000 imviz-0.2.4/src/imviz.cpp
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     1116 2024-05-02 10:00:45.000000 imviz-0.2.4/src/imviz.hpp
--rw-rw-r--   0 ruof      (1000) ruof      (1000)    17988 2023-02-13 10:53:33.000000 imviz-0.2.4/src/input.cpp
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     1464 2023-02-13 10:53:33.000000 imviz-0.2.4/src/input.hpp
--rw-rw-r--   0 ruof      (1000) ruof      (1000)   558672 2023-02-13 10:53:33.000000 imviz-0.2.4/src/source_sans_pro.cpp
--rw-rw-r--   0 ruof      (1000) ruof      (1000)       95 2023-02-13 10:53:33.000000 imviz-0.2.4/src/source_sans_pro.hpp
+drwxrwxr-x   0 ruof      (1000) ruof      (1000)        0 2024-05-24 08:47:33.379793 imviz-0.2.5/
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     5439 2024-05-24 08:46:08.000000 imviz-0.2.5/CMakeLists.txt
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     1071 2024-05-02 10:00:45.000000 imviz-0.2.5/LICENSE
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)       61 2021-11-18 07:19:23.000000 imviz-0.2.5/MANIFEST.in
+-rw-r--r--   0 ruof      (1000) ruof      (1000)     2410 2024-05-24 08:47:33.379793 imviz-0.2.5/PKG-INFO
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     2006 2024-05-02 10:00:45.000000 imviz-0.2.5/README.md
+drwxrwxr-x   0 ruof      (1000) ruof      (1000)        0 2024-05-24 08:47:33.371793 imviz-0.2.5/imviz/
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     1677 2024-05-02 09:40:07.000000 imviz-0.2.5/imviz/__init__.py
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     9803 2024-05-24 08:46:08.000000 imviz-0.2.5/imviz/autogui.py
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     6200 2024-05-02 09:40:07.000000 imviz-0.2.5/imviz/common.py
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     5573 2024-05-02 09:40:07.000000 imviz-0.2.5/imviz/dev.py
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     1187 2024-05-02 09:40:07.000000 imviz-0.2.5/imviz/dev_main.py
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)    23863 2024-05-02 09:40:07.000000 imviz-0.2.5/imviz/export.py
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)       33 2024-05-02 09:40:07.000000 imviz-0.2.5/imviz/storage.py
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     1824 2023-08-10 10:02:29.000000 imviz-0.2.5/imviz/task.py
+drwxrwxr-x   0 ruof      (1000) ruof      (1000)        0 2024-05-24 08:47:33.379793 imviz-0.2.5/imviz.egg-info/
+-rw-r--r--   0 ruof      (1000) ruof      (1000)     2410 2024-05-24 08:47:33.000000 imviz-0.2.5/imviz.egg-info/PKG-INFO
+-rw-r--r--   0 ruof      (1000) ruof      (1000)      731 2024-05-24 08:47:33.000000 imviz-0.2.5/imviz.egg-info/SOURCES.txt
+-rw-r--r--   0 ruof      (1000) ruof      (1000)        1 2024-05-24 08:47:33.000000 imviz-0.2.5/imviz.egg-info/dependency_links.txt
+-rw-r--r--   0 ruof      (1000) ruof      (1000)        1 2024-05-24 06:15:13.000000 imviz-0.2.5/imviz.egg-info/not-zip-safe
+-rw-r--r--   0 ruof      (1000) ruof      (1000)       56 2024-05-24 08:47:33.000000 imviz-0.2.5/imviz.egg-info/requires.txt
+-rw-r--r--   0 ruof      (1000) ruof      (1000)       15 2024-05-24 08:47:33.000000 imviz-0.2.5/imviz.egg-info/top_level.txt
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)      117 2024-05-02 09:40:07.000000 imviz-0.2.5/pyproject.toml
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)       38 2024-05-24 08:47:33.379793 imviz-0.2.5/setup.cfg
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     4337 2024-05-24 08:45:28.000000 imviz-0.2.5/setup.py
+drwxrwxr-x   0 ruof      (1000) ruof      (1000)        0 2024-05-24 08:47:33.375793 imviz-0.2.5/src/
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)    10227 2024-05-02 09:40:07.000000 imviz-0.2.5/src/binding_helpers.cpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     5202 2024-05-02 09:40:07.000000 imviz-0.2.5/src/binding_helpers.hpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)    14972 2024-05-02 10:00:45.000000 imviz-0.2.5/src/bindings.cpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)    73814 2024-05-24 08:14:59.000000 imviz-0.2.5/src/bindings_imgui.cpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)      146 2023-02-13 10:53:33.000000 imviz-0.2.5/src/bindings_imgui.hpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)    36827 2024-05-24 08:46:08.000000 imviz-0.2.5/src/bindings_implot.cpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)      125 2023-02-13 10:53:33.000000 imviz-0.2.5/src/bindings_implot.hpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     5856 2024-05-02 09:40:07.000000 imviz-0.2.5/src/file_dialog.cpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)      204 2023-09-14 13:48:19.000000 imviz-0.2.5/src/file_dialog.hpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)      159 2024-05-02 10:00:45.000000 imviz-0.2.5/src/im_user_config.h
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)    11091 2024-05-02 09:40:07.000000 imviz-0.2.5/src/implot_ext.cpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)      229 2024-05-02 09:40:07.000000 imviz-0.2.5/src/implot_ext.hpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)    10847 2024-05-02 10:00:45.000000 imviz-0.2.5/src/imviz.cpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     1116 2024-05-02 10:00:45.000000 imviz-0.2.5/src/imviz.hpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)    17988 2023-02-13 10:53:33.000000 imviz-0.2.5/src/input.cpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     1464 2023-02-13 10:53:33.000000 imviz-0.2.5/src/input.hpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)   558672 2023-02-13 10:53:33.000000 imviz-0.2.5/src/source_sans_pro.cpp
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)       95 2023-02-13 10:53:33.000000 imviz-0.2.5/src/source_sans_pro.hpp
```

### Comparing `imviz-0.2.4/CMakeLists.txt` & `imviz-0.2.5/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,24 +29,24 @@
 set(BUILD_STATIC_LIBS OFF CACHE BOOL "" FORCE)
 
 include(FetchContent)
 
 FetchContent_Declare(
     imgui
     GIT_REPOSITORY "https://github.com/ocornut/imgui"
-    GIT_TAG "c6aa051629753f0ef0d26bf775a8b6a92aa213b2"
+    GIT_TAG "v1.90.6-docking"
 )
 
 message(STATUS "Loading imgui ...")
 FetchContent_MakeAvailable(imgui)
 
 FetchContent_Declare(
     implot
     GIT_REPOSITORY "https://github.com/epezent/implot"
-    GIT_TAG "f156599faefe316f7dd20fe6c783bf87c8bb6fd9"
+    GIT_TAG "v0.16"
 )
 
 message(STATUS "Loading implot ...")
 FetchContent_MakeAvailable(implot)
 
 FetchContent_Declare(
     pybind
```

### Comparing `imviz-0.2.4/LICENSE` & `imviz-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `imviz-0.2.4/PKG-INFO` & `imviz-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imviz
-Version: 0.2.4
+Version: 0.2.5
 Summary: Pythonic bindings for imgui/implot
 Home-page: https://github.com/joruof/imviz
 Author: Jona Ruof
 Author-email: jona.ruof@uni-ulm.de
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `imviz-0.2.4/README.md` & `imviz-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `imviz-0.2.4/imviz/__init__.py` & `imviz-0.2.5/imviz/__init__.py`

 * *Files identical despite different names*

### Comparing `imviz-0.2.4/imviz/autogui.py` & `imviz-0.2.5/imviz/autogui.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     return AutoguiContext(params=params).render(obj, name)
 
 
 def list_item_context(obj, name, ctx):
 
     i = ctx.path[-1]
 
-    if viz.begin_popup_context_item():
+    if viz.get_item_id() > 0 and viz.begin_popup_context_item():
         if hasattr(ctx.parents[-1], "insert"):
             if viz.menu_item("Duplicate"):
                 ctx.duplicate_item = i
         if hasattr(ctx.parents[-1], "__delitem__"):
             if viz.menu_item("Remove"):
                 ctx.remove_item = i
                 viz.set_mod(True)
```

### Comparing `imviz-0.2.4/imviz/common.py` & `imviz-0.2.5/imviz/common.py`

 * *Files identical despite different names*

### Comparing `imviz-0.2.4/imviz/dev.py` & `imviz-0.2.5/imviz/dev.py`

 * *Files identical despite different names*

### Comparing `imviz-0.2.4/imviz/dev_main.py` & `imviz-0.2.5/imviz/dev_main.py`

 * *Files identical despite different names*

### Comparing `imviz-0.2.4/imviz/export.py` & `imviz-0.2.5/imviz/export.py`

 * *Files identical despite different names*

### Comparing `imviz-0.2.4/imviz/task.py` & `imviz-0.2.5/imviz/task.py`

 * *Files identical despite different names*

### Comparing `imviz-0.2.4/imviz.egg-info/PKG-INFO` & `imviz-0.2.5/imviz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imviz
-Version: 0.2.4
+Version: 0.2.5
 Summary: Pythonic bindings for imgui/implot
 Home-page: https://github.com/joruof/imviz
 Author: Jona Ruof
 Author-email: jona.ruof@uni-ulm.de
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `imviz-0.2.4/imviz.egg-info/SOURCES.txt` & `imviz-0.2.5/imviz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imviz-0.2.4/setup.py` & `imviz-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
             for m in matches:
                 binary_files.append(m)
                 if not is_wheel:
                     self.copy_file(m, dest_dir / m.name) # tmp => lib
 
 
 setup(name="imviz",
-      version="0.2.4",
+      version="0.2.5",
       description="Pythonic bindings for imgui/implot",
       url="https://github.com/joruof/imviz",
       author="Jona Ruof",
       author_email="jona.ruof@uni-ulm.de",
       license="MIT",
       zip_safe=False,
       long_description=Path('README.md').read_text('utf-8'),
```

### Comparing `imviz-0.2.4/src/binding_helpers.cpp` & `imviz-0.2.5/src/binding_helpers.cpp`

 * *Files identical despite different names*

### Comparing `imviz-0.2.4/src/binding_helpers.hpp` & `imviz-0.2.5/src/binding_helpers.hpp`

 * *Files identical despite different names*

### Comparing `imviz-0.2.4/src/bindings.cpp` & `imviz-0.2.5/src/bindings.cpp`

 * *Files identical despite different names*

### Comparing `imviz-0.2.4/src/bindings_imgui.cpp` & `imviz-0.2.5/src/bindings_imgui.cpp`

 * *Files identical despite different names*

### Comparing `imviz-0.2.4/src/bindings_implot.cpp` & `imviz-0.2.5/src/bindings_implot.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -880,14 +880,17 @@
     py::arg("label") = "",
     py::arg("color") = py::array(),
     py::arg("segments") = 36,
     py::arg("line_weight") = 1.0f,
     py::arg("flags") = ImPlotLineFlags_None);
 
     m.def("is_plot_selected", ImPlot::IsPlotSelected);
+    m.def("is_plot_hovered", ImPlot::IsPlotHovered);
+    m.def("is_subplots_hovered", ImPlot::IsSubplotsHovered);
+    m.def("is_axis_hovered", ImPlot::IsAxisHovered);
 
     m.def("is_plot_item_hidden", [&](std::string& label_id) {
         ImPlotContext& gp = *GImPlot;
         ImPlotItem* item = NULL;
         if (label_id == "") {
            item = gp.CurrentItem;
         } else {
```

### Comparing `imviz-0.2.4/src/file_dialog.cpp` & `imviz-0.2.5/src/file_dialog.cpp`

 * *Files identical despite different names*

### Comparing `imviz-0.2.4/src/implot_ext.cpp` & `imviz-0.2.5/src/implot_ext.cpp`

 * *Files identical despite different names*

### Comparing `imviz-0.2.4/src/imviz.cpp` & `imviz-0.2.5/src/imviz.cpp`

 * *Files identical despite different names*

### Comparing `imviz-0.2.4/src/imviz.hpp` & `imviz-0.2.5/src/imviz.hpp`

 * *Files identical despite different names*

### Comparing `imviz-0.2.4/src/input.cpp` & `imviz-0.2.5/src/input.cpp`

 * *Files identical despite different names*

### Comparing `imviz-0.2.4/src/input.hpp` & `imviz-0.2.5/src/input.hpp`

 * *Files identical despite different names*

### Comparing `imviz-0.2.4/src/source_sans_pro.cpp` & `imviz-0.2.5/src/source_sans_pro.cpp`

 * *Files identical despite different names*


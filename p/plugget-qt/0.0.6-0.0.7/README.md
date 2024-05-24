# Comparing `tmp/plugget_qt-0.0.6.tar.gz` & `tmp/plugget_qt-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugget_qt-0.0.6.tar", last modified: Sun Apr 28 10:10:46 2024, max compression
+gzip compressed data, was "plugget_qt-0.0.7.tar", last modified: Fri May 24 17:50:58 2024, max compression
```

## Comparing `plugget_qt-0.0.6.tar` & `plugget_qt-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:10:46.694345 plugget_qt-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:10:46.690345 plugget_qt-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:10:46.690345 plugget_qt-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-28 10:10:42.000000 plugget_qt-0.0.6/.github/workflows/PyPI-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-28 10:10:42.000000 plugget_qt-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-28 10:10:42.000000 plugget_qt-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-28 10:10:46.694345 plugget_qt-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-28 10:10:42.000000 plugget_qt-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:10:46.690345 plugget_qt-0.0.6/plugget_qt/
--rw-r--r--   0 runner    (1001) docker     (127)    10847 2024-04-28 10:10:42.000000 plugget_qt-0.0.6/plugget_qt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 10:10:46.694345 plugget_qt-0.0.6/plugget_qt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-28 10:10:46.000000 plugget_qt-0.0.6/plugget_qt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-28 10:10:46.000000 plugget_qt-0.0.6/plugget_qt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 10:10:46.000000 plugget_qt-0.0.6/plugget_qt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-28 10:10:46.000000 plugget_qt-0.0.6/plugget_qt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-28 10:10:46.000000 plugget_qt-0.0.6/plugget_qt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-28 10:10:42.000000 plugget_qt-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-28 10:10:42.000000 plugget_qt-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-28 10:10:42.000000 plugget_qt-0.0.6/sample_config.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 10:10:46.694345 plugget_qt-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:50:58.865745 plugget_qt-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:50:58.865745 plugget_qt-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:50:58.865745 plugget_qt-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-24 17:50:54.000000 plugget_qt-0.0.7/.github/workflows/PyPI-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-24 17:50:54.000000 plugget_qt-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-24 17:50:54.000000 plugget_qt-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-24 17:50:58.865745 plugget_qt-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-24 17:50:54.000000 plugget_qt-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:50:58.865745 plugget_qt-0.0.7/plugget_qt/
+-rw-r--r--   0 runner    (1001) docker     (127)    12570 2024-05-24 17:50:54.000000 plugget_qt-0.0.7/plugget_qt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 17:50:58.865745 plugget_qt-0.0.7/plugget_qt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-24 17:50:58.000000 plugget_qt-0.0.7/plugget_qt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-24 17:50:58.000000 plugget_qt-0.0.7/plugget_qt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 17:50:58.000000 plugget_qt-0.0.7/plugget_qt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-24 17:50:58.000000 plugget_qt-0.0.7/plugget_qt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-24 17:50:58.000000 plugget_qt-0.0.7/plugget_qt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-24 17:50:54.000000 plugget_qt-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-24 17:50:54.000000 plugget_qt-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-24 17:50:54.000000 plugget_qt-0.0.7/sample_config.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 17:50:58.865745 plugget_qt-0.0.7/setup.cfg
```

### Comparing `plugget_qt-0.0.6/.github/workflows/PyPI-publish.yml` & `plugget_qt-0.0.7/.github/workflows/PyPI-publish.yml`

 * *Files identical despite different names*

### Comparing `plugget_qt-0.0.6/.gitignore` & `plugget_qt-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `plugget_qt-0.0.6/LICENSE` & `plugget_qt-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `plugget_qt-0.0.6/PKG-INFO` & `plugget_qt-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugget-qt
-Version: 0.0.6
+Version: 0.0.7
 Summary: a qt widget to search for plugget packages
 Author: Hannes Delbeke
 Project-URL: Homepage, https://github.com/plugget/plugget-qt
 Project-URL: Documentation, https://github.com/plugget/plugget-qt
 Keywords: dcc,pipeline,qt,widget,plugget,package,manifest,search,installer
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.11
@@ -16,17 +16,17 @@
 
 # Plugget Qt [![PyPI](https://img.shields.io/pypi/v/plugget-qt)](https://pypi.org/project/plugget-qt/)
 
 Plugget Qt is a UI for [plugget](https://github.com/plugget/plugget).  
 Easily search, list & (un)install [plugget packages](https://github.com/plugget/plugget-pkgs).  
 
 Plugget qt is used by:  
-<img src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/Blender-Dark.svg" width="32" style="max-width: 100%;"> [Plugget Qt Blender addon](https://github.com/plugget/plugget-qt-addon)  
-<img src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/UnrealEngine.svg" width="32" style="max-width: 100%;"> [Plugget Qt Unreal plugin](https://github.com/hannesdelbeke/plugget-unreal)  
-- [plugget-qt-maya-plugin](https://github.com/plugget/plugget-qt-maya-plugin) A Maya plugin that launches the Plugget Qt UI window
+- <img src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/Blender-Dark.svg" width="20" style="max-width: 100%;"> [Plugget Qt Blender addon](https://github.com/plugget/plugget-qt-addon)  
+- <img src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/UnrealEngine.svg" width="20" style="max-width: 100%;"> [Plugget Qt Unreal plugin](https://github.com/hannesdelbeke/plugget-unreal)  
+- [plugget-qt-maya-plugin](https://github.com/plugget/plugget-qt-maya-plugin)
 - [plugget qt substance painter](https://github.com/plugget/plugget-substance-painter-plugin)
 
 
 ## Instructions
 To show the qt window:
 ```python
 import plugget_qt
```

### Comparing `plugget_qt-0.0.6/README.md` & `plugget_qt-0.0.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Plugget Qt [![PyPI](https://img.shields.io/pypi/v/plugget-qt)](https://pypi.org/project/plugget-qt/)
 
 Plugget Qt is a UI for [plugget](https://github.com/plugget/plugget).  
 Easily search, list & (un)install [plugget packages](https://github.com/plugget/plugget-pkgs).  
 
 Plugget qt is used by:  
-<img src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/Blender-Dark.svg" width="32" style="max-width: 100%;"> [Plugget Qt Blender addon](https://github.com/plugget/plugget-qt-addon)  
-<img src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/UnrealEngine.svg" width="32" style="max-width: 100%;"> [Plugget Qt Unreal plugin](https://github.com/hannesdelbeke/plugget-unreal)  
-- [plugget-qt-maya-plugin](https://github.com/plugget/plugget-qt-maya-plugin) A Maya plugin that launches the Plugget Qt UI window
+- <img src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/Blender-Dark.svg" width="20" style="max-width: 100%;"> [Plugget Qt Blender addon](https://github.com/plugget/plugget-qt-addon)  
+- <img src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/UnrealEngine.svg" width="20" style="max-width: 100%;"> [Plugget Qt Unreal plugin](https://github.com/hannesdelbeke/plugget-unreal)  
+- [plugget-qt-maya-plugin](https://github.com/plugget/plugget-qt-maya-plugin)
 - [plugget qt substance painter](https://github.com/plugget/plugget-substance-painter-plugin)
 
 
 ## Instructions
 To show the qt window:
 ```python
 import plugget_qt
```

### Comparing `plugget_qt-0.0.6/plugget_qt/__init__.py` & `plugget_qt-0.0.7/plugget_qt/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # local hack for IDE
 import sys
-# sys.path.append("C:\\Users\\hanne\\OneDrive\\Documents\\repos\\plugget")
-# sys.path.append("C:\\Users\\hanne\\OneDrive\\Documents\\repos\\detect-app")
+sys.path.append("D:\\repos\\plugget")
+sys.path.append("D:\\repos\\detect-app")
 
 try:
     from contextlib import suppress
     QtWidgets = None
     with suppress(ImportError):
         import PySide6.QtWidgets as QtWidgets
+        import PySide6.QtCore as QtCore
     with suppress(ImportError):
         import PyQt6.QtWidgets as QtWidgets
+        import PyQt6.QtCore as QtCore
 except:
     try:
         import PyQt5.QtWidgets as QtWidgets
+        import PyQt5.QtCore as QtCore
     except ImportError:
         pass
     try:
         import PySide2.QtWidgets as QtWidgets
+        import PySide2.QtCore as QtCore
     except ImportError:
         import qtpy.QtWidgets as QtWidgets
+        import qtpy.QtCore as QtCore
 
 import plugget.commands as cmd
 import logging
 
 INSTALLED = "Installed"
 INSTALL = "Install"
 NOT_INSTALLED = "Not installed"
@@ -118,14 +123,17 @@
         # layout.addWidget(self.package_list)
         # self.setLayout(layout)
 
         # self.list_packages()
         # set tab to list
         self.tab_widget.setCurrentIndex(1)
 
+        self.package_list.setContextMenuPolicy(QtCore.Qt.CustomContextMenu)
+        self.package_list.customContextMenuRequested.connect(self.context_menu)
+
     def tab_logic(self):
         # if tab is select, run self.list_packages
 
         # clear package list
         self.package_list.clearContents()
         self.package_list.setRowCount(0)
 
@@ -189,14 +197,51 @@
             version_dropdown.setCurrentText(package_meta.latest.version)
 
             # install button
             install_button = QtWidgets.QPushButton(INSTALL)
             install_button.clicked.connect(lambda _=None, r=row: self.install_package(r))
             self.package_list.setCellWidget(row, INDEX_INSTALL, install_button)
 
+            # add actions context menu to right click on package name
+            # each package has package.actions, which is a list of dicts.
+            # the format is {"label": "a label", "command": "python string command"}
+            # todo instead of context menu on every single item
+            #  use context menu on the whole table, and get the row from the click position
+            self.package_list.setContextMenuPolicy(QtCore.Qt.CustomContextMenu)
+    def context_menu(self, pos):
+        item = self.package_list.itemAt(pos)
+        if item is None:
+            return
+
+        row = item.row()
+        package_meta = self.current_packages[row]
+        actions = package_meta.actions
+
+        menu = QtWidgets.QMenu()
+
+        if not actions:
+            actions = [{"label": "No actions available", "command": "print('no commands')"}]
+
+        for action in actions:
+            label = action["label"]
+            command = action["command"]
+            action_item = menu.addAction(label)
+
+            def execute_command(cmd=command):
+                if isinstance(cmd, str):
+                    exec(cmd)
+                elif callable(cmd):
+                    cmd()
+                else:
+                    raise ValueError(f"Unsupported command type: {type(cmd)}")
+
+            action_item.triggered.connect(lambda _, cmd=command: execute_command(cmd))
+
+        menu.exec_(self.package_list.viewport().mapToGlobal(pos))
+
     @try_except
     def install_package(self, row):
         package_meta = self.current_packages[row]
         version = self.package_list.cellWidget(row, INDEX_VERSIONS).currentText()
         cmd.install(package_meta.package_name, version=version)
         self.list_packages()
```

### Comparing `plugget_qt-0.0.6/plugget_qt.egg-info/PKG-INFO` & `plugget_qt-0.0.7/plugget_qt.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugget-qt
-Version: 0.0.6
+Version: 0.0.7
 Summary: a qt widget to search for plugget packages
 Author: Hannes Delbeke
 Project-URL: Homepage, https://github.com/plugget/plugget-qt
 Project-URL: Documentation, https://github.com/plugget/plugget-qt
 Keywords: dcc,pipeline,qt,widget,plugget,package,manifest,search,installer
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.11
@@ -16,17 +16,17 @@
 
 # Plugget Qt [![PyPI](https://img.shields.io/pypi/v/plugget-qt)](https://pypi.org/project/plugget-qt/)
 
 Plugget Qt is a UI for [plugget](https://github.com/plugget/plugget).  
 Easily search, list & (un)install [plugget packages](https://github.com/plugget/plugget-pkgs).  
 
 Plugget qt is used by:  
-<img src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/Blender-Dark.svg" width="32" style="max-width: 100%;"> [Plugget Qt Blender addon](https://github.com/plugget/plugget-qt-addon)  
-<img src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/UnrealEngine.svg" width="32" style="max-width: 100%;"> [Plugget Qt Unreal plugin](https://github.com/hannesdelbeke/plugget-unreal)  
-- [plugget-qt-maya-plugin](https://github.com/plugget/plugget-qt-maya-plugin) A Maya plugin that launches the Plugget Qt UI window
+- <img src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/Blender-Dark.svg" width="20" style="max-width: 100%;"> [Plugget Qt Blender addon](https://github.com/plugget/plugget-qt-addon)  
+- <img src="https://raw.githubusercontent.com/tandpfun/skill-icons/59059d9d1a2c092696dc66e00931cc1181a4ce1f/icons/UnrealEngine.svg" width="20" style="max-width: 100%;"> [Plugget Qt Unreal plugin](https://github.com/hannesdelbeke/plugget-unreal)  
+- [plugget-qt-maya-plugin](https://github.com/plugget/plugget-qt-maya-plugin)
 - [plugget qt substance painter](https://github.com/plugget/plugget-substance-painter-plugin)
 
 
 ## Instructions
 To show the qt window:
 ```python
 import plugget_qt
```

### Comparing `plugget_qt-0.0.6/pyproject.toml` & `plugget_qt-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ]
 dependencies = [
     'importlib-metadata; python_version<"3.4"',
     'plugget',
 ]
 
 # dynamic = ["version"]
-version = "0.0.6"
+version = "0.0.7"
 
 # [project.optional-dependencies]
 # pyside2 = ["PySide2"]
 
 #[project.scripts]
 #my-script = "my_package.module:function"
```


# Comparing `tmp/datadash-0.0.2.tar.gz` & `tmp/datadash-0.0.3.tar.gz`

## Comparing `datadash-0.0.2.tar` & `datadash-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,14 @@
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 datadash-0.0.2/src/datadash/__init__.py
--rw-r--r--   0        0        0     8655 2020-02-02 00:00:00.000000 datadash-0.0.2/src/datadash/__main__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 datadash-0.0.2/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 datadash-0.0.2/LICENSE
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 datadash-0.0.2/README.md
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 datadash-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 datadash-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 datadash-0.0.3/mkdocs.yml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 datadash-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 datadash-0.0.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datadash-0.0.3/docs/guides.md
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 datadash-0.0.3/docs/hotkeys.md
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 datadash-0.0.3/docs/index.md
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 datadash-0.0.3/docs/tutorial.md
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 datadash-0.0.3/src/datadash/__init__.py
+-rw-r--r--   0        0        0     8928 2020-02-02 00:00:00.000000 datadash-0.0.3/src/datadash/__main__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 datadash-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 datadash-0.0.3/LICENSE
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 datadash-0.0.3/README.md
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 datadash-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 datadash-0.0.3/PKG-INFO
```

### Comparing `datadash-0.0.2/src/datadash/__main__.py` & `datadash-0.0.3/src/datadash/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-import sys
+"""Datadash main module."""
+
 import os
-import pandas as pd
 import sqlite3
-from PyQt6.QtWidgets import QApplication, QMainWindow, QVBoxLayout, QWidget, QTextEdit, QTextBrowser, QFileDialog, QTabWidget, QPushButton, QFrame
-from PyQt6.QtGui import QAction, QKeySequence
+import sys
+
+import pandas as pd
 from PyQt6.QtCore import Qt
-from tabulate import tabulate
+from PyQt6.QtGui import QAction, QKeySequence
+from PyQt6.QtWidgets import (QApplication, QFileDialog, QFrame, QMainWindow,
+                             QPushButton, QTabWidget, QTextBrowser, QTextEdit,
+                             QVBoxLayout, QWidget)
+
 
 class SQLTextEdit(QTextEdit):
     """Custom QTextEdit widget for SQL input with special handling for Enter and Shift+Enter keys.
 
     Args:
         parent (QWidget, optional): Parent widget. Defaults to None.
         dashboard (Dashboard, optional): Reference to the Dashboard instance. Defaults to None.
@@ -21,40 +26,47 @@
 
     def keyPressEvent(self, event):
         """Handles key press events to execute query on Enter and add new line on Shift+Enter.
 
         Args:
             event (QKeyEvent): The key press event.
         """
-        if event.key() == Qt.Key.Key_Return and not (event.modifiers() & Qt.KeyboardModifier.ShiftModifier):
+        if event.key() == Qt.Key.Key_Return and not (
+            event.modifiers() & Qt.KeyboardModifier.ShiftModifier
+        ):
             self.dashboard.execute_query()
-        elif event.key() == Qt.Key.Key_Return and (event.modifiers() & Qt.KeyboardModifier.ShiftModifier):
-            self.insertPlainText('\n')
+        elif event.key() == Qt.Key.Key_Return and (
+            event.modifiers() & Qt.KeyboardModifier.ShiftModifier
+        ):
+            self.insertPlainText("\n")
         else:
             super().keyPressEvent(event)
 
+
 class Dashboard(QMainWindow):
     """Main application window for the data dashboard."""
 
     def __init__(self):
         super().__init__()
-        self.setWindowTitle('Datadash')
+        self.setWindowTitle("Datadash")
 
         # Create the "New Query" button
         new_query_button = QPushButton("New Query")
         new_query_button.clicked.connect(self.open_file_dialog)
 
         # Add the "New Query" button to a toolbar
         toolbar = self.addToolBar("Toolbar")
         toolbar.addWidget(new_query_button)
 
         # Create a tab widget
         self.tab_widget = QTabWidget()
         self.tab_widget.setTabsClosable(True)  # Enable closing tabs
-        self.tab_widget.tabCloseRequested.connect(self.close_tab)  # Connect to close_tab method
+        self.tab_widget.tabCloseRequested.connect(
+            self.close_tab
+        )  # Connect to close_tab method
 
         # Layout for the main window
         main_layout = QVBoxLayout()
         main_layout.addWidget(self.tab_widget)
 
         central_widget = QWidget()
         central_widget.setLayout(main_layout)
@@ -134,17 +146,21 @@
         # Separator between the query input and output
         separator_line = QFrame()
         separator_line.setFrameShape(QFrame.Shape.HLine)
         separator_line.setFrameShadow(QFrame.Shadow.Sunken)
 
         # Layout for the SQL query tab
         query_layout = QVBoxLayout()
-        query_layout.addWidget(query_entry, 1)  # Add query_entry to layout, stretch factor 1
+        query_layout.addWidget(
+            query_entry, 1
+        )  # Add query_entry to layout, stretch factor 1
         query_layout.addWidget(separator_line)
-        query_layout.addWidget(query_output_view, 2)  # Add query_output_view to layout, stretch factor 2
+        query_layout.addWidget(
+            query_output_view, 2
+        )  # Add query_output_view to layout, stretch factor 2
 
         query_widget = QWidget()
         query_widget.setLayout(query_layout)
 
         # Store the query_entry and query_output_view widgets in the widget itself
         query_widget.query_entry = query_entry
         query_widget.query_output_view = query_output_view
@@ -170,46 +186,50 @@
             result = pd.read_sql_query(query, conn)
 
             # Convert DataFrame to HTML table
             html_table = result.to_html(index=False)
 
             # Display the HTML table in the QTextBrowser widget
             query_output_view.setHtml(html_table)
-        except Exception as e:
-            query_output_view.setPlainText(str(e))
+        except Exception as exceptional_case:
+            query_output_view.setPlainText(str(exception_case))
 
     def open_file_dialog(self):
         """Opens a file dialog to select a CSV file and loads it into a new tab."""
-        file_path, _ = QFileDialog.getOpenFileName(self, "Open CSV File", "", "CSV Files (*.csv)")
+        file_path, _ = QFileDialog.getOpenFileName(
+            self, "Open CSV File", "", "CSV Files (*.csv)"
+        )
         if file_path:
             self.load_csv_tab(file_path)
 
     def load_csv_tab(self, file_path):
         """Loads a CSV file into a new tab.
 
         Args:
             file_path (str): The path to the CSV file.
         """
-        file_name = os.path.basename(file_path)  # Extract the file name from the file path
+        file_name = os.path.basename(
+            file_path
+        )  # Extract the file name from the file path
         new_query_tab = self.create_query_tab(file_name)
         self.tab_widget.addTab(new_query_tab, file_name)
 
         try:
             # Read the CSV file into a pandas DataFrame
             data = pd.read_csv(file_path)
 
             # Create an in-memory SQLite database and load the data into it
-            conn = sqlite3.connect(':memory:')
-            data.to_sql('data', conn, index=False, if_exists='replace')
+            conn = sqlite3.connect(":memory:")
+            data.to_sql("data", conn, index=False, if_exists="replace")
 
             # Store the connection for this tab using tab index as the key
             tab_index = self.tab_widget.indexOf(new_query_tab)
             self.connections[tab_index] = conn
-        except Exception as e:
-            new_query_tab.query_output_view.setPlainText(str(e))
+        except Exception as exception_case:
+            new_query_tab.query_output_view.setPlainText(str(exceptional_case))
 
     def close_tab(self, index):
         """Closes the tab at the specified index.
 
         Args:
             index (int): The index of the tab to close.
         """
@@ -218,12 +238,13 @@
         widget.deleteLater()
 
         # Close the database connection for the tab and remove it from the dictionary
         conn = self.connections.pop(index, None)
         if conn:
             conn.close()
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     app = QApplication(sys.argv)
     dashboard = Dashboard()
     dashboard.show()
     sys.exit(app.exec())
```

### Comparing `datadash-0.0.2/.gitignore` & `datadash-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `datadash-0.0.2/LICENSE` & `datadash-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datadash-0.0.2/pyproject.toml` & `datadash-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "Datadash"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Galen Seilis", email="galen.seilis@seilis.ca" },
 ]
 description = "Taking a quick look at data."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `datadash-0.0.2/PKG-INFO` & `datadash-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: Datadash
-Version: 0.0.2
+Version: 0.0.3
 Summary: Taking a quick look at data.
 Project-URL: Homepage, https://github.com/galenseilis/datadash
 Project-URL: Issues, https://github.com/galenseilis/datadash/issues
 Author-email: Galen Seilis <galen.seilis@seilis.ca>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


# Comparing `tmp/jupyterexport-0.1.5.tar.gz` & `tmp/jupyterexport-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterexport-0.1.5.tar", last modified: Fri May 24 02:17:48 2024, max compression
+gzip compressed data, was "jupyterexport-0.1.6.tar", last modified: Fri May 24 02:55:00 2024, max compression
```

## Comparing `jupyterexport-0.1.5.tar` & `jupyterexport-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-24 02:17:48.758212 jupyterexport-0.1.5/
-drwxrwxrwx   0        0        0        0 2024-05-24 02:17:48.689907 jupyterexport-0.1.5/JupyterExport/
--rw-rw-rw-   0        0        0       21 2024-05-24 00:49:31.000000 jupyterexport-0.1.5/JupyterExport/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-24 02:17:48.758212 jupyterexport-0.1.5/JupyterExport/assets/
--rw-rw-rw-   0        0        0     6243 2024-02-26 19:58:24.000000 jupyterexport-0.1.5/JupyterExport/assets/Anthracite.json
--rw-rw-rw-   0        0        0   106181 2024-02-26 21:22:45.000000 jupyterexport-0.1.5/JupyterExport/assets/icon.ico
--rw-rw-rw-   0        0        0     4967 2024-05-24 02:15:22.000000 jupyterexport-0.1.5/JupyterExport/main.py
-drwxrwxrwx   0        0        0        0 2024-05-24 02:17:48.758212 jupyterexport-0.1.5/JupyterExport.egg-info/
--rw-rw-rw-   0        0        0     1852 2024-05-24 02:17:48.000000 jupyterexport-0.1.5/JupyterExport.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2024-05-24 02:17:48.000000 jupyterexport-0.1.5/JupyterExport.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-24 02:17:48.000000 jupyterexport-0.1.5/JupyterExport.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-05-24 02:17:48.000000 jupyterexport-0.1.5/JupyterExport.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       50 2024-05-24 02:17:48.000000 jupyterexport-0.1.5/JupyterExport.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-24 02:17:48.000000 jupyterexport-0.1.5/JupyterExport.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1852 2024-05-24 02:17:48.758212 jupyterexport-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1401 2024-05-24 01:24:58.000000 jupyterexport-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-24 02:17:48.758212 jupyterexport-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1088 2024-05-24 01:56:19.000000 jupyterexport-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 02:55:00.877768 jupyterexport-0.1.6/
+drwxrwxrwx   0        0        0        0 2024-05-24 02:55:00.815994 jupyterexport-0.1.6/JupyterExport/
+-rw-rw-rw-   0        0        0       21 2024-05-24 00:49:31.000000 jupyterexport-0.1.6/JupyterExport/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-24 02:55:00.871121 jupyterexport-0.1.6/JupyterExport/assets/
+-rw-rw-rw-   0        0        0     6243 2024-02-26 19:58:24.000000 jupyterexport-0.1.6/JupyterExport/assets/Anthracite.json
+-rw-rw-rw-   0        0        0   106181 2024-02-26 21:22:45.000000 jupyterexport-0.1.6/JupyterExport/assets/icon.ico
+-rw-rw-rw-   0        0        0     5062 2024-05-24 02:53:56.000000 jupyterexport-0.1.6/JupyterExport/main.py
+drwxrwxrwx   0        0        0        0 2024-05-24 02:55:00.877768 jupyterexport-0.1.6/JupyterExport.egg-info/
+-rw-rw-rw-   0        0        0     2084 2024-05-24 02:55:00.000000 jupyterexport-0.1.6/JupyterExport.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2024-05-24 02:55:00.000000 jupyterexport-0.1.6/JupyterExport.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 02:55:00.000000 jupyterexport-0.1.6/JupyterExport.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-05-24 02:55:00.000000 jupyterexport-0.1.6/JupyterExport.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       50 2024-05-24 02:55:00.000000 jupyterexport-0.1.6/JupyterExport.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-24 02:55:00.000000 jupyterexport-0.1.6/JupyterExport.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2084 2024-05-24 02:55:00.877768 jupyterexport-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1633 2024-05-24 02:33:16.000000 jupyterexport-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-24 02:55:00.877768 jupyterexport-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1088 2024-05-24 02:54:56.000000 jupyterexport-0.1.6/setup.py
```

### Comparing `jupyterexport-0.1.5/JupyterExport/assets/Anthracite.json` & `jupyterexport-0.1.6/JupyterExport/assets/Anthracite.json`

 * *Files identical despite different names*

### Comparing `jupyterexport-0.1.5/JupyterExport/assets/icon.ico` & `jupyterexport-0.1.6/JupyterExport/assets/icon.ico`

 * *Files identical despite different names*

### Comparing `jupyterexport-0.1.5/JupyterExport/main.py` & `jupyterexport-0.1.6/JupyterExport/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import customtkinter as ctk
 import tkinter as tk
 from tkinter import filedialog, messagebox
 import nbformat
 from nbconvert import PDFExporter, HTMLExporter
 import os
-import sys
+import threading
 import subprocess
 
 
 ASSETS_DIR = os.path.join(os.path.dirname(__file__), 'assets')
 
 # Load an image
 icon_path = os.path.join(ASSETS_DIR, 'icon.ico')
@@ -77,29 +77,34 @@
             self.text_variable.set(file_name)
         else:
             self.text_variable.set("No file selected")
 
     def check_fun(self):
         # Create a new thread for the long-running function
         if self.text_variable.get() != "No file selected":
-            self.convert_ipynb(file, self.output_file_var.get())
+            self.convert_ipynb_threaded(file, self.output_file_var.get())
         else:
             messagebox.showerror("Error", "Please choose a file to convert!")
 
     def open_file_in_browser(self, file_path):
         """
         Open the file in the default file browser.
         """
         if os.name == 'nt':  # Windows
             os.startfile(file_path)
         elif os.name == 'posix':  # macOS or Linux
             subprocess.Popen(['xdg-open', file_path])
         else:
             raise NotImplementedError("Unsupported operating system")
 
+    def convert_ipynb_threaded(self, ipynb_file, output):
+        # Start a new thread to run the conversion function
+        t = threading.Thread(target=self.convert_ipynb, args=(ipynb_file, output))
+        t.start()
+
     def convert_ipynb(self, ipynb_file, output):
         app.configure(cursor='wait')
         self.convert_btn.configure(state='disabled')
 
         if self.convert_to.get() == 'PDF':
             # Read the IPython Notebook
             with open(ipynb_file, 'r', encoding='utf-8') as f:
@@ -132,13 +137,11 @@
         self.convert_btn.configure(state='normal')
         app.configure(cursor="")
         messagebox.showinfo("Success", "Operation completed successfully!")
 
         # Get the directory where the script is located
         script_dir = os.path.dirname(os.path.realpath(__file__))
 
-        # Open file dialog with initial directory set to script directory
-        file_path = filedialog.askopenfilename(initialdir=script_dir)
-        self.open_file_in_browser(file_path)
+        self.open_file_in_browser(script_dir)
 
 app = App()
 app.mainloop()
```

### Comparing `jupyterexport-0.1.5/JupyterExport.egg-info/PKG-INFO` & `jupyterexport-0.1.6/JupyterExport.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: JupyterExport
-Version: 0.1.5
+Version: 0.1.6
 Summary: Convert .ipynb files to .pdf/.html using a simple graphical interface.
 Home-page: https://github.com/Alan-Analyst/JupyterExport
 Author: Alan
 Author-email: alananalyst00@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: customtkinter
 Requires-Dist: nbformat
 Requires-Dist: nbconvert
 Requires-Dist: IPython
 Requires-Dist: Pygments
 
+<span style="color:red">**Warning:** This project is still in development and may have bugs. I highly recommend creating a virtual environment to install this package instead of installing it in the global environment. </span>
+
+
 # JupyterExport
 
 JupyterExport is a simple GUI application built in Python using Tkinter that allows you to effortlessly convert Jupyter Notebook files to HTML and PDF formats. This tool aims to streamline the process of sharing and distributing Jupyter notebooks by providing a user-friendly interface for exporting them into more accessible formats.
 
 ## Features
 
 - **Easy Conversion**: Convert Jupyter Notebook files (.ipynb) to HTML or PDF format with just a few clicks.
```

### Comparing `jupyterexport-0.1.5/PKG-INFO` & `jupyterexport-0.1.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: JupyterExport
-Version: 0.1.5
+Version: 0.1.6
 Summary: Convert .ipynb files to .pdf/.html using a simple graphical interface.
 Home-page: https://github.com/Alan-Analyst/JupyterExport
 Author: Alan
 Author-email: alananalyst00@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: customtkinter
 Requires-Dist: nbformat
 Requires-Dist: nbconvert
 Requires-Dist: IPython
 Requires-Dist: Pygments
 
+<span style="color:red">**Warning:** This project is still in development and may have bugs. I highly recommend creating a virtual environment to install this package instead of installing it in the global environment. </span>
+
+
 # JupyterExport
 
 JupyterExport is a simple GUI application built in Python using Tkinter that allows you to effortlessly convert Jupyter Notebook files to HTML and PDF formats. This tool aims to streamline the process of sharing and distributing Jupyter notebooks by providing a user-friendly interface for exporting them into more accessible formats.
 
 ## Features
 
 - **Easy Conversion**: Convert Jupyter Notebook files (.ipynb) to HTML or PDF format with just a few clicks.
```

### Comparing `jupyterexport-0.1.5/README.md` & `jupyterexport-0.1.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+<span style="color:red">**Warning:** This project is still in development and may have bugs. I highly recommend creating a virtual environment to install this package instead of installing it in the global environment. </span>
+
+
 # JupyterExport
 
 JupyterExport is a simple GUI application built in Python using Tkinter that allows you to effortlessly convert Jupyter Notebook files to HTML and PDF formats. This tool aims to streamline the process of sharing and distributing Jupyter notebooks by providing a user-friendly interface for exporting them into more accessible formats.
 
 ## Features
 
 - **Easy Conversion**: Convert Jupyter Notebook files (.ipynb) to HTML or PDF format with just a few clicks.
```

### Comparing `jupyterexport-0.1.5/setup.py` & `jupyterexport-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 from JupyterExport import __version__ as version
 
 setup(
     name="JupyterExport",
-    version="0.1.5",
+    version="0.1.6",
     author="Alan",
     author_email="alananalyst00@gmail.com",
     url='https://github.com/Alan-Analyst/JupyterExport',
     description="Convert .ipynb files to .pdf/.html using a simple graphical interface.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```


# Comparing `tmp/md2weasypdf-0.0.8.tar.gz` & `tmp/md2weasypdf-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md2weasypdf-0.0.8.tar", last modified: Thu Apr 25 13:40:05 2024, max compression
+gzip compressed data, was "md2weasypdf-0.0.9.tar", last modified: Fri Apr 26 09:41:04 2024, max compression
```

## Comparing `md2weasypdf-0.0.8.tar` & `md2weasypdf-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:40:05.392287 md2weasypdf-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    26501 2024-04-25 13:40:01.000000 md2weasypdf-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-25 13:40:05.392287 md2weasypdf-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-25 13:40:01.000000 md2weasypdf-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:40:05.388287 md2weasypdf-0.0.8/md2weasypdf/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-25 13:40:01.000000 md2weasypdf-0.0.8/md2weasypdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-25 13:40:01.000000 md2weasypdf-0.0.8/md2weasypdf/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:40:05.392287 md2weasypdf-0.0.8/md2weasypdf/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-25 13:40:01.000000 md2weasypdf-0.0.8/md2weasypdf/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-25 13:40:01.000000 md2weasypdf-0.0.8/md2weasypdf/extensions/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-25 13:40:01.000000 md2weasypdf-0.0.8/md2weasypdf/extensions/footnotes.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-25 13:40:01.000000 md2weasypdf-0.0.8/md2weasypdf/extensions/subscript.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-25 13:40:01.000000 md2weasypdf-0.0.8/md2weasypdf/extensions/textbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-25 13:40:01.000000 md2weasypdf-0.0.8/md2weasypdf/extensions/toa.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-25 13:40:01.000000 md2weasypdf-0.0.8/md2weasypdf/extensions/toc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-04-25 13:40:01.000000 md2weasypdf-0.0.8/md2weasypdf/printer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 13:40:05.392287 md2weasypdf-0.0.8/md2weasypdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-25 13:40:05.000000 md2weasypdf-0.0.8/md2weasypdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-25 13:40:05.000000 md2weasypdf-0.0.8/md2weasypdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 13:40:05.000000 md2weasypdf-0.0.8/md2weasypdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 13:40:05.000000 md2weasypdf-0.0.8/md2weasypdf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 13:40:05.000000 md2weasypdf-0.0.8/md2weasypdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 13:40:05.000000 md2weasypdf-0.0.8/md2weasypdf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-25 13:40:01.000000 md2weasypdf-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-25 13:40:05.392287 md2weasypdf-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 13:40:01.000000 md2weasypdf-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:41:04.435312 md2weasypdf-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    26501 2024-04-26 09:41:00.000000 md2weasypdf-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-04-26 09:41:04.435312 md2weasypdf-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-26 09:41:00.000000 md2weasypdf-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:41:04.435312 md2weasypdf-0.0.9/md2weasypdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-26 09:41:00.000000 md2weasypdf-0.0.9/md2weasypdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-26 09:41:00.000000 md2weasypdf-0.0.9/md2weasypdf/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:41:04.435312 md2weasypdf-0.0.9/md2weasypdf/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-26 09:41:00.000000 md2weasypdf-0.0.9/md2weasypdf/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-26 09:41:00.000000 md2weasypdf-0.0.9/md2weasypdf/extensions/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-26 09:41:00.000000 md2weasypdf-0.0.9/md2weasypdf/extensions/footnotes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-26 09:41:00.000000 md2weasypdf-0.0.9/md2weasypdf/extensions/subscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-26 09:41:00.000000 md2weasypdf-0.0.9/md2weasypdf/extensions/textbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-26 09:41:00.000000 md2weasypdf-0.0.9/md2weasypdf/extensions/toa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-26 09:41:00.000000 md2weasypdf-0.0.9/md2weasypdf/extensions/toc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-04-26 09:41:00.000000 md2weasypdf-0.0.9/md2weasypdf/printer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 09:41:04.435312 md2weasypdf-0.0.9/md2weasypdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-04-26 09:41:04.000000 md2weasypdf-0.0.9/md2weasypdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-26 09:41:04.000000 md2weasypdf-0.0.9/md2weasypdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 09:41:04.000000 md2weasypdf-0.0.9/md2weasypdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 09:41:04.000000 md2weasypdf-0.0.9/md2weasypdf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-26 09:41:04.000000 md2weasypdf-0.0.9/md2weasypdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 09:41:04.000000 md2weasypdf-0.0.9/md2weasypdf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-26 09:41:00.000000 md2weasypdf-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-26 09:41:04.439313 md2weasypdf-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 09:41:00.000000 md2weasypdf-0.0.9/setup.py
```

### Comparing `md2weasypdf-0.0.8/LICENSE` & `md2weasypdf-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.8/PKG-INFO` & `md2weasypdf-0.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2weasypdf
-Version: 0.0.8
+Version: 0.0.9
 Summary: Print PDFs from Markdown Files using Weasyprint
 Home-page: https://github.com/mstingl/md2weasypdf
 Author: Manuel Stingl
 Author-email: contact@stingl.st
 License: GNU LGPLv2.1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
@@ -19,38 +19,44 @@
 Requires-Dist: jinja2
 Requires-Dist: watchdog
 Requires-Dist: markdown-grid-tables
 Requires-Dist: python-frontmatter
 
 # md2weasypdf
 
-Print PDFs from Markdown Files using Weasyprint
+Print PDFs from Markdown Files and a HTML template/layout using Weasyprint.
 
 ## Installation
 
 ```shell
 pip install md2weasypdf
 ```
 
 ## Usage
 
 ```shell
 python -m md2weasypdf <input_folder_or_file> <output_path>
 ```
 
+When a layout is not specified in the files frontmatter (see below), the `--layout` option has to be passed.
+
 ### Watch Mode
 
 The watch mode is intended for creation of layouts. The given layouts directory and input directory will be watched for changes.
 
 For VSCode the extension [vscode-pdf](https://marketplace.visualstudio.com/items?itemName=tomoki1207.pdf) can be recommended, as it refreshes the displayed PDF automatically.
 
 ```shell
 python -m md2weasypdf <input_folder_or_file> <output_path> --watch
 ```
 
+## Layout
+
+The document layout must be given via the command option `--layout` or in the frontmatter of the single file. As layout a directory name inside the `./layouts` directory (default, can be changed using `--layouts-dir`) is expected. In the layout directory, a `index.html.j2` or `index.html` file is expected, which is loaded as entrypoint. The file is parsed using Jinja2.
+
 ## Input
 
 Input files are expected in markdown format with several markdown extensions. The markdown documents can utilize Jinja2 for templating inside the document (e. g. reusing texts).
 
 ### Bundling
 
 The bundling feature allows to bundle multiple documents into one PDF. This is useful when you want to create one PDF file from multiple source files. The bundling feature is enabled by adding the `--bundle` flag to the command. The specified input folder will be searched recursively for `*.md` files, files starting with an underscore will be ignored.
@@ -103,12 +109,12 @@
 
 Use tildes `~` around text to create a subscript formatting.
 
 ### Checkboxes
 
 Use `[ ]` to create a checkbox. Use `[x]` to mark a checkbox as checked.
 
-### Input Fields
+### Fields
 
 Use `[>input_id]` to create a text input. To create a textarea, add `|textarea` after the input id. To create a date field, add `|YYYY-MM-DD` after the input id.
 
 To add a placeholder, append the placeholder text within parens to the end of the input id: `[>input_id] (placeholder text)`.
```

### Comparing `md2weasypdf-0.0.8/README.md` & `md2weasypdf-0.0.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 # md2weasypdf
 
-Print PDFs from Markdown Files using Weasyprint
+Print PDFs from Markdown Files and a HTML template/layout using Weasyprint.
 
 ## Installation
 
 ```shell
 pip install md2weasypdf
 ```
 
 ## Usage
 
 ```shell
 python -m md2weasypdf <input_folder_or_file> <output_path>
 ```
 
+When a layout is not specified in the files frontmatter (see below), the `--layout` option has to be passed.
+
 ### Watch Mode
 
 The watch mode is intended for creation of layouts. The given layouts directory and input directory will be watched for changes.
 
 For VSCode the extension [vscode-pdf](https://marketplace.visualstudio.com/items?itemName=tomoki1207.pdf) can be recommended, as it refreshes the displayed PDF automatically.
 
 ```shell
 python -m md2weasypdf <input_folder_or_file> <output_path> --watch
 ```
 
+## Layout
+
+The document layout must be given via the command option `--layout` or in the frontmatter of the single file. As layout a directory name inside the `./layouts` directory (default, can be changed using `--layouts-dir`) is expected. In the layout directory, a `index.html.j2` or `index.html` file is expected, which is loaded as entrypoint. The file is parsed using Jinja2.
+
 ## Input
 
 Input files are expected in markdown format with several markdown extensions. The markdown documents can utilize Jinja2 for templating inside the document (e. g. reusing texts).
 
 ### Bundling
 
 The bundling feature allows to bundle multiple documents into one PDF. This is useful when you want to create one PDF file from multiple source files. The bundling feature is enabled by adding the `--bundle` flag to the command. The specified input folder will be searched recursively for `*.md` files, files starting with an underscore will be ignored.
@@ -80,12 +86,12 @@
 
 Use tildes `~` around text to create a subscript formatting.
 
 ### Checkboxes
 
 Use `[ ]` to create a checkbox. Use `[x]` to mark a checkbox as checked.
 
-### Input Fields
+### Fields
 
 Use `[>input_id]` to create a text input. To create a textarea, add `|textarea` after the input id. To create a date field, add `|YYYY-MM-DD` after the input id.
 
 To add a placeholder, append the placeholder text within parens to the end of the input id: `[>input_id] (placeholder text)`.
```

### Comparing `md2weasypdf-0.0.8/md2weasypdf/__main__.py` & `md2weasypdf-0.0.9/md2weasypdf/__main__.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.8/md2weasypdf/extensions/checkbox.py` & `md2weasypdf-0.0.9/md2weasypdf/extensions/checkbox.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.8/md2weasypdf/extensions/footnotes.py` & `md2weasypdf-0.0.9/md2weasypdf/extensions/footnotes.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.8/md2weasypdf/extensions/textbox.py` & `md2weasypdf-0.0.9/md2weasypdf/extensions/textbox.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.8/md2weasypdf/extensions/toa.py` & `md2weasypdf-0.0.9/md2weasypdf/extensions/toa.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.8/md2weasypdf/extensions/toc.py` & `md2weasypdf-0.0.9/md2weasypdf/extensions/toc.py`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.8/md2weasypdf/printer.py` & `md2weasypdf-0.0.9/md2weasypdf/printer.py`

 * *Files 3% similar despite different names*

```diff
@@ -208,14 +208,22 @@
             raise ValueError("No layout defined")
 
         if os.path.isdir(layout_dir := self.layouts_dir / layout):
             return layout_dir
 
         raise ValueError("Layout \"{layout}\" could not be found")
 
+    @staticmethod
+    def try_files(path: Path, filenames: List[str]):
+        for filename in filenames:
+            if (filepath := path / filename).exists():
+                return filepath
+
+        raise FileNotFoundError
+
     @cache
     def _load_template(self, layout):
         layout_dir = self._get_layout_dir(layout)
-        with open(layout_dir / "index.html", mode="rb") as file:
+        with self.try_files(layout_dir, ["index.html.j2", "index.html"]).open(mode="rb") as file:
             template = self.jinja_env.from_string(str(file.read(), "utf-8"))
 
         return template, layout_dir
```

### Comparing `md2weasypdf-0.0.8/md2weasypdf.egg-info/PKG-INFO` & `md2weasypdf-0.0.9/md2weasypdf.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2weasypdf
-Version: 0.0.8
+Version: 0.0.9
 Summary: Print PDFs from Markdown Files using Weasyprint
 Home-page: https://github.com/mstingl/md2weasypdf
 Author: Manuel Stingl
 Author-email: contact@stingl.st
 License: GNU LGPLv2.1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
@@ -19,38 +19,44 @@
 Requires-Dist: jinja2
 Requires-Dist: watchdog
 Requires-Dist: markdown-grid-tables
 Requires-Dist: python-frontmatter
 
 # md2weasypdf
 
-Print PDFs from Markdown Files using Weasyprint
+Print PDFs from Markdown Files and a HTML template/layout using Weasyprint.
 
 ## Installation
 
 ```shell
 pip install md2weasypdf
 ```
 
 ## Usage
 
 ```shell
 python -m md2weasypdf <input_folder_or_file> <output_path>
 ```
 
+When a layout is not specified in the files frontmatter (see below), the `--layout` option has to be passed.
+
 ### Watch Mode
 
 The watch mode is intended for creation of layouts. The given layouts directory and input directory will be watched for changes.
 
 For VSCode the extension [vscode-pdf](https://marketplace.visualstudio.com/items?itemName=tomoki1207.pdf) can be recommended, as it refreshes the displayed PDF automatically.
 
 ```shell
 python -m md2weasypdf <input_folder_or_file> <output_path> --watch
 ```
 
+## Layout
+
+The document layout must be given via the command option `--layout` or in the frontmatter of the single file. As layout a directory name inside the `./layouts` directory (default, can be changed using `--layouts-dir`) is expected. In the layout directory, a `index.html.j2` or `index.html` file is expected, which is loaded as entrypoint. The file is parsed using Jinja2.
+
 ## Input
 
 Input files are expected in markdown format with several markdown extensions. The markdown documents can utilize Jinja2 for templating inside the document (e. g. reusing texts).
 
 ### Bundling
 
 The bundling feature allows to bundle multiple documents into one PDF. This is useful when you want to create one PDF file from multiple source files. The bundling feature is enabled by adding the `--bundle` flag to the command. The specified input folder will be searched recursively for `*.md` files, files starting with an underscore will be ignored.
@@ -103,12 +109,12 @@
 
 Use tildes `~` around text to create a subscript formatting.
 
 ### Checkboxes
 
 Use `[ ]` to create a checkbox. Use `[x]` to mark a checkbox as checked.
 
-### Input Fields
+### Fields
 
 Use `[>input_id]` to create a text input. To create a textarea, add `|textarea` after the input id. To create a date field, add `|YYYY-MM-DD` after the input id.
 
 To add a placeholder, append the placeholder text within parens to the end of the input id: `[>input_id] (placeholder text)`.
```

### Comparing `md2weasypdf-0.0.8/md2weasypdf.egg-info/SOURCES.txt` & `md2weasypdf-0.0.9/md2weasypdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `md2weasypdf-0.0.8/setup.cfg` & `md2weasypdf-0.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = md2weasypdf
-version = 0.0.8
+version = 0.0.9
 author = Manuel Stingl
 author_email = contact@stingl.st
 description = Print PDFs from Markdown Files using Weasyprint
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = GNU LGPLv2.1
 classifiers =
```


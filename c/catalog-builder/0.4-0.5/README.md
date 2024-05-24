# Comparing `tmp/catalog_builder-0.4.tar.gz` & `tmp/catalog_builder-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catalog_builder-0.4.tar", last modified: Fri May  3 09:29:05 2024, max compression
+gzip compressed data, was "catalog_builder-0.5.tar", last modified: Fri May 24 09:16:09 2024, max compression
```

## Comparing `catalog_builder-0.4.tar` & `catalog_builder-0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-03 09:29:05.537030 catalog_builder-0.4/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1064 2024-03-06 14:29:44.000000 catalog_builder-0.4/LICENSE
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     7214 2024-05-03 09:29:05.536030 catalog_builder-0.4/PKG-INFO
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     6551 2024-03-19 13:44:29.000000 catalog_builder-0.4/README.md
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-03 09:29:05.533030 catalog_builder-0.4/catalog_builder/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     4400 2024-05-03 09:22:20.000000 catalog_builder-0.4/catalog_builder/catalogs.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     5698 2024-05-03 09:23:52.000000 catalog_builder-0.4/catalog_builder/cli.py
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     2461 2024-03-12 15:34:10.000000 catalog_builder-0.4/catalog_builder/utils.py
-drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-03 09:29:05.535030 catalog_builder-0.4/catalog_builder.egg-info/
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     7214 2024-05-03 09:29:05.000000 catalog_builder-0.4/catalog_builder.egg-info/PKG-INFO
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      338 2024-05-03 09:29:05.000000 catalog_builder-0.4/catalog_builder.egg-info/SOURCES.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        1 2024-05-03 09:29:05.000000 catalog_builder-0.4/catalog_builder.egg-info/dependency_links.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       52 2024-05-03 09:29:05.000000 catalog_builder-0.4/catalog_builder.egg-info/entry_points.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       92 2024-05-03 09:29:05.000000 catalog_builder-0.4/catalog_builder.egg-info/requires.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       16 2024-05-03 09:29:05.000000 catalog_builder-0.4/catalog_builder.egg-info/top_level.txt
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       38 2024-05-03 09:29:05.537030 catalog_builder-0.4/setup.cfg
--rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1040 2024-05-03 09:25:30.000000 catalog_builder-0.4/setup.py
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-24 09:16:09.117289 catalog_builder-0.5/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1064 2024-03-06 14:29:44.000000 catalog_builder-0.5/LICENSE
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     7214 2024-05-24 09:16:09.116289 catalog_builder-0.5/PKG-INFO
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     6551 2024-03-19 13:44:29.000000 catalog_builder-0.5/README.md
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-24 09:16:09.114288 catalog_builder-0.5/catalog_builder/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     4420 2024-05-24 09:13:45.000000 catalog_builder-0.5/catalog_builder/catalogs.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     5698 2024-05-03 09:23:52.000000 catalog_builder-0.5/catalog_builder/cli.py
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     2461 2024-03-12 15:34:10.000000 catalog_builder-0.5/catalog_builder/utils.py
+drwxr-xr-x   0 paul_marcombes  (1000) paul_marcombes  (1000)        0 2024-05-24 09:16:09.116289 catalog_builder-0.5/catalog_builder.egg-info/
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     7214 2024-05-24 09:16:09.000000 catalog_builder-0.5/catalog_builder.egg-info/PKG-INFO
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)      338 2024-05-24 09:16:09.000000 catalog_builder-0.5/catalog_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)        1 2024-05-24 09:16:09.000000 catalog_builder-0.5/catalog_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       52 2024-05-24 09:16:09.000000 catalog_builder-0.5/catalog_builder.egg-info/entry_points.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       92 2024-05-24 09:16:09.000000 catalog_builder-0.5/catalog_builder.egg-info/requires.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       16 2024-05-24 09:16:09.000000 catalog_builder-0.5/catalog_builder.egg-info/top_level.txt
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)       38 2024-05-24 09:16:09.117289 catalog_builder-0.5/setup.cfg
+-rw-r--r--   0 paul_marcombes  (1000) paul_marcombes  (1000)     1040 2024-05-24 09:14:03.000000 catalog_builder-0.5/setup.py
```

### Comparing `catalog_builder-0.4/LICENSE` & `catalog_builder-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `catalog_builder-0.4/PKG-INFO` & `catalog_builder-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: catalog_builder
-Version: 0.4
+Version: 0.5
 Summary: Data Catalogs Made Easy
-Download-URL: https://github.com/unytics/catalog_builder/archive/refs/tags/v0.4.tar.gz
+Download-URL: https://github.com/unytics/catalog_builder/archive/refs/tags/v0.5.tar.gz
 Author: Unytics
 Author-email: paul.marcombes@unytics.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `catalog_builder-0.4/README.md` & `catalog_builder-0.5/README.md`

 * *Files identical despite different names*

### Comparing `catalog_builder-0.4/catalog_builder/catalogs.py` & `catalog_builder-0.5/catalog_builder/catalogs.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
     def generate_markdown(self, markdown_folder_paths_to_include=None, add_children_in_folder_pages=False):
         shutil.rmtree(self.generated_docs_folder, ignore_errors=True)
         if markdown_folder_paths_to_include:
             assert isinstance(markdown_folder_paths_to_include, list), 'markdown_folder_paths_to_include must be a list'
             for folder in markdown_folder_paths_to_include:
                 if os.path.isdir(folder):
-                    shutil.copytree(folder, self.generated_docs_folder)
+                    shutil.copytree(folder, self.generated_docs_folder, dirs_exist_ok=True)
         self._generate_markdown_of_assets()
         if add_children_in_folder_pages:
             self._generate_markdown_of_folders()
 
     def _generate_markdown_of_assets(self):
         for asset in self.assets.to_dict(orient="records"):
             if not asset["path"] or asset["asset_type"] not in self.templates:
```

### Comparing `catalog_builder-0.4/catalog_builder/cli.py` & `catalog_builder-0.5/catalog_builder/cli.py`

 * *Files identical despite different names*

### Comparing `catalog_builder-0.4/catalog_builder/utils.py` & `catalog_builder-0.5/catalog_builder/utils.py`

 * *Files identical despite different names*

### Comparing `catalog_builder-0.4/catalog_builder.egg-info/PKG-INFO` & `catalog_builder-0.5/catalog_builder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: catalog_builder
-Version: 0.4
+Version: 0.5
 Summary: Data Catalogs Made Easy
-Download-URL: https://github.com/unytics/catalog_builder/archive/refs/tags/v0.4.tar.gz
+Download-URL: https://github.com/unytics/catalog_builder/archive/refs/tags/v0.5.tar.gz
 Author: Unytics
 Author-email: paul.marcombes@unytics.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `catalog_builder-0.4/setup.py` & `catalog_builder-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-VERSION = '0.4'
+VERSION = '0.5'
 
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
```


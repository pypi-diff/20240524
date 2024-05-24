# Comparing `tmp/pynestor-1.7.6.tar.gz` & `tmp/pynestor-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynestor-1.7.6.tar", last modified: Fri Apr  5 07:25:03 2024, max compression
+gzip compressed data, was "pynestor-1.7.7.tar", last modified: Fri May 24 15:48:43 2024, max compression
```

## Comparing `pynestor-1.7.6.tar` & `pynestor-1.7.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 07:25:03.124643 pynestor-1.7.6/
--rw-r--r--   0 root         (0) root         (0)     1732 2024-04-05 07:25:03.124643 pynestor-1.7.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1215 2024-04-04 11:40:06.000000 pynestor-1.7.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)      600 2024-03-15 14:47:04.000000 pynestor-1.7.6/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      661 2024-04-05 07:25:03.124643 pynestor-1.7.6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 07:25:03.120643 pynestor-1.7.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 07:25:03.120643 pynestor-1.7.6/src/pynestor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-15 14:47:04.000000 pynestor-1.7.6/src/pynestor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2641 2024-03-15 14:47:04.000000 pynestor-1.7.6/src/pynestor/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      603 2024-03-15 14:47:04.000000 pynestor-1.7.6/src/pynestor/default-preview-nestor-cfg.yml
--rw-rw-rw-   0 root         (0) root         (0)    20913 2024-04-04 11:40:06.000000 pynestor-1.7.6/src/pynestor/preview_odoo_nestor.py
--rw-rw-rw-   0 root         (0) root         (0)    20612 2024-04-04 09:32:46.000000 pynestor-1.7.6/src/pynestor/pynestor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 07:25:03.124643 pynestor-1.7.6/src/pynestor.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1732 2024-04-05 07:25:03.000000 pynestor-1.7.6/src/pynestor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      388 2024-04-05 07:25:03.000000 pynestor-1.7.6/src/pynestor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 07:25:03.000000 pynestor-1.7.6/src/pynestor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2024-04-05 07:25:03.000000 pynestor-1.7.6/src/pynestor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-05 07:25:03.000000 pynestor-1.7.6/src/pynestor.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 07:25:03.124643 pynestor-1.7.6/tests/
--rw-rw-rw-   0 root         (0) root         (0)     4374 2024-04-04 11:40:06.000000 pynestor-1.7.6/tests/tests_spec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 15:48:43.705384 pynestor-1.7.7/
+-rw-r--r--   0 root         (0) root         (0)     1732 2024-05-24 15:48:43.705384 pynestor-1.7.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2024-05-24 15:31:39.000000 pynestor-1.7.7/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      600 2024-05-24 15:31:39.000000 pynestor-1.7.7/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      661 2024-05-24 15:48:43.705384 pynestor-1.7.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 15:48:43.705384 pynestor-1.7.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 15:48:43.705384 pynestor-1.7.7/src/pynestor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 15:48:30.000000 pynestor-1.7.7/src/pynestor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2641 2024-05-24 15:31:39.000000 pynestor-1.7.7/src/pynestor/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      603 2024-05-24 15:31:39.000000 pynestor-1.7.7/src/pynestor/default-preview-nestor-cfg.yml
+-rw-rw-rw-   0 root         (0) root         (0)    21135 2024-05-24 15:31:39.000000 pynestor-1.7.7/src/pynestor/preview_odoo_nestor.py
+-rw-rw-rw-   0 root         (0) root         (0)    20612 2024-05-24 15:31:39.000000 pynestor-1.7.7/src/pynestor/pynestor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 15:48:43.705384 pynestor-1.7.7/src/pynestor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1732 2024-05-24 15:48:43.000000 pynestor-1.7.7/src/pynestor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      388 2024-05-24 15:48:43.000000 pynestor-1.7.7/src/pynestor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 15:48:43.000000 pynestor-1.7.7/src/pynestor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2024-05-24 15:48:43.000000 pynestor-1.7.7/src/pynestor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-24 15:48:43.000000 pynestor-1.7.7/src/pynestor.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 15:48:43.705384 pynestor-1.7.7/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4374 2024-05-24 15:31:39.000000 pynestor-1.7.7/tests/tests_spec.py
```

### Comparing `pynestor-1.7.6/PKG-INFO` & `pynestor-1.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynestor
-Version: 1.7.6
+Version: 1.7.7
 Summary: Nestor wrapper in python
 Home-page: https://gitlab.ndp-systemes.fr/python-libs/py-nestor
 Author: Alexis Pasquier
 Author-email: contact@ndp-systemes.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
```

### Comparing `pynestor-1.7.6/README.md` & `pynestor-1.7.7/README.md`

 * *Files identical despite different names*

### Comparing `pynestor-1.7.6/pyproject.toml` & `pynestor-1.7.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynestor-1.7.6/setup.cfg` & `pynestor-1.7.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pynestor
-version = 1.7.6
+version = 1.7.7
 description = Nestor wrapper in python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.ndp-systemes.fr/python-libs/py-nestor
 author = Alexis Pasquier
 author_email = contact@ndp-systemes.fr
 classifiers =
```

### Comparing `pynestor-1.7.6/src/pynestor/__main__.py` & `pynestor-1.7.7/src/pynestor/__main__.py`

 * *Files identical despite different names*

### Comparing `pynestor-1.7.6/src/pynestor/default-preview-nestor-cfg.yml` & `pynestor-1.7.7/src/pynestor/default-preview-nestor-cfg.yml`

 * *Files identical despite different names*

### Comparing `pynestor-1.7.6/src/pynestor/preview_odoo_nestor.py` & `pynestor-1.7.7/src/pynestor/preview_odoo_nestor.py`

 * *Files 2% similar despite different names*

```diff
@@ -413,14 +413,18 @@
             log("Create instance")
             values = self.get_spec_values(stage="restore")
             self.log_spec(values)
             self.create_with_values(values)
 
         if self.config.ALWAYS_RESTORE or instance_doesnt_exist:
             if not self.config.NO_DB_DUMP:
+                if not instance_doesnt_exist:
+                    values = self.get_spec_values(stage="restore")
+                    self.edit_with_values(values)
+                    self.inst.wait(up=True, postgres=True)
                 self.restore_db()
             if self.config.MODULE_TO_INSTALL:
                 log("Install -i", self.config.MODULE_TO_INSTALL)
                 self.inst.install(self.config.MODULE_TO_INSTALL)
 
         log("MAJ de l'instance", self.inst.name)
         self.stop()
```

### Comparing `pynestor-1.7.6/src/pynestor/pynestor.py` & `pynestor-1.7.7/src/pynestor/pynestor.py`

 * *Files identical despite different names*

### Comparing `pynestor-1.7.6/src/pynestor.egg-info/PKG-INFO` & `pynestor-1.7.7/src/pynestor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynestor
-Version: 1.7.6
+Version: 1.7.7
 Summary: Nestor wrapper in python
 Home-page: https://gitlab.ndp-systemes.fr/python-libs/py-nestor
 Author: Alexis Pasquier
 Author-email: contact@ndp-systemes.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
```

### Comparing `pynestor-1.7.6/tests/tests_spec.py` & `pynestor-1.7.7/tests/tests_spec.py`

 * *Files identical despite different names*


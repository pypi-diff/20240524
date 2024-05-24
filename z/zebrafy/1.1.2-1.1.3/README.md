# Comparing `tmp/zebrafy-1.1.2.tar.gz` & `tmp/zebrafy-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zebrafy-1.1.2.tar", last modified: Thu May 16 06:16:10 2024, max compression
+gzip compressed data, was "zebrafy-1.1.3.tar", last modified: Fri May 24 03:18:33 2024, max compression
```

## Comparing `zebrafy-1.1.2.tar` & `zebrafy-1.1.3.tar`

### file list

```diff
@@ -1,21 +1,75 @@
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-16 06:16:10.856267 zebrafy-1.1.2/
--rw-r--r--   0 m         (1000) m         (1000)     7652 2023-08-06 02:30:03.000000 zebrafy-1.1.2/LICENSE.txt
--rw-r--r--   0 m         (1000) m         (1000)    11576 2024-05-16 06:16:10.856267 zebrafy-1.1.2/PKG-INFO
--rw-r--r--   0 m         (1000) m         (1000)    10083 2024-05-16 06:12:27.000000 zebrafy-1.1.2/README.rst
--rw-r--r--   0 m         (1000) m         (1000)     1780 2024-05-16 06:04:12.000000 zebrafy-1.1.2/pyproject.toml
--rw-r--r--   0 m         (1000) m         (1000)       38 2024-05-16 06:16:10.856267 zebrafy-1.1.2/setup.cfg
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-16 06:16:10.856267 zebrafy-1.1.2/tests/
--rw-r--r--   0 m         (1000) m         (1000)    23562 2024-05-16 06:03:54.000000 zebrafy-1.1.2/tests/test_zebrafy.py
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-16 06:16:10.856267 zebrafy-1.1.2/zebrafy/
--rw-r--r--   0 m         (1000) m         (1000)      196 2024-05-16 06:04:01.000000 zebrafy-1.1.2/zebrafy/__init__.py
--rw-r--r--   0 m         (1000) m         (1000)     3401 2024-05-16 01:49:32.000000 zebrafy-1.1.2/zebrafy/crc.py
--rw-r--r--   0 m         (1000) m         (1000)     6644 2024-05-16 01:49:53.000000 zebrafy-1.1.2/zebrafy/graphic_field.py
--rw-r--r--   0 m         (1000) m         (1000)    12300 2024-05-16 06:02:35.000000 zebrafy-1.1.2/zebrafy/zebrafy_image.py
--rw-r--r--   0 m         (1000) m         (1000)    12363 2024-05-16 06:02:35.000000 zebrafy-1.1.2/zebrafy/zebrafy_pdf.py
--rw-r--r--   0 m         (1000) m         (1000)     5654 2024-05-16 01:48:59.000000 zebrafy-1.1.2/zebrafy/zebrafy_zpl.py
-drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-16 06:16:10.856267 zebrafy-1.1.2/zebrafy.egg-info/
--rw-r--r--   0 m         (1000) m         (1000)    11576 2024-05-16 06:16:10.000000 zebrafy-1.1.2/zebrafy.egg-info/PKG-INFO
--rw-r--r--   0 m         (1000) m         (1000)      344 2024-05-16 06:16:10.000000 zebrafy-1.1.2/zebrafy.egg-info/SOURCES.txt
--rw-r--r--   0 m         (1000) m         (1000)        1 2024-05-16 06:16:10.000000 zebrafy-1.1.2/zebrafy.egg-info/dependency_links.txt
--rw-r--r--   0 m         (1000) m         (1000)      107 2024-05-16 06:16:10.000000 zebrafy-1.1.2/zebrafy.egg-info/requires.txt
--rw-r--r--   0 m         (1000) m         (1000)        8 2024-05-16 06:16:10.000000 zebrafy-1.1.2/zebrafy.egg-info/top_level.txt
+drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-24 03:18:33.728341 zebrafy-1.1.3/
+-rw-r--r--   0 m         (1000) m         (1000)      230 2023-08-07 02:54:40.000000 zebrafy-1.1.3/.editorconfig
+-rw-r--r--   0 m         (1000) m         (1000)       36 2023-08-12 04:33:43.000000 zebrafy-1.1.3/.gitattributes
+drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-24 03:18:33.712340 zebrafy-1.1.3/.github/
+drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-24 03:18:33.712340 zebrafy-1.1.3/.github/workflows/
+-rw-r--r--   0 m         (1000) m         (1000)      843 2024-05-24 03:15:43.000000 zebrafy-1.1.3/.github/workflows/ci.yml
+-rw-r--r--   0 m         (1000) m         (1000)     1587 2023-08-16 03:32:25.000000 zebrafy-1.1.3/.gitignore
+-rw-r--r--   0 m         (1000) m         (1000)     1165 2024-05-24 03:15:43.000000 zebrafy-1.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 m         (1000) m         (1000)      205 2024-05-24 03:15:43.000000 zebrafy-1.1.3/.prettierrc.yml
+-rw-r--r--   0 m         (1000) m         (1000)      402 2024-05-24 01:30:45.000000 zebrafy-1.1.3/.pylintrc
+-rw-r--r--   0 m         (1000) m         (1000)      730 2024-05-24 03:15:43.000000 zebrafy-1.1.3/.readthedocs.yml
+-rw-r--r--   0 m         (1000) m         (1000)     7652 2023-08-06 02:30:03.000000 zebrafy-1.1.3/LICENSE.txt
+-rw-r--r--   0 m         (1000) m         (1000)    11657 2024-05-24 03:18:33.728341 zebrafy-1.1.3/PKG-INFO
+-rw-r--r--   0 m         (1000) m         (1000)    10083 2024-05-16 06:23:33.000000 zebrafy-1.1.3/README.rst
+drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-24 03:18:33.716340 zebrafy-1.1.3/docs/
+-rw-r--r--   0 m         (1000) m         (1000)      634 2023-08-15 03:04:59.000000 zebrafy-1.1.3/docs/Makefile
+-rw-r--r--   0 m         (1000) m         (1000)     1661 2024-05-24 03:15:43.000000 zebrafy-1.1.3/docs/conf.py
+-rw-r--r--   0 m         (1000) m         (1000)      249 2023-08-16 03:34:22.000000 zebrafy-1.1.3/docs/index.rst
+-rw-r--r--   0 m         (1000) m         (1000)      765 2023-08-15 05:00:09.000000 zebrafy-1.1.3/docs/make.bat
+-rw-r--r--   0 m         (1000) m         (1000)       50 2023-08-16 02:46:29.000000 zebrafy-1.1.3/docs/modules.rst
+-rw-r--r--   0 m         (1000) m         (1000)       70 2024-05-24 03:15:43.000000 zebrafy-1.1.3/docs/requirements.in
+-rw-r--r--   0 m         (1000) m         (1000)     1433 2024-05-24 03:15:43.000000 zebrafy-1.1.3/docs/requirements.txt
+-rw-r--r--   0 m         (1000) m         (1000)     7859 2024-05-16 06:02:35.000000 zebrafy-1.1.3/docs/usage.rst
+-rw-r--r--   0 m         (1000) m         (1000)     5962 2023-08-17 03:01:04.000000 zebrafy-1.1.3/docs/zebrafy-64.png
+-rw-r--r--   0 m         (1000) m         (1000)   483090 2023-08-17 02:56:09.000000 zebrafy-1.1.3/docs/zebrafy-long.png
+-rw-r--r--   0 m         (1000) m         (1000)   333682 2023-08-17 02:56:10.000000 zebrafy-1.1.3/docs/zebrafy.png
+-rw-r--r--   0 m         (1000) m         (1000)      763 2023-08-17 02:19:44.000000 zebrafy-1.1.3/docs/zebrafy.rst
+-rw-r--r--   0 m         (1000) m         (1000)     1826 2024-05-24 03:15:43.000000 zebrafy-1.1.3/pyproject.toml
+-rw-r--r--   0 m         (1000) m         (1000)       38 2024-05-24 03:18:33.728341 zebrafy-1.1.3/setup.cfg
+drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-24 03:18:33.716340 zebrafy-1.1.3/tests/
+-rw-r--r--   0 m         (1000) m         (1000)       28 2024-05-24 03:15:43.000000 zebrafy-1.1.3/tests/__init__.py
+drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-24 03:18:33.724341 zebrafy-1.1.3/tests/static/
+-rw-r--r--   0 m         (1000) m         (1000)   261566 2023-08-12 23:38:59.000000 zebrafy-1.1.3/tests/static/test_image.png
+-rw-r--r--   0 m         (1000) m         (1000)   108008 2024-03-24 00:36:09.000000 zebrafy-1.1.3/tests/static/test_image_ascii.png
+-rw-r--r--   0 m         (1000) m         (1000)   409641 2024-03-24 00:36:09.000000 zebrafy-1.1.3/tests/static/test_image_ascii.zpl
+-rw-r--r--   0 m         (1000) m         (1000)   108008 2024-03-24 00:36:09.000000 zebrafy-1.1.3/tests/static/test_image_b64.png
+-rw-r--r--   0 m         (1000) m         (1000)   273119 2024-03-24 00:36:09.000000 zebrafy-1.1.3/tests/static/test_image_b64.zpl
+-rw-r--r--   0 m         (1000) m         (1000)   409631 2023-08-12 03:28:58.000000 zebrafy-1.1.3/tests/static/test_image_broken.zpl
+-rw-r--r--   0 m         (1000) m         (1000)   409641 2023-08-14 03:06:34.000000 zebrafy-1.1.3/tests/static/test_image_high_threshold.zpl
+-rw-r--r--   0 m         (1000) m         (1000)   409641 2023-08-17 01:54:05.000000 zebrafy-1.1.3/tests/static/test_image_invert.zpl
+-rw-r--r--   0 m         (1000) m         (1000)   409641 2023-08-17 01:54:05.000000 zebrafy-1.1.3/tests/static/test_image_invert_no_dither.zpl
+-rw-r--r--   0 m         (1000) m         (1000)   409641 2023-08-14 03:06:34.000000 zebrafy-1.1.3/tests/static/test_image_low_threshold.zpl
+-rw-r--r--   0 m         (1000) m         (1000)   819274 2023-08-14 03:27:47.000000 zebrafy-1.1.3/tests/static/test_image_multiple.zpl
+-rw-r--r--   0 m         (1000) m         (1000)   409641 2023-08-14 03:06:34.000000 zebrafy-1.1.3/tests/static/test_image_no_dither.zpl
+-rw-r--r--   0 m         (1000) m         (1000)   409645 2023-08-17 01:56:19.000000 zebrafy-1.1.3/tests/static/test_image_pos_x_pos_y.zpl
+-rw-r--r--   0 m         (1000) m         (1000)   409641 2024-05-16 06:02:35.000000 zebrafy-1.1.3/tests/static/test_image_rotation.zpl
+-rw-r--r--   0 m         (1000) m         (1000)    63038 2023-08-14 03:06:34.000000 zebrafy-1.1.3/tests/static/test_image_width_height.zpl
+-rw-r--r--   0 m         (1000) m         (1000)   108008 2024-03-24 00:36:09.000000 zebrafy-1.1.3/tests/static/test_image_z64.png
+-rw-r--r--   0 m         (1000) m         (1000)   118567 2024-03-24 00:36:09.000000 zebrafy-1.1.3/tests/static/test_image_z64.zpl
+-rw-r--r--   0 m         (1000) m         (1000)   118567 2024-03-24 00:36:09.000000 zebrafy-1.1.3/tests/static/test_image_z64_broken_compression.zpl
+-rw-r--r--   0 m         (1000) m         (1000)   118567 2024-03-24 00:36:09.000000 zebrafy-1.1.3/tests/static/test_image_z64_broken_crc.zpl
+-rw-r--r--   0 m         (1000) m         (1000)   315326 2023-08-14 03:18:02.000000 zebrafy-1.1.3/tests/static/test_pdf.pdf
+-rw-r--r--   0 m         (1000) m         (1000)   244006 2024-03-24 00:36:09.000000 zebrafy-1.1.3/tests/static/test_pdf_ascii.zpl
+-rw-r--r--   0 m         (1000) m         (1000)   162712 2024-03-24 00:36:09.000000 zebrafy-1.1.3/tests/static/test_pdf_b64.zpl
+-rw-r--r--   0 m         (1000) m         (1000)   244006 2023-08-14 03:06:35.000000 zebrafy-1.1.3/tests/static/test_pdf_high_threshold.zpl
+-rw-r--r--   0 m         (1000) m         (1000)   244006 2023-08-14 03:06:35.000000 zebrafy-1.1.3/tests/static/test_pdf_low_threshold.zpl
+-rw-r--r--   0 m         (1000) m         (1000)   244006 2023-08-14 03:06:35.000000 zebrafy-1.1.3/tests/static/test_pdf_no_dither.zpl
+-rw-r--r--   0 m         (1000) m         (1000)   242422 2024-05-16 06:02:35.000000 zebrafy-1.1.3/tests/static/test_pdf_rotation.zpl
+-rw-r--r--   0 m         (1000) m         (1000)   244014 2024-05-12 01:56:42.000000 zebrafy-1.1.3/tests/static/test_pdf_split_pages.zpl
+-rw-r--r--   0 m         (1000) m         (1000)   460872 2023-08-14 03:06:35.000000 zebrafy-1.1.3/tests/static/test_pdf_width_height.zpl
+-rw-r--r--   0 m         (1000) m         (1000)    31971 2024-03-24 00:36:09.000000 zebrafy-1.1.3/tests/static/test_pdf_z64.zpl
+-rw-r--r--   0 m         (1000) m         (1000)    24019 2024-05-24 03:15:43.000000 zebrafy-1.1.3/tests/test_zebrafy.py
+drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-24 03:18:33.728341 zebrafy-1.1.3/zebrafy/
+-rw-r--r--   0 m         (1000) m         (1000)      465 2024-05-24 03:15:43.000000 zebrafy-1.1.3/zebrafy/__init__.py
+-rw-r--r--   0 m         (1000) m         (1000)     3258 2024-05-24 03:15:43.000000 zebrafy-1.1.3/zebrafy/crc.py
+-rw-r--r--   0 m         (1000) m         (1000)     6324 2024-05-24 03:15:43.000000 zebrafy-1.1.3/zebrafy/graphic_field.py
+-rw-r--r--   0 m         (1000) m         (1000)    11048 2024-05-24 03:15:43.000000 zebrafy-1.1.3/zebrafy/zebrafy_image.py
+-rw-r--r--   0 m         (1000) m         (1000)    10987 2024-05-24 03:15:43.000000 zebrafy-1.1.3/zebrafy/zebrafy_pdf.py
+-rw-r--r--   0 m         (1000) m         (1000)     5553 2024-05-24 03:15:43.000000 zebrafy-1.1.3/zebrafy/zebrafy_zpl.py
+drwxr-xr-x   0 m         (1000) m         (1000)        0 2024-05-24 03:18:33.728341 zebrafy-1.1.3/zebrafy.egg-info/
+-rw-r--r--   0 m         (1000) m         (1000)    11657 2024-05-24 03:18:33.000000 zebrafy-1.1.3/zebrafy.egg-info/PKG-INFO
+-rw-r--r--   0 m         (1000) m         (1000)     1759 2024-05-24 03:18:33.000000 zebrafy-1.1.3/zebrafy.egg-info/SOURCES.txt
+-rw-r--r--   0 m         (1000) m         (1000)        1 2024-05-24 03:18:33.000000 zebrafy-1.1.3/zebrafy.egg-info/dependency_links.txt
+-rw-r--r--   0 m         (1000) m         (1000)      140 2024-05-24 03:18:33.000000 zebrafy-1.1.3/zebrafy.egg-info/requires.txt
+-rw-r--r--   0 m         (1000) m         (1000)        8 2024-05-24 03:18:33.000000 zebrafy-1.1.3/zebrafy.egg-info/top_level.txt
```

### Comparing `zebrafy-1.1.2/LICENSE.txt` & `zebrafy-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.2/PKG-INFO` & `zebrafy-1.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zebrafy
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python library for converting PDF and images to Zebra Programming Language (ZPL)
 Author-email: Miika Nissi <miika@miikanissi.com>
 Maintainer-email: Miika Nissi <miika@miikanissi.com>
 License: LGPLv3
 Project-URL: Homepage, https://github.com/miikanissi/zebrafy/
 Project-URL: Documentation, https://zebrafy.readthedocs.io/
 Classifier: Development Status :: 4 - Beta
@@ -22,21 +22,23 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Manufacturing
 Classifier: Topic :: Printing
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: pillow
-Requires-Dist: pypdfium2<=4.18.0
+Requires-Dist: pypdfium2>=4.8.0
+Provides-Extra: docs
+Requires-Dist: sphinx>=7.0.0; extra == "docs"
+Requires-Dist: sphinx_autodoc_typehints>=2.0.0; extra == "docs"
+Requires-Dist: sphinx_rtd_theme>=2.0.0; extra == "docs"
 Provides-Extra: test
 Requires-Dist: pytest-cov; extra == "test"
-Provides-Extra: dev
-Requires-Dist: sphinx; extra == "dev"
-Requires-Dist: sphinx_autodoc_typehints; extra == "dev"
-Requires-Dist: sphinx_rtd_theme>=1.2.0; extra == "dev"
+Provides-Extra: lint
+Requires-Dist: pre-commit; extra == "lint"
 
 |zebrafy_icon_64| Zebrafy
 =========================
 
 .. |zebrafy_icon_64| image:: https://raw.githubusercontent.com/miikanissi/zebrafy/master/docs/zebrafy-64.png
    :alt: Zebrafy Logo
```

### Comparing `zebrafy-1.1.2/README.rst` & `zebrafy-1.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `zebrafy-1.1.2/pyproject.toml` & `zebrafy-1.1.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = [ "setuptools", "wheel"]
+requires = [ "setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zebrafy"
-version = "1.1.2"
+version = "1.1.3"
 description = "Python library for converting PDF and images to Zebra Programming Language (ZPL)"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     "Operating System :: OS Independent",
     "Natural Language :: English",
     "Programming Language :: Python",
@@ -19,26 +19,28 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "Intended Audience :: Manufacturing",
     "Topic :: Printing",
 ]
-dependencies = ["pillow", "pypdfium2<=4.18.0"]
+dependencies = ["pillow", "pypdfium2>=4.8.0"]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
+docs = [
+    "sphinx>=7.0.0",
+    "sphinx_autodoc_typehints>=2.0.0",
+    "sphinx_rtd_theme>=2.0.0",
+]
 test = [
     "pytest-cov",
 ]
-
-dev = [
-    "sphinx",
-    "sphinx_autodoc_typehints",
-    "sphinx_rtd_theme>=1.2.0",
+lint = [
+    "pre-commit",
 ]
 
 [[project.authors]]
 name = "Miika Nissi"
 email = "miika@miikanissi.com"
 
 [[project.maintainers]]
```

### Comparing `zebrafy-1.1.2/tests/test_zebrafy.py` & `zebrafy-1.1.3/tests/test_zebrafy.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,189 +31,197 @@
 from PIL import Image
 
 # 3. Local imports in the relative form:
 from zebrafy import CRC, GraphicField, ZebrafyImage, ZebrafyPDF, ZebrafyZPL, __version__
 
 
 class TestZebrafy(unittest.TestCase):
+    """Test Zebrafy package."""
+
     def _read_static_file(self, file_name: str) -> Union[bytes, str]:
         """
-        Helper method to read a test file from static directory.
+        Read a test file from static directory.
 
         :param file_name: File name of a file in tests/static directory.
         :returns: File contents as bytes or string
         """
         open_mode = "r" if file_name.endswith(".zpl") else "rb"
         with open(
             os.path.join(os.path.join(os.path.dirname(__file__), "static"), file_name),
             open_mode,
         ) as file:
             return file.read()
 
     def test_version(self):
         """Test package version."""
-        self.assertEqual(__version__, "1.1.2")
+        self.assertEqual(__version__, "1.1.3")
 
     ###########
     # CRC Tests
     ###########
     def test_crc_data_bytes(self):
+        """Test CRC data bytes input."""
         with self.assertRaises(ValueError):
             CRC(None)
         with self.assertRaises(TypeError):
             CRC(123)
 
     def test_crc_poly(self):
+        """Test CRC polynomial input."""
         crc = CRC(b"Python is fun")
         with self.assertRaises(ValueError):
             crc.poly = None
         with self.assertRaises(TypeError):
             crc.poly = "Test"
 
     ####################
     # GraphicField Tests
     ####################
     def test_graphic_field_image(self):
+        """Test GraphicField image input."""
         with self.assertRaises(ValueError):
             GraphicField(None)
         with self.assertRaises(TypeError):
             GraphicField(123)
 
     def test_graphic_field_format(self):
+        """Test GraphicField format input."""
         im = Image.new(mode="RGB", size=(200, 200))
         gf = GraphicField(im)
         with self.assertRaises(ValueError):
             gf.format = None
         with self.assertRaises(TypeError):
             gf.format = 123
         with self.assertRaises(ValueError):
             gf.format = "D"
 
     def test_graphic_field_deprecated_compression_type(self):
+        """Test deprecated GraphicField compression_type input."""
         im = Image.new(mode="RGB", size=(200, 200))
         gfa = GraphicField(im, compression_type="A")
         self.assertEqual(gfa.format, "ASCII")
         gfb = GraphicField(im, compression_type="B")
         self.assertEqual(gfb.format, "B64")
         gfc = GraphicField(im, compression_type="C")
         self.assertEqual(gfc.format, "Z64")
 
     ####################
     # ZebrafyImage Tests
     ####################
     # Input validation
     def test_zebrafy_image_image(self):
-        """Test ZebrafyImage image input"""
+        """Test ZebrafyImage image input."""
         with self.assertRaises(ValueError):
             ZebrafyImage(None)
         with self.assertRaises(TypeError):
             ZebrafyImage(123)
 
     def test_zebrafy_image_format(self):
-        """Test ZebrafyImage format input"""
+        """Test ZebrafyImage format input."""
         im = Image.new(mode="RGB", size=(200, 200))
         zebrafy_image = ZebrafyImage(im)
         with self.assertRaises(ValueError):
             zebrafy_image.format = None
         with self.assertRaises(TypeError):
             zebrafy_image.format = 123
         with self.assertRaises(ValueError):
             zebrafy_image.format = "D"
 
     def test_zebrafy_image_deprecated_compression_type(self):
+        """Test deprecated ZebrafyImage compression_type input."""
         im = Image.new(mode="RGB", size=(200, 200))
         gfa = ZebrafyImage(im, compression_type="A")
         self.assertEqual(gfa.format, "ASCII")
         gfb = ZebrafyImage(im, compression_type="B")
         self.assertEqual(gfb.format, "B64")
         gfc = ZebrafyImage(im, compression_type="C")
         self.assertEqual(gfc.format, "Z64")
 
     def test_zebrafy_image_invert(self):
-        """Test ZebrafyImage invert input"""
+        """Test ZebrafyImage invert input."""
         im = Image.new(mode="RGB", size=(200, 200))
         zebrafy_image = ZebrafyImage(im)
         with self.assertRaises(ValueError):
             zebrafy_image.invert = None
         with self.assertRaises(TypeError):
             zebrafy_image.invert = "123"
 
     def test_zebrafy_image_dither(self):
-        """Test ZebrafyImage dither input"""
+        """Test ZebrafyImage dither input."""
         im = Image.new(mode="RGB", size=(200, 200))
         zebrafy_image = ZebrafyImage(im)
         with self.assertRaises(ValueError):
             zebrafy_image.dither = None
         with self.assertRaises(TypeError):
             zebrafy_image.dither = "123"
 
     def test_zebrafy_image_threshold(self):
-        """Test ZebrafyImage threshold input"""
+        """Test ZebrafyImage threshold input."""
         im = Image.new(mode="RGB", size=(200, 200))
         zebrafy_image = ZebrafyImage(im)
         with self.assertRaises(ValueError):
             zebrafy_image.threshold = None
         with self.assertRaises(TypeError):
             zebrafy_image.threshold = "123"
         with self.assertRaises(ValueError):
             zebrafy_image.threshold = -1
         with self.assertRaises(ValueError):
             zebrafy_image.threshold = 256
 
     def test_zebrafy_image_width(self):
-        """Test ZebrafyImage width input"""
+        """Test ZebrafyImage width input."""
         im = Image.new(mode="RGB", size=(200, 200))
         zebrafy_image = ZebrafyImage(im)
         with self.assertRaises(ValueError):
             zebrafy_image.width = None
         with self.assertRaises(TypeError):
             zebrafy_image.width = "123"
 
     def test_zebrafy_image_height(self):
-        """Test ZebrafyImage height input"""
+        """Test ZebrafyImage height input."""
         im = Image.new(mode="RGB", size=(200, 200))
         zebrafy_image = ZebrafyImage(im)
         with self.assertRaises(ValueError):
             zebrafy_image.height = None
         with self.assertRaises(TypeError):
             zebrafy_image.height = "123"
 
     def test_zebrafy_image_pos_x(self):
-        """Test ZebrafyImage pos_x input"""
+        """Test ZebrafyImage pos_x input."""
         im = Image.new(mode="RGB", size=(200, 200))
         zebrafy_image = ZebrafyImage(im)
         with self.assertRaises(ValueError):
             zebrafy_image.pos_x = None
         with self.assertRaises(TypeError):
             zebrafy_image.pos_x = "123"
 
     def test_zebrafy_image_pos_y(self):
-        """Test ZebrafyImage pos_y input"""
+        """Test ZebrafyImage pos_y input."""
         im = Image.new(mode="RGB", size=(200, 200))
         zebrafy_image = ZebrafyImage(im)
         with self.assertRaises(ValueError):
             zebrafy_image.pos_y = None
         with self.assertRaises(TypeError):
             zebrafy_image.pos_y = "123"
 
     def test_zebrafy_image_rotation(self):
-        """Test ZebrafyImage rotation input"""
+        """Test ZebrafyImage rotation input."""
         im = Image.new(mode="RGB", size=(200, 200))
         zebrafy_image = ZebrafyImage(im)
         with self.assertRaises(ValueError):
             zebrafy_image.rotation = None
         with self.assertRaises(TypeError):
             zebrafy_image.rotation = "123"
         with self.assertRaises(TypeError):
             zebrafy_image.rotation = 90.0
         with self.assertRaises(ValueError):
             zebrafy_image.rotation = 45
 
     def test_zebrafy_image_complete_zpl(self):
-        """Test ZebrafyImage complete_zpl input"""
+        """Test ZebrafyImage complete_zpl input."""
         im = Image.new(mode="RGB", size=(200, 200))
         zebrafy_image = ZebrafyImage(im)
         with self.assertRaises(ValueError):
             zebrafy_image.complete_zpl = None
         with self.assertRaises(TypeError):
             zebrafy_image.complete_zpl = "123"
 
@@ -316,131 +324,132 @@
         )
 
     ##################
     # ZebrafyPDF Tests
     ##################
     # Input validation
     def test_zebrafy_pdf_pdf_bytes(self):
-        """Test ZebrafyImage pdf_bytes input"""
+        """Test ZebrafyImage pdf_bytes input."""
         with self.assertRaises(ValueError):
             ZebrafyPDF(None)
         with self.assertRaises(TypeError):
             ZebrafyPDF(123)
 
     def test_zebrafy_pdf_format(self):
-        """Test ZebrafyPDF format input"""
+        """Test ZebrafyPDF format input."""
         pdf = self._read_static_file("test_pdf.pdf")
         zebrafy_pdf = ZebrafyPDF(pdf)
         with self.assertRaises(ValueError):
             zebrafy_pdf.format = None
         with self.assertRaises(TypeError):
             zebrafy_pdf.format = 123
         with self.assertRaises(ValueError):
             zebrafy_pdf.format = "D"
 
     def test_zebrafy_pdf_deprecated_compression_type(self):
+        """Test deprecated ZebrafyPDF compression_type input."""
         pdf = self._read_static_file("test_pdf.pdf")
         gfa = ZebrafyPDF(pdf, compression_type="A")
         self.assertEqual(gfa.format, "ASCII")
         gfb = ZebrafyPDF(pdf, compression_type="B")
         self.assertEqual(gfb.format, "B64")
         gfc = ZebrafyPDF(pdf, compression_type="C")
         self.assertEqual(gfc.format, "Z64")
 
     def test_zebrafy_pdf_invert(self):
-        """Test ZebrafyPDF invert input"""
+        """Test ZebrafyPDF invert input."""
         pdf = self._read_static_file("test_pdf.pdf")
         zebrafy_pdf = ZebrafyPDF(pdf)
         with self.assertRaises(ValueError):
             zebrafy_pdf.invert = None
         with self.assertRaises(TypeError):
             zebrafy_pdf.invert = "123"
 
     def test_zebrafy_pdf_dither(self):
-        """Test ZebrafyPDF dither input"""
+        """Test ZebrafyPDF dither input."""
         pdf = self._read_static_file("test_pdf.pdf")
         zebrafy_pdf = ZebrafyPDF(pdf)
         with self.assertRaises(ValueError):
             zebrafy_pdf.dither = None
         with self.assertRaises(TypeError):
             zebrafy_pdf.dither = "123"
 
     def test_zebrafy_pdf_threshold(self):
-        """Test ZebrafyPDF threshold input"""
+        """Test ZebrafyPDF threshold input."""
         pdf = self._read_static_file("test_pdf.pdf")
         zebrafy_pdf = ZebrafyPDF(pdf)
         with self.assertRaises(ValueError):
             zebrafy_pdf.threshold = None
         with self.assertRaises(TypeError):
             zebrafy_pdf.threshold = "123"
         with self.assertRaises(ValueError):
             zebrafy_pdf.threshold = -1
         with self.assertRaises(ValueError):
             zebrafy_pdf.threshold = 256
 
     def test_zebrafy_pdf_width(self):
-        """Test ZebrafyPDF width input"""
+        """Test ZebrafyPDF width input."""
         pdf = self._read_static_file("test_pdf.pdf")
         zebrafy_pdf = ZebrafyPDF(pdf)
         with self.assertRaises(ValueError):
             zebrafy_pdf.width = None
         with self.assertRaises(TypeError):
             zebrafy_pdf.width = "123"
 
     def test_zebrafy_pdf_height(self):
-        """Test ZebrafyPDF height input"""
+        """Test ZebrafyPDF height input."""
         pdf = self._read_static_file("test_pdf.pdf")
         zebrafy_pdf = ZebrafyPDF(pdf)
         with self.assertRaises(ValueError):
             zebrafy_pdf.height = None
         with self.assertRaises(TypeError):
             zebrafy_pdf.height = "123"
 
     def test_zebrafy_pdf_pos_x(self):
-        """Test ZebrafyPDF pos_x input"""
+        """Test ZebrafyPDF pos_x input."""
         pdf = self._read_static_file("test_pdf.pdf")
         zebrafy_pdf = ZebrafyPDF(pdf)
         with self.assertRaises(ValueError):
             zebrafy_pdf.pos_x = None
         with self.assertRaises(TypeError):
             zebrafy_pdf.pos_x = "123"
 
     def test_zebrafy_pdf_pos_y(self):
-        """Test ZebrafyPDF pos_y input"""
+        """Test ZebrafyPDF pos_y input."""
         pdf = self._read_static_file("test_pdf.pdf")
         zebrafy_pdf = ZebrafyPDF(pdf)
         with self.assertRaises(ValueError):
             zebrafy_pdf.pos_y = None
         with self.assertRaises(TypeError):
             zebrafy_pdf.pos_y = "123"
 
     def test_zebrafy_pdf_rotation(self):
-        """Test ZebrafyPDF rotation"""
+        """Test ZebrafyPDF rotation."""
         pdf = self._read_static_file("test_pdf.pdf")
         zebrafy_pdf = ZebrafyPDF(pdf)
         with self.assertRaises(ValueError):
             zebrafy_pdf.rotation = None
         with self.assertRaises(TypeError):
             zebrafy_pdf.rotation = "123"
         with self.assertRaises(TypeError):
             zebrafy_pdf.rotation = 90.0
         with self.assertRaises(ValueError):
             zebrafy_pdf.rotation = 45
 
     def test_zebrafy_pdf_complete_zpl(self):
-        """Test ZebrafyPDF complete_zpl input"""
+        """Test ZebrafyPDF complete_zpl input."""
         pdf = self._read_static_file("test_pdf.pdf")
         zebrafy_pdf = ZebrafyPDF(pdf)
         with self.assertRaises(ValueError):
             zebrafy_pdf.complete_zpl = None
         with self.assertRaises(TypeError):
             zebrafy_pdf.complete_zpl = "123"
 
     def test_zebrafy_pdf_split_pages(self):
-        """Test ZebrafyPDF split pages"""
+        """Test ZebrafyPDF split pages."""
         pdf = self._read_static_file("test_pdf.pdf")
         zebrafy_pdf = ZebrafyPDF(pdf)
         with self.assertRaises(ValueError):
             zebrafy_pdf.split_pages = None
         with self.assertRaises(TypeError):
             zebrafy_pdf.split_pages = "123"
 
@@ -512,14 +521,15 @@
         ).to_zpl()
         self.assertEqual(gf_zpl, self._read_static_file("test_pdf_split_pages.zpl"))
 
     ##################
     # ZebrafyZPL Tests
     ##################
     def test_zebrafy_zpl_zpl_data(self):
+        """Test ZebrafyZPL zpl_data input."""
         with self.assertRaises(ValueError):
             ZebrafyZPL(None)
         with self.assertRaises(TypeError):
             ZebrafyZPL(123)
 
     def test_ascii_zpl_to_image(self):
         """Test ZPL GFA ASCII to image bytes."""
```

### Comparing `zebrafy-1.1.2/zebrafy/crc.py` & `zebrafy-1.1.3/zebrafy/crc.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,31 +50,26 @@
 
     @data_bytes.setter
     def data_bytes(self, d):
         if d is None:
             raise ValueError("Bytes data cannot be empty.")
         if not isinstance(d, bytes):
             raise TypeError(
-                "Bytes data must be a valid bytes object. {param_type} was given."
-                .format(param_type=type(d))
+                f"Bytes data must be a valid bytes object. {type(d)} was given."
             )
         self._data_bytes = d
 
     poly = property(operator.attrgetter("_poly"))
 
     @poly.setter
     def poly(self, p):
         if p is None:
             raise ValueError("Polynomial cannot be empty.")
         if not isinstance(p, int):
-            raise TypeError(
-                "Polynomial must be a valid integer. {param_type} was given.".format(
-                    param_type=type(p)
-                )
-            )
+            raise TypeError(f"Polynomial must be a valid integer. {type(p)} was given.")
         self._poly = p
 
     def _get_crc16_ccitt(self) -> int:
         """
         Calculate CRC-16-CCITT Algorithm.
 
         :returns: CRC-16-CCITT
@@ -96,8 +91,8 @@
 
     def get_crc_hex_string(self) -> str:
         """
         Get CRC-16-CCITT as four digit zero padding hexadecimal string.
 
         :returns: CRC-16-CCITT as four digit zero padding hexadecimal string
         """
-        return "%04X" % self._get_crc16_ccitt()
+        return f"{self._get_crc16_ccitt():04X}"
```

### Comparing `zebrafy-1.1.2/zebrafy/graphic_field.py` & `zebrafy-1.1.3/zebrafy/graphic_field.py`

 * *Files 16% similar despite different names*

```diff
@@ -71,42 +71,34 @@
 
     @pil_image.setter
     def pil_image(self, i):
         if not i:
             raise ValueError("Image cannot be empty.")
         if not isinstance(i, Image):
             raise TypeError(
-                "Image must be a valid PIL.Image.Image object. {param_type} was given."
-                .format(param_type=type(i))
+                f"Image must be a valid PIL.Image.Image object. {type(i)} was given."
             )
         self._pil_image = i
 
     format = property(operator.attrgetter("_format"))
 
     @format.setter
     def format(self, f):
         if f is None:
             raise ValueError("Format cannot be empty.")
         if not isinstance(f, str):
-            raise TypeError(
-                "Format must be a valid string. {param_type} was given.".format(
-                    param_type=type(f)
-                )
-            )
+            raise TypeError(f"Format must be a valid string. {type(f)} was given.")
         if f not in ["ASCII", "B64", "Z64"]:
             raise ValueError(
-                'Format type must be "ASCII","B64", or "Z64". {param} was given.'
-                .format(param=f)
+                f'Format type must be "ASCII","B64", or "Z64". {f} was given.'
             )
         self._format = f
 
     def _compression_type_to_format(self, compression_type: str) -> str:
-        """
-        Convert deprecated compression type to format.
-        """
+        """Convert deprecated compression type to format."""
         if compression_type.upper() == "A":
             return "ASCII"
         elif compression_type.upper() == "B":
             return "B64"
         elif compression_type.upper() == "C":
             return "Z64"
 
@@ -178,13 +170,8 @@
 
     def get_graphic_field(self) -> str:
         """
         Get a complete graphic field string for ZPL.
 
         :returns: Complete graphic field string for ZPL.
         """
-        return "^GFA,{bb_count},{gf_count},{bpr},{data}^FS".format(
-            bb_count=self._get_binary_byte_count(),
-            gf_count=self._get_graphic_field_count(),
-            bpr=self._get_bytes_per_row(),
-            data=self._get_data_string(),
-        )
+        return f"^GFA,{self._get_binary_byte_count()},{self._get_graphic_field_count()},{self._get_bytes_per_row()},{self._get_data_string()}^FS"
```

### Comparing `zebrafy-1.1.2/zebrafy/zebrafy_image.py` & `zebrafy-1.1.3/zebrafy/zebrafy_pdf.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,30 +19,27 @@
 #    You should have received a copy of the GNU Lesser General Public License
 #    along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 ########################################################################################
 
 # 1. Standard library imports:
 import operator
-from io import BytesIO
-from typing import Union
 
 # 2. Known third party imports:
-from PIL import Image
+from pypdfium2 import PdfDocument
 
 # 3. Local imports in the relative form:
-from .graphic_field import GraphicField
+from .zebrafy_image import ZebrafyImage
 
 
-class ZebrafyImage:
+class ZebrafyPDF:
     """
-    Provides a method for converting PIL Image or image bytes to Zebra Programming \
-    Language (ZPL).
+    Provides a method for converting PDFs to Zebra Programming Language (ZPL).
 
-    :param image: Image as a PIL Image or bytes object.
+    :param pdf_bytes: PDF as a bytes object.
     :param compression_type (deprecated): ZPL compression type parameter that accepts \
     the following values, defaults to ``"A"``:
 
         - ``"A"``: ASCII hexadecimal - most compatible (default)
         - ``"B"``: Base64 binary
         - ``"C"``: LZ77 / Zlib compressed base64 binary - best compression
     :param format: ZPL format parameter that accepts the following values, \
@@ -50,48 +47,51 @@
 
         - ``"ASCII"``: ASCII hexadecimal - most compatible (default)
         - ``"B64"``: Base64 binary
         - ``"Z64"``: LZ77 / Zlib compressed base64 binary - best compression
     :param invert: Invert the black and white in resulting image, defaults to ``False``
     :param dither: Dither the pixels instead of hard limit on black and white, \
     defaults to ``False``
-    :param threshold: Black pixel threshold for undithered image (``0-255``), defaults \
+    :param threshold: Black pixel threshold for undithered PDF (``0-255``), defaults \
     to ``128``
-    :param width: Width of the image in the resulting ZPL. If ``0``, use default image \
+    :param width: Width of the PDF in the resulting ZPL. If ``0``, use default PDF \
     width, defaults to ``0``
-    :param height: Height of the image in the resulting ZPL. If ``0``, use default \
-    image height, defaults to ``0``
-    :param pos_x: X position of the image on the resulting ZPL, defaults to ``0``
-    :param pos_y: Y position of the image on the resulting ZPL, defaults to ``0``
+    :param height: Height of the PDF in the resulting ZPL. If ``0``, use default \
+    PDF height, defaults to ``0``
+    :param pos_x: X position of the PDF on the resulting ZPL, defaults to ``0``
+    :param pos_y: Y position of the PDF on the resulting ZPL, defaults to ``0``
     :param rotation: Additional rotation in degrees ``0``, ``90``, ``180``, or \
     ``270``, defaults to ``0``
+    :param split_pages: Split each PDF page as a new ZPL label  \
+    (only applies if complete_zpl is set), defaults to ``False``
     :param complete_zpl: Return a complete ZPL with header and footer included. \
     Otherwise return only the graphic field, defaults to ``True``
 
     .. deprecated:: 1.1.0
         The `compression_type` parameter is deprecated in favor of `format` and will \
         be removed in version 2.0.0.
     """
 
     def __init__(
         self,
-        image: Union[bytes, Image.Image],
+        pdf_bytes: bytes,
         compression_type: str = None,
         format: str = None,
         invert: bool = None,
         dither: bool = None,
         threshold: int = None,
         width: int = None,
         height: int = None,
         pos_x: int = None,
         pos_y: int = None,
         rotation: int = None,
+        split_pages: bool = None,
         complete_zpl: bool = None,
     ):
-        self.image = image
+        self.pdf_bytes = pdf_bytes
         if format is None:
             if compression_type is None:
                 format = "ASCII"
             else:
                 format = self._compression_type_to_format(compression_type)
         self.format = format.upper()
         if invert is None:
@@ -114,245 +114,193 @@
         self.pos_x = pos_x
         if pos_y is None:
             pos_y = 0
         self.pos_y = pos_y
         if rotation is None:
             rotation = 0
         self.rotation = rotation
+        if split_pages is None:
+            split_pages = False
+        self.split_pages = split_pages
         if complete_zpl is None:
             complete_zpl = True
         self.complete_zpl = complete_zpl
 
-    image = property(operator.attrgetter("_image"))
+    pdf_bytes = property(operator.attrgetter("_pdf_bytes"))
 
-    @image.setter
-    def image(self, i):
-        if not i:
-            raise ValueError("Image cannot be empty.")
-        if not isinstance(i, bytes) and not isinstance(i, Image.Image):
-            raise TypeError(
-                "Image must be a valid bytes object or PIL.Image.Image object."
-                " {param_type} was given.".format(param_type=type(i))
-            )
-        self._image = i
+    @pdf_bytes.setter
+    def pdf_bytes(self, p):
+        if not p:
+            raise ValueError("PDF cannot be empty.")
+        if not isinstance(p, bytes):
+            raise TypeError(f"PDF must be a valid bytes object {type(p)} was given.")
+        self._pdf_bytes = p
 
     format = property(operator.attrgetter("_format"))
 
     @format.setter
     def format(self, f):
         if f is None:
             raise ValueError("Format cannot be empty.")
         if not isinstance(f, str):
-            raise TypeError(
-                "Format must be a valid string. {param_type} was given.".format(
-                    param_type=type(f)
-                )
-            )
+            raise TypeError(f"Format must be a valid string. {type(f)} was given.")
         if f not in ["ASCII", "B64", "Z64"]:
-            raise ValueError(
-                'Format must be "ASCII","B64", or "Z64". {param} was given.'.format(
-                    param=f
-                )
-            )
+            raise ValueError(f'Format must be "ASCII", "B64", or "Z64". {f} was given.')
         self._format = f
 
     invert = property(operator.attrgetter("_invert"))
 
     @invert.setter
     def invert(self, i):
         if i is None:
             raise ValueError("Invert cannot be empty.")
         if not isinstance(i, bool):
-            raise TypeError(
-                "Invert must be a boolean. {param_type} was given.".format(
-                    param_type=type(i)
-                )
-            )
+            raise TypeError(f"Invert must be a boolean. {type(i)} was given.")
         self._invert = i
 
     dither = property(operator.attrgetter("_dither"))
 
     @dither.setter
     def dither(self, d):
         if d is None:
             raise ValueError("Dither cannot be empty.")
         if not isinstance(d, bool):
-            raise TypeError(
-                "Dither must be a boolean. {param_type} was given.".format(
-                    param_type=type(d)
-                )
-            )
+            raise TypeError(f"Dither must be a boolean. {type(d)} was given.")
         self._dither = d
 
     threshold = property(operator.attrgetter("_threshold"))
 
     @threshold.setter
     def threshold(self, t):
         if t is None:
             raise ValueError("Threshold cannot be empty.")
         if not isinstance(t, int):
-            raise TypeError(
-                "Threshold must be an integer. {param_type} was given.".format(
-                    param_type=type(t)
-                )
-            )
+            raise TypeError(f"Threshold must be an integer. {type(t)} was given.")
         if t < 0 or t > 255:
-            raise ValueError(
-                "Threshold must be within 0 to 255. {param} was given.".format(param=t)
-            )
+            raise ValueError(f"Threshold must be within 0 to 255. {t} was given.")
         self._threshold = t
 
     width = property(operator.attrgetter("_width"))
 
     @width.setter
     def width(self, w):
         if w is None:
             raise ValueError("Width cannot be empty.")
         if not isinstance(w, int):
-            raise TypeError(
-                "Width must be an integer. {param_type} was given.".format(
-                    param_type=type(w)
-                )
-            )
+            raise TypeError(f"Width must be an integer. {type(w)} was given.")
         self._width = w
 
     height = property(operator.attrgetter("_height"))
 
     @height.setter
     def height(self, h):
         if h is None:
             raise ValueError("Height cannot be empty.")
         if not isinstance(h, int):
-            raise TypeError(
-                "Height must be an integer. {param_type} was given.".format(
-                    param_type=type(h)
-                )
-            )
+            raise TypeError(f"Height must be an integer. {type(h)} was given.")
         self._height = h
 
     pos_x = property(operator.attrgetter("_pos_x"))
 
     @pos_x.setter
     def pos_x(self, x):
         if x is None:
             raise ValueError("X position cannot be empty.")
         if not isinstance(x, int):
-            raise TypeError(
-                "X position must be an integer. {param_type} was given.".format(
-                    param_type=type(x)
-                )
-            )
+            raise TypeError(f"X position must be an integer. {type(x)} was given.")
         self._pos_x = x
 
     pos_y = property(operator.attrgetter("_pos_y"))
 
     @pos_y.setter
     def pos_y(self, y):
         if y is None:
             raise ValueError("Y position cannot be empty.")
         if not isinstance(y, int):
-            raise TypeError(
-                "Y position must be an integer. {param_type} was given.".format(
-                    param_type=type(y)
-                )
-            )
+            raise TypeError(f"Y position must be an integer. {type(y)} was given.")
         self._pos_y = y
 
     rotation = property(operator.attrgetter("_rotation"))
 
     @rotation.setter
     def rotation(self, r):
         if r is None:
             raise ValueError("Rotation cannot be empty.")
         if not isinstance(r, int):
-            raise TypeError(
-                "Rotation must be an integer. {param_type} was given.".format(
-                    param_type=type(r)
-                )
-            )
+            raise TypeError(f"Rotation must be an integer. {type(r)} was given.")
         if r not in [0, 90, 180, 270]:
             raise ValueError(
-                'Rotation must be "0", "90", "180" or "270". {param} was given.'.format(
-                    param=r
-                )
+                f'Rotation must be "0", "90", "180" or "270". {r} was given.'
             )
         self._rotation = r
 
+    split_pages = property(operator.attrgetter("_split_pages"))
+
+    @split_pages.setter
+    def split_pages(self, s):
+        if s is None:
+            raise ValueError("Split pages cannot be empty.")
+        if not isinstance(s, bool):
+            raise TypeError(f"Split pages must be a boolean. {type(s)} was given.")
+        self._split_pages = s
+
     complete_zpl = property(operator.attrgetter("_complete_zpl"))
 
     @complete_zpl.setter
     def complete_zpl(self, c):
         if c is None:
             raise ValueError("Complete ZPL cannot be empty.")
         if not isinstance(c, bool):
-            raise TypeError(
-                "Complete ZPL must be a boolean. {param_type} was given.".format(
-                    param_type=type(c)
-                )
-            )
+            raise TypeError(f"Complete ZPL must be a boolean. {type(c)} was given.")
         self._complete_zpl = c
 
     def _compression_type_to_format(self, compression_type: str) -> str:
-        """
-        Convert deprecated compression type to format.
-        """
+        """Convert deprecated compression type to format."""
         if compression_type.upper() == "A":
             return "ASCII"
         elif compression_type.upper() == "B":
             return "B64"
         elif compression_type.upper() == "C":
             return "Z64"
 
     def to_zpl(self) -> str:
         """
-        Converts PIL Image or image bytes to Zebra Programming Language (ZPL).
+        Convert PDF bytes to Zebra Programming Language (ZPL).
 
         :returns: A complete ZPL file string which can be sent to a ZPL compatible \
         printer or a ZPL graphic field if complete_zpl is not set.
         """
-        if isinstance(self._image, bytes):
-            pil_image = Image.open(BytesIO(self._image))
-        else:
-            pil_image = self._image
-
-        # Rotate image based on given parameters
-        if self._rotation:
-            pil_image = pil_image.rotate(self._rotation, expand=False)
-
-        # Resize image if width or height defined in parameters
-        if self._width or self._height:
-            width, height = pil_image.size
-            if self._width:
-                width = self._width
-            if self._height:
-                height = self._height
-            pil_image = pil_image.resize((width, height))
-
-        # Convert image to black and white based on given parameters
-        if self._dither:
-            pil_image = pil_image.convert("1")
-            if self._invert:
-                pil_image = pil_image.point(lambda x: 255 - x)
-        else:
-            pil_image = pil_image.convert("L")
-            pil_image = pil_image.point(
-                lambda x: (
-                    (0 if self._invert else 255)
-                    if x > self._threshold
-                    else (255 if self._invert else 0)
-                ),
-                mode="1",
+        # Open and convert image to grayscale
+        pdf = PdfDocument(self._pdf_bytes)
+        graphic_fields = []
+        for page in pdf:
+            bitmap = page.render(scale=1, rotation=self._rotation)
+            pil_image = bitmap.to_pil()
+            zebrafy_image = ZebrafyImage(
+                pil_image,
+                format=self._format,
+                invert=self._invert,
+                dither=self._dither,
+                threshold=self._threshold,
+                width=self._width,
+                height=self._height,
+                pos_x=self._pos_x,
+                pos_y=self._pos_y,
+                rotation=0,  # Rotation is already handled in the PDF rendering
+                complete_zpl=False,
             )
 
-        graphic_field = GraphicField(pil_image, format=self._format)
+            page_zpl = zebrafy_image.to_zpl() + "\n"
 
-        # Set graphic field position based on given parameters
-        pos = "^FO0,0"
-        if self._pos_x or self._pos_y:
-            pos = "^FO{x},{y}".format(x=self._pos_x, y=self._pos_y)
+            graphic_fields.append(page_zpl)
 
-        # Return complete ZPL with header and footer or only the graphic field based on
-        # given parameters
+        zpl_string = ""
         if self._complete_zpl:
-            return "^XA\n" + pos + graphic_field.get_graphic_field() + "\n^XZ\n"
+            if self._split_pages:
+                for graphic_field in graphic_fields:
+                    zpl_string += "^XA\n" + graphic_field + "^XZ\n"
+            else:
+                zpl_string = "^XA\n" + "".join(graphic_fields) + "^XZ\n"
+        else:
+            zpl_string = "".join(graphic_fields)
 
-        return pos + graphic_field.get_graphic_field()
+        return zpl_string
```

### Comparing `zebrafy-1.1.2/zebrafy/zebrafy_pdf.py` & `zebrafy-1.1.3/zebrafy/zebrafy_image.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,27 +19,29 @@
 #    You should have received a copy of the GNU Lesser General Public License
 #    along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 ########################################################################################
 
 # 1. Standard library imports:
 import operator
+from io import BytesIO
+from typing import Union
 
 # 2. Known third party imports:
-from pypdfium2 import PdfDocument
+from PIL import Image
 
 # 3. Local imports in the relative form:
-from .zebrafy_image import ZebrafyImage
+from .graphic_field import GraphicField
 
 
-class ZebrafyPDF:
+class ZebrafyImage:
     """
-    Provides a method for converting PDFs to Zebra Programming Language (ZPL).
+    Convert a PIL Image or image bytes into Zebra Programming Language (ZPL).
 
-    :param pdf_bytes: PDF as a bytes object.
+    :param image: Image as a PIL Image or bytes object.
     :param compression_type (deprecated): ZPL compression type parameter that accepts \
     the following values, defaults to ``"A"``:
 
         - ``"A"``: ASCII hexadecimal - most compatible (default)
         - ``"B"``: Base64 binary
         - ``"C"``: LZ77 / Zlib compressed base64 binary - best compression
     :param format: ZPL format parameter that accepts the following values, \
@@ -47,51 +49,48 @@
 
         - ``"ASCII"``: ASCII hexadecimal - most compatible (default)
         - ``"B64"``: Base64 binary
         - ``"Z64"``: LZ77 / Zlib compressed base64 binary - best compression
     :param invert: Invert the black and white in resulting image, defaults to ``False``
     :param dither: Dither the pixels instead of hard limit on black and white, \
     defaults to ``False``
-    :param threshold: Black pixel threshold for undithered PDF (``0-255``), defaults \
+    :param threshold: Black pixel threshold for undithered image (``0-255``), defaults \
     to ``128``
-    :param width: Width of the PDF in the resulting ZPL. If ``0``, use default PDF \
+    :param width: Width of the image in the resulting ZPL. If ``0``, use default image \
     width, defaults to ``0``
-    :param height: Height of the PDF in the resulting ZPL. If ``0``, use default \
-    PDF height, defaults to ``0``
-    :param pos_x: X position of the PDF on the resulting ZPL, defaults to ``0``
-    :param pos_y: Y position of the PDF on the resulting ZPL, defaults to ``0``
+    :param height: Height of the image in the resulting ZPL. If ``0``, use default \
+    image height, defaults to ``0``
+    :param pos_x: X position of the image on the resulting ZPL, defaults to ``0``
+    :param pos_y: Y position of the image on the resulting ZPL, defaults to ``0``
     :param rotation: Additional rotation in degrees ``0``, ``90``, ``180``, or \
     ``270``, defaults to ``0``
-    :param split_pages: Split each PDF page as a new ZPL label  \
-    (only applies if complete_zpl is set), defaults to ``False``
     :param complete_zpl: Return a complete ZPL with header and footer included. \
     Otherwise return only the graphic field, defaults to ``True``
 
     .. deprecated:: 1.1.0
         The `compression_type` parameter is deprecated in favor of `format` and will \
         be removed in version 2.0.0.
     """
 
     def __init__(
         self,
-        pdf_bytes: bytes,
+        image: Union[bytes, Image.Image],
         compression_type: str = None,
         format: str = None,
         invert: bool = None,
         dither: bool = None,
         threshold: int = None,
         width: int = None,
         height: int = None,
         pos_x: int = None,
         pos_y: int = None,
         rotation: int = None,
-        split_pages: bool = None,
         complete_zpl: bool = None,
     ):
-        self.pdf_bytes = pdf_bytes
+        self.image = image
         if format is None:
             if compression_type is None:
                 format = "ASCII"
             else:
                 format = self._compression_type_to_format(compression_type)
         self.format = format.upper()
         if invert is None:
@@ -114,251 +113,195 @@
         self.pos_x = pos_x
         if pos_y is None:
             pos_y = 0
         self.pos_y = pos_y
         if rotation is None:
             rotation = 0
         self.rotation = rotation
-        if split_pages is None:
-            split_pages = False
-        self.split_pages = split_pages
         if complete_zpl is None:
             complete_zpl = True
         self.complete_zpl = complete_zpl
 
-    pdf_bytes = property(operator.attrgetter("_pdf_bytes"))
+    image = property(operator.attrgetter("_image"))
 
-    @pdf_bytes.setter
-    def pdf_bytes(self, p):
-        if not p:
-            raise ValueError("PDF cannot be empty.")
-        if not isinstance(p, bytes):
+    @image.setter
+    def image(self, i):
+        if not i:
+            raise ValueError("Image cannot be empty.")
+        if not isinstance(i, bytes) and not isinstance(i, Image.Image):
             raise TypeError(
-                "PDF must be a valid bytes object {param_type} was given.".format(
-                    param_type=type(p)
-                )
+                "Image must be a valid bytes object or PIL.Image.Image object."
+                f" {type(i)} was given."
             )
-        self._pdf_bytes = p
+        self._image = i
 
     format = property(operator.attrgetter("_format"))
 
     @format.setter
     def format(self, f):
         if f is None:
             raise ValueError("Format cannot be empty.")
         if not isinstance(f, str):
-            raise TypeError(
-                "Format must be a valid string. {param_type} was given.".format(
-                    param_type=type(f)
-                )
-            )
+            raise TypeError(f"Format must be a valid string. {type(f)} was given.")
         if f not in ["ASCII", "B64", "Z64"]:
-            raise ValueError(
-                'Format must be "ASCII", "B64", or "Z64". {param} was given.'.format(
-                    param=f
-                )
-            )
+            raise ValueError(f'Format must be "ASCII","B64", or "Z64". {f} was given.')
         self._format = f
 
     invert = property(operator.attrgetter("_invert"))
 
     @invert.setter
     def invert(self, i):
         if i is None:
             raise ValueError("Invert cannot be empty.")
         if not isinstance(i, bool):
-            raise TypeError(
-                "Invert must be a boolean. {param_type} was given.".format(
-                    param_type=type(i)
-                )
-            )
+            raise TypeError(f"Invert must be a boolean. {type(i)} was given.")
         self._invert = i
 
     dither = property(operator.attrgetter("_dither"))
 
     @dither.setter
     def dither(self, d):
         if d is None:
             raise ValueError("Dither cannot be empty.")
         if not isinstance(d, bool):
-            raise TypeError(
-                "Dither must be a boolean. {param_type} was given.".format(
-                    param_type=type(d)
-                )
-            )
+            raise TypeError(f"Dither must be a boolean. {type(d)} was given.")
         self._dither = d
 
     threshold = property(operator.attrgetter("_threshold"))
 
     @threshold.setter
     def threshold(self, t):
         if t is None:
             raise ValueError("Threshold cannot be empty.")
         if not isinstance(t, int):
-            raise TypeError(
-                "Threshold must be an integer. {param_type} was given.".format(
-                    param_type=type(t)
-                )
-            )
+            raise TypeError(f"Threshold must be an integer. {type(t)} was given.")
         if t < 0 or t > 255:
-            raise ValueError(
-                "Threshold must be within 0 to 255. {param} was given.".format(param=t)
-            )
+            raise ValueError(f"Threshold must be within 0 to 255. {t} was given.")
         self._threshold = t
 
     width = property(operator.attrgetter("_width"))
 
     @width.setter
     def width(self, w):
         if w is None:
             raise ValueError("Width cannot be empty.")
         if not isinstance(w, int):
-            raise TypeError(
-                "Width must be an integer. {param_type} was given.".format(
-                    param_type=type(w)
-                )
-            )
+            raise TypeError(f"Width must be an integer. {type(w)} was given.")
         self._width = w
 
     height = property(operator.attrgetter("_height"))
 
     @height.setter
     def height(self, h):
         if h is None:
             raise ValueError("Height cannot be empty.")
         if not isinstance(h, int):
-            raise TypeError(
-                "Height must be an integer. {param_type} was given.".format(
-                    param_type=type(h)
-                )
-            )
+            raise TypeError(f"Height must be an integer. {type(h)} was given.")
         self._height = h
 
     pos_x = property(operator.attrgetter("_pos_x"))
 
     @pos_x.setter
     def pos_x(self, x):
         if x is None:
             raise ValueError("X position cannot be empty.")
         if not isinstance(x, int):
-            raise TypeError(
-                "X position must be an integer. {param_type} was given.".format(
-                    param_type=type(x)
-                )
-            )
+            raise TypeError(f"X position must be an integer. {type(x)} was given.")
         self._pos_x = x
 
     pos_y = property(operator.attrgetter("_pos_y"))
 
     @pos_y.setter
     def pos_y(self, y):
         if y is None:
             raise ValueError("Y position cannot be empty.")
         if not isinstance(y, int):
-            raise TypeError(
-                "Y position must be an integer. {param_type} was given.".format(
-                    param_type=type(y)
-                )
-            )
+            raise TypeError(f"Y position must be an integer. {type(y)} was given.")
         self._pos_y = y
 
     rotation = property(operator.attrgetter("_rotation"))
 
     @rotation.setter
     def rotation(self, r):
         if r is None:
             raise ValueError("Rotation cannot be empty.")
         if not isinstance(r, int):
-            raise TypeError(
-                "Rotation must be an integer. {param_type} was given.".format(
-                    param_type=type(r)
-                )
-            )
+            raise TypeError(f"Rotation must be an integer. {type(r)} was given.")
         if r not in [0, 90, 180, 270]:
             raise ValueError(
-                'Rotation must be "0", "90", "180" or "270". {param} was given.'.format(
-                    param=r
-                )
+                f'Rotation must be "0", "90", "180" or "270". {r} was given.'
             )
         self._rotation = r
 
-    split_pages = property(operator.attrgetter("_split_pages"))
-
-    @split_pages.setter
-    def split_pages(self, s):
-        if s is None:
-            raise ValueError("Split pages cannot be empty.")
-        if not isinstance(s, bool):
-            raise TypeError(
-                "Split pages must be a boolean. {param_type} was given.".format(
-                    param_type=type(s)
-                )
-            )
-        self._split_pages = s
-
     complete_zpl = property(operator.attrgetter("_complete_zpl"))
 
     @complete_zpl.setter
     def complete_zpl(self, c):
         if c is None:
             raise ValueError("Complete ZPL cannot be empty.")
         if not isinstance(c, bool):
-            raise TypeError(
-                "Complete ZPL must be a boolean. {param_type} was given.".format(
-                    param_type=type(c)
-                )
-            )
+            raise TypeError(f"Complete ZPL must be a boolean. {type(c)} was given.")
         self._complete_zpl = c
 
     def _compression_type_to_format(self, compression_type: str) -> str:
-        """
-        Convert deprecated compression type to format.
-        """
+        """Convert deprecated compression type to format."""
         if compression_type.upper() == "A":
             return "ASCII"
         elif compression_type.upper() == "B":
             return "B64"
         elif compression_type.upper() == "C":
             return "Z64"
 
     def to_zpl(self) -> str:
         """
-        Converts PDF bytes to Zebra Programming Language (ZPL).
+        Convert PIL Image or image bytes into Zebra Programming Language (ZPL).
 
         :returns: A complete ZPL file string which can be sent to a ZPL compatible \
         printer or a ZPL graphic field if complete_zpl is not set.
         """
-        # Open and convert image to grayscale
-        pdf = PdfDocument(self._pdf_bytes)
-        graphic_fields = []
-        for page in pdf:
-            bitmap = page.render(scale=1, rotation=self._rotation)
-            pil_image = bitmap.to_pil()
-            zebrafy_image = ZebrafyImage(
-                pil_image,
-                format=self._format,
-                invert=self._invert,
-                dither=self._dither,
-                threshold=self._threshold,
-                width=self._width,
-                height=self._height,
-                pos_x=self._pos_x,
-                pos_y=self._pos_y,
-                rotation=0,  # Rotation is already handled in the PDF rendering
-                complete_zpl=False,
-            )
-
-            page_zpl = zebrafy_image.to_zpl() + "\n"
+        if isinstance(self._image, bytes):
+            pil_image = Image.open(BytesIO(self._image))
+        else:
+            pil_image = self._image
 
-            graphic_fields.append(page_zpl)
+        # Rotate image based on given parameters
+        if self._rotation:
+            pil_image = pil_image.rotate(self._rotation, expand=False)
+
+        # Resize image if width or height defined in parameters
+        if self._width or self._height:
+            width, height = pil_image.size
+            if self._width:
+                width = self._width
+            if self._height:
+                height = self._height
+            pil_image = pil_image.resize((width, height))
+
+        # Convert image to black and white based on given parameters
+        if self._dither:
+            pil_image = pil_image.convert("1")
+            if self._invert:
+                pil_image = pil_image.point(lambda x: 255 - x)
+        else:
+            pil_image = pil_image.convert("L")
+            pil_image = pil_image.point(
+                lambda x: (
+                    (0 if self._invert else 255)
+                    if x > self._threshold
+                    else (255 if self._invert else 0)
+                ),
+                mode="1",
+            )
+
+        graphic_field = GraphicField(pil_image, format=self._format)
+
+        # Set graphic field position based on given parameters
+        pos = "^FO0,0"
+        if self._pos_x or self._pos_y:
+            pos = f"^FO{self._pos_x},{self._pos_y}"
 
-        zpl_string = ""
+        # Return complete ZPL with header and footer or only the graphic field based on
+        # given parameters
         if self._complete_zpl:
-            if self._split_pages:
-                for graphic_field in graphic_fields:
-                    zpl_string += "^XA\n" + graphic_field + "^XZ\n"
-            else:
-                zpl_string = "^XA\n" + "".join(graphic_fields) + "^XZ\n"
-        else:
-            zpl_string = "".join(graphic_fields)
+            return "^XA\n" + pos + graphic_field.get_graphic_field() + "\n^XZ\n"
 
-        return zpl_string
+        return pos + graphic_field.get_graphic_field()
```

### Comparing `zebrafy-1.1.2/zebrafy/zebrafy_zpl.py` & `zebrafy-1.1.3/zebrafy/zebrafy_zpl.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,16 +48,15 @@
 
     ToImagesType = List[Image.Image]
     DimensionsType = Tuple[int, int]
 
 
 class ZebrafyZPL:
     """
-    Provides a method for converting Zebra Programming Language (ZPL) graphic fields \
-    to PDF and images.
+    Convert Zebra Programming Language (ZPL) graphic fields to PDF and images.
 
     :param zpl_data: A valid ZPL string.
     """
 
     def __init__(self, zpl_data: str):
         self.zpl_data = zpl_data
 
@@ -65,35 +64,32 @@
 
     @zpl_data.setter
     def zpl_data(self, d):
         if d is None:
             raise ValueError("ZPL data cannot be empty.")
         if not isinstance(d, str):
             raise TypeError(
-                "ZPL data must be a valid ZPL string. {param_type} was given.".format(
-                    param_type=type(d)
-                )
+                f"ZPL data must be a valid ZPL string. {type(d)} was given."
             )
         self._zpl_data = d
 
     def _match_dimensions(self, total: int, width: int) -> DimensionsType:
         """
         Get image dimensions from ZPL graphic field.
 
         :param total: Total number of bytes comprising the graphic format.
         :param width: Total number of bytes comprising one row of the data.
         :returns: A tuple of integers containing the width and height of the \
         graphic field image.
         """
-
         return int(width * 8), int(total / width)
 
     def to_images(self) -> ToImagesType:
         """
-        Converts Zebra Programming Language (ZPL) graphic fields to PIL Image objects.
+        Convert Zebra Programming Language (ZPL) graphic fields to PIL Image objects.
 
         :returns: A list containing PIL Images converted from ZPL graphic fields.
         """
         matches = GF_MATCHER.findall(self._zpl_data)
         if not matches:
             raise ValueError("Could not find a graphic field (^GF) in ZPL content.")
 
@@ -130,15 +126,15 @@
             pil_image = Image.frombytes("1", (width, height), data_bytes)
             pil_images.append(pil_image)
 
         return pil_images
 
     def to_pdf(self) -> bytes:
         """
-        Converts Zebra Programming Language (ZPL) graphic fields to PDF.
+        Convert Zebra Programming Language (ZPL) graphic fields to PDF.
 
         :returns: PDF bytes from ZPL graphic fields.
         """
         pil_images = self.to_images()
         pdf = PdfDocument.new()
 
         for pil_image in pil_images:
```

### Comparing `zebrafy-1.1.2/zebrafy.egg-info/PKG-INFO` & `zebrafy-1.1.3/zebrafy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zebrafy
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python library for converting PDF and images to Zebra Programming Language (ZPL)
 Author-email: Miika Nissi <miika@miikanissi.com>
 Maintainer-email: Miika Nissi <miika@miikanissi.com>
 License: LGPLv3
 Project-URL: Homepage, https://github.com/miikanissi/zebrafy/
 Project-URL: Documentation, https://zebrafy.readthedocs.io/
 Classifier: Development Status :: 4 - Beta
@@ -22,21 +22,23 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Manufacturing
 Classifier: Topic :: Printing
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: pillow
-Requires-Dist: pypdfium2<=4.18.0
+Requires-Dist: pypdfium2>=4.8.0
+Provides-Extra: docs
+Requires-Dist: sphinx>=7.0.0; extra == "docs"
+Requires-Dist: sphinx_autodoc_typehints>=2.0.0; extra == "docs"
+Requires-Dist: sphinx_rtd_theme>=2.0.0; extra == "docs"
 Provides-Extra: test
 Requires-Dist: pytest-cov; extra == "test"
-Provides-Extra: dev
-Requires-Dist: sphinx; extra == "dev"
-Requires-Dist: sphinx_autodoc_typehints; extra == "dev"
-Requires-Dist: sphinx_rtd_theme>=1.2.0; extra == "dev"
+Provides-Extra: lint
+Requires-Dist: pre-commit; extra == "lint"
 
 |zebrafy_icon_64| Zebrafy
 =========================
 
 .. |zebrafy_icon_64| image:: https://raw.githubusercontent.com/miikanissi/zebrafy/master/docs/zebrafy-64.png
    :alt: Zebrafy Logo
```


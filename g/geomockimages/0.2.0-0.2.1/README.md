# Comparing `tmp/geomockimages-0.2.0.tar.gz` & `tmp/geomockimages-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomockimages-0.2.0.tar", max compression
+gzip compressed data, was "geomockimages-0.2.1.tar", max compression
```

## Comparing `geomockimages-0.2.0.tar` & `geomockimages-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1061 2024-04-19 06:06:31.014821 geomockimages-0.2.0/LICENSE
--rw-r--r--   0        0        0     1929 2024-05-22 10:13:58.232756 geomockimages-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-04-19 07:17:28.778191 geomockimages-0.2.0/geomockimages/__init__.py
--rw-r--r--   0        0        0    14041 2024-05-22 10:13:58.233715 geomockimages-0.2.0/geomockimages/imagecreator.py
--rw-r--r--   0        0        0      923 2024-04-19 07:17:28.779244 geomockimages-0.2.0/geomockimages/logging.py
--rw-r--r--   0        0        0     1511 2024-05-20 08:53:13.724556 geomockimages-0.2.0/geomockimages/raster.py
--rw-r--r--   0        0        0        0 2024-04-19 07:17:28.779518 geomockimages-0.2.0/geomockimages/test/__init__.py
--rw-r--r--   0        0        0     5462 2024-05-22 10:13:58.234271 geomockimages-0.2.0/geomockimages/test/test_geomockimages.py
--rw-r--r--   0        0        0      689 2024-05-22 11:19:22.352422 geomockimages-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 geomockimages-0.2.0/setup.py
--rw-r--r--   0        0        0     2637 1970-01-01 00:00:00.000000 geomockimages-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-04-19 06:06:31.014821 geomockimages-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1893 2024-05-24 04:21:06.692977 geomockimages-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 07:17:28.778191 geomockimages-0.2.1/geomockimages/__init__.py
+-rw-r--r--   0        0        0    14041 2024-05-22 10:13:58.233715 geomockimages-0.2.1/geomockimages/imagecreator.py
+-rw-r--r--   0        0        0      923 2024-04-19 07:17:28.779244 geomockimages-0.2.1/geomockimages/logging.py
+-rw-r--r--   0        0        0     1511 2024-05-20 08:53:13.724556 geomockimages-0.2.1/geomockimages/raster.py
+-rw-r--r--   0        0        0        0 2024-04-19 07:17:28.779518 geomockimages-0.2.1/geomockimages/test/__init__.py
+-rw-r--r--   0        0        0     5462 2024-05-22 10:13:58.234271 geomockimages-0.2.1/geomockimages/test/test_geomockimages.py
+-rw-r--r--   0        0        0      689 2024-05-24 04:23:16.899744 geomockimages-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2787 1970-01-01 00:00:00.000000 geomockimages-0.2.1/setup.py
+-rw-r--r--   0        0        0     2601 1970-01-01 00:00:00.000000 geomockimages-0.2.1/PKG-INFO
```

### Comparing `geomockimages-0.2.0/LICENSE` & `geomockimages-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geomockimages-0.2.0/README.md` & `geomockimages-0.2.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,11 @@
-# fake-geo-images
+# geomockimages
 
 A module to programmatically create geotiff images which can be used for unit tests.
 
-<p align="center">
-    <img src="./coverage.svg">
-</p>
-
 The underlying idea is that in order to write unit tests for geospatial image processsing algorithms,
 it is necessary to have an actual input image file or array. Organising these test images becomes a chore over time,
 they should not be stored in git as they are large binary data and when stored outside, there always
 is the danger that they are not updated according to changes in the code repo.
 
 **geomockimages** provides a solution to the problem by providing simple code that allows to create
 geospatial images (so far geotiffs) in a parameterised way.
@@ -31,22 +27,22 @@
 ```python
 import numpy as np
 import rasterio as rio
 from pathlib import Path
 
 from rasterio.transform import from_origin
 from my_image_processing import ndvi
-from fake_geo_images.fakegeoimages import FakeGeoImage
+from geomockimages.imagecreator import GeoMockImage
 
 def test_ndvi():
     """
     A unit test if an NDVI method works in general
     """
     # Create 4-band image simulating RGBN as needed for NDVI
-    test_image, _ = FakeGeoImage(
+    test_image, _ = GeoMockImage(
         300,
         150,
         4,
         "uint16",
         out_dir=Path("/tmp"),
         crs=4326,
         nodata=0,
@@ -55,14 +51,14 @@
     ).create(seed=42, transform=from_origin(13.428596, 52.494384, 0.000006, 0.000006))
 
     ndvi_image = ndvi(test_image)
 
     with rio.open(str(ndvi_image)) as src:
         ndvi_array = src.read()
         # NDVI only has one band of same size as input bands
-        assert ndvi_array.shape == (1, 300, 150)
+        assert ndvi_array.shape == (1, 150, 300)
         # NDVI has float values between -1 and 1
-        assert ndvi_array.dtype == np.float
-        assert ndvi_array.min >= -1
-        assert ndvi_array.max <= 1
+        assert ndvi_array.dtype == np.dtype('float32')
+        assert np.nanmin(ndvi_array) >= -1
+        assert np.nanmax(ndvi_array) <= 1
 
 ```
```

### Comparing `geomockimages-0.2.0/geomockimages/imagecreator.py` & `geomockimages-0.2.1/geomockimages/imagecreator.py`

 * *Files identical despite different names*

### Comparing `geomockimages-0.2.0/geomockimages/logging.py` & `geomockimages-0.2.1/geomockimages/logging.py`

 * *Files identical despite different names*

### Comparing `geomockimages-0.2.0/geomockimages/raster.py` & `geomockimages-0.2.1/geomockimages/raster.py`

 * *Files identical despite different names*

### Comparing `geomockimages-0.2.0/geomockimages/test/test_geomockimages.py` & `geomockimages-0.2.1/geomockimages/test/test_geomockimages.py`

 * *Files identical despite different names*

### Comparing `geomockimages-0.2.0/pyproject.toml` & `geomockimages-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geomockimages"
-version = "0.2.0"
+version = "0.2.1"
 description = "A module to programmatically create geotiff images which can be used for unit tests."
 authors = ["Markus Müller <markus.u.mueller@zoho.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `geomockimages-0.2.0/setup.py` & `geomockimages-0.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  'rasterio>=1.3.10,<2.0.0',
  'rio-cogeo>=5.3.0,<6.0.0',
  'scikit-image>=0.23.2,<0.24.0',
  'scipy>=1.13.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'geomockimages',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'A module to programmatically create geotiff images which can be used for unit tests.',
-    'long_description': '# fake-geo-images\n\nA module to programmatically create geotiff images which can be used for unit tests.\n\n<p align="center">\n    <img src="./coverage.svg">\n</p>\n\nThe underlying idea is that in order to write unit tests for geospatial image processsing algorithms,\nit is necessary to have an actual input image file or array. Organising these test images becomes a chore over time,\nthey should not be stored in git as they are large binary data and when stored outside, there always\nis the danger that they are not updated according to changes in the code repo.\n\n**geomockimages** provides a solution to the problem by providing simple code that allows to create\ngeospatial images (so far geotiffs) in a parameterised way.\n\n## Install package\n```bash\npip install geomockimages\n```\n\n## Run tests\n```bash\npytest\n```\n\n## Usage\n\nIn the following an example unit test for a hypothetical NDVI function.\n\n```python\nimport numpy as np\nimport rasterio as rio\nfrom pathlib import Path\n\nfrom rasterio.transform import from_origin\nfrom my_image_processing import ndvi\nfrom fake_geo_images.fakegeoimages import FakeGeoImage\n\ndef test_ndvi():\n    """\n    A unit test if an NDVI method works in general\n    """\n    # Create 4-band image simulating RGBN as needed for NDVI\n    test_image, _ = FakeGeoImage(\n        300,\n        150,\n        4,\n        "uint16",\n        out_dir=Path("/tmp"),\n        crs=4326,\n        nodata=0,\n        nodata_fill=3,\n        cog=False,\n    ).create(seed=42, transform=from_origin(13.428596, 52.494384, 0.000006, 0.000006))\n\n    ndvi_image = ndvi(test_image)\n\n    with rio.open(str(ndvi_image)) as src:\n        ndvi_array = src.read()\n        # NDVI only has one band of same size as input bands\n        assert ndvi_array.shape == (1, 300, 150)\n        # NDVI has float values between -1 and 1\n        assert ndvi_array.dtype == np.float\n        assert ndvi_array.min >= -1\n        assert ndvi_array.max <= 1\n\n```\n',
+    'long_description': '# geomockimages\n\nA module to programmatically create geotiff images which can be used for unit tests.\n\nThe underlying idea is that in order to write unit tests for geospatial image processsing algorithms,\nit is necessary to have an actual input image file or array. Organising these test images becomes a chore over time,\nthey should not be stored in git as they are large binary data and when stored outside, there always\nis the danger that they are not updated according to changes in the code repo.\n\n**geomockimages** provides a solution to the problem by providing simple code that allows to create\ngeospatial images (so far geotiffs) in a parameterised way.\n\n## Install package\n```bash\npip install geomockimages\n```\n\n## Run tests\n```bash\npytest\n```\n\n## Usage\n\nIn the following an example unit test for a hypothetical NDVI function.\n\n```python\nimport numpy as np\nimport rasterio as rio\nfrom pathlib import Path\n\nfrom rasterio.transform import from_origin\nfrom my_image_processing import ndvi\nfrom geomockimages.imagecreator import GeoMockImage\n\ndef test_ndvi():\n    """\n    A unit test if an NDVI method works in general\n    """\n    # Create 4-band image simulating RGBN as needed for NDVI\n    test_image, _ = GeoMockImage(\n        300,\n        150,\n        4,\n        "uint16",\n        out_dir=Path("/tmp"),\n        crs=4326,\n        nodata=0,\n        nodata_fill=3,\n        cog=False,\n    ).create(seed=42, transform=from_origin(13.428596, 52.494384, 0.000006, 0.000006))\n\n    ndvi_image = ndvi(test_image)\n\n    with rio.open(str(ndvi_image)) as src:\n        ndvi_array = src.read()\n        # NDVI only has one band of same size as input bands\n        assert ndvi_array.shape == (1, 150, 300)\n        # NDVI has float values between -1 and 1\n        assert ndvi_array.dtype == np.dtype(\'float32\')\n        assert np.nanmin(ndvi_array) >= -1\n        assert np.nanmax(ndvi_array) <= 1\n\n```\n',
     'author': 'Markus Müller',
     'author_email': 'markus.u.mueller@zoho.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `geomockimages-0.2.0/PKG-INFO` & `geomockimages-0.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomockimages
-Version: 0.2.0
+Version: 0.2.1
 Summary: A module to programmatically create geotiff images which can be used for unit tests.
 License: MIT
 Author: Markus Müller
 Author-email: markus.u.mueller@zoho.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,22 +13,18 @@
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: rasterio (>=1.3.10,<2.0.0)
 Requires-Dist: rio-cogeo (>=5.3.0,<6.0.0)
 Requires-Dist: scikit-image (>=0.23.2,<0.24.0)
 Requires-Dist: scipy (>=1.13.0,<2.0.0)
 Description-Content-Type: text/markdown
 
-# fake-geo-images
+# geomockimages
 
 A module to programmatically create geotiff images which can be used for unit tests.
 
-<p align="center">
-    <img src="./coverage.svg">
-</p>
-
 The underlying idea is that in order to write unit tests for geospatial image processsing algorithms,
 it is necessary to have an actual input image file or array. Organising these test images becomes a chore over time,
 they should not be stored in git as they are large binary data and when stored outside, there always
 is the danger that they are not updated according to changes in the code repo.
 
 **geomockimages** provides a solution to the problem by providing simple code that allows to create
 geospatial images (so far geotiffs) in a parameterised way.
@@ -50,22 +46,22 @@
 ```python
 import numpy as np
 import rasterio as rio
 from pathlib import Path
 
 from rasterio.transform import from_origin
 from my_image_processing import ndvi
-from fake_geo_images.fakegeoimages import FakeGeoImage
+from geomockimages.imagecreator import GeoMockImage
 
 def test_ndvi():
     """
     A unit test if an NDVI method works in general
     """
     # Create 4-band image simulating RGBN as needed for NDVI
-    test_image, _ = FakeGeoImage(
+    test_image, _ = GeoMockImage(
         300,
         150,
         4,
         "uint16",
         out_dir=Path("/tmp"),
         crs=4326,
         nodata=0,
@@ -74,15 +70,15 @@
     ).create(seed=42, transform=from_origin(13.428596, 52.494384, 0.000006, 0.000006))
 
     ndvi_image = ndvi(test_image)
 
     with rio.open(str(ndvi_image)) as src:
         ndvi_array = src.read()
         # NDVI only has one band of same size as input bands
-        assert ndvi_array.shape == (1, 300, 150)
+        assert ndvi_array.shape == (1, 150, 300)
         # NDVI has float values between -1 and 1
-        assert ndvi_array.dtype == np.float
-        assert ndvi_array.min >= -1
-        assert ndvi_array.max <= 1
+        assert ndvi_array.dtype == np.dtype('float32')
+        assert np.nanmin(ndvi_array) >= -1
+        assert np.nanmax(ndvi_array) <= 1
 
 ```
```


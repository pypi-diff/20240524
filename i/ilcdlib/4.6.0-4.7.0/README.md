# Comparing `tmp/ilcdlib-4.6.0.tar.gz` & `tmp/ilcdlib-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilcdlib-4.6.0.tar", max compression
+gzip compressed data, was "ilcdlib-4.7.0.tar", max compression
```

## Comparing `ilcdlib-4.6.0.tar` & `ilcdlib-4.7.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0    11357 2024-05-17 16:43:43.172562 ilcdlib-4.6.0/LICENSE
--rw-r--r--   0        0        0     4949 2024-05-17 16:43:43.172562 ilcdlib-4.6.0/README.md
--rw-r--r--   0        0        0     3525 2024-05-17 16:43:43.172562 ilcdlib-4.6.0/pyproject.toml
--rw-r--r--   0        0        0      837 2024-05-17 16:43:43.172562 ilcdlib-4.6.0/src/ilcdlib/__init__.py
--rw-r--r--   0        0        0      910 2024-05-17 16:43:43.172562 ilcdlib-4.6.0/src/ilcdlib/__main__.py
--rw-r--r--   0        0        0      855 2024-05-17 16:43:43.172562 ilcdlib-4.6.0/src/ilcdlib/__version__.py
--rw-r--r--   0        0        0     2959 2024-05-17 16:43:43.172562 ilcdlib-4.6.0/src/ilcdlib/cli.py
--rw-r--r--   0        0        0    19110 2024-05-17 16:43:43.172562 ilcdlib-4.6.0/src/ilcdlib/common.py
--rw-r--r--   0        0        0      837 2024-05-17 16:43:43.172562 ilcdlib-4.6.0/src/ilcdlib/compat/__init__.py
--rw-r--r--   0        0        0     1158 2024-05-17 16:43:43.172562 ilcdlib-4.6.0/src/ilcdlib/compat/pydantic.py
--rw-r--r--   0        0        0     1835 2024-05-17 16:43:43.172562 ilcdlib-4.6.0/src/ilcdlib/const.py
--rw-r--r--   0        0        0     4934 2024-05-17 16:43:43.172562 ilcdlib-4.6.0/src/ilcdlib/data/category_mapping/epdnorge.csv
--rw-r--r--   0        0        0    51577 2024-05-17 16:43:43.172562 ilcdlib-4.6.0/src/ilcdlib/data/category_mapping/oekobaudat.csv
--rw-r--r--   0        0        0   172140 2024-05-17 16:43:43.172562 ilcdlib-4.6.0/src/ilcdlib/data/ilcd_epd_ref.zip
--rw-r--r--   0        0        0     6488 2024-05-17 16:43:43.172562 ilcdlib-4.6.0/src/ilcdlib/dto.py
--rw-r--r--   0        0        0      837 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/entity/__init__.py
--rw-r--r--   0        0        0     7064 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/entity/base_scope_set_reader.py
--rw-r--r--   0        0        0     3361 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/entity/category.py
--rw-r--r--   0        0        0     3052 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/entity/compliance.py
--rw-r--r--   0        0        0     6003 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/entity/contact.py
--rw-r--r--   0        0        0     4173 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/entity/exchage.py
--rw-r--r--   0        0        0     8138 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/entity/flow.py
--rw-r--r--   0        0        0     4224 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/entity/lcia.py
--rw-r--r--   0        0        0     5213 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/entity/material.py
--rw-r--r--   0        0        0     3930 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/entity/pcr.py
--rw-r--r--   0        0        0     3437 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/entity/source.py
--rw-r--r--   0        0        0     3788 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/entity/unit.py
--rw-r--r--   0        0        0     3331 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/entity/validation.py
--rw-r--r--   0        0        0      837 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/epd/__init__.py
--rw-r--r--   0        0        0    10064 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/epd/cli.py
--rw-r--r--   0        0        0      837 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/epd/dialect/__init__.py
--rw-r--r--   0        0        0     6864 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/epd/dialect/environdec.py
--rw-r--r--   0        0        0     2170 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/epd/dialect/epditaly.py
--rw-r--r--   0        0        0     4680 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/epd/dialect/epdnorge.py
--rw-r--r--   0        0        0     1329 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/epd/dialect/indata.py
--rw-r--r--   0        0        0     2326 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/epd/dialect/itb.py
--rw-r--r--   0        0        0     3876 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/epd/dialect/oekobaudat.py
--rw-r--r--   0        0        0     3644 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/epd/factory.py
--rw-r--r--   0        0        0    35487 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/epd/reader.py
--rw-r--r--   0        0        0     2248 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/extension.py
--rw-r--r--   0        0        0     7895 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/http_common.py
--rw-r--r--   0        0        0      837 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/mapping/__init__.py
--rw-r--r--   0        0        0    10680 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/mapping/category.py
--rw-r--r--   0        0        0     3603 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/mapping/common.py
--rw-r--r--   0        0        0     1168 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/mapping/compliance.py
--rw-r--r--   0        0        0     1512 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/mapping/flows.py
--rw-r--r--   0        0        0     3538 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/mapping/impacts.py
--rw-r--r--   0        0        0     1651 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/mapping/indicators.py
--rw-r--r--   0        0        0     1212 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/mapping/properties.py
--rw-r--r--   0        0        0     6247 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/mapping/units.py
--rw-r--r--   0        0        0      837 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/medium/__init__.py
--rw-r--r--   0        0        0     7531 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/medium/archive.py
--rw-r--r--   0        0        0     6496 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/medium/soda4lca.py
--rw-r--r--   0        0        0        0 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/py.typed
--rw-r--r--   0        0        0     1435 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/reference_data.py
--rw-r--r--   0        0        0      837 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/sanitizing/__init__.py
--rw-r--r--   0        0        0     1866 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/sanitizing/domain.py
--rw-r--r--   0        0        0     1336 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/sanitizing/phone.py
--rw-r--r--   0        0        0     1122 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/sanitizing/text.py
--rw-r--r--   0        0        0      837 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/soda4lca/__init__.py
--rw-r--r--   0        0        0    11347 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/soda4lca/api_client.py
--rw-r--r--   0        0        0     2755 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/soda4lca/api_client_4x.py
--rw-r--r--   0        0        0     1206 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/type.py
--rw-r--r--   0        0        0     6465 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/utils.py
--rw-r--r--   0        0        0     2399 2024-05-17 16:43:43.176561 ilcdlib-4.6.0/src/ilcdlib/xml_parser.py
--rw-r--r--   0        0        0     6082 1970-01-01 00:00:00.000000 ilcdlib-4.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-24 03:16:30.801500 ilcdlib-4.7.0/LICENSE
+-rw-r--r--   0        0        0     4949 2024-05-24 03:16:30.801500 ilcdlib-4.7.0/README.md
+-rw-r--r--   0        0        0     3525 2024-05-24 03:16:30.801500 ilcdlib-4.7.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2024-05-24 03:16:30.801500 ilcdlib-4.7.0/src/ilcdlib/__init__.py
+-rw-r--r--   0        0        0      910 2024-05-24 03:16:30.801500 ilcdlib-4.7.0/src/ilcdlib/__main__.py
+-rw-r--r--   0        0        0      855 2024-05-24 03:16:30.801500 ilcdlib-4.7.0/src/ilcdlib/__version__.py
+-rw-r--r--   0        0        0     2959 2024-05-24 03:16:30.801500 ilcdlib-4.7.0/src/ilcdlib/cli.py
+-rw-r--r--   0        0        0    19110 2024-05-24 03:16:30.801500 ilcdlib-4.7.0/src/ilcdlib/common.py
+-rw-r--r--   0        0        0      837 2024-05-24 03:16:30.801500 ilcdlib-4.7.0/src/ilcdlib/compat/__init__.py
+-rw-r--r--   0        0        0     1158 2024-05-24 03:16:30.801500 ilcdlib-4.7.0/src/ilcdlib/compat/pydantic.py
+-rw-r--r--   0        0        0     1835 2024-05-24 03:16:30.801500 ilcdlib-4.7.0/src/ilcdlib/const.py
+-rw-r--r--   0        0        0     4934 2024-05-24 03:16:30.801500 ilcdlib-4.7.0/src/ilcdlib/data/category_mapping/epdnorge.csv
+-rw-r--r--   0        0        0    51577 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/data/category_mapping/oekobaudat.csv
+-rw-r--r--   0        0        0   172140 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/data/ilcd_epd_ref.zip
+-rw-r--r--   0        0        0     6488 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/dto.py
+-rw-r--r--   0        0        0      837 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/entity/__init__.py
+-rw-r--r--   0        0        0     7064 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/entity/base_scope_set_reader.py
+-rw-r--r--   0        0        0     3361 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/entity/category.py
+-rw-r--r--   0        0        0     3052 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/entity/compliance.py
+-rw-r--r--   0        0        0     6003 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/entity/contact.py
+-rw-r--r--   0        0        0     4173 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/entity/exchage.py
+-rw-r--r--   0        0        0     8138 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/entity/flow.py
+-rw-r--r--   0        0        0     4224 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/entity/lcia.py
+-rw-r--r--   0        0        0     5213 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/entity/material.py
+-rw-r--r--   0        0        0     3930 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/entity/pcr.py
+-rw-r--r--   0        0        0     3437 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/entity/source.py
+-rw-r--r--   0        0        0     3788 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/entity/unit.py
+-rw-r--r--   0        0        0     3326 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/entity/validation.py
+-rw-r--r--   0        0        0      837 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/epd/__init__.py
+-rw-r--r--   0        0        0    10064 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/epd/cli.py
+-rw-r--r--   0        0        0      837 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/epd/dialect/__init__.py
+-rw-r--r--   0        0        0     6864 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/epd/dialect/environdec.py
+-rw-r--r--   0        0        0     2170 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/epd/dialect/epditaly.py
+-rw-r--r--   0        0        0     5947 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/epd/dialect/epdnorge.py
+-rw-r--r--   0        0        0     1329 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/epd/dialect/indata.py
+-rw-r--r--   0        0        0     2326 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/epd/dialect/itb.py
+-rw-r--r--   0        0        0     3876 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/epd/dialect/oekobaudat.py
+-rw-r--r--   0        0        0     3644 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/epd/factory.py
+-rw-r--r--   0        0        0    35487 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/epd/reader.py
+-rw-r--r--   0        0        0     2248 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/extension.py
+-rw-r--r--   0        0        0     7895 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/http_common.py
+-rw-r--r--   0        0        0      837 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/mapping/__init__.py
+-rw-r--r--   0        0        0    10680 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/mapping/category.py
+-rw-r--r--   0        0        0     3603 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/mapping/common.py
+-rw-r--r--   0        0        0     1168 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/mapping/compliance.py
+-rw-r--r--   0        0        0     1512 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/mapping/flows.py
+-rw-r--r--   0        0        0     3538 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/mapping/impacts.py
+-rw-r--r--   0        0        0     1651 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/mapping/indicators.py
+-rw-r--r--   0        0        0     1212 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/mapping/properties.py
+-rw-r--r--   0        0        0     6247 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/mapping/units.py
+-rw-r--r--   0        0        0      837 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/medium/__init__.py
+-rw-r--r--   0        0        0     7531 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/medium/archive.py
+-rw-r--r--   0        0        0     6496 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/medium/soda4lca.py
+-rw-r--r--   0        0        0        0 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/py.typed
+-rw-r--r--   0        0        0     1435 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/reference_data.py
+-rw-r--r--   0        0        0      837 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/sanitizing/__init__.py
+-rw-r--r--   0        0        0     1866 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/sanitizing/domain.py
+-rw-r--r--   0        0        0     1336 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/sanitizing/phone.py
+-rw-r--r--   0        0        0     1122 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/sanitizing/text.py
+-rw-r--r--   0        0        0      837 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/soda4lca/__init__.py
+-rw-r--r--   0        0        0    11347 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/soda4lca/api_client.py
+-rw-r--r--   0        0        0     2755 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/soda4lca/api_client_4x.py
+-rw-r--r--   0        0        0     1206 2024-05-24 03:16:30.805500 ilcdlib-4.7.0/src/ilcdlib/type.py
+-rw-r--r--   0        0        0     6465 2024-05-24 03:16:30.809500 ilcdlib-4.7.0/src/ilcdlib/utils.py
+-rw-r--r--   0        0        0     2399 2024-05-24 03:16:30.809500 ilcdlib-4.7.0/src/ilcdlib/xml_parser.py
+-rw-r--r--   0        0        0     6082 1970-01-01 00:00:00.000000 ilcdlib-4.7.0/PKG-INFO
```

### Comparing `ilcdlib-4.6.0/LICENSE` & `ilcdlib-4.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/README.md` & `ilcdlib-4.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/pyproject.toml` & `ilcdlib-4.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ilcdlib"
-version = "4.6.0"
+version = "4.7.0"
 license = "Apache-2.0"
 description = "A toolkit for reading and writing ILCD format and it's derivatives"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <open-source@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/ilcdlib"
 keywords = []
 classifiers = [
```

### Comparing `ilcdlib-4.6.0/src/ilcdlib/__init__.py` & `ilcdlib-4.7.0/src/ilcdlib/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/__main__.py` & `ilcdlib-4.7.0/src/ilcdlib/__main__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/__version__.py` & `ilcdlib-4.7.0/src/ilcdlib/__version__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/cli.py` & `ilcdlib-4.7.0/src/ilcdlib/cli.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/common.py` & `ilcdlib-4.7.0/src/ilcdlib/common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/compat/__init__.py` & `ilcdlib-4.7.0/src/ilcdlib/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/compat/pydantic.py` & `ilcdlib-4.7.0/src/ilcdlib/compat/pydantic.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/const.py` & `ilcdlib-4.7.0/src/ilcdlib/const.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/data/category_mapping/epdnorge.csv` & `ilcdlib-4.7.0/src/ilcdlib/data/category_mapping/epdnorge.csv`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/data/category_mapping/oekobaudat.csv` & `ilcdlib-4.7.0/src/ilcdlib/data/category_mapping/oekobaudat.csv`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/data/ilcd_epd_ref.zip` & `ilcdlib-4.7.0/src/ilcdlib/data/ilcd_epd_ref.zip`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/dto.py` & `ilcdlib-4.7.0/src/ilcdlib/dto.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/entity/__init__.py` & `ilcdlib-4.7.0/src/ilcdlib/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/entity/base_scope_set_reader.py` & `ilcdlib-4.7.0/src/ilcdlib/entity/base_scope_set_reader.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/entity/category.py` & `ilcdlib-4.7.0/src/ilcdlib/entity/category.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/entity/compliance.py` & `ilcdlib-4.7.0/src/ilcdlib/entity/compliance.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/entity/contact.py` & `ilcdlib-4.7.0/src/ilcdlib/entity/contact.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/entity/exchage.py` & `ilcdlib-4.7.0/src/ilcdlib/entity/exchage.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/entity/flow.py` & `ilcdlib-4.7.0/src/ilcdlib/entity/flow.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/entity/lcia.py` & `ilcdlib-4.7.0/src/ilcdlib/entity/lcia.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/entity/material.py` & `ilcdlib-4.7.0/src/ilcdlib/entity/material.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/entity/pcr.py` & `ilcdlib-4.7.0/src/ilcdlib/entity/pcr.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/entity/source.py` & `ilcdlib-4.7.0/src/ilcdlib/entity/source.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/entity/unit.py` & `ilcdlib-4.7.0/src/ilcdlib/entity/unit.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/entity/validation.py` & `ilcdlib-4.7.0/src/ilcdlib/entity/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,26 +35,26 @@
         self,
         element: T_ET.Element,
         data_provider: BaseIlcdMediumSpecificReader,
         *,
         contact_reader_cls: Type[IlcdContactReader] = IlcdContactReader,
     ):
         super().__init__(data_provider)
-        self._entity = element
+        self.entity = element
         self.contact_reader_cls = contact_reader_cls
 
     def get_validation(
         self, lang: LangDef, base_url: str | None = None, provider_domain: str | None = None
     ) -> ValidationDto | None:
         """Return single validation entity."""
-        tree = self._get_external_tree(self._entity, ("common:referenceToNameOfReviewerAndInstitution",))
+        tree = self._get_external_tree(self.entity, ("common:referenceToNameOfReviewerAndInstitution",))
         if tree is None:
             return None
         if contact := self.contact_reader_cls(tree, self.data_provider):
-            review_type = self._entity.attrib.get("type")
+            review_type = self.entity.attrib.get("type")
             validation = ValidationDto(
                 validation_type=IlcdTypeOfReview(review_type) if review_type else None,
                 org=contact.to_openepd_org(lang, base_url, provider_domain),
             )
             return validation
         return None
 
@@ -66,20 +66,20 @@
         self,
         element: T_ET.Element,
         data_provider: BaseIlcdMediumSpecificReader,
         *,
         validation_reader_cls: Type[IlcdValidationReader] = IlcdValidationReader,
     ):
         super().__init__(data_provider)
-        self._entity = element
+        self.entity = element
         self.validation_reader_cls = validation_reader_cls
 
     def get_validations(
         self, lang: LangDef, base_url: str | None = None, provider_domain: str | None = None
     ) -> list[ValidationDto]:
         """Return all validation data."""
         result = []
-        for validation_el in self._entity:
+        for validation_el in self.entity:
             if validation_data := self.validation_reader_cls(validation_el, self.data_provider):
                 if validation := validation_data.get_validation(lang, base_url, provider_domain):
                     result.append(validation)
         return result
```

### Comparing `ilcdlib-4.6.0/src/ilcdlib/epd/__init__.py` & `ilcdlib-4.7.0/src/ilcdlib/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/epd/cli.py` & `ilcdlib-4.7.0/src/ilcdlib/epd/cli.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/epd/dialect/__init__.py` & `ilcdlib-4.7.0/src/ilcdlib/epd/dialect/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/epd/dialect/environdec.py` & `ilcdlib-4.7.0/src/ilcdlib/epd/dialect/environdec.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/epd/dialect/epditaly.py` & `ilcdlib-4.7.0/src/ilcdlib/epd/dialect/epditaly.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/epd/dialect/epdnorge.py` & `ilcdlib-4.7.0/src/ilcdlib/epd/dialect/epdnorge.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #
 #  This software was developed with support from the Skanska USA,
 #  Charles Pankow Foundation, Microsoft Sustainability Fund, Interface, MKA Foundation, and others.
 #  Find out more at www.BuildingTransparency.org
 #
 import datetime
 
-from ilcdlib.dto import IlcdContactInfo, MappedCategory, OpenEpdIlcdOrg, ValidationDto
+from ilcdlib.dto import MappedCategory, OpenEpdIlcdOrg, ValidationDto
 from ilcdlib.epd.reader import IlcdEpdReader
 from ilcdlib.mapping.category import CsvCategoryMapper
 from ilcdlib.type import LangDef
 
 
 class EpdNorgeCategoryMapper(CsvCategoryMapper):
     """A category mapper for EpdNorge."""
@@ -52,27 +52,38 @@
 
     @classmethod
     def _create_category_mapper(cls, classification_name: str) -> CsvCategoryMapper | None:
         if classification_name.lower() == cls.EPDNORGE_CLASSIFICATION_NAME:
             return EpdNorgeCategoryMapper.from_file("epdnorge.csv")
         return None
 
-    def get_third_party_verifier_email(self, validations: list[ValidationDto]) -> OpenEpdIlcdOrg | None:
+    def get_third_party_verifier(self, validations: list[ValidationDto]) -> OpenEpdIlcdOrg | None:
         """
-        Return first third party verifier email.
+        Return the third party verifier.
 
-        EpdNorge contains personal info instead of organization info.
+        EPD Norge contains personal info instead of organization info.
         """
-        verifier = self.get_third_party_verifier(validations)
-        if not verifier:
-            return None
-        contact = verifier.get_contact()
-        if contact is None:
-            return None
-        return IlcdContactInfo.parse_obj(contact).email
+        validation_reader = self.get_validation_reader()
+        validation_el = validation_reader.entity if validation_reader else None
+        reviewer_el = (
+            self._get_el(validation_el[0], ("common:referenceToNameOfReviewerAndInstitution",))
+            if validation_el
+            else None
+        )
+        third_party_verifier = super().get_third_party_verifier(validations)
+        if reviewer_el:
+            reviewer_name = self._get_localized_text(reviewer_el, ("common:shortDescription",), ("en", None))
+            if not reviewer_name:
+                return third_party_verifier
+            normalized_reviewer_name = reviewer_name.split("-")[0].strip()
+            if not third_party_verifier:
+                third_party_verifier = OpenEpdIlcdOrg(name=normalized_reviewer_name)
+            else:
+                third_party_verifier.name = normalized_reviewer_name
+        return third_party_verifier
 
     def get_product_description(self, lang: LangDef) -> str | None:
         """Return the product description in the given language."""
         return self._get_localized_text(
             self.epd_el_tree,
             ("process:processInformation", "process:technology", "process:technologicalApplicability"),
             lang,
@@ -106,7 +117,23 @@
         if descr and self._TIME_REPR_DESC_DELIMITER in descr:
             try:
                 date_str = descr.split(self._TIME_REPR_DESC_DELIMITER)[0].strip().rsplit(" ", 1)[-1].strip()
                 return datetime.date.fromisoformat(date_str)
             except Exception:
                 pass
         return super().get_date_published()
+
+    def get_data_entry_by(self, lang: LangDef, base_url: str | None = None) -> OpenEpdIlcdOrg | None:
+        """Return the data entry by org."""
+        developer = self._get_localized_text(
+            self.epd_el_tree,
+            (
+                "process:administrativeInformation",
+                "process:dataGenerator",
+                "common:referenceToPersonOrEntityGeneratingTheDataSet",
+                "common:shortDescription",
+            ),
+            ("en", None),
+        )
+        if developer:
+            return OpenEpdIlcdOrg(name=developer)
+        return super().get_data_entry_by(lang, base_url)
```

### Comparing `ilcdlib-4.6.0/src/ilcdlib/epd/dialect/indata.py` & `ilcdlib-4.7.0/src/ilcdlib/epd/dialect/indata.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/epd/dialect/itb.py` & `ilcdlib-4.7.0/src/ilcdlib/epd/dialect/itb.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/epd/dialect/oekobaudat.py` & `ilcdlib-4.7.0/src/ilcdlib/epd/dialect/oekobaudat.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/epd/factory.py` & `ilcdlib-4.7.0/src/ilcdlib/epd/factory.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/epd/reader.py` & `ilcdlib-4.7.0/src/ilcdlib/epd/reader.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/extension.py` & `ilcdlib-4.7.0/src/ilcdlib/extension.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/http_common.py` & `ilcdlib-4.7.0/src/ilcdlib/http_common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/mapping/__init__.py` & `ilcdlib-4.7.0/src/ilcdlib/mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/mapping/category.py` & `ilcdlib-4.7.0/src/ilcdlib/mapping/category.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/mapping/common.py` & `ilcdlib-4.7.0/src/ilcdlib/mapping/common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/mapping/compliance.py` & `ilcdlib-4.7.0/src/ilcdlib/mapping/compliance.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/mapping/flows.py` & `ilcdlib-4.7.0/src/ilcdlib/mapping/flows.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/mapping/impacts.py` & `ilcdlib-4.7.0/src/ilcdlib/mapping/impacts.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/mapping/indicators.py` & `ilcdlib-4.7.0/src/ilcdlib/mapping/indicators.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/mapping/properties.py` & `ilcdlib-4.7.0/src/ilcdlib/mapping/properties.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/mapping/units.py` & `ilcdlib-4.7.0/src/ilcdlib/mapping/units.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/medium/__init__.py` & `ilcdlib-4.7.0/src/ilcdlib/medium/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/medium/archive.py` & `ilcdlib-4.7.0/src/ilcdlib/medium/archive.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/medium/soda4lca.py` & `ilcdlib-4.7.0/src/ilcdlib/medium/soda4lca.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/reference_data.py` & `ilcdlib-4.7.0/src/ilcdlib/reference_data.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/sanitizing/__init__.py` & `ilcdlib-4.7.0/src/ilcdlib/sanitizing/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/sanitizing/domain.py` & `ilcdlib-4.7.0/src/ilcdlib/sanitizing/domain.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/sanitizing/phone.py` & `ilcdlib-4.7.0/src/ilcdlib/sanitizing/phone.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/sanitizing/text.py` & `ilcdlib-4.7.0/src/ilcdlib/sanitizing/text.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/soda4lca/__init__.py` & `ilcdlib-4.7.0/src/ilcdlib/soda4lca/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/soda4lca/api_client.py` & `ilcdlib-4.7.0/src/ilcdlib/soda4lca/api_client.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/soda4lca/api_client_4x.py` & `ilcdlib-4.7.0/src/ilcdlib/soda4lca/api_client_4x.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/type.py` & `ilcdlib-4.7.0/src/ilcdlib/type.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/utils.py` & `ilcdlib-4.7.0/src/ilcdlib/utils.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/src/ilcdlib/xml_parser.py` & `ilcdlib-4.7.0/src/ilcdlib/xml_parser.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.6.0/PKG-INFO` & `ilcdlib-4.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilcdlib
-Version: 4.6.0
+Version: 4.7.0
 Summary: A toolkit for reading and writing ILCD format and it's derivatives
 Home-page: https://github.com/cchangelabs/ilcdlib
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: open-source@c-change-labs.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ilcdlib Version: 4.6.0 Summary: A toolkit for
+Metadata-Version: 2.1 Name: ilcdlib Version: 4.7.0 Summary: A toolkit for
 reading and writing ILCD format and it's derivatives Home-page: https://
 github.com/cchangelabs/ilcdlib License: Apache-2.0 Author: C-Change Labs
 Author-email: support@c-change-labs.com Maintainer: C-Change Labs Maintainer-
 email: open-source@c-change-labs.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```


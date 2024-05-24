# Comparing `tmp/scida-0.3.1.tar.gz` & `tmp/scida-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scida-0.3.1.tar", max compression
+gzip compressed data, was "scida-0.3.2.tar", max compression
```

## Comparing `scida-0.3.1.tar` & `scida-0.3.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1074 2024-02-19 22:23:18.049849 scida-0.3.1/LICENSE
--rw-r--r--   0        0        0     1482 2024-02-19 22:23:18.049849 scida-0.3.1/README.md
--rw-r--r--   0        0        0     1741 2024-02-19 22:23:18.077849 scida-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      888 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/__init__.py
--rw-r--r--   0        0        0     8919 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/config.py
--rw-r--r--   0        0        0        0 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/configfiles/__init__.py
--rw-r--r--   0        0        0     1082 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/configfiles/config.yaml
--rw-r--r--   0        0        0     4206 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/configfiles/simulations.yaml
--rw-r--r--   0        0        0        0 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/configfiles/units/__init__.py
--rw-r--r--   0        0        0      985 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/configfiles/units/auriga.yaml
--rw-r--r--   0        0        0     3168 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/configfiles/units/eagle.yaml
--rw-r--r--   0        0        0      342 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/configfiles/units/erosita_events.yaml
--rw-r--r--   0        0        0      234 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/configfiles/units/flamingo.yaml
--rw-r--r--   0        0        0     7100 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/configfiles/units/gadget_cosmological.yaml
--rw-r--r--   0        0        0      662 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/configfiles/units/gaia.yaml
--rw-r--r--   0        0        0       30 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/configfiles/units/general.yaml
--rw-r--r--   0        0        0     1891 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/configfiles/units/gizmo.yaml
--rw-r--r--   0        0        0     3145 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/configfiles/units/lgalaxies.yaml
--rw-r--r--   0        0        0      576 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/configfiles/units/mtng.yaml
--rw-r--r--   0        0        0     1970 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/configfiles/units/rockstar.yaml
--rw-r--r--   0        0        0    12720 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/convenience.py
--rw-r--r--   0        0        0        0 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/customs/__init__.py
--rw-r--r--   0        0        0       31 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/customs/arepo/MTNG/__init__.py
--rw-r--r--   0        0        0     5654 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/customs/arepo/MTNG/dataset.py
--rw-r--r--   0        0        0      105 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/customs/arepo/TNGcluster/__init__.py
--rw-r--r--   0        0        0     9771 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/customs/arepo/TNGcluster/dataset.py
--rw-r--r--   0        0        0        0 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/customs/arepo/__init__.py
--rw-r--r--   0        0        0    53553 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/customs/arepo/dataset.py
--rw-r--r--   0        0        0     1322 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/customs/arepo/helpers.py
--rw-r--r--   0        0        0     4267 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/customs/arepo/selector.py
--rw-r--r--   0        0        0     2320 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/customs/arepo/series.py
--rw-r--r--   0        0        0        0 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/customs/gadgetstyle/__init__.py
--rw-r--r--   0        0        0     8599 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/customs/gadgetstyle/dataset.py
--rw-r--r--   0        0        0     3903 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/customs/gadgetstyle/series.py
--rw-r--r--   0        0        0     3097 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/customs/gizmo/dataset.py
--rw-r--r--   0        0        0     1656 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/customs/gizmo/series.py
--rw-r--r--   0        0        0     1615 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/customs/rockstar/dataset.py
--rw-r--r--   0        0        0     1413 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/customs/swift/dataset.py
--rw-r--r--   0        0        0     1559 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/customs/swift/series.py
--rw-r--r--   0        0        0     7304 2024-02-19 22:23:18.077849 scida-0.3.1/src/scida/discovertypes.py
--rw-r--r--   0        0        0    24208 2024-02-19 22:23:18.081849 scida-0.3.1/src/scida/fields.py
--rw-r--r--   0        0        0    12207 2024-02-19 22:23:18.081849 scida-0.3.1/src/scida/helpers_hdf5.py
--rw-r--r--   0        0        0     4868 2024-02-19 22:23:18.081849 scida-0.3.1/src/scida/helpers_misc.py
--rw-r--r--   0        0        0    14524 2024-02-19 22:23:18.081849 scida-0.3.1/src/scida/interface.py
--rw-r--r--   0        0        0      307 2024-02-19 22:23:18.081849 scida-0.3.1/src/scida/interfaces/mixins/__init__.py
--rw-r--r--   0        0        0       66 2024-02-19 22:23:18.081849 scida-0.3.1/src/scida/interfaces/mixins/base.py
--rw-r--r--   0        0        0     4531 2024-02-19 22:23:18.081849 scida-0.3.1/src/scida/interfaces/mixins/cosmology.py
--rw-r--r--   0        0        0     3460 2024-02-19 22:23:18.081849 scida-0.3.1/src/scida/interfaces/mixins/spatial.py
--rw-r--r--   0        0        0    24116 2024-02-19 22:23:18.081849 scida-0.3.1/src/scida/interfaces/mixins/units.py
--rw-r--r--   0        0        0      166 2024-02-19 22:23:18.081849 scida-0.3.1/src/scida/io/__init__.py
--rw-r--r--   0        0        0    27200 2024-02-19 22:23:18.081849 scida-0.3.1/src/scida/io/_base.py
--rw-r--r--   0        0        0     1738 2024-02-19 22:23:18.081849 scida-0.3.1/src/scida/io/fits.py
--rw-r--r--   0        0        0     9051 2024-02-19 22:23:18.081849 scida-0.3.1/src/scida/misc.py
--rw-r--r--   0        0        0      268 2024-02-19 22:23:18.081849 scida-0.3.1/src/scida/registries.py
--rw-r--r--   0        0        0    17096 2024-02-19 22:23:18.081849 scida-0.3.1/src/scida/series.py
--rw-r--r--   0        0        0      687 2024-02-19 22:23:18.081849 scida-0.3.1/src/scida/utilities.py
--rw-r--r--   0        0        0     2814 1970-01-01 00:00:00.000000 scida-0.3.1/setup.py
--rw-r--r--   0        0        0     2382 1970-01-01 00:00:00.000000 scida-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-24 15:32:03.985654 scida-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2047 2024-05-24 15:32:03.985654 scida-0.3.2/README.md
+-rw-r--r--   0        0        0     1741 2024-05-24 15:32:04.013654 scida-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      888 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/__init__.py
+-rw-r--r--   0        0        0     8919 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/config.py
+-rw-r--r--   0        0        0        0 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/configfiles/__init__.py
+-rw-r--r--   0        0        0     1096 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/configfiles/config.yaml
+-rw-r--r--   0        0        0     4206 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/configfiles/simulations.yaml
+-rw-r--r--   0        0        0        0 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/configfiles/units/__init__.py
+-rw-r--r--   0        0        0      985 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/configfiles/units/auriga.yaml
+-rw-r--r--   0        0        0     3168 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/configfiles/units/eagle.yaml
+-rw-r--r--   0        0        0      342 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/configfiles/units/erosita_events.yaml
+-rw-r--r--   0        0        0      234 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/configfiles/units/flamingo.yaml
+-rw-r--r--   0        0        0     7100 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/configfiles/units/gadget_cosmological.yaml
+-rw-r--r--   0        0        0      662 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/configfiles/units/gaia.yaml
+-rw-r--r--   0        0        0       30 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/configfiles/units/general.yaml
+-rw-r--r--   0        0        0     1891 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/configfiles/units/gizmo.yaml
+-rw-r--r--   0        0        0     3145 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/configfiles/units/lgalaxies.yaml
+-rw-r--r--   0        0        0      576 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/configfiles/units/mtng.yaml
+-rw-r--r--   0        0        0     1970 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/configfiles/units/rockstar.yaml
+-rw-r--r--   0        0        0    12720 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/convenience.py
+-rw-r--r--   0        0        0        0 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/customs/__init__.py
+-rw-r--r--   0        0        0       31 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/customs/arepo/MTNG/__init__.py
+-rw-r--r--   0        0        0     5654 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/customs/arepo/MTNG/dataset.py
+-rw-r--r--   0        0        0      105 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/customs/arepo/TNGcluster/__init__.py
+-rw-r--r--   0        0        0     9771 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/customs/arepo/TNGcluster/dataset.py
+-rw-r--r--   0        0        0        0 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/customs/arepo/__init__.py
+-rw-r--r--   0        0        0    53553 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/customs/arepo/dataset.py
+-rw-r--r--   0        0        0     1322 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/customs/arepo/helpers.py
+-rw-r--r--   0        0        0     5123 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/customs/arepo/selector.py
+-rw-r--r--   0        0        0     2320 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/customs/arepo/series.py
+-rw-r--r--   0        0        0        0 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/customs/gadgetstyle/__init__.py
+-rw-r--r--   0        0        0     8599 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/customs/gadgetstyle/dataset.py
+-rw-r--r--   0        0        0     5181 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/customs/gadgetstyle/series.py
+-rw-r--r--   0        0        0     3097 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/customs/gizmo/dataset.py
+-rw-r--r--   0        0        0     1656 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/customs/gizmo/series.py
+-rw-r--r--   0        0        0     1615 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/customs/rockstar/dataset.py
+-rw-r--r--   0        0        0     1413 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/customs/swift/dataset.py
+-rw-r--r--   0        0        0     1559 2024-05-24 15:32:04.013654 scida-0.3.2/src/scida/customs/swift/series.py
+-rw-r--r--   0        0        0     7304 2024-05-24 15:32:04.017654 scida-0.3.2/src/scida/discovertypes.py
+-rw-r--r--   0        0        0    24208 2024-05-24 15:32:04.017654 scida-0.3.2/src/scida/fields.py
+-rw-r--r--   0        0        0    12207 2024-05-24 15:32:04.017654 scida-0.3.2/src/scida/helpers_hdf5.py
+-rw-r--r--   0        0        0     4868 2024-05-24 15:32:04.017654 scida-0.3.2/src/scida/helpers_misc.py
+-rw-r--r--   0        0        0    14524 2024-05-24 15:32:04.017654 scida-0.3.2/src/scida/interface.py
+-rw-r--r--   0        0        0      307 2024-05-24 15:32:04.017654 scida-0.3.2/src/scida/interfaces/mixins/__init__.py
+-rw-r--r--   0        0        0       66 2024-05-24 15:32:04.017654 scida-0.3.2/src/scida/interfaces/mixins/base.py
+-rw-r--r--   0        0        0     4531 2024-05-24 15:32:04.017654 scida-0.3.2/src/scida/interfaces/mixins/cosmology.py
+-rw-r--r--   0        0        0     3460 2024-05-24 15:32:04.017654 scida-0.3.2/src/scida/interfaces/mixins/spatial.py
+-rw-r--r--   0        0        0    24193 2024-05-24 15:32:04.017654 scida-0.3.2/src/scida/interfaces/mixins/units.py
+-rw-r--r--   0        0        0      166 2024-05-24 15:32:04.017654 scida-0.3.2/src/scida/io/__init__.py
+-rw-r--r--   0        0        0    27200 2024-05-24 15:32:04.017654 scida-0.3.2/src/scida/io/_base.py
+-rw-r--r--   0        0        0     1738 2024-05-24 15:32:04.017654 scida-0.3.2/src/scida/io/fits.py
+-rw-r--r--   0        0        0     9154 2024-05-24 15:32:04.017654 scida-0.3.2/src/scida/misc.py
+-rw-r--r--   0        0        0      268 2024-05-24 15:32:04.017654 scida-0.3.2/src/scida/registries.py
+-rw-r--r--   0        0        0    17096 2024-05-24 15:32:04.017654 scida-0.3.2/src/scida/series.py
+-rw-r--r--   0        0        0      687 2024-05-24 15:32:04.017654 scida-0.3.2/src/scida/utilities.py
+-rw-r--r--   0        0        0     3399 1970-01-01 00:00:00.000000 scida-0.3.2/setup.py
+-rw-r--r--   0        0        0     2947 1970-01-01 00:00:00.000000 scida-0.3.2/PKG-INFO
```

### Comparing `scida-0.3.1/LICENSE` & `scida-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/pyproject.toml` & `scida-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scida"
-version = "0.3.1"
+version = "0.3.2"
 description = "Convenience wrapper around large scientific datasets to process with dask."
 authors = ["Chris Byrohl"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 numpy = "^1.21"
```

### Comparing `scida-0.3.1/src/scida/__init__.py` & `scida-0.3.2/src/scida/__init__.py`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/config.py` & `scida-0.3.2/src/scida/config.py`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/configfiles/config.yaml` & `scida-0.3.2/src/scida/configfiles/config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# example for scida config. copy to ~/.scida.yaml and modify accordingly
+# example for scida config. copy to ~/.config/scida/config.yaml and modify accordingly
 ---
 
 copied_default: True  # if this is set, a warning is printed as the default config has not been adjusted
 # adjust the config to your needs and remove above line to remove warning.
 cache_path: ~/cachedir_scida
 testdata_path: /fastdata/public/testdata-scida  # should be replaced by 'datafolders' logic further below eventually
 nthreads: 8
```

### Comparing `scida-0.3.1/src/scida/configfiles/simulations.yaml` & `scida-0.3.2/src/scida/configfiles/simulations.yaml`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/configfiles/units/auriga.yaml` & `scida-0.3.2/src/scida/configfiles/units/auriga.yaml`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/configfiles/units/eagle.yaml` & `scida-0.3.2/src/scida/configfiles/units/eagle.yaml`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/configfiles/units/gadget_cosmological.yaml` & `scida-0.3.2/src/scida/configfiles/units/gadget_cosmological.yaml`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/configfiles/units/gaia.yaml` & `scida-0.3.2/src/scida/configfiles/units/gaia.yaml`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/configfiles/units/gizmo.yaml` & `scida-0.3.2/src/scida/configfiles/units/gizmo.yaml`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/configfiles/units/lgalaxies.yaml` & `scida-0.3.2/src/scida/configfiles/units/lgalaxies.yaml`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/configfiles/units/mtng.yaml` & `scida-0.3.2/src/scida/configfiles/units/mtng.yaml`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/configfiles/units/rockstar.yaml` & `scida-0.3.2/src/scida/configfiles/units/rockstar.yaml`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/convenience.py` & `scida-0.3.2/src/scida/convenience.py`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/customs/arepo/MTNG/dataset.py` & `scida-0.3.2/src/scida/customs/arepo/MTNG/dataset.py`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/customs/arepo/TNGcluster/dataset.py` & `scida-0.3.2/src/scida/customs/arepo/TNGcluster/dataset.py`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/customs/arepo/dataset.py` & `scida-0.3.2/src/scida/customs/arepo/dataset.py`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/customs/arepo/helpers.py` & `scida-0.3.2/src/scida/customs/arepo/helpers.py`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/customs/arepo/selector.py` & `scida-0.3.2/src/scida/customs/arepo/selector.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Selector for ArepoSnapshot
 """
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 
 from scida.customs.arepo.helpers import grp_type_str
 from scida.interface import Selector
 
 if TYPE_CHECKING:
     from scida.customs.arepo.snapshot import ArepoSnapshot
 
@@ -16,36 +16,52 @@
     Can select for haloID, subhaloID, and unbound particles."""
 
     def __init__(self) -> None:
         """
         Initialize the selector.
         """
         super().__init__()
-        self.keys = ["haloID", "subhaloID", "unbound"]
+        self.keys = ["haloID", "subhaloID", "localSubhaloID", "unbound"]
 
     def prepare(self, *args, **kwargs) -> None:
         if all([kwargs.get(k, None) is None for k in self.keys]):
             return  # no specific selection, thus just return
         snap: ArepoSnapshot = args[0]
         halo_id = kwargs.get("haloID", None)
         subhalo_id = kwargs.get("subhaloID", None)
+        subhalo_id_local: Optional[int] = kwargs.get("localSubhaloID", None)
         unbound = kwargs.get("unbound", None)
 
         if halo_id is not None and subhalo_id is not None:
             raise ValueError("Cannot select for haloID and subhaloID at the same time.")
 
         if unbound is True and (halo_id is not None or subhalo_id is not None):
             raise ValueError(
                 "Cannot select haloID/subhaloID and unbound particles at the same time."
             )
 
+        if subhalo_id_local is not None and subhalo_id is not None:
+            raise ValueError(
+                "Cannot select for localSubhaloID and subhaloID at the same time."
+            )
+
         if snap.catalog is None:
             raise ValueError("Cannot select for haloID without catalog loaded.")
 
         # select for halo
+        if subhalo_id_local is not None:
+            if halo_id is None:
+                raise ValueError("Cannot select for localSubhaloID without haloID.")
+            # compute subhalo_id from subhalo_id_local
+            shid_of_first_sh = snap.data["Group"]["GroupFirstSub"]
+            nshs = int(snap.data["Group"]["GroupNsubs"][halo_id].compute())
+            if subhalo_id_local >= nshs:
+                raise ValueError("localSubhaloID exceeds number of subhalos in halo.")
+            subhalo_id = shid_of_first_sh[halo_id] + subhalo_id_local
+
         idx = subhalo_id if subhalo_id is not None else halo_id
         objtype = "subhalo" if subhalo_id is not None else "halo"
         if idx is not None:
             self.select_group(snap, idx, objtype=objtype)
         elif unbound is True:
             self.select_unbound(snap)
```

### Comparing `scida-0.3.1/src/scida/customs/arepo/series.py` & `scida-0.3.2/src/scida/customs/arepo/series.py`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/customs/gadgetstyle/dataset.py` & `scida-0.3.2/src/scida/customs/gadgetstyle/dataset.py`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/customs/gadgetstyle/series.py` & `scida-0.3.2/src/scida/customs/gadgetstyle/series.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """
 Defines a series representing a Gadget-style simulation.
 """
+
+import logging
 import os
 import pathlib
 from pathlib import Path
 from typing import Dict, Optional
 
 from scida.discovertypes import _determine_mixins, _determine_type
 from scida.interface import create_datasetclass_with_mixins
 from scida.series import DatasetSeries
 
+log = logging.getLogger(__name__)
+
 
 class GadgetStyleSimulation(DatasetSeries):
     """A series representing a Gadget-style simulation."""
 
     def __init__(
         self,
         path,
@@ -51,46 +55,71 @@
         keys = []
         for d in [prefix_dict, subpath_dict, arg_dict]:
             keys.extend(list(d.keys()))
         keys = set(keys)
         for k in keys:
             subpath = subpath_dict.get(k, "output")
             sp = p / subpath
-
+            # by default, we assume that we are given a folder that has an "output" subfolder.
+            # this is not always the case - for example for subboxes.
+            # in such case, we attempt to continue with the given path.
+            if not sp.exists():
+                sp = p
             prefix = _get_snapshotfolder_prefix(sp)
             prefix = prefix_dict.get(k, prefix)
             if not sp.exists():
                 if k != "paths":
                     continue  # do not require optional sources
                 raise ValueError("Specified path '%s' does not exist." % (p / subpath))
             fns = os.listdir(sp)
             prfxs = set([f.split("_")[0] for f in fns if f.startswith(prefix)])
             if len(prfxs) == 0:
+                if k != "paths":
+                    continue  # do not require optional sources
                 raise ValueError(
                     "Could not find any files with prefix '%s' in '%s'." % (prefix, sp)
                 )
             prfx = prfxs.pop()
 
             paths = sorted([p for p in sp.glob(prfx + "_*")])
             # sometimes there are backup folders with different suffix, exclude those.
             paths = [
                 p
                 for p in paths
                 if str(p).split("_")[-1].isdigit() or str(p).endswith(".hdf5")
             ]
+            # attempt additional sorting in case zfill not used
+            try:
+                paths = sorted(paths, key=lambda x: int(str(x).split("_")[-1]))
+            except:  # noqa
+                pass
             paths_dict[k] = paths
 
         # make sure we have the same amount of paths respectively
         length = None
+        mismatch_length = False
         for k in paths_dict.keys():
             paths = paths_dict[k]
             if length is None:
                 length = len(paths)
             else:
-                assert length == len(paths)
+                if length != len(paths):
+                    mismatch_length = True
+        if mismatch_length:
+            msg = """Mismatch between number of groups and snapshots.
+                     Only loading groups that have a snapshot associated."""
+            log.info(msg)
+            # extract ids
+            paths = paths_dict["paths"]
+            ids = [int(str(p).split("_")[-1]) for p in paths]
+            for k in paths_dict.keys():
+                if k == "paths":
+                    continue
+                paths = paths_dict[k]
+                paths_dict[k] = [p for p in paths if int(str(p).split("_")[-1]) in ids]
 
         paths = paths_dict.pop("paths", None)
         if paths is None:
             raise ValueError("Could not find any snapshot paths.")
         p = paths[0]
         cls = _determine_type(p)[1][0]
```

### Comparing `scida-0.3.1/src/scida/customs/gizmo/dataset.py` & `scida-0.3.2/src/scida/customs/gizmo/dataset.py`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/customs/gizmo/series.py` & `scida-0.3.2/src/scida/customs/gizmo/series.py`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/customs/rockstar/dataset.py` & `scida-0.3.2/src/scida/customs/rockstar/dataset.py`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/customs/swift/dataset.py` & `scida-0.3.2/src/scida/customs/swift/dataset.py`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/customs/swift/series.py` & `scida-0.3.2/src/scida/customs/swift/series.py`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/discovertypes.py` & `scida-0.3.2/src/scida/discovertypes.py`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/fields.py` & `scida-0.3.2/src/scida/fields.py`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/helpers_hdf5.py` & `scida-0.3.2/src/scida/helpers_hdf5.py`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/helpers_misc.py` & `scida-0.3.2/src/scida/helpers_misc.py`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/interface.py` & `scida-0.3.2/src/scida/interface.py`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/interfaces/mixins/cosmology.py` & `scida-0.3.2/src/scida/interfaces/mixins/cosmology.py`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/interfaces/mixins/spatial.py` & `scida-0.3.2/src/scida/interfaces/mixins/spatial.py`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/interfaces/mixins/units.py` & `scida-0.3.2/src/scida/interfaces/mixins/units.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         except IndexError:
             try:
                 unitstr = desc.split("(")[1].split(")")[0]
             except IndexError:
                 pass
         if unitstr is not None and unitstr != desc and unitstr != "None":
             unitstr = unitstr.strip("'")
-        unitstr = unitstr.lower()
+            unitstr = unitstr.lower()
 
     return unitstr
 
 
 def extract_units_from_attrs(
     attrs: dict,
     require: bool = False,
@@ -175,15 +175,18 @@
         return unit
 
     unitstr = get_unitstr_from_attrs(attrs)
     if unitstr == "none":
         return "none"
     if unitstr is not None:
         has_expl_units = True
-        unit *= str_to_unit(unitstr, ureg)
+        ures = str_to_unit(unitstr, ureg)
+        if ures == "none":
+            return "none"
+        unit *= ures
         return unit
 
     if not has_expl_units and not has_convfactor:
         if require:
             raise ValueError("Could not find explicit units nor cgs-factor.")
     if require:
         raise ValueError("Could not find units.")
```

### Comparing `scida-0.3.1/src/scida/io/_base.py` & `scida-0.3.2/src/scida/io/_base.py`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/io/fits.py` & `scida-0.3.2/src/scida/io/fits.py`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/misc.py` & `scida-0.3.2/src/scida/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,18 @@
     cp = os.path.expanduser(cp)
     path = pathlib.Path(cp)
     path.mkdir(parents=True, exist_ok=True)
     fp = os.path.join(cp, fname)
     fp = os.path.expanduser(fp)
     bp = os.path.dirname(fp)
     if not os.path.exists(bp):
-        os.mkdir(bp)
+        try:
+            os.mkdir(bp)
+        except FileExistsError:
+            pass  # can happen due to parallel access
     return fp
 
 
 def map_interface_args(paths: list, *args, **kwargs):
     """
     Map arguments for interface if they are not lists.
     Parameters
```

### Comparing `scida-0.3.1/src/scida/series.py` & `scida-0.3.2/src/scida/series.py`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/src/scida/utilities.py` & `scida-0.3.2/src/scida/utilities.py`

 * *Files identical despite different names*

### Comparing `scida-0.3.1/setup.py` & `scida-0.3.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,17 +34,17 @@
  'pyyaml>=5.3.1',
  'requests>=2.31.0,<3.0.0',
  'tqdm>=4.64.1,<5.0.0',
  'zarr>=v2.10.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'scida',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'description': 'Convenience wrapper around large scientific datasets to process with dask.',
-    'long_description': '# scida\n\n![test status](https://github.com/cbyrohl/scida/actions/workflows/tests.yml/badge.svg)\n\nscida is an out-of-the-box analysis tool for large scientific datasets. It primarily supports the astrophysics community, focusing on cosmological and galaxy formation simulations using particles or unstructured meshes, as well as large observational datasets.\nThis tool uses dask, allowing analysis to scale up from your personal computer to HPC resources and the cloud.\n\n## Features\n\n- Unified, high-level interface to load and analyze large datasets from a variety of sources.\n- Parallel, task-based data processing with dask arrays.\n- Physical unit support via pint.\n- Easily extensible architecture.\n\n## Requirements\n\n- Python 3.9, 3.10, 3.11\n\n\n## Documentation\nThe documentation can be found [here](https://cbyrohl.github.io/scida/).\n\n## Install\n\n```\npip install scida\n```\n\n## First Steps\nAfter installing scida, follow the [tutorial](https://cbyrohl.github.io/scida/tutorial/).\n\n## License\n\nDistributed under the terms of the [MIT license](LICENSE),\n_scida_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue](https://github.com/cbyrohl/scida/issues/new) along with a detailed description.\n\n## Acknowledgements\n\nThe project structure was adapted from [Wolt](https://github.com/woltapp/wolt-python-package-cookiecutter) and [Hypermodern Python](https://github.com/cjolowicz/cookiecutter-hypermodern-python) cookiecutter templates.\n',
+    'long_description': '# scida\n\n![test status](https://github.com/cbyrohl/scida/actions/workflows/tests.yml/badge.svg)\n[![DOI](https://joss.theoj.org/papers/10.21105/joss.06064/status.svg)](https://doi.org/10.21105/joss.06064)\n\nscida is an out-of-the-box analysis tool for large scientific datasets. It primarily supports the astrophysics community, focusing on cosmological and galaxy formation simulations using particles or unstructured meshes, as well as large observational datasets.\nThis tool uses dask, allowing analysis to scale up from your personal computer to HPC resources and the cloud.\n\n## Features\n\n- Unified, high-level interface to load and analyze large datasets from a variety of sources.\n- Parallel, task-based data processing with dask arrays.\n- Physical unit support via pint.\n- Easily extensible architecture.\n\n## Requirements\n\n- Python 3.9, 3.10, 3.11\n\n\n## Documentation\nThe documentation can be found [here](https://cbyrohl.github.io/scida/).\n\n## Install\n\n```\npip install scida\n```\n\n## First Steps\n\nAfter installing scida, follow the [tutorial](https://cbyrohl.github.io/scida/tutorial/).\n\n## Citation\n\nIf you use scida in your research, please cite the following [paper](https://joss.theoj.org/papers/10.21105/joss.06064):\n\n```text\n`Byrohl et al., (2024). scida: scalable analysis for scientific big data. Journal of Open Source Software, 9(94), 6064, https://doi.org/10.21105/joss.06064`\n```\n\nwith the following bibtex entry:\n\n```text\n@article{scida,\n  title = {scida: scalable analysis for scientific big data},\n  author = {Chris Byrohl and Dylan Nelson},\n  doi = {10.21105/joss.06064},\n  url = {https://doi.org/10.21105/joss.06064}, year = {2024},\n  publisher = {The Open Journal}, volume = {9}, number = {94},\n  pages = {6064},\n  journal = {Journal of Open Source Software}\n}\n```\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue](https://github.com/cbyrohl/scida/issues/new) along with a detailed description.\n\n## License\n\nDistributed under the terms of the [MIT license](LICENSE),\n_scida_ is free and open source software.\n',
     'author': 'Chris Byrohl',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```


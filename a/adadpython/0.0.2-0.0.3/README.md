# Comparing `tmp/adadpython-0.0.2.tar.gz` & `tmp/adadpython-0.0.3.tar.gz`

## Comparing `adadpython-0.0.2.tar` & `adadpython-0.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/__init__.py
--rw-r--r--   0        0        0   204586 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/base_pokemon.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/dbz.sav
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/dexpoke.py
--rw-r--r--   0        0        0    33947 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/moves.py
--rw-r--r--   0        0        0    91023 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/pokemon.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/pypokemon.sav
--rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/save2.npy
--rw-r--r--   0        0        0    34702 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/somemons.dat
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/texter.py
--rw-r--r--   0        0        0    15640 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/trainerai.py
--rw-r--r--   0        0        0    11099 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/victoryroad.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/LICENSES/numpy_license.txt
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/LICENSES/python_license.txt
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/configurations/config.txt
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/configurations/default_config.txt
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/configurations/second_config.txt
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/documentation/CREDITS.txt
--rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/documentation/game_blurb.md
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/documentation/log.md
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/documentation/time_ref.txt
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/documentation/archive/moremon.py
--rw-r--r--   0        0        0   107092 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/documentation/archive/saved_dexpoke.npy
--rw-r--r--   0        0        0   203144 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/documentation/archive/saved_movedex.npy
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/documentation/archive/saved_natures.npy
--rw-r--r--   0        0        0    34624 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/documentation/archive/somemons_copy.txt
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/elite5/elite_1.npy
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/elite5/elite_2.npy
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/elite5/elite_3.npy
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/elite5/elite_4.npy
--rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 adadpython-0.0.2/src/adadpython/elite5/elite_5.npy
--rw-r--r--   0        0        0    32424 2020-02-02 00:00:00.000000 adadpython-0.0.2/LICENSE
--rw-r--r--   0        0        0     6016 2020-02-02 00:00:00.000000 adadpython-0.0.2/README.md
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 adadpython-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6470 2020-02-02 00:00:00.000000 adadpython-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/__init__.py
+-rw-r--r--   0        0        0   204586 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/base_pokemon.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/dbz.sav
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/dexpoke.py
+-rw-r--r--   0        0        0    33947 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/moves.py
+-rw-r--r--   0        0        0    91023 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/pokemon.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/pypokemon.sav
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/save2.npy
+-rw-r--r--   0        0        0    34702 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/somemons.dat
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/texter.py
+-rw-r--r--   0        0        0    15640 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/trainerai.py
+-rw-r--r--   0        0        0    11099 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/victoryroad.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/LICENSES/numpy_license.txt
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/LICENSES/python_license.txt
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/configurations/config.txt
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/configurations/default_config.txt
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/configurations/second_config.txt
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/documentation/CREDITS.txt
+-rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/documentation/game_blurb.md
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/documentation/log.md
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/documentation/time_ref.txt
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/documentation/archive/moremon.py
+-rw-r--r--   0        0        0   107092 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/documentation/archive/saved_dexpoke.npy
+-rw-r--r--   0        0        0   203144 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/documentation/archive/saved_movedex.npy
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/documentation/archive/saved_natures.npy
+-rw-r--r--   0        0        0    34624 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/documentation/archive/somemons_copy.txt
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/elite5/elite_1.npy
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/elite5/elite_2.npy
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/elite5/elite_3.npy
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/elite5/elite_4.npy
+-rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 adadpython-0.0.3/src/adadpython/elite5/elite_5.npy
+-rw-r--r--   0        0        0    32424 2020-02-02 00:00:00.000000 adadpython-0.0.3/LICENSE
+-rw-r--r--   0        0        0     6016 2020-02-02 00:00:00.000000 adadpython-0.0.3/README.md
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 adadpython-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6470 2020-02-02 00:00:00.000000 adadpython-0.0.3/PKG-INFO
```

### Comparing `adadpython-0.0.2/src/adadpython/base_pokemon.py` & `adadpython-0.0.3/src/adadpython/base_pokemon.py`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.2/src/adadpython/dexpoke.py` & `adadpython-0.0.3/src/adadpython/dexpoke.py`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.2/src/adadpython/moves.py` & `adadpython-0.0.3/src/adadpython/moves.py`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.2/src/adadpython/pokemon.py` & `adadpython-0.0.3/src/adadpython/pokemon.py`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.2/src/adadpython/save2.npy` & `adadpython-0.0.3/src/adadpython/save2.npy`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.2/src/adadpython/somemons.dat` & `adadpython-0.0.3/src/adadpython/somemons.dat`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.2/src/adadpython/texter.py` & `adadpython-0.0.3/src/adadpython/texter.py`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.2/src/adadpython/trainerai.py` & `adadpython-0.0.3/src/adadpython/trainerai.py`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.2/src/adadpython/victoryroad.py` & `adadpython-0.0.3/src/adadpython/victoryroad.py`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.2/src/adadpython/LICENSES/numpy_license.txt` & `adadpython-0.0.3/src/adadpython/LICENSES/numpy_license.txt`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.2/src/adadpython/LICENSES/python_license.txt` & `adadpython-0.0.3/src/adadpython/LICENSES/python_license.txt`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.2/src/adadpython/documentation/CREDITS.txt` & `adadpython-0.0.3/src/adadpython/documentation/CREDITS.txt`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.2/src/adadpython/documentation/game_blurb.md` & `adadpython-0.0.3/src/adadpython/documentation/game_blurb.md`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.2/src/adadpython/documentation/log.md` & `adadpython-0.0.3/src/adadpython/documentation/log.md`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.2/src/adadpython/documentation/archive/moremon.py` & `adadpython-0.0.3/src/adadpython/documentation/archive/moremon.py`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.2/src/adadpython/documentation/archive/saved_dexpoke.npy` & `adadpython-0.0.3/src/adadpython/documentation/archive/saved_dexpoke.npy`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.2/src/adadpython/documentation/archive/saved_movedex.npy` & `adadpython-0.0.3/src/adadpython/documentation/archive/saved_movedex.npy`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.2/src/adadpython/documentation/archive/saved_natures.npy` & `adadpython-0.0.3/src/adadpython/documentation/archive/saved_natures.npy`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.2/src/adadpython/documentation/archive/somemons_copy.txt` & `adadpython-0.0.3/src/adadpython/documentation/archive/somemons_copy.txt`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.2/src/adadpython/elite5/elite_1.npy` & `adadpython-0.0.3/src/adadpython/elite5/elite_1.npy`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.2/src/adadpython/elite5/elite_2.npy` & `adadpython-0.0.3/src/adadpython/elite5/elite_2.npy`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.2/src/adadpython/elite5/elite_3.npy` & `adadpython-0.0.3/src/adadpython/elite5/elite_3.npy`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.2/src/adadpython/elite5/elite_4.npy` & `adadpython-0.0.3/src/adadpython/elite5/elite_4.npy`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.2/src/adadpython/elite5/elite_5.npy` & `adadpython-0.0.3/src/adadpython/elite5/elite_5.npy`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.2/LICENSE` & `adadpython-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.2/README.md` & `adadpython-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `adadpython-0.0.2/pyproject.toml` & `adadpython-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "adadpython"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Antoine" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `adadpython-0.0.2/PKG-INFO` & `adadpython-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: adadpython
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Project-URL: Homepage, https://github.com/
 Project-URL: Issues, https://github.com/issues
 Author: Antoine
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


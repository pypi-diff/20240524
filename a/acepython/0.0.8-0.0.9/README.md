# Comparing `tmp/acepython-0.0.8.tar.gz` & `tmp/acepython-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acepython-0.0.8.tar", last modified: Thu Jan 18 10:43:51 2024, max compression
+gzip compressed data, was "acepython-0.0.9.tar", last modified: Thu Jan 18 10:52:42 2024, max compression
```

## Comparing `acepython-0.0.8.tar` & `acepython-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     3690 2024-01-18 10:42:09.000000 acepython-0.0.8/.cirrus.yml
--rw-r--r--   0        0        0     1799 2024-01-18 10:42:09.000000 acepython-0.0.8/.github/labels.yml
--rw-r--r--   0        0        0      728 2024-01-18 10:42:09.000000 acepython-0.0.8/.github/release-drafter.yml
--rw-r--r--   0        0        0     6777 2024-01-18 10:42:09.000000 acepython-0.0.8/.github/workflows/build_wheels.yml
--rw-r--r--   0        0        0     1350 2024-01-18 10:42:09.000000 acepython-0.0.8/.github/workflows/donotrun.release.yml.old
--rw-r--r--   0        0        0     1470 2024-01-18 10:42:09.000000 acepython-0.0.8/.github/workflows/tests.yml
--rw-r--r--   0        0        0     1909 2024-01-18 10:42:09.000000 acepython-0.0.8/.gitignore
--rw-r--r--   0        0        0     1505 2024-01-18 10:42:09.000000 acepython-0.0.8/LICENSE.md
--rw-r--r--   0        0        0     6927 2024-01-18 10:42:09.000000 acepython-0.0.8/README.md
--rw-r--r--   0        0        0    30467 2024-01-18 10:42:09.000000 acepython-0.0.8/ace_data/Data/NASA.therm
--rw-r--r--   0        0        0     3990 2024-01-18 10:42:09.000000 acepython-0.0.8/ace_data/Data/composes.dat
--rw-r--r--   0        0        0    28121 2024-01-18 10:42:09.000000 acepython-0.0.8/ace_sources/Md_ACE.f90
--rw-r--r--   0        0        0    14282 2024-01-18 10:42:09.000000 acepython-0.0.8/ace_sources/Md_Constantes.f90
--rw-r--r--   0        0        0      401 2024-01-18 10:42:09.000000 acepython-0.0.8/ace_sources/Md_Types_Numeriques.f90
--rw-r--r--   0        0        0    44515 2024-01-18 10:42:09.000000 acepython-0.0.8/ace_sources/Md_Utilitaires.f90
--rw-r--r--   0        0        0    11748 2024-01-18 10:42:09.000000 acepython-0.0.8/ace_sources/Md_numerical_recipes.f90
--rw-r--r--   0        0        0     1421 2024-01-18 10:42:09.000000 acepython-0.0.8/ace_sources/ace.pyf
--rw-r--r--   0        0        0     2101 2024-01-18 10:42:09.000000 acepython-0.0.8/cirrus/cirrus_wheel.yml
--rw-r--r--   0        0        0    96372 2024-01-18 10:42:09.000000 acepython-0.0.8/examples/ace_example.svg
--rw-r--r--   0        0        0      930 2024-01-18 10:42:09.000000 acepython-0.0.8/examples/run_chemistry.py
--rw-r--r--   0        0        0     4303 2024-01-18 10:42:09.000000 acepython-0.0.8/meson.build
--rw-r--r--   0        0        0     1449 2024-01-18 10:42:09.000000 acepython-0.0.8/noxfile.py
--rw-r--r--   0        0        0     1874 2024-01-18 10:42:09.000000 acepython-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       25 2024-01-18 10:42:09.000000 acepython-0.0.8/src/acepython/__init__.py
--rw-r--r--   0        0        0     2710 2024-01-18 10:42:09.000000 acepython-0.0.8/src/acepython/ace.py
--rw-r--r--   0        0        0     1696 2024-01-18 10:42:09.000000 acepython-0.0.8/src/acepython/meson.build
--rw-r--r--   0        0        0     7171 2024-01-18 10:42:09.000000 acepython-0.0.8/src/acepython/taurex3.py
--rw-r--r--   0        0        0      561 2024-01-18 10:42:09.000000 acepython-0.0.8/tests/test_ace.py
--rw-r--r--   0        0        0      173 2024-01-18 10:42:09.000000 acepython-0.0.8/tools/build_sdist.sh
--rw-r--r--   0        0        0    13295 2024-01-18 10:42:09.000000 acepython-0.0.8/tools/openblas_support.py
--rw-r--r--   0        0        0      190 2024-01-18 10:42:09.000000 acepython-0.0.8/tools/test_sdist.sh
--rw-r--r--   0        0        0        7 2024-01-18 10:42:09.000000 acepython-0.0.8/tools/wheels/cibw_before_build_linux.sh
--rw-r--r--   0        0        0     2314 2024-01-18 10:42:09.000000 acepython-0.0.8/tools/wheels/cibw_before_build_macos.sh
--rw-r--r--   0        0        0     1228 2024-01-18 10:42:09.000000 acepython-0.0.8/tools/wheels/cibw_before_build_win.sh
--rw-r--r--   0        0        0      925 2024-01-18 10:42:09.000000 acepython-0.0.8/tools/wheels/publish_cirrus.sh
--rw-r--r--   0        0        0     8489 2024-01-18 10:43:51.521377 acepython-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     3711 2024-01-18 10:50:45.000000 acepython-0.0.9/.cirrus.yml
+-rw-r--r--   0        0        0     1799 2024-01-18 10:50:45.000000 acepython-0.0.9/.github/labels.yml
+-rw-r--r--   0        0        0      728 2024-01-18 10:50:45.000000 acepython-0.0.9/.github/release-drafter.yml
+-rw-r--r--   0        0        0     6777 2024-01-18 10:50:45.000000 acepython-0.0.9/.github/workflows/build_wheels.yml
+-rw-r--r--   0        0        0     1350 2024-01-18 10:50:45.000000 acepython-0.0.9/.github/workflows/donotrun.release.yml.old
+-rw-r--r--   0        0        0     1470 2024-01-18 10:50:45.000000 acepython-0.0.9/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     1909 2024-01-18 10:50:45.000000 acepython-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1505 2024-01-18 10:50:45.000000 acepython-0.0.9/LICENSE.md
+-rw-r--r--   0        0        0     6927 2024-01-18 10:50:45.000000 acepython-0.0.9/README.md
+-rw-r--r--   0        0        0    30467 2024-01-18 10:50:45.000000 acepython-0.0.9/ace_data/Data/NASA.therm
+-rw-r--r--   0        0        0     3990 2024-01-18 10:50:45.000000 acepython-0.0.9/ace_data/Data/composes.dat
+-rw-r--r--   0        0        0    28121 2024-01-18 10:50:45.000000 acepython-0.0.9/ace_sources/Md_ACE.f90
+-rw-r--r--   0        0        0    14282 2024-01-18 10:50:45.000000 acepython-0.0.9/ace_sources/Md_Constantes.f90
+-rw-r--r--   0        0        0      401 2024-01-18 10:50:45.000000 acepython-0.0.9/ace_sources/Md_Types_Numeriques.f90
+-rw-r--r--   0        0        0    44515 2024-01-18 10:50:45.000000 acepython-0.0.9/ace_sources/Md_Utilitaires.f90
+-rw-r--r--   0        0        0    11748 2024-01-18 10:50:45.000000 acepython-0.0.9/ace_sources/Md_numerical_recipes.f90
+-rw-r--r--   0        0        0     1421 2024-01-18 10:50:45.000000 acepython-0.0.9/ace_sources/ace.pyf
+-rw-r--r--   0        0        0     2101 2024-01-18 10:50:45.000000 acepython-0.0.9/cirrus/cirrus_wheel.yml
+-rw-r--r--   0        0        0    96372 2024-01-18 10:50:45.000000 acepython-0.0.9/examples/ace_example.svg
+-rw-r--r--   0        0        0      930 2024-01-18 10:50:45.000000 acepython-0.0.9/examples/run_chemistry.py
+-rw-r--r--   0        0        0     4303 2024-01-18 10:50:45.000000 acepython-0.0.9/meson.build
+-rw-r--r--   0        0        0     1449 2024-01-18 10:50:45.000000 acepython-0.0.9/noxfile.py
+-rw-r--r--   0        0        0     1874 2024-01-18 10:50:45.000000 acepython-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       25 2024-01-18 10:50:45.000000 acepython-0.0.9/src/acepython/__init__.py
+-rw-r--r--   0        0        0     2710 2024-01-18 10:50:45.000000 acepython-0.0.9/src/acepython/ace.py
+-rw-r--r--   0        0        0     1696 2024-01-18 10:50:45.000000 acepython-0.0.9/src/acepython/meson.build
+-rw-r--r--   0        0        0     7171 2024-01-18 10:50:45.000000 acepython-0.0.9/src/acepython/taurex3.py
+-rw-r--r--   0        0        0      561 2024-01-18 10:50:45.000000 acepython-0.0.9/tests/test_ace.py
+-rw-r--r--   0        0        0      173 2024-01-18 10:50:45.000000 acepython-0.0.9/tools/build_sdist.sh
+-rw-r--r--   0        0        0    13295 2024-01-18 10:50:45.000000 acepython-0.0.9/tools/openblas_support.py
+-rw-r--r--   0        0        0      190 2024-01-18 10:50:45.000000 acepython-0.0.9/tools/test_sdist.sh
+-rw-r--r--   0        0        0        7 2024-01-18 10:50:45.000000 acepython-0.0.9/tools/wheels/cibw_before_build_linux.sh
+-rw-r--r--   0        0        0     2314 2024-01-18 10:50:45.000000 acepython-0.0.9/tools/wheels/cibw_before_build_macos.sh
+-rw-r--r--   0        0        0     1228 2024-01-18 10:50:45.000000 acepython-0.0.9/tools/wheels/cibw_before_build_win.sh
+-rw-r--r--   0        0        0      925 2024-01-18 10:50:45.000000 acepython-0.0.9/tools/wheels/publish_cirrus.sh
+-rw-r--r--   0        0        0     8489 2024-01-18 10:52:42.898106 acepython-0.0.9/PKG-INFO
```

### Comparing `acepython-0.0.8/.cirrus.yml` & `acepython-0.0.9/.cirrus.yml`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
       exit 0
     fi
 
     if [[ "$GITHUB_TOKEN" == "" ]]; then
       echo "Please provide GitHub access token via GITHUB_TOKEN environment variable!"
       exit 1
     fi
-
+    pip install twine
     mkdir dist
     cp wheelhouse/* dist/
 
     python -m twine upload dist/
 
 
     file_content_type="application/octet-stream"
```

### Comparing `acepython-0.0.8/.github/labels.yml` & `acepython-0.0.9/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `acepython-0.0.8/.github/release-drafter.yml` & `acepython-0.0.9/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `acepython-0.0.8/.github/workflows/build_wheels.yml` & `acepython-0.0.9/.github/workflows/build_wheels.yml`

 * *Files identical despite different names*

### Comparing `acepython-0.0.8/.github/workflows/donotrun.release.yml.old` & `acepython-0.0.9/.github/workflows/donotrun.release.yml.old`

 * *Files identical despite different names*

### Comparing `acepython-0.0.8/.github/workflows/tests.yml` & `acepython-0.0.9/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `acepython-0.0.8/.gitignore` & `acepython-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `acepython-0.0.8/LICENSE.md` & `acepython-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `acepython-0.0.8/README.md` & `acepython-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `acepython-0.0.8/ace_data/Data/NASA.therm` & `acepython-0.0.9/ace_data/Data/NASA.therm`

 * *Files identical despite different names*

### Comparing `acepython-0.0.8/ace_data/Data/composes.dat` & `acepython-0.0.9/ace_data/Data/composes.dat`

 * *Files identical despite different names*

### Comparing `acepython-0.0.8/ace_sources/Md_ACE.f90` & `acepython-0.0.9/ace_sources/Md_ACE.f90`

 * *Files identical despite different names*

### Comparing `acepython-0.0.8/ace_sources/Md_Constantes.f90` & `acepython-0.0.9/ace_sources/Md_Constantes.f90`

 * *Files identical despite different names*

### Comparing `acepython-0.0.8/ace_sources/Md_Utilitaires.f90` & `acepython-0.0.9/ace_sources/Md_Utilitaires.f90`

 * *Files identical despite different names*

### Comparing `acepython-0.0.8/ace_sources/Md_numerical_recipes.f90` & `acepython-0.0.9/ace_sources/Md_numerical_recipes.f90`

 * *Files identical despite different names*

### Comparing `acepython-0.0.8/ace_sources/ace.pyf` & `acepython-0.0.9/ace_sources/ace.pyf`

 * *Files identical despite different names*

### Comparing `acepython-0.0.8/cirrus/cirrus_wheel.yml` & `acepython-0.0.9/cirrus/cirrus_wheel.yml`

 * *Files identical despite different names*

### Comparing `acepython-0.0.8/examples/ace_example.svg` & `acepython-0.0.9/examples/ace_example.svg`

 * *Files identical despite different names*

### Comparing `acepython-0.0.8/examples/run_chemistry.py` & `acepython-0.0.9/examples/run_chemistry.py`

 * *Files identical despite different names*

### Comparing `acepython-0.0.8/meson.build` & `acepython-0.0.9/meson.build`

 * *Files identical despite different names*

### Comparing `acepython-0.0.8/noxfile.py` & `acepython-0.0.9/noxfile.py`

 * *Files identical despite different names*

### Comparing `acepython-0.0.8/pyproject.toml` & `acepython-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 [project]
 name = "acepython"
 description = "Python wrapper for the FORTRAN ACE code."
 dependencies = [
     "numpy>=1.25.0",
     "astropy>=5.0.0",
 ]
-version="0.0.8"
+version="0.0.9"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
     {name = "Ahmed F. Al-Refaie", email = "ahmed.al-refaie.12@ucl.ac.uk"},
 ]
 maintainers = [
     {name = "Ahmed F. Al-Refaie", email = "ahmed.al-refaie.12@ucl.ac.uk"},
```

### Comparing `acepython-0.0.8/src/acepython/ace.py` & `acepython-0.0.9/src/acepython/ace.py`

 * *Files identical despite different names*

### Comparing `acepython-0.0.8/src/acepython/meson.build` & `acepython-0.0.9/src/acepython/meson.build`

 * *Files identical despite different names*

### Comparing `acepython-0.0.8/src/acepython/taurex3.py` & `acepython-0.0.9/src/acepython/taurex3.py`

 * *Files identical despite different names*

### Comparing `acepython-0.0.8/tests/test_ace.py` & `acepython-0.0.9/tests/test_ace.py`

 * *Files identical despite different names*

### Comparing `acepython-0.0.8/tools/openblas_support.py` & `acepython-0.0.9/tools/openblas_support.py`

 * *Files identical despite different names*

### Comparing `acepython-0.0.8/tools/wheels/cibw_before_build_macos.sh` & `acepython-0.0.9/tools/wheels/cibw_before_build_macos.sh`

 * *Files identical despite different names*

### Comparing `acepython-0.0.8/tools/wheels/cibw_before_build_win.sh` & `acepython-0.0.9/tools/wheels/cibw_before_build_win.sh`

 * *Files identical despite different names*

### Comparing `acepython-0.0.8/tools/wheels/publish_cirrus.sh` & `acepython-0.0.9/tools/wheels/publish_cirrus.sh`

 * *Files identical despite different names*

### Comparing `acepython-0.0.8/PKG-INFO` & `acepython-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acepython
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python wrapper for the FORTRAN ACE code.
 Keywords: taurex taurex3 exoplanet exoplanets transmission spectroscopy atmospheres atmosphere chemistry equilibrium-chemistry chemistry-solver chemistry-equilibrium chemistry-equilibrium-solver fortran
 Author-Email: Ahmed F. Al-Refaie <ahmed.al-refaie.12@ucl.ac.uk>
 Maintainer-Email: Ahmed F. Al-Refaie <ahmed.al-refaie.12@ucl.ac.uk>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: acepython Version: 0.0.8 Summary: Python wrapper
+Metadata-Version: 2.1 Name: acepython Version: 0.0.9 Summary: Python wrapper
 for the FORTRAN ACE code. Keywords: taurex taurex3 exoplanet exoplanets
 transmission spectroscopy atmospheres atmosphere chemistry equilibrium-
 chemistry chemistry-solver chemistry-equilibrium chemistry-equilibrium-solver
 fortran Author-Email: Ahmed F. Al-Refaie
 ucl.ac.uk> Maintainer-Email: Ahmed F. Al-Refaie
 ucl.ac.uk> Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Education
```


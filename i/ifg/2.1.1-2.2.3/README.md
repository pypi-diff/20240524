# Comparing `tmp/ifg-2.1.1.tar.gz` & `tmp/ifg-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifg-2.1.1.tar", max compression
+gzip compressed data, was "ifg-2.2.3.tar", max compression
```

## Comparing `ifg-2.1.1.tar` & `ifg-2.2.3.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1077 2021-09-27 14:30:22.127304 ifg-2.1.1/LICENSE.txt
--rw-r--r--   0        0        0     1428 2021-09-27 14:30:22.127304 ifg-2.1.1/README.md
--rw-r--r--   0        0        0     1255 2021-09-27 14:30:22.127304 ifg-2.1.1/ifg/__init__.py
--rw-r--r--   0        0        0    19478 2021-09-27 14:30:22.127304 ifg-2.1.1/ifg/calculator.py
--rw-r--r--   0        0        0      927 2021-09-27 14:30:22.127304 ifg-2.1.1/ifg/examples.py
--rw-r--r--   0        0        0       22 2021-09-27 14:30:23.259309 ifg-2.1.1/ifg/metadata.py
--rw-r--r--   0        0        0     5237 2021-09-27 14:30:22.127304 ifg-2.1.1/ifg/units_converter.py
--rw-r--r--   0        0        0      525 2021-09-27 14:30:22.127304 ifg-2.1.1/ifg/utils.py
--rw-r--r--   0        0        0     3567 2021-09-27 14:30:23.283309 ifg-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     2688 2021-09-27 14:30:36.831115 ifg-2.1.1/setup.py
--rw-r--r--   0        0        0     3185 2021-09-27 14:30:36.831508 ifg-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-24 09:51:50.524205 ifg-2.2.3/LICENSE.txt
+-rw-r--r--   0        0        0     1428 2024-05-24 09:51:50.524205 ifg-2.2.3/README.md
+-rw-r--r--   0        0        0     1255 2024-05-24 09:51:50.524205 ifg-2.2.3/ifg/__init__.py
+-rw-r--r--   0        0        0    19485 2024-05-24 09:51:50.524205 ifg-2.2.3/ifg/calculator.py
+-rw-r--r--   0        0        0      927 2024-05-24 09:51:50.524205 ifg-2.2.3/ifg/examples.py
+-rw-r--r--   0        0        0       22 2024-05-24 09:51:50.524205 ifg-2.2.3/ifg/metadata.py
+-rw-r--r--   0        0        0     5043 2024-05-24 09:51:50.524205 ifg-2.2.3/ifg/units_converter.py
+-rw-r--r--   0        0        0      525 2024-05-24 09:51:50.524205 ifg-2.2.3/ifg/utils.py
+-rw-r--r--   0        0        0     2180 2024-05-24 09:51:52.208217 ifg-2.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3151 1970-01-01 00:00:00.000000 ifg-2.2.3/PKG-INFO
```

### Comparing `ifg-2.1.1/LICENSE.txt` & `ifg-2.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ifg-2.1.1/README.md` & `ifg-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ifg-2.1.1/ifg/__init__.py` & `ifg-2.2.3/ifg/__init__.py`

 * *Files identical despite different names*

### Comparing `ifg-2.1.1/ifg/calculator.py` & `ifg-2.2.3/ifg/calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     y = chemical_potential / tt
     F = gbar / np.sqrt(2.0) / np.pi ** 2 * tt ** (2.5) * vv
     F *= y * _1d_call(_fdk, y, k=0.5) - 2.0 / 3.0 * _1d_call(_fdk, y, k=1.5)
     return F
 
 
 def get_pressure(vv, tt, chemical_potential, gbar=2.0, *args, **kwargs):
-    # type: (np.ndarray, np.ndarray, float, list, dict) -> np.ndarray
+    # type: (np.ndarray, np.ndarray, float, list, tuple, dict) -> np.ndarray
     """Get IFG pressure P in atomic units.
 
     :param vv: Matrix of specific volumes in atomic units.
     :param tt: Matrix of temperatures in atomic units.
     :param chemical_potential: Chemical potential in atomic units.
     :param gbar: degeneracy factor, for IFG g = 2s + 1
     :return: P[i][j] - Pressure in atomic units.
@@ -498,10 +498,10 @@
                 for i, volume in enumerate(self.vv[0, :]):
                     dump_to_csv(
                         os.path.join(
                             os.getcwd(),
                             csv_dir,
                             "{}_v={}_atomic_units.csv".format(key, volume),
                         ),
-                        np.array([self.tt[0, :], value[:, i]]).T,
+                        np.array([self.tt[:, 0], value[:, i]]).T,
                     )
         return properties
```

### Comparing `ifg-2.1.1/ifg/examples.py` & `ifg-2.2.3/ifg/examples.py`

 * *Files identical despite different names*

### Comparing `ifg-2.1.1/ifg/units_converter.py` & `ifg-2.2.3/ifg/units_converter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,38 @@
-from typing import Iterable, Union
-
 import numpy as np
-import scipy.constants as const
-from scipy.constants import physical_constants
+
+PI = 3.141592653589793
+BOHR_RADIUS = 5.29177210903e-11
+ELEMENTARY_CHARGE = 1.602176634e-19
+BOLTZMANN_CONSTANT = 1.380649e-23
+ELECTRIC_CONSTANT = 8.8541878128e-12
+ATOMIC_UNIT_OF_LENGTH = 5.29177210903e-11
+ATOMIC_UNIT_OF_TIME = 2.4188843265857e-17
+AVOGADRO_CONSTANT = 6.02214076e+23
 
 
 class SiAtomicConverter:
     def __init__(self, from_si=True):
         """Class for converting from SI units to atomic (and visa versa)
 
         :param from_si: Whether to convert from SI or atomic
         """
         self.from_si = from_si
         # self.ab - Bohr radius
-        self.ab = physical_constants["Bohr radius"][0]
+        self.ab = BOHR_RADIUS
         # self.ab3 - Bohr radius to the 3rd power
         self.ab3 = self.ab * self.ab * self.ab
         # self.ec = elementary charge
-        self.ec = physical_constants["elementary charge"][0]
+        self.ec = ELEMENTARY_CHARGE
         # self.kb - Boltzmann constant
-        self.kb = physical_constants["Boltzmann constant"][0]
+        self.kb = BOLTZMANN_CONSTANT
         # self.e0 - Vacuum permeatbility
-        self.e0 = physical_constants["electric constant"][0]
+        self.e0 = ELECTRIC_CONSTANT
         # self.ha - Hartree energy in Joules
-        self.ha = 0.25 * self.ec * self.ec / const.pi / self.e0 / self.ab
+        self.ha = 0.25 * self.ec * self.ec / PI / self.e0 / self.ab
 
     def convert_energy(self, energy):
         """Converts energy.
 
         :param energy: Energy in corresponding units system
         :return: Converted energy
         """
@@ -93,42 +98,34 @@
     def convert_sound_speed(self, sound_speed):
         """Converts sound speed.
 
         :param sound_speed: Sound speed in corresponding units system
         :return: Converted sound speed
         """
         if self.from_si:
-            return (
-                sound_speed
-                / physical_constants["atomic unit of length"][0]
-                * physical_constants["atomic unit of time"][0]
-            )
-        else:
-            return (
-                sound_speed
-                * physical_constants["atomic unit of length"][0]
-                / physical_constants["atomic unit of time"][0]
-            )
+            return sound_speed / ATOMIC_UNIT_OF_LENGTH * ATOMIC_UNIT_OF_TIME
+        else:
+            return sound_speed * ATOMIC_UNIT_OF_LENGTH / ATOMIC_UNIT_OF_TIME
 
     # TODO: ignores `from_si` parameter
 
 
 def convert_density(density_sgs, molar_mass_sgs):
     """
     Converts density from g/cm^3 to specific volume in SI using molar mass.
     NOTE: ignores `from_si` parameter
 
     :param density_sgs: g/cm^3
     :param molar_mass_sgs: g/mol
     :return: specific volume in SI, m^3
     """
     # Per one mol
-    v_si = molar_mass_sgs / density_sgs / 10 ** 6
+    v_si = molar_mass_sgs / density_sgs / 10**6
     # Per one particle
-    v_si /= physical_constants["Avogadro constant"][0]
+    v_si /= AVOGADRO_CONSTANT
     return v_si
 
 
 def get_metal_specific_volume(density_sgs, molar_mass_sgs, num_electrons):
     """Calculate metal's specific volume from its density, molar mass and
     number of electrons on outer shell.
 
@@ -162,8 +159,8 @@
 
     where k = (3 pi^2 * 1/v)^(1/3) is a Fermi wavevector.
 
     The volume should be in atomic units
     """
     tt, vv = np.meshgrid(theta, volumes)
     # 2-d array
-    return tt / 2 * (3 * np.pi ** 2 / vv) ** (2 / 3)
+    return tt / 2. * (3 * np.pi**2 / vv) ** (2. / 3)
```

### Comparing `ifg-2.1.1/ifg/utils.py` & `ifg-2.2.3/ifg/utils.py`

 * *Files identical despite different names*

### Comparing `ifg-2.1.1/PKG-INFO` & `ifg-2.2.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 Metadata-Version: 2.1
 Name: ifg
-Version: 2.1.1
+Version: 2.2.3
 Summary: Calculator of Ideal Fermi gas properties
 Home-page: https://github.com/alekseik1/ifg-py
 License: MIT
 Author: Aleksei Kozharin
 Author-email: 1alekseik1@gmail.com
 Maintainer: Aleksei Kozharin
 Maintainer-email: 1alekseik1@gmail.com
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*
+Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: fdint (>=2.0,<3.0)
-Requires-Dist: numpy (>=1.16.6,<2.0.0); python_version ~= "2.7"
-Requires-Dist: numpy (>=1.18.5,<2.0.0); python_version ~= "3.5.2"
-Requires-Dist: numpy (>=1.19.5,<2.0.0); python_version ~= "3.6"
-Requires-Dist: numpy (>=1.20.3,<2.0.0); python_version ~= "3.7"
-Requires-Dist: numpy (>=1.20.3,<2.0.0); python_version ~= "3.8"
-Requires-Dist: numpy (>=1.20.3,<2.0.0); python_version ~= "3.9"
-Requires-Dist: scipy (>=1.2,<2.0); python_version ~= "2.7"
-Requires-Dist: scipy (>=1.4,<2.0); python_version ~= "3.5.2"
-Requires-Dist: scipy (>=1.5,<2.0); python_version ~= "3.6"
-Requires-Dist: scipy (>=1.6,<2.0); python_version ~= "3.7"
-Requires-Dist: scipy (>=1.6,<2.0); python_version ~= "3.8"
-Requires-Dist: scipy (>=1.6,<2.0); python_version ~= "3.9"
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: fdint_py3 (>=2.0.2,<3.0.0)
+Requires-Dist: numpy (>=1.13.3,<=1.17.3) ; python_version >= "3.5" and python_version < "3.6"
+Requires-Dist: numpy (>=1.14.5,<=1.19.3) ; python_version >= "3.6" and python_version < "3.7"
+Requires-Dist: numpy (>=1.16.5,<=1.20) ; python_version >= "3.7" and python_version < "3.8"
+Requires-Dist: numpy (>=1.17.3,<1.24.0) ; python_version >= "3.8" and python_version < "3.9"
+Requires-Dist: numpy (>=1.22.4,<2.0.0) ; python_version >= "3.9" and python_version < "4.0"
+Requires-Dist: numpy (>=1.8.2,<=1.16) ; python_version >= "2.7" and python_version < "3.5"
 Project-URL: Documentation, https://ifg-py.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/alekseik1/ifg-py
 Description-Content-Type: text/markdown
 
 # Numerical ideal Fermi gas
 
 [![Documentation Status](https://readthedocs.org/projects/ifg-py/badge/?version=latest)](https://ifg-py.readthedocs.io/en/latest/?badge=latest)
```


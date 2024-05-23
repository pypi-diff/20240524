# Comparing `tmp/comp_chem_utils-0.0.1.tar.gz` & `tmp/comp_chem_utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comp_chem_utils-0.0.1.tar", max compression
+gzip compressed data, was "comp_chem_utils-0.0.2.tar", max compression
```

## Comparing `comp_chem_utils-0.0.1.tar` & `comp_chem_utils-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,54 @@
--rwxr-xr-x   0        0        0       62 2023-06-21 08:52:58.000000 comp_chem_utils-0.0.1/AUTHORS.rst
--rwxr-xr-x   0        0        0       86 2023-06-22 21:41:22.000000 comp_chem_utils-0.0.1/CHANGELOG.rst
--rwxr-xr-x   0        0        0     2428 2023-06-22 21:58:43.000000 comp_chem_utils-0.0.1/CONTRIBUTING.rst
--rwxr-xr-x   0        0        0     1103 2023-04-05 14:52:54.000000 comp_chem_utils-0.0.1/LICENSE
--rwxr-xr-x   0        0        0     2962 2023-06-22 21:58:43.000000 comp_chem_utils-0.0.1/README.rst
--rwxr-xr-x   0        0        0     3140 2023-06-22 21:59:34.000000 comp_chem_utils-0.0.1/pyproject.toml
--rwxr-xr-x   0        0        0      215 2023-06-22 21:58:32.000000 comp_chem_utils-0.0.1/src/ccu/__init__.py
--rwxr-xr-x   0        0        0      400 2023-06-22 21:20:06.000000 comp_chem_utils-0.0.1/src/ccu/__main__.py
--rwxr-xr-x   0        0        0        0 2023-06-22 21:20:06.000000 comp_chem_utils-0.0.1/src/ccu/adsorption/__init__.py
--rwxr-xr-x   0        0        0    12600 2023-06-22 21:20:06.000000 comp_chem_utils-0.0.1/src/ccu/adsorption/adsorbatecomplex.py
--rwxr-xr-x   0        0        0     8294 2023-06-22 21:20:06.000000 comp_chem_utils-0.0.1/src/ccu/adsorption/adsorbateorientation.py
--rwxr-xr-x   0        0        0     8925 2023-06-22 21:20:07.000000 comp_chem_utils-0.0.1/src/ccu/adsorption/adsorbates.py
--rwxr-xr-x   0        0        0     2182 2023-06-22 21:20:07.000000 comp_chem_utils-0.0.1/src/ccu/adsorption/cli.py
--rwxr-xr-x   0        0        0     9976 2023-06-22 21:20:07.000000 comp_chem_utils-0.0.1/src/ccu/adsorption/sitefinder.py
--rwxr-xr-x   0        0        0        0 2023-05-31 03:55:11.000000 comp_chem_utils-0.0.1/src/ccu/cli/__init__.py
--rwxr-xr-x   0        0        0     1216 2023-06-22 21:22:41.000000 comp_chem_utils-0.0.1/src/ccu/cli/main.py
--rwxr-xr-x   0        0        0        0 2023-05-31 03:55:12.000000 comp_chem_utils-0.0.1/src/ccu/structure/__init__.py
--rwxr-xr-x   0        0        0     8545 2023-06-22 21:20:07.000000 comp_chem_utils-0.0.1/src/ccu/structure/axisfinder.py
--rwxr-xr-x   0        0        0      697 2023-06-22 21:20:08.000000 comp_chem_utils-0.0.1/src/ccu/structure/cli.py
--rwxr-xr-x   0        0        0    10694 2023-06-22 21:20:08.000000 comp_chem_utils-0.0.1/src/ccu/structure/comparator.py
--rwxr-xr-x   0        0        0     2760 2023-06-22 21:20:08.000000 comp_chem_utils-0.0.1/src/ccu/structure/fingerprint.py
--rwxr-xr-x   0        0        0      941 2023-06-22 21:20:08.000000 comp_chem_utils-0.0.1/src/ccu/structure/geometry.py
--rwxr-xr-x   0        0        0      702 2023-06-22 21:20:08.000000 comp_chem_utils-0.0.1/src/ccu/structure/resizecell.py
--rwxr-xr-x   0        0        0     4075 2023-06-22 21:20:09.000000 comp_chem_utils-0.0.1/src/ccu/structure/symmetry.py
--rw-r--r--   0        0        0     4047 1970-01-01 00:00:00.000000 comp_chem_utils-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      117 2024-05-23 21:57:14.830101 comp_chem_utils-0.0.2/AUTHORS.rst
+-rw-r--r--   0        0        0     1103 2023-07-28 23:31:08.263578 comp_chem_utils-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2908 2024-05-23 22:12:09.791916 comp_chem_utils-0.0.2/README.rst
+-rw-r--r--   0        0        0     4438 2024-05-23 22:24:55.612002 comp_chem_utils-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      215 2024-05-23 22:30:30.131012 comp_chem_utils-0.0.2/src/ccu/__init__.py
+-rw-r--r--   0        0        0      401 2024-05-23 22:30:30.131479 comp_chem_utils-0.0.2/src/ccu/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-23 17:24:09.684819 comp_chem_utils-0.0.2/src/ccu/adsorption/__init__.py
+-rw-r--r--   0        0        0    13917 2024-05-23 22:24:55.613093 comp_chem_utils-0.0.2/src/ccu/adsorption/adsorbatecomplex.py
+-rw-r--r--   0        0        0     8294 2024-05-23 22:04:51.830201 comp_chem_utils-0.0.2/src/ccu/adsorption/adsorbateorientation.py
+-rw-r--r--   0        0        0     9985 2024-05-23 22:05:08.945902 comp_chem_utils-0.0.2/src/ccu/adsorption/adsorbates.py
+-rw-r--r--   0        0        0     2270 2024-05-23 22:24:55.613553 comp_chem_utils-0.0.2/src/ccu/adsorption/cli.py
+-rw-r--r--   0        0        0    10107 2024-05-23 22:24:55.616573 comp_chem_utils-0.0.2/src/ccu/adsorption/sitefinder.py
+-rw-r--r--   0        0        0     1907 2024-05-23 21:57:14.847461 comp_chem_utils-0.0.2/src/ccu/bader/analysis.py
+-rw-r--r--   0        0        0     3077 2024-05-23 22:24:55.616939 comp_chem_utils-0.0.2/src/ccu/bader/bader_analysis.py
+-rw-r--r--   0        0        0     4077 2024-05-23 22:24:55.617270 comp_chem_utils-0.0.2/src/ccu/bader/cli.py
+-rw-r--r--   0        0        0        0 2024-05-23 17:22:36.572484 comp_chem_utils-0.0.2/src/ccu/cli/__init__.py
+-rw-r--r--   0        0        0     1379 2024-05-23 22:24:55.617673 comp_chem_utils-0.0.2/src/ccu/cli/main.py
+-rw-r--r--   0        0        0      621 2024-05-23 21:57:14.850381 comp_chem_utils-0.0.2/src/ccu/fancyplots/cli.py
+-rw-r--r--   0        0        0      958 2024-05-23 22:24:55.618004 comp_chem_utils-0.0.2/src/ccu/fancyplots/data.py
+-rw-r--r--   0        0        0    17815 2024-05-23 22:24:55.618395 comp_chem_utils-0.0.2/src/ccu/fancyplots/fancyplots.py
+-rw-r--r--   0        0        0        0 2024-05-23 21:57:14.851377 comp_chem_utils-0.0.2/src/ccu/fancyplots/gui/__init__.py
+-rw-r--r--   0        0        0     4122 2024-05-23 21:57:14.851834 comp_chem_utils-0.0.2/src/ccu/fancyplots/gui/annotation.py
+-rw-r--r--   0        0        0      393 2024-05-23 21:57:14.852169 comp_chem_utils-0.0.2/src/ccu/fancyplots/gui/defaults.py
+-rw-r--r--   0        0        0    14714 2024-05-23 22:24:55.618899 comp_chem_utils-0.0.2/src/ccu/fancyplots/gui/fed.py
+-rw-r--r--   0        0        0     5258 2024-05-23 21:57:14.852942 comp_chem_utils-0.0.2/src/ccu/fancyplots/gui/footer.py
+-rw-r--r--   0        0        0     8313 2024-05-23 21:57:14.853358 comp_chem_utils-0.0.2/src/ccu/fancyplots/gui/main.py
+-rw-r--r--   0        0        0    18941 2024-05-23 22:24:55.620230 comp_chem_utils-0.0.2/src/ccu/fancyplots/gui/mechanism.py
+-rw-r--r--   0        0        0      934 2024-05-23 22:24:55.620700 comp_chem_utils-0.0.2/src/ccu/fancyplots/gui/menu.py
+-rw-r--r--   0        0        0     9284 2024-05-23 21:57:14.854790 comp_chem_utils-0.0.2/src/ccu/fancyplots/gui/parameters.py
+-rw-r--r--   0        0        0     3748 2024-05-23 21:57:14.855294 comp_chem_utils-0.0.2/src/ccu/fancyplots/gui/root.py
+-rw-r--r--   0        0        0     5731 2024-05-23 21:57:14.855650 comp_chem_utils-0.0.2/src/ccu/fancyplots/gui/text.py
+-rw-r--r--   0        0        0     1249 2024-05-23 22:24:55.621157 comp_chem_utils-0.0.2/src/ccu/fancyplots/gui/tooltip.py
+-rw-r--r--   0        0        0     3690 2024-05-23 21:57:14.856979 comp_chem_utils-0.0.2/src/ccu/fancyplots/gui/utils.py
+-rw-r--r--   0        0        0   617438 2024-05-23 22:30:25.625519 comp_chem_utils-0.0.2/src/ccu/fancyplots/images/color_palette.png
+-rw-r--r--   0        0        0   946990 2024-05-23 22:30:25.629872 comp_chem_utils-0.0.2/src/ccu/fancyplots/images/fancy_plots_tutorial.png
+-rw-r--r--   0        0        0        0 2024-05-23 21:57:14.857145 comp_chem_utils-0.0.2/src/ccu/hubbard/__init__.py
+-rw-r--r--   0        0        0    11567 2024-05-23 22:24:55.621676 comp_chem_utils-0.0.2/src/ccu/hubbard/vasp.py
+-rw-r--r--   0        0        0        0 2024-05-23 21:57:14.857676 comp_chem_utils-0.0.2/src/ccu/py.typed
+-rw-r--r--   0        0        0     1150 2024-05-23 21:57:14.857996 comp_chem_utils-0.0.2/src/ccu/relaxation.py
+-rw-r--r--   0        0        0        0 2024-05-23 17:22:36.589057 comp_chem_utils-0.0.2/src/ccu/structure/__init__.py
+-rw-r--r--   0        0        0     8545 2024-05-23 22:05:50.311887 comp_chem_utils-0.0.2/src/ccu/structure/axisfinder.py
+-rw-r--r--   0        0        0     3438 2024-05-23 22:24:55.622192 comp_chem_utils-0.0.2/src/ccu/structure/cli.py
+-rw-r--r--   0        0        0    10680 2024-05-23 22:24:55.622719 comp_chem_utils-0.0.2/src/ccu/structure/comparator.py
+-rw-r--r--   0        0        0     5630 2024-05-23 22:24:55.623193 comp_chem_utils-0.0.2/src/ccu/structure/defects.py
+-rw-r--r--   0        0        0     2768 2024-05-23 22:24:55.623669 comp_chem_utils-0.0.2/src/ccu/structure/fingerprint.py
+-rw-r--r--   0        0        0      941 2024-05-23 17:24:24.366419 comp_chem_utils-0.0.2/src/ccu/structure/geometry.py
+-rw-r--r--   0        0        0      702 2024-05-23 17:24:24.728554 comp_chem_utils-0.0.2/src/ccu/structure/resizecell.py
+-rw-r--r--   0        0        0     4075 2024-05-23 22:06:12.968222 comp_chem_utils-0.0.2/src/ccu/structure/symmetry.py
+-rw-r--r--   0        0        0        0 2024-05-23 21:57:14.862149 comp_chem_utils-0.0.2/src/ccu/thermo/__init__.py
+-rw-r--r--   0        0        0    37453 2024-05-23 21:57:14.862670 comp_chem_utils-0.0.2/src/ccu/thermo/chempot_calculator.py
+-rw-r--r--   0        0        0     7958 2024-05-23 21:57:14.863121 comp_chem_utils-0.0.2/src/ccu/thermo/cli.py
+-rw-r--r--   0        0        0     7242 2024-05-23 21:57:14.863484 comp_chem_utils-0.0.2/src/ccu/thermo/gibbs.py
+-rw-r--r--   0        0        0     2033 2024-05-23 21:57:14.863838 comp_chem_utils-0.0.2/src/ccu/thermo/vibration.py
+-rw-r--r--   0        0        0     4412 1970-01-01 00:00:00.000000 comp_chem_utils-0.0.2/PKG-INFO
```

### Comparing `comp_chem_utils-0.0.1/LICENSE` & `comp_chem_utils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `comp_chem_utils-0.0.1/README.rst` & `comp_chem_utils-0.0.2/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 =============
 CompChemUtils
 =============
 
-CompChemUtils is a set of tools for computational catalysis workflows.
+CompChemUtils is a set of tools for computational chemistry workflows.
 
 Requirements
 ============
 
 * Python_ 3.10 or later
 * Click_ (package for command line interfaces)
 * NumPy_ (N-dimensional array package)
@@ -28,51 +28,51 @@
 
 or, if you use poetry::
 
     $ poetry add comp-chem-utils
 
 You can also install the in-development version with::
 
-    $ pip install https://gitlab.com/ugognw/python-comp-chem-utils/-/archive/development/ccu-main.zip
+    $ pip install git+ssh://git@gitlab.com:ugognw/python-comp-chem-utils.git
 
 or, similarly::
 
-    $ poetry add git+https://gitlab.com/ugognw/python-comp-chem-utils/-/archive/development/ccu-main.git
+    $ poetry add git+ssh://git@gitlab.com:ugognw/python-comp-chem-utils.git
 
 
 Documentation
 =============
 
 
 https://python-comp-chem-utils.readthedocs.io/en/latest
 
 
 Testing
 ===========
 
 To run all the tests run::
 
-    $ tox
+    $ nox
 
-Note, to combine the coverage data from all the tox environments run:
+Note, to combine the coverage data from all the nox environments run:
 
 .. list-table::
     :widths: 10 90
     :stub-columns: 1
 
     - - Windows
       - ::
 
             set PYTEST_ADDOPTS=--cov-append
-            tox
+            nox
 
     - - Other
       - ::
 
-            PYTEST_ADDOPTS=--cov-append tox
+            PYTEST_ADDOPTS=--cov-append nox
 
 
 Examples
 ========
 
 Determine whether a water molecule is symmetric with respect to a 180 degree rotation about its secondary orientation axis.
```

### Comparing `comp_chem_utils-0.0.1/src/ccu/adsorption/adsorbatecomplex.py` & `comp_chem_utils-0.0.2/src/ccu/adsorption/adsorbatecomplex.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Defines the AdsorbateComplex and AdsorbateComplexFactory classes."""
 
 from collections.abc import Iterator
 import pathlib
 
 import ase
 from ase.io import read
-from numpy import dot
 import numpy as np
+from numpy import dot
+from numpy import ndarray
 from numpy.linalg import norm
 
 from ccu.adsorption import adsorbateorientation
 from ccu.adsorption import adsorbates
 from ccu.adsorption import sitefinder
 from ccu.structure import axisfinder
 from ccu.structure import geometry
@@ -26,53 +27,61 @@
         orientation_description: A string describing the orientation of the
             adsorbate.
         structure: An ase.Atoms object of the adsorbate-surface complex.
     """
 
     def __init__(
         self,
+        adsorbate_description: str,
         site_description: str,
         orientation_description: str,
         structure_desription: str,
         structure: ase.Atoms,
     ) -> None:
         self.structure_description = structure_desription
+        self.adsorbate_description = adsorbate_description
         self.site_description = site_description
         self.orientation_description = orientation_description
         self.structure = structure
 
-    def write(self, destination: pathlib.Path = None) -> pathlib.Path:
+    def write(self, destination: pathlib.Path | None = None) -> pathlib.Path:
         """Writes the AdsorbateComplex object to an ASE .traj file.
 
         Args:
             destination: A pathlib.Path instance indicating the directory in
                 which to write the .traj file. Defaults to the current working
                 directory.
 
         Returns:
             A pathlib.Path instance indicating the path of the written .traj
             file.
         """
         if destination is None:
             destination = pathlib.Path.cwd()
 
-        if self.orientation_description == '':
+        if self.orientation_description == "":
             description = (
-                self.structure_description.replace(' ', '_'),
-                self.site_description.replace(' ', '_'),
+                self.structure_description.replace(" ", "_"),
+                self.adsorbate_description.replace(" ", "_"),
+                self.site_description.replace(" ", "_"),
             )
         else:
             description = (
-                self.structure_description.replace(' ', '_'),
-                self.site_description.replace(' ', '_'),
-                self.orientation_description.replace(' ', '_'),
+                self.structure_description.replace(" ", "_"),
+                self.adsorbate_description.replace(" ", "_"),
+                self.site_description.replace(" ", "_"),
+                self.orientation_description.replace(" ", "_"),
             )
 
-        filename = destination.joinpath('_'.join(description) + '.traj')
-        self.structure.write(filename)
+        filename = "_".join(description)
+        index = 0
+        while destination.joinpath(f"{filename}_{index}.traj").exists():
+            index += 1
+
+        self.structure.write(destination.joinpath(f"{filename}_{index}.traj"))
         return filename
 
 
 class AdsorbateComplexFactory:
     """An AdsorbateComplex factory.
 
     Given an adsorbate, a structure, and various configuration specifications
@@ -80,16 +89,16 @@
     of the adsorption sites and corresponding adsorbate configurations.
 
     Attributes:
         _adsorbate: An ase.Atoms instance representing the adsorbate.
         _structure: An ase.Atoms instance representing the surface structure.
         separation: How far (in Angstroms) the adsorbate should be placed from
             the surface.
-        special_centres: A boolean indicating whether or not atom-centred
-            placement will be used.
+        special_centres: A boolean indicating whether atom-centred
+            placement will be used in addition to centre-of-mass placement.
 
             Note that in addition to be set to true, the ase.Atoms instance
             passed as the adsorbate argument must have the key 'special
             centres' in its info attribute. Further, this key must map to an
             iterable whose elements specify the indices of the atoms to be used
             to centre the adsorbate. If this key is not present in the info
             attribute, then the atom with index 0 will be used to centre the
@@ -112,16 +121,16 @@
     ) -> None:
         self._adsorbate = adsorbate
         self._structure = structure
         self.separation = separation
         self.symmetric = symmetric
         self.vertical = vertical
         self.special_centres = special_centres
-        if special_centres and 'special centres' not in adsorbate.info:
-            self._adsorbate.info['special centres'] = (0,)
+        if special_centres and "special centres" not in adsorbate.info:
+            self._adsorbate.info["special centres"] = (0,)
 
     @property
     def adsorbate(self) -> ase.Atoms:
         return self._adsorbate.copy()
 
     @property
     def structure(self) -> ase.Atoms:
@@ -149,33 +158,41 @@
 
             # Tags to distinguish adsorbate from surface atoms (useful for
             # vibrational calculations)
             oriented_adsorbate.set_tags(adsorbate_tag)
 
             oriented_adsorbate.set_cell(self._structure.cell[:])
 
+            centres: ndarray[np.floating] = [
+                oriented_adsorbate.get_center_of_mass()
+            ]
+
             if self.special_centres:
-                centres = []
-                for i in self._adsorbate.info['special centres']:
-                    centres.append(oriented_adsorbate.positions[i])
-            else:
-                centres = [oriented_adsorbate.get_center_of_mass()]
+                for i in self._adsorbate.info["special centres"]:
+                    new_centre: ndarray[np.floating] = (
+                        oriented_adsorbate.positions[i]
+                    )
+                    if not any(
+                        all(centre == new_centre) for centre in centres
+                    ):
+                        centres.append(new_centre)
 
             for centre in centres:
                 adsorbate_to_place = oriented_adsorbate.copy()
                 self.place_adsorbate(adsorbate_to_place, site, centre)
 
                 # Add adsorbate to structure
                 new_structure = self.structure
                 new_structure.extend(adsorbate_to_place)
 
                 adsorbate_complex = AdsorbateComplex(
+                    self._adsorbate.info.get("name", "adsorbate"),
                     site.description,
                     orientation.description,
-                    new_structure.info['description'],
+                    new_structure.info["description"],
                     new_structure,
                 )
 
                 yield adsorbate_complex
 
     def adsorbate_orientations(
         self, site: sitefinder.AdsorptionSite
@@ -268,46 +285,50 @@
         while separation < self.separation:
             adsorbate.positions += 0.1 * site.surface_norm
             separation = geometry.calculate_separation(
                 adsorbate, self._structure
             )
 
 
-def _get_structure_with_name(structure: pathlib.Path) -> ase.Atoms:
+def _get_structure_with_name(
+    structure: pathlib.Path, *, preserve_info: bool = False
+) -> ase.Atoms:
     """Loads ase.Atoms object from file path with plain text description.
 
     The plain text description is stored in the "info" dictionary of the
     structure under the key "description" and can be accessed as follows:
         atoms = _get_structure_with_name(structure)
         structure_description = atoms.info['description']
 
     Args:
         structure: A pathlib.Path instance indicating the path to the structure
             to be loaded.
+        preserve_info: Whether or not to preserve the structure information in the info dictionary.
+            If False, the `description` key will be set to the structure name. Defaults to False.
 
     Returns:
         The ase.Atoms object representing the structure given.
     """
     atoms = read(structure)
-    if 'description' not in atoms.info:
-        atoms.info['description'] = structure.stem
+    if not preserve_info or "description" not in atoms.info:
+        atoms.info["description"] = structure.stem
 
     return atoms
 
 
 # pylint:disable=too-many-arguments
 def run(
     adsorbate: str,
     structure: pathlib.Path,
-    destination: pathlib.Path = None,
+    destination: pathlib.Path | None = None,
     separation: float = 1.8,
     special_centres: bool = False,
     symmetric: bool = False,
     vertical: bool = False,
-):
+) -> list[tuple[AdsorbateComplex, pathlib.Path]]:
     """Creates MOF-adsorbate complexes for adsorption configurations on the
     SBU of the given MOF and write them to a .traj file.
 
     Args:
         adsorbate: A string indicating the name of the adsorbate to place on
             the surface.
         structure: A pathlib.Path instance indicating the path to the surface
@@ -317,22 +338,30 @@
             exist. Defaults to the current working directory.
         separation: A float indicating how far (in Angstroms) the adsorbate
             should be placed from the surface. Defaults to 1.8.
         symmetric: A boolean indicating whether or not the adsorbate is to be
             treated as symmetric. Defaults to False.
         vertical: A boolean indicating whether or not vertical adsorption
             configurations are to be generated. Defaults to False.
+
+    Returns:
+        A list of 2-tuples (complex_i, path_i) where complex_i is the ith
+        AdsorbateComplex and path_i is a Path object representing the filename
+        under whicn complex_i was saved.
     """
     if destination is None:
         destination = pathlib.Path.cwd()
     elif not destination.exists():
         destination.mkdir()
 
     adsorbate = adsorbates.get_adsorbate(adsorbate)
     structure = _get_structure_with_name(structure)
     finder = sitefinder.MOFSiteFinder(structure)
     placer = AdsorbateComplexFactory(
         adsorbate, structure, separation, special_centres, symmetric, vertical
     )
+    complexes = []
     for site in finder.sites():
         for configuration in placer.next_complex(site):
-            configuration.write(destination)
+            complexes.append((configuration, configuration.write(destination)))
+
+    return complexes
```

### Comparing `comp_chem_utils-0.0.1/src/ccu/adsorption/adsorbateorientation.py` & `comp_chem_utils-0.0.2/src/ccu/adsorption/adsorbateorientation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """This module defines the AdsorbateOrientation and AdsorbateOrientationFactory
 classes."""
 
 from collections.abc import Iterable
 from collections.abc import Sequence
 
 import ase
-from numpy import cross
 import numpy as np
+from numpy import cross
 from numpy.linalg import norm
 from scipy.spatial import transform
 
 from ccu.adsorption import sitefinder
 from ccu.structure import axisfinder
 from ccu.structure import symmetry
 
@@ -75,20 +75,20 @@
         Returns:
             A list of AdsorbateOrientation objects.
         """
         orientations = []
         # Single orientation for zero dimensional adsorbate
         if norm(axisfinder.find_primary_axis(self.adsorbate)) == 0:
             vectors = (self.site.alignments[0].vector, self.site.surface_norm)
-            orientation = AdsorbateOrientation('', vectors)
+            orientation = AdsorbateOrientation("", vectors)
             return [orientation]
 
         for alignment in self.site.alignments:
             orientation = AdsorbateOrientation(
-                f'{alignment.description} 1',
+                f"{alignment.description} 1",
                 [alignment.vector, self.site.surface_norm],
             )
 
             if self.force_symmetry:
                 orientations.append(orientation)
             else:
                 orientations.extend(
@@ -129,15 +129,15 @@
             symmetry_ = symmetry.RotationSymmetry(rotation_)
             if not symmetry_.check_symmetry(self.adsorbate):
                 rot_vec = i * 90 * alignment.vector
                 matrix = transform.Rotation.from_rotvec(rot_vec, degrees=True)
                 vec = matrix.apply(self.site.surface_norm)
                 orientations.append(
                     AdsorbateOrientation(
-                        f'{alignment.description} {i + 1}',
+                        f"{alignment.description} {i + 1}",
                         [alignment.vector, vec],
                     )
                 )
 
         return orientations + self._create_reverse_orientations(
             alignment, orientations
         )
@@ -154,25 +154,25 @@
         no_secondary_axis = norm(secondary_axis) == 0
         for i, alignment in enumerate(self.site.alignments):
             if i != 0 and (no_secondary_axis or self.force_symmetry):
                 break
 
             orientations.append(
                 AdsorbateOrientation(
-                    f'vertical {i+1}',
+                    f"vertical {i+1}",
                     [self.site.surface_norm, alignment.vector],
                 )
             )
 
         reverse_orientations = []
 
         if not self.force_symmetry:
             reverse_orientations.extend(
                 self._create_reverse_orientations(
-                    (self.site.surface_norm, 'vertical'), orientations
+                    (self.site.surface_norm, "vertical"), orientations
                 )
             )
 
         return orientations + reverse_orientations
 
     def _create_reverse_orientations(
         self,
@@ -217,13 +217,13 @@
 
         if not symmetry_.check_symmetry(self.adsorbate):
             vec = -vector
             start = len(orientations)
             for i, orientation in enumerate(orientations):
                 reverse_orientations.append(
                     AdsorbateOrientation(
-                        f'{description} {start + i + 1}',
+                        f"{description} {start + i + 1}",
                         [vec, orientation.vectors[1]],
                     )
                 )
 
         return reverse_orientations
```

### Comparing `comp_chem_utils-0.0.1/src/ccu/adsorption/adsorbates.py` & `comp_chem_utils-0.0.2/src/ccu/adsorption/adsorbates.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,321 +11,370 @@
 
 >>> from ccu.adsorption.adsorbates import get_adsorbate
 >>> get_adsorbate('CO2')
 Atoms(symbols='CO2', pbc=False)
 """
 
 import ase
+from ase import Atoms
 from ase.build import molecule
+from ase.data.pubchem import pubchem_atoms_search
 
 
 def _co2rr_adsorbates() -> dict[str, ase.Atoms]:
-    co2 = molecule('CO2')
+    co2 = molecule("CO2")
 
     # C-O: HCOOH; C=0: HCOOH, O-H: HCOOH
     cooh_cis = ase.Atoms(
-        'CO2H',
+        "CO2H",
         positions=[[0, 0, 0], [1.202, 0, 0], [0, 1.343, 0], [0.972, 1.343, 0]],
     )
     # <OCO: HCOOH
     cooh_cis.set_angle(2, 0, 1, angle=124.9)
     # <COH: HCOOH
     cooh_cis.set_angle(0, 2, 3, angle=106.3)
-    cooh_cis.info['special centres'] = (0,)
+    cooh_cis.info["special centres"] = (0,)
 
     cooh_trans = ase.Atoms(
-        'CO2H',
+        "CO2H",
         positions=[
             [0, 0, 0],
             [1.202, 0, 0],
             [0, 1.343, 0],
             [-0.972, 1.343, 0],
         ],
     )
     # <OCO: HCOOH
     cooh_trans.set_angle(2, 0, 1, angle=124.9)
     # <COH: HCOOH (flipped)
     cooh_trans.set_angle(0, 2, 3, angle=106.3)
-    cooh_trans.info['special centres'] = (0,)
+    cooh_trans.info["special centres"] = (0,)
 
     # C-O: HCOOH; C-H: HCOOH
     ocho = ase.Atoms(
-        'CO2H',
+        "CO2H",
         positions=[[0, 0, 0], [1.343, 0, 0], [0, 1.343, 0], [-1.097, 0, 0]],
     )
     # <OCO: symmetry
     ocho.set_angle(2, 0, 1, angle=120)
     # <COH: HCOOH
     ocho.set_angle(1, 0, 3, angle=120)
-    ocho.info['special centres'] = (0,)
+    ocho.info["special centres"] = (0,)
 
-    co = ase.Atoms('CO', positions=[[0, 0, 0], [1.128, 0, 0]])
+    hcooh = molecule("HCOOH")
+    hcooh.info["special centres"] = (1,)
+
+    co = ase.Atoms("CO", positions=[[0, 0, 0], [1.128, 0, 0]])
 
     # C-O: CH3OH; O-H: CH3OH
-    coh = ase.Atoms('COH', positions=[[0, 0, 0], [1.427, 0, 0], [0, 0.956, 0]])
+    coh = ase.Atoms("COH", positions=[[0, 0, 0], [1.427, 0, 0], [0, 0.956, 0]])
     # <COH: CH3OH
     coh.set_angle(1, 0, 2, angle=108.87)
-    coh.info['special centres'] = (0,)
+    coh.info["special centres"] = (0,)
 
     # C-H: CHO; C-O: CHO
-    cho = ase.Atoms('CHO', positions=[[0, 0, 0], [1.080, 0, 0], [0, 1.198, 0]])
+    cho = ase.Atoms("CHO", positions=[[0, 0, 0], [1.080, 0, 0], [0, 1.198, 0]])
     # <HCO: CHO
     cho.set_angle(1, 0, 2, angle=119.5)
-    cho.info['special centres'] = (0,)
+    cho.info["special centres"] = (0,)
 
-    c = ase.Atoms('C', positions=[[0, 0, 0]])
+    c = ase.Atoms("C", positions=[[0, 0, 0]])
 
     # C-H: HCOOH; C-O: HCOOH; O-H: HCOOH
     choh = ase.Atoms(
-        'CHOH',
+        "CHOH",
         positions=[
             [0, 0, 0],
             [0, -1.097, 0],
             [1.343, 0, 0],
             [1.343, 0.972, 0],
         ],
     )
     # <OCO: HCOOH
     choh.set_angle(1, 0, 2, angle=128.8)
     # <COH: HCOOH
     choh.set_angle(0, 2, 3, angle=106.3)
-    choh.info['special centres'] = (0,)
+    choh.info["special centres"] = (0,)
 
     # C-H: H2CO; C-O: H2CO
     ch2o = ase.Atoms(
-        'CH2O',
+        "CH2O",
         positions=[[0, 0, 0], [0, -1.111, 0], [1.111, 0, 0], [0, 1.205, 0]],
     )
     # <HCH: H2CO
     ch2o.set_angle(2, 0, 1, angle=116.133)
     # <HCO: H2CO
     ch2o.set_angle(1, 0, 3, angle=121.9)
-    ch2o.info['special centres'] = (0,)
+    ch2o.info["special centres"] = (0,)
 
     # C-H: CH3OH; C-O: CH3OH; O-H: CH3OH
     ch2oh = ase.Atoms(
-        'CH2OH',
+        "CH2OH",
         positions=[
             [0, 0, 0],
             [-1.096, 0, 0],
             [0, -1.096, 0],
             [1.427, 0, 0],
             [1.427, 0.956, 0],
         ],
     )
     # <HCH: H2CO
     ch2oh.set_angle(2, 0, 1, angle=116.133)
     # <HCO: symmetry
     ch2oh.set_angle(1, 0, 3, angle=121.9)
     # <HOC: CH3OH
     ch2oh.set_angle(0, 3, 4, angle=108.87)
-    ch2oh.info['special centres'] = (0,)
+    ch2oh.info["special centres"] = (0,)
 
     # Positions from CH3O
     och3 = ase.Atoms(
-        'OCH3',
+        "OCH3",
         positions=[
             [0, 0, 0.8151],
             [0, 0, -0.5899],
             [0, 1.0360, -0.9938],
             [0.8972, -0.5180, -0.9938],
             [-0.8972, -0.5180, -0.9938],
         ],
     )
-    och3.info['special centres'] = (0,)
+    och3.info["special centres"] = (0,)
 
     # C-H: H2CO
     ch2 = ase.Atoms(
-        'CH2', positions=[[0, 0, 0], [0, -1.111, 0], [1.111, 0, 0]]
+        "CH2", positions=[[0, 0, 0], [0, -1.111, 0], [1.111, 0, 0]]
     )
     # <HCH: H2CO
     ch2.set_angle(1, 0, 2, angle=116.133)
-    ch2.info['special centres'] = (0,)
+    ch2.info["special centres"] = (0,)
 
     # Positions from CH3O
     ch3 = ase.Atoms(
-        'CH3',
+        "CH3",
         positions=[
             [0, 0, -0.5899],
             [0, 1.0360, -0.9938],
             [0.8972, -0.5180, -0.9938],
             [-0.8972, -0.5180, -0.9938],
         ],
     )
-    ch3.info['special centres'] = (0,)
+    ch3.info["special centres"] = (0,)
     return {
-        'CO2': co2,
-        'COOH_CIS': cooh_cis,
-        'COOH_TRANS': cooh_trans,
-        'OCHO': ocho,
-        'CO': co,
-        'COH': coh,
-        'CHO': cho,
-        'C': c,
-        'CHOH': choh,
-        'CH2O': ch2o,
-        'HC2OH': ch2oh,
-        'OCH3': och3,
-        'CH2': ch2,
-        'CH3': ch3,
+        "CO2": co2,
+        "COOH_CIS": cooh_cis,
+        "COOH_TRANS": cooh_trans,
+        "OCHO": ocho,
+        "HCOOH": hcooh,
+        "CO": co,
+        "COH": coh,
+        "CHO": cho,
+        "C": c,
+        "CHOH": choh,
+        "CH2O": ch2o,
+        "HC2OH": ch2oh,
+        "OCH3": och3,
+        "CH2": ch2,
+        "CH3": ch3,
     }
 
 
 def _nrr_adsorbates() -> dict[str, ase.Atoms]:
     # N-O: NO3
     no3 = ase.Atoms(
-        'NO3',
+        "NO3",
         positions=[[0, 0, 0], [0, 1.238, 0], [-1.238, 0, 0], [1.238, 0, 0]],
     )
     # <ONO: NO3
     no3.set_angle(2, 0, 1, angle=120)
     no3.set_angle(1, 0, 3, angle=120)
 
     # N-O: HNO3; O-H: HNO3
     no3h = ase.Atoms(
-        'NO3H',
+        "NO3H",
         positions=[
             [0, 0, 0],
             [-1.199, 0, 0],
             [0, 1.211, 0],
             [1.406, 0, 0],
             [1.406, 0.964, 0],
         ],
     )
     # <ONO: HNO3; <HON: HNO3
-    no3h.set_angle(1, 0, 2, angle=130.267)
-    no3h.set_angle(2, 0, 3, angle=115.0883)
-    no3h.set_angle(0, 3, 4, angle=102.15)
-    no3h.info['special centres'] = (0,)
+    no3h = pubchem_atoms_search(cid=944)
+    no3h.info["special centres"] = (3,)
 
     # N-O: HNO2
-    no2 = ase.Atoms('NO2', positions=[[0, 0, 0], [0, 1.442, 0], [1.442, 0, 0]])
+    no2 = ase.Atoms("NO2", positions=[[0, 0, 0], [0, 1.442, 0], [1.442, 0, 0]])
     # <ONO: HNO2
     no2.set_angle(1, 0, 2, angle=110.6)
 
     # N-O: HNO2; N=0: HNO2
     no2h = ase.Atoms(
-        'NO2H',
+        "NO2H",
         positions=[
             [0, 0, 0],
             [-1.442, 0, 0],
             [0, 1.169, 0],
             [-1.442, -0.959, 0],
         ],
     )
     # <ONO: HNO2
     no2h.set_angle(1, 0, 2, angle=110.6)
     # <HON: HNO2
     no2h.set_angle(0, 1, 3, angle=102.1)
-    no2h.info['special centres'] = (0,)
+    no2h.info["special centres"] = (0,)
 
     # N=O: NO
-    no = ase.Atoms('NO', positions=[[0, 0, 0], [1.154, 0, 0]])
+    no = ase.Atoms("NO", positions=[[0, 0, 0], [1.154, 0, 0]])
 
     # N-O: HNO2 & NH2OH (average); O-H: HNO2 & NH2OH (average)
     noh = ase.Atoms(
-        'NOH',
+        "NOH",
         positions=[
             [0, 0, 0],
             [0.5 * (1.442 + 1.453), 0, 0],
             [0.5 * (1.442 + 1.453), 0.5 * (0.959 + 0.962), 0],
         ],
     )
     # <NOH: HNO2 & NH2OH (average)
     noh.set_angle(0, 1, 2, angle=0.5 * (102.1 + 101.37))
-    noh.info['special centres'] = (0,)
+    noh.info["special centres"] = (0,)
 
     # N-H: NH2OH & HNO (average); N-O: NH2OH & HNO (average)
     nho = ase.Atoms(
-        'HNO',
+        "HNO",
         positions=[
             [0, 0, 0],
             [0.5 * (1.016 + 1.090), 0, 0],
             [0.5 * (1.016 + 1.090), 0.5 * (1.453 + 1.209), 0],
         ],
     )
     # <HNO: NH2OH & HNO (average)
     nho.set_angle(0, 1, 2, angle=0.5 * (107.01 + 108.047))
-    nho.info['special centres'] = (2,)
+    nho.info["special centres"] = (2,)
 
     # N-H: NH2OH; N-O: NH2OH; O-H: NH2OH
     nhoh = ase.Atoms(
-        'HNOH',
+        "HNOH",
         positions=[
             [0, 0, 0],
             [1.016, 0, 0],
             [1.016, 1.453, 0],
             [1.016 + 0.962, 1.453, 0],
         ],
     )
     # <HNO: NH2OH
     nhoh.set_angle(0, 1, 2, angle=107.1)
     # <HON: NH2OH
     nhoh.set_angle(1, 2, 3, angle=101.37)
-    nhoh.info['special centres'] = (1,)
+    nhoh.info["special centres"] = (1,)
+
+    n = ase.Atoms("N")
 
     # N-H: NH
-    nh = ase.Atoms('NH', positions=[[0, 0, 0], [1.036, 0, 0]])
+    nh = ase.Atoms("NH", positions=[[0, 0, 0], [1.036, 0, 0]])
 
     # N-H: NH2
     nh2 = ase.ase.Atoms(
-        'HNH',
+        "HNH",
         positions=[
             [0, 0, 0],
             [1.024, 0, 0],
-            [1.024, 1.024, 0],
+            [0, 1.024, 0],
         ],
     )
     # <HNH: NH2
     nh2.set_angle(0, 1, 2, angle=103.4)
 
+    # N-H: NH2; N-O: NH2OH
+    nh2o = ase.ase.Atoms(
+        "NH2O",
+        positions=[
+            [0, 0, 0],
+            [1.024, 0, 0],
+            [0, 1.024, 0],
+            [-0.8523, -0.8523, 0],
+        ],
+    )
+    nh2o.info["special centres"] = (
+        0,
+        3,
+    )
+
+    # N-H: NH2OH
+    nh2oh = ase.ase.Atoms(
+        "NH2OH",
+        positions=[
+            [-0.0094, 0.704, 0],
+            [0.5469, 1.0012, 0.7965],
+            [0.5469, 1.0012, -0.7965],
+            [-0.0094, -0.7490, 0],
+            [-0.9525, -0.9386, 0],
+        ],
+    )
+    nh2oh.info["special centres"] = (
+        0,
+        3,
+    )
+
     # Positions from NH3
     nh3 = ase.Atoms(
-        'NH3',
+        "NH3",
         positions=[
             [0, 0, 0],
             [0, -0.9377, -0.3816],
             [0.812, 0.4689, -0.3816],
             [-0.812, 0.4689, -0.3816],
         ],
     )
 
+    n2 = molecule("N2")
+    n2o = molecule("N2O")
+
     return {
-        'NO3': no3,
-        'NO3H': no3h,
-        'NO2': no2,
-        'NO2H': no2h,
-        'NO': no,
-        'NOH': noh,
-        'NHO': nho,
-        'NHOH': nhoh,
-        'NH': nh,
-        'NH2': nh2,
-        'NH3': nh3,
+        "NO3": no3,
+        "NO3H": no3h,
+        "NO2": no2,
+        "NO2H": no2h,
+        "NO": no,
+        "NOH": noh,
+        "NHO": nho,
+        "NHOH": nhoh,
+        "N": n,
+        "NH": nh,
+        "NH2": nh2,
+        "NH2O": nh2o,
+        "NH2OH": nh2oh,
+        "NH3": nh3,
+        "N2": n2,
+        "N2O": n2o,
     }
 
 
 def _orr_adsorbates() -> dict[str, ase.Atoms]:
     return {
-        'O': ase.Atoms('O'),
+        "O": ase.Atoms("O"),
         # O-H: OH-
-        'OH': ase.Atoms('OH', positions=[[0, 0, 0], [0.964, 0, 0]]),
+        "OH": ase.Atoms("OH", positions=[[0, 0, 0], [0.964, 0, 0]]),
+        "H2O": molecule("H2O"),
     }
 
 
 CO2RR_ADSORBATES = _co2rr_adsorbates()
 NRR_ADSORBATES = _nrr_adsorbates()
 ORR_ADSORBATES = _orr_adsorbates()
-HER_ADSORBATES = {'H': ase.Atoms('H')}
-ALL = {}
+HER_ADSORBATES = {"H": ase.Atoms("H")}
+ALL: dict[str, Atoms] = {}
 ALL.update(CO2RR_ADSORBATES)
 ALL.update(NRR_ADSORBATES)
 ALL.update(ORR_ADSORBATES)
 ALL.update(HER_ADSORBATES)
 
+for name, adsorbate in ALL.items():
+    adsorbate.info["name"] = name
+
 
 def get_adsorbate(adsorbate: str) -> ase.Atoms:
     """Returns the requested adsorbate as an ase.Atoms object.
 
     Args:
         adsorbate: The name of the adsorbate to retrieve as a string
             (case-insensitive).
@@ -334,18 +383,21 @@
         NotImplementedError: The requested adsorbate is neither a molecule
             supported by ASE nor a defined adsorbate in ccu.adsorption.
             adsorbates.
 
     Returns:
         An ase.Atoms instance representing the requested adsorbate.
     """
+    name = adsorbate.upper()
     try:
-        return molecule(adsorbate.upper())
+        atoms = molecule(name)
+        atoms.info["name"] = name
+        return atoms
     except KeyError:
         pass
 
     try:
-        return ALL[adsorbate.upper()]
+        return ALL[name]
     except KeyError as error:
         raise NotImplementedError(
-            f'The {adsorbate} adsorbate is not supported yet.'
+            f"The {adsorbate} adsorbate is not supported yet."
         ) from error
```

### Comparing `comp_chem_utils-0.0.1/src/ccu/adsorption/cli.py` & `comp_chem_utils-0.0.2/src/ccu/adsorption/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,70 @@
 """This module contains the ccu.structure package CLI logic."""
 
-
 import pathlib
 
 import click
 
 from ccu.adsorption import adsorbatecomplex
 from ccu.adsorption.adsorbates import ALL
 
 
 @click.group()
 def main():
     """Adsorption calculation tools."""
 
 
-# pylint:disable=too-many-arguments
-@main.command()
+@main.command(
+    context_settings={"help_option_names": ["-h", "--help"]},
+)
 @click.argument(
-    'adsorbate',
+    "adsorbate",
     type=click.Choice(list(ALL.keys()), case_sensitive=False),
     required=True,
 )
 @click.argument(
-    'structure',
+    "structure",
     required=True,
     type=click.Path(exists=True, path_type=pathlib.Path),
 )
 @click.argument(
-    'destination',
+    "destination",
     default=pathlib.Path.cwd(),
     type=click.Path(file_okay=False, path_type=pathlib.Path),
 )
 @click.option(
-    '-s',
-    '--separation',
-    help='how far the adsorbate should be placed from the surface',
+    "-s",
+    "--separation",
+    help="how far the adsorbate should be placed from the surface",
     default=1.8,
     type=float,
 )
 @click.option(
-    '-c',
-    '--special-centres',
+    "-c",
+    "--special-centres",
     help=(
-        'whether or not the adsorbate will be placed using '
-        'atom-centred placement'
+        "whether or not the adsorbate will be placed using "
+        "atom-centred placement"
     ),
     flag_value=True,
     is_flag=True,
 )
 @click.option(
-    '-Y',
-    '--symmetric',
-    help='whether or not the adsorbate is to be treated as symmetric',
+    "-Y",
+    "--symmetric",
+    help="whether or not the adsorbate is to be treated as symmetric",
     flag_value=True,
     is_flag=True,
 )
 @click.option(
-    '-V',
-    '--vertical',
+    "-V",
+    "--vertical",
     help=(
-        'whether or not vertical adsorption configurations are to '
-        'be generated'
+        "whether or not vertical adsorption configurations are to "
+        "be generated"
     ),
     flag_value=True,
     is_flag=True,
 )
 def place_adsorbate(
     adsorbate,
     structure,
@@ -81,16 +81,17 @@
         ADSORBATE is the name of the adsorbate to place on the surface.
         STRUCTURE is the path to the surface on which the adsorbate will be
             placed.
         DESTINATION is the directory in which to write the .traj files. The
             directory is created if it does not exist. Defaults to the current
             working directory.
     """
-    adsorbatecomplex.run(
+    complexes = adsorbatecomplex.run(
         adsorbate,
         structure,
         destination,
         separation,
         special_centres,
         symmetric,
         vertical,
     )
+    print(f"{len(complexes)} complexes created.")
```

### Comparing `comp_chem_utils-0.0.1/src/ccu/adsorption/sitefinder.py` & `comp_chem_utils-0.0.2/src/ccu/adsorption/sitefinder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """Defines the AdsorptionSite, SiteFinder, and MOFSiteFinder classes."""
 
-
 from abc import ABC
 from abc import abstractmethod
 from collections.abc import Iterable
 from collections.abc import Sequence
 
 import ase
+import numpy as np
 from numpy import cross
 from numpy import dot
-import numpy as np
 from numpy.linalg import norm
 
 
 # pylint:disable=too-few-public-methods
 class SiteAlignment:
     """An alignment that an adsorbate can assume on a site.
 
@@ -107,15 +106,15 @@
         alignments = []
         colinear_vectors = []
         added_elements = []
         for atom in alignment_atoms:
             vector = atom.position - site_anchor
             vector = vector / norm(vector)
             colinear_vectors.append(vector)
-            description = f'colinear with {atom.symbol}'
+            description = f"colinear with {atom.symbol}"
             if atom.symbol not in added_elements:
                 alignments.append(SiteAlignment(vector, description))
                 added_elements.append(atom.symbol)
 
         if self.intermediate_alignments:
             alignments.extend(
                 self.create_intermediate_alignments(colinear_vectors)
@@ -133,16 +132,16 @@
 
         perpendicular_line = (
             colinear_vectors[0]
             - dot(colinear_vectors[0], parallel_line) * parallel_line
         )
         perpendicular_line = perpendicular_line / norm(perpendicular_line)
         return [
-            SiteAlignment(parallel_line, 'parallel'),
-            SiteAlignment(perpendicular_line, 'perpendicular'),
+            SiteAlignment(parallel_line, "parallel"),
+            SiteAlignment(perpendicular_line, "perpendicular"),
         ]
 
 
 # pylint:disable=too-few-public-methods
 class SiteFinder(ABC):
     """An abstract base class for objects which find adsorption sites
     for particular surfaces.
@@ -163,32 +162,36 @@
     of 1 and the metal must possess a tag of 2 for the implementation to work
     correctly.
 
     Args:
         structure: An ase.Atoms object representing a metal-organic framework.
     """
 
-    def __init__(self, structure: ase.Atoms) -> None:
+    def __init__(
+        self, structure: ase.Atoms, *, between_linkers: bool = False
+    ) -> None:
         super().__init__()
         self.structure = structure
+        self.between_linkers = between_linkers
 
     def sites(self) -> list[AdsorptionSite]:
         """Determines all unique SBU adsorption sites for a given MOF.
 
         Note that the AdsorptionSites are defined such that the first and
         second elements in their "alignment_atoms" attribute are linker atoms
         and the third element is the metal.
 
         Returns:
             A list of AdsorptionSite instances representing the SBU adsorption
             sites of the given MOF.
         """
         sites = self.create_linker_sites()
         sites.append(self.create_metal_site())
-        sites.append(self.create_between_linker_site())
+        if self.between_linkers:
+            sites.append(self.create_between_linker_site())
 
         return sites
 
     @property
     def adjacent_linkers(self) -> list[ase.Atom]:
         """A list of ase.Atom instances representing two adjacent linker
         atoms."""
@@ -208,15 +211,15 @@
         """An ase.Atom instance representing the metal atom within the SBU of
         the MOF."""
         for atom in self.structure:
             if atom.tag == 2:
                 return atom
 
         raise ValueError(
-            'No metal atom tagged. (Metal atom must be tagged with 2.)'
+            "No metal atom tagged. (Metal atom must be tagged with 2.)"
         )
 
     @property
     def surface_norm(self) -> np.array:
         """A unit vector normal to the plane determined by two adjacent linker
         atoms and the metal within the SBU.
         """
@@ -237,26 +240,26 @@
         sbu_metal = self.sbu_metal
         surface_norm = self.surface_norm
 
         # Define unique linker sites
         linker_sites = [
             MOFSite(
                 linkers[0].position,
-                f'on {linkers[0].symbol} linker',
+                f"on {linkers[0].symbol} linker",
                 linkers,
                 sbu_metal.position,
                 surface_norm,
                 True,
             )
         ]
         if linkers[0].symbol != linkers[1].symbol:
             linker_sites.append(
                 MOFSite(
                     linkers[1].position,
-                    f'on {linkers[1].symbol} linker',
+                    f"on {linkers[1].symbol} linker",
                     linkers,
                     sbu_metal.position,
                     surface_norm,
                     True,
                 )
             )
 
@@ -267,15 +270,15 @@
         on the MOF metal atom."""
         sbu_metal = self.sbu_metal
         linkers = self.adjacent_linkers
         surface_norm = self.surface_norm
 
         return MOFSite(
             sbu_metal.position,
-            f'on {sbu_metal.symbol}',
+            f"on {sbu_metal.symbol}",
             linkers,
             sbu_metal.position,
             surface_norm,
             True,
         )
 
     def create_between_linker_site(self) -> MOFSite:
@@ -283,13 +286,13 @@
         between the MOF linker atoms."""
         sbu_metal = self.sbu_metal
         linkers = self.adjacent_linkers
         surface_norm = self.surface_norm
 
         return MOFSite(
             0.5 * (linkers[0].position + linkers[1].position),
-            'between linkers',
+            "between linkers",
             linkers,
             sbu_metal.position,
             surface_norm,
             True,
         )
```

### Comparing `comp_chem_utils-0.0.1/src/ccu/structure/axisfinder.py` & `comp_chem_utils-0.0.2/src/ccu/structure/axisfinder.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -45,17 +45,17 @@
 >>> find_tertiary_axis(coh)
 array([0., 0., 1.])
 """
 
 from itertools import product
 
 import ase
+import numpy as np
 from numpy import cross
 from numpy import dot
-import numpy as np
 from numpy.linalg import norm
 
 
 def get_axes(molecule: ase.Atoms) -> tuple[np.array]:
     """Determines a molecule's three orientation axes.
 
     The primary axis is defined as the vector between the two most distant
```

### Comparing `comp_chem_utils-0.0.1/src/ccu/structure/comparator.py` & `comp_chem_utils-0.0.2/src/ccu/structure/comparator.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
             symbols to a numpy.ndarray containing the displacement vectors to
             atoms with the corresponding chemical symbol. The order of the
             displacement vectors is such that the cumulative displacement of
             the displacement vectors is minimized relative to
             fingerprint1._histogram.
         """
         histogram = {}
-        for element in fingerprint2.keys():
+        for element in fingerprint2:
             minimal_cumulative_displacement = math.inf
             minimally_displaced_ordering = fingerprint2[element]
             if element not in fingerprint1:
                 continue
 
             reference_displacements = fingerprint1[element]
             perm_length = min(
@@ -240,13 +240,13 @@
                 cumulative displacement.
 
         Returns:
             A float representing the cumulative displacement for fingerprint2
             relative to fingerprint1.
         """
         cumulative_displacement = 0
-        for element in fingerprint1.keys():
+        for element in fingerprint1:
             for i, displacement in enumerate(fingerprint1[element]):
                 displacement = norm(displacement - fingerprint2[element][i])
                 cumulative_displacement += displacement
 
         return cumulative_displacement
```

### Comparing `comp_chem_utils-0.0.1/src/ccu/structure/fingerprint.py` & `comp_chem_utils-0.0.2/src/ccu/structure/fingerprint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """This module defines the Fingerprint class."""
+
 from __future__ import annotations
 
 from collections.abc import Iterable
 from collections.abc import Iterator
 from collections.abc import MutableMapping
 
 import ase
@@ -28,15 +29,15 @@
             structure used to construct the Fingerprint instance.
     """
 
     def __init__(
         self,
         structure: ase.Atoms,
         reference: int,
-        indices: Iterable[int] = None,
+        indices: Iterable[int] | None = None,
     ) -> None:
         if indices is None:
             indices = range(len(structure))
 
         histogram = {}
         for atom in structure[indices]:
             displacement = atom.position - structure[reference].position
```

### Comparing `comp_chem_utils-0.0.1/src/ccu/structure/geometry.py` & `comp_chem_utils-0.0.2/src/ccu/structure/geometry.py`

 * *Files identical despite different names*

### Comparing `comp_chem_utils-0.0.1/src/ccu/structure/resizecell.py` & `comp_chem_utils-0.0.2/src/ccu/structure/resizecell.py`

 * *Files identical despite different names*

### Comparing `comp_chem_utils-0.0.1/src/ccu/structure/symmetry.py` & `comp_chem_utils-0.0.2/src/ccu/structure/symmetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 
 class SymmetryOperation(abc.ABC):
     """An abstract base class for symmetry operations."""
 
     @abc.abstractmethod
     def transform(self, structure: ase.Atoms) -> ase.Atoms:
-        'Subclasses should override this method.'
+        "Subclasses should override this method."
 
 
 class Rotation(SymmetryOperation):
     """A rotation operation.
 
     Attributes:
         angle: A float specifying a rotation angle in degrees.
@@ -82,19 +82,19 @@
 
 class Symmetry(abc.ABC):
     """An abstract base class for molecule symmetries."""
 
     @property
     @abc.abstractmethod
     def operation(self) -> SymmetryOperation:
-        'Subclasses should override this method.'
+        "Subclasses should override this method."
 
     @abc.abstractmethod
     def check_symmetry(self, structure: ase.Atoms, tol: float) -> bool:
-        'Subclasses should override this method.'
+        "Subclasses should override this method."
 
 
 class RotationSymmetry(Symmetry):
     """A rotational symmetry."""
 
     def __init__(self, operation: Rotation) -> None:
         self._operation = operation
```

### Comparing `comp_chem_utils-0.0.1/PKG-INFO` & `comp_chem_utils-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 Metadata-Version: 2.1
 Name: comp-chem-utils
-Version: 0.0.1
-Summary: Utilities for computational catalysis.
+Version: 0.0.2
+Summary: Utilities for computational chemistry.
 Home-page: https://gitlab.com/ugognw/python-comp-chem-utils
 License: MIT
 Keywords: computational chemistry,catalysis,comp-chem-utils
 Author: Ugochukwu Nwosu
 Author-email: ugognw@gmail.com
 Requires-Python: >=3.10,<3.12
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: ase (>=3.22.1,<4.0.0)
+Requires-Dist: ase (>=3.22.1)
 Requires-Dist: click
-Requires-Dist: numpy (>=1.24.2,<2.0.0)
-Requires-Dist: scipy (>=1.10.1,<2.0.0)
+Requires-Dist: numpy (>=1.24.2)
+Requires-Dist: pymatgen (>=2023.9.2)
+Requires-Dist: scipy (>=1.10.1)
 Project-URL: Documentation, https://python-comp-chem-utils.readthedocs.io/
 Project-URL: Repository, https://gitlab.com/ugognw/python-comp-chem-utils
 Description-Content-Type: text/x-rst
 
 =============
 CompChemUtils
 =============
 
-CompChemUtils is a set of tools for computational catalysis workflows.
+CompChemUtils is a set of tools for computational chemistry workflows.
 
 Requirements
 ============
 
 * Python_ 3.10 or later
 * Click_ (package for command line interfaces)
 * NumPy_ (N-dimensional array package)
@@ -54,51 +63,51 @@
 
 or, if you use poetry::
 
     $ poetry add comp-chem-utils
 
 You can also install the in-development version with::
 
-    $ pip install https://gitlab.com/ugognw/python-comp-chem-utils/-/archive/development/ccu-main.zip
+    $ pip install git+ssh://git@gitlab.com:ugognw/python-comp-chem-utils.git
 
 or, similarly::
 
-    $ poetry add git+https://gitlab.com/ugognw/python-comp-chem-utils/-/archive/development/ccu-main.git
+    $ poetry add git+ssh://git@gitlab.com:ugognw/python-comp-chem-utils.git
 
 
 Documentation
 =============
 
 
 https://python-comp-chem-utils.readthedocs.io/en/latest
 
 
 Testing
 ===========
 
 To run all the tests run::
 
-    $ tox
+    $ nox
 
-Note, to combine the coverage data from all the tox environments run:
+Note, to combine the coverage data from all the nox environments run:
 
 .. list-table::
     :widths: 10 90
     :stub-columns: 1
 
     - - Windows
       - ::
 
             set PYTEST_ADDOPTS=--cov-append
-            tox
+            nox
 
     - - Other
       - ::
 
-            PYTEST_ADDOPTS=--cov-append tox
+            PYTEST_ADDOPTS=--cov-append nox
 
 
 Examples
 ========
 
 Determine whether a water molecule is symmetric with respect to a 180 degree rotation about its secondary orientation axis.
```


# Comparing `tmp/fast_grid-0.1.8-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.whl.zip` & `tmp/fast_grid-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,16 @@
-Zip file size: 196875 bytes, number of entries: 21
-drwxrwxr-x  2.0 unx        0 b- stor 23-Nov-22 18:09 fast_grid/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Nov-22 18:09 fast_grid-0.1.8.dist-info/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Nov-22 18:09 fast_grid.libs/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Nov-22 18:09 fast_grid/assets/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Nov-22 18:09 fast_grid/potential/
--rw-rw-r--  2.0 unx       82 b- defN 23-Nov-22 18:09 fast_grid/__init__.py
--rw-rw-r--  2.0 unx     6356 b- defN 23-Nov-22 18:09 fast_grid/calculate_grid.py
--rw-rw-r--  2.0 unx      692 b- defN 23-Nov-22 18:09 fast_grid/ff.py
--rw-rw-r--  2.0 unx     3817 b- defN 23-Nov-22 18:09 fast_grid/utils.py
--rw-rw-r--  2.0 unx     2139 b- defN 23-Nov-22 18:09 fast_grid/visualize.py
--rw-rw-r--  2.0 unx     1555 b- defN 23-Nov-22 18:09 fast_grid/assets/uff_ff.csv
--rw-rw-r--  2.0 unx      176 b- defN 23-Nov-22 18:09 fast_grid/potential/__init__.py
--rw-rw-r--  2.0 unx   423681 b- defN 23-Nov-22 18:09 fast_grid/potential/gaussian.c
--rwxrwxr-x  2.0 unx    77368 b- defN 23-Nov-22 18:09 fast_grid/potential/gaussian.cpython-310-x86_64-linux-gnu.so
--rw-rw-r--  2.0 unx   429950 b- defN 23-Nov-22 18:09 fast_grid/potential/lj_potential.c
--rwxrwxr-x  2.0 unx    77344 b- defN 23-Nov-22 18:09 fast_grid/potential/lj_potential.cpython-310-x86_64-linux-gnu.so
--rw-rw-r--  2.0 unx      388 b- defN 23-Nov-22 18:09 fast_grid-0.1.8.dist-info/METADATA
--rw-rw-r--  2.0 unx      148 b- defN 23-Nov-22 18:09 fast_grid-0.1.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       59 b- defN 23-Nov-22 18:09 fast_grid-0.1.8.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       10 b- defN 23-Nov-22 18:09 fast_grid-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1397 b- defN 23-Nov-22 18:09 fast_grid-0.1.8.dist-info/RECORD
-21 files, 1025162 bytes uncompressed, 194027 bytes compressed:  81.1%
+Zip file size: 138041 bytes, number of entries: 14
+-rw-rw-r--  2.0 unx       82 b- defN 23-Nov-23 11:52 fast_grid/__init__.py
+-rw-rw-r--  2.0 unx     5187 b- defN 23-Nov-23 11:56 fast_grid/calculate_grid.py
+-rw-rw-r--  2.0 unx      692 b- defN 23-Nov-08 11:45 fast_grid/ff.py
+-rw-rw-r--  2.0 unx     2168 b- defN 23-Nov-23 11:33 fast_grid/potential.py
+-rw-rw-r--  2.0 unx     1323 b- defN 23-Nov-23 11:33 fast_grid/utils.py
+-rw-rw-r--  2.0 unx     2139 b- defN 23-Nov-23 11:54 fast_grid/visualize.py
+-rw-rw-r--  2.0 unx     1555 b- defN 23-Nov-08 08:39 fast_grid/assets/uff_ff.csv
+-rw-rw-r--  2.0 unx   423681 b- defN 23-Nov-22 12:10 fast_grid/potential/gaussian.c
+-rw-rw-r--  2.0 unx   429950 b- defN 23-Nov-22 12:10 fast_grid/potential/lj_potential.c
+-rw-rw-r--  2.0 unx      338 b- defN 23-Nov-23 11:56 fast_grid-0.1.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Nov-23 11:56 fast_grid-0.1.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       60 b- defN 23-Nov-23 11:56 fast_grid-0.1.9.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       10 b- defN 23-Nov-23 11:56 fast_grid-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1132 b- defN 23-Nov-23 11:56 fast_grid-0.1.9.dist-info/RECORD
+14 files, 868409 bytes uncompressed, 136167 bytes compressed:  84.3%
```

## zipnote {}

```diff
@@ -1,64 +1,43 @@
-Filename: fast_grid/
-Comment: 
-
-Filename: fast_grid-0.1.8.dist-info/
-Comment: 
-
-Filename: fast_grid.libs/
-Comment: 
-
-Filename: fast_grid/assets/
-Comment: 
-
-Filename: fast_grid/potential/
-Comment: 
-
 Filename: fast_grid/__init__.py
 Comment: 
 
 Filename: fast_grid/calculate_grid.py
 Comment: 
 
 Filename: fast_grid/ff.py
 Comment: 
 
+Filename: fast_grid/potential.py
+Comment: 
+
 Filename: fast_grid/utils.py
 Comment: 
 
 Filename: fast_grid/visualize.py
 Comment: 
 
 Filename: fast_grid/assets/uff_ff.csv
 Comment: 
 
-Filename: fast_grid/potential/__init__.py
-Comment: 
-
 Filename: fast_grid/potential/gaussian.c
 Comment: 
 
-Filename: fast_grid/potential/gaussian.cpython-310-x86_64-linux-gnu.so
-Comment: 
-
 Filename: fast_grid/potential/lj_potential.c
 Comment: 
 
-Filename: fast_grid/potential/lj_potential.cpython-310-x86_64-linux-gnu.so
-Comment: 
-
-Filename: fast_grid-0.1.8.dist-info/METADATA
+Filename: fast_grid-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: fast_grid-0.1.8.dist-info/WHEEL
+Filename: fast_grid-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: fast_grid-0.1.8.dist-info/entry_points.txt
+Filename: fast_grid-0.1.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: fast_grid-0.1.8.dist-info/top_level.txt
+Filename: fast_grid-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: fast_grid-0.1.8.dist-info/RECORD
+Filename: fast_grid-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## fast_grid/calculate_grid.py

```diff
@@ -4,65 +4,61 @@
 
 from fire import Fire
 
 import numpy as np
 from ase import Atoms
 from ase.io import read
 
+from MDAnalysis.lib.distances import distance_array as mic_distance_matrix
+
 from fast_grid.ff import get_mixing_epsilon_sigma
-from fast_grid.utils import check_inputs_energy_grid
-from fast_grid.potential import lj_potential_cython, gaussian_cython
+from fast_grid.potential import calculate_lj_potential, calculate_gaussian
 from fast_grid.visualize import visualize_grid
 
 warnings.filterwarnings("ignore")
 
 
 def calculate_grid(
     structure: Union[Atoms, str],
     grid_size: Union[int, Iterable] = 30,
-    grid_spacing: float = None,
     ff_type: str = "UFF",
     potential: str = "LJ",
     cutoff: float = 12.8,
-    gas_epsilon: float = 148.0,  # LJ
-    gas_sigma: float = 3.73,  # LJ
+    gas_epsilon: float = 148.0,
+    gas_sigma: float = 3.73,
     visualize: bool = False,
-    gaussian_height: float = 0.1,  # Gaussian
-    gaussian_width: float = 5.0,  # Gaussian
+    gaussian_height: float = 0.1,
+    gaussian_width: float = 5.0,
     float16: bool = False,
     emax: float = 5000.0,
     emin: float = -5000.0,
-    output_shape_grid: bool = False,
 ) -> np.array:
     """Calculate the energy grid for a given structure and force field.
     It takes a structure (ase Atoms object or cif file path) and returns the energy grid.
     The supported potentials are Lennard-Jones and Gaussian.
     The supported force field is UFF.
     The gas parameters are for methane in TraPPE-UA (united-atoms) force field.
     The unit of energy is K and the unit of distance is Angstrom.
     The output shape of energy grid is grid_size * grid_size * grid_size.
 
     :param structure: structure (ase Atoms object or cif file path)
     :param grid_size: grid size, for example, 30 or "(30, 30, 30)", defaults to 30
-    :param grid_spacing: grid spacing, overrides grid_size, defaults to None
     :param ff_type: force field type, defaults to "UFF"
     :param potential: potential function, gaussian or lj, defaults to "LJ"
     :param cutoff: cutoff distance, defaults to 12.8
     :param gas_epsilon: gas epsilon, in K (methane UA in TraPPE), defaults to 148.0
     :param gas_sigma: gas sigma, in Angstrom (methane UA in TraPPE), defaults to 3.73
     :param visualize: visualize the energy grid, defaults to False
     :param gaussian_height: gaussian height
     :param gaussian_width: gaussian width
     :param float16: use float16 to save memory, defaults to False
     :param emax: clip energy values for better visualization, defaults to 5000.0
     :param emin: clip energy values for better visualization, defaults to -5000.0
-    :param output_shape_grid: output shape of energy grid, defaults to False
     :return: energy grid
     """
-    # read structure
     if isinstance(structure, Atoms):
         atoms = structure
     elif isinstance(structure, str):
         if Path(structure).exists():
             atoms = read(structure)
         else:
             raise FileNotFoundError(f"{structure} does not exist")
@@ -73,103 +69,69 @@
     cell_volume = atoms.get_volume()
     cell_vectors = np.array(atoms.cell)
     dist_a = cell_volume / np.linalg.norm(np.cross(cell_vectors[1], cell_vectors[2]))
     dist_b = cell_volume / np.linalg.norm(np.cross(cell_vectors[2], cell_vectors[0]))
     dist_c = cell_volume / np.linalg.norm(np.cross(cell_vectors[0], cell_vectors[1]))
     plane_distances = np.array([dist_a, dist_b, dist_c])
     supercell = np.ceil(2 * cutoff / plane_distances).astype(int)
-    atoms = atoms.repeat(supercell)
+    atoms = atoms.repeat(supercell)  # make supercell
+
     cell_vectors = np.array(atoms.cell)  # redefine cell_vectors after supercell
 
     # get position for grid
     if isinstance(grid_size, int):
         grid_size = np.array([grid_size] * 3)
     else:
         grid_size = eval(grid_size)
-
-    # override grid_size if grid_spacing is not None
-    if grid_spacing is not None:
-        grid_size = np.ceil(
-            np.array(atoms.get_cell_lengths_and_angles()[:3]) / grid_spacing
-        ).astype(int)
-    assert len(grid_size) == 3, "grid_size must be a 3-dim vector"
-
-    indices = np.indices(grid_size).reshape(3, -1).T  # (G, 3)
+        assert len(grid_size) == 3, "grid_size must be a 3-dim vector"
+    indices = np.indices(grid_size).reshape(3, -1).T
     pos_grid = indices.dot(cell_vectors / grid_size)  # (G, 3)
 
     # get positions for atoms
     pos_atoms = atoms.get_positions()  # (N, 3)
 
     # setting force field
     symbols = atoms.get_chemical_symbols()
     epsilon, sigma = get_mixing_epsilon_sigma(
         symbols, ff_type, gas_epsilon, gas_sigma
     )  # (N,) (N,)
 
-    # check inputs for energy grid
-    inverse_cell = np.linalg.inv(cell_vectors)
-    energy_grid = np.zeros([grid_size[0] * grid_size[1] * grid_size[2]])
-    check_inputs_energy_grid(
-        pos1=pos_grid,
-        pos2=pos_atoms,
-        cell_vectors=cell_vectors,
-        inverse_cell=inverse_cell,
-        cutoff=cutoff,
-        energy_grid=energy_grid,
-        epsilon=epsilon,
-        sigma=sigma,
-        gaussian_height=gaussian_height,
-        gaussian_width=gaussian_width,
-    )
+    # calculate distance matrix
+    box = atoms.cell.cellpar()
+    dist_matrix = mic_distance_matrix(pos_grid, pos_atoms, box)  # (G, N)
 
     # calculate energy
     if potential.lower() == "lj":
-        calculated_grid = lj_potential_cython(
-            pos_grid,
-            pos_atoms,
-            cell_vectors,
-            inverse_cell,
-            epsilon,
-            sigma,
-            cutoff,
-            energy_grid,
-        )  # (G, 3)
+        calculated_grid = calculate_lj_potential(
+            dist_matrix,
+            epsilon=epsilon,
+            sigma=sigma,
+            cutoff=cutoff,
+        )  # (G,)
     elif potential.lower() == "gaussian":
-        calculated_grid = gaussian_cython(
-            pos_grid,
-            pos_atoms,
-            cell_vectors,
-            inverse_cell,
-            gaussian_height,
-            gaussian_width,
-            cutoff,
-            energy_grid,
-        )  # (G, 3)
+        calculated_grid = calculate_gaussian(
+            dist_matrix,
+            height=gaussian_height,
+            width=gaussian_width,
+            cutoff=cutoff,
+        )  # (G,)
     else:
         raise NotImplementedError(f"{potential} should be one of ['LJ', 'Gaussian']")
 
-    # flatten energy grid
-    calculated_grid = calculated_grid.reshape(-1)  # (G,)
-
     # convert to float16 to save memory
     if float16:
         # clip energy values for np.float16
         min_float16 = np.finfo(np.float16).min
         max_float16 = np.finfo(np.float16).max
         calculated_grid = np.clip(calculated_grid, min_float16, max_float16)
         # convert to float16
         calculated_grid = calculated_grid.astype(np.float16)
 
-    if output_shape_grid:
-        return calculated_grid.reshape(grid_size)
-
     if visualize:
-        print(
-            f"Visualizing energy grid with {grid_size} grid points | supercell: {supercell}"
-        )
+        print(f"Visualizing energy grid | supercell {supercell}...")
         visualize_grid(pos_grid, pos_atoms, calculated_grid, emax, emin)
 
     return calculated_grid
 
 
 def cli():
     Fire(calculate_grid)
```

## fast_grid/utils.py

```diff
@@ -1,83 +1,25 @@
 import numpy as np
-from numpy.typing import NDArray
 from numba import jit
 
 
-def check_inputs_energy_grid(
-    pos1: NDArray[np.float64],
-    pos2: NDArray[np.float64],
-    cell_vectors: NDArray[np.float64],
-    inverse_cell: NDArray[np.float64],
-    cutoff: float,
-    energy_grid: NDArray[np.float64],
-    epsilon: NDArray[np.float64] = None,
-    sigma: NDArray[np.float64] = None,
-    gaussian_height: float = None,
-    gaussian_width: float = None,
-):
-    """Check inputs to use energy_grid_cython.
-
-    :param pos1: Grid positions for energy grid, expected shape (G, 3).
-    :param pos2: Positions for atoms, expected shape (N, 3).
-    :param cell_vectors: Cell vectors, expected shape (3, 3).
-    :param inverse_cell: Inverse cell, expected shape (3, 3).
-    :param cutoff: Cutoff distance, expected to be a non-negative float.
-    :param energy_grid: Zero array for energy grid, expected shape (G,).
-    :param epsilon: Mixing epsilon, expected shape (N,).
-    :param sigma: Mixing sigma, expected shape (N,).
-    :param gaussian_height: Gaussian height
-    :param gaussian_width: Gaussian width
-    """
-    assert pos1.shape[1] == 3 and pos1.ndim == 2, "pos1 must be of shape (G, 3)"
-    assert pos2.shape[1] == 3 and pos2.ndim == 2, "pos2 must be of shape (N, 3)"
-    assert cell_vectors.shape == (3, 3), "cell_vectors must be of shape (3, 3)"
-    assert inverse_cell.shape == (3, 3), "inv_cell must be of shape (3, 3)"
-    assert (
-        isinstance(cutoff, float) and cutoff >= 0
-    ), "cutoff must be a non-negative float"
-    assert energy_grid.shape == (pos1.shape[0],), "energy_grid must be of shape (G,)"
-    if epsilon is not None:
-        assert (
-            epsilon.ndim == 1 and epsilon.shape[0] == pos2.shape[0]
-        ), "epsilon must be of shape (N,)"
-    if sigma is not None:
-        assert (
-            sigma.ndim == 1 and sigma.shape[0] == pos2.shape[0]
-        ), "sigma must be of shape (N,)"
-    if gaussian_height is not None:
-        assert isinstance(gaussian_height, float), "gaussian_height must be a float"
-    if gaussian_width is not None:
-        assert isinstance(gaussian_width, float), "gaussian_width must be a float"
-    assert (
-        pos1.dtype == np.float64
-        and pos2.dtype == np.float64
-        and cell_vectors.dtype == np.float64
-        and inverse_cell.dtype == np.float64
-        and epsilon.dtype == np.float64
-        and sigma.dtype == np.float64
-        and energy_grid.dtype == np.float64
-    ), "All array inputs must be of type np.float64"
-
-
-# deprecated function
 @jit(nopython=True)
 def mic_distance_matrix(pos1, pos2, cell_vectors):
     """
     Calculate the distance matrix between two sets of positions with minimum image convention
     for a periodic cell.
 
     :param pos1: An array of shape (N1, 3) containing the positions of the first set of atoms.
     :param pos2: An array of shape (N2, 3) containing the positions of the second set of atoms.
     :param cell_vectors: A (3, 3) array where rows are the vectors defining the unit cell.
     :return: A distance matrix of shape (N1, N2).
     """
     N1 = pos1.shape[0]
     N2 = pos2.shape[0]
-    distance_matrix = np.empty((N1, N2), dtype=np.float32)
+    distance_matrix = np.zeros((N1, N2), dtype=np.float64)
     inverse_cell = np.linalg.inv(cell_vectors)
 
     for i in range(N1):
         for j in range(N2):
             diff = pos1[i] - pos2[j]
 
             # Transform diff to the cell basis
```

## Comparing `fast_grid-0.1.8.dist-info/RECORD` & `fast_grid-0.1.9.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-fast_grid/__init__.py,sha256=dtsO73rET_6-AprDKUeKmOekc9jXj6hfcKFnOgKYF1M,82
-fast_grid/calculate_grid.py,sha256=G-PR0KoxuQM3V-ASbhg-DK6CxyQD_VlNulnI6v6WVhY,6356
-fast_grid/ff.py,sha256=QE6mFf1udnYEHCz59-yqOhkdJuofKz4J5DBKeXbwrEQ,692
-fast_grid/utils.py,sha256=L2rmxmVLoPr7m6-ioe9NVBEWJFQgTSS9o50x7QGxm0M,3817
-fast_grid/visualize.py,sha256=F2vmfOz7bMaWR6NnjHZAbKI3NuvCZzT_LiuLt5zttt8,2139
-fast_grid/assets/uff_ff.csv,sha256=P62wojgP3BS9dhXo2VkRgoU4UHqjz-hHu18pD_NSCnk,1555
-fast_grid/potential/__init__.py,sha256=JtovbKx5KGAS3x1cHbe3K2yFwZ-aauNWJkSLg9zqNEA,176
-fast_grid/potential/gaussian.c,sha256=FYMoJugAcQepwgpbAqUFHj08E9ri7Z6cPI0MIirlkyI,423681
-fast_grid/potential/gaussian.cpython-310-x86_64-linux-gnu.so,sha256=JerU2M6c8SYE98HFiQ74i1WgetZaLQG8einIJjo8xvU,77368
-fast_grid/potential/lj_potential.c,sha256=dOA0pY9BwCDL9nqACFEoPoHNB4toAIpY9KOVFn1S-Ps,429950
-fast_grid/potential/lj_potential.cpython-310-x86_64-linux-gnu.so,sha256=SrdBXPgppokMbBRGLAKlDPNaVvU69cALGe266z6Y2Yo,77344
-fast_grid-0.1.8.dist-info/METADATA,sha256=TaLYudSVlgDkjT2b40Ds6y7yyx0p_vIuLmqCt2EquKk,388
-fast_grid-0.1.8.dist-info/WHEEL,sha256=UXEIj3uCzHQ50uLVKUyaf89X90JHG7GLsUpKd_z9iUU,148
-fast_grid-0.1.8.dist-info/entry_points.txt,sha256=UIFafTDAAvSkNgHzFKVG_-TTaefbDUScC1sMagDTvy8,59
-fast_grid-0.1.8.dist-info/top_level.txt,sha256=xEfLhCgdFKcJrHHzsTI_ePqyuCoKXQ_zxZKEVmLsh80,10
-fast_grid-0.1.8.dist-info/RECORD,,
+fast_grid/__init__.py,sha256=dtsO73rET_6-AprDKUeKmOekc9jXj6hfcKFnOgKYF1M,82
+fast_grid/calculate_grid.py,sha256=-I6WmvHQnThdKu_CpXMDg7CsilOqks0t7cyo8iUFgpY,5187
+fast_grid/ff.py,sha256=QE6mFf1udnYEHCz59-yqOhkdJuofKz4J5DBKeXbwrEQ,692
+fast_grid/potential.py,sha256=XjK7pwniKfCO6CEWMikLo6wf4bhmk9LIDXYohPm4V-A,2168
+fast_grid/utils.py,sha256=G0eHwSn1JLi3lLlEelb1zhpUb6GItNOQq8OkOa_JHDg,1323
+fast_grid/visualize.py,sha256=F2vmfOz7bMaWR6NnjHZAbKI3NuvCZzT_LiuLt5zttt8,2139
+fast_grid/assets/uff_ff.csv,sha256=P62wojgP3BS9dhXo2VkRgoU4UHqjz-hHu18pD_NSCnk,1555
+fast_grid/potential/gaussian.c,sha256=FYMoJugAcQepwgpbAqUFHj08E9ri7Z6cPI0MIirlkyI,423681
+fast_grid/potential/lj_potential.c,sha256=dOA0pY9BwCDL9nqACFEoPoHNB4toAIpY9KOVFn1S-Ps,429950
+fast_grid-0.1.9.dist-info/METADATA,sha256=EO_zGORo2xJaaLm2ixeAFDNWHY-9xFyx_oEMFd1iqRY,338
+fast_grid-0.1.9.dist-info/WHEEL,sha256=Xo9-1PvkuimrydujYJAjF7pCkriuXBpUPEjma1nZyJ0,92
+fast_grid-0.1.9.dist-info/entry_points.txt,sha256=21JijUo71fAFDDMvFJkt0AZrjYs1CSn5SIQVtRHixts,60
+fast_grid-0.1.9.dist-info/top_level.txt,sha256=xEfLhCgdFKcJrHHzsTI_ePqyuCoKXQ_zxZKEVmLsh80,10
+fast_grid-0.1.9.dist-info/RECORD,,
```


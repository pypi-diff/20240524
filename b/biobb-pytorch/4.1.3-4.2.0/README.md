# Comparing `tmp/biobb_pytorch-4.1.3.tar.gz` & `tmp/biobb_pytorch-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobb_pytorch-4.1.3.tar", last modified: Tue May  7 21:06:00 2024, max compression
+gzip compressed data, was "biobb_pytorch-4.2.0.tar", last modified: Fri May 24 10:52:37 2024, max compression
```

## Comparing `biobb_pytorch-4.1.3.tar` & `biobb_pytorch-4.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-07 21:06:00.048714 biobb_pytorch-4.1.3/
--rwxr-xr-x   0 pau        (501) staff       (20)    11358 2024-01-25 14:13:16.000000 biobb_pytorch-4.1.3/LICENSE
--rw-r--r--   0 pau        (501) staff       (20)     6841 2024-05-07 21:06:00.048411 biobb_pytorch-4.1.3/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)     5927 2024-05-07 21:05:18.000000 biobb_pytorch-4.1.3/README.md
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-07 21:06:00.039835 biobb_pytorch-4.1.3/biobb_pytorch/
--rw-r--r--   0 pau        (501) staff       (20)       84 2024-05-07 21:05:17.000000 biobb_pytorch-4.1.3/biobb_pytorch/__init__.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-07 21:06:00.047726 biobb_pytorch-4.1.3/biobb_pytorch/mdae/
--rw-r--r--   0 pau        (501) staff       (20)      104 2024-04-25 12:20:08.000000 biobb_pytorch-4.1.3/biobb_pytorch/mdae/__init__.py
--rw-r--r--   0 pau        (501) staff       (20)    12008 2024-05-06 20:44:25.000000 biobb_pytorch-4.1.3/biobb_pytorch/mdae/apply_mdae.py
--rw-r--r--   0 pau        (501) staff       (20)     4284 2024-05-06 14:01:34.000000 biobb_pytorch-4.1.3/biobb_pytorch/mdae/common.py
--rw-r--r--   0 pau        (501) staff       (20)     2195 2024-04-17 09:27:04.000000 biobb_pytorch-4.1.3/biobb_pytorch/mdae/mdae.py
--rw-r--r--   0 pau        (501) staff       (20)     4608 2024-05-06 14:10:58.000000 biobb_pytorch-4.1.3/biobb_pytorch/mdae/plots.py
--rw-r--r--   0 pau        (501) staff       (20)    23393 2024-05-07 17:05:40.000000 biobb_pytorch-4.1.3/biobb_pytorch/mdae/train_mdae.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-07 21:06:00.048091 biobb_pytorch-4.1.3/biobb_pytorch/test/
--rwxr-xr-x   0 pau        (501) staff       (20)        0 2024-01-26 06:36:24.000000 biobb_pytorch-4.1.3/biobb_pytorch/test/__init__.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-07 21:06:00.042678 biobb_pytorch-4.1.3/biobb_pytorch.egg-info/
--rw-r--r--   0 pau        (501) staff       (20)     6841 2024-05-07 21:05:59.000000 biobb_pytorch-4.1.3/biobb_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)      488 2024-05-07 21:05:59.000000 biobb_pytorch-4.1.3/biobb_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 pau        (501) staff       (20)        1 2024-05-07 21:05:59.000000 biobb_pytorch-4.1.3/biobb_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 pau        (501) staff       (20)      114 2024-05-07 21:05:59.000000 biobb_pytorch-4.1.3/biobb_pytorch.egg-info/entry_points.txt
--rw-r--r--   0 pau        (501) staff       (20)       26 2024-05-07 21:05:59.000000 biobb_pytorch-4.1.3/biobb_pytorch.egg-info/requires.txt
--rw-r--r--   0 pau        (501) staff       (20)       14 2024-05-07 21:05:59.000000 biobb_pytorch-4.1.3/biobb_pytorch.egg-info/top_level.txt
--rw-r--r--   0 pau        (501) staff       (20)       38 2024-05-07 21:06:00.048801 biobb_pytorch-4.1.3/setup.cfg
--rw-r--r--   0 pau        (501) staff       (20)     1424 2024-05-07 21:04:51.000000 biobb_pytorch-4.1.3/setup.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-24 10:52:37.247798 biobb_pytorch-4.2.0/
+-rwxr-xr-x   0 pau        (501) staff       (20)    11358 2024-01-25 14:13:16.000000 biobb_pytorch-4.2.0/LICENSE
+-rw-r--r--   0 pau        (501) staff       (20)     6840 2024-05-24 10:52:37.247279 biobb_pytorch-4.2.0/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)     5926 2024-05-24 10:50:21.000000 biobb_pytorch-4.2.0/README.md
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-24 10:52:37.235439 biobb_pytorch-4.2.0/biobb_pytorch/
+-rw-r--r--   0 pau        (501) staff       (20)       84 2024-05-24 10:49:08.000000 biobb_pytorch-4.2.0/biobb_pytorch/__init__.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-24 10:52:37.245490 biobb_pytorch-4.2.0/biobb_pytorch/mdae/
+-rw-r--r--   0 pau        (501) staff       (20)      104 2024-04-25 12:20:08.000000 biobb_pytorch-4.2.0/biobb_pytorch/mdae/__init__.py
+-rw-r--r--   0 pau        (501) staff       (20)    12008 2024-05-06 20:44:25.000000 biobb_pytorch-4.2.0/biobb_pytorch/mdae/apply_mdae.py
+-rw-r--r--   0 pau        (501) staff       (20)     4284 2024-05-06 14:01:34.000000 biobb_pytorch-4.2.0/biobb_pytorch/mdae/common.py
+-rw-r--r--   0 pau        (501) staff       (20)     2195 2024-04-17 09:27:04.000000 biobb_pytorch-4.2.0/biobb_pytorch/mdae/mdae.py
+-rw-r--r--   0 pau        (501) staff       (20)     4791 2024-05-16 21:00:18.000000 biobb_pytorch-4.2.0/biobb_pytorch/mdae/plots.py
+-rw-r--r--   0 pau        (501) staff       (20)    24201 2024-05-09 09:41:52.000000 biobb_pytorch-4.2.0/biobb_pytorch/mdae/train_mdae.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-24 10:52:37.246855 biobb_pytorch-4.2.0/biobb_pytorch/test/
+-rwxr-xr-x   0 pau        (501) staff       (20)        0 2024-01-26 06:36:24.000000 biobb_pytorch-4.2.0/biobb_pytorch/test/__init__.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2024-05-24 10:52:37.238513 biobb_pytorch-4.2.0/biobb_pytorch.egg-info/
+-rw-r--r--   0 pau        (501) staff       (20)     6840 2024-05-24 10:52:37.000000 biobb_pytorch-4.2.0/biobb_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)      488 2024-05-24 10:52:37.000000 biobb_pytorch-4.2.0/biobb_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 pau        (501) staff       (20)        1 2024-05-24 10:52:37.000000 biobb_pytorch-4.2.0/biobb_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 pau        (501) staff       (20)      114 2024-05-24 10:52:37.000000 biobb_pytorch-4.2.0/biobb_pytorch.egg-info/entry_points.txt
+-rw-r--r--   0 pau        (501) staff       (20)       26 2024-05-24 10:52:37.000000 biobb_pytorch-4.2.0/biobb_pytorch.egg-info/requires.txt
+-rw-r--r--   0 pau        (501) staff       (20)       14 2024-05-24 10:52:37.000000 biobb_pytorch-4.2.0/biobb_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 pau        (501) staff       (20)       38 2024-05-24 10:52:37.247902 biobb_pytorch-4.2.0/setup.cfg
+-rw-r--r--   0 pau        (501) staff       (20)     1424 2024-05-24 10:48:33.000000 biobb_pytorch-4.2.0/setup.py
```

### Comparing `biobb_pytorch-4.1.3/LICENSE` & `biobb_pytorch-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_pytorch-4.1.3/PKG-INFO` & `biobb_pytorch-4.2.0/biobb_pytorch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: biobb_pytorch
-Version: 4.1.3
+Name: biobb-pytorch
+Version: 4.2.0
 Summary: biobb_pytorch is the Biobb module collection to create and train ML & DL models.
 Home-page: https://github.com/bioexcel/biobb_pytorch
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
 Project-URL: Documentation, http://biobb-pytorch.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
@@ -21,15 +21,15 @@
 License-File: LICENSE
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_pytorch?label=Version)](https://GitHub.com/bioexcel/biobb_pytorch/tags/)
 [![](https://img.shields.io/pypi/v/biobb-pytorch.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-pytorch/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_pytorch?label=Conda)](https://anaconda.org/bioconda/biobb_pytorch)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_pytorch?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_pytorch)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_pytorch?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.3--pyhdfd78af_1)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pytorch:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_pytorch)
 [![](https://img.shields.io/pypi/pyversions/biobb-pytorch.svg?label=Python%20Versions)](https://pypi.org/project/biobb-pytorch/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_pytorch)
 
 [![](https://readthedocs.org/projects/biobb-pytorch/badge/?version=latest&label=Docs)](https://biobb-pytorch.readthedocs.io/en/latest/?badge=latest)
@@ -45,75 +45,75 @@
 [![](https://img.shields.io/github/issues/bioexcel/biobb_pytorch.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_pytorch/issues/)
 
 [![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
 [![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
 
 [](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
 
- [//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractives URL)
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
 
 
 # biobb_pytorch
 
 ### Introduction
 biobb_pytorch is the Biobb module collection to create and train ML & DL models using the popular [PyTorch](https://pytorch.org/) Python library.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-pytorch.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.3 2024.2
+v4.2.0 2024.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_pytorch>=4.1.3"
+        pip install "biobb_pytorch>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-pytorch.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_pytorch>=4.1.3"
+        conda install -c bioconda "biobb_pytorch>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-pytorch.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-pytorch.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_pytorch:4.1.3--pyhdfd78af_1
+        docker pull quay.io/biocontainers/biobb_pytorch:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_pytorch:4.1.3--pyhdfd78af_1 <command>
+        docker run quay.io/biocontainers/biobb_pytorch:4.2.0--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_pytorch.sif https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.3--pyhdfd78af_1
+        singularity pull --name biobb_pytorch.sif https://depot.galaxyproject.org/singularity/biobb_pytorch:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_pytorch.sif <command>
```

### Comparing `biobb_pytorch-4.1.3/README.md` & `biobb_pytorch-4.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_pytorch?label=Version)](https://GitHub.com/bioexcel/biobb_pytorch/tags/)
 [![](https://img.shields.io/pypi/v/biobb-pytorch.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-pytorch/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_pytorch?label=Conda)](https://anaconda.org/bioconda/biobb_pytorch)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_pytorch?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_pytorch)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_pytorch?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.3--pyhdfd78af_1)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pytorch:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_pytorch)
 [![](https://img.shields.io/pypi/pyversions/biobb-pytorch.svg?label=Python%20Versions)](https://pypi.org/project/biobb-pytorch/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_pytorch)
 
 [![](https://readthedocs.org/projects/biobb-pytorch/badge/?version=latest&label=Docs)](https://biobb-pytorch.readthedocs.io/en/latest/?badge=latest)
@@ -23,75 +23,75 @@
 [![](https://img.shields.io/github/issues/bioexcel/biobb_pytorch.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_pytorch/issues/)
 
 [![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
 [![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
 
 [](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
 
- [//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractives URL)
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
 
 
 # biobb_pytorch
 
 ### Introduction
 biobb_pytorch is the Biobb module collection to create and train ML & DL models using the popular [PyTorch](https://pytorch.org/) Python library.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-pytorch.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.3 2024.2
+v4.2.0 2024.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_pytorch>=4.1.3"
+        pip install "biobb_pytorch>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-pytorch.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_pytorch>=4.1.3"
+        conda install -c bioconda "biobb_pytorch>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-pytorch.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-pytorch.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_pytorch:4.1.3--pyhdfd78af_1
+        docker pull quay.io/biocontainers/biobb_pytorch:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_pytorch:4.1.3--pyhdfd78af_1 <command>
+        docker run quay.io/biocontainers/biobb_pytorch:4.2.0--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_pytorch.sif https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.3--pyhdfd78af_1
+        singularity pull --name biobb_pytorch.sif https://depot.galaxyproject.org/singularity/biobb_pytorch:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_pytorch.sif <command>
```

### Comparing `biobb_pytorch-4.1.3/biobb_pytorch/mdae/apply_mdae.py` & `biobb_pytorch-4.2.0/biobb_pytorch/mdae/apply_mdae.py`

 * *Files identical despite different names*

### Comparing `biobb_pytorch-4.1.3/biobb_pytorch/mdae/common.py` & `biobb_pytorch-4.2.0/biobb_pytorch/mdae/common.py`

 * *Files identical despite different names*

### Comparing `biobb_pytorch-4.1.3/biobb_pytorch/mdae/mdae.py` & `biobb_pytorch-4.2.0/biobb_pytorch/mdae/mdae.py`

 * *Files identical despite different names*

### Comparing `biobb_pytorch-4.1.3/biobb_pytorch/mdae/plots.py` & `biobb_pytorch-4.2.0/biobb_pytorch/mdae/plots.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 def _numpy_rmsd(reference, trajectory):
     return np.sqrt(np.mean(np.sum((reference - trajectory) ** 2, axis=2), axis=1))
 
 
 def plot_rmsd(traj_file_npy_path, output_reconstructed_traj_npy_path) -> None:
     perf_data = np.load(traj_file_npy_path)
     output = np.load(output_reconstructed_traj_npy_path)
-    rmsd_trajectory = _numpy_rmsd(perf_data[0], perf_data)
-    rmsd_output = _numpy_rmsd(perf_data[0], output)
+    rmsd_trajectory = _numpy_rmsd(perf_data[0], perf_data)*10  # Convert to Å
+    rmsd_output = _numpy_rmsd(perf_data[0], output)*10  # Convert to Å
     frames = np.arange(len(rmsd_trajectory))
     fig, ax = plt.subplots(figsize=(20, 6))
     ax.plot(frames, rmsd_trajectory, color='blue', linewidth=1, label='Original')
     ax.plot(frames, rmsd_output, color='red', linewidth=1, label='Reconstruction')
     # Labels, title, and legend
     ax.set_xlabel('# Frame')
     ax.set_ylabel('RMSD (Å)')
@@ -73,34 +73,35 @@
 def _numpy_rmsf_by_atom(trajectory):
     return np.sqrt(np.mean(np.sum((trajectory - np.mean(trajectory, axis=0)) ** 2, axis=2), axis=0))
 
 
 def plot_rmsf(original_traj_npy_file, mutated_reconstructed_traj_npy_file):
     original_traj = np.load(original_traj_npy_file)
     mutated_reconstructed_traj = np.load(mutated_reconstructed_traj_npy_file)
-    rmsf_trajectory = _numpy_rmsf_by_atom(original_traj)
-    rmsf_output = _numpy_rmsf_by_atom(mutated_reconstructed_traj)
+    rmsf_trajectory = _numpy_rmsf_by_atom(original_traj)*10  # Convert to Å
+    rmsf_output = _numpy_rmsf_by_atom(mutated_reconstructed_traj)*10  # Convert to Å
     fig, ax = plt.subplots(figsize=(20, 6))
     indices = np.arange(len(rmsf_trajectory))
     ax.plot(indices, rmsf_trajectory, color='blue', linewidth=1, label='Original')
     ax.plot(indices, rmsf_output, color='red', linewidth=1, label='Reconstruction')
     ax.set_xlabel('# Atom')
     ax.set_ylabel('RMSD (Å) Average structure as reference')
     plt.title('RMSF Plot')
     plt.legend()
     plt.show()
 
 
 def plot_rmsf_difference(original_traj_npy_file, mutated_reconstructed_traj_npy_file):
     original_traj = np.load(original_traj_npy_file)
     mutated_reconstructed_traj = np.load(mutated_reconstructed_traj_npy_file)
-    rmsf_trajectory = _numpy_rmsf_by_atom(original_traj)
-    rmsf_output = _numpy_rmsf_by_atom(mutated_reconstructed_traj)
+    rmsf_trajectory = _numpy_rmsf_by_atom(original_traj)*10  # Convert to Å
+    rmsf_output = _numpy_rmsf_by_atom(mutated_reconstructed_traj)*10  # Convert to Å
     fig, ax = plt.subplots(figsize=(20, 6))
     indices = np.arange(len(rmsf_trajectory))
     # Plot RMSF for diference between input and output
     ax.plot(indices, (rmsf_trajectory - rmsf_output), color='orange', linewidth=1, label='DIO')
+    ax.axhline(y=1, color='grey', linestyle='--', linewidth=1)
     ax.set_xlabel('# Atom')
     ax.set_ylabel('RMSD (Å)')
     plt.title('RMSF Plot')
     plt.legend()
     plt.show()
```

### Comparing `biobb_pytorch-4.1.3/biobb_pytorch/mdae/train_mdae.py` & `biobb_pytorch-4.2.0/biobb_pytorch/mdae/train_mdae.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,25 +26,26 @@
         output_train_data_npz_path (str) (Optional): Path to the output train data file. File type: output. `Sample file <https://github.com/bioexcel/biobb_pytorch/raw/master/biobb_pytorch/test/reference/mdae/ref_output_train_data.npz>`_. Accepted formats: npz (edam:format_4003).
         output_performance_npz_path (str) (Optional): Path to the output performance file. File type: output.  `Sample file <https://github.com/bioexcel/biobb_pytorch/raw/master/biobb_pytorch/test/reference/mdae/ref_output_performance.npz>`_. Accepted formats: npz (edam:format_4003).
         properties (dict - Python dictionary object containing the tool parameters, not input/output files):
             * **latent_dimensions** (*int*) - (2) min dimensionality of the latent space.
             * **num_layers** (*int*) - (4) number of layers in the encoder/decoder (4 to encode and 4 to decode).
             * **num_epochs** (*int*) - (100) number of epochs (iterations of whole dataset) for training.
             * **lr** (*float*) - (0.0001) learning rate.
-            * **self.lr_step_size** (*int*) - (100) Period of learning rate decay.
-            * **self.gamma** (*float*) - (0.1) Multiplicative factor of learning rate decay.
+            * **lr_step_size** (*int*) - (100) Period of learning rate decay.
+            * **gamma** (*float*) - (0.1) Multiplicative factor of learning rate decay.
             * **checkpoint_interval** (*int*) - (25) number of epochs interval to save model checkpoints o 0 to disable.
             * **output_checkpoint_prefix** (*str*) - ("checkpoint_epoch") prefix for the checkpoint files.
             * **partition** (*float*) - (0.8) 0.8 = 80% partition of the data for training and validation.
             * **batch_size** (*int*) - (1) number of samples/frames per batch.
             * **log_interval** (*int*) - (10) number of epochs interval to log the training progress.
             * **input_dimensions** (*int*) - (None) input dimensions by default it should be the number of features in the input data (number of atoms * 3 corresponding to x, y, z coordinates).
             * **output_dimensions** (*int*) - (None) output dimensions by default it should be the number of features in the input data (number of atoms * 3 corresponding to x, y, z coordinates).
             * **loss_function** (*str*) - ("MSELoss") Loss function to be used. Values: MSELoss, L1Loss, SmoothL1Loss, BCELoss, BCEWithLogitsLoss, CrossEntropyLoss, CTCLoss, NLLLoss, KLDivLoss, PoissonNLLLoss, NLLLoss2d, CosineEmbeddingLoss, HingeEmbeddingLoss, MarginRankingLoss, MultiLabelMarginLoss, MultiLabelSoftMarginLoss, MultiMarginLoss, TripletMarginLoss, HuberLoss, SoftMarginLoss, MultiLabelSoftMarginLoss, CosineEmbeddingLoss, MultiMarginLoss, TripletMarginLoss, MarginRankingLoss, HingeEmbeddingLoss, CTCLoss, NLLLoss, PoissonNLLLoss, KLDivLoss, CrossEntropyLoss, BCEWithLogitsLoss, BCELoss, SmoothL1Loss, L1Loss, MSELoss.
             * **optimizer** (*str*) - ("Adam") Optimizer algorithm to be used. Values: Adadelta, Adagrad, Adam, AdamW, SparseAdam, Adamax, ASGD, LBFGS, RMSprop, Rprop, SGD.
+            * **seed** (*int*) - (None) Random seed for reproducibility.
 
     Examples:
         This is a use case of how to use the building block from Python::
 
             from biobb_pytorch.mdae.train_mdae import trainMDAE
 
             prop = {
@@ -103,14 +104,15 @@
         self.num_epochs: int = int(properties.get('num_epochs', 100))  # number of epochs (iterations of whole dataset) for training
         self.lr: float = float(properties.get('lr', 0.0001))  # learning rate
         self.lr_step_size: int = int(properties.get('lr_step_size', 100))  # Period of learning rate decay
         self.gamma: float = float(properties.get('gamma', 0.1))  # Multiplicative factor of learning rate decay
         self.checkpoint_interval: int = int(properties.get('checkpoint_interval', 25))  # number of epochs interval to save model checkpoints o 0 to disable
         self.output_checkpoint_prefix: str = properties.get('output_checkpoint_prefix', 'checkpoint_epoch_')  # prefix for the checkpoint files,
         self.partition: float = float(properties.get('partition', 0.8))  # 0.8 = 80% partition of the data for training and validation
+        self.seed: Optional[int] = int(properties.get('seed', '42')) if properties.get('seed', None) else None  # Random seed for reproducibility
         self.batch_size: int = int(properties.get('batch_size', 1))  # number of samples/frames per batch
         self.log_interval: int = int(properties.get('log_interval', 10))  # number of epochs interval to log the training progress
 
         # Input data section
         input_raw_data = np.load(self.io_dict['in']['input_train_npy_path'])
         # Reshape the input data to be a 2D array and normalization
         input_train_reshaped_data: np.ndarray = np.reshape(input_raw_data, (len(input_raw_data), input_raw_data.shape[1]*input_raw_data.shape[2]))
@@ -132,14 +134,21 @@
         train_tensor = torch.FloatTensor(input_train_data[:index_train_data, :])
         validation_tensor = torch.FloatTensor(input_train_data[-index_validation_data:, :])
         performance_tensor = torch.FloatTensor(input_train_data)
         train_dataset = torch.utils.data.TensorDataset(train_tensor)
         validation_dataset = torch.utils.data.TensorDataset(validation_tensor)
         performance_dataset = torch.utils.data.TensorDataset(performance_tensor)
 
+        # Seed
+        if self.seed:
+            torch.manual_seed(self.seed)
+            np.random.seed(self.seed)
+            if torch.cuda.is_available():
+                torch.cuda.manual_seed_all(self.seed)
+
         self.train_dataloader: torch.utils.data.DataLoader = torch.utils.data.DataLoader(dataset=train_dataset,
                                                                                          batch_size=self.batch_size,
                                                                                          drop_last=True,
                                                                                          shuffle=True)
         self.validation_dataloader: torch.utils.data.DataLoader = torch.utils.data.DataLoader(dataset=validation_dataset,
                                                                                               batch_size=self.batch_size,
                                                                                               drop_last=True,
@@ -222,45 +231,43 @@
 
         start_time: float = time.time()
         fu.log("Start Training:", self.out_log)
         fu.log(f"  Device: {self.model.device}", self.out_log)
         fu.log(f"  Train input file: {self.stage_io_dict['in']['input_train_npy_path']}", self.out_log)
         fu.log(f"    File size: {human_readable_file_size(self.stage_io_dict['in']['input_train_npy_path'])}", self.out_log)
         fu.log(f"  Number of atoms: {int(len(next(iter(self.train_dataloader))[0][0])/3)}", self.out_log)
-        fu.log(f"  Number of frames for training: {len(self.train_dataloader)}    Total number of frames: {int((len(self.train_dataloader)*self.train_dataloader.batch_size)/self.partition) if self.partition is not None else 'Unknown'}", self.out_log)  # type: ignore
+        fu.log(f"  Number of frames for training: {len(self.train_dataloader)*self.train_dataloader.batch_size} Total number of frames: {int((len(self.train_dataloader)*self.train_dataloader.batch_size)/self.partition) if self.partition is not None else 'Unknown'}", self.out_log)  # type: ignore
         fu.log(f"  Number of epochs: {self.num_epochs}", self.out_log)
         fu.log(f"  Partition: {self.partition}", self.out_log)
         fu.log(f"  Batch size: {self.batch_size}", self.out_log)
         fu.log(f"  Learning rate: {self.lr}", self.out_log)
         fu.log(f"  Learning rate step size: {self.lr_step_size}", self.out_log)
         fu.log(f"  Learning rate gamma: {self.gamma}", self.out_log)
         fu.log(f"  Number of layers: {self.num_layers}", self.out_log)
         fu.log(f"  Input dimensions: {self.input_dimensions}", self.out_log)
         fu.log(f"  Latent dimensions: {self.latent_dimensions}", self.out_log)
         fu.log(f"  Loss function: {str(self.loss_function).split('(')[0]}", self.out_log)
         fu.log(f"  Optimizer: {str(self.optimizer).split('(')[0]}", self.out_log)
+        fu.log(f"  Seed: {self.seed}", self.out_log)
         fu.log(f"  Checkpoint interval: {self.checkpoint_interval}", self.out_log)
         fu.log(f"  Log interval: {self.log_interval}\n", self.out_log)
 
         scheduler = torch.optim.lr_scheduler.StepLR(self.optimizer, step_size=self.lr_step_size, gamma=self.gamma)
         for epoch_index in range(self.num_epochs):
             loop_start_time: float = time.time()
 
-            # Training step
-            avg_train_loss: float = self.training_step(self.train_dataloader, self.optimizer, self.loss_function)
+            # Training & validation step
+            avg_train_loss, avg_validation_loss = self.training_step(self.train_dataloader, self.optimizer, self.loss_function)
             train_losses.append(avg_train_loss)
-
-            # Validation step
-            avg_validation_loss, _, _ = self.evaluate_model(self.validation_dataloader, self.loss_function)
             validation_losses.append(avg_validation_loss)
 
             # Logging
             if self.log_interval and (epoch_index % self.log_interval == 0 or epoch_index == self.num_epochs-1):
                 epoch_time: float = time.time() - loop_start_time
-                fu.log(f'{"Epoch":>4} {epoch_index+1}/{self.num_epochs} - Train Loss: {avg_train_loss:.3f}, Validation Loss: {avg_validation_loss:.3f}, LR: {scheduler.get_last_lr()}, Duration: {format_time(epoch_time)}, ETA: {format_time((self.num_epochs-(epoch_index+1))*epoch_time)}', self.out_log)
+                fu.log(f'{"Epoch":>4} {epoch_index+1}/{self.num_epochs}, Train Loss: {avg_train_loss:.3f}, Validation Loss: {avg_validation_loss:.3f}, LR: {scheduler.get_last_lr()[0]:.5f}, Duration: {format_time(epoch_time)}, ETA: {format_time((self.num_epochs-(epoch_index+1))*epoch_time)}', self.out_log)
                 loop_start_time = time.time()
 
             # Save checkpoint
             if self.checkpoint_interval and (epoch_index % self.checkpoint_interval == 0 or epoch_index == self.num_epochs-1):
                 checkpoint_path = str(Path(self.stage_io_dict.get("unique_dir", '')).joinpath(f'{self.output_checkpoint_prefix}_{epoch_index}.pth'))
                 fu.log(f'{"Saving: ":>4} {checkpoint_path}', self.out_log)
                 torch.save(self.model.state_dict(), checkpoint_path)
@@ -274,27 +281,36 @@
                 best_model: Dict = self.model.state_dict()
                 best_model_epoch: int = epoch_index
 
         fu.log(f"End Training, total time: {format_time((time.time() - start_time))}", self.out_log)
 
         return train_losses, validation_losses, best_model, best_model_epoch
 
-    def training_step(self, dataloader: torch.utils.data.DataLoader, optimizer: torch.optim.Optimizer, loss_function: torch.nn.modules.loss._Loss) -> float:
+    def training_step(self, dataloader: torch.utils.data.DataLoader, optimizer: torch.optim.Optimizer, loss_function: torch.nn.modules.loss._Loss) -> Tuple[float, float]:
         self.model.train()
-        losses: List[float] = []
+        train_losses: List[float] = []
         for data in dataloader:
             data = data[0].to(self.model.device)
             _, output = self.model(data)
             loss = loss_function(output, data)
             optimizer.zero_grad()
             loss.backward()
             optimizer.step()
-            losses.append(loss.item())
+            train_losses.append(loss.item())
+
+        self.model.eval()
+        valid_losses: List[float] = []
+        with torch.no_grad():
+            for data in dataloader:
+                data = data[0].to(self.model.device)
+                _, output = self.model(data)
+                loss = loss_function(output, data)
+                valid_losses.append(loss.item())
 
-        return float(np.mean(losses))
+        return float(np.mean(train_losses)), float(torch.mean(torch.tensor(valid_losses)))
 
     def evaluate_model(self, dataloader: torch.utils.data.DataLoader, loss_function: torch.nn.modules.loss._Loss) -> Tuple[float, np.ndarray, np.ndarray]:
         return execute_model(self.model, dataloader, self.input_dimensions, self.latent_dimensions, loss_function)
 
 
 def trainMDAE(input_train_npy_path: str, output_model_pth_path: str, input_model_pth_path: Optional[str] = None,
               output_train_data_npz_path: Optional[str] = None, output_performance_npz_path: Optional[str] = None,
```

### Comparing `biobb_pytorch-4.1.3/biobb_pytorch.egg-info/PKG-INFO` & `biobb_pytorch-4.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: biobb-pytorch
-Version: 4.1.3
+Name: biobb_pytorch
+Version: 4.2.0
 Summary: biobb_pytorch is the Biobb module collection to create and train ML & DL models.
 Home-page: https://github.com/bioexcel/biobb_pytorch
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
 Project-URL: Documentation, http://biobb-pytorch.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
@@ -21,15 +21,15 @@
 License-File: LICENSE
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_pytorch?label=Version)](https://GitHub.com/bioexcel/biobb_pytorch/tags/)
 [![](https://img.shields.io/pypi/v/biobb-pytorch.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-pytorch/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_pytorch?label=Conda)](https://anaconda.org/bioconda/biobb_pytorch)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_pytorch?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_pytorch)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_pytorch?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.3--pyhdfd78af_1)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_pytorch:4.2.0--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_pytorch)
 [![](https://img.shields.io/pypi/pyversions/biobb-pytorch.svg?label=Python%20Versions)](https://pypi.org/project/biobb-pytorch/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_pytorch)
 
 [![](https://readthedocs.org/projects/biobb-pytorch/badge/?version=latest&label=Docs)](https://biobb-pytorch.readthedocs.io/en/latest/?badge=latest)
@@ -45,75 +45,75 @@
 [![](https://img.shields.io/github/issues/bioexcel/biobb_pytorch.svg?color=brightgreen&label=Issues)](https://GitHub.com/bioexcel/biobb_pytorch/issues/)
 
 [![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F-green)](https://fair-software.eu)
 [![](https://www.bestpractices.dev/projects/8847/badge)](https://www.bestpractices.dev/projects/8847)
 
 [](https://bestpractices.coreinfrastructure.org/projects/8847/badge)
 
- [//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractives URL)
+[//]: # (The previous line invisible link is for compatibility with the howfairis script https://github.com/fair-software/howfairis-github-action/tree/main wich uses the old bestpractices URL)
 
 
 # biobb_pytorch
 
 ### Introduction
 biobb_pytorch is the Biobb module collection to create and train ML & DL models using the popular [PyTorch](https://pytorch.org/) Python library.
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb-pytorch.readthedocs.io/en/latest/).
 
 ### Version
-v4.1.3 2024.2
+v4.2.0 2024.2
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_pytorch>=4.1.3"
+        pip install "biobb_pytorch>=4.2.0"
 
 
 * Usage: [Python API documentation](https://biobb-pytorch.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_pytorch>=4.1.3"
+        conda install -c bioconda "biobb_pytorch>=4.2.0"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-pytorch.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-pytorch.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_pytorch:4.1.3--pyhdfd78af_1
+        docker pull quay.io/biocontainers/biobb_pytorch:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_pytorch:4.1.3--pyhdfd78af_1 <command>
+        docker run quay.io/biocontainers/biobb_pytorch:4.2.0--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_pytorch.sif https://depot.galaxyproject.org/singularity/biobb_pytorch:4.1.3--pyhdfd78af_1
+        singularity pull --name biobb_pytorch.sif https://depot.galaxyproject.org/singularity/biobb_pytorch:4.2.0--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_pytorch.sif <command>
```

### Comparing `biobb_pytorch-4.1.3/setup.py` & `biobb_pytorch-4.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_pytorch",
-    version="4.1.3",
+    version="4.2.0",
     author="Biobb developers",
     author_email="pau.andrio@bsc.es",
     description="biobb_pytorch is the Biobb module collection to create and train ML & DL models.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_pytorch",
     project_urls={
         "Documentation": "http://biobb-pytorch.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs', 'test']),
-    install_requires=['biobb_common==4.1.0', 'torch'],
+    install_requires=['biobb_common==4.2.0', 'torch'],
     python_requires='>=3.8',
     entry_points={
         "console_scripts": [
             "train_mdae = biobb_pytorch.mdae.train_mdae:main",
             "apply_mdae = biobb_pytorch.mdae.apply_mdae:main"
         ]
     },
```


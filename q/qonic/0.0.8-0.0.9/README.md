# Comparing `tmp/qonic-0.0.8.tar.gz` & `tmp/qonic-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qonic-0.0.8.tar", last modified: Sun Jan 29 18:09:07 2023, max compression
+gzip compressed data, was "qonic-0.0.9.tar", last modified: Fri May 24 19:48:59 2024, max compression
```

## Comparing `qonic-0.0.8.tar` & `qonic-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 18:09:07.110535 qonic-0.0.8/
--rw-r--r--   0 root         (0) root         (0)    16280 2023-01-29 18:09:07.110535 qonic-0.0.8/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)    15794 2023-01-29 00:46:32.000000 qonic-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 18:09:07.106535 qonic-0.0.8/qonic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 18:09:07.110535 qonic-0.0.8/qonic/ConstraintSatisfaction/
--rw-rw-r--   0 root         (0) root         (0)    72927 2022-10-09 17:06:18.000000 qonic-0.0.8/qonic/ConstraintSatisfaction/ConstraintSatisfaction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 18:09:07.110535 qonic-0.0.8/qonic/QProgram/
--rw-rw-r--   0 root         (0) root         (0)    12571 2022-10-23 03:52:17.000000 qonic-0.0.8/qonic/QProgram/QProgram.py
--rw-rw-r--   0 root         (0) root         (0)      152 2023-01-29 18:06:04.000000 qonic-0.0.8/qonic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 18:09:07.110535 qonic-0.0.8/qonic.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16280 2023-01-29 18:09:07.000000 qonic-0.0.8/qonic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      272 2023-01-29 18:09:07.000000 qonic-0.0.8/qonic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-29 18:09:07.000000 qonic-0.0.8/qonic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-01-29 18:09:07.000000 qonic-0.0.8/qonic.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-01-29 18:09:07.000000 qonic-0.0.8/qonic.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      131 2023-01-29 18:09:07.110535 qonic-0.0.8/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      821 2023-01-29 18:09:00.000000 qonic-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 19:48:59.868789 qonic-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)    16616 2024-05-24 19:48:59.868789 qonic-0.0.9/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    15794 2023-01-29 00:46:32.000000 qonic-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 19:48:59.868789 qonic-0.0.9/qonic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 19:48:59.868789 qonic-0.0.9/qonic/ConstraintSatisfaction/
+-rw-rw-r--   0 root         (0) root         (0)    72927 2022-10-09 17:06:18.000000 qonic-0.0.9/qonic/ConstraintSatisfaction/ConstraintSatisfaction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 19:48:59.868789 qonic-0.0.9/qonic/QProgram/
+-rw-rw-r--   0 root         (0) root         (0)    12586 2024-05-24 19:43:45.000000 qonic-0.0.9/qonic/QProgram/QProgram.py
+-rw-rw-r--   0 root         (0) root         (0)      152 2023-01-29 18:06:04.000000 qonic-0.0.9/qonic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 19:48:59.868789 qonic-0.0.9/qonic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16616 2024-05-24 19:48:59.000000 qonic-0.0.9/qonic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      272 2024-05-24 19:48:59.000000 qonic-0.0.9/qonic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 19:48:59.000000 qonic-0.0.9/qonic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      191 2024-05-24 19:48:59.000000 qonic-0.0.9/qonic.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-24 19:48:59.000000 qonic-0.0.9/qonic.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      131 2024-05-24 19:48:59.868789 qonic-0.0.9/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      881 2024-05-24 19:48:38.000000 qonic-0.0.9/setup.py
```

### Comparing `qonic-0.0.8/PKG-INFO` & `qonic-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 Metadata-Version: 2.1
 Name: qonic
-Version: 0.0.8
+Version: 0.0.9
 Summary: The Qonic project is an open source, expandable framework for solving problems using hybrid quantum computing solutions.
 Home-page: https://github.com/Qonic-Team/qonic.git
+Download-URL: https://github.com/Qonic-Team/qonic/archive/refs/heads/main.zip
 Author: cogrpar
 Author-email: owen.r.welsh@hotmail.com
 License: Apache License 2.0
-Download-URL: https://github.com/Qonic-Team/qonic/archive/refs/heads/main.zip
 Keywords: qonic,quantum computing
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Requires-Dist: numpy>=1.22.2
+Requires-Dist: sympy>=1.12
+Requires-Dist: PyYAML>=5.4.1
+Requires-Dist: tequila-basic>=1.8.1
+Requires-Dist: qiskit>=0.21.2
+Requires-Dist: forest-benchmarking>=0.8.0
+Requires-Dist: dimod>=0.11.5
+Requires-Dist: dwavebinarycsp>=0.2.0
+Requires-Dist: pillow>=10.3.0
+Requires-Dist: fonttools>=4.43.0
+Requires-Dist: setuptools>=65.5.1
 
 [![Python application](https://github.com/Qonic-Team/qonic/actions/workflows/python-app.yml/badge.svg)](https://github.com/Qonic-Team/qonic/actions/workflows/python-app.yml)
 [![CodeQL](https://github.com/Qonic-Team/qonic/actions/workflows/codeql.yml/badge.svg)](https://github.com/Qonic-Team/qonic/actions/workflows/codeql.yml)
 <sup>[`Snyk Vulnerability Report`](https://snyk.io/test/github/Qonic-Team/qonic?targetFile=source_dir/requirements.txt)</sup>
 
 # qonic
 The Qonic project is an open source, expandable framework for solving problems using hybrid quantum computing solutions.  The base library includes tools for defining optimization problems to be run on gate quantum computers on a variety of backends or simulators, as well as on simulated or physical quantum annealers.
@@ -302,9 +312,7 @@
   1
   ```
 
 **Attributes**
 * `__b <type 'dict'>`: a dictionary storing a list of binary variables and the corresponding names
 * `__f <type 'dict'>`: a dictionary storing the binary polynomial expressions approximating 16 bit real floats (stored as strings) and the corresponding float variable names
 * `__j <type 'dict'>` a dictionary storing the binary polynomial expressions approximating 32 bit complex floats (stored as strings) and the corresponding float variable namesu
-
-
```

### Comparing `qonic-0.0.8/README.md` & `qonic-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `qonic-0.0.8/qonic/ConstraintSatisfaction/ConstraintSatisfaction.py` & `qonic-0.0.9/qonic/ConstraintSatisfaction/ConstraintSatisfaction.py`

 * *Files identical despite different names*

### Comparing `qonic-0.0.8/qonic/QProgram/QProgram.py` & `qonic-0.0.9/qonic/QProgram/QProgram.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,27 +206,27 @@
     def to_superop(self): # function to return the super operator form of the current QProgram
         return kraus2superop([self.to_unitary()])
 
     def wlp(self, Q): # function to compute the weakest liberal precondition for the current QProgram given a postcondition Q
         if (np.shape(Q)[0] != np.shape(Q)[1] or np.shape(Q)[0] != len(self.q̅)):
             raise ValueError('the passed postcondition has a different shape than the current program\'s unitary')
 
-        S_star = np.conj(self.to_superop()) # the complex conjugate of the QProgram in super operator form: ⟦S⟧*
+        S_star = np.transpose(np.conj(self.to_superop())) # the complex conjugate of the QProgram in super operator form: ⟦S⟧*
         dif = np.identity(len(self.q̅)) - Q # the difference (I - Q)
         P_dash = np.identity(len(self.q̅)) - unvec(np.matmul(S_star, vec(dif))) # calculate P' using I - ⟦S⟧*(I-Q)
         return P_dash
 
-    def correct_q_hoare_triple(self, Q, P): # function that checks if the QHoare triple {Q}S{P} is valid
+    def correct_q_hoare_triple(self, P, Q): # function that checks if the QHoare triple {P}S{Q} is valid
         if (np.shape(Q)[0] != np.shape(Q)[1] or np.shape(Q)[0] != len(self.q̅)):
             raise ValueError('the passed postcondition has a different shape than the current program\'s unitary')
 
         if (np.shape(Q)[0] != np.shape(P)[1] or np.shape(P)[0] != len(self.q̅)):
             raise ValueError('the passed precondition has a different shape than the current program\'s unitary')
 
         P_dash = self.wlp(Q)
 
         # check to see if P ⊑ P' (where ⊑ denotes a Löwner partial order)
         dif = P_dash - P
-        if (np.all(np.linalg.eigvals(dif) >= -0.000001)): # the partial order is satisfied
+        if (np.sum(np.linalg.eigvals(dif) >= -0.000001)): # the partial order is satisfied
             return True # the program is correct
         else:
-            return False # the program is not correct
+            return False # the program is not correct
```

### Comparing `qonic-0.0.8/qonic.egg-info/PKG-INFO` & `qonic-0.0.9/qonic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 Metadata-Version: 2.1
 Name: qonic
-Version: 0.0.8
+Version: 0.0.9
 Summary: The Qonic project is an open source, expandable framework for solving problems using hybrid quantum computing solutions.
 Home-page: https://github.com/Qonic-Team/qonic.git
+Download-URL: https://github.com/Qonic-Team/qonic/archive/refs/heads/main.zip
 Author: cogrpar
 Author-email: owen.r.welsh@hotmail.com
 License: Apache License 2.0
-Download-URL: https://github.com/Qonic-Team/qonic/archive/refs/heads/main.zip
 Keywords: qonic,quantum computing
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Requires-Dist: numpy>=1.22.2
+Requires-Dist: sympy>=1.12
+Requires-Dist: PyYAML>=5.4.1
+Requires-Dist: tequila-basic>=1.8.1
+Requires-Dist: qiskit>=0.21.2
+Requires-Dist: forest-benchmarking>=0.8.0
+Requires-Dist: dimod>=0.11.5
+Requires-Dist: dwavebinarycsp>=0.2.0
+Requires-Dist: pillow>=10.3.0
+Requires-Dist: fonttools>=4.43.0
+Requires-Dist: setuptools>=65.5.1
 
 [![Python application](https://github.com/Qonic-Team/qonic/actions/workflows/python-app.yml/badge.svg)](https://github.com/Qonic-Team/qonic/actions/workflows/python-app.yml)
 [![CodeQL](https://github.com/Qonic-Team/qonic/actions/workflows/codeql.yml/badge.svg)](https://github.com/Qonic-Team/qonic/actions/workflows/codeql.yml)
 <sup>[`Snyk Vulnerability Report`](https://snyk.io/test/github/Qonic-Team/qonic?targetFile=source_dir/requirements.txt)</sup>
 
 # qonic
 The Qonic project is an open source, expandable framework for solving problems using hybrid quantum computing solutions.  The base library includes tools for defining optimization problems to be run on gate quantum computers on a variety of backends or simulators, as well as on simulated or physical quantum annealers.
@@ -302,9 +312,7 @@
   1
   ```
 
 **Attributes**
 * `__b <type 'dict'>`: a dictionary storing a list of binary variables and the corresponding names
 * `__f <type 'dict'>`: a dictionary storing the binary polynomial expressions approximating 16 bit real floats (stored as strings) and the corresponding float variable names
 * `__j <type 'dict'>` a dictionary storing the binary polynomial expressions approximating 32 bit complex floats (stored as strings) and the corresponding float variable namesu
-
-
```

### Comparing `qonic-0.0.8/setup.py` & `qonic-0.0.9/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'qonic',
     packages = ['qonic', 'qonic.ConstraintSatisfaction', 'qonic.QProgram'],
-    version = '0.0.8',
+    version = '0.0.9',
     description = 'The Qonic project is an open source, expandable framework for solving problems using hybrid quantum computing solutions.',
     author = 'cogrpar',
     author_email = 'owen.r.welsh@hotmail.com',
     url = 'https://github.com/Qonic-Team/qonic.git',
     download_url = 'https://github.com/Qonic-Team/qonic/archive/refs/heads/main.zip',
     license='Apache License 2.0',
     keywords = ['qonic', 'quantum computing'],
     setup_requires=['wheel'],
-    install_requires=['numpy>=1.19.2', 'sympy>=1.11', 'PyYAML>=5.4.1', 'tequila-basic>=1.8.1', 'qiskit>=0.21.2', 'forest-benchmarking>=0.8.0', 'dimod>=0.11.5', 'dwavebinarycsp>=0.2.0']
+    install_requires=['numpy>=1.22.2', 'sympy>=1.12', 'PyYAML>=5.4.1', 'tequila-basic>=1.8.1', 'qiskit>=0.21.2', 'forest-benchmarking>=0.8.0', 'dimod>=0.11.5','dwavebinarycsp>=0.2.0', 'pillow>=10.3.0', 'fonttools>=4.43.0', 'setuptools>=65.5.1']
 )
```


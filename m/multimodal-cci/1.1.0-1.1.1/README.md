# Comparing `tmp/multimodal_cci-1.1.0.tar.gz` & `tmp/multimodal_cci-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multimodal_cci-1.1.0.tar", last modified: Thu May 23 02:10:31 2024, max compression
+gzip compressed data, was "multimodal_cci-1.1.1.tar", last modified: Fri May 24 04:48:51 2024, max compression
```

## Comparing `multimodal_cci-1.1.0.tar` & `multimodal_cci-1.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 uqlhocke (1100037689) qris-uq  (60001)        0 2024-05-23 02:10:31.885646 multimodal_cci-1.1.0/
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     1525 2024-03-05 02:02:14.000000 multimodal_cci-1.1.0/LICENSE.txt
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)        0 2024-03-05 02:02:14.000000 multimodal_cci-1.1.0/MANIFEST.in
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     5593 2024-05-23 02:10:31.885450 multimodal_cci-1.1.0/PKG-INFO
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     3087 2024-03-22 01:57:30.000000 multimodal_cci-1.1.0/README.md
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)       85 2024-03-05 02:02:14.000000 multimodal_cci-1.1.0/pyproject.toml
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)      982 2024-05-23 02:10:31.886077 multimodal_cci-1.1.0/setup.cfg
-drwxr-xr-x   0 uqlhocke (1100037689) qris-uq  (60001)        0 2024-05-23 02:10:31.870690 multimodal_cci-1.1.0/src/
-drwxr-xr-x   0 uqlhocke (1100037689) qris-uq  (60001)        0 2024-05-23 02:10:31.878288 multimodal_cci-1.1.0/src/multimodal_cci/
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)      168 2024-04-16 04:38:24.000000 multimodal_cci-1.1.0/src/multimodal_cci/__init__.py
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)    23578 2024-05-23 02:08:00.000000 multimodal_cci-1.1.0/src/multimodal_cci/analysis.py
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)    10198 2024-04-22 06:47:06.000000 multimodal_cci-1.1.0/src/multimodal_cci/integration.py
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     7068 2024-03-05 02:02:14.000000 multimodal_cci-1.1.0/src/multimodal_cci/plot_helper.py
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)    17908 2024-05-23 01:47:03.000000 multimodal_cci-1.1.0/src/multimodal_cci/plotting.py
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     3496 2024-03-05 02:02:14.000000 multimodal_cci-1.1.0/src/multimodal_cci/scoring.py
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     8889 2024-04-17 06:13:41.000000 multimodal_cci-1.1.0/src/multimodal_cci/tools.py
-drwxr-xr-x   0 uqlhocke (1100037689) qris-uq  (60001)        0 2024-05-23 02:10:31.881376 multimodal_cci-1.1.0/src/multimodal_cci.egg-info/
-drwxr-xr-x   0 uqlhocke (1100037689) qris-uq  (60001)        0 2024-05-23 02:10:31.884800 multimodal_cci-1.1.0/src/multimodal_cci.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     2281 2024-03-05 02:02:14.000000 multimodal_cci-1.1.0/src/multimodal_cci.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)      393 2024-03-05 02:02:14.000000 multimodal_cci-1.1.0/src/multimodal_cci.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)        1 2024-03-05 02:02:14.000000 multimodal_cci-1.1.0/src/multimodal_cci.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)       32 2024-03-05 02:02:14.000000 multimodal_cci-1.1.0/src/multimodal_cci.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)       15 2024-03-05 02:02:14.000000 multimodal_cci-1.1.0/src/multimodal_cci.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     5593 2024-05-23 02:10:31.878999 multimodal_cci-1.1.0/src/multimodal_cci.egg-info/PKG-INFO
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)      845 2024-05-23 02:10:31.879437 multimodal_cci-1.1.0/src/multimodal_cci.egg-info/SOURCES.txt
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)        1 2024-05-23 02:10:31.880275 multimodal_cci-1.1.0/src/multimodal_cci.egg-info/dependency_links.txt
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)      152 2024-05-23 02:10:31.881004 multimodal_cci-1.1.0/src/multimodal_cci.egg-info/requires.txt
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)       15 2024-05-23 02:10:31.881474 multimodal_cci-1.1.0/src/multimodal_cci.egg-info/top_level.txt
+drwxr-xr-x   0 uqlhocke (1100037689) qris-uq  (60001)        0 2024-05-24 04:48:51.888989 multimodal_cci-1.1.1/
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     1525 2024-03-05 02:02:14.000000 multimodal_cci-1.1.1/LICENSE.txt
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)        0 2024-03-05 02:02:14.000000 multimodal_cci-1.1.1/MANIFEST.in
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     5555 2024-05-24 04:48:51.888315 multimodal_cci-1.1.1/PKG-INFO
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     3049 2024-05-23 03:02:27.000000 multimodal_cci-1.1.1/README.md
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)       85 2024-03-05 02:02:14.000000 multimodal_cci-1.1.1/pyproject.toml
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)      982 2024-05-24 04:48:51.889762 multimodal_cci-1.1.1/setup.cfg
+drwxr-xr-x   0 uqlhocke (1100037689) qris-uq  (60001)        0 2024-05-24 04:48:51.841642 multimodal_cci-1.1.1/src/
+drwxr-xr-x   0 uqlhocke (1100037689) qris-uq  (60001)        0 2024-05-24 04:48:51.873052 multimodal_cci-1.1.1/src/multimodal_cci/
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)      168 2024-05-24 04:48:28.000000 multimodal_cci-1.1.1/src/multimodal_cci/__init__.py
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)    23578 2024-05-23 02:08:00.000000 multimodal_cci-1.1.1/src/multimodal_cci/analysis.py
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)    10198 2024-04-22 06:47:06.000000 multimodal_cci-1.1.1/src/multimodal_cci/integration.py
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     7068 2024-03-05 02:02:14.000000 multimodal_cci-1.1.1/src/multimodal_cci/plot_helper.py
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)    17908 2024-05-23 01:47:03.000000 multimodal_cci-1.1.1/src/multimodal_cci/plotting.py
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     3496 2024-03-05 02:02:14.000000 multimodal_cci-1.1.1/src/multimodal_cci/scoring.py
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     8889 2024-04-17 06:13:41.000000 multimodal_cci-1.1.1/src/multimodal_cci/tools.py
+drwxr-xr-x   0 uqlhocke (1100037689) qris-uq  (60001)        0 2024-05-24 04:48:51.879051 multimodal_cci-1.1.1/src/multimodal_cci.egg-info/
+drwxr-xr-x   0 uqlhocke (1100037689) qris-uq  (60001)        0 2024-05-24 04:48:51.886202 multimodal_cci-1.1.1/src/multimodal_cci.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     2281 2024-03-05 02:02:14.000000 multimodal_cci-1.1.1/src/multimodal_cci.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)      393 2024-03-05 02:02:14.000000 multimodal_cci-1.1.1/src/multimodal_cci.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)        1 2024-03-05 02:02:14.000000 multimodal_cci-1.1.1/src/multimodal_cci.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)       32 2024-03-05 02:02:14.000000 multimodal_cci-1.1.1/src/multimodal_cci.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)       15 2024-03-05 02:02:14.000000 multimodal_cci-1.1.1/src/multimodal_cci.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     5555 2024-05-24 04:48:51.874778 multimodal_cci-1.1.1/src/multimodal_cci.egg-info/PKG-INFO
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)      845 2024-05-24 04:48:51.875625 multimodal_cci-1.1.1/src/multimodal_cci.egg-info/SOURCES.txt
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)        1 2024-05-24 04:48:51.876617 multimodal_cci-1.1.1/src/multimodal_cci.egg-info/dependency_links.txt
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)      152 2024-05-24 04:48:51.877870 multimodal_cci-1.1.1/src/multimodal_cci.egg-info/requires.txt
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)       15 2024-05-24 04:48:51.879215 multimodal_cci-1.1.1/src/multimodal_cci.egg-info/top_level.txt
```

### Comparing `multimodal_cci-1.1.0/LICENSE.txt` & `multimodal_cci-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `multimodal_cci-1.1.0/PKG-INFO` & `multimodal_cci-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: multimodal_cci
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python package for processing multi-modal CCI data
 Home-page: https://github.com/BiomedicalMachineLearning/MultimodalCCI
 Author: Genomics and Machine Learning lab
 Author-email: l.hockey@uq.edu.au
 Project-URL: Bug Tracker, https://github.com/BiomedicalMachineLearning/MultimodalCCI/issues
 Project-URL: repository, https://github.com/BiomedicalMachineLearning/MultimodalCCI
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy>=1.24.0
 Requires-Dist: pandas>=2.1.4
 Requires-Dist: networkx>=3.2.1
 Requires-Dist: matplotlib>=3.8.2
 Requires-Dist: scikit-learn>=1.3.0
@@ -88,27 +88,25 @@
 
 ## CCI Integration
 
 MMCCI allows users to integrate multiple CCI results together, both:
 1. Samples from a single modality (eg. Visium)
 2. Samples from multiple modalities (eg. Visium, Xenium and CosMX)
 
-![Integration Method](docs/images/integration_method.png)
+![Integration and Analysis Method](docs/images/analyses_pipeline.png)
 
 ## CCI Analysis
 
 MMCCI provides multiple useful analyses that can be run on the integrated networks or from a single sample:
 1. Network comparison between groups with permutation testing
 2. CLustering of LR pairs with similar networks
 3. Clustering of spots/cells with similar interaction scores
 4. Sender-receiver LR querying
 5. GSEA pathway analysis
 
-![Downstream Analyses](docs/images/analyses.png)
-
 ### Pipeline Diagram
 
 ![MMCCI Pipeline](docs/images/pipeline.png)
 
 ## Citing MMCCI
 
 If you have used MMCCI in your research, please consider citing us:
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: multimodal_cci Version: 1.1.0 Summary: A Python
+Metadata-Version: 2.1 Name: multimodal_cci Version: 1.1.1 Summary: A Python
 package for processing multi-modal CCI data Home-page: https://github.com/
 BiomedicalMachineLearning/MultimodalCCI Author: Genomics and Machine Learning
 lab Author-email: l.hockey@uq.edu.au Project-URL: Bug Tracker, https://
 github.com/BiomedicalMachineLearning/MultimodalCCI/issues Project-URL:
 repository, https://github.com/BiomedicalMachineLearning/MultimodalCCI
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
+Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE.txt Requires-Dist: numpy>=1.24.0 Requires-Dist: pandas>=2.1.4 Requires-
 Dist: networkx>=3.2.1 Requires-Dist: matplotlib>=3.8.2 Requires-Dist: scikit-
 learn>=1.3.0 Requires-Dist: scipy>=1.9.1 Requires-Dist: tqdm>=4.66.1 Requires-
 Dist: gseapy>=1.1.1 Requires-Dist: scanpy>=1.9.0 Requires-Dist: seaborn>=0.11.2
 # MMCCI: Multimodal Cell-Cell Interaction Integrative Analysis of Single Cell
 and Spatial Data
                     PPaacckkaaggee _[_P_y_P_I_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _d_o_w_n_l_o_a_d_s_]
@@ -27,38 +27,37 @@
 issues raised by users. - There is a brain aging tutorial notebook [here]
 (examples/brain_aging_example.ipynb) - There is a melanoma tutorial notebook
 [here](examples/melanoma_example.ipynb) - To understand how to load CCI results
 from different tools, look at this notebook [here](examples/
 loading_CCI_results.ipynb) ## CCI Integration MMCCI allows users to integrate
 multiple CCI results together, both: 1. Samples from a single modality (eg.
 Visium) 2. Samples from multiple modalities (eg. Visium, Xenium and CosMX) !
-[Integration Method](docs/images/integration_method.png) ## CCI Analysis MMCCI
-provides multiple useful analyses that can be run on the integrated networks or
-from a single sample: 1. Network comparison between groups with permutation
-testing 2. CLustering of LR pairs with similar networks 3. Clustering of spots/
-cells with similar interaction scores 4. Sender-receiver LR querying 5. GSEA
-pathway analysis ![Downstream Analyses](docs/images/analyses.png) ### Pipeline
-Diagram ![MMCCI Pipeline](docs/images/pipeline.png) ## Citing MMCCI If you have
-used MMCCI in your research, please consider citing us: ``` Hockey, L., Mulay,
-O., Xiong, Z., Khosrotehrani, K., Nefzger, C. M., & Nguyen, Q. (2024). MMCCI:
-Multimodal Cell-Cell Interaction Integrative Analysis of Single Cell and
-Spatial Data. bioRxiv. doi:10.1101/2024.02.28.582639 ``` BSD License Copyright
-(c) 2024, Genomics and Machine Learning lab All rights reserved. Redistribution
-and use in source and binary forms, with or without modification, are permitted
-provided that the following conditions are met: * Redistributions of source
-code must retain the above copyright notice, this list of conditions and the
-following disclaimer. * Redistributions in binary form must reproduce the above
-copyright notice, this list of conditions and the following disclaimer in the
-documentation and/or other materials provided with the distribution. * Neither
-the name of the copyright holder nor the names of its contributors may be used
-to endorse or promote products derived from this software without specific
-prior written permission. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS
-AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT
-NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A
-PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
-CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
-EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT
-OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
-INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
-CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING
-IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY
-OF SUCH DAMAGE.
+[Integration and Analysis Method](docs/images/analyses_pipeline.png) ## CCI
+Analysis MMCCI provides multiple useful analyses that can be run on the
+integrated networks or from a single sample: 1. Network comparison between
+groups with permutation testing 2. CLustering of LR pairs with similar networks
+3. Clustering of spots/cells with similar interaction scores 4. Sender-receiver
+LR querying 5. GSEA pathway analysis ### Pipeline Diagram ![MMCCI Pipeline]
+(docs/images/pipeline.png) ## Citing MMCCI If you have used MMCCI in your
+research, please consider citing us: ``` Hockey, L., Mulay, O., Xiong, Z.,
+Khosrotehrani, K., Nefzger, C. M., & Nguyen, Q. (2024). MMCCI: Multimodal Cell-
+Cell Interaction Integrative Analysis of Single Cell and Spatial Data. bioRxiv.
+doi:10.1101/2024.02.28.582639 ``` BSD License Copyright (c) 2024, Genomics and
+Machine Learning lab All rights reserved. Redistribution and use in source and
+binary forms, with or without modification, are permitted provided that the
+following conditions are met: * Redistributions of source code must retain the
+above copyright notice, this list of conditions and the following disclaimer. *
+Redistributions in binary form must reproduce the above copyright notice, this
+list of conditions and the following disclaimer in the documentation and/or
+other materials provided with the distribution. * Neither the name of the
+copyright holder nor the names of its contributors may be used to endorse or
+promote products derived from this software without specific prior written
+permission. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
+"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE
+GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
+HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
+LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
+OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `multimodal_cci-1.1.0/README.md` & `multimodal_cci-1.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -62,27 +62,25 @@
 
 ## CCI Integration
 
 MMCCI allows users to integrate multiple CCI results together, both:
 1. Samples from a single modality (eg. Visium)
 2. Samples from multiple modalities (eg. Visium, Xenium and CosMX)
 
-![Integration Method](docs/images/integration_method.png)
+![Integration and Analysis Method](docs/images/analyses_pipeline.png)
 
 ## CCI Analysis
 
 MMCCI provides multiple useful analyses that can be run on the integrated networks or from a single sample:
 1. Network comparison between groups with permutation testing
 2. CLustering of LR pairs with similar networks
 3. Clustering of spots/cells with similar interaction scores
 4. Sender-receiver LR querying
 5. GSEA pathway analysis
 
-![Downstream Analyses](docs/images/analyses.png)
-
 ### Pipeline Diagram
 
 ![MMCCI Pipeline](docs/images/pipeline.png)
 
 ## Citing MMCCI
 
 If you have used MMCCI in your research, please consider citing us:
```

#### html2text {}

```diff
@@ -14,18 +14,18 @@
 issues raised by users. - There is a brain aging tutorial notebook [here]
 (examples/brain_aging_example.ipynb) - There is a melanoma tutorial notebook
 [here](examples/melanoma_example.ipynb) - To understand how to load CCI results
 from different tools, look at this notebook [here](examples/
 loading_CCI_results.ipynb) ## CCI Integration MMCCI allows users to integrate
 multiple CCI results together, both: 1. Samples from a single modality (eg.
 Visium) 2. Samples from multiple modalities (eg. Visium, Xenium and CosMX) !
-[Integration Method](docs/images/integration_method.png) ## CCI Analysis MMCCI
-provides multiple useful analyses that can be run on the integrated networks or
-from a single sample: 1. Network comparison between groups with permutation
-testing 2. CLustering of LR pairs with similar networks 3. Clustering of spots/
-cells with similar interaction scores 4. Sender-receiver LR querying 5. GSEA
-pathway analysis ![Downstream Analyses](docs/images/analyses.png) ### Pipeline
-Diagram ![MMCCI Pipeline](docs/images/pipeline.png) ## Citing MMCCI If you have
-used MMCCI in your research, please consider citing us: ``` Hockey, L., Mulay,
-O., Xiong, Z., Khosrotehrani, K., Nefzger, C. M., & Nguyen, Q. (2024). MMCCI:
-Multimodal Cell-Cell Interaction Integrative Analysis of Single Cell and
-Spatial Data. bioRxiv. doi:10.1101/2024.02.28.582639 ```
+[Integration and Analysis Method](docs/images/analyses_pipeline.png) ## CCI
+Analysis MMCCI provides multiple useful analyses that can be run on the
+integrated networks or from a single sample: 1. Network comparison between
+groups with permutation testing 2. CLustering of LR pairs with similar networks
+3. Clustering of spots/cells with similar interaction scores 4. Sender-receiver
+LR querying 5. GSEA pathway analysis ### Pipeline Diagram ![MMCCI Pipeline]
+(docs/images/pipeline.png) ## Citing MMCCI If you have used MMCCI in your
+research, please consider citing us: ``` Hockey, L., Mulay, O., Xiong, Z.,
+Khosrotehrani, K., Nefzger, C. M., & Nguyen, Q. (2024). MMCCI: Multimodal Cell-
+Cell Interaction Integrative Analysis of Single Cell and Spatial Data. bioRxiv.
+doi:10.1101/2024.02.28.582639 ```
```

### Comparing `multimodal_cci-1.1.0/setup.cfg` & `multimodal_cci-1.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = multimodal_cci
-version = 1.1.0
+version = 1.1.1
 author = Genomics and Machine Learning lab
 author_email = l.hockey@uq.edu.au
 description = A Python package for processing multi-modal CCI data
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/BiomedicalMachineLearning/MultimodalCCI
 project_urls = 
@@ -15,15 +15,15 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.9
+python_requires = >=3.8
 install_requires = 
 	numpy>=1.24.0
 	pandas>=2.1.4
 	networkx>=3.2.1
 	matplotlib>=3.8.2
 	scikit-learn>=1.3.0
 	scipy>=1.9.1
```

### Comparing `multimodal_cci-1.1.0/src/multimodal_cci/analysis.py` & `multimodal_cci-1.1.1/src/multimodal_cci/analysis.py`

 * *Files identical despite different names*

### Comparing `multimodal_cci-1.1.0/src/multimodal_cci/integration.py` & `multimodal_cci-1.1.1/src/multimodal_cci/integration.py`

 * *Files identical despite different names*

### Comparing `multimodal_cci-1.1.0/src/multimodal_cci/plot_helper.py` & `multimodal_cci-1.1.1/src/multimodal_cci/plot_helper.py`

 * *Files identical despite different names*

### Comparing `multimodal_cci-1.1.0/src/multimodal_cci/plotting.py` & `multimodal_cci-1.1.1/src/multimodal_cci/plotting.py`

 * *Files identical despite different names*

### Comparing `multimodal_cci-1.1.0/src/multimodal_cci/scoring.py` & `multimodal_cci-1.1.1/src/multimodal_cci/scoring.py`

 * *Files identical despite different names*

### Comparing `multimodal_cci-1.1.0/src/multimodal_cci/tools.py` & `multimodal_cci-1.1.1/src/multimodal_cci/tools.py`

 * *Files identical despite different names*

### Comparing `multimodal_cci-1.1.0/src/multimodal_cci.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint` & `multimodal_cci-1.1.1/src/multimodal_cci.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint`

 * *Files identical despite different names*

### Comparing `multimodal_cci-1.1.0/src/multimodal_cci.egg-info/PKG-INFO` & `multimodal_cci-1.1.1/src/multimodal_cci.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: multimodal_cci
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python package for processing multi-modal CCI data
 Home-page: https://github.com/BiomedicalMachineLearning/MultimodalCCI
 Author: Genomics and Machine Learning lab
 Author-email: l.hockey@uq.edu.au
 Project-URL: Bug Tracker, https://github.com/BiomedicalMachineLearning/MultimodalCCI/issues
 Project-URL: repository, https://github.com/BiomedicalMachineLearning/MultimodalCCI
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy>=1.24.0
 Requires-Dist: pandas>=2.1.4
 Requires-Dist: networkx>=3.2.1
 Requires-Dist: matplotlib>=3.8.2
 Requires-Dist: scikit-learn>=1.3.0
@@ -88,27 +88,25 @@
 
 ## CCI Integration
 
 MMCCI allows users to integrate multiple CCI results together, both:
 1. Samples from a single modality (eg. Visium)
 2. Samples from multiple modalities (eg. Visium, Xenium and CosMX)
 
-![Integration Method](docs/images/integration_method.png)
+![Integration and Analysis Method](docs/images/analyses_pipeline.png)
 
 ## CCI Analysis
 
 MMCCI provides multiple useful analyses that can be run on the integrated networks or from a single sample:
 1. Network comparison between groups with permutation testing
 2. CLustering of LR pairs with similar networks
 3. Clustering of spots/cells with similar interaction scores
 4. Sender-receiver LR querying
 5. GSEA pathway analysis
 
-![Downstream Analyses](docs/images/analyses.png)
-
 ### Pipeline Diagram
 
 ![MMCCI Pipeline](docs/images/pipeline.png)
 
 ## Citing MMCCI
 
 If you have used MMCCI in your research, please consider citing us:
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: multimodal_cci Version: 1.1.0 Summary: A Python
+Metadata-Version: 2.1 Name: multimodal_cci Version: 1.1.1 Summary: A Python
 package for processing multi-modal CCI data Home-page: https://github.com/
 BiomedicalMachineLearning/MultimodalCCI Author: Genomics and Machine Learning
 lab Author-email: l.hockey@uq.edu.au Project-URL: Bug Tracker, https://
 github.com/BiomedicalMachineLearning/MultimodalCCI/issues Project-URL:
 repository, https://github.com/BiomedicalMachineLearning/MultimodalCCI
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
+Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE.txt Requires-Dist: numpy>=1.24.0 Requires-Dist: pandas>=2.1.4 Requires-
 Dist: networkx>=3.2.1 Requires-Dist: matplotlib>=3.8.2 Requires-Dist: scikit-
 learn>=1.3.0 Requires-Dist: scipy>=1.9.1 Requires-Dist: tqdm>=4.66.1 Requires-
 Dist: gseapy>=1.1.1 Requires-Dist: scanpy>=1.9.0 Requires-Dist: seaborn>=0.11.2
 # MMCCI: Multimodal Cell-Cell Interaction Integrative Analysis of Single Cell
 and Spatial Data
                     PPaacckkaaggee _[_P_y_P_I_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _d_o_w_n_l_o_a_d_s_]
@@ -27,38 +27,37 @@
 issues raised by users. - There is a brain aging tutorial notebook [here]
 (examples/brain_aging_example.ipynb) - There is a melanoma tutorial notebook
 [here](examples/melanoma_example.ipynb) - To understand how to load CCI results
 from different tools, look at this notebook [here](examples/
 loading_CCI_results.ipynb) ## CCI Integration MMCCI allows users to integrate
 multiple CCI results together, both: 1. Samples from a single modality (eg.
 Visium) 2. Samples from multiple modalities (eg. Visium, Xenium and CosMX) !
-[Integration Method](docs/images/integration_method.png) ## CCI Analysis MMCCI
-provides multiple useful analyses that can be run on the integrated networks or
-from a single sample: 1. Network comparison between groups with permutation
-testing 2. CLustering of LR pairs with similar networks 3. Clustering of spots/
-cells with similar interaction scores 4. Sender-receiver LR querying 5. GSEA
-pathway analysis ![Downstream Analyses](docs/images/analyses.png) ### Pipeline
-Diagram ![MMCCI Pipeline](docs/images/pipeline.png) ## Citing MMCCI If you have
-used MMCCI in your research, please consider citing us: ``` Hockey, L., Mulay,
-O., Xiong, Z., Khosrotehrani, K., Nefzger, C. M., & Nguyen, Q. (2024). MMCCI:
-Multimodal Cell-Cell Interaction Integrative Analysis of Single Cell and
-Spatial Data. bioRxiv. doi:10.1101/2024.02.28.582639 ``` BSD License Copyright
-(c) 2024, Genomics and Machine Learning lab All rights reserved. Redistribution
-and use in source and binary forms, with or without modification, are permitted
-provided that the following conditions are met: * Redistributions of source
-code must retain the above copyright notice, this list of conditions and the
-following disclaimer. * Redistributions in binary form must reproduce the above
-copyright notice, this list of conditions and the following disclaimer in the
-documentation and/or other materials provided with the distribution. * Neither
-the name of the copyright holder nor the names of its contributors may be used
-to endorse or promote products derived from this software without specific
-prior written permission. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS
-AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT
-NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A
-PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
-CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
-EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT
-OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
-INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
-CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING
-IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY
-OF SUCH DAMAGE.
+[Integration and Analysis Method](docs/images/analyses_pipeline.png) ## CCI
+Analysis MMCCI provides multiple useful analyses that can be run on the
+integrated networks or from a single sample: 1. Network comparison between
+groups with permutation testing 2. CLustering of LR pairs with similar networks
+3. Clustering of spots/cells with similar interaction scores 4. Sender-receiver
+LR querying 5. GSEA pathway analysis ### Pipeline Diagram ![MMCCI Pipeline]
+(docs/images/pipeline.png) ## Citing MMCCI If you have used MMCCI in your
+research, please consider citing us: ``` Hockey, L., Mulay, O., Xiong, Z.,
+Khosrotehrani, K., Nefzger, C. M., & Nguyen, Q. (2024). MMCCI: Multimodal Cell-
+Cell Interaction Integrative Analysis of Single Cell and Spatial Data. bioRxiv.
+doi:10.1101/2024.02.28.582639 ``` BSD License Copyright (c) 2024, Genomics and
+Machine Learning lab All rights reserved. Redistribution and use in source and
+binary forms, with or without modification, are permitted provided that the
+following conditions are met: * Redistributions of source code must retain the
+above copyright notice, this list of conditions and the following disclaimer. *
+Redistributions in binary form must reproduce the above copyright notice, this
+list of conditions and the following disclaimer in the documentation and/or
+other materials provided with the distribution. * Neither the name of the
+copyright holder nor the names of its contributors may be used to endorse or
+promote products derived from this software without specific prior written
+permission. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
+"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE
+GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
+HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
+LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
+OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `multimodal_cci-1.1.0/src/multimodal_cci.egg-info/SOURCES.txt` & `multimodal_cci-1.1.1/src/multimodal_cci.egg-info/SOURCES.txt`

 * *Files identical despite different names*


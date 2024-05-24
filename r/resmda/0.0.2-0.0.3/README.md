# Comparing `tmp/resmda-0.0.2.tar.gz` & `tmp/resmda-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resmda-0.0.2.tar", last modified: Fri May 24 13:48:34 2024, max compression
+gzip compressed data, was "resmda-0.0.3.tar", last modified: Fri May 24 19:38:10 2024, max compression
```

## Comparing `resmda-0.0.2.tar` & `resmda-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:48:34.509767 resmda-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-24 13:48:28.000000 resmda-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-24 13:48:34.509767 resmda-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-24 13:48:28.000000 resmda-0.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:48:34.509767 resmda-0.0.2/resmda/
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-24 13:48:28.000000 resmda-0.0.2/resmda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-24 13:48:28.000000 resmda-0.0.2/resmda/data_assimilation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-05-24 13:48:28.000000 resmda-0.0.2/resmda/reservoir_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-24 13:48:28.000000 resmda-0.0.2/resmda/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-24 13:48:34.000000 resmda-0.0.2/resmda/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 13:48:34.509767 resmda-0.0.2/resmda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-24 13:48:34.000000 resmda-0.0.2/resmda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-24 13:48:34.000000 resmda-0.0.2/resmda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 13:48:34.000000 resmda-0.0.2/resmda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 13:48:34.000000 resmda-0.0.2/resmda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 13:48:34.000000 resmda-0.0.2/resmda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 13:48:34.509767 resmda-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-24 13:48:28.000000 resmda-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:38:10.435236 resmda-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-24 19:38:03.000000 resmda-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-24 19:38:10.435236 resmda-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-24 19:38:03.000000 resmda-0.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:38:10.435236 resmda-0.0.3/resmda/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-24 19:38:03.000000 resmda-0.0.3/resmda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-05-24 19:38:03.000000 resmda-0.0.3/resmda/data_assimilation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13810 2024-05-24 19:38:03.000000 resmda-0.0.3/resmda/reservoir_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-24 19:38:03.000000 resmda-0.0.3/resmda/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-24 19:38:10.000000 resmda-0.0.3/resmda/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:38:10.435236 resmda-0.0.3/resmda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-24 19:38:10.000000 resmda-0.0.3/resmda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-24 19:38:10.000000 resmda-0.0.3/resmda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 19:38:10.000000 resmda-0.0.3/resmda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-24 19:38:10.000000 resmda-0.0.3/resmda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 19:38:10.000000 resmda-0.0.3/resmda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 19:38:10.435236 resmda-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-24 19:38:03.000000 resmda-0.0.3/setup.py
```

### Comparing `resmda-0.0.2/LICENSE` & `resmda-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `resmda-0.0.2/PKG-INFO` & `resmda-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resmda
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple 2D reservoir modeller plus ESMDA.
 Home-page: https://github.com/tuda-geo/resmda
 Author: Dieter Werthmüller, Gabriel Serrao Seabra
 Author-email: info@emsig.xyz
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `resmda-0.0.2/README.rst` & `resmda-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `resmda-0.0.2/resmda/__init__.py` & `resmda-0.0.3/resmda/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
 # License for the specific language governing permissions and limitations under
 # the License.
 
 from resmda import utils
 from resmda.utils import Report
-from resmda.data_assimilation import esmda
+from resmda.data_assimilation import esmda, build_localization_matrix
 from resmda.reservoir_simulator import Simulator, RandomPermeability
 
 
 __all__ = ['reservoir_simulator', 'data_assimilation', 'utils',
-           'Simulator', 'RandomPermeability', 'esmda', 'Report']
+           'Simulator', 'RandomPermeability',
+           'esmda', 'build_localization_matrix',
+           'Report']
 
 __version__ = utils.__version__
```

### Comparing `resmda-0.0.2/resmda/utils.py` & `resmda-0.0.3/resmda/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,15 @@
           :func:`numpy.random.default_rng()`` instance, instantiated with
           ``int`` as seed.
         - If it is already a :class:`numpy.random.Generator` instance, it
           simply returns it.
 
 
     Returns
+    -------
     rng : random number generator
         A :class:`numpy.random.Generator` instance.
 
     """
     if isinstance(random, int):
         return np.random.default_rng(random)
     elif isinstance(random, np.random.Generator):
```

### Comparing `resmda-0.0.2/resmda.egg-info/PKG-INFO` & `resmda-0.0.3/resmda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resmda
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple 2D reservoir modeller plus ESMDA.
 Home-page: https://github.com/tuda-geo/resmda
 Author: Dieter Werthmüller, Gabriel Serrao Seabra
 Author-email: info@emsig.xyz
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `resmda-0.0.2/setup.py` & `resmda-0.0.3/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/litdata-0.2.6.tar.gz` & `tmp/litdata-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litdata-0.2.6.tar", last modified: Tue May  7 15:02:46 2024, max compression
+gzip compressed data, was "litdata-0.2.7.tar", last modified: Fri May 24 18:52:35 2024, max compression
```

## Comparing `litdata-0.2.6.tar` & `litdata-0.2.7.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:02:46.176143 litdata-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-07 15:02:36.000000 litdata-0.2.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-05-07 15:02:36.000000 litdata-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-07 15:02:36.000000 litdata-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20631 2024-05-07 15:02:46.176143 litdata-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18917 2024-05-07 15:02:36.000000 litdata-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 15:02:36.000000 litdata-0.2.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 15:02:46.176143 litdata-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-07 15:02:36.000000 litdata-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:02:46.168143 litdata-0.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:02:46.172143 litdata-0.2.6/src/litdata/
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/imports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:02:46.172143 litdata-0.2.6/src/litdata/processing/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42431 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/processing/data_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    17166 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/processing/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/processing/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/processing/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:02:46.176143 litdata-0.2.6/src/litdata/streaming/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/streaming/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/streaming/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9542 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/streaming/combined.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/streaming/compression.py
--rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/streaming/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    25796 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/streaming/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/streaming/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/streaming/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8731 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/streaming/item_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/streaming/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    12365 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/streaming/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     9749 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/streaming/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    14520 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/streaming/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/streaming/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (127)    18050 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/streaming/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:02:46.176143 litdata-0.2.6/src/litdata/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52973 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/utilities/_pytree.py
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/utilities/broadcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/utilities/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/utilities/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/utilities/packing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-07 15:02:36.000000 litdata-0.2.6/src/litdata/utilities/shuffle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:02:46.176143 litdata-0.2.6/src/litdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20631 2024-05-07 15:02:46.000000 litdata-0.2.6/src/litdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-07 15:02:46.000000 litdata-0.2.6/src/litdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 15:02:46.000000 litdata-0.2.6/src/litdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 15:02:46.000000 litdata-0.2.6/src/litdata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-07 15:02:46.000000 litdata-0.2.6/src/litdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 15:02:46.000000 litdata-0.2.6/src/litdata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:52:35.936136 litdata-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-24 18:52:27.000000 litdata-0.2.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-05-24 18:52:27.000000 litdata-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-24 18:52:27.000000 litdata-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20631 2024-05-24 18:52:35.936136 litdata-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18917 2024-05-24 18:52:27.000000 litdata-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-24 18:52:27.000000 litdata-0.2.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 18:52:35.936136 litdata-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-24 18:52:27.000000 litdata-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:52:35.928136 litdata-0.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:52:35.928136 litdata-0.2.7/src/litdata/
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:52:35.932136 litdata-0.2.7/src/litdata/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42431 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/processing/data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17166 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/processing/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/processing/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/processing/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:52:35.932136 litdata-0.2.7/src/litdata/streaming/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/combined.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8333 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26312 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20079 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8801 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/item_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12365 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9749 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14940 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18050 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/streaming/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:52:35.936136 litdata-0.2.7/src/litdata/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52973 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/utilities/_pytree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/utilities/broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/utilities/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/utilities/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/utilities/packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-05-24 18:52:27.000000 litdata-0.2.7/src/litdata/utilities/shuffle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 18:52:35.936136 litdata-0.2.7/src/litdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20631 2024-05-24 18:52:35.000000 litdata-0.2.7/src/litdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-24 18:52:35.000000 litdata-0.2.7/src/litdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 18:52:35.000000 litdata-0.2.7/src/litdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 18:52:35.000000 litdata-0.2.7/src/litdata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-24 18:52:35.000000 litdata-0.2.7/src/litdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-24 18:52:35.000000 litdata-0.2.7/src/litdata.egg-info/top_level.txt
```

### Comparing `litdata-0.2.6/LICENSE` & `litdata-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `litdata-0.2.6/MANIFEST.in` & `litdata-0.2.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `litdata-0.2.6/PKG-INFO` & `litdata-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litdata
-Version: 0.2.6
+Version: 0.2.7
 Summary: The Deep Learning framework to train, deploy, and ship AI products Lightning fast.
 Home-page: https://github.com/Lightning-AI/lit-data
 Download-URL: https://github.com/Lightning-AI/litdata
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/litdata/issues
```

### Comparing `litdata-0.2.6/README.md` & `litdata-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `litdata-0.2.6/setup.py` & `litdata-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.6/src/litdata/__about__.py` & `litdata-0.2.7/src/litdata/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import time
 
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 __author__ = "Lightning AI et al."
 __author_email__ = "pytorch@lightning.ai"
 __license__ = "Apache-2.0"
 __copyright__ = f"Copyright (c) 2023-{time.strftime('%Y')}, {__author__}."
 __homepage__ = "https://github.com/Lightning-AI/lit-data"
 __docs_url__ = "https://lightning.ai/docs/pytorch/stable/"
 # this has to be simple string, see: https://github.com/pypa/twine/issues/522
```

### Comparing `litdata-0.2.6/src/litdata/__init__.py` & `litdata-0.2.7/src/litdata/__init__.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.6/src/litdata/constants.py` & `litdata-0.2.7/src/litdata/constants.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.6/src/litdata/imports.py` & `litdata-0.2.7/src/litdata/imports.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.6/src/litdata/processing/__init__.py` & `litdata-0.2.7/src/litdata/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.6/src/litdata/processing/data_processor.py` & `litdata-0.2.7/src/litdata/processing/data_processor.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.6/src/litdata/processing/functions.py` & `litdata-0.2.7/src/litdata/processing/functions.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.6/src/litdata/processing/readers.py` & `litdata-0.2.7/src/litdata/processing/readers.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.6/src/litdata/processing/utilities.py` & `litdata-0.2.7/src/litdata/processing/utilities.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.6/src/litdata/streaming/__init__.py` & `litdata-0.2.7/src/litdata/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.6/src/litdata/streaming/cache.py` & `litdata-0.2.7/src/litdata/streaming/cache.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.6/src/litdata/streaming/client.py` & `litdata-0.2.7/src/litdata/streaming/client.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.6/src/litdata/streaming/combined.py` & `litdata-0.2.7/src/litdata/streaming/combined.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,23 +76,35 @@
         else:
             self._weights = [w / sum(weights) for w in weights]
 
         self._iterator: Optional[_CombinedDatasetIterator] = None
         self._use_streaming_dataloader = False
         self._num_samples_yielded: Optional[List[int]] = None
         self._current_epoch = 0
+        self.num_workers = 1
+        self.batch_size = 1
 
-    def __len__(self) -> Optional[int]:
+    def get_len(self, num_workers: int, batch_size: int) -> Optional[int]:
+        self.num_workers = num_workers
+        self.batch_size = batch_size
         if self._iterate_over_all:
             return self._get_total_length()
         return None
 
+    def __len__(self) -> Optional[int]:
+        return self.get_len(1, 1)
+
     # total length of the datasets
     def _get_total_length(self) -> int:
-        return sum(len(d) for d in self._datasets)
+        return sum(self._get_len(d) for d in self._datasets)
+
+    def _get_len(self, d: Any) -> int:
+        if isinstance(d, StreamingDataset):
+            return d.get_len(self.num_workers, self.batch_size)
+        return len(d)
 
     def set_epoch(self, current_epoch: int) -> None:
         """Set the current epoch to the datasets on epoch starts.
 
         When using the StreamingDataLoader, this is done automatically
 
         """
```

### Comparing `litdata-0.2.6/src/litdata/streaming/compression.py` & `litdata-0.2.7/src/litdata/streaming/compression.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.6/src/litdata/streaming/config.py` & `litdata-0.2.7/src/litdata/streaming/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -67,14 +67,29 @@
 
         self._compressor_name = self._config["compression"]
         self._compressor: Optional[Compressor] = None
 
         if self._compressor_name in _COMPRESSORS:
             self._compressor = _COMPRESSORS[self._compressor_name]
 
+        self._skip_chunk_indexes_deletion: Optional[List[int]] = None
+
+    def can_delete(self, chunk_index: int) -> bool:
+        if self._skip_chunk_indexes_deletion is None:
+            return True
+        return chunk_index not in self._skip_chunk_indexes_deletion
+
+    @property
+    def skip_chunk_indexes_deletion(self) -> Optional[List[int]]:
+        return self._skip_chunk_indexes_deletion
+
+    @skip_chunk_indexes_deletion.setter
+    def skip_chunk_indexes_deletion(self, skip_chunk_indexes_deletion: List[int]) -> None:
+        self._skip_chunk_indexes_deletion = skip_chunk_indexes_deletion
+
     def download_chunk_from_index(self, chunk_index: int) -> None:
         chunk_filename = self._chunks[chunk_index]["filename"]
 
         local_chunkpath = os.path.join(self._cache_dir, chunk_filename)
 
         if os.path.exists(local_chunkpath):
             self.try_decompress(local_chunkpath)
```

### Comparing `litdata-0.2.6/src/litdata/streaming/dataloader.py` & `litdata-0.2.7/src/litdata/streaming/dataloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -611,14 +611,24 @@
 
                     yield batch[__SAMPLES_KEY__]
                 else:
                     yield batch
 
         self.restore = False
 
+    def __len__(self) -> int:
+        if self._dataset_kind == _DatasetKind.Iterable:
+            length = self._IterableDataset_len_called = self.dataset.get_len(self.num_workers, self.batch_size)
+            if self.batch_size is not None:  # IterableDataset doesn't allow custom sampler or batch_sampler
+                from math import ceil
+
+                return length // self.batch_size if self.drop_last else ceil(length / self.batch_size)
+            return length
+        return len(self._index_sampler)
+
     def state_dict(self) -> Dict[str, Any]:
         if isinstance(self.dataset, StreamingDataset):
             assert self.batch_size
             return {
                 "dataset": self.dataset.state_dict(
                     self._num_samples_yielded_streaming, self.num_workers, self.batch_size
                 ),
```

### Comparing `litdata-0.2.6/src/litdata/streaming/dataset.py` & `litdata-0.2.7/src/litdata/streaming/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from litdata.streaming import Cache
 from litdata.streaming.item_loader import BaseItemLoader
 from litdata.streaming.resolver import Dir, _resolve_dir
 from litdata.streaming.sampler import ChunkedIndex
 from litdata.streaming.serializers import Serializer
 from litdata.streaming.shuffle import FullShuffle, NoShuffle, Shuffle
 from litdata.utilities.env import _DistributedEnv, _is_in_dataloader_worker, _WorkerEnv
+from litdata.utilities.shuffle import _find_chunks_per_ranks_on_which_to_skip_deletion
 
 logger = Logger(__name__)
 
 
 class StreamingDataset(IterableDataset):
     """The streaming dataset can be used once your data have been optimised using the DatasetOptimiser class."""
 
@@ -102,14 +103,16 @@
         self.has_triggered_download = False
         self.min_items_per_replica: Optional[int] = None
         self.current_epoch = 1
         self.random_state = None
         self.shuffler: Optional[Shuffle] = None
         self.serializers = serializers
         self._state_dict: Optional[Dict[str, Any]] = None
+        self.num_workers: Optional[int] = None
+        self.batch_size: Optional[int] = None
 
     def set_shuffle(self, shuffle: bool) -> None:
         self.shuffle = shuffle
 
     def set_epoch(self, current_epoch: int) -> None:
         """Set the current epoch to the dataset on epoch starts.
 
@@ -152,18 +155,24 @@
         if self._state_dict is not None:
             state: Dict[str, Any] = self._state_dict
             seed = state["seed"]
             drop_last = state["drop_last"]
         return FullShuffle(cache, seed, drop_last) if self.shuffle else NoShuffle(cache, seed, drop_last)
 
     def __len__(self) -> int:
+        return self.get_len(1, 1)
+
+    def get_len(self, num_workers: int, batch_size: int) -> int:
+        self.num_workers = num_workers
+        self.batch_size = batch_size
+        worker_env = _WorkerEnv.detect()
         if self.shuffler is None:
-            cache = self._create_cache(worker_env=_WorkerEnv.detect())
+            cache = self._create_cache(worker_env=worker_env)
             self.shuffler = self._create_shuffler(cache)
-        return self.shuffler.get_len(self.distributed_env, self.current_epoch)
+        return self.shuffler.get_len(self.distributed_env, num_workers, batch_size, self.current_epoch)
 
     def __iter__(self) -> "StreamingDataset":
         # When the StreamingDataset is used within map or optimize, let's refetch the distributed env.
         if os.getenv("DATA_OPTIMIZER_GLOBAL_RANK"):
             self.distributed_env = _DistributedEnv.detect()
 
         self.worker_env = _WorkerEnv.detect()
@@ -173,42 +182,44 @@
         # Handle restart
         if self._state_dict:
             self._validate_state_dict()
             state: Dict[str, Any] = self._state_dict
             self.current_epoch = state["current_epoch"]
 
         chunks_per_replica, intervals_per_replica = self.shuffler.get_chunks_and_intervals_per_ranks(
-            self.distributed_env, self.current_epoch
+            self.distributed_env, self.worker_env.world_size, self.batch_size or 1, self.current_epoch
         )
         chunks_replica = chunks_per_replica[self.distributed_env.global_rank % self.distributed_env.world_size]
         intervals_replica = intervals_per_replica[self.distributed_env.global_rank % self.distributed_env.world_size]
 
         # Handle restart
         if self._state_dict:
             self._resume(chunks_replica, intervals_replica)
         else:
-            chunks_per_replica, intervals_per_replica = self.shuffler.get_chunks_and_intervals_per_ranks(
-                self.distributed_env, self.current_epoch
+            # Find the chunks shared across multiple ranks.
+            # For each shared chunk, find the rank to use the chunk last and prevent deletion
+            # for the other ranks.
+            chunks_indexes_skip_deletion = _find_chunks_per_ranks_on_which_to_skip_deletion(
+                self.worker_env.world_size, chunks_per_replica, intervals_per_replica
+            )
+            if self.distributed_env.global_rank in chunks_indexes_skip_deletion:
+                self.cache._reader.config.skip_chunk_indexes_deletion = chunks_indexes_skip_deletion[
+                    self.distributed_env.global_rank
+                ]
+
+            workers_chunks, workers_intervals = _associate_chunks_to_workers(
+                self.worker_env,
+                chunks_per_replica[self.distributed_env.global_rank],
+                intervals_per_replica[self.distributed_env.global_rank],
             )
-            chunks_replica = chunks_per_replica[self.distributed_env.global_rank % self.distributed_env.world_size]
-            intervals_replica = intervals_per_replica[
-                self.distributed_env.global_rank % self.distributed_env.world_size
-            ]
-
-            self.worker_chunks = []
-            self.worker_intervals = []
-
-            for i, (chunk_index, chunk_interval) in enumerate(zip(chunks_replica, intervals_replica)):
-                if i % self.worker_env.world_size != self.worker_env.rank:
-                    continue
-                self.worker_chunks.append(chunk_index)
-                self.worker_intervals.append(chunk_interval)
 
-            self.num_chunks = len(self.worker_chunks)
+            self.worker_chunks = workers_chunks[self.worker_env.rank]
+            self.worker_intervals = workers_intervals[self.worker_env.rank]
 
+            self.num_chunks = len(self.worker_chunks)
             self.current_indexes = []
             self.chunk_index = 0
             self.global_index = 0
             self.index = 0
 
         self.has_triggered_download = False
         self.last_time = time()
@@ -226,15 +237,15 @@
         batch_size = state["batch_size"]
 
         # TODO: Implement elastic sampling where the number of workers, ranks can change.
         num_samples_yielded = self._state_dict["num_samples_yielded"]
 
         # replay sampling from each worker / chunks using the batch size
         workers_chunks, workers_intervals = _associate_chunks_to_workers(
-            num_workers, self.worker_env, chunks_replica, intervals_replica
+            self.worker_env, chunks_replica, intervals_replica
         )
         indexes = _replay_sampling(num_samples_yielded, batch_size, num_workers)
         chunks_index, indexes = _replay_chunks_sampling(workers_intervals, indexes)
 
         # select the chunks and intervals associated to this worker
         worker_rank = self.worker_env.rank
         self.num_chunks = len(workers_intervals[worker_rank])
@@ -423,20 +434,20 @@
         int(value)
         return True
     except Exception:
         return False
 
 
 def _associate_chunks_to_workers(
-    num_workers: int, worker_env: _WorkerEnv, chunks_replica: List[int], intervals_replica: List[Any]
+    worker_env: _WorkerEnv, chunks_replica: List[int], intervals_replica: List[Any]
 ) -> Any:
     workers_chunks = {}
     workers_intervals = {}
 
-    for worker_idx in range(num_workers):
+    for worker_idx in range(worker_env.world_size):
         worker_chunks = []
         worker_intervals = []
         for i, (chunk_index, chunk_interval) in enumerate(zip(chunks_replica, intervals_replica)):
             if i % worker_env.world_size != worker_idx:
                 continue
 
             worker_chunks.append(chunk_index)
```

### Comparing `litdata-0.2.6/src/litdata/streaming/downloader.py` & `litdata-0.2.7/src/litdata/streaming/downloader.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.6/src/litdata/streaming/item_loader.py` & `litdata-0.2.7/src/litdata/streaming/item_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import functools
 import os
 from abc import ABC, abstractmethod
+from copy import deepcopy
 from time import sleep
 from typing import Any, Dict, List, Optional, Tuple
 
 import numpy as np
 import torch
 
 from litdata.constants import (
@@ -29,22 +30,23 @@
 
 class BaseItemLoader(ABC):
     """The base item loader is responsible to decide how the items within a chunk are loaded."""
 
     def setup(self, config: Dict, chunks: List, serializers: Dict[str, Serializer]) -> None:
         self._config = config
         self._chunks = chunks
-        self._serializers = serializers
+        self._serializers = {**serializers}
         self._data_format = self._config["data_format"]
         self._shift_idx = len(self._data_format) * 4
 
         # setup the serializers on restart
         for data_format in self._data_format:
-            serializer = self._serializers[self._data_format_to_key(data_format)]
+            serializer = deepcopy(self._serializers[self._data_format_to_key(data_format)])
             serializer.setup(data_format)
+            self._serializers[data_format] = serializer
 
     @functools.lru_cache(maxsize=128)
     def _data_format_to_key(self, data_format: str) -> str:
         if ":" in data_format:
             serialier, serializer_sub_type = data_format.split(":")
             if serializer_sub_type in self._serializers:
                 return serializer_sub_type
@@ -124,15 +126,15 @@
 
     def deserialize(self, raw_item_data: bytes) -> "PyTree":
         """Deserialize the raw bytes into their python equivalent."""
         idx = self._shift_idx
         sizes = np.frombuffer(raw_item_data[:idx], np.uint32)
         data = []
         for size, data_format in zip(sizes, self._data_format):
-            serializer = self._serializers[self._data_format_to_key(data_format)]
+            serializer = self._serializers[data_format]
             data_bytes = raw_item_data[idx : idx + size]
             data.append(serializer.deserialize(data_bytes))
             idx += size
         return tree_unflatten(data, self._config["data_spec"])
 
     def delete(self, chunk_index: int, chunk_filepath: str) -> None:
         if os.path.exists(chunk_filepath):
```

### Comparing `litdata-0.2.6/src/litdata/streaming/reader.py` & `litdata-0.2.7/src/litdata/streaming/reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import contextlib
-import multiprocessing
 import os
 import warnings
 from logging import Logger
-from queue import Empty
-from threading import Thread
+from queue import Empty, Queue
+from threading import Event, Thread
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from litdata.constants import _TORCH_GREATER_EQUAL_2_1_0
 from litdata.streaming.config import ChunksConfig
 from litdata.streaming.item_loader import BaseItemLoader, PyTreeLoader
 from litdata.streaming.sampler import ChunkedIndex
 from litdata.streaming.serializers import Serializer, _get_serializers
@@ -61,16 +60,17 @@
         self._max_pre_download = max_pre_download
         self._pre_download_counter = 0
         self._distributed_env = distributed_env
 
         self._chunks_index_to_be_deleted: List[int] = []
         self._max_cache_size = max_cache_size
         self._parent_cache_dir = os.path.dirname(self._config._cache_dir)
-        self._to_download_queue: multiprocessing.Queue = multiprocessing.Queue()
-        self._to_delete_queue: multiprocessing.Queue = multiprocessing.Queue()
+        self._to_download_queue: Queue = Queue()
+        self._to_delete_queue: Queue = Queue()
+        self._force_stop_event = Event()
 
         # Check whether a dataset slice fits on the node
         num_bytes_per_nodes = self._config.num_bytes // self._distributed_env.num_nodes
         self._delete_chunks_when_processed = num_bytes_per_nodes > max_cache_size if max_cache_size else False
         self._has_exited = False
 
     def download(self, chunk_indexes: List[int]) -> None:
@@ -81,21 +81,29 @@
     def delete(self, chunk_indexes: List[int]) -> None:
         """Receive the list of the chunk indices to delete for the current epoch."""
         for chunk_index in chunk_indexes:
             self._to_delete_queue.put(chunk_index)
 
     def _delete(self, chunk_index: int) -> None:
         """Inform the item loader of the chunk to delete."""
-        chunk_filepath, _, _ = self._config[ChunkedIndex(index=-1, chunk_index=chunk_index)]
-        self._item_loader.delete(chunk_index, chunk_filepath)
+        if self._config.can_delete(chunk_index):
+            chunk_filepath, _, _ = self._config[ChunkedIndex(index=-1, chunk_index=chunk_index)]
+            self._item_loader.delete(chunk_index, chunk_filepath)
+
+            locak_chunk_path = chunk_filepath + ".lock"
+            if os.path.exists(locak_chunk_path):
+                os.remove(locak_chunk_path)
 
     def stop(self) -> None:
         """Receive the list of the chunk indices to download for the current epoch."""
         self._to_download_queue.put(_END_TOKEN)
 
+    def force_stop(self) -> None:
+        self._force_stop_event.set()
+
     def _maybe_delete_chunks(self) -> None:
         reached_pre_download = self._pre_download_counter == self._max_pre_download
 
         # we have already pre-downloaded some chunks, we just need to wait for them to be processed.
         chunk_index = _get_from_queue(
             self._to_delete_queue, timeout=_LONG_DEFAULT_TIMEOUT if reached_pre_download else _DEFAULT_TIMEOUT
         )
@@ -120,14 +128,17 @@
 
     def _pre_load_chunk(self, chunk_index: int) -> None:
         chunk_filepath, _, _ = self._config[ChunkedIndex(index=-1, chunk_index=chunk_index)]
         self._item_loader.pre_load_chunk(chunk_index, chunk_filepath)
 
     def run(self) -> None:
         while True:
+            if self._force_stop_event.is_set():
+                self._has_exited = True
+                return
             if self._pre_download_counter < self._max_pre_download:
                 chunk_index = _get_from_queue(self._to_download_queue)
                 if chunk_index == _END_TOKEN:
                     self._has_exited = True
                     return
 
                 if chunk_index is not None:
@@ -251,15 +262,19 @@
         chunk_filepath, begin, chunk_bytes = self.config[index]
         item = self._item_loader.load_item_from_chunk(
             index.index, index.chunk_index, chunk_filepath, begin, chunk_bytes
         )
 
         # We need to request deletion after the latest element has been loaded.
         # Otherwise, this could trigger segmentation fault error depending on the item loader used.
-        if self._config and self._config._remote_dir and index.chunk_index != self._last_chunk_index:
+        if (
+            self._config
+            and (self._config._remote_dir or self._config._compressor)
+            and index.chunk_index != self._last_chunk_index
+        ):
             assert self._prepare_thread
             assert self._last_chunk_index is not None
 
             # inform the chunk has been completely consumed
             self._prepare_thread.delete([self._last_chunk_index])
 
             # track the new chunk index as the latest one
@@ -287,14 +302,19 @@
         return self.config.intervals
 
     def __getstate__(self) -> Dict[str, Any]:
         state = self.__dict__.copy()
         state["_prepare_thread"] = None
         return state
 
+    def __del__(self) -> None:
+        if self._prepare_thread and not self._prepare_thread._has_exited:
+            self._prepare_thread.force_stop()
+            self._prepare_thread = None
+
 
 def _get_folder_size(path: str) -> int:
     """Collect the size of each files within a folder.
 
     This method is robust to file deletion races
 
     """
@@ -302,15 +322,15 @@
     for dirpath, _, filenames in os.walk(str(path)):
         for filename in filenames:
             with contextlib.suppress(FileNotFoundError):
                 size += os.stat(os.path.join(dirpath, filename)).st_size
     return size
 
 
-def _get_from_queue(queue: multiprocessing.Queue, timeout: float = _DEFAULT_TIMEOUT) -> Optional[Any]:
+def _get_from_queue(queue: Queue, timeout: float = _DEFAULT_TIMEOUT) -> Optional[Any]:
     try:
         return queue.get(timeout=timeout)
     except Empty:
         pass
     except OSError as err:
         # handle closed queue before the thread terminates
         if "handle is closed" in str(err) or "Bad file descriptor" in str(err):
```

### Comparing `litdata-0.2.6/src/litdata/streaming/resolver.py` & `litdata-0.2.7/src/litdata/streaming/resolver.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.6/src/litdata/streaming/sampler.py` & `litdata-0.2.7/src/litdata/streaming/sampler.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.6/src/litdata/streaming/serializers.py` & `litdata-0.2.7/src/litdata/streaming/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 import io
 import os
 import pickle
 import tempfile
 from abc import ABC, abstractmethod
 from collections import OrderedDict
+from copy import deepcopy
 from typing import Any, Dict, Optional, Tuple, Union
 
 import numpy as np
 import torch
 
 from litdata.constants import _NUMPY_DTYPES_MAPPING, _TORCH_DTYPES_MAPPING
 from litdata.imports import RequirementCache
@@ -179,15 +180,21 @@
     def deserialize(self, data: bytes) -> torch.Tensor:
         dtype_indice = np.frombuffer(data[0:4], np.uint32).item()
         dtype = _TORCH_DTYPES_MAPPING[dtype_indice]
         shape_size = np.frombuffer(data[4:8], np.uint32).item()
         shape = []
         for shape_idx in range(shape_size):
             shape.append(np.frombuffer(data[8 + 4 * shape_idx : 8 + 4 * (shape_idx + 1)], np.uint32).item())
-        tensor = torch.frombuffer(data[8 + 4 * (shape_idx + 1) : len(data)], dtype=dtype)
+        idx_start = 8 + 4 * (shape_idx + 1)
+        idx_end = len(data)
+        if idx_end > idx_start:
+            tensor = torch.frombuffer(data[idx_start:idx_end], dtype=dtype)
+        else:
+            assert idx_start == idx_end, "The starting index should never be greater than end ending index."
+            tensor = torch.empty(shape, dtype=dtype)
         shape = torch.Size(shape)
         if tensor.shape == shape:
             return tensor
         return torch.reshape(tensor, shape)
 
     def can_serialize(self, item: torch.Tensor) -> bool:
         return isinstance(item, torch.Tensor) and type(item) == torch.Tensor and len(item.shape) > 1
@@ -206,15 +213,15 @@
 
     def serialize(self, item: torch.Tensor) -> Tuple[bytes, Optional[str]]:
         dtype_indice = self._dtype_to_indices[item.dtype]
         return item.numpy().tobytes(order="C"), f"no_header_tensor:{dtype_indice}"
 
     def deserialize(self, data: bytes) -> torch.Tensor:
         assert self._dtype
-        return torch.frombuffer(data, dtype=self._dtype)
+        return torch.frombuffer(data, dtype=self._dtype) if len(data) > 0 else torch.empty((0,), dtype=self._dtype)
 
     def can_serialize(self, item: torch.Tensor) -> bool:
         return isinstance(item, torch.Tensor) and type(item) == torch.Tensor and len(item.shape) == 1
 
 
 class NumpySerializer(Serializer):
     """The NumpySerializer serialize and deserialize numpy to and from bytes."""
@@ -390,13 +397,16 @@
         "tensor": TensorSerializer(),
         "pickle": PickleSerializer(),
     }
 )
 
 
 def _get_serializers(serializers: Optional[Dict[str, Serializer]]) -> Dict[str, Serializer]:
-    if serializers:
-        serializers = OrderedDict(**serializers)
-        serializers.update(_SERIALIZERS)
-    else:
-        serializers = _SERIALIZERS
+    if serializers is None:
+        serializers = {}
+    serializers = OrderedDict(serializers)
+
+    for key, value in _SERIALIZERS.items():
+        if key not in serializers:
+            serializers[key] = deepcopy(value)
+
     return serializers
```

### Comparing `litdata-0.2.6/src/litdata/streaming/shuffle.py` & `litdata-0.2.7/src/litdata/streaming/shuffle.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,50 +27,56 @@
 
     def __init__(self, cache: Cache, seed: int, drop_last: bool):
         self.cache = cache
         self.seed = seed
         self.drop_last = drop_last
 
     @lru_cache(maxsize=10)
-    def get_len(self, distributed_env: _DistributedEnv, current_epoch: int) -> int:
-        _, intervals_per_ranks = self.get_chunks_and_intervals_per_ranks(distributed_env, current_epoch)
+    def get_len(self, distributed_env: _DistributedEnv, num_workers: int, batch_size: int, current_epoch: int) -> int:
+        _, intervals_per_ranks = self.get_chunks_and_intervals_per_ranks(
+            distributed_env, num_workers, batch_size, current_epoch
+        )
 
         if self.drop_last:
             items_per_process = [
                 sum((interval[-1] - interval[0]) for interval in intervals) for intervals in intervals_per_ranks
             ]
             # Validate each processes gets the exact number of elements
             if len(items_per_process) > 1:
                 assert all(items_per_process[0] == items_to_process for items_to_process in items_per_process[:1])
             return items_per_process[0]
 
         return sum((interval[-1] - interval[0]) for interval in intervals_per_ranks[distributed_env.global_rank])
 
     @abstractmethod
-    def get_chunks_and_intervals_per_ranks(self, distributed_env: _DistributedEnv, current_epoch: int) -> Any:
+    def get_chunks_and_intervals_per_ranks(
+        self, distributed_env: _DistributedEnv, num_workers: int, batch_size: int, current_epoch: int
+    ) -> Any:
         pass
 
     @abstractmethod
     def __call__(self, array: np.ndarray, num_chunks: int, current_epoch: int, chunk_index: int) -> List[int]:
         pass
 
 
 class NoShuffle(Shuffle):
     """NoShuffle doesn't shuffle the items and ensure all the processes receive the same number of items if drop_last
     is True."""
 
     @lru_cache(maxsize=10)
-    def get_chunks_and_intervals_per_ranks(self, distributed_env: _DistributedEnv, current_epoch: int) -> Any:
+    def get_chunks_and_intervals_per_ranks(
+        self, distributed_env: _DistributedEnv, num_workers: int, batch_size: int, current_epoch: int
+    ) -> Any:
         # 1. Get the intervals
         chunk_intervals = self.cache.get_chunk_intervals()
         indexes = range(len(chunk_intervals))
 
         # 2. Compute the items budget of each rank
         chunks_per_ranks, intervals_per_ranks = _associate_chunks_and_internals_to_ranks(
-            distributed_env, indexes, chunk_intervals, self.drop_last
+            distributed_env, indexes, chunk_intervals, self.drop_last, num_workers, batch_size
         )
 
         return chunks_per_ranks, intervals_per_ranks
 
     def __call__(self, array: np.ndarray, num_chunks: int, current_epoch: int, chunk_index: int) -> List[int]:
         return array.tolist()
 
@@ -90,15 +96,17 @@
 
     As a result, we lose at most (number of ranks) items. However, as some chunks are shared across ranks. This leads to
     the same chunk to be downloaded multiple times.
 
     """
 
     @lru_cache(maxsize=10)
-    def get_chunks_and_intervals_per_ranks(self, distributed_env: _DistributedEnv, current_epoch: int) -> Any:
+    def get_chunks_and_intervals_per_ranks(
+        self, distributed_env: _DistributedEnv, num_workers: int, batch_size: int, current_epoch: int
+    ) -> Any:
         # 1. Get the intervals
         chunk_intervals = self.cache.get_chunk_intervals()
 
         # 2. Shuffle them
         indexes = range(len(chunk_intervals))
 
         # If we have multiple nodes, the seed_shift is constant here.
@@ -109,27 +117,27 @@
         # This is done slighyly down this function.
         seed_shift = 1 if distributed_env.num_nodes > 1 else current_epoch
         shuffled_indexes = np.random.RandomState(seed=self.seed + seed_shift).permutation(indexes)
         shuffled_chunk_intervals = np.asarray(chunk_intervals)[shuffled_indexes].tolist()
 
         # 3. Compute the items budget of each rank
         chunks_per_ranks, intervals_per_ranks = _associate_chunks_and_internals_to_ranks(
-            distributed_env, shuffled_indexes, shuffled_chunk_intervals, self.drop_last
+            distributed_env, shuffled_indexes, shuffled_chunk_intervals, self.drop_last, num_workers, batch_size
         )
 
         # For the first epoch, no need of further shuffling
         if current_epoch == 1 or distributed_env.num_nodes == 1:
             return chunks_per_ranks, intervals_per_ranks
 
         # Perform shuffle within the nodes to avoid cache miss.
         # Note: It is possible for the overlapping chunks to change due to the changing order.
         shuffled_indexes = _intra_node_chunk_shuffle(distributed_env, chunks_per_ranks, self.seed, current_epoch)
         shuffled_chunk_intervals = np.asarray(chunk_intervals)[shuffled_indexes].tolist()
 
         chunks_per_ranks, intervals_per_ranks = _associate_chunks_and_internals_to_ranks(
-            distributed_env, shuffled_indexes, shuffled_chunk_intervals, self.drop_last
+            distributed_env, shuffled_indexes, shuffled_chunk_intervals, self.drop_last, num_workers, batch_size
         )
 
         return chunks_per_ranks, intervals_per_ranks
 
     def __call__(self, array: np.ndarray, num_chunks: int, current_epoch: int, chunk_index: int) -> List[int]:
         return np.random.RandomState([self.seed, num_chunks * current_epoch, chunk_index]).permutation(array).tolist()
```

### Comparing `litdata-0.2.6/src/litdata/streaming/writer.py` & `litdata-0.2.7/src/litdata/streaming/writer.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.6/src/litdata/utilities/__init__.py` & `litdata-0.2.7/src/litdata/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.6/src/litdata/utilities/_pytree.py` & `litdata-0.2.7/src/litdata/utilities/_pytree.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.6/src/litdata/utilities/broadcast.py` & `litdata-0.2.7/src/litdata/utilities/broadcast.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.6/src/litdata/utilities/env.py` & `litdata-0.2.7/src/litdata/utilities/env.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,18 @@
             world_size = None
             global_rank = 0
             num_nodes = 1
 
         if world_size is None or world_size == -1:
             world_size = 1
 
+        world_size = int(os.environ.get("WORLD_SIZE", world_size))
+        global_rank = int(os.environ.get("GLOBAL_RANK", global_rank))
+        num_nodes = int(os.environ.get("NNODES", num_nodes))
+
         return cls(world_size=world_size, global_rank=global_rank, num_nodes=num_nodes)
 
     @classmethod
     def _instantiate_in_map_or_optimize(cls) -> "_DistributedEnv":
         global_rank = int(os.getenv("DATA_OPTIMIZER_GLOBAL_RANK", "0"))
         num_workers = int(os.getenv("DATA_OPTIMIZER_NUM_WORKERS", "0"))
         num_nodes = int(os.getenv("DATA_OPTIMIZER_NUM_NODES", 1))
```

### Comparing `litdata-0.2.6/src/litdata/utilities/format.py` & `litdata-0.2.7/src/litdata/utilities/format.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.6/src/litdata/utilities/packing.py` & `litdata-0.2.7/src/litdata/utilities/packing.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.6/src/litdata.egg-info/PKG-INFO` & `litdata-0.2.7/src/litdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litdata
-Version: 0.2.6
+Version: 0.2.7
 Summary: The Deep Learning framework to train, deploy, and ship AI products Lightning fast.
 Home-page: https://github.com/Lightning-AI/lit-data
 Download-URL: https://github.com/Lightning-AI/litdata
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/litdata/issues
```

### Comparing `litdata-0.2.6/src/litdata.egg-info/SOURCES.txt` & `litdata-0.2.7/src/litdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*


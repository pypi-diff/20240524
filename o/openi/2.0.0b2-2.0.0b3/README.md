# Comparing `tmp/openi-2.0.0b2.tar.gz` & `tmp/openi-2.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openi-2.0.0b2.tar", last modified: Thu May 23 06:51:20 2024, max compression
+gzip compressed data, was "openi-2.0.0b3.tar", last modified: Fri May 24 07:41:32 2024, max compression
```

## Comparing `openi-2.0.0b2.tar` & `openi-2.0.0b3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 06:51:20.753149 openi-2.0.0b2/
--rw-rw-rw-   0        0        0     2126 2024-05-23 06:51:20.751138 openi-2.0.0b2/PKG-INFO
--rw-rw-rw-   0        0        0     1491 2024-05-22 02:56:56.000000 openi-2.0.0b2/README.md
--rw-rw-rw-   0        0        0       80 2024-05-20 06:59:24.000000 openi-2.0.0b2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-23 06:51:20.753149 openi-2.0.0b2/setup.cfg
--rw-rw-rw-   0        0        0     1016 2024-05-23 06:47:17.000000 openi-2.0.0b2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 06:51:20.695720 openi-2.0.0b2/src/
-drwxrwxrwx   0        0        0        0 2024-05-23 06:51:20.725884 openi-2.0.0b2/src/openi/
--rw-rw-rw-   0        0        0      214 2024-05-20 06:59:24.000000 openi-2.0.0b2/src/openi/__init__.py
--rw-rw-rw-   0        0        0    11006 2024-05-23 03:12:22.000000 openi-2.0.0b2/src/openi/_dataclass.py
--rw-rw-rw-   0        0        0     7895 2024-05-23 04:00:55.000000 openi-2.0.0b2/src/openi/_exceptions.py
--rw-rw-rw-   0        0        0     7127 2024-05-22 07:30:55.000000 openi-2.0.0b2/src/openi/_file.py
--rw-rw-rw-   0        0        0     4576 2024-05-23 03:19:45.000000 openi-2.0.0b2/src/openi/_login.py
--rw-rw-rw-   0        0        0     9663 2024-05-22 03:00:39.000000 openi-2.0.0b2/src/openi/_session.py
--rw-rw-rw-   0        0        0     4120 2024-05-20 06:59:24.000000 openi-2.0.0b2/src/openi/_tqdm.py
--rw-rw-rw-   0        0        0    36678 2024-05-23 03:19:56.000000 openi-2.0.0b2/src/openi/api.py
-drwxrwxrwx   0        0        0        0 2024-05-23 06:51:20.743909 openi-2.0.0b2/src/openi/commands/
--rw-rw-rw-   0        0        0      328 2024-05-20 06:59:24.000000 openi-2.0.0b2/src/openi/commands/__init__.py
--rw-rw-rw-   0        0        0     6802 2024-05-23 03:19:57.000000 openi-2.0.0b2/src/openi/commands/dataset.py
--rw-rw-rw-   0        0        0     8628 2024-05-23 03:19:57.000000 openi-2.0.0b2/src/openi/commands/model.py
--rw-rw-rw-   0        0        0      897 2024-05-20 06:59:24.000000 openi-2.0.0b2/src/openi/commands/openi_cli.py
--rw-rw-rw-   0        0        0     2562 2024-05-23 02:22:22.000000 openi-2.0.0b2/src/openi/commands/user.py
--rw-rw-rw-   0        0        0     2111 2024-05-20 06:59:24.000000 openi-2.0.0b2/src/openi/constants.py
--rw-rw-rw-   0        0        0    10840 2024-05-23 03:19:56.000000 openi-2.0.0b2/src/openi/downloader.py
--rw-rw-rw-   0        0        0     3780 2024-05-20 06:59:24.000000 openi-2.0.0b2/src/openi/log.py
--rw-rw-rw-   0        0        0     9731 2024-05-23 06:51:20.000000 openi-2.0.0b2/src/openi/uploader.py
--rw-rw-rw-   0        0        0     2775 2024-05-20 06:59:24.000000 openi-2.0.0b2/src/openi/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 06:51:20.749653 openi-2.0.0b2/src/openi.egg-info/
--rw-rw-rw-   0        0        0     2126 2024-05-23 06:51:20.000000 openi-2.0.0b2/src/openi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      686 2024-05-23 06:51:20.000000 openi-2.0.0b2/src/openi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 06:51:20.000000 openi-2.0.0b2/src/openi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-05-23 06:51:20.000000 openi-2.0.0b2/src/openi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2024-05-23 06:51:20.000000 openi-2.0.0b2/src/openi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-23 06:51:20.000000 openi-2.0.0b2/src/openi.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-23 06:51:20.746944 openi-2.0.0b2/test/
--rw-rw-rw-   0        0        0     1149 2024-04-29 07:10:45.000000 openi-2.0.0b2/test/test.py
--rw-rw-rw-   0        0        0      179 2024-05-23 03:08:38.000000 openi-2.0.0b2/test/test_openi.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:41:32.599674 openi-2.0.0b3/
+-rw-rw-rw-   0        0        0     2126 2024-05-24 07:41:32.597674 openi-2.0.0b3/PKG-INFO
+-rw-rw-rw-   0        0        0     1491 2024-05-22 02:56:56.000000 openi-2.0.0b3/README.md
+-rw-rw-rw-   0        0        0       80 2024-05-20 06:59:24.000000 openi-2.0.0b3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-24 07:41:32.599674 openi-2.0.0b3/setup.cfg
+-rw-rw-rw-   0        0        0     1016 2024-05-24 07:40:40.000000 openi-2.0.0b3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:41:32.417097 openi-2.0.0b3/src/
+drwxrwxrwx   0        0        0        0 2024-05-24 07:41:32.540984 openi-2.0.0b3/src/openi/
+-rw-rw-rw-   0        0        0      214 2024-05-20 06:59:24.000000 openi-2.0.0b3/src/openi/__init__.py
+-rw-rw-rw-   0        0        0    11006 2024-05-23 03:12:22.000000 openi-2.0.0b3/src/openi/_dataclass.py
+-rw-rw-rw-   0        0        0     7895 2024-05-23 04:00:55.000000 openi-2.0.0b3/src/openi/_exceptions.py
+-rw-rw-rw-   0        0        0     7127 2024-05-22 07:30:55.000000 openi-2.0.0b3/src/openi/_file.py
+-rw-rw-rw-   0        0        0     4576 2024-05-23 03:19:45.000000 openi-2.0.0b3/src/openi/_login.py
+-rw-rw-rw-   0        0        0     9663 2024-05-22 03:00:39.000000 openi-2.0.0b3/src/openi/_session.py
+-rw-rw-rw-   0        0        0     4120 2024-05-20 06:59:24.000000 openi-2.0.0b3/src/openi/_tqdm.py
+-rw-rw-rw-   0        0        0    36678 2024-05-23 03:19:56.000000 openi-2.0.0b3/src/openi/api.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:41:32.557981 openi-2.0.0b3/src/openi/commands/
+-rw-rw-rw-   0        0        0      328 2024-05-20 06:59:24.000000 openi-2.0.0b3/src/openi/commands/__init__.py
+-rw-rw-rw-   0        0        0     6892 2024-05-24 07:41:32.000000 openi-2.0.0b3/src/openi/commands/dataset.py
+-rw-rw-rw-   0        0        0     8628 2024-05-23 03:19:57.000000 openi-2.0.0b3/src/openi/commands/model.py
+-rw-rw-rw-   0        0        0      897 2024-05-20 06:59:24.000000 openi-2.0.0b3/src/openi/commands/openi_cli.py
+-rw-rw-rw-   0        0        0     2562 2024-05-23 02:22:22.000000 openi-2.0.0b3/src/openi/commands/user.py
+-rw-rw-rw-   0        0        0     2111 2024-05-20 06:59:24.000000 openi-2.0.0b3/src/openi/constants.py
+-rw-rw-rw-   0        0        0    10795 2024-05-24 07:41:32.000000 openi-2.0.0b3/src/openi/downloader.py
+-rw-rw-rw-   0        0        0     3780 2024-05-20 06:59:24.000000 openi-2.0.0b3/src/openi/log.py
+-rw-rw-rw-   0        0        0     9806 2024-05-23 09:58:19.000000 openi-2.0.0b3/src/openi/uploader.py
+-rw-rw-rw-   0        0        0     2775 2024-05-20 06:59:24.000000 openi-2.0.0b3/src/openi/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-24 07:41:32.596675 openi-2.0.0b3/src/openi.egg-info/
+-rw-rw-rw-   0        0        0     2126 2024-05-24 07:41:32.000000 openi-2.0.0b3/src/openi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2024-05-24 07:41:32.000000 openi-2.0.0b3/src/openi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 07:41:32.000000 openi-2.0.0b3/src/openi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-05-24 07:41:32.000000 openi-2.0.0b3/src/openi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2024-05-24 07:41:32.000000 openi-2.0.0b3/src/openi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-24 07:41:32.000000 openi-2.0.0b3/src/openi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-24 07:41:32.594673 openi-2.0.0b3/test/
+-rw-rw-rw-   0        0        0     1149 2024-04-29 07:10:45.000000 openi-2.0.0b3/test/test.py
+-rw-rw-rw-   0        0        0      298 2024-05-24 07:34:44.000000 openi-2.0.0b3/test/test_openi.py
```

### Comparing `openi-2.0.0b2/PKG-INFO` & `openi-2.0.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi
-Version: 2.0.0b2
+Version: 2.0.0b3
 Summary: A package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-2.0.0b2/README.md` & `openi-2.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b2/setup.py` & `openi-2.0.0b3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="openi",
-    version="2.0.0.b2",
+    version="2.0.0.b3",
     description="A package for openi pypi",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi",
     author="chenzh05",
```

### Comparing `openi-2.0.0b2/src/openi/_dataclass.py` & `openi-2.0.0b3/src/openi/_dataclass.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b2/src/openi/_exceptions.py` & `openi-2.0.0b3/src/openi/_exceptions.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b2/src/openi/_file.py` & `openi-2.0.0b3/src/openi/_file.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b2/src/openi/_login.py` & `openi-2.0.0b3/src/openi/_login.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b2/src/openi/_session.py` & `openi-2.0.0b3/src/openi/_session.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b2/src/openi/_tqdm.py` & `openi-2.0.0b3/src/openi/_tqdm.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b2/src/openi/api.py` & `openi-2.0.0b3/src/openi/api.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b2/src/openi/commands/dataset.py` & `openi-2.0.0b3/src/openi/commands/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from argparse import (
-    _SubParsersAction,
-    Namespace,
-    SUPPRESS,
+    _SubParsersAction, Namespace, SUPPRESS,
 )
 from pathlib import Path
 from typing import Optional
 
 from openi.commands import BaseOpeniCLICommand
 from .._exceptions import LocalPathNotFound
 from ..constants import DEFAULT_SAVE_PATH
@@ -80,14 +78,16 @@
         )
         download_parser_optional_args.add_argument(
             "-c",
             "--cluster",
             dest="cluster",
             metavar="",
             required=False,
+            default="npu",
+            choices=["npu", "gpu"],
             help="选填: 指定数据集文件存储类型，可填写`npu` 或 `gpu`; 默认 `npu`",
         )
         download_parser_optional_args.add_argument(
             "-p",
             "--save_path",
             dest="save_path",
             metavar="",
@@ -129,14 +129,15 @@
         self.token: Optional[str] = args.token
         self.endpoint: Optional[str] = args.endpoint
 
     def run(self):
         download_file(
             repo_id=self.repo_id,
             file=self.filename,
+            cluster=self.cluster,
             save_path=self.save_path,
             force=self.force,
             token=self.token,
             endpoint=self.endpoint,
         )
```

### Comparing `openi-2.0.0b2/src/openi/commands/model.py` & `openi-2.0.0b3/src/openi/commands/model.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b2/src/openi/commands/openi_cli.py` & `openi-2.0.0b3/src/openi/commands/openi_cli.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b2/src/openi/commands/user.py` & `openi-2.0.0b3/src/openi/commands/user.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b2/src/openi/constants.py` & `openi-2.0.0b3/src/openi/constants.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b2/src/openi/downloader.py` & `openi-2.0.0b3/src/openi/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,28 @@
 from pathlib import Path
 from typing import (
-    Literal,
-    Optional,
-    Union,
+    Literal, Optional, Union,
 )
 
 from ._dataclass import (
-    DatasetFile,
-    ModelFile,
+    DatasetFile, ModelFile,
 )
 from ._exceptions import (
-    KeyboardInterruptError,
-    OpenIError,
-    ServerFileNotFoundError,
+    KeyboardInterruptError, OpenIError, ServerFileNotFoundError,
     validate_openi_args,
 )
 from ._file import (
-    CacheFile,
-    split_subdir_name,
+    CacheFile, split_subdir_name,
 )
 from ._tqdm import (
-    create_pbar,
-    FileProgressBar,
+    create_pbar, FileProgressBar,
 )
 from .api import OpenIApi
 from .constants import (
-    DEFAULT_SAVE_PATH,
-    UPLOAD_TYPE,
+    DEFAULT_SAVE_PATH, UPLOAD_TYPE,
 )
 from .log import setup_logger
 
 logger = setup_logger()
 
 
 def single_file_downloader(
@@ -310,15 +302,15 @@
             size=f.Size,
             save_path=file_save_path,
             force=force,
         )
         cache_file_list.append(cache_file)
 
         pbar: FileProgressBar = create_pbar(
-            display_name=cache_file.name,
+            display_name=f.FileName,
             size=cache_file.size,
             position=pos,
         )
         pbar_list.append(pbar)
 
     completed_count = 0
     raise_err = None
```

### Comparing `openi-2.0.0b2/src/openi/log.py` & `openi-2.0.0b3/src/openi/log.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b2/src/openi/uploader.py` & `openi-2.0.0b3/src/openi/uploader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,38 @@
 from pathlib import Path
 from typing import (
-    List, Literal, Optional, Union,
+    List,
+    Literal,
+    Optional,
+    Union,
 )
 
 from ._exceptions import (
-    DatasetNotFound, EmptyFolderError, FileSizeError, FileTypeError,
-    KeyboardInterruptError, LocalDirNotFound, LocalPathNotFound,
-    ModelNotFoundError, OpenIError, ServerFileExistsError, UnauthorizedError,
-    UploadError, validate_openi_args,
+    DatasetNotFound,
+    EmptyFolderError,
+    FileSizeError,
+    FileTypeError,
+    KeyboardInterruptError,
+    LocalDirNotFound,
+    LocalPathNotFound,
+    ModelNotFoundError,
+    OpenIError,
+    ServerFileExistsError,
+    UnauthorizedError,
+    UploadError,
+    validate_openi_args,
 )
 from ._file import (
-    get_local_dir_files, is_zip, UploadFile,
+    get_local_dir_files,
+    is_zip,
+    UploadFile,
 )
 from ._tqdm import (
-    create_pbar, FileProgressBar,
+    create_pbar,
+    FileProgressBar,
 )
 from .api import OpenIApi
 from .constants import MAX_FILE_SIZE
 from .log import setup_logger
 from .utils import convert_bytes
 
 logger = setup_logger()
```

### Comparing `openi-2.0.0b2/src/openi/utils.py` & `openi-2.0.0b3/src/openi/utils.py`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b2/src/openi.egg-info/PKG-INFO` & `openi-2.0.0b3/src/openi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openi
-Version: 2.0.0b2
+Version: 2.0.0b3
 Summary: A package for openi pypi
 Home-page: https://openi.pcl.ac.cn/OpenIOSSG/openi-pypi
 Author: chenzh05
 Author-email: chenzh.ds@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `openi-2.0.0b2/src/openi.egg-info/SOURCES.txt` & `openi-2.0.0b3/src/openi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openi-2.0.0b2/test/test.py` & `openi-2.0.0b3/test/test.py`

 * *Files identical despite different names*


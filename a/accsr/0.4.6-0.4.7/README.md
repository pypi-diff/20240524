# Comparing `tmp/accsr-0.4.6.tar.gz` & `tmp/accsr-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accsr-0.4.6.tar", last modified: Wed Dec  6 14:58:15 2023, max compression
+gzip compressed data, was "accsr-0.4.7.tar", last modified: Fri May 24 11:44:56 2024, max compression
```

## Comparing `accsr-0.4.6.tar` & `accsr-0.4.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 14:58:15.598071 accsr-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-12-06 14:58:06.000000 accsr-0.4.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-06 14:58:06.000000 accsr-0.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      255 2023-12-06 14:58:15.598071 accsr-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2023-12-06 14:58:06.000000 accsr-0.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      319 2023-12-06 14:58:06.000000 accsr-0.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-12-06 14:58:06.000000 accsr-0.4.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-06 14:58:15.598071 accsr-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      728 2023-12-06 14:58:06.000000 accsr-0.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 14:58:15.594071 accsr-0.4.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 14:58:15.598071 accsr-0.4.6/src/accsr/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-06 14:58:06.000000 accsr-0.4.6/src/accsr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12970 2023-12-06 14:58:06.000000 accsr-0.4.6/src/accsr/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2023-12-06 14:58:06.000000 accsr-0.4.6/src/accsr/conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2023-12-06 14:58:06.000000 accsr-0.4.6/src/accsr/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2023-12-06 14:58:06.000000 accsr-0.4.6/src/accsr/loading.py
--rw-r--r--   0 runner    (1001) docker     (127)    42089 2023-12-06 14:58:06.000000 accsr-0.4.6/src/accsr/remote_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 14:58:15.598071 accsr-0.4.6/src/accsr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2023-12-06 14:58:15.000000 accsr-0.4.6/src/accsr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      372 2023-12-06 14:58:15.000000 accsr-0.4.6/src/accsr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-06 14:58:15.000000 accsr-0.4.6/src/accsr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-12-06 14:58:15.000000 accsr-0.4.6/src/accsr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-06 14:58:15.000000 accsr-0.4.6/src/accsr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:44:56.485584 accsr-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-24 11:44:47.000000 accsr-0.4.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-24 11:44:47.000000 accsr-0.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-24 11:44:56.485584 accsr-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-24 11:44:47.000000 accsr-0.4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-24 11:44:47.000000 accsr-0.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-24 11:44:47.000000 accsr-0.4.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 11:44:56.485584 accsr-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-24 11:44:47.000000 accsr-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:44:56.481584 accsr-0.4.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:44:56.485584 accsr-0.4.7/src/accsr/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-24 11:44:47.000000 accsr-0.4.7/src/accsr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-05-24 11:44:47.000000 accsr-0.4.7/src/accsr/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-24 11:44:47.000000 accsr-0.4.7/src/accsr/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-24 11:44:47.000000 accsr-0.4.7/src/accsr/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-24 11:44:47.000000 accsr-0.4.7/src/accsr/loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44919 2024-05-24 11:44:47.000000 accsr-0.4.7/src/accsr/remote_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:44:56.485584 accsr-0.4.7/src/accsr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-24 11:44:56.000000 accsr-0.4.7/src/accsr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-24 11:44:56.000000 accsr-0.4.7/src/accsr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 11:44:56.000000 accsr-0.4.7/src/accsr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-24 11:44:56.000000 accsr-0.4.7/src/accsr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-24 11:44:56.000000 accsr-0.4.7/src/accsr.egg-info/top_level.txt
```

### Comparing `accsr-0.4.6/LICENSE.md` & `accsr-0.4.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `accsr-0.4.6/README.md` & `accsr-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `accsr-0.4.6/setup.py` & `accsr-0.4.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 setup(
     name="accsr",
     python_requires=">=3.8",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     include_package_data=True,
-    version="0.4.6",
+    version="0.4.7",
     description="Utils for accessing data from anywhere",
     install_requires=open("requirements.txt").readlines(),
     setup_requires=["wheel"],
     tests_require=test_requirements,
     extras_require={
         "test": test_requirements,
         "docs": docs_requirements,
```

### Comparing `accsr-0.4.6/src/accsr/config.py` & `accsr-0.4.7/src/accsr/config.py`

 * *Files identical despite different names*

### Comparing `accsr-0.4.6/src/accsr/conversions.py` & `accsr-0.4.7/src/accsr/conversions.py`

 * *Files identical despite different names*

### Comparing `accsr-0.4.6/src/accsr/loading.py` & `accsr-0.4.7/src/accsr/loading.py`

 * *Files identical despite different names*

### Comparing `accsr-0.4.6/src/accsr/remote_storage.py` & `accsr-0.4.7/src/accsr/remote_storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,25 +7,28 @@
 from copy import copy
 from dataclasses import asdict, dataclass, field, is_dataclass
 from enum import Enum
 from functools import cached_property
 from pathlib import Path
 from typing import (
     Dict,
+    Generator,
     List,
+    Literal,
     Optional,
     Pattern,
     Protocol,
     Sequence,
     Union,
+    cast,
     runtime_checkable,
 )
 
-import libcloud
 from libcloud.storage.base import Container, StorageDriver
+from libcloud.storage.providers import get_driver
 from libcloud.storage.types import (
     ContainerAlreadyExistsError,
     InvalidContainerNameError,
 )
 from tqdm import tqdm
 
 from accsr.files import md5sum
@@ -59,15 +62,15 @@
 
 
 def _replace_driver_by_name(obj):
     # The driver object from libcloud stores a connection and is not serializable.
     # Since sometimes we want to be able to deepcopy these things around,
     # we replace the driver by its name. This is needed for `asdict` to work.
     if isinstance(obj, RemoteObjectProtocol) and hasattr(obj, "driver"):
-        obj.driver = obj.driver.name
+        obj.driver = obj.driver.name  # type: ignore
     if isinstance(obj, list) or isinstance(obj, tuple):
         for item in obj:
             _replace_driver_by_name(item)
     if isinstance(obj, dict):
         for key, value in obj.items():
             _replace_driver_by_name(value)
 
@@ -77,15 +80,15 @@
         return json.dumps(self, indent=2, sort_keys=True, cls=_SummariesJSONEncoder)
 
     def __repr__(self):
         return f"\n{self.__class__.__name__}: \n{self.to_json()}\n"
 
 
 @contextmanager
-def _switch_to_dir(path: str = None) -> bool:
+def _switch_to_dir(path: Optional[str] = None) -> Generator[None, None, None]:
     if path:
         cur_dir = os.getcwd()
         try:
             os.chdir(path)
             yield
         finally:
             os.chdir(cur_dir)
@@ -124,17 +127,17 @@
     It is not recommended creating or manipulate instances of this class outside RemoteStorage, in particular
     in user code. This class forms part of the public interface because instances of it are given to users for
     introspection.
     """
 
     def __init__(
         self,
-        local_path: str = None,
-        remote_obj: RemoteObjectProtocol = None,
-        remote_path: str = None,
+        local_path: Optional[str] = None,
+        remote_obj: Optional[RemoteObjectProtocol] = None,
+        remote_path: Optional[str] = None,
     ):
         if remote_path is not None:
             remote_path = remote_path.lstrip("/")
         if remote_obj is not None:
             remote_obj = copy(remote_obj)
             remote_obj.name = remote_obj.name.lstrip("/")
 
@@ -157,16 +160,21 @@
                 )
             self.remote_path = remote_path
         else:
             if remote_obj is None:
                 raise ValueError(f"Either remote_path or remote_obj should be not None")
             self.remote_path = remote_obj.name
 
-        self.local_size = os.path.getsize(local_path) if self.exists_locally else 0
-        self.local_hash = md5sum(local_path) if self.exists_locally else None
+        if self.exists_locally:
+            assert self.local_path is not None
+            self.local_size = os.path.getsize(self.local_path)
+            self.local_hash = md5sum(self.local_path)
+        else:
+            self.local_size = 0
+            self.local_hash = None
 
     @property
     def name(self):
         return self.remote_path
 
     @property
     def exists_on_target(self) -> bool:
@@ -257,15 +265,15 @@
     on_target_neq_md5: List[SyncObject] = field(default_factory=list)
     unresolvable_collisions: Dict[str, Union[List[RemoteObjectProtocol], str]] = field(
         default_factory=dict
     )
     skipped_source_files: List[SyncObject] = field(default_factory=list)
 
     synced_files: List[SyncObject] = field(default_factory=list)
-    sync_direction: Optional[str] = None
+    sync_direction: Optional[Literal["push", "pull"]] = None
 
     def __post_init__(self):
         if self.sync_direction not in ["pull", "push", None]:
             raise ValueError(
                 f"sync_direction can only be set to pull, push or None, instead got: {self.sync_direction}"
             )
 
@@ -373,17 +381,17 @@
     to a bucket within the remote storage, and the base path on the remote.
     """
 
     provider: str
     key: str
     bucket: str
     secret: str = field(repr=False)
-    region: str = None
-    host: str = None
-    port: int = None
+    region: Optional[str] = None
+    host: Optional[str] = None
+    port: Optional[int] = None
     base_path: str = ""
     secure: bool = True
 
 
 class RemoteStorage:
     """
     Wrapper around lib-cloud for accessing remote storage services.
@@ -451,38 +459,32 @@
     @cached_property
     def bucket(self) -> Container:
         log.info(f"Establishing connection to bucket {self.conf.bucket}")
         return self.driver.get_container(self.conf.bucket)
 
     @cached_property
     def driver(self) -> StorageDriver:
-        storage_driver_factory = libcloud.get_driver(
-            libcloud.DriverType.STORAGE, self.provider
-        )
+        storage_driver_factory = get_driver(self.provider)
         return storage_driver_factory(**self.driver_kwargs)
 
     def _execute_sync(
-        self, sync_object: SyncObject, direction: str, force=False
+        self, sync_object: SyncObject, direction: Literal["push", "pull"], force=False
     ) -> SyncObject:
         """
         Synchronizes the local and the remote file in the given direction. Will raise an error if a file from the source
         would overwrite an already existing file on the target and force=False. In this case, no operations will be
         performed on the target.
 
         :param sync_object: instance of SyncObject that will be used as basis for synchronization. Usually
             created from a get_*_summary method.
         :param direction: either "push" or "pull"
         :param force: if True, all already existing files on the target (with a different md5sum than the source files)
             will be overwritten.
         :return: a SyncObject that represents the status of remote and target after the synchronization
         """
-        if direction not in ["push", "pull"]:
-            raise ValueError(
-                f"Unknown direction {direction}, has to be either 'push' or 'pull'."
-            )
         if sync_object.equal_md5_hash_sum:
             log.debug(
                 f"Skipping {direction} of {sync_object.name} because of coinciding hash sums"
             )
             return sync_object
 
         if sync_object.exists_on_target and not force:
@@ -491,38 +493,46 @@
             )
 
         if direction == "push":
             if not sync_object.exists_locally:
                 raise FileNotFoundError(
                     f"Cannot push non-existing file: {sync_object.local_path}"
                 )
-            # noinspection PyTypeChecker
-            remote_obj: RemoteObjectProtocol = self.bucket.upload_object(
-                sync_object.local_path,
-                sync_object.remote_path,
-                verify_hash=False,
+            assert sync_object.local_path is not None
+            remote_obj = cast(
+                RemoteObjectProtocol,
+                self.bucket.upload_object(
+                    sync_object.local_path,
+                    sync_object.remote_path,
+                    verify_hash=False,
+                ),
             )
             return SyncObject(sync_object.local_path, remote_obj)
 
         elif direction == "pull":
             if None in [sync_object.remote_obj, sync_object.local_path]:
                 raise RuntimeError(
                     f"Cannot pull without remote object and local path. Affects: {sync_object.name}"
                 )
+            assert sync_object.local_path is not None
             if os.path.isdir(sync_object.local_path):
                 raise FileExistsError(
                     f"Cannot pull file to a path which is an existing directory: {sync_object.local_path}"
                 )
 
             log.debug(f"Fetching {sync_object.remote_obj.name} from {self.bucket.name}")
             os.makedirs(os.path.dirname(sync_object.local_path), exist_ok=True)
             sync_object.remote_obj.download(
                 sync_object.local_path, overwrite_existing=force
             )
             return SyncObject(sync_object.local_path, sync_object.remote_obj)
+        else:
+            raise ValueError(
+                f"Unknown direction {direction}, has to be either 'push' or 'pull'."
+            )
 
     @staticmethod
     def _get_remote_path(remote_obj: RemoteObjectProtocol) -> str:
         """
         Returns the full path to the remote object. The resulting path never starts with "/" as it can cause problems
         with some backends (e.g. google cloud storage).
         """
@@ -616,37 +626,41 @@
             )
 
         desc = f"{summary.sync_direction}ing (bytes)"
         if force:
             desc = "force " + desc
         with tqdm(total=summary.size_files_to_sync(), desc=desc) as pbar:
             for sync_obj in summary.files_to_sync:
+                assert summary.sync_direction is not None
                 synced_obj = self._execute_sync(
                     sync_obj, direction=summary.sync_direction, force=force
                 )
                 pbar.update(synced_obj.local_size)
                 summary.synced_files.append(synced_obj)
         return summary
 
     def pull(
         self,
         remote_path: str,
-        local_base_dir="",
-        force=False,
-        include_regex: Union[Pattern, str] = None,
-        exclude_regex: Union[Pattern, str] = None,
-        convert_to_linux_path=True,
-        dryrun=False,
-        path_regex: Union[Pattern, str] = None,
+        local_base_dir: str = "",
+        force: bool = False,
+        include_regex: Optional[Union[Pattern, str]] = None,
+        exclude_regex: Optional[Union[Pattern, str]] = None,
+        convert_to_linux_path: bool = True,
+        dryrun: bool = False,
+        path_regex: Optional[Union[Pattern, str]] = None,
+        strip_abspath_prefix: Optional[str] = None,
+        strip_abs_local_base_dir: bool = True,
     ) -> TransactionSummary:
         r"""
         Pull either a file or a directory under the given path relative to local_base_dir.
 
         :param remote_path: remote path on storage bucket relative to the configured remote base path.
-            e.g. 'data/ground_truth/some_file.json'
+            e.g. 'data/ground_truth/some_file.json'. Can also be an absolute local path if ``strip_abspath_prefix``
+            is specified.
         :param local_base_dir: Local base directory for constructing local path
             e.g. passing 'local_base_dir' will download to the path
             'local_base_dir/data/ground_truth/some_file.json' in the above example
         :param force: If False, pull will raise an error if an already existing file deviates from the remote in
             its md5sum. If True, these files are overwritten.
         :param include_regex: If not None only files with paths matching the regex will be pulled. This is useful for
             filtering files within a remote directory before pulling them.
@@ -654,16 +668,47 @@
             Takes precedence over ``include_regex``, i.e. if a file matches both, it will be excluded.
         :param convert_to_linux_path: if True, will convert windows path to linux path (as needed by remote storage) and
             thus passing a remote path like 'data\my\path' will be converted to 'data/my/path' before pulling.
             This should only be set to False if you want to pull a remote object with '\' in its file name
             (which is discouraged).
         :param dryrun: If True, simulates the pull operation and returns the remote objects that would have been pulled.
         :param path_regex: DEPRECATED! Use ``include_regex`` instead.
+        :param strip_abspath_prefix: Will only have an effect if the `remote_path` is absolute.
+            Then the given prefix is removed from it before pulling. This is useful for pulling files from a remote storage
+            by directly specifying absolute local paths instead of first converting them to actual remote paths.
+            Similar in logic to `local_path_prefix` in `push`.
+            A common use case is to always set `local_base_dir` to the same value and to always pass absolute paths
+            as `remote_path` to `pull`.
+        :param strip_abs_local_base_dir: If True, and `local_base_dir` is an absolute path, then
+            the `local_base_dir` will be treated as `strip_abspath_prefix`. See explanation of `strip_abspath_prefix`.
         :return: An object describing the summary of the operation.
         """
+
+        if strip_abs_local_base_dir and os.path.isabs(local_base_dir):
+            if strip_abspath_prefix is not None:
+                raise ValueError(
+                    f"Cannot specify both `strip_abs_local_base_dir`={strip_abs_local_base_dir} "
+                    f"and `strip_abspath_prefix`={strip_abspath_prefix}"
+                    f"when `local_base_dir`={local_base_dir} is an absolute path."
+                )
+            strip_abspath_prefix = local_base_dir
+
+        remote_path_is_abs = remote_path.startswith("/") or os.path.isabs(remote_path)
+
+        if strip_abspath_prefix is not None and remote_path_is_abs:
+            remote_path = remote_path.replace("\\", "/")
+            strip_abspath_prefix = strip_abspath_prefix.replace("\\", "/").rstrip("/")
+            if not remote_path.startswith(strip_abspath_prefix):
+                raise ValueError(
+                    f"Remote path {remote_path} is absolute but does not start "
+                    f"with the given prefix {strip_abspath_prefix}"
+                )
+            # +1 for removing the leading '/'
+            remote_path = remote_path[len(strip_abspath_prefix) + 1 :]
+
         include_regex = self._handle_deprecated_path_regex(include_regex, path_regex)
         summary = self._get_pull_summary(
             remote_path,
             local_base_dir,
             include_regex=include_regex,
             exclude_regex=exclude_regex,
             convert_to_linux_path=convert_to_linux_path,
@@ -680,19 +725,19 @@
         """
         relative_obj_path = self._get_relative_remote_path(obj)
         return os.path.join(local_base_dir, relative_obj_path)
 
     def _get_pull_summary(
         self,
         remote_path: str,
-        local_base_dir="",
-        include_regex: Union[Pattern, str] = None,
-        exclude_regex: Union[Pattern, str] = None,
-        convert_to_linux_path=True,
-        path_regex: Union[Pattern, str] = None,
+        local_base_dir: str = "",
+        include_regex: Optional[Union[Pattern, str]] = None,
+        exclude_regex: Optional[Union[Pattern, str]] = None,
+        convert_to_linux_path: bool = True,
+        path_regex: Optional[Union[Pattern, str]] = None,
     ) -> TransactionSummary:
         r"""
         Creates TransactionSummary of the specified pull operation.
 
         :param remote_path: remote path on storage bucket relative to the configured remote base path.
             e.g. 'data/ground_truth/some_file.json'
         :param local_base_dir: Local base directory for constructing local path.
@@ -717,16 +762,16 @@
         local_base_dir = os.path.abspath(local_base_dir)
         if convert_to_linux_path:
             remote_path = remote_path.replace("\\", "/")
 
         summary = TransactionSummary(sync_direction="pull")
         full_remote_path = self._full_remote_path(remote_path)
         # noinspection PyTypeChecker
-        remote_objects: List[RemoteObjectProtocol] = list(
-            self.bucket.list_objects(full_remote_path)
+        remote_objects = cast(
+            List[RemoteObjectProtocol], list(self.bucket.list_objects(full_remote_path))
         )
 
         for obj in tqdm(
             remote_objects,
             desc=f"Scanning remote paths in {self.bucket.name}/{full_remote_path}: ",
         ):
             local_path = None
@@ -833,39 +878,43 @@
                 desc=f"Scanning files in {os.path.join(os.getcwd(), path)}: ",
             ):
                 collides_with = None
                 remote_obj = None
                 skip = self._should_skip(file, include_regex, exclude_regex)
 
                 remote_path = self.get_push_remote_path(file)
-                # noinspection PyTypeChecker
+
+                all_matched_remote_obj = cast(
+                    List[RemoteObjectProtocol], self.bucket.list_objects(remote_path)
+                )
                 matched_remote_obj = [
                     obj
-                    for obj in self.bucket.list_objects(remote_path)
+                    for obj in all_matched_remote_obj
                     if not self._listed_due_to_name_collision(remote_path, obj)
                 ]
 
                 # name collision of local file with remote dir
                 if len(matched_remote_obj) > 1:
                     collides_with = matched_remote_obj
 
                 elif matched_remote_obj:
                     remote_obj = matched_remote_obj[0]
-
                 synced_obj = SyncObject(file, remote_obj, remote_path=remote_path)
                 summary.add_entry(
                     synced_obj,
                     collides_with=collides_with,
                     skip=skip,
                 )
 
         return summary
 
     @staticmethod
-    def _should_skip(file: str, include_regex: Pattern, exclude_regex: Pattern):
+    def _should_skip(
+        file: str, include_regex: Optional[Pattern], exclude_regex: Optional[Pattern]
+    ):
         if include_regex is not None and not include_regex.match(file):
             log.debug(
                 f"Skipping {file} since it does not match regular expression '{include_regex}'."
             )
             return True
         if exclude_regex is not None and exclude_regex.match(file):
             log.debug(
@@ -891,26 +940,26 @@
                 )
             include_regex = path_regex
         return include_regex
 
     def push(
         self,
         path: str,
-        local_path_prefix: str = None,
+        local_path_prefix: Optional[str] = None,
         force: bool = False,
-        include_regex: Union[Pattern, str] = None,
-        exclude_regex: Union[Pattern, str] = None,
+        include_regex: Optional[Union[Pattern, str]] = None,
+        exclude_regex: Optional[Union[Pattern, str]] = None,
         dryrun: bool = False,
-        path_regex: Union[Pattern, str] = None,
+        path_regex: Optional[Union[Pattern, str]] = None,
     ) -> TransactionSummary:
         """
         Upload files into the remote storage.
         Does not upload files for which the md5sum matches existing remote files.
         The remote path for uploading will be constructed from the remote_base_path and the provided path.
-        The local_path_prefix serves for finding the directory on the local system or for stripping off
+        The `local_path_prefix` serves for finding the directory on the local system or for stripping off
         parts of absolute paths if path is absolute, see examples below.
 
         Examples:
            1) path=foo/bar, local_path_prefix=None -->
                 ./foo/bar uploaded to remote_base_path/foo/bar
            2) path=/home/foo/bar, local_path_prefix=None -->
                 /home/foo/bar uploaded to remote_base_path/home/foo/bar
@@ -944,17 +993,17 @@
             exclude_regex=exclude_regex,
         )
         return self._execute_sync_from_summary(summary, dryrun=dryrun, force=force)
 
     def delete(
         self,
         remote_path: str,
-        include_regex: Union[Pattern, str] = None,
-        exclude_regex: Union[Pattern, str] = None,
-        path_regex: Union[Pattern, str] = None,
+        include_regex: Optional[Union[Pattern, str]] = None,
+        exclude_regex: Optional[Union[Pattern, str]] = None,
+        path_regex: Optional[Union[Pattern, str]] = None,
     ) -> List[RemoteObjectProtocol]:
         """
         Deletes a file or a directory under the given path relative to local_base_dir. Use with caution!
 
         :param remote_path: remote path on storage bucket relative to the configured remote base path.
         :param include_regex: If not None only files with paths matching the regex will be deleted.
         :param exclude_regex: If not None only files with paths not matching the regex will be deleted.
@@ -964,44 +1013,42 @@
         """
         include_regex = self._handle_deprecated_path_regex(include_regex, path_regex)
         include_regex = _to_optional_pattern(include_regex)
         exclude_regex = _to_optional_pattern(exclude_regex)
 
         full_remote_path = self._full_remote_path(remote_path)
 
-        remote_objects = self.bucket.list_objects(full_remote_path)
+        remote_objects = cast(
+            List[RemoteObjectProtocol], self.bucket.list_objects(full_remote_path)
+        )
         if len(remote_objects) == 0:
             log.warning(
                 f"No such remote file or directory: {full_remote_path}. Not deleting anything"
             )
             return []
         deleted_objects = []
         for remote_obj in remote_objects:
-            remote_obj: RemoteObjectProtocol
-
             if self._listed_due_to_name_collision(full_remote_path, remote_obj):
                 log.debug(
                     f"Skipping deletion of {remote_obj.name} as it was listed due to name collision"
                 )
                 continue
 
             relative_obj_path = self._get_relative_remote_path(remote_obj)
             if include_regex is not None and not include_regex.match(relative_obj_path):
                 log.info(f"Skipping {relative_obj_path} due to regex {include_regex}")
                 continue
             if exclude_regex is not None and exclude_regex.match(relative_obj_path):
                 log.info(f"Skipping {relative_obj_path} due to regex {exclude_regex}")
                 continue
             log.debug(f"Deleting {remote_obj.name}")
-            # noinspection PyTypeChecker
-            self.bucket.delete_object(remote_obj)
+            self.bucket.delete_object(remote_obj)  # type: ignore
             deleted_objects.append(remote_obj)
         return deleted_objects
 
     def list_objects(self, remote_path: str) -> List[RemoteObjectProtocol]:
         """
         :param remote_path: remote path on storage bucket relative to the configured remote base path.
         :return: list of remote objects under the remote path (multiple entries if the remote path is a directory)
         """
         full_remote_path = self._full_remote_path(remote_path)
-        # noinspection PyTypeChecker
-        return self.bucket.list_objects(full_remote_path)
+        return self.bucket.list_objects(full_remote_path)  # type: ignore
```


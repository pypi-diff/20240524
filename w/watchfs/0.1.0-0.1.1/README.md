# Comparing `tmp/watchfs-0.1.0.tar.gz` & `tmp/watchfs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchfs-0.1.0.tar", max compression
+gzip compressed data, was "watchfs-0.1.1.tar", max compression
```

## Comparing `watchfs-0.1.0.tar` & `watchfs-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1090 2024-02-17 08:43:42.708787 watchfs-0.1.0/LICENSE
--rw-r--r--   0        0        0     1275 2024-02-17 08:43:42.708787 watchfs-0.1.0/README.md
--rw-r--r--   0        0        0     1689 2024-02-17 08:43:42.708787 watchfs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      287 2024-02-17 08:43:42.708787 watchfs-0.1.0/watchfs/__init__.py
--rw-r--r--   0        0        0     3911 2024-02-17 08:43:42.708787 watchfs-0.1.0/watchfs/__main__.py
--rw-r--r--   0        0        0      386 2024-02-17 08:43:42.708787 watchfs-0.1.0/watchfs/as_sync.py
--rw-r--r--   0        0        0      357 2024-02-17 08:43:42.708787 watchfs-0.1.0/watchfs/colorful.py
--rw-r--r--   0        0        0      789 2024-02-17 08:43:42.708787 watchfs-0.1.0/watchfs/exceptions.py
--rw-r--r--   0        0        0      865 2024-02-17 08:43:42.708787 watchfs-0.1.0/watchfs/rusty.py
--rw-r--r--   0        0        0     2080 1970-01-01 00:00:00.000000 watchfs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-05-24 02:38:05.206722 watchfs-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1281 2024-05-24 02:38:05.206722 watchfs-0.1.1/README.md
+-rw-r--r--   0        0        0     1745 2024-05-24 02:38:05.206722 watchfs-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      287 2024-05-24 02:38:05.210722 watchfs-0.1.1/watchfs/__init__.py
+-rw-r--r--   0        0        0     5007 2024-05-24 02:38:05.210722 watchfs-0.1.1/watchfs/__main__.py
+-rw-r--r--   0        0        0      386 2024-05-24 02:38:05.210722 watchfs-0.1.1/watchfs/as_sync.py
+-rw-r--r--   0        0        0      357 2024-05-24 02:38:05.210722 watchfs-0.1.1/watchfs/colorful.py
+-rw-r--r--   0        0        0      789 2024-05-24 02:38:05.210722 watchfs-0.1.1/watchfs/exceptions.py
+-rw-r--r--   0        0        0     2675 2024-05-24 02:38:05.210722 watchfs-0.1.1/watchfs/filters.py
+-rw-r--r--   0        0        0      865 2024-05-24 02:38:05.210722 watchfs-0.1.1/watchfs/rusty.py
+-rw-r--r--   0        0        0     2148 1970-01-01 00:00:00.000000 watchfs-0.1.1/PKG-INFO
```

### Comparing `watchfs-0.1.0/LICENSE` & `watchfs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `watchfs-0.1.0/README.md` & `watchfs-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
    <a href="https://github.com/astral-sh/ruff"><img alt="ruff" src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json&style=flat-square"></a>
    <a href="https://gitmoji.dev"><img alt="Gitmoji" src="https://img.shields.io/badge/gitmoji-%20😜%20😍-FFDD67?style=flat-square"></a>
 </p>
 
 ## Installation
 
 ```python
-pipx install .
+pipx install watchfs
 ```
 
 ## Usage
 
 ```python
 watchfs src1:dst1 src2:dst2
 ```
```

#### html2text {}

```diff
@@ -1,5 +1,5 @@
 # WatchFS Watch and sync files to another directory.
            _[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_p_y_p_i_]_[_P_y_P_I_ _-_ _D_o_w_n_l_o_a_d_s_]_[_L_I_C_E_N_S_E_]
                             _[_b_l_a_c_k_]_[_r_u_f_f_]_[_G_i_t_m_o_j_i_]
-## Installation ```python pipx install . ``` ## Usage ```python watchfs src1:
-dst1 src2:dst2 ```
+## Installation ```python pipx install watchfs ``` ## Usage ```python watchfs
+src1:dst1 src2:dst2 ```
```

### Comparing `watchfs-0.1.0/pyproject.toml` & `watchfs-0.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "watchfs"
-version = "0.1.0"
-description = ""
+version = "0.1.1"
+description = "Watch and sync files to another directory"
 authors = ["Nyakku Shigure <sigure.qaq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ShigureLab/watchfs"
 repository = "https://github.com/ShigureLab/watchfs"
-keywords = []
+keywords = ["watch", "sync"]
 classifiers = [
   "Operating System :: OS Independent",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
@@ -24,15 +24,15 @@
 aiofiles = "^23.2.1"
 colored = "^2.2.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
 pyright = "^1.1.333"
 pytest-rerunfailures = "^12.0"
-ruff = "^0.2.0"
+ruff = "^0.4.0"
 
 [tool.poetry.scripts]
 watchfs = "watchfs.__main__:main"
 
 [tool.pyright]
 include = ["watchfs", "tests"]
 pythonVersion = "3.12"
```

### Comparing `watchfs-0.1.0/watchfs/__main__.py` & `watchfs-0.1.1/watchfs/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 import asyncio
 import shutil
 from pathlib import Path
 
 from aiofiles.os import wrap
 from colored import Back, Fore  # type: ignore
 from watchfiles import Change, awatch  # type: ignore
+from watchfiles.filters import BaseFilter
 
 from watchfs import __version__
 from watchfs.as_sync import as_sync
 from watchfs.colorful import Badge
 from watchfs.exceptions import ParseError
+from watchfs.filters import ChangeCacheFilter, ExcludeFilter, combine_filters
 from watchfs.rusty import Err, Ok, Result
 
 BADGE_ADD = Badge("ADDED", Fore.black, Back.green)
 BADGE_DEL = Badge("DELETED", Fore.black, Back.red)
 BADGE_MOD = Badge("MODIFIED", Fore.black, Back.blue)
 CHANGE_TYPE_TO_BADGE = {
     Change.added: BADGE_ADD,
@@ -50,61 +52,80 @@
             child_rel_to_dst = child.relative_to(dst_dir)
             await handle_removed(src_dir, dst_dir, src_dir / child_rel_to_dst)
         dst.rmdir()
     elif dst.is_file():
         dst.unlink()
 
 
-async def sync(src_dir: str, dst_dir: str):
+async def sync(src_dir: str, dst_dir: str, filter: BaseFilter):
     src = Path(src_dir).absolute()
     dst = Path(dst_dir).absolute()
-    async for changes in awatch(src):
+    async for changes in awatch(src, watch_filter=filter):
         for change, path in changes:
             path = Path(path).absolute()
             print(f"{CHANGE_TYPE_TO_BADGE[change]} {path}")
             match change:
                 case Change.added:
                     await handle_added(src, dst, path)
                 case Change.modified:
                     await handle_modified(src, dst, path)
                 case Change.deleted:
                     await handle_removed(src, dst, path)
 
 
-def parse_sync_mapping(sync_mapping: str) -> Result[tuple[str, str], ParseError]:
-    splited_sync_mapping = sync_mapping.split(":")
+def parse_sync_mapping(sync_mapping: str) -> Result[tuple[str, str, bool], ParseError]:
+    splited_sync_mapping: list[str] = sync_mapping.split(":")
+    bidirectional: bool = False
+    if ":" in sync_mapping:
+        splited_sync_mapping = sync_mapping.split(":")
+    elif "<->" in sync_mapping:
+        splited_sync_mapping = sync_mapping.split("<->")
+        bidirectional = True
+    elif "->" in sync_mapping:
+        splited_sync_mapping = sync_mapping.split("->")
     if len(splited_sync_mapping) != 2:
         return Err(ParseError("Invalid sync mapping."))
-    src_dir, dst_dir = sync_mapping.split(":")
+    src_dir, dst_dir = splited_sync_mapping
 
     # check if src_dir is a subdirectory of dst_dir
     abs_src_dir = Path(src_dir).resolve()
     abs_dst_dir = Path(dst_dir).resolve()
     if abs_src_dir in abs_dst_dir.parents:
         return Err(ParseError(f"src_dir({abs_src_dir}) is a subdirectory of dst_dir({abs_dst_dir})."))
 
-    return Ok((src_dir, dst_dir))
+    return Ok((src_dir, dst_dir, bidirectional))
 
 
 @as_sync
 async def main():
     parser = argparse.ArgumentParser(prog="watchfs", description="Watch and sync files.")
     parser.add_argument("-v", "--version", action="version", version=__version__)
     parser.add_argument("sync_mapping", metavar="SRC_DIR:DST_DIR", type=str, nargs="+", help="Sync mapping file.")
+    parser.add_argument("--exclude", type=str, help="Exclude directories or files, separated by comma.")
+    parser.add_argument("-cc", "--enable-content-caching", action="store_true", help="Enable content caching.")
     args = parser.parse_args()
     parsed_sync_mapping: list[tuple[str, str]] = []
     for sync_src_with_dst in args.sync_mapping:
         match parse_sync_mapping(sync_src_with_dst):
-            case Ok((src_dir, dst_dir)):
+            case Ok((src_dir, dst_dir, bidirectional)):
                 parsed_sync_mapping.append((src_dir, dst_dir))
+                if bidirectional:
+                    parsed_sync_mapping.append((dst_dir, src_dir))
             case Err(err):
                 raise err
+    filters: list[BaseFilter] = []
+    if args.exclude:
+        filters.append(ExcludeFilter(args.exclude))
+    if args.enable_content_caching:
+        filters.append(ChangeCacheFilter())
+
+    combined_filter = combine_filters(filters)
     print(f"Starting watch {', '.join(map(lambda src_dst: f"{src_dst[0]} -> {src_dst[1]}", parsed_sync_mapping))}")
     print("Press Ctrl+C to exit.")
     try:
-        await asyncio.gather(*[sync(src_dir, dst_dir) for src_dir, dst_dir in parsed_sync_mapping])
+        await asyncio.gather(*[sync(src_dir, dst_dir, combined_filter) for src_dir, dst_dir in parsed_sync_mapping])
     except asyncio.exceptions.CancelledError:
         print("Bye!")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `watchfs-0.1.0/watchfs/exceptions.py` & `watchfs-0.1.1/watchfs/exceptions.py`

 * *Files identical despite different names*

### Comparing `watchfs-0.1.0/watchfs/rusty.py` & `watchfs-0.1.1/watchfs/rusty.py`

 * *Files identical despite different names*

### Comparing `watchfs-0.1.0/PKG-INFO` & `watchfs-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: watchfs
-Version: 0.1.0
-Summary: 
+Version: 0.1.1
+Summary: Watch and sync files to another directory
 Home-page: https://github.com/ShigureLab/watchfs
 License: MIT
+Keywords: watch,sync
 Author: Nyakku Shigure
 Author-email: sigure.qaq@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -34,15 +35,15 @@
    <a href="https://github.com/astral-sh/ruff"><img alt="ruff" src="https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json&style=flat-square"></a>
    <a href="https://gitmoji.dev"><img alt="Gitmoji" src="https://img.shields.io/badge/gitmoji-%20😜%20😍-FFDD67?style=flat-square"></a>
 </p>
 
 ## Installation
 
 ```python
-pipx install .
+pipx install watchfs
 ```
 
 ## Usage
 
 ```python
 watchfs src1:dst1 src2:dst2
 ```
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1 Name: watchfs Version: 0.1.0 Summary: Home-page: https://
-github.com/ShigureLab/watchfs License: MIT Author: Nyakku Shigure Author-email:
+Metadata-Version: 2.1 Name: watchfs Version: 0.1.1 Summary: Watch and sync
+files to another directory Home-page: https://github.com/ShigureLab/watchfs
+License: MIT Keywords: watch,sync Author: Nyakku Shigure Author-email:
 sigure.qaq@gmail.com Requires-Python: >=3.12,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Programming Language :: Python :: Implementation :: CPython Requires-Dist:
 aiofiles (>=23.2.1,<24.0.0) Requires-Dist: colored (>=2.2.3,<3.0.0) Requires-
 Dist: typing-extensions (>=4.8.0,<5.0.0) Requires-Dist: watchfiles
 (>=0.21.0,<0.22.0) Project-URL: Repository, https://github.com/ShigureLab/
 watchfs Description-Content-Type: text/markdown # WatchFS Watch and sync files
 to another directory.
            _[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_p_y_p_i_]_[_P_y_P_I_ _-_ _D_o_w_n_l_o_a_d_s_]_[_L_I_C_E_N_S_E_]
                             _[_b_l_a_c_k_]_[_r_u_f_f_]_[_G_i_t_m_o_j_i_]
-## Installation ```python pipx install . ``` ## Usage ```python watchfs src1:
-dst1 src2:dst2 ```
+## Installation ```python pipx install watchfs ``` ## Usage ```python watchfs
+src1:dst1 src2:dst2 ```
```


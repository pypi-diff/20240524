# Comparing `tmp/nfs-estepona-0.2.4.tar.gz` & `tmp/nfs_estepona-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nfs-estepona-0.2.4.tar", last modified: Mon Sep 27 19:50:56 2021, max compression
+gzip compressed data, was "nfs_estepona-0.3.0.tar", last modified: Fri May 24 00:27:18 2024, max compression
```

## Comparing `nfs-estepona-0.2.4.tar` & `nfs_estepona-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 estepona  (1000) estepona  (1000)        0 2021-09-27 19:50:56.764187 nfs-estepona-0.2.4/
--rw-r--r--   0 estepona  (1000) estepona  (1000)     1092 2021-09-19 15:43:55.000000 nfs-estepona-0.2.4/LICENSE
--rw-r--r--   0 estepona  (1000) estepona  (1000)     5450 2021-09-27 19:50:56.764187 nfs-estepona-0.2.4/PKG-INFO
--rw-r--r--   0 estepona  (1000) estepona  (1000)     4890 2021-09-27 19:36:15.000000 nfs-estepona-0.2.4/README.md
-drwxr-xr-x   0 estepona  (1000) estepona  (1000)        0 2021-09-27 19:50:56.754187 nfs-estepona-0.2.4/nfs_estepona.egg-info/
--rw-r--r--   0 estepona  (1000) estepona  (1000)     5450 2021-09-27 19:50:56.000000 nfs-estepona-0.2.4/nfs_estepona.egg-info/PKG-INFO
--rw-r--r--   0 estepona  (1000) estepona  (1000)      327 2021-09-27 19:50:56.000000 nfs-estepona-0.2.4/nfs_estepona.egg-info/SOURCES.txt
--rw-r--r--   0 estepona  (1000) estepona  (1000)        1 2021-09-27 19:50:56.000000 nfs-estepona-0.2.4/nfs_estepona.egg-info/dependency_links.txt
--rw-r--r--   0 estepona  (1000) estepona  (1000)       37 2021-09-27 19:50:56.000000 nfs-estepona-0.2.4/nfs_estepona.egg-info/entry_points.txt
--rw-r--r--   0 estepona  (1000) estepona  (1000)       33 2021-09-27 19:50:56.000000 nfs-estepona-0.2.4/nfs_estepona.egg-info/requires.txt
--rw-r--r--   0 estepona  (1000) estepona  (1000)        4 2021-09-27 19:50:56.000000 nfs-estepona-0.2.4/nfs_estepona.egg-info/top_level.txt
--rw-r--r--   0 estepona  (1000) estepona  (1000)        1 2021-09-26 04:16:32.000000 nfs-estepona-0.2.4/nfs_estepona.egg-info/zip-safe
--rw-r--r--   0 estepona  (1000) estepona  (1000)       90 2021-09-20 14:46:06.000000 nfs-estepona-0.2.4/pyproject.toml
--rw-r--r--   0 estepona  (1000) estepona  (1000)      739 2021-09-27 19:50:56.764187 nfs-estepona-0.2.4/setup.cfg
--rw-r--r--   0 estepona  (1000) estepona  (1000)       38 2021-09-21 02:32:29.000000 nfs-estepona-0.2.4/setup.py
-drwxr-xr-x   0 estepona  (1000) estepona  (1000)        0 2021-09-27 19:50:56.764187 nfs-estepona-0.2.4/src/
--rw-r--r--   0 estepona  (1000) estepona  (1000)        0 2021-09-20 14:50:03.000000 nfs-estepona-0.2.4/src/__init__.py
--rw-r--r--   0 estepona  (1000) estepona  (1000)     5944 2021-09-27 19:35:31.000000 nfs-estepona-0.2.4/src/app.py
+drwxrwxrwx   0        0        0        0 2024-05-24 00:27:18.820672 nfs_estepona-0.3.0/
+-rw-rw-rw-   0        0        0     1092 2024-05-23 18:49:46.000000 nfs_estepona-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     5701 2024-05-24 00:27:18.820672 nfs_estepona-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5079 2024-05-23 18:53:26.000000 nfs_estepona-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-24 00:27:18.819671 nfs_estepona-0.3.0/nfs_estepona.egg-info/
+-rw-rw-rw-   0        0        0     5701 2024-05-24 00:27:18.000000 nfs_estepona-0.3.0/nfs_estepona.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2024-05-24 00:27:18.000000 nfs_estepona-0.3.0/nfs_estepona.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-24 00:27:18.000000 nfs_estepona-0.3.0/nfs_estepona.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-24 00:27:18.000000 nfs_estepona-0.3.0/nfs_estepona.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2024-05-24 00:27:18.000000 nfs_estepona-0.3.0/nfs_estepona.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-24 00:27:18.000000 nfs_estepona-0.3.0/nfs_estepona.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-05-24 00:27:18.000000 nfs_estepona-0.3.0/nfs_estepona.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       93 2024-05-23 18:49:46.000000 nfs_estepona-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0      773 2024-05-24 00:27:18.822667 nfs_estepona-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0       41 2024-05-23 18:49:46.000000 nfs_estepona-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-24 00:27:18.817667 nfs_estepona-0.3.0/src/
+-rw-rw-rw-   0        0        0        0 2024-05-23 18:49:46.000000 nfs_estepona-0.3.0/src/__init__.py
+-rw-rw-rw-   0        0        0     6158 2024-05-23 18:49:46.000000 nfs_estepona-0.3.0/src/app.py
```

### Comparing `nfs-estepona-0.2.4/LICENSE` & `nfs_estepona-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nfs-estepona-0.2.4/PKG-INFO` & `nfs_estepona-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,142 +1,124 @@
-Metadata-Version: 2.1
-Name: nfs-estepona
-Version: 0.2.4
-Summary: a simple CLI tool to split a file into several smaller chunks at data level and merge them back
-Home-page: https://github.com/estepona/naive-file-splitter
-Author: Binghuan Zhang
-Author-email: esteponawondering@gmail.com
-License: MIT
-Keywords: CLI,file,split,utility
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<div align=center>
-  <h1>Naive File Splitter</h1>
-  <img src="https://img.shields.io/badge/nfs--estepona-0.2.*-blue"/>
-  <img src="https://img.shields.io/badge/python->=3.5-blueviolet"/>
-  <img src="https://img.shields.io/badge/click-7.0-brightgreen"/>
-  <img src="./assets/banner.png">
-</div>
-
-Naive File Splitter (NFS) is a simple CLI tool to split a file into several smaller chunks at data level and merge them back. It does not compress or transform the original file in any way. NFS only reads the file in binary stream and writes it into chunks whose number or size is given by the user.
-
-By having smaller chunks of a file instead of a large one, it allows easier and faster data download and upload, and bypasses file size limits inplaced by some cloud providers.
-
-NFS works with *any* file format.
-
-## Install
-
-NFS requires *Python >= 3.5*.
-
-`pip install nfs-estepona`
-
-Upon installation, a new `nfs` binary will be added to system's path.
-
-## Command
-
-### Split
-
-#### Usage
-
-`nfs split [OPTIONS] SRC`
-
-Split the file into several chunks by specifying EITHER:
-- number of chunks with `--chunk` flag
-- size of each chunk with `--size-per-chunk` flag, and the number of chunks is calculated accordingly, i.e. *5kb*, *10mb*, *1gb*
-
-`SRC` is the filepath.
-
-Options:
-- `-c, --chunk`, *INTEGER*, number of chunks to output
-- `-s, --size`, *TEXT*, size of each chunk
-
-#### Example
-
-##### Split a file into 5 chunks
-
-`nfs split -c 5 /mnt/c/Users/estep/Videos/Captures/mgs1.mp4`
-
-```bash
-$ nfs split -c 5 /mnt/c/Users/estep/Videos/Captures/mgs1.mp4
-100%|█████████████████████████████████████████████████████████████████████████████████████| 5/5 [00:00<00:00, 37.28it/s]
-splitted /mnt/c/Users/estep/Videos/Captures/mgs1.mp4 into 5 chunks
-```
-
-##### Split a file into chunks of 25MB each
-
-`nfs split -s 25mb /mnt/c/Users/estep/Videos/Captures/medium.webm`
-
-```bash
-$ nfs split -s 25mb /mnt/c/Users/estep/Videos/Captures/medium.webm
-100%|███████████████████████████████████████████████████████████████████████████████████| 18/18 [00:08<00:00,  2.00it/s]
-splitted /mnt/c/Users/estep/Videos/Captures/medium.webm into 18 chunks
-```
-
-### Merge
-
-#### Usage
-
-`nfs merge [OPTIONS] SRC`
-
-Merge NFS splitted file chunks into one.
-
-NFS splitted file chunks can be identified with *.c1*, *.c2* (etc.) appended to the end of original file's name (path).
-
-If multiple files that are splitted are found, user can choose which one to merge.
-
-If the original file exists under the same directory, a new file with *_copy* appended to the filename will be created.
-
-`SRC` is the directory path that contains (parent to) splitted file chunks.
-
-Options:
-- `-r, --remove`, remove splitted file chunks after merge
-
-#### Example
-
-##### Merge splitted file chunks into one
-
-`nfs merge /mnt/c/Users/estep/Videos/Captures`
-
-```bash
-$ nfs merge /mnt/c/Users/estep/Videos/Captures
-100%|█████████████████████████████████████████████████████████████████████████████████████| 5/5 [00:00<00:00, 50.87it/s]
-merged splitted file chunks to /mnt/c/Users/estep/Videos/Captures/mgs1_copy.mp4
-```
-##### Merge splitted file chunks into one and remove chunks
-
-`nfs merge -r /mnt/c/Users/estep/Videos/Captures`
-
-```bash
-$ nfs merge -r /mnt/c/Users/estep/Videos/Captures
-100%|█████████████████████████████████████████████████████████████████████████████████████| 5/5 [00:00<00:00, 49.96it/s]
-merged splitted file chunks to /mnt/c/Users/estep/Videos/Captures/mgs1_copy.mp4
-removed splitted file chunks
-```
-
-##### Merge splitted file chunks into one where chunks of other files exist
-
-`nfs merge /mnt/c/Users/estep/Videos/Captures`
-
-```bash
-$ nfs merge /mnt/c/Users/estep/Videos/Captures
-found 2 splitted file chunks, choose one to proceed:
-1 - dup.mov
-2 - mgs1.mp4
-your answer: 2
-100%|█████████████████████████████████████████████████████████████████████████████████████| 5/5 [00:00<00:00, 47.95it/s]
-merged splitted file chunks to /mnt/c/Users/estep/Videos/Captures/mgs1_copy.mp4
-```
-
-## Author
-
-[Binghuan Zhang](https://github.com/estepona) - esteponawondering@gmail.com
-
-## LICENSE
-
-MIT
-
-
+<div align=center>
+  <h1>Naive File Splitter</h1>
+  <img src="https://img.shields.io/badge/nfs--estepona-0.2.*-blue"/>
+  <img src="https://img.shields.io/badge/python->=3.5-blueviolet"/>
+  <img src="https://img.shields.io/badge/click-7.0-brightgreen"/>
+  <img src="./assets/banner.png">
+</div>
+
+Naive File Splitter is a simple CLI tool to split a file into several smaller chunks at data level and merge them back. It does not compress or transform the original file in any way. NFS only reads the file in binary stream and writes it into chunks whose number or size is given by the user.
+
+By having smaller chunks of a file instead of a large one, it allows easier and faster data download and upload, and bypasses file size limits inplaced by some cloud providers.
+
+Naive File Splitter works with *any* file format.
+
+## Install
+
+Naive File Splitter requires *Python >= 3.5*.
+
+`pip install nfs-estepona`
+
+Upon installation, a new `nsplit` binary will be added to system's path.
+
+## Command
+
+### Split
+
+#### Usage
+
+`nsplit split [OPTIONS] SRC`
+
+Split the file into several chunks by specifying EITHER:
+- number of chunks with `--chunk` flag
+- size of each chunk with `--size-per-chunk` flag, and the number of chunks is calculated accordingly, i.e. *5kb*, *10mb*, *1gb*
+
+`SRC` is the filepath.
+
+Options:
+- `-c, --chunk`, *INTEGER*, number of chunks to output
+- `-s, --size`, *TEXT*, size of each chunk
+
+#### Example
+
+##### Split a file into 5 chunks
+
+`nsplit split -c 5 /mnt/c/Users/estep/Videos/Captures/mgs1.mp4`
+
+```bash
+$ nsplit split -c 5 /mnt/c/Users/estep/Videos/Captures/mgs1.mp4
+100%|█████████████████████████████████████████████████████████████████████████████████████| 5/5 [00:00<00:00, 37.28it/s]
+splitted /mnt/c/Users/estep/Videos/Captures/mgs1.mp4 into 5 chunks
+```
+
+##### Split a file into chunks of 25MB each
+
+`nsplit split -s 25mb /mnt/c/Users/estep/Videos/Captures/medium.webm`
+
+```bash
+$ nsplit split -s 25mb /mnt/c/Users/estep/Videos/Captures/medium.webm
+100%|███████████████████████████████████████████████████████████████████████████████████| 18/18 [00:08<00:00,  2.00it/s]
+splitted /mnt/c/Users/estep/Videos/Captures/medium.webm into 18 chunks
+```
+
+### Merge
+
+#### Usage
+
+`nsplit merge [OPTIONS] SRC`
+
+Merge NFS splitted file chunks into one.
+
+NFS splitted file chunks can be identified with *.c1*, *.c2* (etc.) appended to the end of original file's name (path).
+
+If multiple files that are splitted are found, user can choose which one to merge.
+
+If the original file exists under the same directory, a new file with *_copy* appended to the filename will be created.
+
+`SRC` is the directory path that contains (parent to) splitted file chunks.
+
+Options:
+- `-r, --remove`, remove splitted file chunks after merge
+
+#### Example
+
+##### Merge splitted file chunks into one
+
+`nsplit merge /mnt/c/Users/estep/Videos/Captures`
+
+```bash
+$ nsplit merge /mnt/c/Users/estep/Videos/Captures
+100%|█████████████████████████████████████████████████████████████████████████████████████| 5/5 [00:00<00:00, 50.87it/s]
+merged splitted file chunks to /mnt/c/Users/estep/Videos/Captures/mgs1_copy.mp4
+```
+##### Merge splitted file chunks into one and remove chunks
+
+`nsplit merge -r /mnt/c/Users/estep/Videos/Captures`
+
+```bash
+$ nsplit merge -r /mnt/c/Users/estep/Videos/Captures
+100%|█████████████████████████████████████████████████████████████████████████████████████| 5/5 [00:00<00:00, 49.96it/s]
+merged splitted file chunks to /mnt/c/Users/estep/Videos/Captures/mgs1_copy.mp4
+removed splitted file chunks
+```
+
+##### Merge splitted file chunks into one where chunks of other files exist
+
+`nsplit merge /mnt/c/Users/estep/Videos/Captures`
+
+```bash
+$ nsplit merge /mnt/c/Users/estep/Videos/Captures
+found 2 splitted file chunks, choose one to proceed:
+1 - dup.mov
+2 - mgs1.mp4
+your answer: 2
+100%|█████████████████████████████████████████████████████████████████████████████████████| 5/5 [00:00<00:00, 47.95it/s]
+merged splitted file chunks to /mnt/c/Users/estep/Videos/Captures/mgs1_copy.mp4
+```
+
+## Author
+
+[Binghuan Zhang](https://github.com/estepona) - esteponawondering@gmail.com
+
+## LICENSE
+
+MIT
```

### Comparing `nfs-estepona-0.2.4/nfs_estepona.egg-info/PKG-INFO` & `nfs_estepona-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,142 +1,142 @@
-Metadata-Version: 2.1
-Name: nfs-estepona
-Version: 0.2.4
-Summary: a simple CLI tool to split a file into several smaller chunks at data level and merge them back
-Home-page: https://github.com/estepona/naive-file-splitter
-Author: Binghuan Zhang
-Author-email: esteponawondering@gmail.com
-License: MIT
-Keywords: CLI,file,split,utility
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<div align=center>
-  <h1>Naive File Splitter</h1>
-  <img src="https://img.shields.io/badge/nfs--estepona-0.2.*-blue"/>
-  <img src="https://img.shields.io/badge/python->=3.5-blueviolet"/>
-  <img src="https://img.shields.io/badge/click-7.0-brightgreen"/>
-  <img src="./assets/banner.png">
-</div>
-
-Naive File Splitter (NFS) is a simple CLI tool to split a file into several smaller chunks at data level and merge them back. It does not compress or transform the original file in any way. NFS only reads the file in binary stream and writes it into chunks whose number or size is given by the user.
-
-By having smaller chunks of a file instead of a large one, it allows easier and faster data download and upload, and bypasses file size limits inplaced by some cloud providers.
-
-NFS works with *any* file format.
-
-## Install
-
-NFS requires *Python >= 3.5*.
-
-`pip install nfs-estepona`
-
-Upon installation, a new `nfs` binary will be added to system's path.
-
-## Command
-
-### Split
-
-#### Usage
-
-`nfs split [OPTIONS] SRC`
-
-Split the file into several chunks by specifying EITHER:
-- number of chunks with `--chunk` flag
-- size of each chunk with `--size-per-chunk` flag, and the number of chunks is calculated accordingly, i.e. *5kb*, *10mb*, *1gb*
-
-`SRC` is the filepath.
-
-Options:
-- `-c, --chunk`, *INTEGER*, number of chunks to output
-- `-s, --size`, *TEXT*, size of each chunk
-
-#### Example
-
-##### Split a file into 5 chunks
-
-`nfs split -c 5 /mnt/c/Users/estep/Videos/Captures/mgs1.mp4`
-
-```bash
-$ nfs split -c 5 /mnt/c/Users/estep/Videos/Captures/mgs1.mp4
-100%|█████████████████████████████████████████████████████████████████████████████████████| 5/5 [00:00<00:00, 37.28it/s]
-splitted /mnt/c/Users/estep/Videos/Captures/mgs1.mp4 into 5 chunks
-```
-
-##### Split a file into chunks of 25MB each
-
-`nfs split -s 25mb /mnt/c/Users/estep/Videos/Captures/medium.webm`
-
-```bash
-$ nfs split -s 25mb /mnt/c/Users/estep/Videos/Captures/medium.webm
-100%|███████████████████████████████████████████████████████████████████████████████████| 18/18 [00:08<00:00,  2.00it/s]
-splitted /mnt/c/Users/estep/Videos/Captures/medium.webm into 18 chunks
-```
-
-### Merge
-
-#### Usage
-
-`nfs merge [OPTIONS] SRC`
-
-Merge NFS splitted file chunks into one.
-
-NFS splitted file chunks can be identified with *.c1*, *.c2* (etc.) appended to the end of original file's name (path).
-
-If multiple files that are splitted are found, user can choose which one to merge.
-
-If the original file exists under the same directory, a new file with *_copy* appended to the filename will be created.
-
-`SRC` is the directory path that contains (parent to) splitted file chunks.
-
-Options:
-- `-r, --remove`, remove splitted file chunks after merge
-
-#### Example
-
-##### Merge splitted file chunks into one
-
-`nfs merge /mnt/c/Users/estep/Videos/Captures`
-
-```bash
-$ nfs merge /mnt/c/Users/estep/Videos/Captures
-100%|█████████████████████████████████████████████████████████████████████████████████████| 5/5 [00:00<00:00, 50.87it/s]
-merged splitted file chunks to /mnt/c/Users/estep/Videos/Captures/mgs1_copy.mp4
-```
-##### Merge splitted file chunks into one and remove chunks
-
-`nfs merge -r /mnt/c/Users/estep/Videos/Captures`
-
-```bash
-$ nfs merge -r /mnt/c/Users/estep/Videos/Captures
-100%|█████████████████████████████████████████████████████████████████████████████████████| 5/5 [00:00<00:00, 49.96it/s]
-merged splitted file chunks to /mnt/c/Users/estep/Videos/Captures/mgs1_copy.mp4
-removed splitted file chunks
-```
-
-##### Merge splitted file chunks into one where chunks of other files exist
-
-`nfs merge /mnt/c/Users/estep/Videos/Captures`
-
-```bash
-$ nfs merge /mnt/c/Users/estep/Videos/Captures
-found 2 splitted file chunks, choose one to proceed:
-1 - dup.mov
-2 - mgs1.mp4
-your answer: 2
-100%|█████████████████████████████████████████████████████████████████████████████████████| 5/5 [00:00<00:00, 47.95it/s]
-merged splitted file chunks to /mnt/c/Users/estep/Videos/Captures/mgs1_copy.mp4
-```
-
-## Author
-
-[Binghuan Zhang](https://github.com/estepona) - esteponawondering@gmail.com
-
-## LICENSE
-
-MIT
-
-
+Metadata-Version: 2.1
+Name: nfs-estepona
+Version: 0.3.0
+Summary: a simple CLI tool to split a file into several smaller chunks at data level and merge them back
+Home-page: https://github.com/estepona/naive-file-splitter
+Author: Binghuan Zhang
+Author-email: esteponawondering@gmail.com
+License: MIT
+Keywords: CLI,file,split,utility
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: click
+Requires-Dist: tqdm
+
+<div align=center>
+  <h1>Naive File Splitter</h1>
+  <img src="https://img.shields.io/badge/nfs--estepona-0.2.*-blue"/>
+  <img src="https://img.shields.io/badge/python->=3.5-blueviolet"/>
+  <img src="https://img.shields.io/badge/click-7.0-brightgreen"/>
+  <img src="./assets/banner.png">
+</div>
+
+Naive File Splitter is a simple CLI tool to split a file into several smaller chunks at data level and merge them back. It does not compress or transform the original file in any way. NFS only reads the file in binary stream and writes it into chunks whose number or size is given by the user.
+
+By having smaller chunks of a file instead of a large one, it allows easier and faster data download and upload, and bypasses file size limits inplaced by some cloud providers.
+
+Naive File Splitter works with *any* file format.
+
+## Install
+
+Naive File Splitter requires *Python >= 3.5*.
+
+`pip install nfs-estepona`
+
+Upon installation, a new `nsplit` binary will be added to system's path.
+
+## Command
+
+### Split
+
+#### Usage
+
+`nsplit split [OPTIONS] SRC`
+
+Split the file into several chunks by specifying EITHER:
+- number of chunks with `--chunk` flag
+- size of each chunk with `--size-per-chunk` flag, and the number of chunks is calculated accordingly, i.e. *5kb*, *10mb*, *1gb*
+
+`SRC` is the filepath.
+
+Options:
+- `-c, --chunk`, *INTEGER*, number of chunks to output
+- `-s, --size`, *TEXT*, size of each chunk
+
+#### Example
+
+##### Split a file into 5 chunks
+
+`nsplit split -c 5 /mnt/c/Users/estep/Videos/Captures/mgs1.mp4`
+
+```bash
+$ nsplit split -c 5 /mnt/c/Users/estep/Videos/Captures/mgs1.mp4
+100%|█████████████████████████████████████████████████████████████████████████████████████| 5/5 [00:00<00:00, 37.28it/s]
+splitted /mnt/c/Users/estep/Videos/Captures/mgs1.mp4 into 5 chunks
+```
+
+##### Split a file into chunks of 25MB each
+
+`nsplit split -s 25mb /mnt/c/Users/estep/Videos/Captures/medium.webm`
+
+```bash
+$ nsplit split -s 25mb /mnt/c/Users/estep/Videos/Captures/medium.webm
+100%|███████████████████████████████████████████████████████████████████████████████████| 18/18 [00:08<00:00,  2.00it/s]
+splitted /mnt/c/Users/estep/Videos/Captures/medium.webm into 18 chunks
+```
+
+### Merge
+
+#### Usage
+
+`nsplit merge [OPTIONS] SRC`
+
+Merge NFS splitted file chunks into one.
+
+NFS splitted file chunks can be identified with *.c1*, *.c2* (etc.) appended to the end of original file's name (path).
+
+If multiple files that are splitted are found, user can choose which one to merge.
+
+If the original file exists under the same directory, a new file with *_copy* appended to the filename will be created.
+
+`SRC` is the directory path that contains (parent to) splitted file chunks.
+
+Options:
+- `-r, --remove`, remove splitted file chunks after merge
+
+#### Example
+
+##### Merge splitted file chunks into one
+
+`nsplit merge /mnt/c/Users/estep/Videos/Captures`
+
+```bash
+$ nsplit merge /mnt/c/Users/estep/Videos/Captures
+100%|█████████████████████████████████████████████████████████████████████████████████████| 5/5 [00:00<00:00, 50.87it/s]
+merged splitted file chunks to /mnt/c/Users/estep/Videos/Captures/mgs1_copy.mp4
+```
+##### Merge splitted file chunks into one and remove chunks
+
+`nsplit merge -r /mnt/c/Users/estep/Videos/Captures`
+
+```bash
+$ nsplit merge -r /mnt/c/Users/estep/Videos/Captures
+100%|█████████████████████████████████████████████████████████████████████████████████████| 5/5 [00:00<00:00, 49.96it/s]
+merged splitted file chunks to /mnt/c/Users/estep/Videos/Captures/mgs1_copy.mp4
+removed splitted file chunks
+```
+
+##### Merge splitted file chunks into one where chunks of other files exist
+
+`nsplit merge /mnt/c/Users/estep/Videos/Captures`
+
+```bash
+$ nsplit merge /mnt/c/Users/estep/Videos/Captures
+found 2 splitted file chunks, choose one to proceed:
+1 - dup.mov
+2 - mgs1.mp4
+your answer: 2
+100%|█████████████████████████████████████████████████████████████████████████████████████| 5/5 [00:00<00:00, 47.95it/s]
+merged splitted file chunks to /mnt/c/Users/estep/Videos/Captures/mgs1_copy.mp4
+```
+
+## Author
+
+[Binghuan Zhang](https://github.com/estepona) - esteponawondering@gmail.com
+
+## LICENSE
+
+MIT
```

### Comparing `nfs-estepona-0.2.4/setup.cfg` & `nfs_estepona-0.3.0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,49 @@
-00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
-00000010: 3d20 6e66 732d 6573 7465 706f 6e61 0a76  = nfs-estepona.v
-00000020: 6572 7369 6f6e 203d 2030 2e32 2e34 0a75  ersion = 0.2.4.u
-00000030: 726c 203d 2068 7474 7073 3a2f 2f67 6974  rl = https://git
-00000040: 6875 622e 636f 6d2f 6573 7465 706f 6e61  hub.com/estepona
-00000050: 2f6e 6169 7665 2d66 696c 652d 7370 6c69  /naive-file-spli
-00000060: 7474 6572 0a64 6573 6372 6970 7469 6f6e  tter.description
-00000070: 203d 2061 2073 696d 706c 6520 434c 4920   = a simple CLI 
-00000080: 746f 6f6c 2074 6f20 7370 6c69 7420 6120  tool to split a 
-00000090: 6669 6c65 2069 6e74 6f20 7365 7665 7261  file into severa
-000000a0: 6c20 736d 616c 6c65 7220 6368 756e 6b73  l smaller chunks
-000000b0: 2061 7420 6461 7461 206c 6576 656c 2061   at data level a
-000000c0: 6e64 206d 6572 6765 2074 6865 6d20 6261  nd merge them ba
-000000d0: 636b 0a6c 6f6e 675f 6465 7363 7269 7074  ck.long_descript
-000000e0: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
-000000f0: 4d45 2e6d 640a 6c6f 6e67 5f64 6573 6372  ME.md.long_descr
-00000100: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
-00000110: 7970 6520 3d20 7465 7874 2f6d 6172 6b64  ype = text/markd
-00000120: 6f77 6e0a 6175 7468 6f72 203d 2042 696e  own.author = Bin
-00000130: 6768 7561 6e20 5a68 616e 670a 6175 7468  ghuan Zhang.auth
-00000140: 6f72 5f65 6d61 696c 203d 2065 7374 6570  or_email = estep
-00000150: 6f6e 6177 6f6e 6465 7269 6e67 4067 6d61  onawondering@gma
-00000160: 696c 2e63 6f6d 0a6b 6579 776f 7264 7320  il.com.keywords 
-00000170: 3d20 434c 492c 2066 696c 652c 2073 706c  = CLI, file, spl
-00000180: 6974 2c20 7574 696c 6974 790a 6c69 6365  it, utility.lice
-00000190: 6e73 6520 3d20 4d49 540a 636c 6173 7369  nse = MIT.classi
-000001a0: 6669 6572 7320 3d20 0a09 5072 6f67 7261  fiers = ..Progra
-000001b0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000001c0: 3a20 5079 7468 6f6e 203a 3a20 330a 094c  : Python :: 3..L
-000001d0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
-000001e0: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
-000001f0: 6365 6e73 650a 094f 7065 7261 7469 6e67  cense..Operating
-00000200: 2053 7973 7465 6d20 3a3a 204f 5320 496e   System :: OS In
-00000210: 6465 7065 6e64 656e 740a 0a5b 6f70 7469  dependent..[opti
-00000220: 6f6e 735d 0a7a 6970 5f73 6166 6520 3d20  ons].zip_safe = 
-00000230: 5472 7565 0a70 6163 6b61 6765 7320 3d20  True.packages = 
-00000240: 7372 630a 696e 7374 616c 6c5f 7265 7175  src.install_requ
-00000250: 6972 6573 203d 200a 0963 6c69 636b 0a09  ires = ..click..
-00000260: 7471 646d 0a09 7079 7468 6f6e 5f76 6572  tqdm..python_ver
-00000270: 7369 6f6e 203e 3d20 2233 2e35 220a 0a5b  sion >= "3.5"..[
-00000280: 6f70 7469 6f6e 732e 656e 7472 795f 706f  options.entry_po
-00000290: 696e 7473 5d0a 636f 6e73 6f6c 655f 7363  ints].console_sc
-000002a0: 7269 7074 7320 3d20 0a09 6e66 7320 3d20  ripts = ..nfs = 
-000002b0: 7372 632e 6170 703a 636c 690a 0a5b 6567  src.app:cli..[eg
-000002c0: 675f 696e 666f 5d0a 7461 675f 6275 696c  g_info].tag_buil
-000002d0: 6420 3d20 0a74 6167 5f64 6174 6520 3d20  d = .tag_date = 
-000002e0: 300a 0a                                  0..
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
+00000010: 203d 206e 6673 2d65 7374 6570 6f6e 610d   = nfs-estepona.
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e33 2e30  .version = 0.3.0
+00000030: 0d0a 7572 6c20 3d20 6874 7470 733a 2f2f  ..url = https://
+00000040: 6769 7468 7562 2e63 6f6d 2f65 7374 6570  github.com/estep
+00000050: 6f6e 612f 6e61 6976 652d 6669 6c65 2d73  ona/naive-file-s
+00000060: 706c 6974 7465 720d 0a64 6573 6372 6970  plitter..descrip
+00000070: 7469 6f6e 203d 2061 2073 696d 706c 6520  tion = a simple 
+00000080: 434c 4920 746f 6f6c 2074 6f20 7370 6c69  CLI tool to spli
+00000090: 7420 6120 6669 6c65 2069 6e74 6f20 7365  t a file into se
+000000a0: 7665 7261 6c20 736d 616c 6c65 7220 6368  veral smaller ch
+000000b0: 756e 6b73 2061 7420 6461 7461 206c 6576  unks at data lev
+000000c0: 656c 2061 6e64 206d 6572 6765 2074 6865  el and merge the
+000000d0: 6d20 6261 636b 0d0a 6c6f 6e67 5f64 6573  m back..long_des
+000000e0: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
+000000f0: 2052 4541 444d 452e 6d64 0d0a 6c6f 6e67   README.md..long
+00000100: 5f64 6573 6372 6970 7469 6f6e 5f63 6f6e  _description_con
+00000110: 7465 6e74 5f74 7970 6520 3d20 7465 7874  tent_type = text
+00000120: 2f6d 6172 6b64 6f77 6e0d 0a61 7574 686f  /markdown..autho
+00000130: 7220 3d20 4269 6e67 6875 616e 205a 6861  r = Binghuan Zha
+00000140: 6e67 0d0a 6175 7468 6f72 5f65 6d61 696c  ng..author_email
+00000150: 203d 2065 7374 6570 6f6e 6177 6f6e 6465   = esteponawonde
+00000160: 7269 6e67 4067 6d61 696c 2e63 6f6d 0d0a  ring@gmail.com..
+00000170: 6b65 7977 6f72 6473 203d 2043 4c49 2c20  keywords = CLI, 
+00000180: 6669 6c65 2c20 7370 6c69 742c 2075 7469  file, split, uti
+00000190: 6c69 7479 0d0a 6c69 6365 6e73 6520 3d20  lity..license = 
+000001a0: 4d49 540d 0a63 6c61 7373 6966 6965 7273  MIT..classifiers
+000001b0: 203d 200d 0a09 5072 6f67 7261 6d6d 696e   = ...Programmin
+000001c0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000001d0: 7468 6f6e 203a 3a20 330d 0a09 4c69 6365  thon :: 3...Lice
+000001e0: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+000001f0: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
+00000200: 7365 0d0a 094f 7065 7261 7469 6e67 2053  se...Operating S
+00000210: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
+00000220: 7065 6e64 656e 740d 0a0d 0a5b 6f70 7469  pendent....[opti
+00000230: 6f6e 735d 0d0a 7a69 705f 7361 6665 203d  ons]..zip_safe =
+00000240: 2054 7275 650d 0a70 6163 6b61 6765 7320   True..packages 
+00000250: 3d20 7372 630d 0a70 7974 686f 6e5f 7265  = src..python_re
+00000260: 7175 6972 6573 203d 203e 3d33 2e35 0d0a  quires = >=3.5..
+00000270: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
+00000280: 203d 200d 0a09 636c 6963 6b0d 0a09 7471   = ...click...tq
+00000290: 646d 0d0a 0d0a 5b6f 7074 696f 6e73 2e65  dm....[options.e
+000002a0: 6e74 7279 5f70 6f69 6e74 735d 0d0a 636f  ntry_points]..co
+000002b0: 6e73 6f6c 655f 7363 7269 7074 7320 3d20  nsole_scripts = 
+000002c0: 0d0a 096e 7370 6c69 7420 3d20 7372 632e  ...nsplit = src.
+000002d0: 6170 703a 636c 690d 0a0d 0a5b 6567 675f  app:cli....[egg_
+000002e0: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
+000002f0: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
+00000300: 300d 0a0d 0a                             0....
```

### Comparing `nfs-estepona-0.2.4/src/app.py` & `nfs_estepona-0.3.0/src/app.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,214 +1,214 @@
-import os
-from collections import defaultdict
-from os.path import abspath, normpath
-from pathlib import Path
-
-import click
-import tqdm
-
-BYTES_PER_KB = 1_024
-BYTES_PER_MB = 1_048_576
-BYTES_PER_GB = 1_073_741_824
-
-MAX_BUFFER_SIZE = BYTES_PER_MB * 16
-
-KB_SUFFIX_LOWERCASE = 'kb'
-MB_SUFFIX_LOWERCASE = 'mb'
-GB_SUFFIX_LOWERCASE = 'gb'
-
-SPLITTED_CHUNKS_PREFIX = 'c'
-SPLITTED_CHUNKS_PATTERN = '*.*.c*'
-
-
-def get_path(path: str) -> Path:
-  return Path(abspath(normpath(path)))
-
-
-def read_in_chunks(file_object, chunk_size: int):
-  while True:
-    data = file_object.read(chunk_size)
-    if not data:
-      yield None
-      break
-
-    yield data
-
-
-@click.group()
-def cli():
-  return
-
-
-def split_(src: str, chunk: int, size: str):
-  if (not chunk) and (not size):
-    click.echo('either --chunk or --size should be provided')
-    return
-  if chunk and chunk <= 1:
-    click.echo('--chunk has to be greater than 1')
-    return
-  if size:
-    if (len(size) <= 2) or\
-       (size[-2:].lower() not in {KB_SUFFIX_LOWERCASE, MB_SUFFIX_LOWERCASE, GB_SUFFIX_LOWERCASE}):
-      click.echo('--size has to end with kb/KB, mb/MB, or gb/GB')
-      return
-    elif int(size[:-2]) <= 0:
-      click.echo('--size has to be greater than 0')
-      return
-
-  if chunk and size:
-    click.echo('both --chunk and --size provided, using --chunk...')
-  use_chunk = bool(chunk)
-
-  src_size = os.stat(src).st_size
-
-  if use_chunk:
-    spc = (src_size // chunk) if (src_size % chunk == 0) else (src_size//chunk + 1)
-  else:
-    spc_num = int(size[:-2])
-    spc_unit = size[-2:].lower()
-
-    if spc_unit == KB_SUFFIX_LOWERCASE:
-      spc = spc_num * BYTES_PER_KB
-    elif spc_unit == MB_SUFFIX_LOWERCASE:
-      spc = spc_num * BYTES_PER_MB
-    elif spc_unit == GB_SUFFIX_LOWERCASE:
-      spc = spc_num * BYTES_PER_GB
-
-    chunk = (src_size // spc) if (src_size % spc == 0) else (src_size//spc + 1)
-
-  chunk_size = min(spc, MAX_BUFFER_SIZE)
-  chunk_index = 1
-  cur_l = 0
-
-  src_file = open(src, 'rb')
-  dst_file = open(f'{src}.{SPLITTED_CHUNKS_PREFIX}{chunk_index}', 'wb')
-  pbar = tqdm.tqdm(total=chunk)
-
-  for cnk in read_in_chunks(src_file, chunk_size):
-    if cur_l == spc:
-      dst_file.close()
-      pbar.update(1)
-
-      dst_file = open(f'{src}.{SPLITTED_CHUNKS_PREFIX}{chunk_index + 1}', 'wb')
-
-      cur_l = 0
-      chunk_index += 1
-
-    if cnk is not None:
-      cnk_l = len(cnk)
-      if cur_l < spc:
-        if cur_l + cnk_l > spc:
-          dst_file.write(cnk[:spc - cur_l])
-          dst_file.close()
-          pbar.update(1)
-
-          dst_file = open(f'{src}.{SPLITTED_CHUNKS_PREFIX}{chunk_index + 1}', 'wb')
-          dst_file.write(cnk[spc - cur_l:])
-
-          cur_l = cnk_l - (spc-cur_l)
-          chunk_index += 1
-        else:
-          dst_file.write(cnk)
-          cur_l += cnk_l
-
-  src_file.close()
-  if dst_file:
-    if dst_file.tell() == 0:
-      dst_file.close()
-      os.remove(dst_file.name)
-    else:
-      dst_file.close()
-      pbar.update(1)
-  pbar.close()
-  click.echo(f'splitted {src_file.name} into {chunk} chunks')
-
-
-@cli.command()
-@click.argument('src', nargs=1, type=click.Path(exists=True))
-@click.option('-c', '--chunk', type=int, help='number of chunks to output')
-@click.option('-s', '--size', type=str, help='size of each chunk')
-def split(src: str, chunk: int, size: str):
-  """ Split the file into several chunks by specifying EITHER:\n
-  - number of chunks with --chunk flag\n
-  - size of each chunk with --size flag, and the number of chunks is calculated accordingly, i.e. 5kb, 10mb, 1gb
-
-  SRC is the filepath.
-  """
-  split_(src, chunk, size)
-
-
-def merge_(src: str, remove: bool):
-  dirpath = get_path(src)
-
-  all_chunks = list(dirpath.glob(SPLITTED_CHUNKS_PATTERN))
-  if not all_chunks:
-    click.echo('no splitted file chunks found')
-    return
-
-  files = defaultdict(list)
-  for c in all_chunks:
-    name = c.stem
-    files[name].append(c)
-
-  file_names = list(files.keys())
-  if len(file_names) >= 2:
-    question = f'found {len(file_names)} splitted file chunks, choose one to proceed:\n'
-    for i, v in enumerate(file_names):
-      question += f'{i+1} - {v}\n'
-    question += 'your answer'
-
-    file_choice = click.prompt(question, type=int)
-    while (file_choice > len(file_names)) or (file_choice < 1):
-      file_choice = click.prompt('incorrect input, please try again', type=int)
-    file = file_names[file_choice - 1]
-  else:
-    file = file_names[0]
-
-  chunks = sorted(files[file], key=lambda x: int(x.suffix.split(SPLITTED_CHUNKS_PREFIX)[1]))
-  pbar = tqdm.tqdm(total=len(chunks))
-
-  dst = chunks[0].parent / chunks[0].stem
-  if dst.is_file():
-    filename = chunks[0].stem.split('.')[0]
-    extension = chunks[0].stem.split('.')[1]
-    dst = chunks[0].parent / f'{filename}_copy.{extension}'
-
-  dst_file = open(dst, 'wb')
-  for c in chunks:
-    p_size = os.stat(c).st_size
-    with open(c, 'rb') as f:
-      for cnk in read_in_chunks(f, min(p_size, MAX_BUFFER_SIZE)):
-        if cnk:
-          dst_file.write(cnk)
-    pbar.update(1)
-
-  dst_file.close()
-  pbar.close()
-  click.echo(f'merged splitted file chunks to {dst}')
-
-  if remove:
-    for c in chunks:
-      os.remove(c)
-    click.echo('removed splitted file chunks')
-
-
-@cli.command()
-@click.argument('src', nargs=1, type=click.Path(exists=True))
-@click.option('-r', '--remove', default=False, is_flag=True, help='remove splitted file chunks after merge')
-def merge(src: str, remove: bool):
-  """ Merge NFS splitted file chunks into one.
-
-  NFS splitted file chunks can be identified with '.c1', '.c2' (etc.) appended to the end of original file's name (path).
-
-  If multiple files that are splitted are found, user can choose which one to merge.
-
-  If the original file exists under the same directory, a new file with '_copy' appended to the filename will be created.
-
-  SRC is the directory path that contains (parent to) splitted file chunks.
-  """
-  merge_(src, remove)
-
-
-if __name__ == '__main__':
-  # pylint: disable=no-value-for-parameter
-  cli()
+import os
+from collections import defaultdict
+from os.path import abspath, normpath
+from pathlib import Path
+
+import click
+import tqdm
+
+BYTES_PER_KB = 1_024
+BYTES_PER_MB = 1_048_576
+BYTES_PER_GB = 1_073_741_824
+
+MAX_BUFFER_SIZE = BYTES_PER_MB * 16
+
+KB_SUFFIX_LOWERCASE = 'kb'
+MB_SUFFIX_LOWERCASE = 'mb'
+GB_SUFFIX_LOWERCASE = 'gb'
+
+SPLITTED_CHUNKS_PREFIX = 'c'
+SPLITTED_CHUNKS_PATTERN = '*.*.c*'
+
+
+def get_path(path: str) -> Path:
+  return Path(abspath(normpath(path)))
+
+
+def read_in_chunks(file_object, chunk_size: int):
+  while True:
+    data = file_object.read(chunk_size)
+    if not data:
+      yield None
+      break
+
+    yield data
+
+
+@click.group()
+def cli():
+  return
+
+
+def split_(src: str, chunk: int, size: str):
+  if (not chunk) and (not size):
+    click.echo('either --chunk or --size should be provided')
+    return
+  if chunk and chunk <= 1:
+    click.echo('--chunk has to be greater than 1')
+    return
+  if size:
+    if (len(size) <= 2) or\
+       (size[-2:].lower() not in {KB_SUFFIX_LOWERCASE, MB_SUFFIX_LOWERCASE, GB_SUFFIX_LOWERCASE}):
+      click.echo('--size has to end with kb/KB, mb/MB, or gb/GB')
+      return
+    elif int(size[:-2]) <= 0:
+      click.echo('--size has to be greater than 0')
+      return
+
+  if chunk and size:
+    click.echo('both --chunk and --size provided, using --chunk...')
+  use_chunk = bool(chunk)
+
+  src_size = os.stat(src).st_size
+
+  if use_chunk:
+    spc = (src_size // chunk) if (src_size % chunk == 0) else (src_size//chunk + 1)
+  else:
+    spc_num = int(size[:-2])
+    spc_unit = size[-2:].lower()
+
+    if spc_unit == KB_SUFFIX_LOWERCASE:
+      spc = spc_num * BYTES_PER_KB
+    elif spc_unit == MB_SUFFIX_LOWERCASE:
+      spc = spc_num * BYTES_PER_MB
+    elif spc_unit == GB_SUFFIX_LOWERCASE:
+      spc = spc_num * BYTES_PER_GB
+
+    chunk = (src_size // spc) if (src_size % spc == 0) else (src_size//spc + 1)
+
+  chunk_size = min(spc, MAX_BUFFER_SIZE)
+  chunk_index = 1
+  cur_l = 0
+
+  src_file = open(src, 'rb')
+  dst_file = open(f'{src}.{SPLITTED_CHUNKS_PREFIX}{chunk_index}', 'wb')
+  pbar = tqdm.tqdm(total=chunk)
+
+  for cnk in read_in_chunks(src_file, chunk_size):
+    if cur_l == spc:
+      dst_file.close()
+      pbar.update(1)
+
+      dst_file = open(f'{src}.{SPLITTED_CHUNKS_PREFIX}{chunk_index + 1}', 'wb')
+
+      cur_l = 0
+      chunk_index += 1
+
+    if cnk is not None:
+      cnk_l = len(cnk)
+      if cur_l < spc:
+        if cur_l + cnk_l > spc:
+          dst_file.write(cnk[:spc - cur_l])
+          dst_file.close()
+          pbar.update(1)
+
+          dst_file = open(f'{src}.{SPLITTED_CHUNKS_PREFIX}{chunk_index + 1}', 'wb')
+          dst_file.write(cnk[spc - cur_l:])
+
+          cur_l = cnk_l - (spc-cur_l)
+          chunk_index += 1
+        else:
+          dst_file.write(cnk)
+          cur_l += cnk_l
+
+  src_file.close()
+  if dst_file:
+    if dst_file.tell() == 0:
+      dst_file.close()
+      os.remove(dst_file.name)
+    else:
+      dst_file.close()
+      pbar.update(1)
+  pbar.close()
+  click.echo(f'splitted {src_file.name} into {chunk} chunks')
+
+
+@cli.command()
+@click.argument('src', nargs=1, type=click.Path(exists=True))
+@click.option('-c', '--chunk', type=int, help='number of chunks to output')
+@click.option('-s', '--size', type=str, help='size of each chunk')
+def split(src: str, chunk: int, size: str):
+  """ Split the file into several chunks by specifying EITHER:\n
+  - number of chunks with --chunk flag\n
+  - size of each chunk with --size flag, and the number of chunks is calculated accordingly, i.e. 5kb, 10mb, 1gb
+
+  SRC is the filepath.
+  """
+  split_(src, chunk, size)
+
+
+def merge_(src: str, remove: bool):
+  dirpath = get_path(src)
+
+  all_chunks = list(dirpath.glob(SPLITTED_CHUNKS_PATTERN))
+  if not all_chunks:
+    click.echo('no splitted file chunks found')
+    return
+
+  files = defaultdict(list)
+  for c in all_chunks:
+    name = c.stem
+    files[name].append(c)
+
+  file_names = list(files.keys())
+  if len(file_names) >= 2:
+    question = f'found {len(file_names)} splitted file chunks, choose one to proceed:\n'
+    for i, v in enumerate(file_names):
+      question += f'{i+1} - {v}\n'
+    question += 'your answer'
+
+    file_choice = click.prompt(question, type=int)
+    while (file_choice > len(file_names)) or (file_choice < 1):
+      file_choice = click.prompt('incorrect input, please try again', type=int)
+    file = file_names[file_choice - 1]
+  else:
+    file = file_names[0]
+
+  chunks = sorted(files[file], key=lambda x: int(x.suffix.split(SPLITTED_CHUNKS_PREFIX)[1]))
+  pbar = tqdm.tqdm(total=len(chunks))
+
+  dst = chunks[0].parent / chunks[0].stem
+  if dst.is_file():
+    filename = chunks[0].stem.split('.')[0]
+    extension = chunks[0].stem.split('.')[1]
+    dst = chunks[0].parent / f'{filename}_copy.{extension}'
+
+  dst_file = open(dst, 'wb')
+  for c in chunks:
+    p_size = os.stat(c).st_size
+    with open(c, 'rb') as f:
+      for cnk in read_in_chunks(f, min(p_size, MAX_BUFFER_SIZE)):
+        if cnk:
+          dst_file.write(cnk)
+    pbar.update(1)
+
+  dst_file.close()
+  pbar.close()
+  click.echo(f'merged splitted file chunks to {dst}')
+
+  if remove:
+    for c in chunks:
+      os.remove(c)
+    click.echo('removed splitted file chunks')
+
+
+@cli.command()
+@click.argument('src', nargs=1, type=click.Path(exists=True))
+@click.option('-r', '--remove', default=False, is_flag=True, help='remove splitted file chunks after merge')
+def merge(src: str, remove: bool):
+  """ Merge NFS splitted file chunks into one.
+
+  NFS splitted file chunks can be identified with '.c1', '.c2' (etc.) appended to the end of original file's name (path).
+
+  If multiple files that are splitted are found, user can choose which one to merge.
+
+  If the original file exists under the same directory, a new file with '_copy' appended to the filename will be created.
+
+  SRC is the directory path that contains (parent to) splitted file chunks.
+  """
+  merge_(src, remove)
+
+
+if __name__ == '__main__':
+  # pylint: disable=no-value-for-parameter
+  cli()
```

